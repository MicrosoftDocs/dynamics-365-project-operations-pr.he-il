---
title: ביצועים של ממשקי API של לוחות זמנים
description: נושא זה מספק מידע על מדדי הביצועים של ממשקי ה-API של לוח הזמנים של הפרויקט ומזהה שיטות עבודה מומלצות לשימוש מיטבי.
author: ruhercul
ms.date: 11/03/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 3c14d27c561a86cd359cbdcbb448ae764dd3d90e
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8593843"
---
# <a name="project-schedule-api-performance"></a>ביצועים של ממשקי API של לוחות זמנים

_**חל על:** Project Operations עבור תרחישים מבוססי-משאב/לא במלאי, פריסה קלה - עסקה להנפקת חשבונית פרופורמה, Project for the web_

נושא זה מספק מידע על מדדי הביצועים של ממשקי ה-API של לוח הזמנים של הפרויקט ומזהה את שיטות העבודה המומלצות לשימוש מיטבי.

## <a name="project-scheduling-service"></a>שירות תזמון פרויקטים
שירות תזמון הפרויקטים הוא שירות מרובה דיירים שפועל ב- Microsoft Azure. הוא נועד לשפר את האינטראקציה על ידי יצירת חוויה מהירה וזורמת כאשר משתמשים עובדים על פרויקטים. שיפור זה מושג על ידי קבלת בקשות שינוי, עיבודן ולאחר מכן החזרת התוצאה מידית. השירות ממשיך באופן אסינכרוני את Dataverse ואינו חוסם משתמשים מלבצע פעולות אחרות.

ממשקי ה-API של לוח הזמנים של הפרויקט מסתמכים על שירות תזמון הפרויקטים כדי להפעיל בקשות המתוארות בפירוט רב יותר בסעיפים מאוחרים יותר של נושא זה.

ממשקי ה-API של לוח הזמנים של הפרויקט נועדו לעבוד עם הישויות הבאות של מבנה התפלגות עבודה (WBS):

  - פרויקט
  - משימת הפרוייקט
  - ‏‫יחס תלות במשימת פרוייקט
  - חבר צוות פרוייקט
  - הקצאת משאבים
  
גם שדות שמוגדרים במוצר המקורי וגם שדות מותאמים אישית נתמכים. אלא אם צוין אחרת, כל הפעולות הנפוצות נתמכות, כגון יצירה, עדכון ומחיקה. למידע נוסף, ראה [השתמש בממשקי API של תזמון פרויקטים כדי לבצע פעולות עם ישויות תזמון](schedule-api-preview.md).

כחלק מממשקי ה-API של לוח הזמנים של הפרויקט, נוסף דפוס של יחידת עבודה. דפוס זה ידוע בתור OperationSet, וניתן להשתמש בו כאשר רוצים לעבד מספר בקשות בעסקה אחת.

האיור הבא מציג את הזרימה ששותף יחווה כאשר נעשה שימוש בתכונה זו.

![Dataverse ושרימה של שירות תזמון פרויקטים.](./media/dataverse-project-scheduling-service-flow.png)

**שלב 1**: לקוח מבצע קריאת API לנקודת קצה של Open Data Protocol ‏(OData) ב- Dataverse כדי ליצור OperationSet.

**שלב 2**: לאחר יצירת ה-OperationSet החדש מוחזר הערך **OperationSetId**.

**שלב 3**: הלקוח משתמש בערך **OperationSetId** כדי לבצע בקשה נוספת ל-API של לוח זמנים של פרויקט. התוצאה היא בקשה ליצירה, עדכון או מחיקה של ישות תזמון. כאשר בקשה זו מתבצעת, מתבצע אימות מטא נתונים. אם האימות נכשל, הבקשה תסתיים ומוחזרת שגיאה.

**שלבים 4א-4ג**: שלבים אלה מייצגים את שלב הקבלה. הלקוח מתקשר אל **ExecuteOperationSetV1** API, ששולח את כל השינויים לשירות תזמון הפרויקטים באצווה אחת. שירות תזמון הפרויקט מפעיל אימותים משלו בבקשות באצווה. כל כשל אימות מבטל את האצווה ומחזיר חריגה למתקשר. אם האצווה התקבלה בהצלחה על ידי שירות תזמון הפרויקט, המצב OperationSet מתעדכן כך שישקף את העובדה ש- OperationSet מעובד על ידי שירות תזמון הפרויקט.

**שלב 5**: שלב זה מייצג את השלב PERSIST. שירות תזמון הפרויקט כותב את האצווה באופן אסינכרוני ל- Dataverse בעסקה. אם פעולת הכתיבה הצליחה, ה- OperationSet מסומן כ- **הושלם**. כל שגיאה מחזירה את העסקה ואת האצווה, ו- OperationSet מסומן כ- **נכשל**.

