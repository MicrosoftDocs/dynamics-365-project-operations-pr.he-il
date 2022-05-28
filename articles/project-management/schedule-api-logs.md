---
title: יומנים של תזמון פרויקטים
description: נושא זה מספק מידע ודוגמאות שיעזרו לך להשתמש ביומני תזמון פרויקטים כדי לעקוב אחר כשלים הקשורים לשירות תזמון פרויקטים ול-API של תזמון פרויקטים.
author: ruhercul
ms.date: 11/30/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: 1a58a588d3e2fb92f1b4a4ed0f6f69d0a63908db
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8589519"
---
# <a name="project-scheduling-logs"></a>יומנים של תזמון פרויקטים

_**חל על:** Project Operations עבור תרחישים מבוססי-משאב/לא במלאי, פריסה קלה - עסקה להנפקת חשבונית פרופורמה_, _Project for the web_

Microsoft Dynamics 365 Project Operations משתמש ב- [Project for the Web](https://support.microsoft.com/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5) בתור מנוע התזמון הראשי שלו. במקום להשתמש בתקן ממשקי תכנות יישומי אינטרנט (API) של Microsoft Dataverse, ‏Project Operations משתמש בממשקי ה-API החדשים של Project Scheduling כדי ליצור, לעדכן ולמחוק משימות פרויקט, הקצאות משאבים, תלות במשימות, מיכלי פרויקטים וחברי צוות בפרויקטים. עם זאת, כאשר פעולות יצירה, עדכון או מחיקה מופעלות באופן פרוגרמטי על ישויות של מבנה התפלגות עבודה (WBS), עלולות להתרחש שגיאות. כדי לעקוב אחר שגיאות אלו והיסטוריית הפעולות, יושמו שני יומנים אדמיניסטרטיביים חדשים: **קבוצת פעולות‬** ו- **שירות תזמון פרויקטים (PSS)**. כדי לגשת ליומנים אלה, עבור אל **הגדרות** \> **שילוב לוח זמנים**.

האיור הבא מציג את מודל הנתונים עבור יומני תזמון הפרויקט.

![מודל נתונים עבור יומני תזמון פרויקטים.](media/LOGDATAMODEL.jpg)

## <a name="operation-set-log"></a>יומן קבוצת פעולות

יומן קבוצת הפעולות עוקב אחר הביצוע של קבוצות פעולות המשמשת ליצירה, עדכון או מחיקה של פעולות, אחת או רבות, באצווה, משימות פרויקט, הקצאות משאבים, תלות בפעילויות, מיכלים בפרויקט או חברי צוות בפרויקט. השדה **פעולה במצב** מציג את המצב הכולל של קבוצת הפעולות. הפרטים של קבוצת הפעולות נלכדים ברשומות הפרטים הקשורות של קבוצת הפעולות.

### <a name="operation-set"></a>קבוצת פעולות

הטבלה הבאה מציגה את השדות הקשורים לישות **קבוצת פעולות**.

| SchemaName            | Description                                                                                                  | שם תצוגה            |
|-----------------------|--------------------------------------------------------------------------------------------------------------|------------------------|
| msdyn_completedon     | התאריך והשעה שבהם הושלמה או נכשלה קבוצת הפעולות.                                                | CompletedOn            |
| msdyn_correlationid   | הערך **correlationId** של הרשומה.                                                                  | CorrelationId          |
| msdyn_description     | התיאור של קבוצת הפעולות.                                                                        | Description            |
| msdyn_executedon      | התאריך והשעה שבהם הופעלה הרשומה.                                                                       | בוצע ב:            |
| msdyn_operationsetId  | המזהה הייחודי של מופעי הישות.                                                                   | OperationSet           |
| msdyn_Project         | הפרוייקט הקשור לקבוצת אפשרויות.                                                            | פרויקט                |
| msdyn_projectid       | הערך **projectId** של הרשומה.                                                                      | ProjectId (הוצא משימוש) |
| msdyn_projectName     | לא ישים.                                                                                              | לא ישים         |
| msdyn_PSSErrorLog     | המזהה הייחודי של יומן השגיאות של שירות תזמון הפרוייקטים המשויך לקבוצת הפעולות. | יומן שגיאות PSS          |
| msdyn_PSSErrorLogName | לא ישים.                                                                                              | לא ישים         |
| msdyn_status          | המצב של קבוצת הפעולות.                                                                             | סטטוס                 |
| msdyn_statusName      | לא ישים.                                                                                              | לא ישים         |
| msdyn_useraadid       | מזהה האובייקט של Azure Active Directory (Azure AD) של המשתמש שאליו שייכת הבקשה.                     | UserAADID              |

### <a name="operation-set-detail"></a>פרט של קבוצת פעולות

הטבלה הבאה מציגה את השדות הקשורים לישות **פרט של קבוצת פעולות**.

| SchemaName                 | Description                                                                                 | שם תצוגה           |
|----------------------------|---------------------------------------------------------------------------------------------|-----------------------|
| msdyn_cdspayload           | שדות Dataverse הסדרתיים של הבקשה.                                            | CdsPayload            |
| msdyn_entityname           | שם הישות עבור הבקשה.                                                     | EntityName            |
| msdyn_httpverb             | שיטת הבקשה.                                                                         | פועל HTTP (הוצא משימוש) |
| msdyn_httpverbName         | לא ישים.                                                                             | לא ישים        |
| msdyn_operationset         | המזהה הייחודי של קבוצת הפעולות שאליה שייכת רשומה זו.                      | OperationSet          |
| msdyn_operationsetdetailId | המזהה הייחודי של מופעי הישות.                                                  | פרט OperationSet   |
| msdyn_operationsetName     | לא ישים.                                                                             | לא ישים        |
| msdyn_operationtype        | סוג הפעולה של פרטי קבוצת הפעולות.                                             | OperationType         |
| msdyn_operationtypeName    | לא ישים.                                                                             | לא ישים        |
| msdyn_psspayload           | השדות הסדרתיים של שירות תזמון פרויקטים עבור הבקשה.                           | PssPayload            |
| msdyn_recordid             | המזהה של רשומת הבקשה.                                                       | מזהה רשומה             |
| msdyn_requestnumber        | מספר שנוצר אוטומטית ומזהה את סדר קבלת הבקשות. | מספר בקשה        |

## <a name="project-scheduling-service-error-logs"></a>יומני שגיאות של שירות תזמון פרויקטים

יומני השגיאות של שירות תזמון הפרויקטים מתעדים כשלים שמתרחשים כאשר שירות תזמון הפרויקטים מנסה **לשמור** או **לפתוח** פעולה. ישנם שלושה תרחישים נתמכים שבהם יומנים אלה נוצרים:

- פעולות ביוזמת המשתמש שנכשלות באופן קריטי (לדוגמה, לא ניתן ליצור מטלה בגלל שחסרות הרשאות).
- שירות תזמון הפרויקטים אינו יכול ליצור, לעדכן, למחוק או לבצע כל פעולת מדורגת אחרת על ישות.
- המשתמש מתקל בשגיאות כאשר רשומה לא מצליחה להיפתח (לדוגמה, כאשר פרויקט נפתח או מידע של חבר צוות מתעדכן).

### <a name="project-scheduling-service-log"></a>יומן שירות תזמון פרויקטים

הטבלה הבאה מציגה את השדות שכלולים ביומן של שירות תזמון הפרוייקטים.

| SchemaName          | Description                                                                    | שם תצוגה    |
|---------------------|--------------------------------------------------------------------------------|----------------|
| msdyn_CallStack     | מחסנית קריאות של החריגה.                                               | מחסנית קריאות     |
| msdyn_correlationid | מזהה המתאם של השגיאה.                                               | CorrelationId  |
| msdyn_errorcode     | שדה המשמש לאחסון קוד השגיאה של Dataverse או קוד שגיאה של HTTP. | קוד שגיאה     |
| msdyn_HelpLink      | קישור לתיעוד עזרה ציבורי.                                       | קישור עזרה      |
| msdyn_log           | היומן משירות תזמון הפרויקטים.                                   | יומן רישום            |
| msdyn_project       | הפרוייקט שמשויך ליומן השגיאות.                             | פרויקט        |
| msdyn_projectName   | שם הפרויקט אם העומס של קבוצת הפעולות יימשך. | לא ישים |
| msdyn_psserrorlogId | המזהה הייחודי של מופעי הישות.                                     | יומן שגיאות PSS  |
| msdyn_SessionId     | מזהה ההפעלה של הפרוייקט.                                                        | מזהה הפעלה     |

## <a name="error-log-cleanup"></a>ניקוי יומן שגיאות

כברירת מחדל, ניתן לנקות גם את יומני השגיאות של שירות תזמון הפרוייקטים וגם את היומן של קבוצת הפעולות כל 90 יום. כל הרשומות שנוצרו לפני יותר מ- 90 ימים נמחקות. עם זאת, על ידי שינוי הערך של השדה **msdyn_StateOperationSetAge** בדף **פרמטרים של פרויקט**, מנהלי המערכת יכולים להתאים את טווח הניקוי כך שיהיה בין 1 ל-120 יום. קיימות מספר שיטות לשינוי ערך זה:

- התאם אישית את הישות **פרמטר של פרויקט** על ידי יצירת דף מותאם אישית והוספת השדה **הגיל של קבוצת פעולות מיושנות**.
- השתמש בקוד לקוח המשתמש ב- [ערכת פיתוח תוכנה WebApi ‏(SDK)](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/updaterecord).
- השתמש בקוד Service SDK המשתמש בשיטה Xrm SDK **updateRecord** (הפניה ל-Client API) ביישומים מונחי דגמים. Power Apps כולל תיאור ופרמטרים נתמכים עבור השיטה **updateRecord**.

    ```C#
    Xrm.WebApi.retrieveMultipleRecords('msdyn_projectparameter').then(function (response) {
        parameter = response.entities[0];
        var staleOperationValue = prompt("All records older than (x) days will be deleted, please enter X between 1 to 90 days", 1)
        var newData = {};
        newData.msdyn_projectparameterid = parameter.msdyn_projectparameterid;
        newData.msdyn_staleoperationsetage = parseInt(staleOperationValue);
        Xrm.WebApi.updateRecord("msdyn_projectparameter", parameter.msdyn_projectparameterid, newData).then(
            function success(result) {
                console.log("Project Parameter: Stale Operation Expiry is set to: " + newData.msdyn_staleoperationsetage);
                // perform operations on record update
                Xrm.WebApi.retrieveMultipleRecords('msdyn_projectparameter')
                .then(function (response2) { console.log("Confirmed Project Parameter: Stale Operation Expiry is set to: " + response2.entities[0].msdyn_staleoperationsetage) });
            },
            function (error) {
                console.log("Failed to Update Project Ednpoint with error: " + error.message);
            // handle error conditions
            }
        );
    });
    ```
