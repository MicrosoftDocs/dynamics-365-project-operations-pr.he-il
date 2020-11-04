---
title: תרחישים מרובי מטבעות (גירסה ‎3.x)
description: נושא זה מספק מידע אודות תרחישים מרובי מטבעות.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 12/26/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 7be029eeca3129d30f4bec1bf9b180a0a5122a86
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077418"
---
# <a name="multiple-currency-scenarios"></a>תרחישים מרובי מטבעות

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Microsoft Dynamics 365 כולל שני מושגים של מטבעות:

- **מטבע עסקה** - המטבע שבו מתבצעת עסקה. 
- **מטבע בסיס** - המטבע של מופע Dynamics 365. מטבע זה מוגדר כאשר מופע של Dynamics 365 מוקצה. אין אפשרות לשנות אותו.

לדוגמה, Contoso US מכרה 100 חולצות טי ללקוח בבריטניה תמורת 15 ליש"ט (GBP) לכל אחת. הטבלה הבאה מציגה את אופן תיעוד העסקה בישות 'מוצר הזמנה'.

| מוצר | כמות | מחיר ליחידה | מטבע | סכום | שער חליפין | מחיר ליחידה (בסיס)| סכום (בסיס)|
|---------|----------|----------------|----------|--------|---------------|----------------------|--------------|
| חולצת טי | 100      | 15             | GBP      | 1500   | 0.94          | $17.25               | $1,725       |

העמודה **מטבע** מציגה את מטבע העסקה, שהוא המטבע שבו התבצעה המכירה. העמודה **שער חליפין** היא שער החליפין בין מטבע העסקה למטבע הבסיס. ‏‏מטבע הבסיס הוא דולר אמריקני (USD). מטבע בסיס זה הוגדר כאשר המופע של Dynamics 365 הוקצה.
כפי שמראה הטבלה, כל עסקה מתועדת הן במטבע העסקה והן במטבע הבסיס. Dynamics 365 משתמש בשער החליפין של המטבע כדי לחשב את סכומי מטבע הבסיס.

## <a name="project-service-automation-extensions"></a>הרחבות של Project Service Automation

Dynamics 365 Project Service Automation משפיע על מטבע העסקה, משום שלעסקאות יש בדרך כלל שני היבטים: עלות ומכירות.

הישויות הבאות נחשבות לעסקאות:

- פרטים בשורת הצעת מחיר
- פרט סעיף חוזה של פרוייקט
- שורת הערכה
- שורת יומן
- פרט שורה בחשבונית
- בפועל

בכל אחת מישויות אלה, קיימת רשומה המייצגת את סכום העלות או את סכום המכירה. בדומה לכל ישות Dynamics 365 הכוללת שדה **סכום** , כל רשומה כוללת סכומים הן במטבע העסקה והן במטבע הבסיס. 

PSA מרחיב את המושג של מטבע עסקה עבור העלות והמכירות באופנים הבאים:

- מטבע העסקה של העלות עבור עסקאות זמן מגיע תמיד מהמטבע של היחידה הארגונית שמנהלת את הפרוייקט או שהפרוייקט נמצא בבעלותה. יחידה ארגונית זו מוכרת כיחידת החוזה.
- מטבע העסקה של המכירות עבור עסקאות זמן והוצאה מגיע תמיד מהמטבע של חוזה הפרוייקט.
- מטבע העסקה של העלות עבור הוצאות מגיע מהמטבע שבו נוצר ערך ההוצאות.

## <a name="multiple-currency-scenario"></a>תרחיש מרובה מטבעות

סעיף זה מתאר דוגמה לפרוייקט ש- Contoso UK מספקת עבור לקוח בשם Fabrikam, Japan. להלן אופן ההגדרה של התרחיש:

1. ליש"ט וין יפני (JPY) מוגדרים תחת **הגדרות** \> **ניהולע סקי** \> **מטבעות**. 
2. חשבון לקוח בשם **Fabrikam - Japan** מוגדר, ו- JPY נבחר כמטבע בתיק הלקוח.
3. יחידה ארגונית בשם **Contoso UK** מוגדרת ו- GBP נבחר כמטבע.
4. נוצר חוזה פרוייקט שבו **Contoso UK** מצוינת כיחידת החוזה ו- **Fabrikam – Japan** מצוינת כלקוח.
5. סעיפי חוזה של פרוייקט נוצרים, בהתבסס על הסדרי החיוב עבור מחלקות העסקה השונות בפרוייקט, כגון חיוב עבור זמן לעומת חיוב עבור הוצאות.
6. נוצר פרוייקט שבו **Contoso UK** מצוינת כיחידת החוזה. פרוייקט זה נוצר וממופה לסעיפי החוזה של הפרוייקט.


