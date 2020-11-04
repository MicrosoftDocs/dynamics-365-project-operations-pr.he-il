---
title: סקירה כללית של מבני התפלגות עבודה
description: מבנה התפלגות עבודה (WBS) הוא תיאור העבודה שתושלם לפרויקט. זוהי היררכיית משימות המייצגת את הבנת צוות הפרויקט את הרכב העבודה, ואת הגודל, העלות ומשך הזמן של כל רכיב או משימה.
author: Yowelle
manager: AnnBe
ms.date: 07/25/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjWorkBreakdownStructure
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 23861
ms.assetid: 241a0464-0056-4a69-b468-0afbe2d5f3ae
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 9d0cfcc27c69695fc6fe897e798b2831528833e6
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077283"
---
# <a name="work-breakdown-structures-overview"></a>סקירה כללית של מבני התפלגות עבודה

[!include [banner](../includes/banner.md)]

מבנה התפלגות עבודה (WBS) הוא תיאור העבודה שתושלם לפרויקט. זוהי היררכיית משימות המייצגת את הבנת צוות הפרויקט את הרכב העבודה, ואת הגודל, העלות ומשך הזמן של כל רכיב או משימה. ל- WBS יש שלוש מטרות עיקריות:

-   תאר את פירוט או הרכב העבודה במשימות.
-   תזמון העבודה על הפרויקט.
-   הערך את העלות של כל משימה.

מידת הפירוט ב- WBS תלויה ברמת הדיוק הנדרשת באומדנים וברמת המעקב הנדרשת לעומת הערכות אלה. פרויקטים שיש להם סובלנות נמוכה מאוד להחלקות בלוח הזמנים או בעלויות דורשים בדרך כלל WBS מפורט יותר ומעקב קפדני אחר התקדמות העבודה ועלותה מול ה- WBS. פרויקט מסוג זה נפוץ בענפי הבנייה וההנדסה. 

לעומת זאת, פרויקטים בתעשיות כמו מדיה ופרסום, תוכנה ותשתית IT נוטים להיות ייחודיים במינם, והפרודוקטיביות תלויה בחוויה ובמיומנות של האדם שמבצע את המשימה. לכן, ענפים אלה משתמשים ב- WBS כדי לקבל הערכה של גודל הפרויקט, ולא כדי לעקוב אחר התקדמות הפרויקט בפירוט. 

בניית WBS היא תהליך אינטנסיבי שבדרך כלל נעשה לאורך תקופה ארוכה, ודורש שיתוף פעולה ומידע ממגוון רחב של אנשים. נושא זה מתאר כיצד תוכלו להשתמש בשיפורי WBS כדי לעמוד בדרישות שלכם לאומדנים ומעקב.

## <a name="prerequisites-for-creating-a-wbs"></a>תנאים מוקדמים ליצירת WBS
כדי ליצור WBS, עליך להיות מסוגל ליצור לוח זמנים לעבודה ולהעריך את עלות העבודה.

### <a name="prerequisites-for-creating-a-work-schedule"></a>תנאים מוקדמים ליצירת לוח זמנים לעבודה

כדי להשתמש ביכולות התזמון המלאות של תכונות ה- WBS, השלם את ההגדרה הבאה:

1.  הגדר יומן ברירת מחדל ולוח שנה של פרויקט:
    1.  לחץ על **ניהול פרויקטים וחשבונאות** &gt; **הגדרה** &gt; **ניהול פרויקטים ופרמטרים חשבונאיים** &gt; **תזמון**. בשדה **יומן עבודה המוגדר כברירת מחדל** , ציין יומן ברירת מחדל. זה יהיה יומן העבודה המוגדר כברירת מחדל עבור כל פרויקט חדש שנוצר.
    2.  באפשרותך לשנות את לוח השנה המוגדר כברירת מחדל עבור פרויקט מסוים. לחץ על דף הפרויקט של הפרויקט, ואז על ה- FastTab **צוות פרויקט ותזמון** , עדכן את השדה **תזמון לוח שנה** על ידי בחירת לוח שנה אחר.

2.  קבע ימי עבודה ושעות עבודה סטנדרטיים. לוח השנה שהגדרת כיומן העבודה עבור הפרויקט שלך ישמש ב- WBS כדי לקבוע את המידע הבא:

-   ימי עבודה וחגים
-   מספר שעות העבודה ביום

להגדרת ימי העבודה ושעות העבודה עבור לוח שנה, או ליצירת לוח שנה חדש, לחץ על **הנהלת הארגון** &gt; **שכיח** &gt; **לוחות שנה**.

