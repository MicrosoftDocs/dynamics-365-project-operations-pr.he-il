---
title: השתמש בממשקי API של לוח זמנים של הפרוייקט לביצוע פעולות עם ישויות תזמון
description: מאמר זה מספק מידע ודוגמאות לשימוש בממשקי API של לוח זמנים של פרויקט.
author: sigitac
ms.date: 01/13/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 3248a057b831d81fdc2bc198b4ed4da5e46462f2
ms.sourcegitcommit: 8edd24201cded2672cec16cd5dc84c6a3516b6c2
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/06/2022
ms.locfileid: "9230316"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a>השתמש בממשקי API של לוח זמנים של הפרוייקט לביצוע פעולות עם ישויות תזמון

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_



## <a name="scheduling-entities"></a>ישויות תזמון

ממשקי API של לוח הזמנים של הפרוייקט מאפשרים לבצע פעולות יצירה, עדכון ומחיקה באמצעות **ישויות תזמון**. ישויות אלה מנוהלות דרך מנוע התזמון ב- Project for the Web. פעולות יצירה, עדכון ומחיקה בעזרת **ישויות תזמון** הוגבלו במהדרות הקודמות של Dynamics 365 Project Operations.

הטבלה הבאה מספקת רשימה מלאה של ישויות לוח הזמנים של הפרוייקט.

| שם הישות  | שם לוגי של ישות |
| --- | --- |
| פרויקט | msdyn_project |
| משימת פרוייקט  | msdyn_projecttask  |
| ‏‫יחס תלות במשימת פרוייקט  | msdyn_projecttaskdependency  |
| הקצאת משאבים | msdyn_resourceassignment |
| מיכל של פרוייקט  | msdyn_projectbucket |
| חבר צוות פרוייקט | msdyn_projectteam |

## <a name="operationset"></a>OperationSet

OperationSet הוא דפוס יחידת עבודה שניתן להשתמש בו כאשר יש לעבד מספר בקשות המשפיעות על לוחות זמנים במסגרת עסקה.

## <a name="project-schedule-apis"></a>ממשקי API ללוחות זמנים של פרוייקט

להלן רשימה של ממשקי ה- API הנוכחיים של לוח הזמנים של פרוייקט.

- **msdyn_CreateProjectV1** : ניתן להשתמש בממשק API זה ליצירת פרויקט. הפרוייקט ומיכל הפרוייקטים המוגדר כברירת מחדל נוצרים באופן מיידי.
- **msdyn_CreateTeamMemberV1** : ניתן להשתמש בממשק API זה ליצירת חבר צוות פרוייקט. רשומת חבר הצוות נוצרת באופן מיידי.
- **msdyn_CreateOperationSetV1** : ניתן להשתמש בממשק API זה לתזמון מספר בקשות שיש לבצע במסגרת עסקה.
- **msdyn_PssCreateV1** : ניתן להשתמש בממשק API זה ליצירת ישות. הישות יכולה להיות כל אחת מישויות תזמון הפרוייקט התומכות בפעולת היצירה.
- **msdyn_PssUpdateV1**: ניתן להשתמש בממשק API זה לעדכון ישות. הישות יכולה להיות כל אחת מישויות תזמון הפרוייקט התומכות בפעולת העדכון.
- **msdyn_PssDeleteV1**: ניתן להשתמש בממשק API זה למחיקת ישות. הישות יכולה להיות כל אחת מישויות תזמון הפרוייקט התומכות בפעולת המחיקה.
- **msdyn_ExecuteOperationSetV1** : ממשק API זה משמש לביצוע כל הפעולות במסגרת קבוצת הפעולות הנתונה.

## <a name="using-project-schedule-apis-with-operationset"></a>שימוש בממשקי API של לוח הזמנים של הפרוייקט עם OperationSet

מפני שהרשומות **CreateProjectV1** ו- **CreateTeamMemberV1** נוצרות באופן מיידי, לא ניתן להשתמש בממשקי API אלה ב- **OperationSet** ישירות. עם זאת, ניתן להשתמש ב- API כדי ליצור רשומות נדרשות, ליצור **OperationSet** ולאחר מכן להשתמש ברשומות אלה שנוצרו מראש ב- **OperationSet**.

