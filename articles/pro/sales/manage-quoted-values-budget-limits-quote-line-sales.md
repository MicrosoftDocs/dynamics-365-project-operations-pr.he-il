---
title: מבט כולל על שורות הצעות מחיר מבוססות פרוייקט - לייט
description: נושא זה מספק מידע על עבודה עם שורות הצעות מחיר המבוססות פרויקט לעבודת פרויקט. (Pro)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 4865c06691fba09eacf5fe6449adfaf542444520
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5272974"
---
# <a name="project-based-quote-lines-overview---lite"></a>מבט כולל על שורות הצעות מחיר מבוססות פרוייקט - לייט

_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_

שורות הצעת מחיר מבוססות פרויקט נועדו לעזור להעריך את עבודת הפרויקט עבור התקשרות. המבנה של שורת הצעות מחיר מבוסס פרויקט מורחב להערכות פרויקט באמצעות המושגים הבאים:

- שיטת חיוב
- מיפוי פרויקטים ומשימות
- סווגי עסקה כלולים
- מגבלת 'אין לחרוג'
- הגדרת יכולת חיוב
- הערכה באמצעות פרטי קו הצעת מחיר
- לקוחות של שורת הצעת מחיר

הטבלה הבאה מספקת מידע אודות השדות המופיעים בכרטיסיה **כללי** של שורת הצעת מחיר מבוססת פרויקט. שדות אלה מסייעים בהכנת הבסיס לביצוע הערכה מפורטת ויסודיות לעבודת הפרויקט.