### <a name="prerequisites-for-estimating-the-cost-of-work"></a>תנאים מוקדמים לאומדן עלות העבודה

כדי להשתמש ביכולות הערכת העלות המלאות של ה- WBS, עליך להגדיר את העלויות ומחירי המכירה לעובדים, קטגוריות עבודה, הוצאות ושכר טרחה ופריטים.

-   להגדרת מחיר ומחיר מכירה של קטגוריות עבודה, הוצאות ושכר טרחה, לחץ על **ניהול פרויקטים וחשבונאות** &gt; **הגדרה** &gt; **מחירים**.
-   כדי להגדיר את עלות ומחיר המכירה של פריטים, השתמש בדף **הסכמי סחר** עבור כל פריט בדף הרשימה **מוצרים שהופצו** שבניהול מידע על מוצרים.

## <a name="creating-a-wbs"></a>יצירת WBS
יצירת WBS כוללת שלוש פעילויות:

1.  **פירוק העבודה** - צור התפלגות של עבודה לחתיכות או משימות הניתנות לניהול.
2.  **לוח זמני עבודה‬** - הערך את הזמן הנדרש להשלמת משימה, קביעת תלות הדדית במשימה ובחר תאריכי התחלה וסיום למשימות.
3.  **הערכת מחיר** - הערך עלויות לכל משימה.

החלקים הבאים דנים כיצד יכולות ה- WBS עשויות לעזור בכל אחת מהפעילויות הללו.

### <a name="work-decomposition"></a>פירוק העבודה

יצירת התפלגות או פירוק של העבודה היא בדרך כלל השלב הראשון בתהליך יצירת WBS. הפונקציונליות של WBS תומכת במבנים הבסיסיים הבאים להתפלגות או לפירוק של העבודה. 

**משימת שורש הפרויקט** משימת שורש הפרויקט היא משימת הסיכום ברמה העליונה של פרויקט. כל המשימות האחרות של הפרויקט ייווצרו תחתיה. שם משימת השורש תמיד תוגדר כשם הפרויקט. המאמץ, התאריכים ומשך צומת השורש מסכמים את הערכים עבור המשימות שמתחת למשימת השורש. אי אפשר לשנות את המאפיינים של צומת השורש או למחוק אותה.

**‏‫משימות סיכום או גורם מכיל** משימת סיכום היא משימה שמתחתיה משימות משנה או משימות מכוננות. לפעילות ערסל אין עבודה או עלות משלה. במקום זאת, מאמץ העבודה והעלות של משימת סיכום הם סכום מאמץ העבודה ועלות המשימות המרכיבות אותה. תאריך ההתחלה המוקדם ביותר של המשימות המכוננות משמש כתאריך ההתחלה של משימת הסיכום ותאריך הסיום המאוחר ביותר של המשימות המכוננות משמש כתאריך הסיום. ניתן לערוך את שם משימת הסיכום, אך לא ניתן לשנות את מאפייני התזמון עבור מאמץ, תאריכים ומשך זמן. אם תמחק משימת סיכום, תמחק גם את כל המשימות המכוננות שלה. 

**משימות צומת עלה** משימת צומת עלה מייצגת את חבילת העבודה הגרעינית ביותר בפרויקט. לצומת עלה יש הערכות של כמות העבודה, מספר משאבים מתוכנן, תאריך התחלה וסיום ומשך פעילות מתוכננים. 

באפשרותך להשלים את פעולות ההיררכיה הבאות כדי לאפשר יצירת היררכיה או פירוק של עבודה עבור פרויקט. 

**משימה חדשה** כל משימה חדשה שתיצור תתווסף אוטומטית מתחת לצומת הבסיס, ומספר WBS מוקצה אוטומטית למשימה. מספר ה- WBS מייצג את רמת המשימה בהיררכיה. במשימות ברמה הראשונה תחת משימת השורש של הפרויקט, נעשה שימוש בסכימת מספור של 1, 2, 3 וכן הלאה. במשימות תחת הרמה הראשונה, נעשה שימוש בסכימת מספור של 1.1, 1.2, 1.3 וכן הלאה. עבור כל רמה שמתווספת תחת רמה קודמת, מתווספת סדרת מספרים מנוקדת חדשה. 

נכון לעכשיו, אינך יכול להתאים אישית את מספור ה- WBS. 

**משימת כניסה** כשאתה מכניס משימה למשימה, היא הופכת לצאצא של המשימה שקודמת לה. מספר ה- WBS של משימת הצאצא החדשה מחושב מחדש באופן אוטומטי בהתבסס על מספר ה- WBS של ההורה החדש. משימת ההורה היא כעת משימת סיכום או גורם מכיל, ולכן הופכת למכלול של המשימות המכוננות שלה. 