## <a name="supported-operations"></a>פעולות נתמכות

| ישות תזמון | צור | עדכן | מחק | שיקולים חשובים: |
| --- | --- | --- | --- | --- |
משימת פרוייקט | כן | כן | כן | ניתן לערוך את השדות **התקדמות**, **EffortCompleted** ו- **EffortRemaining** ב- Project for the Web, אך לא ניתן לערוך אותם ב- Project Operations.  |
| ‏‫יחס תלות במשימת פרוייקט | כן |  | כן | רשומות יחס תלות במשימת פרוייקט אינן מעודכנות. במקום זאת, ניתן למחוק רשומה ישנה וליצור רשומה חדשה. |
| הקצאת משאבים | כן | כן | | פעולות עם השדות הבאים אינן נתמכות: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** ו- **PlannedWork**. רשומות הקצאת משאבים אינן מעודכנות. במקום זאת, ניתן למחוק את הרשומה הישנה וליצור רשומה חדשה. |
| מיכל של פרוייקט | כן | כן | כן | מיכל ברירת המחדל נוצר באמצעות ממשק ה- API **CreateProjectV1**. תמיכה ביצירה ומחיקה של מיכלי פרוייקטים נוספה במהדורת עדכון 16. |
| חבר צוות פרויקט | כן | כן | כן | לצורך פעולת היצירה, השתמש בממשק API **CreateTeamMemberV1**. |
| פרויקט | כן | כן |  | פעולות עם השדות הבאים אינן נתמכות: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** ו- **Duration**. |

ניתן לקרוא לממשקי API אלה באמצעות אובייקטים של ישויות הכוללים שדות מותאמים אישית.

מאפיין המזהה הוא אופציונלי. אם הוא מסופק, המערכת מנסה להשתמש בו ומציגה חריגה אם לא ניתן להשתמש בו. אם הוא לא מסופק, המערכת תיצור אותו.

## <a name="restricted-fields"></a>שדות מוגבלים

הטבלאות הבאות מגדירות את השדות שהאפשרויות **יצירה** ו **עריכה** מוגבלות בהם.

### <a name="project-task"></a>משימת פרוייקט

| שם לוגי                           | אפשר ליצור     | יכול לערוך         |
|----------------------------------------|----------------|------------------|
| msdyn_actualcost                       | כן             | כן               |
| msdyn_actualcost_base                  | כן             | כן               |
| msdyn_actualend                        | כן             | כן               |
| msdyn_actualsales                      | כן             | כן               |
| msdyn_actualsales_base                 | כן             | כן               |
| msdyn_actualstart                      | כן             | כן               |
| msdyn_costatcompleteestimate           | כן             | כן               |
| msdyn_costatcompleteestimate_base      | כן             | כן               |
| msdyn_costconsumptionpercentage        | כן             | כן               |
| msdyn_effortcompleted                  | לא (כן עבור פרוייקט)             | לא (כן עבור פרוייקט)               |
| msdyn_effortremaining                  | לא (כן עבור פרוייקט)              | לא (כן עבור פרוייקט)                |
| msdyn_effortestimateatcomplete         | כן             | כן               |
| msdyn_iscritical                       | כן             | כן               |
| msdyn_iscriticalname                   | כן             | כן               |
| msdyn_ismanual                         | כן             | כן               |
| msdyn_ismanualname                     | כן             | כן               |
| msdyn_ismilestone                      | כן             | כן               |
| msdyn_ismilestonename                  | כן             | כן               |
| msdyn_LinkStatus                       | כן             | כן               |
| msdyn_linkstatusname                   | כן             | כן               |
| msdyn_msprojectclientid                | כן             | כן               |
| msdyn_plannedcost                      | כן             | כן               |
| msdyn_plannedcost_base                 | כן             | כן               |
| msdyn_plannedsales                     | כן             | כן               |
| msdyn_plannedsales_base                | כן             | כן               |
| msdyn_pluginprocessingdata             | כן             | כן               |
| msdyn_progress                         | לא (כן עבור פרוייקט)             | לא (כן עבור פרוייקט) |
| msdyn_remainingcost                    | כן             | כן               |
| msdyn_remainingcost_base               | כן             | כן               |
| msdyn_remainingsales                   | כן             | כן               |
| msdyn_remainingsales_base              | כן             | כן               |
| msdyn_requestedhours                   | כן             | כן               |
| msdyn_resourcecategory                 | כן             | כן               |
| msdyn_resourcecategoryname             | כן             | כן               |
| msdyn_resourceorganizationalunitid     | כן             | כן               |
| msdyn_resourceorganizationalunitidname | כן             | כן               |
| msdyn_salesconsumptionpercentage       | כן             | כן               |
| msdyn_salesestimateatcomplete          | כן             | כן               |
| msdyn_salesestimateatcomplete_base     | כן             | כן               |
| msdyn_salesvariance                    | כן             | כן               |
| msdyn_salesvariance_base               | כן             | כן               |
| msdyn_scheduleddurationminutes         | כן             | כן               |
| msdyn_scheduledend                     | כן             | כן               |
| msdyn_scheduledstart                   | כן             | כן               |
| msdyn_schedulevariance                 | כן             | כן               |
| msdyn_skipupdateestimateline           | כן             | כן               |
| msdyn_skipupdateestimatelinename       | כן             | כן               |
| msdyn_summary                          | כן             | כן               |
| msdyn_varianceofcost                   | כן             | כן               |
| msdyn_varianceofcost_base              | כן             | כן               |

