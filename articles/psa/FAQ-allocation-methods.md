---
title: שיטות הקצאת הזמנות ב-Project Service Automation
description: נושא זה מספק מידע אודות הדרכים השונות שבהן באפשרותך להזמין הקצאות.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 295da428ce15e7775450dfa94e96047f200bdede
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077302"
---
# <a name="booking-allocation-methods-in-project-service-automation"></a>שיטות הקצאת הזמנות ב-Project Service Automation

בין אם אתה מוסיף חבר צוות ישירות לפרויקט בכרטיסיה **צוות** , או מזמין משאב לפרויקט או דרישה מלוח הזמנים, קיימות כמה שיטות שונות להקצאת הזמנה שניתן להשתמש בהן. נושא זה מסביר כיצד פועלת כל שיטה ואילו שיטות עלול לגרום להזמנת יתר של משאבים.

## <a name="full-capacity"></a>קיבולת מלאה 
השיטה 'קיבולת מלאה' מזמינה קיבולת מלאה של המשאב עבור התאריכים 'מ' ו'עד' שצוינו. לדוגמה, אם למשאב יש לוח שנה שמוגדר לעבודה שמונה שעות ביום, חמישה ימים בשבוע, הגדרת תאריך התחלה וסיום המכסה חמישה ימי עבודה תזמין את המשאב ל- 40 שעות. ההזמנה מתבצעת ללא קשר לקיבולת הנותרת של משאב. אם משאב מוזמן כבר במהלך תקופה זו לפרוייקטים אחרים, 40 השעות מוזמנות כשעות נוספות, מה שעלול להוביל להזמנות יתר.

## <a name="remaining-capacity"></a>קיבולת שנותרה
השיטה 'קיבולת שנותרה' זמינה רק כאשר אתה מזמין ישירות אל פרוייקט באמצעות לוח הזמנים. שיטה זו מזמינה את הקיבולת הזמינה של משאב בטווח התאריכים שצוין. לדוגמה, אם למשאב יש קיבולת של 40 שעות שבועיות, והוא כבר הוזמן ל- 10 שעות, הזמנה עבור אותו שבוע מזמינה את המשאב ל- 30 השעות הנותרות בקיבולת לשבוע זה.

## <a name="percentage-capacity"></a>קיבולת באחוזים
השיטה 'קיבולת באחוזים' מזמינה את המשאב לאחוז הקיבולת עבור התאריכים 'מ' ו'עד' שצוינו. לדוגמה, אם למשאב יש לוח שנה שמוגדר לעבודה שמונה שעות ביום, חמישה ימים בשבוע, הגדרת תאריך התחלה וסיום המכסה חמישה ימי עבודה בקיבולת של 50% תזמין את המשאב ל- 20 שעות. ההזמנות הנפרדות ליום נפרסות באופן שווה על-פני התקופה, ארבע שעות ביום בדוגמה זו. ההזמנה מתבצעת ללא קשר לקיבולת הנותרת של משאב. אם המשאב מוזמן כבר במהלך תקופה זו לפרוייקטים אחרים, 20 השעות מוזמנות כשעות נוספות, מה שעלול להוביל להזמנות יתר.

## <a name="evenly-distribute-hours"></a>הפצת שעות באופן שווה
השיטה '‏‫הפצת שעות באופן שווה'‬ מזמינה את המשאב למספר מסוים של שעות, ומפיצה את הזמן באופן שווה בכל יום בטווח התאריכים 'מ'/'עד' שצוינו. לדוגמה, אם אתה מזמין משאב עבור 20 שעות במשך תקופה של חמישה ימים, שיטה זו תפזר את 20 השעות באופן שווה לארבע שעות ביום. ההזמנה מתבצעת ללא קשר לקיבולת הנותרת של משאב. אם המשאב מוזמן כבר במהלך תקופה זו לפרוייקטים אחרים, 20 השעות מוזמנות כשעות נוספות, מה שעלול להוביל להזמנות יתר.