> [!NOTE] 
> כאשר אתה מכניס משימות תחת משימה שהייתה צומת עלה לפני פעולת הכניסה, משימת הסיכום החדשה שנוצרה מאבדת את התאריכים, המאמץ ומספר המשאבים שהיו שלה. כעת היא משתמשת בסיכום הערכים של המשימות המכוננות החדשות שלה. 

**משימה חריגה** כשאתה מחריג משימה, זו כבר לא משימה מכוננת של ההורה שלה. מספר ה- WBS של משימה זו מחושב מחדש באופן אוטומטי כדי לשקף את הרמה החדשה של המשימה בהיררכיה. המאמץ, העלות והתאריכים של פעילות ההורה הקודמת מחושבים מחדש כך שלא יכללו את המשימה הזו. 

**הזז למעלה והזז למטה‬** כשאתה לוחץ על **הזז למעלה** ועל **הזז למטה** , אתה משנה את המיקום של משימה בתוך ההירארכיה של ההורה שלה. המיקום של משימה אינו משפיע על המאמץ, העלות, התאריכים או משך הזמן של הפעילות. עם זאת, מספר ה- WBS של המשימה מחושב מחדש באופן אוטומטי כדי לשקף את המיקום החדש של המשימה.

### <a name="schedule-estimation"></a>אומדן לוח זמנים

אומדן לוח הזמנים הוא בדרך כלל השלב השני ביצירת WBS. כשיטה מומלצת, עליך להשלים את הערכת לוח הזמנים לאחר יצירת המשימות. לדף **מבנה התפלגות עבודה** שב- Finance יש שני חלקים. החלונית העליונה מיועדת להערכת לוח זמנים, והחלונית התחתונה כוללת כרטיסיית **עלויות והכנסות משוערות** שבה תוכל להשתמש לצורך הערכת עלויות. 
**תלות במשימה** ב- WBS, אתה יכול ליצור קשרי פעילויות קדם בין המשימות. בעת הקצאת משימות פעילות קדם למשימה, אותה משימה תוכל להתחיל רק לאחר השלמת כל המשימות של פעילויות הקדם שלה. תאריך ההתחלה המתוכנן של המשימה מוגדר אוטומטית לתאריך האחרון של כל קודמיו. 

**תזמון משימות** הגורמים הבאים קובעים את תזמון משימות צומת העלה:

-   ‏‏פעילויות קדם
-   מאמץ
-   מספר המשאבים
-   תאריכי ההתחלה והסיום

תאריך ההתחלה של משימת צומת עלה שאין לה פעילויות קדם נקבע באופן אוטומטי לתאריך ההתחלה של הפרויקט. משך פעילות צומת עלה תמיד מחושב כמספר ימי העבודה בין תאריכי ההתחלה והסיום שלו. 

*<strong><em>כללי תזמון</em></strong>* כאשר מופעלת עזרה אוטומטית בתזמון, הכללים הבאים חלים על תזמון משימות למשימות צומת עלה:

-   תאריכי ההתחלה והסיום של משימה חייבים להיות ימי עבודה לפי לוח השנה לתזמון הפרויקט.
-   תאריך ההתחלה של משימה שיש לה פעילות קדם נקבע אוטומטית לתאריך הסיום האחרון של פעילויות הקדם שלה.
-   המאמץ למשימה מחושב באופן אוטומטי כדלקמן:

מאמץ = מספר אנשים * משך זמן * שעות ביום עבודה רגיל בלוח השנה של הפרויקט. 

במקרים מסוימים, ייתכן שתרצה לסטות מכללים אלה. אתה יכול לכבות את התזמון האוטומטי כדי למנוע מה- Finance להגדיר או לתקן מאפיינים של משימות צומת עלה באופן אוטומטי. כאשר אתה מזין מידע עבור משימה הגורמת להפרת כללי תזמון כלשהם, מוצג סמל שגיאת תזמון עבור המשימה. אם אינך רוצה שיוצגו שגיאות תזמון, לחץ על **שגיאות תזמון מוצגות** כדי לכבות את התכונה. 

> [!NOTE] 
> הערכים עבור משימת סיכום או גורם מכיל ממשיכים להיות מחושבים כסכום הערכים של המשימות המכוננות, ללא קשר אם העזרה האוטומטית בתזמון מופעלת או מושבתת. 

**תיקון שגיאות תזמון** כאשר עזרה אוטומטית בתזמון מופעלת, סביר להניח שלא יתרחשו שגיאות תזמון. עם זאת, אם תכבה את הסיוע בתזמון אוטומטי ולאחר מכן תפעיל אותו שוב מאוחר יותר, סמלי שגיאות תזמון עשויים להופיע ב- WBS. 

