---
title: מבט כולל על שורות הצעת מחיר של פרוייקט
description: נושא זה מסביר כיצד להשתמש בשורות הצעת מחיר של פרוייקט עבור עבודת פרוייקט.
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: c585bbc55119e678a4f75f5dfe8966a436db1a34
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368072"
---
# <a name="project-quote-lines-overview"></a>מבט כולל על שורות הצעת מחיר של פרוייקט

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

שורות הצעת מחיר מבוססות פרויקט נועדו לעזור להעריך את עבודת הפרויקט עבור התקשרות. המבנה של שורת הצעות מחיר מבוסס פרויקט מורחב להערכות פרויקט באמצעות המושגים הבאים:

- שיטת חיוב
- מיפוי פרויקטים
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
| פרויקט | השתמש בשדה אופציונלי זה כדי לזהות את הפרויקט שישמש להגשת העבודה בהתקשרות זו. כאשר פרויקט ממופה לשורת הצעת מחיר, זה עוזר בהגדרת משימות הניתנות לחיוב וגם בכנסת הערכה מבוססת פרויקט לשורת הצעת המחיר, כפרטים בשורת הצעת מחיר. כאשר פרויקט אינו ממופה לשורת הצעת מחיר מבוססת פרויקט, יש ליצור את ההערכה באופן ידני על ידי יצירת כל פרט שבשורת הצעת המחיר. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| כלול זמן | דגל **כן**/**לא** מציין אם עסקאות זמן או עלויות עבודה בפרויקט שנבחר ייכללו בהערכה בשורת הצעת מחיר זו. הערך **לא** מציין שעסקאות זמן או עלויות עבודה לא ייכללו בהערכה בשורת הצעת מחיר זו. הערך **כן** מציין שעסקאות זמן או עלויות עבודה ייכללו בהערכה בשורת הצעת מחיר זו. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| כלול הוצאה | דגל **כן**/**לא** מציין אם עלויות ההוצאות בפרויקט שנבחר ייכללו בהערכה בשורת הצעת מחיר זו. הערך **לא** מציין שעלויות ההוצאות לא ייכללו בהערכה בשורת הצעת מחיר זו. הערך **כן** מציין שעלויות ההוצאות ייכללו בהערכה בשורת הצעת מחיר זו. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| כלול תשלום | דגל **כן**/**לא** מציין אם עמלות על הפרויקט שנבחר ייכללו בהערכה בשורת הצעת מחיר זו. הערך **לא** מציין שהעמלות לא ייכללו בהערכה בשורת הצעת מחיר זו. הערך **כן** מציין שהעמלות ייכללו בהערכה בשורת הצעת מחיר זו. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| הסכום של הצעת המחיר | זהו סכום הצעת המחיר שינתן ללקוח עבור כל העבודה החזויה בשורת הצעת מחיר מבוססת פרויקט זו. בהצעת מחיר שנוצרת מהזדמנות, ערך זה מועתק מהשדה **תקציב הלקוח** שבשורת הזדמנות. כשבשורת צעת מחיר מבוססת הפרויקט יש פרטי שורה, שדה זה נעול לעריכה ומסוכם מהסכום שנמצא בפרטים בשורת הצעת המחיר. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| מס משוער | זהו שדה הניתן לעריכה שהמשתמש יכול להוסיף בו את סכום המס המשוער בשורת הצעת המחיר. כשבשורת צעת מחיר מבוססת הפרויקט יש פרטי שורה, שדה זה נעול לעריכה ומסוכם מסכום המס שנמצא בפרטים בשורת הצעת המחיר. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| סכום הצעת המחיר, אחרי מס | שדה זה הוא סכום שורת הצעת המחיר לאחר מס והוא לקריאה בלבד. הסכום בשדה זה מחושב כ *סכום הצעת המחיר + מס*. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| מגבלת 'אין לחרוג' | שדה זה ניתן לעריכה והוא זמין רק בשורות הצעות מחיר מבוססות פרויקט עם שיטת חיוב של **זמן וחומרים**. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |
| תקציב הלקוח | שדה זה ניתן לעריכה ומועתק מהשדה התואם בשורת ההזדמנות אם הצעת המחיר נוצרה מהזדמנות. | ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר. |

## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a>כללי אימות עבור שדות בכרטיסיה 'כללי' של שורות הצעות מחיר מבוססות פרויקט

**כלל 1**: ניתן לכלול סיווג עסקאות מסוים רק בשורת הצעת מחיר מבוססת פרויקט אחת של הצעת מחיר.

**כלל 2**: אם להזדמנות יש הצעות מחיר מרובות, יכולות להיות שורות הצעות מחיר מהצעות מחיר שונות, אשר מתייחסות כולן לאותו פרויקט וכוללות את אותו סיווג עסקאות.

**כלל 3**: אם הצעות המחיר אינן שייכות לאותה הזדמנות, הן אינן יכולות לכלול את אותו פרויקט וסיווג עסקאות.

<table border="1" cellspacing="0" cellpadding="0">
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
                    <strong>עמלה</strong>
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
הפרת כלל מס' 1. זמן, הוצאות ועמלות בפרויקט P1 כלולים בשתי שורות הצעות המחיר QL1 ו-QL2.
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
הפרת כלל מס' 1. זמן ועמלות בפרויקט P1 כלולים בשתי שורות הצעות המחיר QL1 ו-QL2.
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
אין חפיפה במה שנכלל בכל שורת הצעת מחיר כך ושהיא תקפה.
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
הפרת כלל מס' 1 שלעיל </p>
                <p>
ר1 כולל זמן, הוצאות ועמלות עבור הפרויקט P1 בכללותו.
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
בהתבסס על כלל מס' 2, Q1 ו-Q2 הן שתי הצעות מחיר באותה הזדמנות, כך ששתיהן יכולות לשמש להערכת אותם רכיבי פרויקט.
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
‏‏QL1 ב-Q2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
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
בהתבסס על כלל מס' 3, Q1 ו-Q2 הן שתי הצעות מחיר עבור הזדמנויות שונות, כך שהן אינן יכולות לשמש להערכת אותם הרכיבים של אותו הפרויקט.
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



[!INCLUDE[footer-include](../includes/footer-banner.md)]
