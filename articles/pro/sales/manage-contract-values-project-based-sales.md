---
title: מבט כולל על סעיפי חוזה מבוססי פרוייקט
description: נושא זה מספק מידע על עבודה עם סעיפי חוזה מבוססי פרויקט.
author: rumant
ms.date: 10/28/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: 22e8ff927c5ff6c3748a35031e7703e3fcfe0dab
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 07/07/2021
ms.locfileid: "6369917"
---
# <a name="project-based-contract-lines-overview"></a>מבט כולל על סעיפי חוזה מבוססי פרוייקט

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

סעיפי חוזה מבוססי פרויקטים ב- Dynamics 365 Project Operations נועדו להחזיק את הסכמי ההערכה והחיוב עבור רכיבים ספציפיים בעבודת הפרויקט של ההתקשרות. המבנה של סעיף חוזה מבוסס פרויקט מורחב להערכות פרויקט ותרחישי החיוב עם המושגים הבאים:

- שיטת חיוב
- מיפוי פרוייקט ומשימות
- סווגי עסקה כלולים
- מגבלת 'אין לחרוג'
- הגדרת יכולת חיוב
- הערכות המשתמשות בפרטי סעיף חוזה
- לקוחות סעיף חוזה

הטבלה הבאה כוללת את השדות בכרטיסיה **כללי** של סעיפי חוזה מבוססי פרויקטים המסייעים בהגדרת הבסיס להערכה מפורטת ומבוססת והסדרי חיוב עבור עבודה מבוססת פרויקטים.