**תיקון שגיאות תזמון לפי משימה** כאשר אתה לוחץ פעמיים על סמל שגיאת התזמון עבור משימה מסוימת, תיבת דו-שיח מציגה את כל שגיאות התזמון עבור אותה משימה. אתה יכול להחליט אילו שגיאות תזמון לתקן למשימה. 

**תיקון כל שגיאות התזמון** אם ברצונך שה- Finance יתקן את כל שגיאות התזמון ב- WBS, בחלונית הפעולה לחץ על **תקן את כל אי-ההתאמות בתזמון**. 

> [!NOTE] 
> תכונה זו עלולה לגרום לשינויים משמעותיים ב- WBS. שגיאות מתוקנות בסדר הבא:

1.  המאמץ המשוער בכל המשימות שונה כך שהוא שווה ליכולת המוגדרת בלוח השנה של הפרויקט.
2.  תאריך ההתחלה של כל משימה שונה כך שהמשימה תתחיל לאחר השלמת כל המשימות שקדמו לה.
3.  תאריך ההתחלה של כל משימה שונה כדי להסיר פערים בתאריכי ההתחלה של משימות קודמות.

### <a name="cost-estimation"></a>הערכת מחיר

כפי שהוזכר קודם במסמך זה, אתה מזין את אומדן העלות עבור כל משימת צומת עלה באמצעות הכרטיסיה **עלויות והכנסות משוערות** שבחלונית התחתונה של הדף **מבנה התפלגות עבודה**. 

> [!NOTE] 
> אינך יכול לשנות את אומדן העלות עבור משימת סיכום או גורם מכיל. אומדן העלות עבור משימת סיכום שווה לסכום אומדן העלות של משימות צומת העלה שלה. העלות הכוללת המשוערת עבור כל משימה מחושבת כסכום סכומי העלות המשוערים עבור סוגי העסקאות הבאים:

-   עבודה
-   פריט או חומר
-   הוצאות

סוג עסקה **תשלום** משמש לאומדן הכנסות מבוסס עמלות. לסוג עסקה זה אין רכיב עלות ולכן הוא אינו נחשב בעת אומדן העלויות. 

סוג עסקה **על חשבון** משמש לרישום ערך המכירה בחוזה בסוג של פרויקט בעל ערך קבוע. סוג עסקה זה גם אינו נלקח בחשבון בעת אומדן העלויות. 

כאשר אתה מעריך עלויות עבור עבודה, חומר והוצאות עבור כל משימה, עליך להקצות קטגוריית פרויקט לעלות המשוערת. 

**הערכת עלויות העבודה** לכל משימת צומת עלה, אתה מקצה מאמץ עבודה בשעות וקטגוריית ברירת מחדל. לכן, כאשר אתה מגדיר לוח זמנים למשימה, אומדן עלות העבודה עבור משימה זו מתווסף אוטומטית בקטגוריית ברירת המחדל לעבודה. אומדן עלות זה מוצג בכרטיסיה **עלויות והכנסות משוערות** ברשת **פרטי שורה** למשימה זו. אם אתה זקוק לאומדני עלות עבודה נוספים, תוכל להוסיף אותם בכרטיסייה זו. אם אתה מגדיל או מקטין את שעות הערכת עלות העבודה, לוח הזמנים למשימה מחושב מחדש באופן אוטומטי. 

**הערכת הוצאות ועלויות חומר** הכרטיסיה **עלויות והכנסות משוערות** גם מאפשרת לאמוד הוצאות ועלויות חומר למשימה, אם אתה זקוק לאומדנים. 

מחיר העלות ומחיר המכירה עבור כל שורת אומדן עבודה או הוצאה מבוססים על ההגדרה שהוגדרה עבור כל קטגוריה בטבלאות התמחור ב **ניהול פרויקטים וחשבונאות** &gt; **הגדרה** &gt; **תמחור**. כשמדובר בפריטים העלות ומחיר המכירה נוספים כברירת מחדל מהסכמי הפריט או הסחר שבדף הרשימה **מוצרים שהופצו** שבניהול פרטי מוצר.

## <a name="tracking-progress-on-the-wbs"></a>מעקב אחר התקדמות ב- WBS
יש תעשיות שעוקבות אחר התקדמות הפרויקט מול WBS ברמה מאוד פרטנית, ואילו אחרות עוקבות אחר התקדמות ברמה גבוהה יותר של WBS. סעיף זה מתאר כיצד תוכלו להשתמש במעקב WBS לצורך דרישות הפרויקט שלכם. 