### <a name="project-task-dependency"></a>‏‫יחס תלות במשימת פרוייקט

| שם לוגי                  | אפשר ליצור     | יכול לערוך     |
|-------------------------------|----------------|--------------|
| msdyn_linktype                | כן             | כן           |
| msdyn_linktypename            | כן             | כן           |
| msdyn_predcessortask         | כן            | כן           |
| msdyn_predecessortaskname     | כן            | כן           |
| msdyn_project                 | כן            | כן           |
| msdyn_projectname             | כן            | כן           |
| msdyn_projecttaskdependencyid | כן            | כן           |
| msdyn_successortask           | כן            | כן           |
| msdyn_successortaskname       | כן            | כן           |

### <a name="resource-assignment"></a>הקצאת משאבים

| שם לוגי                 | אפשר ליצור     | יכול לערוך     |
|------------------------------|----------------|--------------|
| msdyn_bookableresourceid     | כן            | כן           |
| msdyn_bookableresourceidname | כן            | כן           |
| msdyn_bookingstatusid        | כן             | כן           |
| msdyn_bookingstatusidname    | כן             | כן           |
| msdyn_committype             | כן             | כן           |
| msdyn_committypename         | כן             | כן           |
| msdyn_effort                 | כן             | כן           |
| msdyn_effortcompleted        | כן             | כן           |
| msdyn_effortremaining        | כן             | כן           |
| msdyn_finish                 | כן             | כן           |
| msdyn_plannedcost            | כן             | כן           |
| msdyn_plannedcost_base       | כן             | כן           |
| msdyn_plannedcostcontour     | כן             | כן           |
| msdyn_plannedsales           | כן             | כן           |
| msdyn_plannedsales_base      | כן             | כן           |
| msdyn_plannedsalescontour    | כן             | כן           |
| msdyn_plannedwork            | כן             | כן           |
| msdyn_projectid              | כן            | כן           |
| msdyn_projectidname          | כן             | כן           |
| msdyn_projectteamid          | כן             | כן           |
| msdyn_projectteamidname      | כן             | כן           |
| msdyn_start                  | כן             | כן           |
| msdyn_taskid                 | כן             | כן           |
| msdyn_taskidname             | כן             | כן           |
| msdyn_userresourceid         | כן             | כן           |

### <a name="project-team-member"></a>חבר צוות פרויקט