| **שדה** | **תיאור** | **השפעה במורד הזרם** |
| --- | --- | --- |
| שם | שם שורת הצעת המחיר אשר אמורה לעזור לך לזהות את המרכיב המובדל של הצעת המחיר שעבורה מתבצעת הערכה. | מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| שיטת חיוב | כשנוצרת הצעת מחיר מהזדמנות, ערך זה מועתק מהשדה התואם שבשורת הזדמנות. תחום זה כולל את שני המודלים העיקריים לחוזים, שנתמכים על ידי Dynamics 365 Project Operations:</br>- מחיר קבוע</br>- זמן וחומרים.| ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| פרויקט | השתמש בשדה אופציונלי זה כדי לזהות את הפרויקט שישמש להגשת העבודה בהתקשרות זו. כאשר פרויקט ממופה לשורת הצעת מחיר, זה עוזר בהגדרת משימות הניתנות לחיוב וגם בכנסת הערכה מבוססת פרויקט לשורת הצעת המחיר, כפרטים בשורת הצעת מחיר. כאשר פרויקט אינו ממופה לשורת הצעת מחיר מבוססת פרויקט, יש ליצור את ההערכה באופן ידני על ידי יצירת כל פרט שבשורת הצעת המחיר. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.|
| משימות כלולות | הוא מציין אם שורת הצעת מחיר זו משמשת עבור כל משימות הפרויקט של הפרויקט שנבחר או עבור חלקן. שדהזה כולל את הערכים אפשריים הבאים:</br>- כל משימות הפרויקט</br>- משימות פרויקט נבחרות בלבד</br>ערך ריק בשדה זה שווה ערך לאפשרות **כל משימות הפרויקט**. | כשנבחרת האפשרות **משימות הפרויקט נבחרות בלבד**, אז בדף הפרויקט, הכרטיסיה **הגדרת חיוב משימות** מאפשרת לך לבחור משימות ספציפיות כדי לשייך אותן לשורת הצעת מחיר זו. ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| כלול זמן | דגל **כן**/**לא** מציין אם עסקאות זמן או עלויות עבודה בפרויקט שנבחר ייכללו בהערכה בשורת הצעת מחיר זו. הערך **לא** מציין שעסקאות זמן או עלויות עבודה לא ייכללו בהערכה בשורת הצעת מחיר זו. הערך **כן** מציין שעסקאות זמן או עלויות עבודה ייכללו בהערכה בשורת הצעת מחיר זו. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| כלול הוצאה | דגל **כן**/**לא** מציין אם עלויות ההוצאות בפרויקט שנבחר ייכללו בהערכה בשורת הצעת מחיר זו. הערך **לא** מציין שעלויות ההוצאות לא ייכללו בהערכה בשורת הצעת מחיר זו. הערך **כן** מציין שעלויות ההוצאות ייכללו בהערכה בשורת הצעת מחיר זו. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| כלול תשלום | דגל **כן**/**לא** מציין אם עמלות על הפרויקט שנבחר ייכללו בהערכה בשורת הצעת מחיר זו. הערך **לא** מציין שהעמלות לא ייכללו בהערכה בשורת הצעת מחיר זו. הערך **כן** מציין שהעמלות ייכללו בהערכה בשורת הצעת מחיר זו. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| הסכום של הצעת המחיר | זהו סכום הצעת המחיר שינתן ללקוח עבור כל העבודה החזויה בשורת הצעת מחיר מבוססת פרויקט זו. בהצעת מחיר שנוצרת מהזדמנות, ערך זה מועתק מהשדה **תקציב הלקוח** שבשורת הזדמנות. כשבשורת צעת מחיר מבוססת הפרויקט יש פרטי שורה, שדה זה נעול לעריכה ומסוכם מהסכום שנמצא בפרטים בשורת הצעת המחיר. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| מס משוער | זהו שדה הניתן לעריכה שהמשתמש יכול להוסיף בו את סכום המס המשוער בשורת הצעת המחיר. כשבשורת צעת מחיר מבוססת הפרויקט יש פרטי שורה, שדה זה נעול לעריכה ומסוכם מסכום המס שנמצא בפרטים בשורת הצעת המחיר. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| סכום הצעת המחיר, אחרי מס | שדה זה הוא סכום שורת הצעת המחיר לאחר מס והוא לקריאה בלבד. הסכום בשדה זה מחושב כ *סכום הצעת המחיר + מס*. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| מגבלת 'אין לחרוג' | שדה זה ניתן לעריכה והוא זמין רק בשורות הצעות מחיר מבוססות פרויקט עם שיטת חיוב של **זמן וחומרים**. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| תקציב הלקוח | שדה זה ניתן לעריכה ומועתק מהשדה התואם בשורת ההזדמנות אם הצעת המחיר נוצרה מהזדמנות. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a>כללי אימות עבור שדות בכרטיסיה 'כללי' של שורות הצעות מחיר מבוססות פרויקט

**כלל 1**: אם השדה **משימות כלולות** ריק, או אם הוא מוגדר ל **כל משימות הפרויקט**, פרויקט כלול בשורת הצעת המחיר.

**כלל 2**: אם השדה **משימות כלולות** ריק, או אם הוא מוגדר ל **כל משימות הפרויקט**, פרויקט וסיווג עסקאות מסוים יכולים להיכלל רק בשורת הצעת מחיר מבוססת פרויקט אחת של הצעת מחיר.

**כלל 3**: אם השדה **משימות כלולות** מוגדר ל **משימות הפרויקט נבחרות בלבד**, פרויקט וסיווג עסקאות מסוים יכולים להיכלל בשורת הצעת מחיר מבוססת פרויקט מרובות של הצעת מחיר.

**כלל 4**: אם להזדמנות יש הצעות מחיר מרובות, יכולות להיות שורות הצעות מחיר מהצעות מחיר שונות, שכולן מתייחסות לאותו פרויקט וכוללות את אותו סיווג עסקאות.

**כלל 5**: אם הצעות המחיר אינן שייכות לאותה הזדמנות, הן אינן יכולות לכלול את אותו פרויקט וסיווג עסקאות.

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p>
                    <strong>הזדמנות</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>הצעת מחיר</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>שורת הצעת מחיר</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>פרויקט</strong>
                </p>
            </td>
            <td width="90" valign="top">
                <p>
                    <strong>משימות כלולות</strong>
                </p>
            </td>
            <td width="48" valign="top">
                <p>
                    <strong>כלול זמן</strong>
                </p>
            </td>
            <td width="48" valign="top">
                <p>
                    <strong>כלול הוצאה</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>הכללה</strong>
                </p>
                <p>
                    <strong>תשלום</strong>
                </p>
            </td>
            <td width="54" valign="top">
                <p>
                    <strong>חוקי/לא חוקי</strong>
                </p>
            </td>
            <td width="308" valign="top">
                <p>
                    <strong>סיבה</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
ריק </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
לא חוקי </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
הפרת כלל מס' 2. זמן, הוצאות ועמלות בפרויקט P1 כלולים בשורות הצעות מחיר QL1 ו-QL2.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
ריק </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
ריק </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
לא חוקי </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
הפרת כלל מס' 2. זמן ועמלות בפרויקט P1 כלולים בשורות הצעות מחיר QL1 ו-QL2.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
ריק </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
ריק </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
חוקי </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
זמן ועמלות בפרויקט P1 כלולים ב-QL1.
הוצאות בפרויקט P1 כלולות ב-QL2.
אין חפיפה במה שנכלל בכל שורת הצעת מחיר והוא תקף.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
ריק </p>
            </td>
            <td width="48" valign="top">
                <p>
Yes </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
משימות נבחרות בלבד </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
לא חוקי </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
הפרת כלל מס' 2 שלעיל </p>
                <p>
ר1 כולל זמן, הוצאות ועמלות על קבוצת משנה של משימות בפרויקט P1.
                </p>
                <p>
QL2 כולל זמן, הוצאות ועמלות עבור כל הפרויקט P1 וחופף למה שנכלל ר1.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
ריק </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
משימות נבחרות בלבד </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
חוקי </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
לפי כלל מס' 3 לעיל, </p>
                <p>
ר1 כולל זמן, הוצאות ועמלות על קבוצת משנה של משימות בפרויקט P1.
                </p>
                <p>
QL2 כולל זמן, הוצאות ועמלות עבור קבוצת משנה של משימות בפרויקט P1.
                </p>
                <p>
האימות הנוסף היחיד הוא סביב קבוצת המשנה של המשימות ב-QL1 אשר שונה מקבוצת המשנה של המשימות ב-QL2. דבר זה מבטיח שלא יהיו חפיפות. פעולה זו מתבצעת על ידי המערכת כאשר משימות משויכות.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
משימות נבחרות בלבד </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
כל משימות הפרויקט או ריק </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="54" valign="top">
                <p>
חוקי </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
בהתבסס על כלל מס' 5, Q1 ו-Q2 הן שתי הצעות מחיר באותה הזדמנות, כך ששתיהן יכולות לשמש להערכת אותם רכיבי פרויקט.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ר2 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
כל משימות הפרויקט או ריק </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="54" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
כל משימות הפרויקט או ריק </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="54" valign="top">
                <p>
חוקי </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
בהתבסס על כלל מס' 4, Q1 ו-Q2 הן שתי הצעות מחיר עבור הזדמנויות שונות, כך שהן אינן יכולות לשמש להערכת אותם הרכיבים של אותו הפרויקט.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O2 </p>
            </td>
            <td width="41" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
כל משימות הפרויקט או ריק </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="48" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="54" valign="top">
                <p>
לא חוקי </p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]