ל- Finance יש שלוש תצוגות עבור ה- WBS של פרויקט: תצוגת התכנון, תצוגת מעקב המאמצים ותצוגת מעקב העלויות.

### <a name="planning-view"></a>תצוגת תכנון

תצוגת התכנון מציגה את האומדן המתוכנן או הבסיסי של לוח הזמנים ומידע העלויות. למרות שאין תכונות למעקב אחר הגרסה וקו הבסיס לפרויקט WBS, הערכים בתצוגה זו מיועדים לייצג את גרסת הבסיס. החלקים של אומדן לוח הזמנים והערכת עלויות של נושא זה מתארים תפיסה זו ואת אופן השימוש בה ליצירת WBS.

### <a name="effort-tracking-view"></a>תצוגה של מעקב אחר המאמץ

התצוגה מעקב אחר מאמץ מציגה את המעקב אחר ההתקדמות במשימות שב-WBS. הוא משווה את שעות המאמץ האמיתיות שנצברו למשימה לשעות המאמץ המתוכננות. הנוסחאות הבאות מספקות את הערכים בתצוגת מעקב המאמצים:

-   אחוז התקדמות = מאמץ בפועל עד היום ÷ מאמץ מתוכנן עבור המשימה
-   המאמץ שנותר (ידוע גם בשם הערכה להשלמה \[ETC\]) = מאמץ מתוכנן - מאמץ בפועל עד היום
-   הערכה בעת סיום (EAC) = מאמץ שנותר + מאמץ בפועל עד היום
-   סטיית מאמץ חזוי = מאמץ מתוכנן – EAC

תצוגת המעקב אחר מאמץ מציגה השלכה של שונות המאמץ למשימה, בהתבסס על האם ה- EAC הוא פחות או יותר מהמאמץ המתוכנן:

-   אם ה- EAC הוא יותר מהמאמץ המתוכנן, המשימה מתוכננת להימשך זמן רב יותר ממה שתוכנן במקור והיא בפיגור אל מול לוח הזמנים.
-   אם ה- EAC הוא פחות מהמאמץ המתוכנן, המשימה מתוכננת להימשך זמן קצר יותר ממה שתוכנן במקור והיא מקדימה את לוח הזמנים.

**חיזוי מאמץ מחדש של מנהל הפרויקט** לעיתים, מנהל הפרויקט או אישיות אחרת העוקבת אחר התקדמות הפרויקט יצטרכו לשנות את האומדנים המקוריים למשימה. המשימה עשויה לנוע מהר יותר או לאט יותר מהצפוי במקור מסיבות שונות. לדוגמה, ההיקף הצטמצם, או שלעובדים יש פחות ניסיון מהמתוכנן במקור. חיזויים מחדש הם תפיסות של מנהל הפרויקט להערכות, בהתבסס על המצב הנוכחי של פרויקט. באופן כללי, אין לשנות את המספרים הבסיסיים, מכיוון שבסיס הפרויקט הוא מסמך שפורסם עבור לוח הזמנים של הפרויקט והערכת העלות שעליה הסכימו כל בעלי העניין בפרויקט. 

קיימות שתי דרכים שבהן מנהלי פרויקטים יכולים לשנות את המאמץ במשימות:

-   שנה את המאמץ הנותר שמוגדר אוטומטית לעדכון המאמץ שנותר בפועל במשימה.
-   שנה את אחוז ההתקדמות שמוגדר אוטומטית לעדכון ההתקדמות האמיתית במשימה.

שתי הגישות האלו גורמות לחישוב מחדש של ה- ETC, ‏EAC ואחוז ההתקדמות במשימה ושל סטיית המאמץ החזוי במשימה. ה- EAC, ‏ETC ואחוז ההתקדמות במשימות הסיכום מחושבים גם כן, ושונות המאמץ שנחזתה מתעדכנת. 

**מאמץ שונה במשימות סיכום** אתה יכול לשנות את המאמץ במשימות סיכום או גורם מכיל. בין אם אתה משנה את הערכים האלו באמצעות המאמץ שנותר או אחוז ההתקדמות במשימות הסיכום, החישובים מתבצעים אוטומטית בסדר הבא:

1.  מתבצע חישוב ל- EAC,‏‏ ל- ETC ולאחוז ההתקדמות במשימה.
2.  ה- EAC החדש מופץ לפעילויות הצאצא ביחס זהה לזה שהיה בכמות ה- EAC המקורי.
3.  ה- EAC החדש בכל משימה של צומת עלה מחושב.
4.  יתרת המאמץ ואחוז ההתקדמות מחושבים מחדש עבור כל משימות הצאצא המושפעות, בהתבסס על ערך ה- EAC החדש. שונות המאמץ של המשימות מחושבת גם היא מחדש.
5.  ה- EAC של משימות הסיכום מחושב מחדש גם מצמתי העלים.

