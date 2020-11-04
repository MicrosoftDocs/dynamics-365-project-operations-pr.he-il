---
title: הפקת חשבונית ב- Project Service Automation
description: נושא זה מספק מידע על הפקת חשבוניות.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 08/03/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: f8107a660f9993c7b6a32d69047a81fb7e0abef8
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077372"
---
# <a name="invoicing-in-project-service-automation"></a>הפקת חשבונית ב- Project Service Automation

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

הפקת חשבונית ב- Dynamics 365 Project Service Automation היא דבר שימושי מכיוון שהיא מעניקה למנהלי פרויקטים רמת אישור שנייה לפני שהם יוצרים חשבוניות ללקוחות. רמת האישור הראשונה מסתיימת כאשר ערכי הזמן וההוצאות שמגישים חברי צוות הפרויקט מאושרים.

PSA אינו מיועד ליצור חשבוניות המוצגות ללקוח, מהסיבות הבאות:

- הוא לא מכיל מידע בנושא מס.
- הוא לא ממיר מטבעות אחרים למטבע בהפקת החשבונית באמצעות שערי חליפין שתצורתם נקבעה כראוי.
- הוא לא מעצב כראוי חשבוניות כך שניתן להדפיס אותן.

במקום זאת, באפשרותך להשתמש במערכת פיננסית או חשבונאית כדי ליצור חשבוניות ללקוח המשתמשות במידע מהצעות לחשבוניות שנוצרות ב- PSA.

## <a name="creating-project-invoices-in-psa"></a>יצירת חשבוניות פרויקט ב- PSA

ניתן ליצור חשבונית פרויקט אחת בכל פעם או בצובר. באפשרותך ליצור אותן באופן ידני או להגדיר אותן כך שייווצרו בהפעלות אוטומטיות.

### <a name="manually-create-project-invoices-in-psa"></a>יצירה ידנית של חשבוניות פרויקט ב- PSA

מדף הרשימה של **חוזי הפרויקט‬** , תוכל ליצור חשבוניות פרויקט בנפרד עבור כל חוזה פרויקט, או שתוכל ליצור חשבוניות בצובר עבור כמה חוזי פרויקטים.

בצע שלב זה כדי ליצור חשבונית עבור חוזה פרויקט ספציפי.

- בדף הרשימה של **חוזי הפרויקט** , פתח חוזה פרויקט ולאחר מכן בחר **צור חשבונית**.

    ![יצירת חשבוניות פרויקט עבור חוזה פרויקט ספציפי](media/CreateProjectInvoicesOneByOne.png)

    חשבונית נוצרת עבור כל העסקאות בחוזה הפרויקט שנבחר במצב **מוכן להגיש חשבונית‬**. עסקאות אלה כוללות מועד, הוצאות, אבני דרך וסעיפי חוזה מבוססי מוצר.

בצע את השלבים הבאים כדי ליצור חשבוניות בצובר.

1. בדף הרשימה של **חוזי הפרויקט** , בחר חוזה פרויקט אחד או יותר שעבורו תרצה ליצור חשבונות ולאחר מכן בחר **‏‫צור חשבוניות פרויקט**.

    ![יצירת חשבוניות פרויקט בצובר](media/CreateProjectInvoicesBulk.png)

    הודעת אזהרה מיידעת אותך שייתכן שיהיה עיכוב לפני יצירת חשבוניות. התהליך גם מוצג.

2. בחר **אישור** כדי לסגור את תיבת ההודעה.

    חשבונית נוצרת עבור כל העסקאות בסעיף חוזה שנמצא במצב **מוכן להגיש חשבונית‬**. עסקאות אלה כוללות מועד, הוצאות, אבני דרך וסעיפי חוזה מבוססי מוצר.

3. כדי להציג את החשבוניות שנוצרות, עבור אל **מכירות** \> **חיוב** \> **חשבוניות**. אתה תראה חשבונית אחת עבור כל חוזה פרויקט.

