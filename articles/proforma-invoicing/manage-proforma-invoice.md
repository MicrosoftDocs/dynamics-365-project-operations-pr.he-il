---
title: ניהול חשבונית פרופורמה
description: נושא זה מספק מידע על אופן ניהול העבודה עם חשבוניות פרופורמה.
author: rumant
manager: Annbe
ms.date: 10/27/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 2f3aab57f159dbb522ebe5d24dc3693034f6f81f
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181453"
---
# <a name="manage-a-proforma-invoice"></a>ניהול חשבונית פרופורמה

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

ב-Dynamics 365 Project Operations, חשבוניות פרופורמה נבנות כהרחבה לחשבוניות ב-Dynamics 365 Sales. עם זאת, ישנם הבדלים רבים בתהליך הפקת החשבונית בין Sales ל-Project Operations בכל הנוגע להפקת חשבוניות. לדוגמה, לא ניתן ליצור חשבונית חדשה מהדף **רשימת חשבוניות** ב-Project Operations, אך ניתן לעשות זאת ב-Sales. הבדלים והרחבות אלה קיימים כדי לתמוך בתהליכי הפקת חשבוניות לפרויקטים ששונים מחשבונית אופיינית של הזמנת מכירה.

> [!IMPORTANT]
> בגלל ההבדלים, אין להשתמש בחשבוניות ב-Sales וב-Project Opertitions בצורה חליפית.

## <a name="invoice-header"></a>כותרת חשבונית

המידע הבא זמין בכותרת חשבונית פרופורמה ב-Project Operations.

| שדה | מיקום | תיאור | השפעה במורד הזרם |
| --- | --- | --- | --- |
| **מזהה חשבונית** | כרטיסיית **סיכום** | המזהה שנוצר באופן אוטומטי בעת יצירת חשבונית פרופורמה. שדה לקריאה בלבד שנעול לעריכה. | שדה זה משמש כהפניה לכל חשבונית פרופורמה. |
| **שם** | כרטיסיית **סיכום** | מוגדר לשם חוזה הפרויקט כברירת מחדל. המשתמש יכול לערוך שדה זה. | &nbsp;  |
| **מטבע** | כרטיסיית **סיכום** | מוגדר למטבע חוזה הפרויקט כברירת מחדל. שדה לקריאה בלבד שנעול לעריכה. |&nbsp; |
| **מחירון** | כרטיסיית **סיכום** | מוגדר מחירון חוזה הפרויקט כברירת מחדל. שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **הזדמנות** | כרטיסיית **סיכום** | ההפנייה להזדמנות המקושרת. שדה לקריאה בלבד שנעול לעריכה. | &nbsp;  |
| **חוזה** | כרטיסיית **סיכום** | ההפנייה לחוזה הפרויקט המקושר. שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **לקוח** | כרטיסיית **סיכום** | ההפנייה לחוזה הפרויקט המקושר. שדה לקריאה בלבד שנעול לעריכה. |&nbsp;  |
| **תיאור** | כרטיסיית **סיכום** | שדה הטקסט המתאר את החשבונית. המשתמש יכול לערוך שדה זה. | &nbsp; |
| **לחיוב** ושדות קשורים | **כרטיסיית סיכום** | ברירות המחדל נקבעות מלקוח חוזה הפרויקט. המשתמש יכול לערוך שדה זה.  | &nbsp; |
| **מצב** | כרטיסיית **סיכום** | מגדיר את האפשרויות הבאות: **פעיל**, **סגור**, **שולם**, ו **מבוטל**, וניתן לעריכה על ידי המשתמש. | מצבים לא נתמכים עבור פעולות פרויקט כוללים **סגור** ו **מבוטל**. </br> המצב מוגדר ל **פעיל** כאשר נוצרת החשבונית. </br>יש להגדיר את המצב ל **שולם** רק לאחר אישור החשבונית. |
| **מצב חשבונית פרויקט** | כרטיסיית **סיכום** | מגדיר את האפשרויות הבאות: **טיוטה**, **בבדיקה** ו **מאושר**, וניתן לעריכה על ידי המשתמש. | בשני המצבים **טיוטה** ו **בבדיקה**, ניתן לערוך את החשבונית. לא ניתן לערוך את החשבונית לאחר אישורה. |
| **סכום מפורט** | כרטיסיית **סיכום** | סך הסכומים בכל שורות החשבונית לאחר מקדמות במזומן וניכויים. שדה לקריאה בלבד שנעול לעריכה. | שדה זה משמש לחישוב הסכום הסופי. |
| **הנחה (%)** | כרטיסיית **סיכום** | ניתן לערוך שדה זה כדי להזין אחוזי הנחה. שדה זה אינו נתמך על ידי הפונקציונליות של Project Operations. | זהו שדה שאינו נתמך. |
| **סכום הנחה** | כרטיסיית **סיכום** | ניתן לערוך שדה זה כדי להזין את סכום ההנחה. שדה זה אינו נתמך על ידי הפונקציונליות של Project Operations. | זהו שדה שאינו נתמך. |
| **סכום לפני עלויות הובלה** | **כרטיסיית סיכום** | סכום החשבונית הכולל לאחר החלת ההנחות. שדה לקריאה בלבד שנעול לעריכה. | שדה זה משמש לחישוב הסכום הסופי. |
| **סכום הובלה** | כרטיסיית **סיכום** | ניתן לערוך שדה זה כדי להזין את סכום ההובלה. שדה זה אינו נתמך על ידי הפונקציונליות של Project Operations. | זהו שדה שאינו נתמך. |
| **סה''כ מס** | כרטיסיית **סיכום** | המס הכולל מכל שורות החשבונית שבחשבונית. שדה לקריאה בלבד שנעול לעריכה. | ללא. |
| **סכום כולל** | כרטיסיית **סיכום** | סך הסכום לאחר הנחות ומסים. | הסך הוא הסכום שהלקוח צריך לשלם. |

