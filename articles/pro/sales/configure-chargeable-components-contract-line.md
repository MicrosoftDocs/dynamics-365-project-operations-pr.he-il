---
title: ‏‫קביעת תצורה של רכיבים ניתנים לחיוב בסעיף חוזה מבוסס פרוייקט‬
description: מאמר זה מספק מידע על אופן הוספת רכיבים הניתנים לחיוב לסעיפי חוזה ב- Project Operations.
author: rumant
ms.date: 10/08/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 0e4118e8e56d45ef75f53d828e267a8a9c1c903a
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922959"
---
# <a name="configure-chargeable-components-of-a-project-based-contract-line"></a>‏‫קביעת תצורה של רכיבים ניתנים לחיוב בסעיף חוזה מבוסס פרוייקט‬

_**חל על:** פריסה קלה - עסקה עם חשבונית פרופורמה, Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

בסעיף חוזה מבוסס פרויקט יש רכיבים *כלולים* ורכיבים *הניתנים לחיוב*.

רכיבים כלולים הם רכיבים הכפופים ל:

  - שיטת חיוב ופיצולי לקוחות
  - מגבלות 'אין לחרוג' 
  - הגדרות תדירות חשבוניות שהוגדרה בסעיף החוזה מבוסס הפרויקט

ניתן לסמן תת קבוצה של הרכיבים הכלולים כניתנים לחיוב באמצעות השדה **סוג חיוב**. השדה **סוג חיוב** הוא קבוצת אפשרויות המאפשרת את הערכים הבאים בהקשר של סעיף חוזה:

  - ניתן לחיוב
  - לא ניתן לחיוב

ניתן להגדיר רכיבים הניתנים לחיוב במשימות, בתפקידים ובקטגוריות של עסקאות.

יכולת חיוב מוגדרת במשימות עבור סעיף חוזה פרויקט וחל על כל סיווגי העסקאות הכלולות בסעיף. אם השדה **כלול משימות** בסעיף החוזה ריק או מוגדר **כפרויקט כולו**, הכרטיסיה **משימות ניתנות לחיוב** לא תהיה זמינה.

יכולת חיוב המוגדרת בתפקידים עבור סעיף חוזה פרויקט חלה רק על סיווג העסקאות **זמן**. אם השדה **כלול משימות** בסעיף החוזה ריק או מוגדר **לא**, הכרטיסיה **תפקידים ניתנים לחיוב** לא תהיה זמינה.

יכולת חיוב המוגדרת בקטגוריות של עסקאות עבור סעיף חוזה פרויקט חלה רק על סיווג העסקאות **הוצאה**. אם השדה **לכלול הוצאות** מוגדר כ **לא**, הכרטיסיה **קטגוריות הניתנות לחיוב** לא תהיה זמינה.

### <a name="update-a-project-task-as-chargeable-or-non-chargeable"></a>עדכן משימת פרויקט כניתנת לחיוב או כלא ניתנת לחיוב

משימת פרויקט יכולה להיות ניתנת לחיוב או לא ניתנת לחיוב בסעיף חוזה ספציפי, דבר המאפשר את הגדרה הבאה:

אם סעיף חוזה מבוסס פרויקט כולל **זמן** ומשימה מסוימת, **T1** משוייכת אליו כניתנת לתשלום. אם יש סעיף חוזה שני שכולל **הוצאה**, ניתן לשייך את המשימת T1 בסעיף החוזה כלא ניתנת לחיוב. התוצאה היא שכל הזמן שנרשם במשימה ניתן לחיוב וכל ההוצאות אינן ניתנות לחיוב.

ניתן להגדיר את סוג החיוב של משימה בכרטיסיה **משימות הניתנות לחיוב** של סעיף החוזה על ידי עדכון השדה **סוג החיוב** ברשת המשנה של משימות סעיף החוזה. לחלופין, ניתן לעדכן את השדה **סוג חיוב** ברשת המשנה של הגדרת חיוב משימה של פרויקט המציג את סעיפי החוזה המשויכים למשימה.

### <a name="update-a-role-as-chargeable-or-non-chargeable"></a>עדכן תפקיד כניתן לחיוב או כלא ניתן לחיוב

תפקיד יכול להיות ניתן לחיוב או לא ניתן לחייב בסעיף חוזה ספציפי.

ניתן להגדיר את סוג החיוב של תפקיד בכרטיסיה **תפקידים הניתנים לחיוב** של סעיף חוזה. לשם כך, עדכן את השדה **סוג חיוב** ברשת המשנה **תפקידים הניתנים לחיוב**.

### <a name="update-a-transaction-category-as-chargeable-or-non-chargeable"></a>עדכן קטגוריה של עסקאות כניתנת לחיוב או כלא ניתנת לחיוב

קטגוריה של עסקאות יכולה להיות ניתנת לחיוב או לא ניתנת לחייב בסעיף חוזה ספציפי.

ניתן להגדיר את סוג החיוב של עסקה בכרטיסיה **קטגוריות הניתנות לחיוב** של סעיף חוזה מבוסס פרויקט. לשם כך, עדכן את השדה **סוג חיוב** ברשת המשנה **קטגוריות הניתנות לחיוב**.