| שדה | תיאור | השפעה במורד הזרם |
| --- | --- | --- |
| **שם** | שם סעיף החוזה. שם זה מזהה את המרכיב הנפרד של החוזה שמוערך. עבור חוזה פרויקט שנוצר מהצעת מחיר, ערך זה מועתק מערך מקביל בשורת הצעת המחיר מבוססת הפרויקט. | השם שהועתק לשורת חשבונית הפרויקט שנוצרת מסעיף חוזה זה בעת יצירת החשבונית. |
| **שיטת חיוב** | בחוזה פרויקט שנוצר מהצעת מחיר, ערך זה מועתק מהשדה המקביל בשורת הצעת המחיר. זהו קבוצת אפשרויות המייצג את שני המודלי החוזה העיקריים הנתמכים על ידי Project Operations:</br>- **מחיר קבוע**</br>- **זמן וחומרים** | העסקה בפועל תעובד בהתבסס על שיטת החיוב של סעיף החוזה המוזכר. אם לסעיף החוזה אליו מתייחס הנתון בפועל יש שיטת חיוב של זמן וחומרים, נוצרים רשומות של נתונים בפועל של עלויות ומכירות שלא חויבו. אם לסעיף החוזה אליו מתייחס הנתון בפועל יש שיטת חיוב במחיר קבוע, נוצר רק נתון בפועל של עלות. |
| **פרויקט** | השתמש בשדה זה כדי לזהות את הפרויקט שישמש מסירת העבודה בהתקשרות זו. | ערך זה ישמש יחד עם **משימות כלולות** ו **סיווגי עסקאות כלולים** כדי לפענח את ההפניה לסעיף החוזה ברשומת שורת הערכה או נתונים בפועל. |
| **משימות כלולות** | מציין אם סעיף חוזה זה כולל את כל משימות הפרויקט עבור הפרויקט שנבחר או רק קבוצת משנה של המשימות. זוהי קבוצת אפשרויות בעלת הערכים האפשריים הבאים:</br>- **כל משימות הפרויקט**</br>- **משימות פרויקט נבחרות בלבד**. ערך ריק בשדה זה שווה לבחירה של **כל משימות הפרויקט**. | אם האפשרות **משימות נבחרות בלבד** נבחרת, ניתן לבחור משימות ספציפיות ולשייך אותן לסעיף חוזה זה בכרטיסיה **הגדרת חיוב משימות**  בדף **פרויקט**. ערך זה ישמש יחד עם הסיווגים **פרוייקט** ו **משימה כלולה** כדי לפתור את הפניה ברשומת שורה של נתון בפועל או הערכה. |
| **כלול זמן** | הערך **כן**/**לא** מציין אם עסקאות זמן או עלויות עבודה בפרויקט שנבחר ייכללו בסעיף חוזה זה. הערך **לא** מציין שעסקאות זמן או עלויות עבודה לא ייכללו בסעיף החוזה הזה. הערך **כן** מציין שהם יכללו. | ערך זה משמש בשילוב עם הפרויקט כדי לפענח את הפניה לסעיף החוזה ברשומת שורת הערכה או נתונים בפועל. |
| **כלול הוצאה** | הערך **כן**/**לא** מציין אם עלויות הוצאה בפרויקט שנבחר ייכללו בסעיף חוזה זה. הערך **לא** מציין שעלות ההוצאה לא תיכלל בסעיף החוזה הזה. הערך **כן** מציין שהיא תיכלל. | ערך זה משמש בשילוב עם הפרויקט כדי לפענח את הפניה לסעיף החוזה ברשומת שורת הערכה או נתונים בפועל. |
| **כלול חומרים** | הערך **כן**/**לא** מציין אם עלויות חומר בפרויקט שנבחר ייכללו בסעיף חוזה זה. הערך **לא** מציין שעלויות חומר לא ייכללו בסעיף חוזה זה. הערך **כן** מציין שהיא תיכלל. | ערך זה משמש בשילוב עם הפרויקט כדי לפענח את הפניה לסעיף החוזה ברשומת שורת הערכה או נתונים בפועל. |
| **כלול תשלום** | הערך **כן**/**לא** מציין אם עמלות בפרויקט שנבחר ייכללו בסעיף חוזה זה. הערך **לא** מציין שעמלות לא יכללו בסעיף החוזה הזה. הערך **כן** מציין שהם יכללו. | ערך זה משמש בשילוב עם הפרויקט כדי לפענח את הפניה לסעיף החוזה ברשומת שורת הערכה או נתונים בפועל. |
| **הסכום שעליו סוכם בחוזה** | בסעיף חוזה במחיר קבוע, סכום זה הוא הערך המוסכם שיחויב ללקוח עבור כל רכיבי העבודה הקשורים לסעיף חוזה זה. בסעיף חוזה במחיר קבוע, סכום זה הוא ערך מעורך של מה שיחויב ללקוח עבור כל רכיבי העבודה הקשורים לסעיף חוזה זה. בחוזה פרויקט שנוצר מהצעת מחיר, ערך זה מועתק מהשדה המקביל בשורת הצעת המחיר. כאשר בסעיף חוזה מבוסס פרויקט יש פרטי סעיף, שדה זה נעול לעריכה ומסוכם מהסכום המופיע בפרטי סעיף החוזה. | כאשר בסעיף החוזה יש פרטי סעיף, ניתן לשנות ערך זה על ידי שינוי הסכומים בפרטי הסעיף. בסעיף חוזה במחיר קבוע, ערך זה משמש להפקת הסכום לפני מס בגין אבני דרך תקופתיות לחיוב. |
| **מס משוער** | המשתמש יכול לערוך שדה זה כדי להזין את סכום המס המשוער בסעיף החוזה. כאשר בסעיף חוזה מבוסס פרויקט יש פרטי סעיף, שדה זה נעול לעריכה ומסוכם מסכום המס המופיע בפרטי סעיף החוזה. | כאשר בסעיף החוזה יש פרטי סעיף, ניתן לשנות ערך זה על ידי שינוי סכומי המס בפרטי הסעיף. בסעיף חוזה במחיר קבוע, ערך זה משמש להפקת המס בגין אבני דרך תקופתיות לחיוב. |
| **הסכום שעליו סוכם בחוזה, אחרי מס** | הסכום סעיף החוזה, אחרי מס. שדה זה הוא לקריאה בלבד ומחושב כ **הסכום שעלו סוכם בחוזה + מס**. | בסעיף חוזה במחיר קבוע, ערך זה משמש להפקת אבני דרך תקופתיות לחיוב. |
| **מגבלת 'אין לחרוג'** | המשתמש יכול לערוך שדה זה והוא זמין רק סעיפי חוזה מבוססי פרויקט שבהם מגדרת שיטת החיוב כזמן וחומרים. | המשתמש יכול לערוך שדה זה. כאשר נתון בפעול של זמן וחומרים מפנה לסעיף חוזה זה עבור זמן וחומרים, הסכום בנתון פועל מוערך מול מגבלת אין לחרוג בסעיף החוזה. הערכה זו מסתיימת לאחר שהסכומים שכבר הוצאו ושמחויבים הובאו בחשבון. |
| **תקציב הלקוח** | שדה זה ניתן לעריכה ומועתק מהשדה המקביל בשורת הצעת המחיר עם החוזה נוצר מהצעת מחיר. | שדה זה משמש למידע בלבד ואין לו שום משמעות במורד הזרם. |

