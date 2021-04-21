---
title: שימוש בממשקי API של לוח זמנים לביצוע פעולות דרך ישויות תזמון
description: נושא זה מספק מידע ודוגמאות לשימוש בממשקי API של לוח זמנים.
author: sigitac
manager: Annbe
ms.date: 04/07/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a50a2c6220bb49de8146d0758019827e120e0526
ms.sourcegitcommit: 8ff9fe396db6dec581c21cd6bb9acc2691c815b0
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/07/2021
ms.locfileid: "5868130"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a>שימוש בממשקי API של לוח זמנים לביצוע פעולות דרך ישויות תזמון

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

> [!IMPORTANT] 
> כל הפונקציונליות או חלק ממנה המצוינת בנושא זה זמינה כחלק ממהדורת Preview. התוכן והפונקציונליות כפופים לשינויים. 

## <a name="scheduling-entities"></a>ישויות תזמון

ממשקי API של לוח הזמנים מאפשרים לבצע פעולות יצירה, עדכון ומחיקה בעזרת **ישויות תזמון**. ישויות אלה מנוהלות דרך מנוע התזמון ב- Project for the Web. פעולות יצירה, עדכון ומחיקה בעזרת **ישויות תזמון** הוגבלו במהדרות הקודמות של Dynamics 365 Project Operations.

הטבלה הבאה מספקת רשימה מלאה של **ישויות התזמון**.

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

## <a name="schedule-apis"></a>ממשקי API של לוח זמנים

להלן רשימה של ממשקי API נוכחיים של לוח זמנים.

- **msdyn_CreateProjectV1** : ניתן להשתמש בממשק API זה ליצירת פרויקט. הפרויקט ומיכל הפרויקט המוגדר כברירת מחדל נוצרים באופן מיידי.
- **msdyn_CreateTeamMemberV1** : ניתן להשתמש בממשק API זה ליצירת חבר צוות פרוייקט. רשומת חבר הצוות נוצרת באופן מיידי.
- **msdyn_CreateOperationSetV1** : ניתן להשתמש בממשק API זה לתזמון מספר בקשות שיש לבצע במסגרת עסקה.
- **msdyn_PSSCreateV1** : ניתן להשתמש בממשק API זה ליצירת ישות. הישות יכולה להיות כל אחת מיישויות התזמון התומכות בפעולת היצירה.
- **msdyn_PSSUpdateV1**: ניתן להשתמש בממשק API זה לעדכון ישות. הישות יכולה להיות כל אחת מיישויות התזמון התומכות בפעולת העדכון.
- **msdyn_PSSDeleteV1**: ניתן להשתמש בממשק API זה למחיקת ישות. הישות יכולה להיות כל אחת מיישויות התזמון התומכות בפעולת המחיקה.
- **msdyn_ExecuteOperationSetV1** : ממשק API זה משמש לביצוע כל הפעולות במסגרת קבוצת הפעולות הנתונה.

## <a name="using-schedule-apis-with-operationset"></a>שימוש בממשקי API של לוח זמנים עם OperationSet

מפני שהרשומות **CreateProjectV1** ו- **CreateTeamMemberV1** נוצרות באופן מיידי, לא ניתן להשתמש בממשקי API אלה ב- **OperationSet** ישירות. עם זאת, ניתן להשתמש ב- API כדי ליצור רשומות נדרשות, ליצור **OperationSet** ולאחר מכן להשתמש ברשומות אלה שנוצרו מראש ב- **OperationSet**.

## <a name="supported-operations"></a>פעולות נתמכות

| ישות תזמון | צור | עדכון | DELETE | שיקולים חשובים: |
| --- | --- | --- | --- | --- |
משימת פרוייקט | ‏‏כן | ‏‏כן | ‏‏כן | ללא |
| ‏‫יחס תלות במשימת פרוייקט | ‏‏כן | ‏‏כן | | רשומות יחס תלות במשימת פרוייקט אינן מעודכנות. במקום זאת, ניתן למחוק רשומה ישנה וליצור רשומה חדשה. |
| הקצאת משאבים | ‏‏כן | ‏‏כן | | פעולות עם השדות הבאים אינן נתמכות: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** ו- **PlannedWork**. רשומות הקצאת משאבים אינן מעודכנות. במקום זאת, ניתן למחוק את הרשומה הישנה וליצור רשומה חדשה. |
| מיכל של פרוייקט | לא זמין | לא זמין | לא זמין | מיכל ברירת המחדל נוצר באמצעות ממשק ה- API **CreateProjectV1**. |
| חבר צוות פרויקט | ‏‏כן | ‏‏כן | ‏‏כן | לצורך פעולת היצירה, השתמש בממשק API **CreateTeamMemberV1**. |
| פרויקט | ‏‏כן | ‏‏כן | לא זמין | פעולות עם השדות הבאים אינן נתמכות: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** ו- **Duration**. |