### <a name="resolve-chargeability"></a>פתרון של יכולת חיוב

הערכה או נתונים בפועל שנוצרו עבור זמן נחשבים כניתנים לחיוב רק אם:

   - **זמן** כלול בסעיף חוזה.
   - **תפקיד** מוגדר כניתן לחיוב בסעיף חוזה.
   - **משימות כלולות** מוגדרות בתור **משימות נבחרות** בסעיף חוזה.
 
 אם שלושת הדברים הללו נכונים, המשימה מוגדרת כניתנת לחיוב. 

הערכה או נתונים בפועל שנוצרו עבור הוצאה נחשבים כניתנים לחיוב רק אם:

   - **הוצאה** כלולה בסעיף חוזה
   - **קטגוריית עסקה** מוגדרת כניתנת לחיוב בסעיף חוזה
   - **משימות כלולות** מוגדרות בתור **משימות נבחרות** בסעיף חוזה
  
 אם שלושת הדברים הללו נכונים **המשימה** מוגדרת כניתנת לחיוב. 

הערכה או נתונים בפועל שנוצרו עבור חומר נחשבים כניתנים לחיוב רק אם:

   - **חומרים** כלולים בסעיף חוזה
   - **משימות כלולות** מוגדרות בתור **משימות נבחרות** בסעיף חוזה

אם שני הדברים הללו נכונים **המשימה** מוגדרת כניתנת לחיוב. 

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p>
                    <strong>כולל זמן</strong>
                </p>
            </td>
            <td width="78" valign="top">
                <p>
                    <strong>כולל הוצאה</strong>
                    <strong></strong>
                </p>
            </td>
            <td width="63" valign="top">
                <p>
                    <strong>כולל חומרים</strong>
                    <strong></strong>
                </p>
            </td>
            <td width="75" valign="top">
                <p>
                    <strong>משימות כלולות</strong>
                    <strong></strong>
                </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>תפקיד</strong>
                    <strong></strong>
                </p>
            </td>
            <td width="70" valign="top">
                <p>
                    <strong>קטגוריה</strong>
                    <strong></strong>
                </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>משימה</strong>
                    <strong></strong>
                </p>
            </td>
            <td width="350" valign="top">
                <p>
                    <strong>השפעת יכולת החיוב</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="78" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="63" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="75" valign="top">
                <p>
הפרוייקט כולו </p>
            </td>
            <td width="65" valign="top">
                <p>
ניתן לחיוב </p>
            </td>
            <td width="70" valign="top">
                <p>
ניתן לחיוב </p>
            </td>
            <td width="65" valign="top">
                <p>
לא ניתן להגדיר </p>
            </td>
            <td width="350" valign="top">
                <p>
חיוב לפי נתוני זמן בפועל: <strong>ניתן לחיוב</strong>
                </p>
                <p>
סוג חיוב עבור נתוני הוצאה בפועל: <strong>ניתן לחיוב</strong>
                </p>
                <p>
סוג חיוב עבור נתוני חומר בפועל: <strong>ניתן לחיוב</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="78" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="63" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="75" valign="top">
                <p>
משימות נבחרות בלבד </p>
            </td>
            <td width="65" valign="top">
                <p>
ניתן לחיוב </p>
            </td>
            <td width="70" valign="top">
                <p>
ניתן לחיוב </p>
            </td>
            <td width="65" valign="top">
                <p>
ניתן לחיוב </p>
            </td>
            <td width="350" valign="top">
                <p>
חיוב לפי נתוני זמן בפועל: <strong>ניתן לחיוב</strong>
                </p>
                <p>
סוג חיוב עבור נתוני הוצאה בפועל: <strong>ניתן לחיוב</strong>
                </p>
                <p>
סוג חיוב עבור נתוני חומר בפועל: <strong>ניתן לחיוב</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="78" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="63" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="75" valign="top">
                <p>
משימות נבחרות בלבד </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>לא ניתן לחיוב</strong>
                </p>
            </td>
            <td width="70" valign="top">
                <p>
ניתן לחיוב </p>
            </td>
            <td width="65" valign="top">
                <p>
ניתן לחיוב </p>
            </td>
            <td width="350" valign="top">
                <p>
חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </p>
                <p>
סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב </p>
                <p>
סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="78" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="63" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="75" valign="top">
                <p>
משימות נבחרות בלבד </p>
            </td>
            <td width="65" valign="top">
                <p>
ניתן לחיוב </p>
            </td>
            <td width="70" valign="top">
                <p>
ניתן לחיוב </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>לא ניתן לחיוב</strong>
                </p>
            </td>
            <td width="350" valign="top">
                <p>
חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </p>
                <p>
סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </p>
                <p>
סוג חיוב עבור נתוני חומר בפועל: <strong>לא ניתן לחיוב</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="78" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="63" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="75" valign="top">
                <p>
משימות נבחרות בלבד </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>לא ניתן לחיוב</strong>
                </p>
            </td>
            <td width="70" valign="top">
                <p>