### <a name="set-up-automated-creation-of-project-invoices-in-psa"></a>הגדרת יצירה אוטומטית של חשבוניות פרויקט ב- PSA

בצע את השלבים הבאים כדי לקבוע את התצורה של הפעלת חשבונית אוטומטית ב- PSA.

1. עבור אל **Project Service** \> **הגדרות** \> **משימות אצווה**.
2. צור משימת אצווה ושנה את שמה ל- **צור חשבוניות ב- PSA**. שם משימת האצווה חייב לכלול את המונח "צור חשבוניות".
3. בשדה **סוג משימה** , בחר **ללא**. כברירת מחדל, האפשרות **תדירות יומית** והאפשרות **הוא פעיל** מוגדרות בתור **כן**.
4. בחר **הפעל זרימת עבודה**. בתיבת הדו-שיח **חיפוש רשומה** תראה שלוש זרימות עבודה:

    - ProcessRunCaller
    - ProcessRunner
    - UpdateRoleUtilization

5. בחר את **ProcessRunCaller** ולאחר מכן בחר **הוסף**.
6. בתיבת הדו-שיח הבאה, בחר **אישור**. אחרי זרימת עבודה **שינה** תופיע זרימת עבודה **תהליך**.

    תוכל גם לבחור את **ProcessRunner** בשלב 5. לאחר מכן, כשתבחר **אישור** , אחרי זרימת העבודה **תהליך** תופיע זרימת עבודה **שינה**.

זרימת העבודה **ProcessRunCaller** וזרימת העבודה **ProcessRunner** יוצרות חשבוניות. **ProcessRunCaller** קורא ל- **ProcessRunner**. **ProcessRunner** היא למעשה זרימת העבודה שיוצרת למעשה את החשבוניות. היא עוברת על כל סעיפי החוזה שעבורם יש ליצור חשבונית, והיא יוצרת שורות עבור שורות אלו. כדי לקבוע את סעיפי החוזה שעבורם יש ליצור חשבוניות, המשימה מחפשת תאריכים של הפעלת חשבוניות עבור סעיפי החוזה. אם לסעיפי חוזה השייכים לחוזה אחד יש תאריך הפעלת חשבונית זהה, העסקאות משולבות לחשבונית אחת הכוללת שתי שורות בחשבונית. אם אין עסקאות שעבורן יש ליצור חשבוניות, המשימה מדלגת על יצירת חשבונית.

לאחר שהפעלת **ProcessRunner** הסתיימה, היא קוראת ל- **ProcessRunCaller** , מספקת את שעת הסיום ונסגרת. לאחר מכן, **ProcessRunCaller** מפעילה שעון עצר הפועל במשך 24 שעות משעת הסיום שצוינה. כששעון העצר מפסיק, **ProcessRunCaller** נסגרת.

משימת תהליך האצווה ליצירת חשבוניות היא משימה חוזרת. אם תהליך אצווה זה מופעל פעמים רבות, נוצרים מופעים מרובים של המשימה וגורמים לשגיאות. לכן עליך להתחיל את תהליך האצווה רק פעם אחת, ועליך להפעיל אותו מחדש רק אם הוא מפסיק לפעול.

