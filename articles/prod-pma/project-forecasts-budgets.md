---
title: תחזיות פרויקטים ותקציבים
description: Microsoft Dynamics 365 Finance מספק תחזיות לפרויקטים ותקציבים לפרויקטים לניהול הפרויקטים ולביצוע בקרה עליהם.
author: Yowelle
manager: AnnBe
ms.date: 10/25/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ForecastModel, ProjYearEndProcess
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 23501
ms.assetid: 4e6d1384-19a2-4232-b3f3-d2590c218bd7
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: f99c00effbb0678f1f55e5068a7128cbfb86f5ce
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077421"
---
# <a name="project-forecasts-and-budgets"></a>תחזיות פרויקטים ותקציבים

[!include [banner](../includes/banner.md)]

ישנן שתי דרכים לניהול ובקרה של הפרויקטים שלך: תחזיות פרויקטים ותקציבי פרויקטים. 

השתמש בחיזוי לפרויקט אם לארגון שלך יש נקודת מבט תפעולית, ואם הוא מתמקד בהכנסות ובעלויות שמקורן בעסקאות ספציפיות. השתמש בתקצוב פרויקט אם הארגון מתמקד יותר בסכומים כספיים. 

תחזיות לפרויקטים ותקציבי פרויקטים משתמשים במודלי תחזית כדי לאסחן את סכומי העסקאות החזויים. 

לכל שיטה יתרונותיה. עליך לשקול את הנקודות הבאות לפני שתבחר שיטה לארגון.

|   שיטת הקצאה       |           חיזוי פרויקטים            |        תקצוב פרויקט                           |
|---------------------------|------------------------------------------|----------------------------------------------------|
| **הקצאת תקופה**     | אינך יכול להקצות במפורש עסקאות במהלך תקופת כספים. במקום זאת, התחזית והבקרה על התחזית מבוססים על חיי הפרויקט. מכיוון שתחזיות מבוססות על תאריך ספציפי, עליך להסיק את התקופה מהתאריך. | באפשרותך להקצות עסקאות במהלך הפרויקט כולו או תקופת כספים. אם אתה מקצה לאורך תקופה, תוכל להעביר סכומים שאינם בשימוש קדימה לתקופת הכספים הבאה. |
| **הצגת עסקאות**  | תוכל להציג עסקאות בטופסי התחזית, שבהם ניתן לראות את התחזיות עבור כל החברה ולכל הפרויקטים, ללא קשר להירארכיה. כדי להתמקד בפרויקט מסוים, עליך לסנן את הנתונים.                                       | באפשרותך להציג עסקאות מתוקצבות עבור הירארכיית פרויקט אחת. לכן, באפשרותך להציג פרטי עסקה עבור פרויקט אב או את פרויקטי המשנה שלו.                 |
| **משתני עסקה** | בעת הזנת עסקאות תחזית, תוכל להשתמש בכל תכונה שקיימת לעסקה בפועל. זה מאפשר פירוט רב יותר בתחזית. לדוגמה, תוכל להזין פרטים עבור כמויות, עובדים, פריטים או מאפייני שורה.         | כאשר אתה מזין פרטי תקציב, תוכל להשתמש רק בסכומים, בקטגוריות ובפעילויות.                    |
| **אבטחה**              | חיזוי מבוסס על עסקאות שאתה מזין בטפסי התחזית ואינו כולל מנגנון בקרת תהליכים. כל עובד שיש לו הרשאות לטופס תחזית יכול לשנות מידע ללא אישור.                                        | תקצוב משתמש במערכת זרימת העבודה, המאפשרת ניהול שינויים ומאפשרת לשמור היסטוריה של התיקונים.         |
| **סוגי ערכים**           | ערכי עסקאות תחזית מבוססים על מספר היחידות ועל מחירי יחידת מכירה ועלויות.  | פרטי התקציב מבוססים על סכומים המתחלקים בין עלויות והכנסות.                                          |
| **מודלי תחזית**       | מכיוון שכל תחזית חייבת להיות משויכת למודל, באפשרותך ליצור כמה מודלי תחזית וכן להגדיר מודלי משנה.           | תקצוב הפרויקט מגביל את מודלי התחזית המשמשים לתקצוב. כמות מועטה של מודלי תחזית יכולה לעזור בהגברת העקביות בחיזויים.                           |
| **גלישת עלויות**         | תוכל לאשר או לא לאשר את ערך העסקאות שיגרמו לגלישת העלות.   | תקצוב פרויקטים מספק אפשרויות בקרה נוספות למשתמשים. אתה יכול לאפשר אזהרות וגלישות.                    |
| **פקד**               | בקרת התחזית מתבצעת באמצעות הפחתת תחזית. הסכומים בפועל מופחתים מיתרות העסקה התחזית ללא כל נתיב ביקורת. פעולה זו עשויה להקשות על המעקב אחר המקומות שבהם התרחשו העסקאות בפועל.                   | בבקרת תקציב הפרויקט, הסכומים בפועל מופחתים מהסכומים בתקציב שנותר. זה מאפשר נתיב ביקורת ברור יותר.                                   |

## <a name="project-forecasts"></a>תחזיות פרויקטים
בעת שימוש בחיזוי פרויקטים, תוכל להזין עסקאות תחזית בטפסי תחזית לכל סוג עסקה. כל תכונה שזמינה לעסקה בפועל יכולה לשמש לעסקת תחזית, למשל רווחיות ענף, תכונות ענף, עובדים או תיאורים. תוכל גם לשקף כמה זמן אחרי שתיצבר עלות תחייב את הלקוח. 