## <a name="project-based-invoice-lines"></a>שורות חשבינית מבוססות פרוייקט

ב-Project Operations, יש תמיד שורת חשבונית אחת לכל סעיף חוזה פרויקט. שורת החשבונית נוצר גם אם אין נתונים בפועל. המידע הבא זמין בשורת חשבונית פרופורמה.

| שדה | מיקום | תיאור | השפעה במורד הזרם |
| --- | --- | --- | --- |
| **מזהה חשבונית** | כרטיסיה **כללי** | הפנייה למזהה החשבונית. שדה לקריאה בלבד שנעול לעריכה. | ניתן להשתמש בקישור מזהה החשבונית כדי לנווט חזרה לכותרת החשבונית. |
| **שם** | כרטיסיה **כללי** | שם שורת החשבונית שהוגדר כברירת מחדל משם שורת החוזה. המשתמש יכול לערוך שדה זה. | &nbsp; |
| **פרויקט** | כרטיסיה **כללי** | הפרויקט בסעיף חוזה הפרויקט הקשור. שדה לקריאה בלבד שנעול לעריכה. | ניתן להשתמש בקישור הפרויקט כדי לנווט אל הפרויקט. |
| **שיטת חיוב** | כרטיסיה **כללי** | שיטת החיוב בסעיף חוזה הפרויקט הקשור. שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **סכום בסעיף חוזה** | כרטיסיה **כללי** | סכום שסוכם עליו בסעיף חוזה הפרוייקט הקשור. שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **הוגשה חשבונית עד ליום** | כרטיסיה **כללי** | סך הסכומים בכל פרטי שורת החשבונית של חשבונית זו. שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **סכום** | כרטיסיה **כללי** | סך הסכומים בכל פרטי שורת החשבונית הניתנים לחיוב של חשבונית זו. שדה לקריאה בלבד שנעול לעריכה. | שדה זה משמש לחישוב הסכום בכותרת החשבונית. |
| **מס** | כרטיסיה **כללי** | סך הסכומי המס בכל פרטי שורת החשבונית של שורת חשבונית זו. שדה לקריאה בלבד שנעול לעריכה. | שדה זה משמש לחישוב סכום המס הסופי בכותרת החשבונית. |
| **סכום מורחב** | כרטיסיה **כללי** | סך הסכומים הכוללים (**מס + סכומים**) בכל פרטי שורת החשבונית הניתנים לחיוב של שורת חשבונית זו. שדה לקריאה בלבד שנעול לעריכה. | שדה זה משמש לחישוב הסכום בכותרת החשבונית. |

