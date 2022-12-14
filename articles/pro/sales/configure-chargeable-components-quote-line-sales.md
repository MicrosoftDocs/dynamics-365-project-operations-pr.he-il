---
title: קביעת תצורה של הרכיבים הניתנים לחיוב בשורות הצעות מחיר של פרוייקט
description: מאמר זה מספק מידע על הגדרת רכיבים הניתנים לחיוב ורכיבים שלא ניתנים חיוב בשורת הצעת מחיר מבוססת פרויקט.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 1e454278a1c5c24ac346c537c778b25448d9ea03
ms.sourcegitcommit: e0cbbe7c6f03d4978134405cf04bd8bc1d019f65
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 12/05/2022
ms.locfileid: "9825518"
---
# <a name="configure-chargeable-components-on-project-quote-lines"></a>קביעת תצורה של הרכיבים הניתנים לחיוב בשורות הצעות מחיר של פרוייקט

_**חל על:** פריסה קלה - עסקה עם חשבונית פרופורמה, Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

בסעיף חוזה מבוסס פרויקט יש מושג של רכיבים *כלולים* ורכיבים *הניתנים לחיוב*.

הרכיבים הכלולים כפופים ל:

  - שיטת חיוב ופיצולי לקוחות
  - מגבלות 'אין לחרוג' 
  - הגדרות תדירות חשבוניות שהוגדרה בשורת הצעת המחיר מבוססת פרויקט

ניתן לסמן תת קבוצה של הרכיבים הכלולים כניתנים לחיוב באמצעות השדה **סוג חיוב**. השדה **סוג החיוב** הוא קבוצת אפשרויות המאפשרת את הערכים הבאים בהקשר של שורת הצעת מחיר:

  - ניתן לחיוב
  - לא ניתן לחיוב

ניתן להגדיר רכיבים הניתנים לחיוב במשימות, בתפקידים ובקטגוריות של עסקאות.

יכולת חיוב מוגדרת במשימות עבור שורת הצעת מחיר וחלה על כל סיווגי העסקאות הכלולות באותה שורה. אם השדה **כלול משימות** מוגדר **כפרויקט כולו**, או נותר ריק, הכרטיסיה **משימות ניתנות לחיוב** לא תהיה זמינה.

יכולת חיוב המוגדרת בתפקידים עבור שורת הצעת מחיר וחלה רק על סיווג העסקאות **זמן**. אם השדה **כלול משימות** מוגדר כ **לא** בשורת הצעת מחיר של פרויקט, הכרטיסיה **תפקידים ניתנים לחיוב** לא תהיה זמינה.

יכולת חיוב המוגדרת בקטגוריות של עסקאות עבור שורת הצעת מחיר וחלה רק על סיווג העסקאות **הוצאה**. אם השדה **כלול הוצאות** מוגדר כ **לא** בשורת הצעת מחיר של פרויקט, הכרטיסיה **קטגוריות הניתנות לחיוב** לא תהיה זמינה.

### <a name="update-a-project-task-to-be-chargeable-or-non-chargeable"></a>עדכן משימת פרויקט כניתנת לחיוב או כלא ניתנת לחיוב

משימת פרויקט יכולה להיות ניתנת לחיוב או לא ניתנת לחיוב בהקשר של שורת הצעת מחיר מבוססת פרויקט ספציפית, דבר המאפשר את הגדרה הבאה.

אם שורת הצעת מחיר מבוססת פרויקט כוללת **זמן** והמשימה **T1**, המשימה משויכת לשורת הצעת המחיר כניתנת לחיוב. אם יש שורת הצעת מחיר שניה שכוללת **הוצאות**, ניתן לשייך את המשימת **T1** בשורת הצעת המחיר כלא ניתנת לחיוב. התוצאה היא שכל הזמן שנרשם במשימה ניתן לחיוב וכל ההוצאות הנרשמות במשימה אינן ניתנות לחיוב.

ניתן להגדיר את סוג החיוב של משימה בכרטיסיה **משימות הניתנות לחיוב** של שורת הצעת מחיר מבוססת פרויקט על ידי עדכון השדה **סוג החיוב** ברשת המשנה של **משימות של שורת הצעת מחיר**. לחלופין, ניתן לעדכן את סוג החיוב עבור משימת פרויקט בשדה **סוג החיוב** ברשת המשנה של הגדרת חיוב משימה של פרויקט, שמציג את שורות הצעות המחיר המשויכות למשימה.

### <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a>עדכן תפקיד כניתן לחיוב או כלא ניתן לחיוב

תפקיד יכול להיות ניתן לחיות או לא ניתן לחייב בהקשר של שורת הצעת מחיר מבוססת פרויקט ספציפית.

ניתן להגדיר את סוג החיוב של תפיקד בכרטיסיה **תפקידים הניתנים לחיוב** של שורת הצעת מחיר על ידי עדכון השדה **סוג החיוב** ברשת המשנה של **תפקידים הניתנים לחיוב**.

### <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a>עדכן קטגוריית עסקאות כניתנת לחיוב או כלא ניתנת לחיוב

קטגוריה של עסקאות יכולה להיות ניתנת לחיוב או לא ניתנת לחייב בשורת הצעת מחיר ספציפית.

ניתן להגדיר את סוג החיוב של עסקה בכרטיסיה **קטגוריות הניתנות לחיוב** של שורת הצעת מחיר על ידי עדכון השדה **סוג החיוב** ברשת המשנה של **קטגוריות הניתנות לחיוב**.

### <a name="resolve-chargeability"></a>פתרון של יכולת חיוב
הערכה או נתונים בפועל שנוצרו עבור זמן נחשבים כניתנים לחיוב רק אם:

   - **זמן** כלול בסעיף הצעת מחיר.
   - **תפקיד** מוגדר כניתן לחיוב בסעיף הצעת מחיר.
   - **משימות כלולות** מוגדרות בתור **משימות נבחרות** בסעיף הצעת מחיר. 

אם שלושת הדברים הללו נכונים **המשימה** גם מוגדרת כניתנת לחיוב. 

הערכה או נתונים בפועל שנוצרו עבור הוצאה נחשבים כניתנים לחיוב רק אם: 

   - **הוצאה** כלולה בסעיף הצעת מחיר.
   - **קטגוריית עסקה** מוגדרת כניתנת לחיוב בסעיף הצעת מחיר.
   - **משימות כלולות** מוגדרות בתור **משימות נבחרות** בסעיף הצעת מחיר.

אם שלושת הדברים הללו נכונים **המשימה** גם מוגדרת כניתנת לחיוב. 

הערכה או נתונים בפועל שנוצרו עבור חומר נחשבים כניתנים לחיוב רק אם:

   - **חומרים** כלולים בסעיף הצעת מחיר.
   - **משימות כלולות** מוגדרות בתור **משימות נבחרות** בסעיף הצעת מחיר.

אם שני הדברים הללו נכונים, **המשימה** גם צריכה להיות מוגדרת כניתנת לחיוב. 


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
חיוב לפי נתוני זמן בפועל: ניתן לחיוב </p>
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
ניתן לחיוב </p>
            </td>
            <td width="350" valign="top">
                <p>
חיוב לפי נתוני זמן בפועל: ניתן לחיוב </p>
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
