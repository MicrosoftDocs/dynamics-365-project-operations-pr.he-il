---
title: השתמש בממשקי API של לוח זמנים של הפרוייקט לביצוע פעולות עם ישויות תזמון
description: מאמר זה מספק מידע ודוגמאות לשימוש בממשקי API של לוח זמנים של פרויקט.
author: sigitac
ms.date: 01/13/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 159d395efff98f2af780e5ed1e5ab3d6483cba89
ms.sourcegitcommit: b1c26ea57be721c5b0b1a33f2de0380ad102648f
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/20/2022
ms.locfileid: "9541125"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a>השתמש בממשקי API של לוח זמנים של הפרוייקט לביצוע פעולות עם ישויות תזמון

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_


**ישויות תזמון**

ממשקי API של לוח הזמנים של הפרוייקט מאפשרים לבצע פעולות יצירה, עדכון ומחיקה באמצעות **ישויות תזמון**. ישויות אלה מנוהלות דרך מנוע התזמון ב- Project for the Web. פעולות יצירה, עדכון ומחיקה בעזרת **ישויות תזמון** הוגבלו במהדרות הקודמות של Dynamics 365 Project Operations.

הטבלה הבאה מספקת רשימה מלאה של ישויות לוח הזמנים של הפרוייקט.

| **שם ישות**         | **שם לוגי של ישות**     |
|-------------------------|-----------------------------|
| פרויקט                 | msdyn_project               |
| משימת פרוייקט            | msdyn_projecttask           |
| ‏‫יחס תלות במשימת פרוייקט | msdyn_projecttaskdependency |
| הקצאת משאבים     | msdyn_resourceassignment    |
| מיכל של פרוייקט          | msdyn_projectbucket         |
| חבר צוות פרוייקט     | msdyn_projectteam           |
| רשימות פעולות של פרויקט      | msdyn_projectchecklist      |
| תווית הפרוייקט           | msdyn_projectlabel          |
| משימת פרוייקט לתווית   | msdyn_projecttasktolabel    |
| סבב פרוייקט          | msdyn_projectsprint         |

**OperationSet**

OperationSet הוא דפוס יחידת עבודה שניתן להשתמש בו כאשר יש לעבד מספר בקשות המשפיעות על לוחות זמנים במסגרת עסקה.

**ממשקי API ללוחות זמנים של פרוייקט**

להלן רשימה של ממשקי ה- API הנוכחיים של לוח הזמנים של פרוייקט.

| **API**                                 | תיאור‬‏‫‬                                                                                                                       |
|-----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| **msdyn_CreateProjectV1**               | ממשק API זה משמש ליצירת פרויקט. הפרוייקט ומיכל הפרוייקטים המוגדר כברירת מחדל נוצרים באופן מיידי.                         |
| **msdyn_CreateTeamMemberV1**            | ממשק API זה משמש ליצירת חבר צוות. רשומת חבר הצוות נוצרת באופן מיידי.                                  |
| **msdyn_CreateOperationSetV1**          | ממשק API זה משמש לתזמון מספר בקשות שיש לבצע במסגרת עסקה.                                        |
| **msdyn_PssCreateV1**                   | ממשק API זה משמש ליצירת ישות. הישות יכולה להיות כל אחת מישויות תזמון הפרוייקט התומכות בפעולת היצירה. |
| **msdyn_PssUpdateV1**                   | ממשק API זה משמש לעדכון ישות. הישות יכולה להיות כל אחת מישויות תזמון הפרוייקט התומכות בפעולת העדכון  |
| **msdyn_PssDeleteV1**                   | ממשק API זה משמש למחיקת ישות. הישות יכולה להיות כל אחת מישויות תזמון הפרוייקט התומכות בפעולת המחיקה. |
| **msdyn_ExecuteOperationSetV1**         | ממשק API זה משמש לביצוע כל הפעולות במסגרת קבוצת הפעולות הנתונה.                                                 |
| **msdyn_PssUpdateResourceAssignmentV1** | ממשק API זה משמש לעדכון קו מתאר עבודה מתוכנן של הקצאת משאבים.                                                        |