| שם לוגי                                     | אפשר ליצור     | יכול לערוך     |
|--------------------------------------------------|----------------|--------------|
| msdyn_calendarid                                 | כן             | כן           |
| msdyn_creategenericteammemberwithrequirementname | כן             | כן           |
| msdyn_deletestatus                               | כן             | כן           |
| msdyn_deletestatusname                           | כן             | כן           |
| msdyn_effort                                     | כן             | כן           |
| msdyn_effortcompleted                            | כן             | כן           |
| msdyn_effortremaining                            | כן             | כן           |
| msdyn_finish                                     | כן             | כן           |
| msdyn_hardbookedhours                            | כן             | כן           |
| msdyn_hours                                      | כן             | כן           |
| msdyn_markedfordeletiontimer                     | כן             | כן           |
| msdyn_markedfordeletiontimestamp                 | כן             | כן           |
| msdyn_msprojectclientid                          | כן             | כן           |
| msdyn_percentage                                 | כן             | כן           |
| msdyn_requiredhours                              | כן             | כן           |
| msdyn_softbookedhours                            | כן             | כן           |
| msdyn_start                                      | כן             | כן           |

### <a name="project"></a>פרויקט

| שם לוגי                           | אפשר ליצור     | יכול לערוך     |
|----------------------------------------|----------------|--------------|
| msdyn_actualexpensecost                | כן             | כן           |
| msdyn_actualexpensecost_base           | כן             | כן           |
| msdyn_actuallaborcost                  | כן             | כן           |
| msdyn_actuallaborcost_base             | כן             | כן           |
| msdyn_actualsales                      | כן             | כן           |
| msdyn_actualsales_base                 | כן             | כן           |
| msdyn_contractlineproject              | כן            | כן           |
| msdyn_contractorganizationalunitid     | כן            | כן           |
| msdyn_contractorganizationalunitidname | כן            | כן           |
| msdyn_costconsumption                  | כן             | כן           |
| msdyn_costestimateatcomplete           | כן             | כן           |
| msdyn_costestimateatcomplete_base      | כן             | כן           |
| msdyn_costvariance                     | כן             | כן           |
| msdyn_costvariance_base                | כן             | כן           |
| msdyn_duration                         | כן             | כן           |
| msdyn_effort                           | כן             | כן           |
| msdyn_effortcompleted                  | כן             | כן           |
| msdyn_effortestimateatcompleteeac      | כן             | כן           |
| msdyn_effortremaining                  | כן             | כן           |
| msdyn_finish                           | כן            | כן          |
| msdyn_globalrevisiontoken              | כן             | כן           |
| msdyn_islinkedtomsprojectclient        | כן             | כן           |
| msdyn_islinkedtomsprojectclientname    | כן             | כן           |
| msdyn_linkeddocumenturl                | כן             | כן           |
| msdyn_msprojectdocument                | כן             | כן           |
| msdyn_msprojectdocumentname            | כן             | כן           |
| msdyn_plannedexpensecost               | כן             | כן           |
| msdyn_plannedexpensecost_base          | כן             | כן           |
| msdyn_plannedlaborcost                 | כן             | כן           |
| msdyn_plannedlaborcost_base            | כן             | כן           |
| msdyn_plannedsales                     | כן             | כן           |
| msdyn_plannedsales_base                | כן             | כן           |
| msdyn_progress                         | כן             | כן           |
| msdyn_remainingcost                    | כן             | כן           |
| msdyn_remainingcost_base               | כן             | כן           |
| msdyn_remainingsales                   | כן             | כן           |
| msdyn_remainingsales_base              | כן             | כן           |
| msdyn_replaylogheader                  | כן             | כן           |
| msdyn_salesconsumption                 | כן             | כן           |
| msdyn_salesestimateatcompleteeac       | כן             | כן           |
| msdyn_salesestimateatcomplete_base  | כן             | כן           |
| msdyn_salesvariance                    | כן             | כן           |
| msdyn_salesvariance_base               | כן             | כן           |
| msdyn_scheduleperformance              | כן             | כן           |
| msdyn_scheduleperformancename          | כן             | כן           |
| msdyn_schedulevariance                 | כן             | כן           |
| msdyn_taskearlieststart                | כן             | כן           |
| msdyn_teamsize                         | כן             | כן           |
| msdyn_teamsize_date                    | כן             | כן           |
| msdyn_teamsize_state                   | כן             | כן           |
| msdyn_totalactualcost                  | כן             | כן           |
| msdyn_totalactualcost_base             | כן             | כן           |
| msdyn_totalplannedcost                 | כן             | כן           |
| msdyn_totalplannedcost_base            | כן             | כן           |

