---
title: לוחות זמנים של חשבוניות בשורת הצעת מחיר מבססת פרויקט
description: נושא זה מספק מידע על יצירת לוחות זמנים ואבני דרך של חשבוניות עבור שורות הצעת מחיר.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 0ecaf4d872873473b0e7fe3b08d62c6fe5af9c3d
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908193"
---
# <a name="invoice-schedules-on-project-based-quote-lines"></a>לוחות זמנים של חשבוניות בשורות הצעת מחיר מבססות פרויקט

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

שורת הצעת מחיר מבוססת פרויקט נותנת את היכולת לקבוע לוח זמנים של חשבונית. אפשרות זה אופציונלי בשלב הצעת המחיר מכיוון שהיישום אינו תומך בהפקת חשבונית עבור פרויקט כאשר הוא קשור לשורת הצעת מחיר. הפקת חשבוניות מותרת רק לאחר זכיית הצעת המחיר. ההשפעה היחידה במורד הזרם שיש ליצירת לוח זמנים של חשבוניות בשלב הצעת המחיר היא שלוח הזמנים של החשבוניות מועתק לסעיף החוזה מבוסס הפרויקט. אם לא יוצרים לוח זמנים של חשבוניות בשלב הצעת המחיר, אפשר לעשות זאת בסעיף החוזה מבוסס הפרויקט.

בסך הכל, המטרה של לוחות הזמנים של החשבוניות היא לאפשר יצירה אוטומטית של טיוטות של חשבוניות עבור סעיף חוזה מבוסס פרויקט. 

## <a name="create-a-time-and-material-invoice-schedule-for-a-project-based-quote-line"></a>יצירת לוח זמנים לחשבונית זמן וחומר עבור שורת הצעת מחיר מבוססת פרויקט

כאשר שיטת החיוב עבור שורת הצעת מחיר מבוססת פרויקט היא זמן וחומר, המערכת מייצרת לוח זמנים מבוסס תאריך של חשבוניות. להפקת אוטומתית של לוח זמנים מבוסס תאריך של חשבוניות, בצע את השלבים הבאים.

1. עבור אל **הגדרות** > **תדירויות של הגשת חשבונית** והגדר את תדירות הגשת חשבונית.
2. בדף **הצעות מחיר**, פתח את הצעת המחיר של הפרויקט ובכרטיסיה **סיכום** הכרטיסייה, הגדר תאריך ההגשה מבוקש.
3. פתח את שורת הצעת המחיר של זמן וחומרים שעבורה צריך ליצור לוח זמנים מבוסס תאריך של חשבונית. 
4. בכרטיסיה **לוח הזמנים של חשבוניות**, בחר ערכים בשדות **התחלת החיוב** ו**תדירות הגשת חשבוניות**. 
5. ברשת המשנה, בחר **צור לוח זמנים של חשבוניות**.
6. היישום מייצר את לוח הזמנים של החשבוניות עם השדות **תאריך הפעלת החשבונית**, **תאריך אחרון של העסקה**, ו**מצב ההפעלה**  מוגדרים בצורה הבאה:

    - **תאריך הפעלת החשבונית** מוגדר לתאריך המוכתב על ידי תדירות החשבונית.
    - **תאריך אחרון של העסקה** מוגדר ליום לפני **תאריך הרצת החשבונית**.
    - **מצב הפעלה** מוגדר אוטומטית ל**לא מופעל**. כאשר משימת יצירת החשבונית האוטומטית מופעלת עבור תאריך הפעלת חשבונית מסוים, היא תעדכן שדה זה או ל**ההפעלה הצליחה** או ל**ההפעלה נכשלה**.

## <a name="create-a-fixed-price-invoice-schedule-for-a-project-based-quote-line"></a>יצירת לוח זמנים לחשבונית מחיר עבור שורת הצעת מחיר מבוססת פרויקט

