---
title: מבט כולל על שורות הצעות מחיר מבוססות פרוייקט
description: נושא זה מספק מידע על עבודה עם שורות הצעות מחיר המבוססות פרויקט לעבודת פרויקט.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: b7076a4b9280472f8c30d0b58c3aa9b9bc86d651
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 07/07/2021
ms.locfileid: "6369872"
---
# <a name="project-based-quote-lines-overview"></a>מבט כולל על שורות הצעות מחיר מבוססות פרוייקט 

_**חל על:** פריסה קלה - עסקה עם חשבונית פרופורמה, Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

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
| שם | שם שורת הצעת המחיר המסייע לך לזהות את המרכיב הנפרד של הצעת המחיר המוערכת. | מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| שיטת חיוב | כשנוצרת הצעת מחיר מהזדמנות, ערך זה מועתק מהשדה התואם שבשורת הזדמנות. תחום זה כולל את שני המודלים העיקריים לחוזים, שנתמכים על ידי Dynamics 365 Project Operations:</br>- מחיר קבוע</br>- זמן וחומרים.| ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה. |
| פרויקט | השתמש בשדה אופציונלי זה כדי לזהות את הפרויקט שישמש להגשת העבודה בהתקשרות זו. כאשר פרויקט ממופה לשורת הצעת מחיר, זה עוזר בהגדרת משימות הניתנות לחיוב וגם בכנסת הערכה מבוססת פרויקט לשורת הצעת המחיר, כפרטים בשורת הצעת מחיר. כאשר פרויקט אינו ממופה לשורת הצעת מחיר מבוססת פרויקט, יש ליצור את ההערכה באופן ידני על ידי יצירת כל פרט שבשורת הצעת המחיר. | ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.|
| משימות כלולות | הוא מציין אם שורת הצעת מחיר זו משמשת עבור כל משימות הפרויקט של הפרויקט שנבחר או עבור חלקן. שדהזה כולל את הערכים אפשריים הבאים:</br>- כל משימות הפרויקט</br>- משימות פרויקט נבחרות בלבד</br>ערך ריק בשדה זה שווה ערך לאפשרות **כל משימות הפרויקט**. | בעת בחירה באפשרות **משימות פרויקט נבחרות בלבד** בדף הפרויקט, הכרטיסיה **הגדרת חיוב משימה** מאפשרת לך לבחור משימות ספציפיות כדי לשייך אותן לשורת הצעת מחיר זו. ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה. |
| כלול זמן | הערך **כן**/**לא** מציין אם עסקאות זמן או עלויות עבודה בפרויקט שנבחר ייכללו בהערכה לשורת הצעת מחיר זו. הערך **לא** מציין שעסקאות זמן או עלויות עבודה לא ייכללו בהערכה בשורת הצעת מחיר זו. הערך **כן** מציין שעסקאות זמן או עלויות עבודה ייכללו בהערכה בשורת הצעת מחיר זו. | ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה. |
| כלול הוצאה | הערך **כן**/**לא** מציין אם עלויות הוצאה בפרויקט שנבחר ייכללו בהערכה לשורת הצעת מחיר זו. הערך **לא** מציין שעלויות ההוצאות לא ייכללו בהערכה בשורת הצעת מחיר זו. הערך **כן** מציין שעלויות ההוצאות ייכללו בהערכה בשורת הצעת מחיר זו. | ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה. |
| כלול חומר | הערך **כן**/**לא** מציין אם עלויות חומר בפרויקט שנבחר ייכללו בהערכה לשורת הצעת מחיר זו. הערך **לא** מציין שעלויות חומר לא ייכללו בהערכה לשורת הצעת מחיר זו. הערך **כן** מציין שעלויות חומר ייכללו בהערכה לשורת הצעת מחיר זו. | ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה. |
| כלול תשלום | הערך **כן**/**לא** מציין אם עמלות בפרויקט שנבחר ייכללו בהערכה לשורת הצעת מחיר זו. הערך **לא** מציין שהעמלות לא ייכללו בהערכה בשורת הצעת מחיר זו. הערך **כן** מציין שהעמלות ייכללו בהערכה בשורת הצעת מחיר זו. | ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה. |
| הסכום של הצעת המחיר | זהו הסכום שיוצע כהצעת מחיר ללקוח עבור כל העבודה החזויה בשורת הצעת מחיר זו המבוססת על פרויקט. בהצעת מחיר שנוצרת מהזדמנות, ערך זה מועתק מהשדה **תקציב הלקוח** שבשורת הזדמנות. כשבשורת צעת מחיר מבוססת הפרויקט יש פרטי שורה, שדה זה נעול לעריכה ומסוכם מהסכום שנמצא בפרטים בשורת הצעת המחיר. | ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה. |
| מס משוער | זהו שדה הניתן לעריכה שהמשתמש יכול להוסיף בו את סכום המס המשוער בשורת הצעת המחיר. כשבשורת צעת מחיר מבוססת הפרויקט יש פרטי שורה, שדה זה נעול לעריכה ומסוכם מסכום המס שנמצא בפרטים בשורת הצעת המחיר. | ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה. |
| סכום הצעת המחיר, אחרי מס | שדה זה הוא סכום שורת הצעת המחיר לאחר מס והוא לקריאה בלבד. הסכום בשדה זה מחושב כ *סכום הצעת המחיר + מס*. | ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה. |
| מגבלת 'אין לחרוג' | שדה זה ניתן לעריכה והוא זמין רק בשורות הצעות מחיר מבוססות פרויקט עם שיטת חיוב של **זמן וחומרים**. | ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה. |
| תקציב הלקוח | שדה זה ניתן לעריכה ומועתק מהשדה התואם בשורת ההזדמנות אם הצעת המחיר נוצרה מהזדמנות. | ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה. |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a>כללי אימות עבור שדות בכרטיסיה 'כללי' של שורות הצעות מחיר מבוססות פרויקט