## <a name="performance-methodology"></a>מתודולוגיית ביצועים
זמן הביצוע מוגדר כזמן מהקריאה ל- **ExecuteOperationSetV1** API עד ששירות תזמון הפרויקטים סיים לכתוב ל- Dataverse. כל הפעולות פועלות ביחד 2,200 פעמים, ומדידות זמן הביצוע של P99 מדווחות. פעולות של רשומות בודדות ופעולות בכמות גדולה נמדדות.

עבור פעולה של רשומה אחת, ה- OperationSet מכיל בקשה אחת. עבור פעולות בכמות גדולה, הוא מכיל 20, 50 או 100 בקשות. כל גודל באצווה מדווח בנפרד.

הפעולות פועלות על פריסת UR 15 Project Operations Lite בצפון אמריקה.

## <a name="results"></a>תוצאות
### <a name="create-operations"></a>צור פעולות
#### <a name="single-record-create-operations"></a>פעולות יצירת רשומה אחת
הטבלה הבאה מציגה את זמני הביצוע ליצירת רשומה בודדת. הזמנים בשניות.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax" rowspan="2">סוג&nbsp;&nbsp;&nbsp;רשומה</th>
    <th class="tg-0lax" colspan="2">זמן</th>
  </tr>
  <tr>
    <th class="tg-0lax">שדות נדרשים</th>
    <th class="tg-0lax">כל השדות נתמכים</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">פרויקט</td>
    <td class="tg-0lax">2.5</td>
    <td class="tg-0lax">3.78</td>
  </tr>
  <tr>
    <td class="tg-0lax">משימה</td>
    <td class="tg-0lax">8.82</td>
    <td class="tg-0lax">9.34</td>
  </tr>
  <tr>
    <td class="tg-0lax">הקצאה</td>
    <td class="tg-0lax">9.19</td>
    <td class="tg-0lax">9.19</td>
  </tr>
  <tr>
    <td class="tg-0lax">חבר צוות</td>
    <td class="tg-0lax">0.84</td>
    <td class="tg-0lax">4.2</td>
  </tr>
  <tr>
    <td class="tg-0lax">יחס תלות</td>
    <td class="tg-0lax">8.84</td>
    <td class="tg-0lax">8.84</td>
  </tr>
</tbody>
</table>

#### <a name="bulk-create-operations"></a>פעולות יצירה בצובר
הטבלה הבאה מציגה את זמני הביצוע ליצירת כמה רשומות. באופן ספציפי, Microsoft מדדה את זמני הביצוע ליצירת 20, 50 ו-100 רשומות ב- OperationSet יחיד. הזמנים בשניות.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax" rowspan="3">סוג&nbsp;&nbsp;&nbsp;רשומה</th>
    <th class="tg-0lax" colspan="6">זמן</th>
  </tr>
  <tr>
    <th class="tg-0lax" colspan="2">20 רשומות</th>
    <th class="tg-0lax" colspan="2">50 רשומות</th>
    <th class="tg-0lax" colspan="2">100 רשומות</th>
  </tr>
  <tr>
    <th class="tg-0lax">שדות נדרשים</th>
    <th class="tg-0lax">כל השדות נתמכים</th>
    <th class="tg-0lax">שדות נדרשים</th>
    <th class="tg-0lax">כל השדות נתמכים</th>
    <th class="tg-0lax">שדות נדרשים</th>
    <th class="tg-0lax">כל השדות נתמכים</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">משימה</td>
    <td class="tg-0lax">19.92</td>
    <td class="tg-0lax">38.35</td>
    <td class="tg-0lax">36.67</td>
    <td class="tg-0lax">99.13</td>
    <td class="tg-0lax">116.77</td>
    <td class="tg-0lax">174.06</td>
  </tr>
  <tr>
    <td class="tg-0lax">הקצאה</td>
    <td class="tg-0lax">13.94</td>
    <td class="tg-0lax">13.94</td>
    <td class="tg-0lax">43.95</td>
    <td class="tg-0lax">43.95</td>
    <td class="tg-0lax">69.38</td>
    <td class="tg-0lax">69.38</td>
  </tr>
  <tr>
    <td class="tg-0lax">יחס תלות</td>
    <td class="tg-0lax">30.04</td>
    <td class="tg-0lax">30.04</td>
    <td class="tg-0lax">77.82</td>
    <td class="tg-0lax">77.82</td>
    <td class="tg-0lax">176.89</td>
    <td class="tg-0lax">176.89</td>
  </tr>
</tbody>
</table>