> [!NOTE]
> חשבוניות באצווה ב- Project Service Automation פועלות רק בסעיפי חוזה של פרויקט המוגדרים על פי לוחות זמנים של חשבוניות. אבני דרך חייבים להיות מוגדרים בסעיף חוזה בשיטת חיוב במחיר קבוע. סעיף חוזה בפרויקט בשיטת חיוב לפי זמן וחומר יצטרך הגדרה של לוח זמנים לחשבוניות המבוסס על תאריכים. מידע על הגדרת שכיחות חשבוניות בהקשר של פרויקט המבוסס על שורה בהצעת מחיר, ניתן בנושא [הצעת מחיר ו‏‫שורות הצעת המחיר](basic-quote-lines.md#invoice-schedule). כך גם בסעיף חוזה שמבוסס על פרויקטים.      
 
### <a name="edit-a-draft-psa-invoice"></a>עריכת טיוטת חשבונית של PSA

בעת יצירת טיוטה של חשבונית פרויקט, כל עסקאות המכירה שלא חויבו ושנוצרו בעת אישור ערכי הזמן וההוצאה יוכנסו לחשבונית. באפשרותך לבצע את ההתאמות הבאות כאשר החשבונית עדיין נמצאת בשלב טיוטה:

- מחיקה או עריכה של פרטי שורת חשבונית.
- עריכה והתאמה של הכמות וסוג החיוב.
- הוספה ישירה של זמן, הוצאה ועמלות כעסקאות בחשבונית. תוכל להשתמש בתכונה זו אם שורת החשבונית מופתה אל סעיף חוזה שמאפשר את סיווגי העסקאות האלו.

בחר **אשר** כדי לאשר חשבונית. פעולת האישור היא פעולה חד-סטרית. בעת בחירה באפשרות **אשר** , המערכת הופכת את החשבונית לקריאה בלבד ויוצרת נתונים בפועל של מכירות שחויבו מכל פירוט של שורת חשבונית עבור כל שורת חשבונית. אם הפירוט בשורת החשבונית מפנה לנתונים בפועל של מכירות שלא חויבו, המערכת גם מבטלת את הנתונים בפועל של מכירות שלא חויבו. (כל פירוט בשורת חשבונית שנוצר מערך זמן או הוצאה יפנה לנתונים בפועל של מכירות שלא חויבו.) מערכות שילוב של ספר ראשי יכולות להשתמש בביטול זה כדי לבטל עבודת פרויקט בתהליך (WIP) למטרה חשבונאית.

### <a name="correct-a-confirmed-psa-invoice"></a>תיקון חשבונית PSA מאושרת

ניתן לערוך חשבוניות PSA מאושרות (מתוקנות). בעת תיקון חשבונית מאושרת, נוצרת טיוטה חדשה לחשבונית תיקון. מכיוון שההנחה היא שברצונך לבטל את כל העסקאות והכמויות מהחשבונית המקורית, חשבונית תיקון זו כוללת את כל העסקאות מהחשבונית המקורית וכל הכמויות שבה הן 0 (אפס).

אם יש עסקאות כלשהן שלא דורשות תיקון, תוכל להסיר אותן מהטיוטה של חשבונית התיקון. אם ברצונך לבטל או להחזיר כמות חלקית בלבד, תוכל לערוך את השדה **כמות** בפירוט השורה. אם תפתח את הפירוט בשורת החשבונית, תוכל לראות את הכמות בחשבונית המקורית. לאחר מכן תוכל לערוך את הכמות בחשבונית הנוכחית כך שתהיה קטנה או גדולה מהכמות בחשבונית המקורית.

בעת אישור חשבונית תיקון, הנתונים בפועל המקוריים של המכירות שחויבו מבוטלים, ונוצרים נתונים בפועל חדשים למכירות שחויבו. אם הכמות הופחתה, ההפרש יגרום גם ליצירה של נתונים בפועל חדשים של מכירות שלא חויבו. לדוגמה, אם המכירה המקורית שחויבה היתה עבור שמונה שעות, ובפרטי שורת חשבונית התיקון יש כמות מופחתת של שש שעות, PSA יבטל את השורה המקורית של המכירות שחויבו ויצור שני נתונים בפועל חדשים:

- נתונים בפועל למכירות שחויבו עבור שש שעות.
- נתונים בפועל למכירות שלא חויבו עבור השעתיים שנותרו. ניתן לחייב עסקה זו במועד מאוחר יותר או לסמנה כלא ניתנת לחיוב, בהתאם למשא ומתן עם הלקוח.