### <a name="project-bucket"></a>מיכל של פרוייקט

| שם לוגי          | אפשר ליצור      | יכול לערוך     |
|-----------------------|-----------------|--------------|
| msdyn_displayorder    | כן             | כן           |
| msdyn_name            | כן             | כן          |
| msdyn_project         | כן             | כן           |
| msdyn_projectbucketid | כן             | כן           |

## <a name="limitations-and-known-issues"></a>בעיות ומגבלות ידועות
להלן רשימה של מגבלות ובעיות ידועות:

- רק **משתמשים עם רישיון Microsoft Project** יכולים להשתמש בממשקי API של לוח הזמנים של פרוייקט. המשתמשים שיכולים להשתמש בהם:

    - משתמשים ביישום
    - משתמשי מערכת
    - משתמשי שילוב
    - משתמשים אחרים שאין להם את הרישיון הנדרש

- כל **OperationSet** יכולה לבצע מקסימום 100 פעולות.
- לכל משתמש יכולות להיות עד 10 **OperationSets** פתוחות.
- Project Operations תומך כיום במקסימום 500 משימות בסה"כ לפרויקט.
- מצב כשל של **OperationSet** ויומני כשל אינם זמינים כרגע.
- [מגבלות וגבולות בפרויקטים ובמשימות](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a>טיפול בשגיאות

- כדי לסקור שגיאות שנוצרו מערכי תפעול, עבור אל **גדרות** \> **שילוב תזמון** \> **מערכי תפעול**.
- כדי לבדוק שגיאות שנוצרו משירות לוח הזמנים של הפרוייקט, עבור אל **הגדרות** \>**שילוב של לוח זמנים** \> **יומני שגיאה של PSS**.

## <a name="sample-scenario"></a>תרחיש לדוגמה

בתרחיש זה, תיצור פרויקט, חבר צוות, ארבע משימות ושתי הקצאות משאבים. לאחר מכן, תעדכן משימה אחת, תעדכן את הפרויקט, תמחק משימה אחת, תמחק הקצאת משאבים אחת ותיצור תלות במשימה.

```csharp
Entity project = CreateProject();
project.Id = CallCreateProjectAction(project);
var projectReference = project.ToEntityReference();

var teamMember = new Entity("msdyn_projectteam", Guid.NewGuid());
teamMember["msdyn_name"] = $"TM {DateTime.Now.ToShortTimeString()}";
teamMember["msdyn_project"] = projectReference;
var createTeamMemberResponse = CallCreateTeamMemberAction(teamMember);

var description = $"My demo {DateTime.Now.ToShortTimeString()}";
var operationSetId = CallCreateOperationSetAction(project.Id, description);

var task1 = GetTask("1WW", projectReference);
var task2 = GetTask("2XX", projectReference, task1.ToEntityReference());
var task3 = GetTask("3YY", projectReference);
var task4 = GetTask("4ZZ", projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment("R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

var assignment1Response = CallPssCreateAction(assignment1, operationSetId);
var assignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

var assignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a>דוגמאות נוספות

```csharp
#region Call actions --- Sample code ----

/// <summary>
/// Calls the action to create an operationSet
/// </summary>
/// <param name="projectId">project id for the operations to be included in this operationSet</param>
/// <param name="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
private string CallCreateOperationSetAction(Guid projectId, string description)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_CreateOperationSetV1");
    operationSetRequest["ProjectId"] = projectId.ToString();
    operationSetRequest["Description"] = description;
    OrganizationResponse response = organizationService.Execute(operationSetRequest);
    return response["OperationSetId"].ToString();
}

/// <summary>
/// Calls the action to create an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>