ניתן לקרוא לממשקי API אלה באמצעות אובייקטים של ישויות הכוללים שדות מותאמים אישית.

מאפיין המזהה הוא אופציונלי. אם הוא מסופק, המערכת מנסה להשתמש בו ומציגה חריגה אם לא ניתן להשתמש בו. אם הוא לא מסופק, המערכת תיצור אותו.

## <a name="limitations-and-known-issues"></a>בעיות ומגבלות ידועות
להלן רשימה של מגבלות ובעיות ידועות:

- רק **משתמשים עם רישיון ל-Microsoft Project License** יכולים להשתמש בממשקי API של לוח הזמנים. המשתמשים שיכולים להשתמש בהם:
    - משתמשים ביישום
    - משתמשי מערכת
    - משתמשי שילוב
    - משתמשים אחרים שאין להם את הרישיון הנדרש
- כל **OperationSet** יכולה לבצע מקסימום 100 פעולות.
- לכל משתמש יכולות להיות עד 10 **OperationSets** פתוחות.
- Project Operations תומך כיום במקסימום 500 משימות בסה"כ לפרויקט.
- מצב כשל של **OperationSet** ויומני כשל אינם זמינים כרגע.
- ממשקי API של לוח זמנים הם כרגע במהדורת Public Preview. השימוש בממשקי API אלה בסביבת ייצור אינו נתמך על ידי Microsoft.

## <a name="sample-scenario"></a>תרחיש לדוגמה

בתרחיש זה, תיצור פרויקט, חבר צוות, ארבע משימות ושתי הקצאות משאבים. לאחר מכן, תעדכן משימה אחת, תעדכן את הפרויקט, תמחק משימה אחת, תמחק הקצאת משאבים אחת ותיצור תלות במשימה.

```C#
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
var task4 = GetTask("4ZZ";, projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment"R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

varassignment1Response = CallPssCreateAction(assignment1, operationSetId);
varassignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

varassignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a>דוגמאות נוספות

```C#
#region Call actions 

///<summary>
/// Calls the action to create an operationSet
/// </summary>
/// <paramname="projectId">project id for the operations to be included in this operationSet>/param>
/// <paramname="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
privatestring CallCreateOperationSetAction(Guid projectId, string description)
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
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary<
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet Id</param>
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
/// <summary>
/// <paramname="recordId">Id of the record to be deleted</param>
/// <paramname="entityLogicalName">Entity logical name of the record</param>
/// <paramname="operationSetId">OperationSet Id</param>
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
/// <summary>
/// <paramname="operationSetId">operationSet id</param>
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
/// <paramname="operationSetId">operationSet id</param>
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
/// <paramname="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1";
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);

    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <paramname="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
privatestring CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject><OperationSetResponse>
    ((string)orgResponse.Results["OperationSetResponse";]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet(";msdyn_project", "msdyn_name");
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
    task["msdyn_effort";] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
        task["new_custom1"] = "Just my test";
        task[";new_age"] = 98;
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
    assignment["msdyn_start"] = DateTime.Now;
    assignment["msdyn_finish"] = DateTime.Now;
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
publicclassOperationSetResponse
{
    [DataMember(Name = "operationSetId")]
    public Guid OperationSetId { get; set; }

    [DataMember(Name = "operationSetDetailId")]
    public Guid OperationSetDetailId { get; set; }

    [DataMember(Name = "operationType")]
    publicstring OperationType { get; set; }

    [DataMember(Name = "recordId")]
    publicstring RecordId { get; set; }

    [DataMember(Name = "correlationId")]
    publicstring CorrelationId { get; set; }
}

#endregion
```