עסקאות חיזוי פרויקטים מבוססות על יחידות וסכומים. 

עליך לשייך כל תחזית פרויקט למודל תחזית. בעת הזנת עסקת תחזית, מודל תחזית מוצע אוטומטית. מודל התחזית משמש כגורם מכיל לעסקאות התחזית. 

תוכל לייעד מודלי תחזית כמודלי משנה עבור מודל. פעולה זו תאפשר לך ליצור תחזית לפי אזור, תקופת זמן או מחלקה. תוכל להעתיק את עסקאות התחזית במודל כדי ליצור מודל חדש. בנוסף, תוכל להעביר את העסקאות אל הספר הראשי. מכיוון שקיים קשר יחיד ליחיד בין תחזית ומודל, כל מודל תחזית מהווה תקציב נפרד לפרויקט. 

מודלי תחזית יכולים להשתמש בהפחתת תחזית כמנגנון הבקרה לפרויקטים. בהפחתת התחזית, עסקאות בפועל מקטינות את יתרות העסקאות בתחזית. עם זאת, בגלל שהפחתת התחזית חלה על הפרויקט הגבוה ביותר בהירארכיה, היא מספקת תצוגה מוגבלת של שינויים בתחזית. לדוגמה, אם עובד משויך לפרויקט משנה, העסקאות בפועל עבור העובד נרשמות בפרויקט האב. זה יכול להקשות על מעקב אחר שינויים מכיוון שלא ניתן לקבוע בקלות איזו עסקה בפרויקט משנה כלשהו גרמה להפחתה בסכום התחזית. לכן, מומלץ ליצור עותק של מודל תחזית שיהיה בשימוש בהפחתת התחזית. לאחר מכן תוכל להשתמש בדוחות כדי להציג את התחזיות המקוריות. 

באפשרותך לשנות, להעתיק, למחוק או להעביר תחזיות פרויקטים לתקציב ספר ראשי. עם זאת, אין בקרת תהליכים. כל עובד שיש לו הרשאה לטופס תחזית יכול לבצע תיקונים ללא סקירה.

-   **תיקון** – תוכל לתקן עסקת תחזית באותם הטפסים שבהם הוזנו הערכים המקוריים.
-   **העתקה או מחיקה** – בעת העתקת עסקאות תחזית, אתה מעתיק את שורות העסקאות במודל תחזית אחד למודל תחזית אחר. בעת מחיקת תחזית, אתה מוחק את עסקאות התחזית ממודל תחזית. להגבלת עסקאות התחזית שהועתקו או שנמחקו, בחר סוגי עסקאות ותאריכים ספציפיים. פעולה זו מאפשרת לך להעתיק או למחוק רק חלקים ספציפיים בתחזית.
-   **העברה** – בעת העברת תחזית פרויקט לתקציב ספר ראשי, אתה מעביר את עסקאות התחזית של מודל תחזית לתקציב ספר ראשי. תוכל להחליף כל עסקה שהועברה בעבר בתקציב הספר הראשי שאליו אתה מעביר את תחזית הפרויקט שלך.

## <a name="project-budgets"></a>תקציבי פרויקט
תקצוב פרויקט הוא שיטה פשוטה יותר מחיזוי, אם כי הוא משתלב במודלי התחזית. הוא משתמש בטופס ערך יחיד לפרטי תקציב מקוריים ותיקונים, ומאפשר תחזיות המבוססות רק על סכום, קטגוריה או פעילות. 

בתקצוב הפרויקט, יש לשלוח את כל התקציבים המקוריים והשינויים לזרימת העבודה של הפרויקט לאישור. זרימות עבודה מעניקות לך בקרה מוגברת על התהליך ויוצרות רשומת היסטוריית שינויים. 

תקצוב הפרויקט דומה לתקצוב ספר ראשי, אך הוא מהיר וקל יותר להגדרה. אפשרויות רבות בתקצוב ספר ראשי, כגון רצפי מספרים או מטבע, לא דורשות הגדרה בנפרד עבור פרויקטים.

תקציבי הפרויקט משויכים אוטומטית לשני מודלי תחזית, אחד לתקציב המקורי ואחד לתקציב שנותר. לכן, דוחות המבוססים על מודלי תחזית יכולים להשתמש בנתוני תקציב. כאשר תקציב הפרויקט מחויב, המערכת יוצרת עסקאות תחזית המבוססות על המודלים המשויכים, המשמשים למטרות דיווח ובקרה.

## <a name="forecast-models"></a>מודלי תחזית
למודלי תחזית יש הירארכיה של שכבה אחת. משמעות הדבר היא שתחזית פרויקט אחת חייבת להיות משויכת למודל תחזית אחד.

אם אתה משתמש בחיזוי פרויקטים, אתה יכול לזהות מודלים כמודלי משנה. לאחר מכן תוכל ליצור תחזיות לפי מחלקה, תקופת זמן או אזור. לדוגמה, תוכל ליצור מודל תחזית לשנה, ולאחר מכן ליצור מודלי משנה עבור תחזיות לאזור צפון מזרח, דרום מזרח, צפון מערב ודרום מערב שראשי האזורים מגישים. על ידי בחירת אפשרויות שונות בדוחות הזמינים, תוכל להציג מידע לפי תחזית כוללת או לפי מודל משנה.


