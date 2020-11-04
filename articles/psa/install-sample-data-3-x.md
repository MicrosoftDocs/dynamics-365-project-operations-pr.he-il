---
title: התקנת נתונים לדוגמה
description: נושא זה מספק מידע על התקנת נתוני דוגמה ב-Project Service Automation.
ms.custom: dyn365-projectservice
ms.date: 11/08/2018
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.suite: ''
applies_to: Dynamics 365 Project Service Automation
author: ruhercul
ms.author: ruhercul
search.audienceType: IT Pro, Developer
search.app: ''
ms.openlocfilehash: 46dbd8d125396baa97537ea5d11c47864558c113
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077373"
---
# <a name="sample-data-installation-for-the-project-service-application"></a>התקנת הנתונים לדוגמה עבור Project Service

כדי לעזור לך לבנות סביבות הדגמה משלך, Microsoft מספקת חבילות נתונים לדוגמה שניתן להוריד, שמציגות את היכולות של היישומים שלך. קיימים שני סוגים של חבילות נתונים לדוגמה:
- נתוני הפניה/הגדרה
- נתוני הדגמה (הפניה/הגדרה ונתוני טרנזקציות, כגון הזמנות עבודה ופרוייקטים)

חבילות נתוני **הפניה** לדוגמה ניתנות להורדה בשלוש חבילות נפרדות, כך שבאפשרותך להתקין נתונים רק עבור Project Service או רק עבור Field Service, או להתקין את הנתונים לדוגמה עבור שני היישומים בו-זמנית.

חבילות נתוני הגדרה/הפניה לדוגמה הן:

- [**V902PSMasterData** - Project Service גירסה 3.x בלבד](https://go.microsoft.com/fwlink/?linkid=2026540&clcid=0x409)

- [**V902FSMasterData** - Field Service גירסה 8.x בלבד](https://go.microsoft.com/fwlink/?linkid=2026536&clcid=0x409)

- [**V902FPSMasterData** - Field Service 8.x ו- Project Service 3.x](https://go.microsoft.com/fwlink/?linkid=2026041&clcid=0x409)

חבילת נתוני **הדגמה** האחרונה היא:

 - [**FPSDemoData** - Field Service 8.x ו- Project Service 3.x](https://aka.ms/fpsdemodatapackage)

   הוראות התקנה משתנות מעט במקטע 'משתמשים ליצירה ולהגדרה' אך היתר זהה ל [**לפרסום הבלוג**](https://aka.ms/fpsdemodatablog) הקודם. חבילה זו כוללת קבוצת נתוני הדגמה מופחתת והתקנתה אורכת כ- 3 שעות.

חבילות אלו של נתונים לדוגמה זמינות באנגלית בלבד.

> [!IMPORTANT]
> **אין דרך להסיר את התקנת הנתונים לדוגמה.** עליך להתקין חבילות אלו רק במערכות הדגמה, הערכה, הדרכה או בדיקה. בנוסף, שים לב שאין תמיכה בהתקנת חבילה יחידה ולאחר מכן התקנה של חבילה יחידה אחרת. (במילים אחרות, אין באפשרותך להתקין את **FSMasterData** ואחריו **PSMasterData** , או להפך.) אם לדעתך אתה צריך נתונים לדוגמה עבור שני יישומים בשלב כלשהו בעתיד, עליך להתקין חבילת **v902FPSMasterData**.

כאשר אתה מתקין אחת מחבילות הנתונים לדוגמה, תהליך ההתקנה יבצע את הפעולות הבאות:

- יצירה או הגדרה של ברירת מחדל לפרמטרים לצורך שימוש ב-Project Service, ב-Field Service או בשני היישומים (אם ישים).

- ייבוא נתונים לדוגמה עבור היישומים, כגון משאבים שניתנים להזמנה, תפקידים ספציפיים ליישום, רשימות של מכירות ומחירונים, יחידות ארגוניות, רשומות של תהליכי מכירה וישויות אחרות כדי להדגים יכולות מרכזיות.  

עם חבילת **נתונים לדוגמה** , תקבל את הנתונים לעיל ונתוני טרנזקציות נוספים, כגון הזמנות עבודה ופרוייקטים.

האם אתה תוהה אילו יכולות באפשרותך להדגים עם הנתונים לדוגמה? עיין בתרחיש הבדוי Fabrikam Robotics ב[‏‫הערות טכניות‬](#technical-notes).

אם יש לך שאלות לגבי התקנת חבילות אלה של נתונים לדוגמה, [שלח לנו הודעת דואר אלקטרוני אל fpsdemodata@microsoft.com](mailto:fpsdemodata@microsoft.com).

## <a name="requirements"></a>דרישות

פרוטוקול ההתקנה מניח כמה הנחות לגבי מופע היעד שלך (הארגוני):

- שפת הבסיס היא אנגלית, ומטבע הבסיס הוא דולר אמריקני (USD, $).

- לארגון עדיין אין נתונים של Project Service או של Field Service, או שיש לו רק נתוני ברירת מחדל גולמיים המגיעים עם כל ארגון חדש.

- כבר הותקנה הגירסה הנכונה של יישומים עסקיים:
       
    - **עבור FPSDemoData או v902FPSMasterData:** בארגון מותקנות גירסה Field Service 8.x ו- Project Service 3. x.

    - **עבור v902PSMasterData:** בארגון מותקנת גירסה 3. x של Project Service.

    - **עבור v902FSMasterData:** בארגון מותקנת גירסה ‎ 8.xשל Field Service.

> [!NOTE]
> אם עליך להתקין את הנתונים לדוגמה מעל גירסת ניסיון קיימת של Field Service ו-Project Service או סביבת הדגמה שכבר יש בה נתונים (לא מומלץ), יהיה עליך להפסיק את בדיקות הבטיחות המבוצעות על-ידי תוכנית ההתקנה. לקבלת מידע נוסף, עיין בהערות הטכניות שבהמשך.

## <a name="prepare-for-installation"></a>התכונן להתקנה

עליך להפעיל את תוכנית ההתקנה במחשב עם גירסה עדכנית של Windows‏ (Windows 10 מועדף).

עליך לתכנן כך שהמחשב יישאר מחובר לרשת, ושההתקנה תפעל במשך פרק זמן של עד **שעה** עבור **נתוני הגדרה/הפניה**. (בדרך כלל ההתקנה אורכת בסביבות 30 דקות עבור **FPSMasterData** , שכולל נתונים לדוגמה עבור שני היישומים.) עבור **FPSDemoData** , ההתקנה תימשך סביב **3 שעות**.

הפונקציה של שומר מסך במחשב צריכה להיות כבויה. אחרת, אישורי ההפעלה של ההתקנה יאבדו כאשר שומר המסך פעיל (אלא אם תשמור את ההפעלה פעילה).

> [!div class="mx-imgBorder"]
> ![צילום מסך של הגדרות שומר מסך, עם שומר מסך כבוי](media/sample-data-1.png)

## <a name="download-and-unpack"></a>הורד וחלץ

מתקין הנתונים לדוגמה של Project Service ושל Field Service מופץ בצורה של קובץ הפעלה בחילוץ עצמי. שמות הקבצים עשויים להשתנות בהתאם לחבילת הנתונים לדוגמה, אך בכל מקרה השלבים זהים כך שלא משנה איזו חבילה התקנת.

לאחר הורדת החבילה, הרץ את קובץ ה-.exe, ולאחר מכן קבל את התנאים כדי לפרוס את קובץ ה-zip הדחוס. לאחר מכן עליך לחלץ את תוכן הקובץ לתיקיה במחשב שלך.

בהתאם למערכת ההפעלה ולהגדרות האבטחה, ייתכן שיהיה עליך לבצע את הפעולות הבאות לאחר פתיחת קובץ ה-zip:

1. חפש ולחץ באמצעות לחצן העכבר הימני על קובץ **FPSDemoData.dll** בתיקיה **v902FPSMasterData** / **PackageDeployer_FPSDemoData**.

2. בחר **ביטול חסימה**.

3. בחר **החל**.

4. בחר **אישור**.


## <a name="create-or-configure-users"></a>יצירה או קביעת תצורה של משתמשים

החבילה **FPSDemoData** דורשת שישה משתמשים, בעוד שחבילות **FPSMasterData** דורשות משתמש אחד. התייחס לחבילה הנכונה עבור חבילת הנתונים לדוגמה שלך.

## <a name="create-or-configure-users---setupreference-data-packages"></a>יצירה או הגדרה של משתמשים - חבילות נתוני הגדרה/הפניה

החבילה **FPSMasterData** מיועדת להתקנה עם משתמש אחד בשם Spencer Low עם ההגדרות המתוארות כאן. כדי להתקין את החבילה כראוי, תצטרך ליצור משתמשים (או לשנות להם שם באופן זמני) בסביבה שלך כדי להתאים לתצורת הנתונים לדוגמה.

כדי ליצור משתמשים או לקבוע תצורה של משתמשים, עבור אל **הגדרות** > **אבטחה** > **משתמשים** , ובצע את הפעולות הבאות:

1. הגדר UserFullname = "Spencer Low" עם שם המשתמש "spencerl" ( **אותיות קטנות** ) לתפקידים של מנהל הפרוייקט ומנהל התרגול.

2. בחר את המשתמש **Spencer Low** ולאחר מכן בחר ‏‫ **ניהול תפקידים‬**. חפש ובחר את התפקיד **מנהל המערכת** , ולאחר מכן בחר **אישור** כדי להעניק הרשאות ניהול מלאות ל-Spencer Low. שלב זה הוא הכרחי כדי להבטיח שרשומות לדוגמה נוצרות עם הבעלות הנכונה של משתמש ולאכלס תצוגות כראוי.

3. מתוך החבילת שהורדת, עליך לעדכן את קובץ מיפוי הנתונים עם כתובות דואר אלקטרוני של הקשר המשתמש המהווה ברירת מחדל. כדי לעשות זאת, פתח את **PkgFolder** , ולאחר מכן חפש ופתח את הקובץ **ImportUserMapFile.xml** ב-Notepad (או ב- Visual Studio או בעורך XML אחר). הגדר את השדה **DefaultUserToMapTo =** לכתובת הדואר האלקטרוני של המשתמש Spencer Low.

4. אם אינך משתמש ב-Spencer Low עם שם משתמש **spencerl** , עליך לעדכן קובץ נוסף. פתח את הקובץ **DemoDataPreImportConfig.xml** , ולאחר מכן חפש את התג **userstocreateandconfigure**. עדכן את התג **\<login\>** עם שם המשתמש של המשתמש שלך. לקבלת פרטים נוספים, ראה [הערות טכניות](#technical-notes).

## <a name="create-or-configure-users---demo-data-package"></a>יצירה או הגדרה של משתמשים - חבילת נתוני הדגמה

חבילת נתוני הדגמה דורשת שישה משתמשים. כדי שהחבילה תותקן כראוי, בצע את הפעולות הבאות:

 1. צור או שנה באופן זמני את שם המשתמשים הקיימים כך שיתאימו לתצורת הנתונים לדוגמה הנכנסים על-ידי מעבר אל **הגדרות** > **אבטחה** > **משתמשים**.
 
    תפקידים אלה נחוצים רק עבור הדגמות המבוססות על אדם כלשהו.  
    - שם מלא של משתמש="David So" כטכנאי Field Service   
    - שם מלא של משתמש="Jamie Reding" כמשגר Customer Service ו- Field Service   
    - שם מלא של משתמש="Molly Clark" כמנהל תיקי לקוחות   
    - שם מלא של משתמש="Spencer Low" כמנהל פרויקט ושיטת עבודה  
    - שם מלא של משתמש="Veronica Quek" כחבר צוות   
    - שם מלא של משתמש="William Contoso"
  
2. למטרות ייבוא נתוני הדגמה, הקצה לששת המשתמשים שלעיל את תפקיד מנהל המערכת כדי לייבא רשומות לדוגמה כהלכה. 

3. פתח את **PkgFolder** ולאחר מכן חפש ופתח את **ImportUserMapFile.xml**. עדכן את השדות **חדש =** בכתובות דואר אלקטרוני של המשתמשים המתאימים במערכת שלך.

   > [!div class="mx-imgBorder"]
   > ![צילום מסך של UserMapFile](media/sample-data-7.png)

4. אם לשם מלא של משתמש "Spencer Low" יש מזהה משתמש השונה מ- **"spencerl"** , עליך לעדכן קובץ נוסף. פתח את **DemoDataPreImportConfig.xml** וחפש את התג **userstocreateandconfigure**. עדכן את התג **\<login\>** ב- loginId (תלוי רישיות). 

5. לוח השנה של המשתמש הראשון (בתג **userstocreateandconfigure** ) משמש לאכלוס שעות העבודה עבור כל המשאבים הניתנים להזמנה בעת ייבוא נתוני הדגמה. נווט אל **הגדרות** > **אבטחה** > **משתמשים** , חפש את המשתמש "Spencer Low" ופתח את האפשרות "שעות עבודה". ערוך את שעות העבודה הקיימות, תוך בחירת האפשרות **‏‫לוח הזמנים השבועי המחזורי בשלמותו, מן ההתחלה ועד הסיום‬**. ודא כי **שעות העבודה מוגדרות ל- 8 בבוקר עד 5 בערב (9 שעות), בימים שני עד שישי, ואזור הזמן מוגדר לשעון החוף המערבי (ארה"ב וקנדה)**. הדבר נדרש כדי לוודא כי לוח הפרוייקט ולוח הזמנים מוצגים כצפוי.

**המלצה:** שקול ליצור גיבוי של הארגון שלך כעת, למקרה שיהיה עליך לחזור לנקודת ההתחלה אם משהו משתבש במהלך התקנת הנתונים לדוגמה. לקבלת מידע נוסף, ראה [מופעי גיבוי ושחזור](https://docs.microsoft.com/dynamics365/customer-engagement/admin/backup-restore-instances).

## <a name="run-the-package-deployer"></a>הפעל את Package Deployer

1. חפש והפעל את **PackageDeployer.exe** בתיקיה **v902FPSMasterData** או **PackageDeployer_FPSDemoData**.

2. קבל את התנאים וההתניות.

3. בחלון הבא:

   א. בחר סוג פריסה **Office 365**.

   ב. השתמש במשתמש ובסיסמה של מנהל המערכת שהוגדר ב"צור או קבע תצורה של משתמשים" ("Spencer Low" עם שם המשתמש "spencerl").

   ג.‎ ודא שהאפשרות **הצג רשימה של ארגונים זמינים** נבחרה.

      > [!div class="mx-imgBorder"]
      > ![צילום מסך של חלון Package Deployer עם סימון של "הצג רשימת ארגונים זמינה"](media/sample-data-2.png)

4. בחר את הארגון שבו ברצונך להתקין את הנתונים לדוגמה.

5. בחר **הבא** עד שתראה את הדו-שיח **הגדרת נתוני הדגמה**.

   > [!div class="mx-imgBorder"]
   > ![צילום מסך של חלון מצב המתקין של נתוני הדגמה](media/sample-data-3.png)

6. לפני שתמשיך, שים לב שהתקנת הנתונים לדוגמה עלולה להימשך עד שעה (בדרך כלל ~ 10 דקות). יהיה עליך לוודא כי המחשב נשאר מחובר לרשת במהלך ההתקנה וההפעלה שלך נשארת פעילה.   

7. כאשר תהיה מוכן, לחץ על **הבא** כדי להתחיל את תהליך ההתקנה של נתונים לדוגמה. לאחר טעינת הנתונים לדוגמה, לחץ על **סיום**.

## <a name="verify-the-sample-data-installation"></a>ודא שהתקנת הנתונים לדוגמה הושלמה

לצורך הבדיקה, ודא כי מספר הרשומות וסוגי הישויות מופיעים בתרחיש הפיקטיבי Fabrikam Robotics והם נראים כצפוי.

לאחר שהנתונים לדוגמה הועלו, היכנס כמשתמש Spencer Low ואשר את הנקודות הבאות:

- אם Project Service מותקן, עבור אל **Project Service** > **הגדרות** > **מחירונים**. בדוק כי שיעורי החיוב והעלויות קיימים, עם המטבע המתאים, לכל מדינה/אזור בערכת הנתונים.

- אם היישום Project Service מותקן, עבור אל **Universal Resource Scheduling** > **הגדרות** > **יחידות ארגוניות**. אשר כי מחירון עם המטבע המתאים שויך לכל יחידה ארגונית (למעט ערכי עיר). אם הם חסרים, חפש ושייך את המחירון הנכון.

- אם Field Service מותקן, עבור אל **Project Service** > **הגדרות** > **מחירונים**. אשר שתעריפי החיוב והעלויות קיימים. עבור אל **Field Service** > **הגדרות** > **מחירונים** ובדוק כי שיעורי החיוב והעלויות קיימים, עם המטבע המתאים, לכל מדינה/אזור בערכת הנתונים.

  > [!div class="mx-imgBorder"]
  > ![צילום מסך של מחירונים פעילים](media/sample-data-4.png)

  > [!div class="mx-imgBorder"]
  > ![צילום מסך של יחידות ארגוניות פעילות](media/sample-data-5.png)

## <a name="technical-notes"></a>הערות טכניות

ראה בהמשך פרטים טכניים נוספים לגבי ההתקנה של נתונים אלה.

### <a name="installing-sample-data-on-top-of-existing-data-not-recommended"></a>התקנת הנתונים לדוגמה על גבי נתונים קיימים (לא מומלץ)

הערה: אם עליך להתקין את הנתונים לדוגמה מעל גירסת ניסיון קיימת של Field Service או Project Service או סביבת הדגמה שכבר יש בה נתונים (לא מומלץ), יהיה עליך להפסיק את בדיקות הבטיחות המבוצעות על-ידי תוכנית ההתקנה.

כדי לעשות זאת, עבור אל תיקיה **PkgFolder** כדי לחפש ולפתוח את הקובץ **DemoDataPreImportConfig.xml** עם 'פנקס רשימות' (או עורך XML אחר).

חפש את הערך הבא, ולאחר מכן שנה את ההגדרה true ל-false:

```alias
<TerminateOnPreCheckFailure>true</TerminateOnPreCheckFailure>
```

שינוי זה גורם למתקין לעקוף כמה בדיקות בטיחות חשובות, כולל:

- אישור כי אין יותר מפרופיל אחד פעיל של **יחידה ארגונית** ולאחר מכן שינוי השם ל- **Fabrikam US**.

- אישור כי אין יותר מפרופיל אחד פעיל של רשומת **תבנית עבודה**.

- אישור כי אין יותר מפרופיל אחד פעיל של **פרמטרים בפרויקט** ולאחר מכן שינוי השם של הערך ל- **Parameters**.

### <a name="configuration-components"></a>תצורת רכיבים

קיימים מספר רכיבי תצורה אחרים בקובץ זה שעבר ייבוא. עבור משתמשים טכניים, חלק משינויים אלה כוללים:

- **\<RequiredSolutions\>** מציין התקנות פתרון שהן דרישה מוקדמת ואת מספרי הגירסה שלהם.

- **\<InstallSampleData\>** קובע אם יותקנו דוגמאות מוכנות לשימוש עבור היישומים.

    - False - מדלג על התקנה של נתונים מוכללים אלה (שניתן להסיר)

    - True - מתקין את הנתונים המוכללים במקביל להתקנה של הנתונים לדוגמה FS ו- PSA

- **\<PreImportDataCollection\>** מציין מפות נתונים בצורת קובץ שטוח ואת הרשומות המשויכות לייבוא לפני ההתקנה הראשית של הנתונים לדוגמה.

- **\<EntitiesToEnableScheduling\>** מציין אילו ישויות צריכות להיות מופעלות עבור הזמנה ב- Microsoft Dynamics Scheduling (נקרא גם Universal Resource Scheduling).

- **\<UsersToCreateAndConfigure\>** מציין משאבים שניתנים להזמנה שיווצרו (אם הם עדיין לא קיימים) לפני ייבוא הנתונים לדוגמה. שים לב כי משאב הניתן להזמנה של מקור הנתונים לדוגמה תואם לרשומות המשאב הניתן להזמנה של מערכת היעד וב-FullName ובכניסה של כל משאב. לפיכך, אין אפשרות לשנות את השמות בקובץ זה של קביעת תצורה מראש, אלא אם ראשית ביצעת ייבוא של הנתונים לדוגמה לתוך מערכת היעד באמצעות שמות אלה ולאחר מכן שינית את שמות המשאבים הניתנים להזמנה לשם הרצוי יחד עם רשומות המשתמשים הזמינים, ולאחר מכן ביצעת ייצוא של הנתונים כדי שתוכל לייבא אותם לתוך מערכת היעד הסופית שוב (מעדכן את הערכים הישנים והחדשים של **ImportUserMapFile.xml** בהתאם).

- **\<PluginsToDisable\>** מציין פריטי שורה נפרדים של יישומי plug-in שצריכים להיות זמינים במהלך ייבוא הנתונים לדוגמה ולאחר מכן יש להפעילם.

### <a name="fabrikam-robotics-fictitious-scenario"></a>התרחיש הפיקטיבי Fabrikam Robotics

חבילות נתוני ההפניה לדוגמה של Field Service ו-Project Service מתקינות את הפתרון **Fabrikam Manufacturing Master Data (v3.0.0.0)‎** , יחד עם כ-4,000 רשומות וכ-40 ישויות שונות. חבילות הנתונים לדוגמה הנפרדות של Field Service או Project Service מכילות קבוצת משנה של הנתונים לדוגמה **v902FPSMasterData** עבור יישום זה. חבילת **נתוני ההדגמה** מתקינה את **הפתרון Fabrikam Manufacturing Demo Data (v3.0.0.7)** עם כ- 22,000 רשומות ב- 148 ישויות.

החברה הבדויה, Fabrikam Robotics, היא יצרנית של רובוטים בקו הרכבה של מכשירים אלקטרוניים, והיא ידועה באיכות המוצר, חדשנות ושירות לקוחות מוצלח, כולל שירותי התקנה, תכנון, יישום ותחזוקה שוטפת. המשרדים הראשיים של Fabrikam נמצאים בארצות הברית (Fabrikam US), ויש לחברה פעילות שירות המבוססת על פרויקטים בצרפת, בהודו, בבריטניה ובשוויץ.

הפעולות של Field Service מתרכזות בעיקר בארה"ב, באזור סיאטל. החברה מתמקדת במינוף קישוריות של אינטרנט של הדברים (IoT) כדי לפקח על הביצועים של נכסי הלקוחות ולספק שירותים מקדימים יותר ויותר באתר הלקוח.

מבט כולל ברמה גבוהה על הנתונים לדוגמה:

- רכיבים רגילים של נתונים לדוגמה (כלול עבור שני יישומים)

    - משתמש 1

    - 71 תיקי לקוחות

    - 137 אנשי קשר

    - סוגי תנועות וקטגוריות שונות

    - 50 מוצרים במחירון אחד

    - 14 מחירונים/רשימות עלות

    - 31 מאפיינים (כישורי משאבים) ב-2 מודלים לדירוג עם 3 רמות (דירוג ערכים)

- Project Service

    - 8 יחידות ארגוניות

    - 6 רמות ניצול ספציפיות לתפקיד

    - מעל 2.8 אלף מפרטים של מחיר-תפקיד

- Field Service

    - 4 אזורים

    - 5 סוגי הזמנת עבודה

    - 22 נכסי לקוחות

    - 9 סוגי אירועים עם מגוון של מאפייני משאבים משויכים (9), שירותים (13) ומשימות שירות (13)
   
חבילת **נתוני ההדגמה** מתקינה כ- 179 הזמנות עבודה, 12 פרוייקטים ונתוני טרנזקציות קשורים. 

### <a name="change-the-work-hours-for-sample-resources"></a>שנה את שעות העבודה עבור משאבים לדוגמה

כברירת מחדל, לכל המשאבים הניתנים להזמנה יש לוח שנה עם 24 שעות עבודה.

אם עליך לשנות את שעות העבודה עבור משאבים לדוגמה שניתנים להזמנה, עבור אל **Universal Resource Scheduling** > **תזמון** > **משאבים**.

בחר משתמש (לדוגמה, Spencer Low) ושנה את שעות עבודה שלו לשעות שברצונך להחיל על משתמשים מרובים. עבור אל **Universal Resource Scheduling** > **הגדרות** > **תבניות שעות עבודה** וערוך את הרשומה **תבנית עבודה המהווה ברירת מחדל**. בשדה **משאב תבנית** , בחר משתמש עם שעות עבודה שברצונך להחיל על משאבים אחרים. עבור אל **Universal Resource Scheduling** > **תזמון** > **משאבים** > **משאבים פעילים הניתנים להזמנה**. בחר את המשאבים שברצונך לשנות ולאחר מכן בחר **הגדר לוח שנה**. ברשימה הנפתחת **תבנית עבודה** , בחר את התבנית **שעות העבודה המהוות ברירת מחדל** או תבנית אחרת עם המשאב הנכון ליצירת תבנית. כאשר אתה עובר ללוח הזמנים, אתה אמור לראות שהמשאבים כעת עדכנו את שעות העבודה.

> [!div class="mx-imgBorder"]
> ![צילום מסך של משאבים פעילים הניתנים להזמנה](media/sample-data-6.png)