כאשר בשורת הצעת המחיר מבוססת הפרויקט משתמשת בשיטת חיוב **קבועה**, המערכת יוצרת לוח זמנים של חשבונית מבוסס אבן דרך. בצע את השלבים הבאים כדי ליצור אוטומטית לוח זמנים זה עבור קבוצה קבועה של אבני דרך המחולקות באופן שווה לאורך התקופה הקלנדרית.

1. עבור אל **הגדרות** > **תדירויות של הגשת חשבונית** והגדר את תדירות הגשת חשבונית.
2. בדף **הצעות מחיר**, פתח את הצעת המחיר של הפרויקט ובכרטיסיה **סיכום** הכרטיסייה, הגדר תאריך ההגשה מבוקש.
3. פתח את שורת הצעת המחיר של מחיר קבוע שעבורה צריך ליצור לוח זמנים של אבני דרך. 
4. בכרטיסיה **לוח הזמנים של חשבוניות**, בחר ערכים בשדות **התחלת החיוב** ו**תדירות הגשת חשבוניות**. 
5. ברשת המשנה, בחר **צור אבני דרך תקופתיות**.
6. היישום מייצר את לוח הזמנים של החשבוניות עם שם של אבן דרך, תאריך וסכום.

    - שם אבן הדרך מוגדר לתאריך המוכתב על ידי תדירות החשבונית.
    - תאריך אבן הדרך מוגדר לתאריך המוכתב על ידי תדירות החשבונית.
    - סכום אבן הדרך מחושב על ידי חלוקת סכום ההצעה בשורת הצעת המחיר מבוססת הפרויקט במספר אבני הדרך כפי שמוכתב על ידי התדירות, תאריך תחילת החיוב ותאריך ההגשה המבוקשים.
    - אם שורת הצעת המחיר כוללת גם סכום מס משוער, ערך זה מתחלק באופן שווה בין כל אבני הדרך בעת יצירת אבני דרך תקופתיות.

### <a name="manually-create-milestones"></a>יצירת אבני דרך באופן ידני

ניתן ליצור אבני דרך של מחיר קבוע גם באופן ידני כאשר הן אינן מפוצלות מעת לעת. ליצירת אבני דרך באופן ידני:

פתח את שורת הצעת המחיר של מחיר קבוע שבה צריך ליצור אבן דרך. ברשת המשנה של הכרטיסיה **לוח הזמנים של חשבוניות**, בחר **+ צור אבן דרך חדשה לשורת הצעת מחיר** והזן את המידע הנדרש לפי הטבלה הבאה.

| **שדה** | **מיקום** | **רלוונטיות, מטרה והכוונה** | **השפעה במורד הזרם** |
| --- | --- | --- | --- |
| שם אבן הדרך | יצירה מהירה | שם אבן הדרך. | מידע זה מופץ לאבן הדרך של סעיף החוזה של פרויקט ולחשבונית |
| משימת פרויקט | יצירה מהירה | אם אבן הדרך קשורה למשימת הפרויקט, באפשרותך להשתמש בהפניה זו כדי להגדיר את מצב אבן הדרך בהתבסס על מצב המשימה. | לאפליקציה אין השפעה במורד הזרם של הפניה זו למשימה. |
| תאריך אבן דרך | יצירה מהירה | הגדר את התאריך שבו על תהליך יצירת החשבונית האוטומטי לבצע חיפוש למצב אבן דרך זו כדי לשקול הפקת חשבונית עבורו. | מידע זה מופץ לאבן הדרך של סעיף החוזה של פרויקט ולחשבונית. |
| מצב חשבונית | יצירה מהירה | כאשר נוצרת אבן דרך, מצב זה מוגדר תמיד ל**לא מוכן להגשת חשבונית**. | מידע זה מופץ לאבן הדרך של סעיף החוזה של פרויקט ולחשבונית. |
| סכום סעיף | יצירה מהירה | סכום או ערך אבן הדרך שבו יחויב הלקוח. | מידע זה מופץ לאבן הדרך של סעיף החוזה של פרויקט ולחשבונית. |
| מס | יצירה מהירה | סכום המס שיוחל על אבן הדרך. | מידע זה מופץ לאבן הדרך של סעיף החוזה של פרויקט ולחשבונית. |