לחץ על **הרחב לרמה** בתצוגת המעקב אחר מאמץ כדי לקבוע את הרמה שבה יש לעקוב אחר ה-WBS ולתחזק אותו. ה- WBS מורחב אוטומטית לרמה זו בתצוגת המעקב אחר מאמץ בכל פעם שאתה פותח אותו.

### <a name="cost-tracking-view"></a>תצוגת מעקב עלות

תצוגת מעקב העלויות מציגה את המעקב אחר צריכת העלויות למשימה. בתצוגה זו, משווים את העלות בפועל שהושקעה במשימה עד היום לעלות המתוכננת למשימה. הנוסחאות הבאות מספקות את הערכים בתצוגת מעקב העלות:

-   אחוז העלות הנצרכת = עלות בפועל עד היום ÷ עלות מתוכננת עבור המשימה
-   עלות לסיום (CTC) = עלות מתוכננת – עלות בפועל עד היום
-   הערכה במלואה (EAC‏) = CTC + עלות בפועל עד היום
-   סטיית עלות חזויה = עלות מתוכננת – EAC

תצוגת המעקב אחר עלות מציגה תחזית של שונות העלות למשימה, בהתבסס על האם ה- EAC הוא פחות או יותר מהעלות המתוכננת:

-   אם ה- EAC הוא יותר מהעלות המתוכננת, התחזית היא שהמשימה תדרוש יותר כסף ממה שתוכנן במקור והיא תחרוג מהתקציב.
-   אם ה- EAC הוא פחות מהעלות המתוכננת, התחזית היא שהמשימה תדרוש פחות כסף ממה שתוכנן במקור והיא לא תגיע לסף התקציב.

**חיזוי עלות מחדש של מנהל הפרויקט‬** על מנהלי פרויקטים להשתמש ב- CTC כדי לשנות את אומדן העלות המקורי במשימה. מנהל הפרויקט יכול לשנות את ערך ה- CTC לעלות הנדרשת להשלמת המשימה. אם תשנה את ערך ה- CTC, ה- CTC של המשימה, ה- EAC ואחוז העלות הנצרכת ושונות העלות החזויה במשימה מחושבים מחדש. ה- EAC, ‏ETC ואחוז העלות הנצרכת במשימות הסיכום מחושבים גם כן, ושונות העלות שלהם שנחזתה מתעדכנת. 

> [!NOTE] 
> כאשר אתה משנה את המאמץ למשימת WBS בתצוגת המעקב אחר מאמץ, מחושב מחדש CTC, EAC, אחוז העלות הנצרכת ושונות העלויות החזויה בתצוגת מעקב העלויות. עם זאת, תיקוני עלויות אינם משפיעים על הערכים בתצוגת המעקב אחר מאמץ, מכיוון שהעלות לפי סוג העסקה (עבודה, חומר או הוצאה) או קטגוריית הפרויקט אינה מתוקנת. 

**עדכון תחזית לעלויות במשימות סיכום** באפשרותך לשנות עלויות במשימות סיכום, והחישובים מתרחשים באופן אוטומטי בסדר הבא:

1.  ה- EAC, ה- CTC ואחוז העלות הנצרכת במשימה מחושבים מחדש.
2.  ה- EAC החדש מופץ לפעילויות הצאצא ביחס זהה לזה שהיה ב- EAC המקורי במשימות.
3.  מחושב ה- EAC החדש עבור כל משימה.
4.  ה- CTS ואחוז העלות הנצרכת מחושבים מחדש עבור משימות הצאצא המושפעות, בהתבסס על ערך ה- EAC. שונות העלות של המשימות מחושבת גם היא מחדש.
5.  ה- EAC עבור כל משימות הסיכום מחושב מחדש בהתבסס על שינוי זה.

לחץ על **הרחב לרמה** בתצוגת המעקב אחר עלות כדי לקבוע את הרמה שבה יש לעקוב אחר ה-WBS ולתחזק אותו. ה- WBS מורחב אוטומטית לרמה זו בתצוגת המעקב אחר עלות בכל פעם שאתה פותח אותו.

### <a name="earned-value-management"></a>ניהול ערך שנצבר

באפשרותך להשתמש בשיטת הערך הנצבר (EVM) כדי לעקוב אחר התקדמות הפרויקט. תוכל להציג מדדי ערך נצבר במרכז התפקידים של מנהל הפרויקט. רכיב תרשים הערך הנצבר מציג את הערכים המדורגים בזמן של הערך המתוכנן והעלות בפועל. ערך שנצבר נכון לתאריך הנוכחי מוצג כנקודה. נתונים בשלבי זמן עבור ערך שנצבר אינם זמינים כרגע. 