> [!NOTE] 
> יצירת פעולות בכמות גדולה בישויות **פרוייקט** ו- **חבר צוות** אינן נכללות בטבלה זו, מכיוון שזמן הריצה עבור פעולות אלו דומה לזמן הריצה כאשר ה-API ליצירת רשומה בודדת נקרא מספר פעמים. ממשקי API אלה מופעלים באופן מיידי ב- Dataverse.

האיור הבא מציג איור של זמני הביצוע עבור הישויות **משימה**, **הקצאה** ו- **תלות** כאשר נוצרות 20, 50 ו-100 רשומות ומשתמשים בכל השדות הנתמכים.

![צור גרף זמן ביצוע לרשומה.](./media/create-record-execution-time.png)

### <a name="update-operations"></a>עדכן פעולות
#### <a name="single-record-update-operations"></a>פעולות עדכון רשומה אחת
הטבלה הבאה מציגה את זמני הביצוע לעדכון רשומה בודדת. הזמנים בשניות.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax" rowspan="2">סוג&nbsp;&nbsp;&nbsp;רשומה</th>
    <th class="tg-0lax" colspan="2">זמן</th>
  </tr>
  <tr>
    <th class="tg-0lax">שדות נדרשים </th>
    <th class="tg-0lax">כל השדות נתמכים</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">פרויקט</td>
    <td class="tg-0lax">9.53</td>
    <td class="tg-0lax">13.91</td>
  </tr>
  <tr>
    <td class="tg-0lax">משימה</td>
    <td class="tg-0lax">8.82</td>
    <td class="tg-0lax">9.91</td>
  </tr>
  <tr>
    <td class="tg-0lax">חבר צוות</td>
    <td class="tg-0lax">9</td>
    <td class="tg-0lax">8.96</td>
  </tr>
</tbody>
</table>

> [!NOTE]
> עדכון פעולות בישויות **הקצאות משאבים** ו- **יחס תלות במשימת פרוייקט** אינו נתמך.

#### <a name="bulk-update-operations"></a>פעולות עדכון בצובר
הטבלה הבאה מציגה את זמני הביצוע לעדכון כמה רשומות. באופן ספציפי, Microsoft מדדה את זמני הביצוע לעדכון 20, 50 ו-100 רשומות ב- OperationSet יחיד. הזמנים בשניות.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax" rowspan="3">סוג&nbsp;&nbsp;&nbsp;רשומה</th>
    <th class="tg-0lax" colspan="6">זמן</th>
  </tr>
  <tr>
    <th class="tg-0lax" colspan="2">20 רשומות</th>
    <th class="tg-0lax" colspan="2">50 רשומות</th>
    <th class="tg-0lax" colspan="2">100 רשומות</th>
  </tr>
  <tr>
    <th class="tg-0lax">שדות נדרשים</th>
    <th class="tg-0lax">כל השדות נתמכים</th>
    <th class="tg-0lax">שדות נדרשים</th>
    <th class="tg-0lax">כל השדות נתמכים</th>
    <th class="tg-0lax">שדות נדרשים</th>
    <th class="tg-0lax">כל השדות נתמכים</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">משימה</td>
    <td class="tg-0lax">8.91</td>
    <td class="tg-0lax">38.71</td>
    <td class="tg-0lax">20.92</td>
    <td class="tg-0lax">87.13</td>
    <td class="tg-0lax">36.68</td>
    <td class="tg-0lax">190.34</td>
  </tr>
  <tr>
    <td class="tg-0lax">חבר צוות</td>
    <td class="tg-0lax">20.52</td>
    <td class="tg-0lax">26.06</td>
    <td class="tg-0lax">41.93</td>
    <td class="tg-0lax">44.51</td>
    <td class="tg-0lax">38.63</td>
    <td class="tg-0lax">66.53</td>
  </tr>
</tbody>
</table>

> [!NOTE]
> עדכון פעולות בישויות **הקצאות משאבים** ו- **יחס תלות במשימת פרוייקט** אינו נתמך.

האיור הבא מציג איור של זמני הביצוע עבור הישויות משימה וחבר צוות כאשר מעדכנים 20, 50 ו-100 רשומות ומשתמשים בכל השדות הנתמכים.

![עדכן גרף זמן ביצוע לרשומה.](./media/update-record-execution-time.png)

### <a name="delete-operations"></a>מחק פעולות
#### <a name="single-record-delete-operations"></a>פעולות מחיקה של רשומה אחת
הטבלה הבאה מציגה את זמני הביצוע למחיקת רשומה בודדת. הזמנים בשניות.

| סוג רשומה‏ | זמן  |
|-------------|-------|
| משימה        | 20.12 |
| הקצאה  | 10.86 |
| חבר צוות | 12.52 |
| יחס תלות  | 20.89 |

> [!NOTE]
> מחיקת פעולות בישויות **פרוייקט** אינה נתמכת.