## <a name="invoice-line-details"></a>פרטי שורת החשבונית

כל שורת חשבוניות בחשבונית פרויקט כוללת פרטי שורת חשבונית. פרטי שורה אלו קשורים ניתונים בפועל של המכירות ואבני דרך שלא חויבו הקשורים לקו החוזה אליו מפנה שורת החשבונית. כל העסקאות הללו מסומנות כ **מוכן להפקת חשבונית**.

עבור שורת **חשבונית זמן וחומרים**, פרטי שורת החשבונית מקובצים ל **ניתנים לחיוב**, **אינם ניתנים לחיוב**, ו **ללא תשלום** בדף של **שורת חשבונית**. הפרטים של **שורת חשבונית הניתנת לחיוב** מסתכמים לסך הכל של שורת החשבונית. פרטים **לא לתשלום** ו **נתונים בפועל שאינם ניתנים לחיוב** אינם מתווספים לסך שורת החשבונית.

עבור השורה של **חשבונית מחיר קבוע**, פרטי שורת החשבונית נוצרים מאבני דרך המסומנות כ **מוכן להפקת חשבונית** בסעיף החוזה הקשור. לאחר יצירת פרט שורת החשבונית מאבן דרך, מצב החיוב באבן דרך מתעדכן ל **חשבונית הלקוח נוצרה**.

### <a name="edit-invoice-line-details"></a>עריכת פרטי שורת חשבונית

השדות הבאים זמינים בפרט שורת החשבונית שמגובה על ידי נתון בפועל של מכירות שלא חויב.