שלב הזמן בתרשים הערך הנצבר מוצג לפי שבוע או לפי חודש. סעיף זה מתאר את שלושת עמודי התווך של EVM: ערך מתוכנן, ערך נצבר ועלות בפועל. 

**ערך מתוכנן** תיאוריית EVM קובעת כי מתווה הערך המתוכנן מייצג את הקצב שבו צוות הפרויקט תכנן להרוויח ערך בפרויקט. 

ה-Finance משתמש בכלל הרווחים 0:100 כאשר הוא מתווה ערך מתוכנן. תחת כלל זה, ערך המשימה מוצג למשימה החל מתאריך הסיום שלה. שום ערך לא מפורסם עד שהמשימה הושלמה במאת האחוזים. 

בניהול פרויקטים וחשבונאות, אתה מזין את תאריך הסיום של צמתים העלים ואת העלות המתוכננת עבורו. כאשר הגרף של הערך המתוכנן מוצג לפי שבוע, הערך המתוכנן מסוכם לפי שבוע עבור כל משימות צומת העלה למשך הפרויקט. 

**ערך שנצבר** תיאוריית EVM קובעת כי מתווה הערך שנצבר מייצג את הקצב שבו צוות הפרויקט מרוויח בפועל ערך בפרויקט. 

ה-Finance משתמש בכלל הרווחים 0:100 כאשר הוא מתווה ערך נצבר. תחת כלל זה, ערך המשימה מוצג למשימה החל מתאריך הסיום שלה. שום ערך לא מפורסם עד שהמשימה הושלמה במאת האחוזים. 

כאשר מחשבים ערך נצבר, אחוז ההתקדמות של כל משימה נחשב. על פי כלל ההשתכרות 0:100, רק משימות שהושלמו בתקופה נתונה נחשבות לחישוב הערך הנצבר בסוף התקופה ההיא. הערך שנצבר בפרויקט מחושב עבור כל המשימות שהושלמו בעת יצירת הגרף. 

> [!NOTE] 
> נכון לעכשיו, למערכת עבור מעקב WBS אין מבני נתונים לאחסון אחוזי התקדמות היסטוריים בכל משימה. לכן ניתן לדווח על ערך שנצבר רק בזמן עיבוד הקוביה. עבד את הקוביה באופן קבוע כדי לעדכן את נתוני הערך הנצבר המוצגים במרכז התפקידים. 

**עלות בפועל** תיאוריית ה- EVM קובעת כי מתווה העלויות בפועל מייצג את קצב ההוצאה הכספית לפרויקט. 

עסקאות המתפרסמות לפרויקט משמשות לרישום שורת העלות בפועל. העלויות מסוכמות לפי תאריך. לאחר מכן משתמשים בנתונים אלה כדי לשרטט את העלויות בפועל לפי שבוע או לפי חודש בתרשים הערך הנצבר.

### <a name="how-to-use-the-concepts-of-planned-value-earned-value-and-actual-cost"></a>כיצד להשתמש במושגי הערך המתוכנן, הערך הנצבר והעלות בפועל

**תזמון שונות** במהלך התכנון אתה יוצר תחזית לעבודה על ציר הזמן. לכן, הערך המתוכנן הוא הקצב שבו חשבו מתכנני הפרויקט כי תסתיים העבודה על הפרויקט. לאחר שפרויקט נכנס לביצוע, העבודה הסתיימה והפרויקט מרוויח ערך. על ידי השוואת ערך מתוכנן לערך שנצבר, תוכל לראות כיצד מתקדמת העבודה בפרויקט. התוצאה של השוואה זו נקראת שונות תזמון. 

אם הערך המתוכנן לתקופה הוא יותר מהערך שנצבר, כמות העבודה שבוצעה על פרויקט קטנה מהמתוכנן. לכן, הפרויקט מפגר אחר לוח הזמנים. מכיוון ששווי מתוכנן וערך שנצבר באים לידי ביטוי במונחים כספיים, זמן ההשהיה בפרויקט מקבל גם ערך כספי. 

אם הערך המתוכנן לתקופה הוא פחות מהערך שנצבר, כמות העבודה שבוצעה על פרויקט גדולה מהמתוכנן. לכן, הפרויקט מקדים את לוח הזמנים. לזמן הביצוע הזה ניתן גם ערך כספי.