במהלך הערכה המשתמשת בפרט של שורת הצעת המחיר, פרט סעיף החוזה של הפרוייקט או בשורת ההערכה של לוח הזמנים, שתי רשומות נוצרות תמיד בישות. רשומה אחת היא עבור עלות, והרשומה השנייה היא עבור מכירות.

- כברירת מחדל, מטבע העסקה ברשומת העלות מוגדר למטבע של יחידת החוזה של הפרוייקט. בדוגמה זו, המטבע הוא GBP.
- כברירת מחדל, מטבע העסקה ברשומת המכירות מוגדר למטבע של חוזה הפרוייקט. בדוגמה זו, המטבע הוא JPY.

כאשר הנתונים בפועל נוצרים עבור זמן באמצעות ערך הזמן או שורת היומן, אופן הפעולה הבא מתרחש:

- כברירת מחדל, מטבע העסקה ברשומת העלות מוגדר למטבע של יחידת החוזה של הפרוייקט.
- כברירת מחדל, מטבע העסקה ברשומת המכירות מוגדר למטבע של חוזה הפרוייקט.

כאשר הנתונים בפועל נוצרים עבור הוצאות על-ידי ערך ההוצאה או שורת היומן, אופן הפעולה הבא מתרחש:

- באפשרותך לתעד את סכום ההוצאה בכל מטבע. בחר את המטבע על-ידי שימוש בבורר המטבעות בדף **ערך הוצאה** או בדף **שורת יומן**. כברירת מחדל, מטבע העסקה עבור רשומת העלות מוגדר למטבע בערך ההוצאה. 
- כברירת מחדל, מטבע העסקה עבור רשומת מכירות הוא המטבע של חוזה הפרוייקט. כדי להגדיר מטבע זה, המערכת ממירה תחילה את סכום העסקה במטבע שהמשתמש הזין למטבע הבסיס. לאחר מכן היא ממירה את הסכום למטבע של חוזה הפרוייקט. 

### <a name="computing-roll-ups-when-project-actuals-are-recorded-in-multiple-transaction-currencies"></a>חישוב פעולות סיכום כאשר הנתונים בפועל של הפרוייקט מתועדים במטבעות עסקה מרובים

Dynamics 365 מטפל באופן אוטומטי בפעולות סיכום של סכומים במטבעות שונים. הנה דוגמה.

| מחלקת עסקאות | סוג עסקה| Date   | משאב | קטגוריית עסקה | כמות | מחיר יחידה | סכום      | שער חליפין | סכום בבסיס |
|-------------------|------------------|--------|----------|----------------------|----------|--------------|-------------|---------------|----------------|
| Time              | מכירות שלא חויבו   | 14 ביוני | שי  |                      | 8 שעות    | 20,00‎0 JPY    | 160,000‎0 JPY | 123           | 1,300.8‎1 USD    |
| Time              | מכירות שלא חויבו   | 15 ביוני | שי  |                      | 8 שעות    | 20,00‎0 JPY    | 160,000‎0 JPY | 123           | 1,300.8‎1 USD    |
| הוצאות           | מכירות שלא חויבו   | 16 ביוני | שי  | בתי מלון                | ‎1 ea     | 25‎0 EUR      | 25‎0 EUR     | 0.94          | 265.95‎ USD     |
| הוצאות           | מכירות שלא חויבו   | 17 ביוני | שי  | השכרת רכב           | ‎1 ea     | 150‎ EUR      | 150‎ EUR     | 0.94          | 159.57‎ USD     |

כדי לחשב את ערך המכירות הכולל שלא חויב בפרוייקט, באפשרותך ליצור שדה סיכום עבור השדה **סכום** בכל הנתונים בפועל הקשורים של המכירות שלא חויבו. שדה הסיכום הוא מבנה של Dynamics 365 המאפשר נוסחאות מהירות ברשומות קשורות.