#### <a name="bulk-delete-operations"></a>פעולות מחיקה בצובר
הטבלה הבאה מציגה את זמני הביצוע למחיקה של כמה רשומות. באופן ספציפי, Microsoft מדדה את זמני הביצוע למחיקת 20, 50 ו-100 רשומות ב- OperationSet יחיד. הזמנים בשניות.

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax" rowspan="2">סוג&nbsp;&nbsp;&nbsp;רשומה</th>
    <th class="tg-0lax" colspan="3">זמן</th>
  </tr>
  <tr>
    <th class="tg-0lax">20 רשומות</th>
    <th class="tg-0lax">50 רשומות</th>
    <th class="tg-0lax">100 רשומות</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">משימה</td>
    <td class="tg-0lax">20.91</td>
    <td class="tg-0lax">67.43</td>
    <td class="tg-0lax">71.96</td>
  </tr>
  <tr>
    <td class="tg-0lax">הקצאה</td>
    <td class="tg-0lax">11.75</td>
    <td class="tg-0lax">25.79</td>
    <td class="tg-0lax">47.66</td>
  </tr>
  <tr>
    <td class="tg-0lax">חבר צוות</td>
    <td class="tg-0lax">9.78</td>
    <td class="tg-0lax">39.73</td>
    <td class="tg-0lax">24.33</td>
  </tr>
  <tr>
    <td class="tg-0lax">יחס תלות</td>
    <td class="tg-0lax">24.61</td>
    <td class="tg-0lax">54.9</td>
    <td class="tg-0lax">109.16</td>
  </tr>
</tbody>
</table>

> [!NOTE]
> מחיקת פעולות בישויות **פרוייקט** אינה נתמכת.

האיור הבא מציג איור של זמני הביצוע עבור הישויות **משימה**, **הקצאה**, **חבר צוות** ו- **יחס תלות** כאשר מוחקים 20, 50 ו-100 רשומות ומשתמשים.

![מחק גרף זמן ביצוע לרשומה.](./media/delete-record-execution-time.png)

## <a name="observations"></a>תצפיות
עבור כל פעולה על רשומה, ל- API **ExecuteOperationSet** לוקח בערך 800 מילישניות לשלוח בקשה לשירות תזמון הפרויקטים. לאחר מכן לוקח לשירות תזמון הפרויקטים כחמש שניות לעבד את המטען ולהתקשר אל Dataverse. שאר זמן הביצוע מושקע בהפעלת לוגיקה עסקית וכתיבת נתונים למסד הנתונים ב- Dataverse.

כאשר נוצרות, מעודכנות או נמחקות 100 רשומות, ל-API **ExecuteOperationSet** לוקח בערך שלוש שניות לשלוח את הבקשה לשירות תזמון הפרויקטים. לאחר מכן לוקח לשירות תזמון הפרויקטים כחמש שניות לעבד את הבקשות ולהתקשר אל Dataverse. פעולות בצובר חייבות לשלם **מס שירות תזמון פרויקטים** פעם אחת, עבור כל הרשומות ב- OperationSet. לכן, לפעולות בצובר יש זמן ביצוע ממוצע נמוך משמעותית מפעולות של רשומה בודדת.

## <a name="scenarios"></a>תרחישים
הטבלה הבאה מציגה את זמני הביצוע שבהם משתמשים ב-API של לוח הזמנים של הפרויקט כדי לבצע תרחישים ספציפיים. הזמנים בשניות.

| תרחיש                                                                   | זמן  |
|----------------------------------------------------------------------------|-------|
| צור פרויקט הכולל 40 משימות.                                      | 36.01 |
| צור פרויקט שכולל 40 משימות ו- 20 יחסי תלות.                  | 38.11 |
| צור פרויקט שכולל 40 משימות ו- 30 הקצאות.                   | 60.17 |
| צור פרויקט שכולל 40 משימות, 20 יחסי תלות ו- 30 הקצאות. | 60.27 |

## <a name="best-practices"></a>שיטות עבודה מומלצות
בהתבסס על תוצאות התרחיש הקודם, ממשקי ה-API מתפקדים טוב יותר בתנאים הבאים:

  - קבץ כמה שיותר פעולות ביחד. זמן הריצה הממוצע עבור פעולות בצובר טוב יותר מזמן הריצה הממוצע עבור פעולות של רשומה בודדת. ככל שמספר פעולות OperationSets בשימוש קטן יותר, כך זמן הביצוע הממוצע יהיה מהיר יותר.
  - הגדר רק את התכונות המינימליות הנדרשות כדי לבצע את התרחיש שלך. כדאי להיות סלקטיבי לגבי סוגי השדות שאינם נדרשים הכלולים בבקשת OperationSet. שדות המכילים מפתחות זרים או שדות אוסף ישפיעו לרעה על הביצועים.
