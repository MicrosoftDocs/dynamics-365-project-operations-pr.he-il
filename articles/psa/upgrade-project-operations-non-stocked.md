---
title: שדרג מ- Project Service Automation ל- Project Operations
description: מאמר זה מספק סקירה כללית של התהליך השדרוג מ- Microsoft Dynamics 365 Project Service Automation ל- Dynamics 365 Project Operations.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/13/2022
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
ms.reviewer: johnmichalak
ms.openlocfilehash: 30eb02240de6617d4c550ce59db2a454eee36f5b
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912977"
---
# <a name="upgrade-from-project-service-automation-to-project-operations"></a>שדרג מ- Project Service Automation ל- Project Operations

אנו נרגשים להכריז על השלב הראשון מבין שלושה לשדרוג מ- Microsoft Dynamics 365 Project Service Automation ל- Dynamics 365 Project Operations. מאמר זה מספק סקירה כללית ללקוחות שיוצאים למסע המרגש הזה. מאמרים עתידיים יכללו שיקולי מפתחים ופרטים על שיפורים בתכונות. הם לא רק יספקו הנחיות שיעזרו לך להתכונן לשדרוג שלך ל- Project Operations אלא גם יסבירו למה לצפות לאחר השדרוג.

תוכנית אספקת השדרוג תפוצל לשלושה שלבים.

| אספקת השדרוג | שלב 1 (ינואר 2022) | שלב 2 (גל אפריל 2022) | שלב 3  |
|------------------|------------------------|---------------------------|---------------------------|
| אין תלות במבנה התפלגות העבודה (WBS) עבור פרויקטים | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| ה-WBS במסגרת המגבלות של Project Operations שנתמכות כרגע | | :heavy_check_mark: | :heavy_check_mark: |
| ה-WBS מחוץ למגבלות של Project Operations שנתמכות כרגע, כולל תמיכה ב- Project Desktop Client | | | :heavy_check_mark: |

## <a name="upgrade-process-features"></a>תכונות ‏‏תהליך השדרוג 

כחלק מתהליך השדרוג, הוספנו יומני שדרוג למפת האתר, כך שמנהלי מערכת יוכלו לאבחן תקלות ביתר קלות. בנוסף לממשק החדש, כללי אימות חדשים יתווספו כדי להבטיח את שלמות הנתונים לאחר שדרוג. האימותים הבאים יתווספו לתהליך השדרוג.

| אימותים | שלב 1 (ינואר 2022) | שלב 2 (גל אפריל 2022) | שלב 3  |
|-------------|------------------------|---------------------------|---------------------------|
| ה-WBS יאומת כנגד הפרות נפוצות של שלמות הנתונים (לדוגמה, הקצאות של משאבים המשויכות לאותה משימת אב אך יש להן פרויקטי אב שונים). | | :heavy_check_mark: | :heavy_check_mark: |
| ה-WBS יאומת כנגד [המגבלות הידועות של Project for the Web](/project-for-the-web/project-for-the-web-limits-and-boundaries). | | :heavy_check_mark: | :heavy_check_mark: |
| ה-WBS יאומת כנגד המגבלות הידועות של Project Desktop Client. | |  | :heavy_check_mark: |
| משאבים הניתנים להזמנה ולוחות שנה של פרויקטים יוערכו מול חריגים נפוצים של כלל לוח שנה לא תואם. | | :heavy_check_mark: | :heavy_check_mark: |

בשלב 2, הפרויקטים הקיימים של לקוחות שישדרגו ל- Project Operations ישודרגו לחוויית ׳לקריאה בלבד׳ לתכנון פרויקטים. בחוויית ׳לקריאה בלבד׳ זו, ה-WBS המלא יהיה גלוי ברשת המעקב. כדי לערוך את ה-WBS, מנהלי פרויקטים יכולים לבחור באפשרות **המר** בדף ה **פרויקטים** הראשי. תהליך רקע יעדכן את הפרויקט כך שיתמוך בחוויית תזמון הפרויקט החדשה מ- Project for the Web. שלב זה מתאים ללקוחות שיש להם פרויקטים המתאימים [למגבלות ידועות של Project for the Web](/project-for-the-web/project-for-the-web-limits-and-boundaries).