ניתן לחיוב </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>לא ניתן לחיוב</strong>
                </p>
            </td>
            <td width="350" valign="top">
                <p>
חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </p>
                <p>
סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </p>
                <p>
סוג חיוב עבור נתוני חומר בפועל: <strong>לא ניתן לחיוב</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="78" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="63" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="75" valign="top">
                <p>
משימות נבחרות בלבד </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>לא ניתן לחיוב</strong>
                </p>
            </td>
            <td width="70" valign="top">
                <p>
                    <strong>לא ניתן לחיוב</strong>
                </p>
            </td>
            <td width="65" valign="top">
                <p>
ניתן לחיוב </p>
            </td>
            <td width="350" valign="top">
                <p>
חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </p>
                <p>
סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </p>
                <p>
סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
                    <strong>Yes</strong>
                </p>
            </td>
            <td width="78" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="63" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="75" valign="top">
                <p>
הפרוייקט כולו </p>
            </td>
            <td width="65" valign="top">
                <p>
לא ניתן להגדיר </p>
            </td>
            <td width="70" valign="top">
                <p>
                    <strong>ניתן לחיוב</strong>
                </p>
            </td>
            <td width="65" valign="top">
                <p>
לא ניתן להגדיר </p>
            </td>
            <td width="350" valign="top">
                <p>
חיוב לפי נתוני זמן בפועל: <strong>לא זמין</strong>
                </p>
                <p>
סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב </p>
                <p>
סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
                    <strong>Yes</strong>
                </p>
            </td>
            <td width="78" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="63" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="75" valign="top">
                <p>
הפרוייקט כולו </p>
            </td>
            <td width="65" valign="top">
                <p>
לא ניתן להגדיר </p>
            </td>
            <td width="70" valign="top">
                <p>
                    <strong>לא ניתן לחיוב</strong>
                </p>
            </td>
            <td width="65" valign="top">
                <p>
לא ניתן להגדיר </p>
            </td>
            <td width="350" valign="top">
                <p>
חיוב לפי נתוני זמן בפועל: <strong>לא זמין</strong>
                </p>
                <p>
סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </p>
                <p>
סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="78" valign="top">
                <p>
                    <strong>Yes</strong>
                </p>
            </td>
            <td width="63" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="75" valign="top">
                <p>
הפרוייקט כולו </p>
            </td>
            <td width="65" valign="top">
                <p>
ניתן לחיוב </p>
            </td>
            <td width="70" valign="top">
                <p>
לא ניתן להגדיר </p>
            </td>
            <td width="65" valign="top">
                <p>
לא ניתן להגדיר </p>
            </td>
            <td width="350" valign="top">
                <p>
חיוב לפי נתוני זמן בפועל: ניתן לחיוב </p>
                <p>
סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא זמין</strong>
                </p>
                <p>
סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="78" valign="top">
                <p>
                    <strong>Yes</strong>
                </p>
            </td>
            <td width="63" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="75" valign="top">
                <p>
הפרוייקט כולו </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>לא ניתן לחיוב</strong>
                </p>
            </td>
            <td width="70" valign="top">
                <p>
לא ניתן להגדיר </p>
            </td>
            <td width="65" valign="top">
                <p>
לא ניתן להגדיר </p>
            </td>
            <td width="350" valign="top">
                <p>
חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </p>
                <p>
סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא זמין</strong>
                </p>
                <p>
סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="78" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="63" valign="top">
                <p>
                    <strong>Yes</strong>
                </p>
            </td>
            <td width="75" valign="top">
                <p>
הפרוייקט כולו </p>
            </td>
            <td width="65" valign="top">
                <p>
ניתן לחיוב </p>
            </td>
            <td width="70" valign="top">
                <p>
ניתן לחיוב </p>
            </td>
            <td width="65" valign="top">
                <p>
לא ניתן להגדיר </p>
            </td>
            <td width="350" valign="top">
                <p>
חיוב לפי נתוני זמן בפועל: ניתן לחיוב </p>
                <p>
סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב </p>
                <p>
סוג חיוב עבור נתוני חומר בפועל: <strong>לא זמין</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="78" valign="top">
                <p>
‏‏כן </p>
            </td>
            <td width="63" valign="top">
                <p>
                    <strong>Yes</strong>
                </p>
            </td>
            <td width="75" valign="top">
                <p>
הפרוייקט כולו </p>
            </td>
            <td width="65" valign="top">
                <p>
                    <strong>לא ניתן לחיוב</strong>
                </p>
            </td>
            <td width="70" valign="top">
                <p>
                    <strong>לא ניתן לחיוב</strong>
                </p>
            </td>
            <td width="65" valign="top">
                <p>
לא ניתן להגדיר </p>
            </td>
            <td width="350" valign="top">
                <p>
חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </p>
                <p>
סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </p>
                <p>
סוג חיוב עבור נתוני חומר בפועל: <strong>לא זמין</strong>
                </p>
            </td>
        </tr>
    </tbody>
</table>





[!INCLUDE[footer-include](../../includes/footer-banner.md)]