**שונות עלויות** מכיוון שערך שנצבר משתמש במחיר העלות כמכפיל, הערך שנצבר מציין את עלות העבודה שנעשית בפרויקט. עם התקדמות הפרויקט, יומן העסקאות מספק תיעוד של כסף שהושקע בפועל על אותו פרויקט. על ידי השוואת ערך שנצבר לעלות בפועל, תוכל להציג את סכום הכסף שהושקע לעומת הערך שנצבר. התוצאה של השוואה זו נקראת שונות עלויות. 

אם העלות בפועל שמושקעת לתקופה גבוהה יותר מהערך שנצבר, הושקע יותר כסף מאשר נצבר. לכן, הפרויקט חורג מהתקציב. 

אם העלות בפועל שמושקעת לתקופה נמוכה יותר מהערך שנצבר, נצבר יותר כסף מאשר הושקע. לכן, הפרויקט אינו חורג מהתקציב.

## <a name="wbs-templates"></a>תבניות WBS
אתה יכול להשתמש בפונקציונליות של תבניות WBS כדי ליצור תבניות סטנדרטיות לפרויקטים. אם הפרויקטים שהחברה שלך מציעה כרוכים בעבודות רבות שניתן לחזור עליהן, כדאי לשקול ליצור תבנית WBS. 

באפשרותך ליצור תבנית WBS מ- WBS של פרויקט קיים, כך שניתן יהיה לעשות שימוש חוזר בידע ובשיטות העבודה המומלצות שאספת במהלך תכנון אותו פרויקט בעתיד. עם זאת, לפעמים, אולי לא הגיוני לשמור את כל ה- WBS כתבנית. לכן, אתה יכול גם ליצור תבניות מחלקים של ה- WBS לפרויקט.

### <a name="saving-a-projects-wbs-as-a-template"></a>שמירת ה- WBS של הפרויקט כתבנית

לאחר שתיצור תבנית, תוכל לייבא אותה ל- WBS של פרויקט חדש מתחת לצומת השורש, או לכל משימה ב- WBS של הפרויקט.

### <a name="importing-a-wbs-template-into-a-projects-wbs"></a>ייבוא תבנית WBS ל- WBS של פרויקט

בעת ייבוא משימות, המשימות בתבנית מאורגנות על סמך תאריך ההתחלה של המשימה שתחתיה הן מיובאות. במהלך הייבוא, משתמשים בקשרי פעילויות קדם במשימות התבנית לחישוב תאריכי ההתחלה של המשימות המיובאות. לוח העבודה הרגיל של פרויקט היעד מיושם על מנת לחשב את תאריכי הסיום של המשימות המיובאות, כך שיישמרו ימי עבודה ושעות עבודה סטנדרטיות המוגדרים בלוח העבודה של הפרויקט הנוכחי. 

סכומי עלות ומחירי מכירה בקווי האומדן מיושמים על מנת להבטיח שלמחירים הספציפיים לפרויקט או לחוזה הפרויקט יש תאריכים תקפים.

### <a name="differences-between-a-projects-wbs-and-a-wbs-template"></a>ההבדלים בין WBS של פרויקט לתבנית WBS

-   למשימות בתבניות WBS אין תאריכי התחלה ותאריכי סיום.

ימי העבודה וימי חגים וחופשות אינם מוגדרים עבור תבניות WBS.

-   תבניות WBS משתמשות תמיד ביומן התזמון שהוגדר כלוח השנה המוגדר כברירת מחדל עבור כל הפרויקטים.

לוח השנה לתזמון המוגדר כברירת מחדל משמש רק כדי לגלות שעות ביום עבודה רגיל.

-   קשרי פעילויות קדם אינם מועתקים לתבנית WBS.

מכיוון שלתבניות WBS אין תאריכים, הלוגיקה של תאריך ההתחלה המבוססת על תאריך הסיום של פעילות הקדם אינה נדרשת.

-   שורת אומדן עלות עבודה נוצרת אוטומטית כאשר נוצרת משימה בתבנית WBS. מחיר המכירה וסכום העלות מועתקים מהעובד שנבחר.

ניתן ליצור עלויות ופריטים באופן ידני, בדיוק כפי שניתן ב- WBS של הפרויקט.

-   שגיאות תזמון מוצגות כשיש חריגות מהנוסחה הבאה:

מאמץ = מספר משאבים × משך זמן × מספר שעות ביום עבודה רגיל 

באפשרותך לתקן את כל שגיאות התזמון בו זמנית על ידי לחיצה **תקן את כל שגיאות התזמון**. 

לחלופין, תוכל לתקן שגיאות תזמון בנפרד על ידי לחיצה על סמל האזהרה עבור כל משימה.