**שימוש בממשקי API של לוח הזמנים של הפרוייקט עם OperationSet**

מפני שהרשומות **CreateProjectV1** ו- **CreateTeamMemberV1** נוצרות באופן מיידי, לא ניתן להשתמש בממשקי API אלה ב- **OperationSet** ישירות. עם זאת, ניתן להשתמש ב- API כדי ליצור רשומות נדרשות, ליצור **OperationSet** ולאחר מכן להשתמש ברשומות אלה שנוצרו מראש ב- **OperationSet**.

**פעולות נתמכות**

| **ישות תזמון**   | **צור** | **עדכון** | **מחק** | **שיקולים חשובים:**                                                                                                                                                                                                                                                                                                                            |
|-------------------------|------------|------------|------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| משימת פרוייקט            | כן        | כן        | כן        | ניתן לערוך את השדות **התקדמות**, **EffortCompleted** ו- **EffortRemaining** ב- Project for the Web, אך לא ניתן לערוך אותם ב- Project Operations.                                                                                                                                                                                             |
| ‏‫יחס תלות במשימת פרוייקט | ‏‏כן‬        | כן         | ‏‏כן‬        | רשומות יחס תלות במשימת פרוייקט אינן מעודכנות. במקום זאת, ניתן למחוק רשומה ישנה וליצור רשומה חדשה.                                                                                                                                                                                                                                 |
| הקצאת משאבים     | ‏‏כן‬        | כן\*      | ‏‏כן‬        | פעולות עם השדות הבאים אינן נתמכות: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** ו- **PlannedWork**. רשומות הקצאת משאבים אינן מעודכנות. במקום זאת, ניתן למחוק את הרשומה הישנה וליצור רשומה חדשה. ממשק API נפרד סופק לצורך עדכון קווי המתאר של הקצאת משאבים. |
| מיכל של פרוייקט          | ‏‏כן‬        | ‏‏כן‬        | ‏‏כן‬        | מיכל ברירת המחדל נוצר באמצעות ממשק ה- API **CreateProjectV1**. תמיכה ביצירה ומחיקה של מיכלי פרוייקטים נוספה במהדורת עדכון 16.                                                                                                                                                                                                   |
| חבר צוות פרויקט     | כן        | כן        | כן        | לצורך פעולת היצירה, השתמש בממשק API **CreateTeamMemberV1**.                                                                                                                                                                                                                                                                                           |
| פרויקט                 | כן        | כן        |            | פעולות עם השדות הבאים אינן נתמכות: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** ו- **Duration**.                                                                                       |
| רשימות פעולות של פרויקט      | ‏‏כן‬        | ‏‏כן‬        | ‏‏כן‬        |                                                                                                                                                                                                                                                                                                                                                         |
| תווית הפרוייקט           | כן         | ‏‏כן‬        | כן         | ניתן לשנות את שמות התוויות. תכונה זו זמינה עבור Project for the Web בלבד.                                                                                                                                                                                                                                                                      |
| משימת פרוייקט לתווית   | ‏‏כן‬        | כן         | ‏‏כן‬        | תכונה זו זמינה עבור Project for the Web בלבד.                                                                                                                                                                                                                                                                                                  |
| סבב פרוייקט          | ‏‏כן‬        | ‏‏כן‬        | ‏‏כן‬        | השדה **התחלה** חייב להכיל תאריך מוקדם מהתאריך בשדה **סיום**. סבבים של אותו פרוייקט לא יכולים לחפוף זה עם זה. תכונה זו זמינה עבור Project for the Web בלבד.                                                                                                                                                                    |




מאפיין המזהה הוא אופציונלי. אם הוא מסופק, המערכת מנסה להשתמש בו ומציגה חריגה אם לא ניתן להשתמש בו. אם הוא לא מסופק, המערכת תיצור אותו.

**בעיות ומגבלות ידועות**

להלן רשימה של מגבלות ובעיות ידועות:

-   רק **משתמשים עם רישיון Microsoft Project** יכולים להשתמש בממשקי API של לוח הזמנים של פרוייקט. המשתמשים שיכולים להשתמש בהם:
    -   משתמשים ביישום
    -   משתמשי מערכת
    -   משתמשי שילוב
    -   משתמשים אחרים שאין להם את הרישיון הנדרש
-   כל **OperationSet** יכולה לבצע מקסימום 100 פעולות.
-   לכל משתמש יכולות להיות עד 10 **OperationSets** פתוחות.
-   Project Operations תומך כיום במקסימום 500 משימות בסה"כ לפרויקט.
-   כל פעולת עדכון קו מתאר של הקצאת משאבים נחשבת כפעולה בודדת.
-   כל רשימת קווי מתאר מעודכנים יכולה להכיל 100 פרוסות זמן לכל היותר.
-   מצב כשל של **OperationSet** ויומני כשל אינם זמינים כרגע.
-   יש מגבלת מקסימום של 400 סבבים לכל פרוייקט.
-   [מגבלות וגבולות בפרויקטים ובמשימות](/project-for-the-web/project-for-the-web-limits-and-boundaries).
-   התוויות זמינות כעת עבור Project for the Web בלבד.

**טיפול בשגיאות**

-   כדי לסקור שגיאות שנוצרו מערכי תפעול, עבור אל **גדרות** \> **שילוב תזמון** \> **מערכי תפעול**.
-   כדי לבדוק שגיאות שנוצרו משירות לוח הזמנים של הפרוייקט, עבור אל **הגדרות** \>**שילוב של לוח זמנים** \> **יומני שגיאה של PSS**.

**עריכת קווי מתאר של הקצאת משאבים**

שלא כמו ממשקי API אחרים לתזמון פרוייקט שמעדכנים ישות, ממשק ה- API לקו מתאר של הקצאת משאבים אחראי אך ורק על עדכונים בשדה יחיד, msdyn_plannedwork, בישות יחידה, msydn_resourceassignment.

מצב לוח זמנים נתון הוא:

-   **יחידות קבועות**
-   לוח השנה של הפרוייקט הוא 9-5P הוא 9-5 PST, שני, שלישי, חמישי, שישי (ללא עבודה בימי רביעי)
-   ולוח הזמנים של המשאבים הוא 9-1P‏ (PST), שני עד שישי

הקצאה זו היא עבור שבוע אחד, ארבע שעות ביום. הסיבה לכך היא שלוח השנה של המשאבים הוא בין 9-1 ‏(PST), או ארבע שעות ביום.

| &nbsp;     | משימה | תאריך התחלה | תאריך סיום  | כמות | 6/13/2022 | 6/14/2022 | 6/15/2022 | 6/16/2022 | 6/17/2022 |
|------------|------|------------|-----------|----------|-----------|-----------|-----------|-----------|-----------|
| עובד בשעות 9-1 |  T1  | 6/13/2022  | 6/17/2022 | 20       | 4         | 4         | 4         | 4         | 4         |

לדוגמה, אם אתה רוצה שהעובד יעבוד רק שלוש שעות בכל יום השבוע, ויקדיש שעה אחת למשימות אחרות.

#### <a name="updatedcontours-sample-payload"></a>מטען לדוגמא של UpdatedContours:

```json
[{

"minutes":900.0,

"start":"2022-06-13T00:00:00-07:00",

"end":"2022-06-18T00:00:00-07:00"

}]
```

זו ההקצאה לאחר הפעלת ממשק ה- API של Update Contour Schedule.

| &nbsp;     | משימה | תאריך התחלה | תאריך סיום  | כמות | 6/13/2022 | 6/14/2022 | 6/15/2022 | 6/16/2022 | 6/17/2022 |
|------------|------|------------|-----------|----------|-----------|-----------|-----------|-----------|-----------|
| עובד בשעות 9-1 | T1   | 6/13/2022  | 6/17/2022 | 15       | 3         | 3         | 3         | 3         | 3         |


**תרחיש לדוגמה**

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

** דוגמאות נוספות

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