בשלב 3 תתווסף תמיכה ב- Project Desktop Client, לטובת לקוחות שרוצים להמשיך לערוך את הפרויקטים שלהם מאותה אפליקציה. עם זאת, אם פרויקטים קיימים יומרו לחוויית Project for the Web החדשה, הגישה לתוספת תושבת עבור כל פרויקט שהומר.

## <a name="prerequisites"></a>דרישות מוקדמות

כדי להיות להתאים לשדרוג שלב 1, על הלקוח לעמוד בקריטריונים הבאים:

- אסור לסביבת היעד להכיל רשומות כלשהן בישות **msdyn_projecttask**.
- יש להקצות רישיונות תקפים של Project Operations לכל המשתמשים הפעילים של הלקוח. 
- על הלקוח לאמת את תהליך השדרוג לפחות בסביבה אחת שאינה סביבת ייצור, שיש בה ערכת נתונים טיפוסית שמתיישרת עם נתוני הייצור.
- יש לעדכן את סביבת היעד ל-Project Service Automation מהדורת עדכון 41 (3.10.62.162) ואילך.

תנאים מוקדמים לשלב 2 ושלב 3 יעודכנו כשתאריכי הזמינות הכוללת יתקרבו.

## <a name="licensing"></a>רישוי

אם יש לך רישיונות פעילים עבור Project Service Automation, תוכל להתקין ולהשתמש ב- Project Operations, הכולל את כל היכולות של Project Service Automation ועוד. בדרך זו, תוכל לבדוק את היכולות של Project Operations בזמן שאתה ממשיך להשתמש ב-Project Service Automation בייצור. לאחר פקיעת הרישיונות של Project Service Automation, תצטרך לעבור ל- Project Operations. בעת תכנון מעבר זה, עליך לתת את הדעת לכך שרישיון Project Operations אינו כולל רישיון Project Service Automation.

## <a name="testing-and-refactoring-customizations"></a>בדיקת התאמות אישיות וארגון הקוד מחדש

כנקודת התחלה, ייבא את כל ההתאמות האישיות לסביבת Project Operations (לייט) נקייה כדי לאשר שהיבוא הצליח ושהפעולות העסקיות פועלות כמצופה.

הנה כמה דברים שכדאי לשים לב אליהם:

- הייבוא עלול להיכשל בגלל יחסי תלות חסרים. במילים אחרות, ההתאמות האישיות מתייחסות לשדות או לרכיבים אחרים שהוסרו ב- Project Operations. במקרה זה, הסר את יחסי התלות הללו מסביבת הפיתוח.
- אם הפתרונות המנוהלים והלא מנוהלים שלך כוללים רכיבים שאינם מותאמים אישית, הסר רכיבים אלה מהפתרון. לדוגמה, כאשר מתאימים אישית את היישות **פרויקט**, יש להוסיף רק את כותרת הישות לפתרון שלך. אל תוסיף את כל השדות. אם הוספת בעבר את כל רכיבי המשנה, ייתכן שיהיה עליך ליצור באופן ידני פתרון חדש ולהוסיף לו רכיבים רלוונטיים.
- טפסים ותצוגות עשויות שלא להופיע כצפוי. בנסיבות מסוימות, אם עשית התאמה אישית של אחד מהטפסים או התצוגות שמגיעות מוכנות לשימוש, ההתאמות האישיות עשויות למנוע כניסת לתוקף של עדכונים חדשים ב- Project Operations. כדי לזהות את הבעיות האלו, אנו ממליצים לעשות סקירה, זה לצד זה, של התקנה נקייה של Project Operations והתקנה של Project Operations הכוללת את ההתאמות האישיות שלך. השווה את הטפסים הנפוצים ביותר בעסק שלך כדי לוודא שהגרסה שלך של הטופס עדיין הגיונית ושלא חסר בה משהו מגרסה הנקייה של הטופס. בצע את אותו סוג של סקירה, זה לצד זה, עבור כל התצוגות שהתאמת אישית.
- הלוגיקה העסקית עלולה להיכשל בזמן ריצה. מכיוון שהפניות לשדות בתוספי הפלאגין שלך לא מאומתות בזמן הייבוא, הלוגיקה העסקית עלולה להיכשל בגלל הפניות לשדות שכבר לא קיימים, וייתכן שתקבל הודעת שגיאה הדומה לדוגמה הבאה: "היישות 'פרויקט' אינה מכילה תכונה עם ‎Name = 'msdyn_plannedhours'‎ ו-NameMapping = 'Logical'‎." במקרה זה, שנה את ההתאמות האישיות שלך כך שישתמשו בשדות החדשים. אם אתה משתמש במחלקות פרוקסי שנוצרו אוטומטית ובהפניות מסוג חזק בלוגיקת התוסף שלך, שקול ליצור מחדש את מחלקות הפרוקסי אלה מהתקנה נקייה. בדרך זו, תוכל לזהות בקלות את כל המקומות שבהם התוספים שלך תלויים בשדות שהוצאו משימוש.

