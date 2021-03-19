---
title: פיתוח תבניות פרוייקט בעזרת 'העתק פרוייקט'
description: נושא זה מספק מידע על אופן יצירת תבניות פרוייקט באמצעות הפעולה המותאמת אישית העתק פרויקט.
author: stsporen
manager: Annbe
ms.date: 01/21/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 27847575e2d6ec9af77d24f756b13d3aeb0efea7
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286924"
---
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="eb662-103">פיתוח תבניות פרוייקט בעזרת 'העתק פרוייקט'</span><span class="sxs-lookup"><span data-stu-id="eb662-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="eb662-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="eb662-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="eb662-105">Dynamics 365 Project Operations תומך ביכולת להעתיק פרויקט ולהחזיר כל משימה למשאבים הגנריים המייצגים את התפקיד.</span><span class="sxs-lookup"><span data-stu-id="eb662-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="eb662-106">לקוחות יכולים להשתמש בפונקציונליות זו לבניית תבניות פרוייקט בסיסיות.</span><span class="sxs-lookup"><span data-stu-id="eb662-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="eb662-107">כשבוחרים **העתק פרויקט**, מצב פרויקט היעד מתעדכן.</span><span class="sxs-lookup"><span data-stu-id="eb662-107">When you select **Copy Project**, the status of the target project is updated.</span></span> <span data-ttu-id="eb662-108">השתמש ב **סיבת המצב** כדי לקבוע מתי הושלמה פעולת ההעתקה.</span><span class="sxs-lookup"><span data-stu-id="eb662-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="eb662-109">בחירה ב **העתק פרויקט** מעדכן גם את תאריך ההתחלה של הפרויקט לתאריך ההתחלה הנוכחי אם לא מזוהה תאריך יעד בישות פרויקט היעד.</span><span class="sxs-lookup"><span data-stu-id="eb662-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="eb662-110">פעולה מותאמת אישית 'העתק פרויקט'</span><span class="sxs-lookup"><span data-stu-id="eb662-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="eb662-111">שם</span><span class="sxs-lookup"><span data-stu-id="eb662-111">Name</span></span> 

<span data-ttu-id="eb662-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="eb662-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="eb662-113">פרמטרי קלט</span><span class="sxs-lookup"><span data-stu-id="eb662-113">Input parameters</span></span>
<span data-ttu-id="eb662-114">ישנם ‏שלושה פרמטרי קלט:</span><span class="sxs-lookup"><span data-stu-id="eb662-114">There are three input parameters:</span></span>

| <span data-ttu-id="eb662-115">פרמטר</span><span class="sxs-lookup"><span data-stu-id="eb662-115">Parameter</span></span>          | <span data-ttu-id="eb662-116">סוג</span><span class="sxs-lookup"><span data-stu-id="eb662-116">Type</span></span>   | <span data-ttu-id="eb662-117">ערכים</span><span class="sxs-lookup"><span data-stu-id="eb662-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="eb662-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="eb662-118">ProjectCopyOption</span></span>  | <span data-ttu-id="eb662-119">String</span><span class="sxs-lookup"><span data-stu-id="eb662-119">String</span></span> | <span data-ttu-id="eb662-120">**{"removeNamedResources":true}** או **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="eb662-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="eb662-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="eb662-121">SourceProject</span></span>      | <span data-ttu-id="eb662-122">הפניית ישות</span><span class="sxs-lookup"><span data-stu-id="eb662-122">Entity Reference</span></span> | <span data-ttu-id="eb662-123">פרויקט מקור</span><span class="sxs-lookup"><span data-stu-id="eb662-123">Source Project</span></span> |
| <span data-ttu-id="eb662-124">יעד</span><span class="sxs-lookup"><span data-stu-id="eb662-124">Target</span></span>             | <span data-ttu-id="eb662-125">הפניית ישות</span><span class="sxs-lookup"><span data-stu-id="eb662-125">Entity Reference</span></span> | <span data-ttu-id="eb662-126">פרויקט יעד</span><span class="sxs-lookup"><span data-stu-id="eb662-126">Target Project</span></span> |


- <span data-ttu-id="eb662-127">**{"clearTeamsAndAssignments":true}**: התנהגות ברירת המחדל עבור Project באינטרנט ותסיר את כל ההקצאות וחברי הצוות..</span><span class="sxs-lookup"><span data-stu-id="eb662-127">**{"clearTeamsAndAssignments":true}**: Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="eb662-128">**{"removeNamedResources":true}** אופן הפעולה המהווה ברירת המחדל ב-Project Operations שיחזיר את ההקצאות למשאבים כלליים.</span><span class="sxs-lookup"><span data-stu-id="eb662-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="eb662-129">לקבלת מידע נוסף על פעולות ברירת מחדל נוספיות, ראה [שימוש בפולות Web API](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span><span class="sxs-lookup"><span data-stu-id="eb662-129">For more defaults on actions, see [Use Web API actions](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="eb662-130">ציון שדות להעתקה</span><span class="sxs-lookup"><span data-stu-id="eb662-130">Specify fields to copy</span></span> 
<span data-ttu-id="eb662-131">כאשר נקראת הפעולה, **העתק פרויקט** יבדק את תצוגת הפרויקט **העתק עמודות פרוייקט** כדי לקבוע אילו שדות יש להעתיק בעת העתקת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="eb662-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>


### <a name="example"></a><span data-ttu-id="eb662-132">דוגמה</span><span class="sxs-lookup"><span data-stu-id="eb662-132">Example</span></span>
<span data-ttu-id="eb662-133">הדוגמה הבאה מראה כיצד להתקשר לפעולה מותאמת אישית **CopyProject** עם ערכת הפרמטרים **removeNamedResources**.</span><span class="sxs-lookup"><span data-stu-id="eb662-133">The following example shows how to call the **CopyProject** custom action with the **removeNamedResources** parameter set.</span></span>
```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

    [DataContract]
    public class ProjectCopyOption
    {
        /// <summary>
        /// Clear teams and assignments.
        /// </summary>
        [DataMember(Name = "clearTeamsAndAssignments")]
        public bool ClearTeamsAndAssignments { get; set; }

        /// <summary>
        /// Replace named resource with generic resource.
        /// </summary>
        [DataMember(Name = "removeNamedResources")]
        public bool ReplaceNamedResources { get; set; }
    }

    public class CopyProjectSample
    {
        private IOrganizationService organizationService;

        public CopyProjectSample(IOrganizationService organizationService)
        {
            this.organizationService = organizationService;
        }

        public void SampleRun()
        {
            // Example source project GUID
            Guid sourceProjectId = new Guid("11111111-1111-1111-1111-111111111111");
            var sourceProject = new Entity("msdyn_project", sourceProjectId);

            Entity targetProject = new Entity("msdyn_project");
            targetProject["msdyn_subject"] = "Example Project";
            targetProject.Id = organizationService.Create(targetProject);

            ProjectCopyOption copyOption = new ProjectCopyOption();
            copyOption.ReplaceNamedResources = true;

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, ProjectCopyOption projectCopyOption)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV2");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;
            req["ProjectCopyOption"] = JsonConvert.SerializeObject(projectCopyOption);
            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```


[!INCLUDE[footer-include](../includes/footer-banner.md)]