**כלל 1**: אם השדה **משימות כלולות** ריק, או אם הוא מוגדר ל **כל משימות הפרויקט**, פרויקט כלול בשורת הצעת המחיר.

**כלל 2**: אם השדה **משימות כלולות** ריק, או אם הוא מוגדר ל **כל משימות הפרויקט**, פרויקט וסיווג עסקאות מסוים יכולים להיכלל רק בשורת הצעת מחיר מבוססת פרויקט אחת של הצעת מחיר.

**כלל 3**: אם השדה **משימות כלולות** מוגדר ל **משימות הפרויקט נבחרות בלבד**, פרויקט וסיווג עסקאות מסוים יכולים להיכלל בשורת הצעת מחיר מבוססת פרויקט מרובות של הצעת מחיר.

**כלל 4**: אם להזדמנות יש הצעות מחיר מרובות, יכולות להיות שורות הצעות מחיר מהצעות מחיר שונות, שכולן מתייחסות לאותו פרויקט וכוללות את אותו סיווג עסקאות.

**כלל 5**: אם הצעות המחיר אינן שייכות לאותה הזדמנות, הן אינן יכולות לכלול את אותו פרויקט וסיווג עסקאות.

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="59" valign="top">
                <p>
                    <strong>הזדמנות</strong>
                </p>
            </td>
            <td width="39" valign="top">
                <p>
                    <strong>הצעת מחיר</strong>
                </p>
            </td>
            <td width="40" valign="top">
                <p>
                    <strong>שורת הצעת מחיר</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>פרויקט</strong>
                </p>
            </td>
            <td width="77" valign="top">
                <p>
                    <strong>משימות כלולות</strong>
                </p>
            </td>
            <td width="45" valign="top">
                <p>
                    <strong>כלול זמן</strong>
                </p>
            </td>
            <td width="46" valign="top">
                <p>
                    <strong>כלול הוצאה</strong>
                </p>
            </td>
            <td width="43" valign="top">
                <p>
                    <strong>כלול חומר</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>כולל</strong>
                </p>
                <p>
                    <strong>תשלום</strong>
                </p>
            </td>
            <td width="49" valign="top">
                <p>
                    <strong>חוקי/לא חוקי</strong>
                </p>
            </td>
            <td width="200" valign="top">
                <p>
                    <strong>סיבה</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