| שדה | תיאור | השפעה במורד הזרם |
| --- | --- | --- |
| **שורת חשבונית** | הפנייה ל **מזהה שורת החשבונית**. שדה לקריאה בלבד, נעול לעריכה. | ניתן להשתמש בקישור זה כדי לנווט חזרה לכותרת החשבונית. |
| **תיאור** | תיאור של פרט שורת החשבונית. מוגדר כברירת מחדל מהשדה **הערות פנימיות** ב **ערך זמן**, ומהשדה **תיאור** ב **ערך הוצאות**. המשתמש יכול לערוך שדה זה.| &nbsp; |
| **תיאור חיצוני** | תיאור של פרט שורת החשבונית. מוגדר כברירת מחדל מהשדה **הערות חיצוניות** ב **ערך זמן**, ומהשדה **תיאור** ב **ערך הוצאות**. המשתמש יכול לערוך שדה זה. | ניתן להשתמש בתיאור זה כדי לקבוע מה צריך להיות בחשבונית המודפסת שתישלח ללקוח. ב-Project Operations, לחשבונית פרופורמה אין את כל הפונקציונליות הנדרשת להגדרת הגדרות הדפסה עבור חשבונית. |
| **תאריך התחלה** | מוגדר כברירת מחדל מהנתון בפועל מקור. שדה לקריאה בלבד שנעול לעריכה. | ניתן לערוך שדה זה בפרט שורת חשבוניות חדש שאינו מגובה על ידי נתון בפועל מקור. |
| **פרויקט** | מוגדר כברירת מחדל מהנתון בפועל מקור. שדה לקריאה בלבד שנעול לעריכה. | מוגדר כברירת מחדל לפרויקט בסעיף החוזה הקשור. |
| **משימה** | מוגדר כברירת מחדל מהנתון בפועל מקור. שדה לקריאה בלבד שנעול לעריכה. | השדה ניתן לעריכה בפרט שורת חשבוניות חדש שאינו מגובה על ידי נתון בפועל מקור. רשימה נפתחת מציגה את כל המשימות המשויכות לסעיף חוזה הפרויקט הקשור.  |
| **קטגוריית עסקה** | מוגדר כברירת מחדל מהנתון בפועל מקור. שדה לקריאה בלבד שנעול לעריכה. | השדה ניתן לעריכה בפרט שורת חשבוניות חדש שאינו מגובה על ידי מקור של נתון בפועל. |
| **תפקיד** | מוגדר כברירת מחדל מהנתון בפועל מקור. שדה לקריאה בלבד שנעול לעריכה. | השדה ניתן לעריכה בפרט שורת חשבוניות חדש שאינו מגובה על ידי נתון בפועל מקור. |
| **משאב הניתן להזמנה** | מוגדר כברירת מחדל מהנתון בפועל מקור. שדה לקריאה בלבד שנעול לעריכה. | השדה ניתן לעריכה בפרט שורת חשבוניות חדש שאינו מגובה על ידי מקור של נתון בפועל. |
| **החברה של הקצאת המשאבים** | מוגדר כברירת מחדל מהנתון בפועל מקור. שדה לקריאה בלבד שנעול לעריכה. | השדה ניתן לעריכה בפרט שורת חשבוניות חדש שאינו מגובה על ידי נתון בפועל מקור. |
| **יחידת הקצאת משאבים** | מוגדר כברירת מחדל מהנתון בפועל מקור. שדה לקריאה בלבד שנעול לעריכה. | השדה ניתן לעריכה בפרט שורת חשבוניות חדש שאינו מגובה על ידי נתון בפועל מקור. |
| **כמות** | מוגדר כברירת מחדל מהנתון בפועל מקור. שדה לקריאה בלבד שנעול לעריכה. | השדה ניתן לעריכה בפרט שורת חשבוניות חדש שאינו מגובה על ידי נתון בפועל מקור. |
| **לוח זמני יחידה** | לפרטי שורת חשבונית לזמן, זה תמיד מוגדר לזמן ולא ניתן לעריכה. עבור הוצאות, זה מוגדר כברירת מחדל מהנתון בפועל של הוצאות המקור. שדה לקריאה בלבד שנעול לעריכה. | מוגדר כברירת מחדל ל **זמן** הפרט שורת חשבוניות חדש שאינו מגובה בנתון בפועל. |
| **יחידה** | מוגדר כברירת מחדל מהנתון בפועל מקור. שדה לקריאה בלבד שנעול לעריכה. | השדה ניתן לעריכה בפרט שורת חשבוניות חדש שאינו מגובה על ידי נתון בפועל מקור |
| **מחיר** | מוגדר כברירת מחדל מהנתון בפועל מקור. שדה לקריאה בלבד שנעול לעריכה. | השדה ניתן לעריכה בפרט שורת חשבוניות חדש שאינו מגובה על ידי נתון בפועל מקור. אם לא הוזן שום ערך, הוא מוגדר כברירת מחדל לאחר **שמירה**. |
| **מטבע** | מוגדר כברירת מחדל מהנתון בפועל מקור. שדה לקריאה בלבד שנעול לעריכה. | מוגדר כברירת מחדל מכותרת החשבונית בעת יצירת פרט חשבונית חדש ללא גיבוי של נתון בפועל.  שדה לקריאה בלבד שנעול לעריכה. |
| **סכום** | מוגדר כברירת מחדל מהנתון בפועל מקור. שדה לקריאה בלבד שנעול לעריכה. | מחושב כ **כמות\*מחיר** בעת יצירת פרט חשבונית חדש ללא גיבוי של נתון בפועל. מחושב לאחר **שמירה**. שדה לקריאה בלבד שנעול לעריכה. |
| **מס** | מוגדר כברירת מחדל מהנתון בפועל מקור. המשתמש יכול לערוך שדה זה | המשתמש יכול לערוך את השדה בעת יצירת פרט שורת חשבונית חדש ללא גיבוי של נתון בפועל. |
| **סכום מורחב** | שדה מחושב, המחושב כ **סכום + מס**. שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **סוג חיוב** | מוגדר כברירת מחדל מהנתון בפועל מקור. המשתמש יכול לערוך שדה זה. | בחירה ב **חיוב** מוסיף את השורה לסך כל שורת החשבונית. **ללא תשלום** ו **לא ניתן לחיוב** יגרמו לכך שלא יכלל בסכום שורת החשבוניות. |
| **סוג עסקה** | מוגדר כברירת מחדל מהנתון בפועל מקור. שדה לקריאה בלבד שנעול לעריכה. | מוגדר כברירת מחדל ל **מכירות שחויבו** וננעל בעת יצירת **פרט שורת חשבונית** חדש ללא נתון בפועל מגבה.  |
| **מחלקת עסקאות** | מוגדר כברירת מחדל מהנתון בפועל מקור. שדה לקריאה בלבד שנעול לעריכה. | מוגדר כברירת מחדל על סמך בחירת המשתמש ליצור פרט שורת חשבונית של **זמן**, **הוצאה**, או **עמלה** תוך יצירת **פרט שורת חשבונית** ללא נתון בפועל מגבה. נעול לעריכה. |