private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssUpdateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssUpdateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="recordId">Id of the record to be deleted</param>
/// <param name="entityLogicalName">Entity logical name of the record</param>
/// <param name="operationSetId">OperationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssDeleteAction(string recordId, string entityLogicalName, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssDeleteV1");
    operationSetRequest["RecordId"] = recordId;
    operationSetRequest["EntityLogicalName"] = entityLogicalName;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to execute requests in an operationSet
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallExecuteOperationSetAction(string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_ExecuteOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// This can be used to abandon an operationSet that is no longer needed
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
protected OperationSetResponse CallAbandonOperationSetAction(Guid operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_AbandonOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId.ToString();
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}


/// <summary>
/// Calls the action to create a new project
/// </summary>
/// <param name="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1");
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);
    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <param name="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
private string CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject<OperationSetResponse>((string)orgResponse.Results["OperationSetResponse"]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet("msdyn_project", "msdyn_name");
    var getDefaultBucket = new QueryExpression("msdyn_projectbucket")
    {
        ColumnSet = columnsToFetch,
        Criteria =
        {
            Conditions =
            {
                new ConditionExpression("msdyn_project", ConditionOperator.Equal, projectReference.Id),
                new ConditionExpression("msdyn_name", ConditionOperator.Equal, "Bucket 1")
            }
        }
    };

    return organizationService.RetrieveMultiple(getDefaultBucket);
}

private Entity GetBucket(EntityReference projectReference)
{
    var bucketCollection = GetDefaultBucket(projectReference);
    if (bucketCollection.Entities.Count > 0)
    {
        return bucketCollection[0].ToEntity<Entity>();
    }

    throw new Exception($"Please open project with id {projectReference.Id} in the Dynamics UI and navigate to the Tasks tab");
}

private Entity CreateProject()
{
    var project = new Entity("msdyn_project", Guid.NewGuid());
    project["msdyn_subject"] = $"Proj {DateTime.Now.ToShortTimeString()}";

    return project;
}



private Entity GetTask(string name, EntityReference projectReference, EntityReference parentReference = null)
{
    var task = new Entity("msdyn_projecttask", Guid.NewGuid());
    task["msdyn_project"] = projectReference;
    task["msdyn_subject"] = name;
    task["msdyn_effort"] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
    task["new_custom1"] = "Just my test";
    task["new_age"] = 98;
    task["new_amount"] = 591.34m;
    task["new_isready"] = new OptionSetValue(100000000);
    */

    if (parentReference == null)
    {
        task["msdyn_outlinelevel"] = 1;
    }
    else
    {
        task["msdyn_parenttask"] = parentReference;
    }

    return task;
}

private Entity GetResourceAssignment(string name, Entity teamMember, Entity task, Entity project)
{
    var assignment = new Entity("msdyn_resourceassignment", Guid.NewGuid());
    assignment["msdyn_projectteamid"] = teamMember.ToEntityReference();
    assignment["msdyn_taskid"] = task.ToEntityReference();
    assignment["msdyn_projectid"] = project.ToEntityReference();
    assignment["msdyn_name"] = name;
   
    return assignment;
}

protected Entity GetTaskDependency(Entity project, Entity predecessor, Entity successor)
{
    var taskDependency = new Entity("msdyn_projecttaskdependency", Guid.NewGuid());
    taskDependency["msdyn_project"] = project.ToEntityReference();
    taskDependency["msdyn_predecessortask"] = predecessor.ToEntityReference();
    taskDependency["msdyn_successortask"] = successor.ToEntityReference();
    taskDependency["msdyn_linktype"] = new OptionSetValue(192350000);

    return taskDependency;
}

#endregion


#region OperationSetResponse DataContract --- Sample code ----

[DataContract]
public class OperationSetResponse
{
[DataMember(Name = "operationSetId")]
public Guid OperationSetId { get; set; }

[DataMember(Name = "operationSetDetailId")]
public Guid OperationSetDetailId { get; set; }

[DataMember(Name = "operationType")]
public string OperationType { get; set; }

[DataMember(Name = "recordId")]
public string RecordId { get; set; }

[DataMember(Name = "correlationId")]
public string CorrelationId { get; set; }
}

#endregion
```