## <a name="validation-rules-for-the-options-on-the-general-tab-of-project-based-contract-lines"></a>כללי אימות עבור האפשרויות בכרטיסיה 'כללי' של סעיפי חוזה מבוססי פרויקט

כלל 1: אם השדה **משימות כלולות** ריק או מוגדר כ **כל משימות הפרויקט**, כל המשימות של הפרויקט כלולות בסעיף החוזה.

כלל 2: כאשר השדה **משימות כלולות** ריק או מוגדר במפורש כ **כל משימות הפרויקט**, פרויקט וסיווג עסקאות מסוים יכולים להיכלל בסעיף חוזה מבוסס פרויקט אחד בלבד של חוזה.

כלל 3: כאשר השדה **משימות כלולות** מוגדר כ **משימות הפרויקט נבחרות בלבד**, פרויקט וסיווג עסקאות מסוים יכולים להיכלל בסעיפי חוזה מבוססי פרויקט מרובים של חוזה.

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="43" valign="top">
                <p>
                    <strong>חוזה</strong>
                </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>סעיף חוזה</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>פרויקט</strong>
                </p>
            </td>
            <td width="67" valign="top">
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
                    <strong>כלול חומרים</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>כולל</strong>
                </p>
                <p>
                    <strong>תשלום</strong>
                </p>
            </td>
            <td width="53" valign="top">
                <p>
                    <strong>חוקי/לא חוקי</strong>
                </p>
            </td>
            <td width="250" valign="top">
                <p>
                    <strong>סיבה</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
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
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
לא חוקי </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
הפרת כלל מס' 2. זמן, הוצאות, חומרים ועמלות בפרויקט P1 כלולים בסעיפי החוזה CL1 ו- CL2.
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
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
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
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
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
לא חוקי </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
הפרת כלל מס' 2. זמן, חומרים ועמלות בפרויקט P1 כלולים בסעיפי החוזה CL1 ו- CL2.
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
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
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
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
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
חוקי </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
זמן, חומרים ועמלות בפרויקט P1 כלולים ב- CL1.
                </p>
                <ul>
                    <li>
הוצאות בפרויקט P1 כלולות ב-CL2.
                    </li>
                </ul>
                <p>
אין חפיפה במה שנכלל בכל סעיף חוזה, ולכן תקף.
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
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
            <td width="42" valign="top">
                <p>
Yes </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
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
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
לא חוקי </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
הפרת כלל מס' 2 </p>
                <p>
C1 כולל זמן, חומרים, הוצאות ועמלות לקבוצת משנה של משימות בפרויקט P1.
                </p>
                <p>
CL2 כולל זמן, חומרים, הוצאות ועמלות עבור כל הפרויקט P1 ולכן חופף למה שנכלל ב- C1.
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
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
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
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
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
חוקי </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
לפי כלל מס '3 </p>
                <p>
C1 כולל זמן, חומרים, הוצאות ועמלות לקבוצת משנה של משימות בפרויקט P1.
                </p>
                <p>
CL2 כולל זמן, חומרים, הוצאות ועמלות לקבוצת משנה של משימות בפרויקט P1.
                </p>
                <p>
האימות הנוסף היחיד הוא שקבוצת המשנה של המשימות ב- CL1 שונה מקבוצת משנה של המשימות ב- CL2 כדי להבטיח שאין שם חפיפה. פעולה זו מתבצעת על ידי המערכת כאשר משימות משויכות.
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
C1 </p>
            </td>
            <td width="65" valign="top">
                <p>
CL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="67" valign="top">
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
            <td width="42" valign="top">
                <p>
‏‏כן </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