השדות הבאים זמינים בפרט שורת חשבונית שמגובה על ידי אבן דרך:

| שדה | תיאור | השפעה במורד הזרם |
| --- | --- | --- |
| **שורת חשבונית** | הפנייה ל **מזהה שורת החשבונית**. שדה לקריאה בלבד שנעול לעריכה. | ניתן להשתמש בקישור כדי לנווט חזרה לכותרת החשבונית. |
| **תיאור** | תיאור של פרט שורת החשבונית. מוגדר כברירת מחדל מתיאור אבן הדרך המקור. | &nbsp; |
|**תיאור חיצוני** | תיאור פרט שורת החשבונית המוגדר כברירת מחדל מתיאור אבן דרך המקור. | ניתן להשתמש בשדה זה כדי לקבוע מה צריך להיכלל בחשבונית המודפסת שתישלח ללקוח. לחשבונית פרופורמה ב-Project Operations אין את כל הפונקציונליות הנדרשת להגדרת הגדרות הדפסה עבור חשבונית. |
| **תאריך התחלה** | מוגדר כברירת מחדל מתאריך **אבן הדרך**  שבאבן דרך המקור. שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **פרויקט** | מוגדר כברירת מחדל מאבן דרך המקור. שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **משימה** | מוגדר כברירת מחדל מאבן דרך המקור. שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **קטגוריית עסקה** | שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **תפקיד** | שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **משאב הניתן להזמנה** | שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **יחידת הקצאת משאבים** | שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **לוח זמני יחידה** | שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **יחידה** | שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **מחיר** | מוגדר כברירת מחדל מהסכום באבן הדרך המקור. שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **מטבע** | מוגדר כברירת מחדל מאבן דרך המקור. שדה לקריאה בלבד שנעול לעריכה. |&nbsp; |
| **סכום** | מוגדר כברירת מחדל מהסכום באבן הדרך המקור. שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **מס** | מוגדר כברירת מחדל מהסכום המס באבן הדרך המקור. שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **סכום מורחב** | מוגדר כברירת מחדל מהסכום המורחב באבן הדרך המקור. המשתמש יכול לערוך שדה זה | &nbsp; |
| **סוג חיוב** | תמיד מוגדר כברירת מחדל ל **ניתן לחיוב**. שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **סוג עסקה** | מוגדר כברירת מחדל מאבן דרך המקור. שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |
| **מחלקת עסקאות** | מוגדר כברירת מחדל מאבן דרך המקור. שדה לקריאה בלבד שנעול לעריכה. | &nbsp; |

## <a name="refresh-invoice-transactions"></a>רענון עסקאות חשבונית

אם קיימים ניתונים בפועל שנכנסו לאחר יצירת החשבונית, ניתן לכלול נתונים בפועל אלה בחשבונית.

1. ב **תצוגת מצבור פרטי עבודה של חיוב**, סמן את הנתונים כ **מוכן להפקת חשבונית**.   
2. פתח את טיוטת חשבונית הפרופורמה ועל רצועת הכלים **פעולות** לחץ על **רענן עסקאות של שורת חשבוניות**.

  פעולה זו יוצרת פרטי שורת חשבונית עבור כל נתון בפועל שהתאריך שלו עבר ושמסומן כ **מוכן להפקת חשבונית**, אך אינו כלול בחשבונית.