לאחר שתעדכן את ההתאמות האישיות שלך כדי לאפשר ייבוא נקי של Project Operations, המשך לשלבים הבאים.

## <a name="end-to-end-testing-in-development-environments"></a>בדיקות מקצה לקצה בסביבות פיתוח

### <a name="initiate-upgrade"></a>התחל שדרוג 

1. במרכז הניהול של Power Platform, בחר בסביבה שלך. ואחר כך, באפליקציות, מלא את השדות ובחר ב **Dynamics 365 Project Operations**.
2. ‏‏בחר **התקן** כדי להתחיל בשדרוג. מרכז הניהול של Power Platform יציג את ההתקנה הזאת כהתקנה חדשה. עם זאת, תזוהה נוכחות של גרסה קודמת של Project Service Automation, וההתקנה הקיימת תשודרג.

    לאחר השלמת השדרוג, הסביבה צריכה להראות ש- Project Operations מותקנת וש- Project Service Automation אינה מותקנת.

    > [!NOTE]
    > בהתאם לכמות הנתונים בסביבה, השדרוג עשוי להימשך מספר שעות. בהתאם לכך, על צוות הליבה שמנהל את השדרוג לתכנן להפעיל את השדרוג בשעות שאינן שעות עבודה. במקרים מסוימים, אם נפח הנתונים גדול, יש להפעיל את השדרוג במהלך סוף השבוע. ההחלטה לגבי תזמון צריכה להתבסס על תוצאות הבדיקה בסביבות נמוכות יותר.

