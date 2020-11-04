---
title: הגדרת תעריפי עלות ומכירות עבור הוצאות
description: נושא זה מספק מידע על הדרך להגדרת שיעורי עלות ומכירות עבור קטגוריות של הוצאות ועסקאות.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: e5a2402a2c1059ff11dbe1a331a028da77958235
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077227"
---
# <a name="set-up-cost-and-sales-rates-for-expenses"></a>הגדרת תעריפי עלות ומכירות עבור הוצאות

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

באפשרותך להגדיר מחירי עלות ומכירות עבור קטגוריות עסקאות ב- Dynamics 365 Project Operations. מכיוון שמחירי העלות והמכירות מיועדים להוצאות, יש להגדיר כל קטגוריית עסקאות הכוללת אותם גם כקטגוריית הוצאות. הגדרה זו מבטיחה דיוק בפונקציונליות במורד הזרם. מחירי עלות ומכירות לקטגוריות עסקאות יכולים להיות רשומים רק במטבע אחד, שעליו להיות המטבע בכותרת המחירון.

להגדרת עלויות ושיעורי מכירות עבור קטגוריות עסקאות, בצע את השלבים הבאים. 

1. צור מחירון על בסיס כותרת המחירון. 
2. ב **מחירי קטגוריות** , בתפריט רשת המשנה, בחר **+ מחיר קטגוריה חדש**. 
3. בדף **יצירה מהירה** , הזן את קטגוריית העסקה ואת היחידה שעבורה אתה יוצר את המחיר החדש.

הטבלה הבאה מפרטת את השדות בכרטיסיה **כללי** ובדף **יצירה מהירה** בשורת מחירים של קטגוריות שכדאי לקחת בחשבון בעת יצירת מחירי קטגוריות במחיר מכירות או במחירון.

| שדה | מיקום | רלוונטיות, מטרה והכוונה | השפעה במורד הזרם |
| --- | --- | --- | --- |
| קטגוריית עסקה | הכרטיסיה **כללי** ודפי **יצירה מהירה** | בחר את קטגוריית העסקאות שאתה יוצר לה מחיר מכירות או עלות. | קטגוריית העסקאות בהערכה או בנתון בפועל שנכנסים תותאם לשורה זו כדי להגדיר כברירת מחדל את תעריף עלות המכירות. |
| לוח זמני יחידה | הכרטיסיה **כללי** ודפי **יצירה מהירה** | ברירת המחדל של לוח הזמנים ליחידה מתזמון היחידות בקטגוריית העסקה. | אין השפעה במורד הזרם משדה זה. |
| יחידה | הכרטיסיה **כללי** ודפי **יצירה מהירה** | בחר את היחידה שלגביה מוגדרים התעריפים. | היחידה בהערכת האומדן הנכנס או בפועל תואמת ליחידה בשורה זו כדי להגדיר את ברירת המחדל באומדן ההוצאות או בפועל. |
| שיטת תמחור | הכרטיסיה **כללי** ודפי **יצירה מהירה** | ערכים אפשריים של השדה **שיטת תמחור** הם **מחיר ליחידה** , **במחיר** , ו **ייקור מעל לעלות**. | במהלך הגדרת המחיר, בחירה של **מחיר ליחידה** נועלת את השדה **אחוז** בשורת מחיר הקטגוריה. אם נבחר **במחיר** , השדות **מחיר** ו **אחוּז** נעולים במחירון המכירות. בחירה של **ייקור מעל לעלות** נועלת את השדה **מחיר** במחירון המכירות. בשורה של נתון בפועל נכנס להוצאות, שיטת תמחור של **במחיר** או **ייקור מעל לעלות** מביאה לכך ששורת המכירות המקבילה ללא חיוב משויכת למחיר השווה למחיר העלות בפועל או מחושבת כייקור מעל לעלות. |
| מחיר | הכרטיסיה **כללי** ודפי **יצירה מהירה** | הגדר תעריף ליחידה עבור קטגוריית העסקה ושילוב היחידות. לדוגמה, הקילומטראז' הוא 10 דולר למייל ו- 8 דולר לקילומטר. | הקילומטראז' הוא התעריף שמוגדר כברירת מחדל של עלות ליחידה או המחיר של שורת ההערכה או הנתון בפועל הנכנסים עבור סיווג העסקה כהוצאה.|
| אחוז | הכרטיסיה **כללי** ודפי **יצירה מהירה** | הגדר עלות באחוזים עבור קטגוריית העסקה ושילוב היחידות. לדוגמה, יש לסמן את שיעור מכירות כרטיסי הטיסה בכ- 10 אחוז מעלות הוצאות כרטיסי הטיסה. | אחוז זה של תוספת על העלות חל רק על מחירון המכירות כאשר שיטת חישוב המחיר שנבחרה היא **ייקור מעל לעלות**. |
| מטבע | הכרטיסיה **כללי** ודפי **יצירה מהירה** | כברירת מחדל, ערך זה מגיע מהשדה מטבע שבכותרת המחירון. בתמחור קטגוריות עסקאות לא ניתן לבטל את המטבע. | מטבע זה מוגדר כברירת מחדל לפי המחיר ליחידה של שורת הנתון בפועל הנכנסת עבור סיווג העסקה הוצאות לעלות ולמכירות. |

## <a name="pricing-methods-for-expenses"></a>שיטות תמחור להוצאות

כאשר אתה מגדיר מחירי קטגוריות שרלוונטיים רק בהקשר של תמחור הוצאות, תוכל להשתמש באחת משלוש שיטות התמחור הבאות:

- **מחיר ליחידה**
- **לפי עלות**
- **ייקור של עלות**

### <a name="price-per-unit"></a>מחיר ליחידה
כאשר נבחרת שיטת תמחור זו בשורת מחירים של קטגוריות המקושרת למחירון מכירות, ברירת המחדל של המחיר היא שילוב הקטגוריות והיחידות הן באומדן והן בפועל. ההערכה מתייחסת לסעיפי ההערכה של הפרויקט מבחינת הוצאות, לפרטי השורות בהצעת המחיר ולסעיף החוזה של ההוצאות.

### <a name="at-cost"></a>לפי עלות
כאשר נבחרת שיטת תמחור זו בשורת מחירים של קטגוריות המקושרת למחירון מכירות, ברירת המחדל של המחירון היא שילוב רק עבור ההוצאות בפועל. לדוגמה, נתוני מכירות שלא חויבו עבור מחלקת עסקאות ההוצאות. מחיר היחידה נקבע בנתונים בפועל של מכירות שטרם חויבו ממחיר היחידה של העלות בפועל עבור אותה הוצאה. ברירת מחדל של מחיר שמבוססת על עלות אינה מתבצעת על פי הערכות הפרויקט להוצאות או שורת הצעת המחיר ופרטי סעיף החוזה להוצאות.

### <a name="markup-over-cost"></a>ייקור של עלות
כאשר נבחרת שיטת תמחור זו בשורת מחירים של קטגוריות המקושרת למחירון מכירות, ברירת המחדל של המחירון היא שילוב רק עבור ההוצאות בפועל. לדוגמה, נתוני מכירות שלא חויבו עבור מחלקת עסקאות ההוצאות. מחיר יחידה זה נקבע על פי מכירות בפועל שלא חויבו לפי ערך מחושב ממחיר היחידה בעלות בפועל עבור אותה הוצאה לאחר החלת אחוז הייקור שהוגדר. ברירת מחדל של מחיר שמבוססת על עלות אינה מתבצעת על פי הערכות הפרויקט להוצאות או שורת הצעת המחיר ופרטי סעיף החוזה להוצאות.