## <a name="front-load-hours"></a>שעות עומס חזיתי
השיטה 'שעות עומס חזיתי' מזמינה את המשאב למספר מסוים של שעות, ומחלקת את השעות ביום לפי עומס חזיתי בטווח התאריכים 'מ' ו'עד' שצוינו. חלוקה לפי עומס חזיתי צורכת את הקיבולת זמינה של משאב בסדר "ראשון-בראשון-שנצרך". לדוגמה, אם זמני העבודה של משאב הם שמונה שעות ביום, חמישה ימים בשבוע, ואין לו הזמנות נוכחיות, הזמנת המשאב ל- 20 שעות לאורך תקופה של חמישה ימי עבודה תביא לדפוס ההזמנה היומי הבא: 

|         הזמנות          |    יום 1    |    יום 2    |    יום 3    |    יום 4    |    יום 5    |    סה''כ    |
|---------------------------|-------------|-------------|-------------|-------------|-------------|-------------|
|    הזמנות קיימות    |    1        |    1        |    1        |    1        |    1        |    1        |
|    הזמנה חדשה          |    8        |    8        |    4        |    0        |    0        |    20       |

שיטת העומס הקדמי מתחשבת בהזמנות קיימות ובקיבולת זמינה. לדוגמה, אם לאותו משאב יש כבר 20 שעות של הזמנות בשבוע העבודה, ההזמנות החדשות צורכות את הקיבולת הנותרת כדלקמן:

|   הזמנות          | יום 1 | יום 2 | יום 3 | יום 4 | יום 5 | סה''כ |
|---------------------|-------|-------|-------|-------|-------|-------|
| הזמנות קיימות | 8     | 8     | 4     | 1     | 1     | 20    |
| הזמנה חדשה       | 0     | 0     | 4     | 8     | 8     | 20    |

מאחר שהשיטה מתחשבת בקיבולת זמינה, ייתכן שתקבל הודעת שגיאה אם למשאב אין קיבולת נותרת שניתן לספוג בהזמנה. בשיטה זו לא ניתן ליצור הזמנת יתר.

## <a name="none"></a>ללא
השיטה 'ללא' זמינה רק בעת הזמנה מהכרטיסיה **צוות** בפרויקט. שיטה זו מוסיפה את המשאב בתור חבר בצוות הפרויקט, אך אינה יוצרת הזמנות כלשהן אשר סופגות את קיבולת המשאב. שיטה זו משמשת כאשר חבר צוות המשמש כמנהל פרויקט בברירת המחדל מתווסף בעת יצירת פרויקט. משתמש שהוא מנהל הפרויקט שיצר את הפרויקט מתווסף כברירת מחדל לפרויקט, כך שלרשומת ישות של הפרויקט יש בעלים וקיים מאשר אחד בפרויקט. מאחר שלמשתמש זה אין הזמנות כלשהן, אם ברצונך להזמין את המשאב, באפשרותך למחוק ולהוסיף אותו מחדש באמצעות שיטת הקצאה אחרת, או להוסיף את המשאב למשימות ולאחר מכן להשתמש ב **הזמנות מורחבות** בכרטיסיה **פיוס** ליצירת הזמנות עבור ההקצאות.

## <a name="allocation-methods-that-lead-to-overbooking"></a>שיטות הקצאה שמובילות להזמנת יתר
לסיכום, שיטות ההקצאה הבאות מובילות להזמנת יתר אם המשאב כבר מחויב בפרויקטים אחרים (או עבור הזמנות עבודה אחרות או ישויות אחרות הניתנות לתזמון):

- קיבולת מלאה
- קיבולת באחוזים
- הפצת שעות באופן שווה

בעת שימוש באחת משלוש שיטות ההקצאה הללו, לא תקבל הודעה בעת הזמנת יתר של משאב. כדי לתקן את הזמנת היתר, יהיה עליך להשתמש בלוח הזמנים.