3. שדרג פתרונות מותאמים אישית לפי הצורך. בשלב זה, פרוס את כל השינויים שביצעת בהתאמות האישיות שלך במקטע [‏‫בדיקת התאמות אישיות וארגון הקוד מחדש‬](#testing-and-refactoring-customizations) של מאמר זה.
4. עבור אל **הגדרות** \> **פתרונות**, ובחר להסיר את ההתקנה של הפתרון **רכיבים של Project Operations שהוצאו משימוש**.

    פתרון זה הינו פתרון זמני המחזיק את מודל הנתונים הקיים ואת הרכיבים הקיימים במהלך השדרוג. על ידי הסרת פתרון זה, אתה מסיר את כל השדות והרכיבים שאינם בשימוש עוד. בדרך זו, אתה עוזר לפשט את הממשק ולהקל על האינטגרציה וההרחבה.
    
### <a name="validate-common-scenarios"></a>אימות תרחישים נפוצים

כאשר אתה מאמת התאמות אישיות ספציפיות, אנחנו ממליצים לסקור גם את התהליכים העסקיים הנתמכים ביישומים. תהליכים עסקיים אלה כוללים, בין היתר, יצירה של ישויות מכירה כגון הצעות מחיר וחוזים, ויצירת פרוייקטים הכוללים פריטי WBS ואישור של נתונים בפועל.

## <a name="major-changes-between-project-service-automation-and-project-operations"></a>הבדלים עיקריים בין Project Service Automation לבין Project Operations

מקטע זה מספק סיכום של ההבדלים העיקריים בין Project Service Automation ו-Project Operations.

### <a name="project-planning"></a>תכנון פרוייקטים

יכולות תכנון הפרויקט ב-Project Operations אינן מסתמכות עוד על שילוב לוגיקה בצד הלקוח והיגיון בצד השרת. במקום זה, Project Operations משתמש ב- Project for the Web בתור מנוע התזמון שלו. שינוי זה ביכולות התזמון מאפשר מספר תכונות חדשות, כגון תצוגות Board ו-Gantt, תכנון מונחה משאבים, [פריטי רשימת משימות](https://support.microsoft.com/office/use-task-checklists-in-microsoft-project-for-the-web-c69bcf73-5c75-4ad3-9893-6d6f92360e9c), ומצבי תזמון פרויקטים. יכולות התזמון החדשות נתמכות גם על ידי סט עשיר של [ממשקי תכנות יישומים (API)](../project-management/schedule-api-preview.md) חדשים. ממשקי API אלה נועדו לסייע לך להבטיח ששום פעולה פרוגרמטית ליצירה, עדכון או מחיקה של ישות ב-WBS לא תשחית את השדות המחושבים בלוח הזמנים.

## <a name="billing-and-pricing"></a>חיוב ותמחור

כחלק מהמשך ההשקעות ב- Project Operations, מספר יכולות חדשות זמינות ב'חיוב' ו'בתמחור'. להלן מספר דוגמאות:

- [רישום השימוש בחומרים בפרוייקטים ובמשימות הפרוייקט](../material/material-usage-log.md)
- [ניהול חוזי משנה](../pro/subcontracting/managing-subcontracts-overview.md)
- [חוזים מבוססי מקדמות וריטיינרים](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [חוזה מצב ואימות של 'אין לחרוג'](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- חיוב מבוסס משימה

## <a name="frequently-asked-questions"></a>שאלות נפוצות

### <a name="which-deployment-types-are-currently-supported-for-upgrade"></a>אילו סוגי פריסה נתמכים כעת לשדרוג?

| מקור                                                 | יעד                                                    | סטטוס                  |
|--------------------------------------------------------|-----------------------------------------------------------|-------------------------|
| Project Service Automation                             | פריסת לייט של Project Operations                        | נתמך               |
| Dynamics 365 Finance - ניהול וחשבונאות של פרוייקטים | פריסת לייט של Project Operations                        | נכון לעכשיו לא נתמך |
| ניהול וחשבונאות של פרוייקטים ב- Finance              | Project Operations לתרחישים של משאבים/ללא מלאי     | נכון לעכשיו לא נתמך |
| Project Service Automation ‏‎3.x                         | Project Operations לתרחישים של משאבים/ללא מלאי     | נכון לעכשיו לא נתמך |
| Project for the Web (סביבה ייעודית)            | פריסת לייט של Project Operations                        | נכון לעכשיו לא נתמך |

### <a name="how-can-i-install-project-operations-before-the-upgrade-tooling-is-available"></a>כיצד אוכל להתקין את Project Operations לפני שכלי השדרוג זמין?

ישנן שתי אפשרויות להתקנת Project Operations לפני שכלי השדרוג זמין:

- הקצאת סביבה חדשה.
- פרוס את Project Operations בנפרד בכל ארגון מכירות שבו Project Service Automation אינו קיים.

> [!NOTE]
> אם Project Service Automation מותקן בארגון, אך לא נעשה בו שימוש, ניתן להסיר את ההתקנה. לאחר שתסיר לחלוטין את Project Service Automation, ניתן להתקין את Project Operations באותו ארגון.
