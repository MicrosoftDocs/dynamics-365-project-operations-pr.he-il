---
title: שימוש בממשקי API של לוחות זמנים עם ‬Power Automate
description: מאמר זה מספק זרימה לדוגמה המשתמשת בממשק תכנות (API) של יישומי לוח זמנים של פרוייקט.
author: ruhercul
ms.date: 01/26/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: 2527375ff3f3d631f3bb3de1458abb3b8838db54
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8916335"
---
# <a name="use-project-schedule-apis-with-power-automate"></a>שימוש בממשקי API של לוחות זמנים עם ‬Power Automate

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

מאמר זה מתאר זרימה לדוגמה המדגימה כיצד ליצור תוכנית פרויקט מלאה על ידי שימוש ב- Microsoft Power Automate, כיצד ליצור קבוצת פעולות וכיצד לעדכן ישות. דוגמה זו מדגימה כיצד ליצור פרוייקט, חבר צוות של פרוייקט, קבוצות פעולות, משימות של פרוייקט והקצאות משאבים. מאמר מסביר גם כיצד לעדכן ישות ולבצע קבוצת פעולות.

להלן רשימה מלאה של השלבים המתועדים בזרימה לדוגמה במאמר זה:

1. [יצירת גורם מפעיל של PowerApps](#1)
2. [יצירת פרוייקט](#2)
3. [אתחול משתנה עבור חבר הצוות](#3)
4. [יצירה של חבר צוות כללי](#4)
5. [יצירת קבוצת פעולות](#5)
6. [יצירת מיכל של פרוייקט](#6)
7. [אתחול משתנה עבור מצב הקישור](#7)
8. [אתחול משתנה עבור מספר המשימות](#8)
9. [אתחול משתנה עבור משימת הפרוייקט](#9)
10. [בצע עד](#10)
11. [הגדרת משימת פרוייקט](#11)
12. [יצירת משימת פרוייקט](#12)
13. [יצירת הקצאת משאב](#13)
14. [הקטנת משתנה](#14)
15. [שינוי שם של משימת פרוייקט](#15)
16. [הפעלת קבוצת פעולות](#16)

## <a name="assumptions"></a>הנחות

מאמר זה נכתב מתוך הנחה שיש לך היכרות בסיסית עם פלטפורמת Dataverse, זרימות ענן וממשק תכנות (API) של יישומי לוח זמנים של פרוייקט. לקבלת מידע נוסף, ראה את המקטע [הפניות](#references) בהמשך מאמר זה.

## <a name="create-a-flow"></a>צור זרימה

### <a name="select-an-environment"></a>בחר סביבה

תוכל ליצור את זרימת Power Automate בסביבה שלך.

1. עבור אל <https://flow.microsoft.com> והשתמש באישורי מנהל מערכת כדי להיכנס.
2. בפינה השמאלית העליונה, בחר **‏‫סביבות‬**.
3. מתוך הרשימה, בחר את הסביבה שבה מותקן Dynamics 365 Project Operations.

### <a name="create-a-solution"></a>יצירת פתרון

בצע את השלבים הבאים כדי ליצור [זרימה תומכת בפתרון](/power-automate/overview-solution-flows). על-ידי יצירת זרימה תומכת בפתרון תוכל לייצא את הזרימה בקלות רבה יותר לשימוש בהמשך.

1. בחלונית הניווט, בחר **פתרונות**.
2. בדף **פתרונות**, בחר **פתרון חדש**.
3. בתיבת הדו-שיח **פתרון חדש**, הגדר את השדות הדרושים ובחר **צור**.

## <a name="step-1-create-a-powerapps-trigger"></a><a id="1"></a>שלב 1: יצירת גורם מפעיל של PowerApps

1. בדף **פתרונות**, בחר את הפתרון שיצרת ולאחר מכן בחר **חדש**.
2. בחלונית הימנית, בחר **זרימות ענן** \> **אוטומציה** \> **זרימת ענן** \> **מיידי**.
3. בשדה **שם הזרימה**, הזן **זרימת הדגמה של API של לוח זמנים**.
4. ברשימה **בחר כיצד להפעיל זרימה זו**, בחר **Power Apps**. כאשר אתה יוצר גורם מפעיל של Power Apps, הלוגיקה תלויה בך כמחבר. במאמר זה, השאר את פרמטרי הקלט ריקים למטרות בדיקה.
5. בחר **צור**

## <a name="step-2-create-a-project"></a><a id="2"></a>שלב 2: יצירת פרוייקט

בצע את השלבים הבאים כדי ליצור פרוייקט לדוגמה.

1. בזרימה שיצרת, בחר **צעד חדש**.

    ![הוספת צעד חדש.](media/newstep.png)

2. בתיבת הדו-שיח **בחר פעולה** בשדה החיפוש, הזן **בצע פעולה לא מאוגדת**. לאחר מכן, בכרטיסיה **פעולות**, בחר את הפעולה ברשימת התוצאות.

    ![בחירת פעולה.](media/chooseactiontab.png)

3. בצעד החדש, בחר שלוש נקודות (**...**) ולאחר מכן בחר **שנה שם**.

![שינוי שם של צעד.](media/renamestep.png)

4. שנה את שם הצעד ל **יצירת פרויקט**.
5. בשדה **שם פעולה** בחר **msdyn\_CreateProjectV1**.
6. תחת השדה **msdyn\_subject**, בחר **הוסף תוכן דינמי**.
7. בכרטיסיה **ביטוי** בשדה פונקציה, הזן **שם פרוייקט - utcNow()**.
8. בחר **OK**.

## <a name="step-3-initialize-a-variable-for-the-team-member"></a><a id="3"></a>צעד 3: אתחול משתנה עבור חבר הצוות

1. בזרימה, בחר **צעד חדש**.
2. בתיבת הדו-שיח **בחר פעולה** בשדה החיפוש, הזן **אתחל משתנה**. לאחר מכן, בכרטיסיה **פעולות**, בחר את הפעולה ברשימת התוצאות.
3. בצעד החדש, בחר שלוש נקודות (**...**) ולאחר מכן בחר **שנה שם**.
4. שנה את שם השלב ל **אתחל חבר צוות**.
5. בשדה **שם**, הזן **TeamMemberAction**.
6. בשדה **סוג**, בחר **מחרוזת**.
7. בשדה **ערך**, הזן **msdyn\_CreateTeamMemberV1**.

## <a name="step-4-create-a-generic-team-member"></a><a id="4"></a>צעד 4: צור חבר צוות פרויקט כללי

1. בזרימה, בחר **צעד חדש**.
2. בתיבת הדו-שיח **בחר פעולה** בשדה החיפוש, הזן **בצע פעולה לא מאוגדת**. לאחר מכן, בכרטיסיה **פעולות**, בחר את הפעולה ברשימת התוצאות.
3. בצעד החדש, בחר שלוש נקודות (**...**) ולאחר מכן בחר **שנה שם**.
4. שנה את שם השלב ל **צור חבר צוות**.
5. עבור השדה **שם פעולה**, בחר **TeamMemberAction** בתיבת הדו-שיח **תוכן דינמי**.
6. בשדה **פרמטרי פעולה**, הזן את פרטי הפרמטרים הבאים.

    ```
    {
        "TeamMember": {
            "@@odata.type": "Microsoft.Dynamics.CRM.msdyn_projectteam",
            "msdyn_projectteamid": "@{guid()}",
            "msdyn_project@odata.bind": "/msdyn_projects(@{outputs('Create_Project')?['body/ProjectId']})",
            "msdyn_name": "ScheduleAPIDemoTM1"
        }
    } 
    ```

    להלן הסבר על הפרמטרים:

    - **\@\@odata.type** - שם הישות. לדוגמה, הזן **"Microsoft.Dynamics.CRM.msdyn\_projectteam"**.
    - **msdyn\_projectteamid** – המפתח הראשי של מזהה צוות הפרוייקט. הערך הוא ביטוי של מזהה ייחודי כללי (GUID).   המזהה נוצר מכרטיסיית הביטוי.

    - **msdyn\_project\@odata.bind** – מזהה הפרוייקט של פרוייקט הבעלות. הערך יהיה תוכן דינמי שמגיע מהתגובה של הצעד "יצירת פרוייקט". ודא שאתה מזין את הנתיב המלא ומוסף תוכן דינמי בין הסוגריים. יש צורך במירכאות. למשל, הזן **"/msdyn\_projects(הזן תוכן דינמי)"**.
    - **msdyn\_name** – שם חבר הצוות. לדוגמה, הזן **ScheduleAPIDemoTM1**.

## <a name="step-5-create-an-operation-set"></a><a id="5"></a>צעד 5: צור קבוצת פעולות

1. בזרימה, בחר **צעד חדש**.
2. בתיבת הדו-שיח **בחר פעולה** בשדה החיפוש, הזן **בצע פעולה לא מאוגדת**. לאחר מכן, בכרטיסיה **פעולות**, בחר את הפעולה ברשימת התוצאות.
3. בצעד החדש, בחר שלוש נקודות (**...**) ולאחר מכן בחר **שנה שם**.
4. שנה את שם הצעד ל **יצירת קבוצת פעולות**.
5. בשדה **שם פעולה**, בחר פעולה מותאמת אישית **msdyn\_CreateOperationSetV1** של Dataverse.
6. בשדה **תיאור**, הזן **ScheduleAPIDemoOperationSet**.
7. בשדה **פרוייקט**, הזן **/msdyn\_projects(**.
8. בתיבת הדו-שיח **תוכן דינמי**, בחר **msdyn\_CreateProjectV1Response ProjectId**.
9. בשדה **פרוייקט**, הזן **)**.

## <a name="step-6-create-a-project-bucket"></a><a id="6"></a>צעד 6: יצירת מיכל של פרוייקט

1. בזרימה, בחר **צעד חדש**.
2. בתיבת הדו-שיח **בחר פעולה** בשדה החיפוש, הזן **הוסף שורה חדשה**. לאחר מכן, בכרטיסיה **פעולות**, בחר את הפעולה ברשימת התוצאות.
3. בצעד החדש, בחר שלוש נקודות (**...**) ולאחר מכן בחר **שנה שם**.
4. שנה את שם הצעד ל **צור מיכל**.
5. בשדה **שם טבלה**, בחר **מיכלים של פרוייקט**.
6. בשדה **שם**, הזן **ScheduleAPIDemoBucket1**.
7. עבור השדה **Project**, בחר **msdyn\_CreateProjectV1Response ProjectId** בתיבת הדו-שיח **תוכן דינמי**.

## <a name="step-7-initialize-a-variable-for-the-link-status"></a><a id="7"></a>צעד 7: אתחול משתנה עבור מצב הקישור

1. בזרימה, בחר **צעד חדש**.
2. בתיבת הדו-שיח **בחר פעולה** בשדה החיפוש, הזן **אתחל משתנה**. לאחר מכן, בכרטיסיה **פעולות**, בחר את הפעולה ברשימת התוצאות.
3. בצעד החדש, בחר שלוש נקודות (**...**) ולאחר מכן בחר **שנה שם**.
4. שנה את שם הצעד ל **Init linkstatus**.
5. בשדה **שם**, הזן **linkstatus**.
6. בשדה **סוג**, בחר **מספר שלם**.
7. בשדה **ערך**, הזן **192350000**.

## <a name="step-8-initialize-a-variable-for-the-number-of-tasks"></a><a id="8"></a>צעד 8: אתחול משתנה עבור מספר המשימות

1. בזרימה, בחר **צעד חדש**.
2. בתיבת הדו-שיח **בחר פעולה** בשדה החיפוש, הזן **אתחל משתנה**. לאחר מכן, בכרטיסיה **פעולות**, בחר את הפעולה ברשימת התוצאות.
3. בצעד החדש, בחר שלוש נקודות (**...**) ולאחר מכן בחר **שנה שם**.
4. שנה את שם השלב ל **אתחל מספר משימות**.
5. בשדה **שם**, הזן **מספר משימות**.
6. בשדה **סוג**, בחר **מספר שלם**.
7. בשדה **ערך**, הזן **5**.

## <a name="step-9-initialize-a-variable-for-the-project-task-id"></a><a id="9"></a>צעד 9: אתחול משתנה עבור משימת הפרוייקט

1. בזרימה, בחר **צעד חדש**.
2. בתיבת הדו-שיח **בחר פעולה** בשדה החיפוש, הזן **אתחל משתנה**. לאחר מכן, בכרטיסיה **פעולות**, בחר את הפעולה ברשימת התוצאות.
3. בצעד החדש, בחר שלוש נקודות (**...**) ולאחר מכן בחר **שנה שם**.
4. שנה את שם השלב ל **Init ProjectTaskID**.
5. בשדה **שם**, הזן **מספר משימות**.
6. בשדה **סוג**, בחר **מחרוזת**.
7. עבור השדה **Value**, הזן **guid()** בבונה הביטויים.

## <a name="step-10-do-until"></a><a id="10"></a>צעד 10: בצע עד

1. בזרימה, בחר **צעד חדש**.
2. בתיבת הדו-שיח **בחר פעולה** בשדה החיפוש, הזן **בצע עד**. לאחר מכן, בכרטיסיה **פעולות**, בחר את הפעולה ברשימת התוצאות.
3. הגדר את הערך הראשון במשפט המותנה למשתנה **מספר משימות** מתיבת הדו-שיח **תוכן דינמי**.
4. הגדר את התנאי ל **קטן או שווה ל**
5. הגדר את הערך השנה במשפט המותנה ל **0**.

## <a name="step-11-set-a-project-task"></a><a id="11"></a>צעד 11: הגדרת משימת פרוייקט

1. בזרימה, בחר **צעד חדש**.
2. בתיבת הדו-שיח **בחר פעולה** בשדה החיפוש, הזן **הגדר משתנה**. לאחר מכן, בכרטיסיה **פעולות**, בחר את הפעולה ברשימת התוצאות.
3. בצעד החדש, בחר שלוש נקודות (**...**) ולאחר מכן בחר **שנה שם**.
4. שנה את שם השלב ל **הגדרת משימת פרוייקט**.
5. בשדה **שם פעולה** בחר **msdyn\_projecttaskid**.
6. עבור השדה **Value**, הזן **guid()** בבונה הביטויים.

## <a name="step-12-create-a-project-task"></a><a id="12"></a>צעד 12: יצירת משימת פרוייקט

בצע את השלבים הבאים כדי ליצור משימת פרוייקט עם מזהה ייחודי השייך לפרוייקט הנוכחי ולמיכל הפרוייקט שיצרת.

1. בזרימה, בחר **צעד חדש**.
2. בתיבת הדו-שיח **בחר פעולה** בשדה החיפוש, הזן **בצע פעולה לא מאוגדת**. לאחר מכן, בכרטיסיה **פעולות**, בחר את הפעולה ברשימת התוצאות.
3. בצעד, בחר שלוש נקודות (**...**) ולאחר מכן בחר **שנה שם**.
4. שנה את שם השלב ל **יצירת משימת פרוייקט**.
5. בשדה **שם פעולה** בחר **msdyn\_PssCreateV1**.
6. בשדה **ישות**, הזן את פרטי הפרמטרים הבאים.

    ```
    {
        "@@odata.type": "Microsoft.Dynamics.CRM.msdyn_projecttask",
        "msdyn_projecttaskid": "@{variables('msdyn_projecttaskid')}",
        "msdyn_project@odata.bind": "/msdyn_projects(@{outputs('Create_Project')?['body/ProjectId']})",
        "msdyn_subject": "ScheduleAPIDemoTask1",
        "msdyn_projectbucket@odata.bind": "/msdyn_projectbuckets(@{outputs('Create_Project_Buckets')?['body/msdyn_projectbucketid']})",
        "msdyn_start": "@{addDays(utcNow(), 1)}",
        "msdyn_scheduledstart": "@{utcNow()}",
        "msdyn_scheduledend": "@{addDays(utcNow(), 5)}",
        "msdyn_LinkStatus": "192350000"
    }
    ```

    להלן הסבר על הפרמטרים:

    - **\@\@odata.type** - שם הישות. לדוגמה, הזן **"Microsoft.Dynamics.CRM.msdyn\_projecttask"**.
    - **msdyn\_projecttaskid** – המזהה הייחודי של המשימה. יש להגדיר את הערך למשתנה דינמי מ- **msdyn\_projecttaskid**.
    - **msdyn\_project\@odata.bind** – מזהה הפרוייקט של פרוייקט הבעלות. הערך יהיה תוכן דינמי שמגיע מהתגובה של הצעד "יצירת פרוייקט". ודא שאתה מזין את הנתיב המלא ומוסף תוכן דינמי בין הסוגריים. יש צורך במירכאות. למשל, הזן **"/msdyn\_projects(הזן תוכן דינמי)"**.
    - **msdyn\_subject** – כל שם של משימה.
    - **msdyn\_projectbucket\@odata.bind** – מיכל הפרוייקט המכיל את המשימות. הערך יהיה תוכן דינמי שמגיע מהתגובה של הצעד "יצירת מיכל". ודא שאתה מזין את הנתיב המלא ומוסף תוכן דינמי בין הסוגריים. יש צורך במירכאות. למשל, הזן **"/msdyn\_projectbuckets(הוסף תוכן דינמי)"**.
    - **msdyn\_start** – תוכן דינמי עבור תאריך ההתחלה. לדוגמה, יום המחר מיוצג כ- **"addDays(utcNow(), 1)"**.
    - **msdyn\_scheduledstart** – תאריך ההתחלה המתוזמן. לדוגמה, יום המחר מיוצג כ- **"addDays(utcNow(), 1)"**.
    - **msdyn\_scheduleend** – תאריך הסיום המתוזמן. בחר תאריך בעתיד. למשל, ציין **"addDays(utcNow(), 5)"**.
    - **msdyn\_LinkStatus** – מצב הקישור. לדוגמה, הזן **"192350000"**.

7. עבור השדה **OperationSetId**, בחר **msdyn\_CreateOperationSetV1Response** בתיבת הדו-שיח **תוכן דינמי**.

## <a name="step-13-create-a-resource-assignment"></a><a id="13"></a>שלב 13: יצירת הקצאת משאבים

1. בזרימה, בחר **צעד חדש**.
2. בתיבת הדו-שיח **בחר פעולה** בשדה החיפוש, הזן **בצע פעולה לא מאוגדת**. לאחר מכן, בכרטיסיה **פעולות**, בחר את הפעולה ברשימת התוצאות.
3. בצעד, בחר שלוש נקודות (**...**) ולאחר מכן בחר **שנה שם**.
4. שנה את שם הצעד ל **יצירת הקצאה**.
5. בשדה **שם פעולה** בחר **msdyn\_PssCreateV1**.
6. בשדה **ישות**, הזן את פרטי הפרמטרים הבאים.

    ```
    {
        "@odata.type": "Microsoft.Dynamics.CRM.msdyn_resourceassignment",
        "msdyn_resourceassignmentid": "@{guid()}",
        "msdyn_name": "ScheduleAPIDemoAssign1",
        "msdyn_taskid@odata.bind": "/msdyn_projecttasks(@{variables('msdyn_projecttaskid')})",
        "msdyn_projectteamid@odata.bind": "/msdyn_projectteams(@{outputs('Create_Team_Member')?['body/TeamMemberId']})",
        "msdyn_projectid@odata.bind": "/msdyn_projects(@{outputs('Create_Project')?['body/ProjectId']})"
    }
    ```

7. עבור השדה **OperationSetId**, בחר **msdyn\_CreateOperationSetV1Response** בתיבת הדו-שיח **תוכן דינמי**.

## <a name="step-14-decrement-a-variable"></a><a id="14"></a>צעד 14: הקטנת משתנה

1. בזרימה, בחר **צעד חדש**.
2. בתיבת הדו-שיח **בחר פעולה** בשדה החיפוש, הזן **הקטן משתנה**. לאחר מכן, בכרטיסיה **פעולות**, בחר את הפעולה ברשימת התוצאות.
3. בשדה **שם**, בחר **מספר משימות**.
4. בשדה **ערך**, הזן **1**.

## <a name="step-15-rename-a-project-task"></a><a id="15"></a>צעד 15: שינוי שם של משימת פרוייקט

1. בזרימה, בחר **צעד חדש**.
2. בתיבת הדו-שיח **בחר פעולה** בשדה החיפוש, הזן **בצע פעולה לא מאוגדת**. לאחר מכן, בכרטיסיה **פעולות**, בחר את הפעולה ברשימת התוצאות.
3. בצעד, בחר שלוש נקודות (**...**) ולאחר מכן בחר **שנה שם**.
4. שנה את שם השלב ל **שינוי שם של משימת פרוייקט**.
5. בשדה **שם פעולה** בחר **msdyn\_PssUpdateV1**.
6. בשדה **ישות**, הזן את פרטי הפרמטרים הבאים.

    ```
    {
        "@@odata.type": "Microsoft.Dynamics.CRM.msdyn_projecttask",
        "msdyn_projecttaskid": "@{variables('msdyn_projecttaskid')}",
        "msdyn_subject": "ScheduleDemoTask1-UpdatedName"
    }
    ```

7. עבור השדה **OperationSetId**, בחר **msdyn\_CreateOperationSetV1Response** בתיבת הדו-שיח **תוכן דינמי**.

## <a name="step-16-run-an-operation-set"></a><a id="16"></a>צעד 16: הפעלת קבוצת פעולות

1. בזרימה, בחר **צעד חדש**.
2. בתיבת הדו-שיח **בחר פעולה** בשדה החיפוש, הזן **בצע פעולה לא מאוגדת**. לאחר מכן, בכרטיסיה **פעולות**, בחר את הפעולה ברשימת התוצאות.
3. בצעד, בחר שלוש נקודות (**...**) ולאחר מכן בחר **שנה שם**.
4. שנה את שם הצעד ל **ביצוע קבוצת פעולות**.
5. בשדה **שם פעולה** בחר **msdyn\_ExecuteOperationSetV1**.
6. עבור השדה **OperationSetId**, בחר **msdyn\_CreateOperationSetV1Response OperationSetId** בתיבת הדו-שיח **תוכן דינמי**.

## <a name="references"></a>הפניות

- [מבט כולל על אופן השילוב של זרמים עם Dataverse - Power Automate](/power-automate/dataverse/overview?WT.mc_id=email)
- [השתמש בממשקי API של לוח זמנים של הפרוייקט לביצוע פעולות עם ישויות תזמון](schedule-api-preview.md)
- [מבט כולל על זרימות הענן - Power Automate](/power-automate/overview-cloud?WT.mc_id=email)
- [מבט כולל על זרימות מוכנות לפתרון - Power Automate](/power-automate/overview-solution-flows?WT.mc_id=email)