ריק </p>
            </td>
            <td width="45" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="46" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="43" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="41" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
לא חוקי </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
הפרת כלל מס' 2. זמן, הוצאות ועמלות בפרויקט P1 כלולים בשורות הצעות מחיר QL1 ו-QL2 </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
ריק </p>
            </td>
            <td width="45" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="46" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="43" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="41" valign="top">
                <p>
‏‏כן </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
ריק </p>
            </td>
            <td width="45" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="46" valign="top">
                <p>
Yes </p>
            </td>
            <td width="43" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="41" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
לא חוקי </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
הפרת כלל מס' 2. זמן, חומר ועמלות בפרויקט P1 כלולים בשורות הצעות מחיר QL1 ו-QL2 </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
ריק </p>
            </td>
            <td width="45" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="46" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="43" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="41" valign="top">
                <p>
‏‏כן </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
ריק </p>
            </td>
            <td width="45" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="46" valign="top">
                <p>
Yes </p>
            </td>
            <td width="43" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="41" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
חוקי </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
זמן, חומר ועמלות בפרויקט P1 כלולים ב- QL1 <br>
הוצאות בפרויקט P1 כלולות ב-QL2 <br>
אין חפיפה במה שנכלל בכל שורת הצעת מחיר, ולכן תקף.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
ריק </p>
            </td>
            <td width="45" valign="top">
                <p>
Yes </p>
            </td>
            <td width="46" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="43" valign="top">
                <p>
Yes </p>
            </td>
            <td width="41" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
משימות נבחרות בלבד </p>
            </td>
            <td width="45" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="46" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="43" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="41" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
לא חוקי </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
הפרת כלל מס' 2 </p>
                <p>
Q1 כולל זמן, חומר, הוצאות ועמלות לקבוצת משנה של משימות בפרויקט P1 </p>
                <p>
QL2 כולל זמן, הוצאות ועמלות עבור כל הפרויקט P1 ולכן חופף את מה שנכלל ב-Q1.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
ריק </p>
            </td>
            <td width="45" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="46" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="43" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="41" valign="top">
                <p>
‏‏כן </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
משימות נבחרות בלבד </p>
            </td>
            <td width="45" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="46" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="43" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="41" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
חוקי </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
לפי כלל מס '3, </p>
                <p>
Q1 כולל זמן, חומר, הוצאות ועמלות לקבוצת משנה של משימות בפרויקט P1.
                </p>
                <p>
QL2 כולל זמן, חומרים, הוצאות ועמלות לקבוצת משנה של משימות בפרויקט P1.
                </p>
                <p>
האימות הנוסף היחיד הוא שקבוצת המשנה של המשימות ב- QL1 שונה מקבוצת משנה של המשימות ב- QL2 כדי להבטיח שאין חפיפה. פעולה זו מתבצעת על ידי המערכת כאשר משימות משויכות.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
משימות נבחרות בלבד </p>
            </td>
            <td width="45" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="46" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="43" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="41" valign="top">
                <p>
‏‏כן </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
כל משימות הפרויקט או ריק </p>
            </td>
            <td width="45" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="46" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="43" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="41" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
חוקי </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
לפי כלל מס '5, Q1 ו- Q2 הן שתי הצעות מחיר לאותה הזדמנות, כך שניתן להשתמש בשתיהן להערכת אותם מרכיבי הפרויקט.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ר2 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
כל משימות הפרויקט או ריק </p>
            </td>
            <td width="45" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="46" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="43" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="41" valign="top">
                <p>
‏‏כן </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
כל משימות הפרויקט או ריק </p>
            </td>
            <td width="45" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="46" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="43" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="41" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
לא חוקי </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
לפי כלל מס '4, Q1 ו- Q2 הן שתי הצעות מחיר להזדמנויות שונות, כך שלא ניתן להשתמש בשתיהן להערכת אותם מרכיבים של אותו הפרויקט.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O2 </p>
            </td>
            <td width="39" valign="top">
                <p>
ר1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
כל משימות הפרויקט או ריק </p>
            </td>
            <td width="45" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="46" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="43" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="41" valign="top">
                <p>
‏‏כן </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
