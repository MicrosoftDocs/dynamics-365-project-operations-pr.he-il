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
ms.openlocfilehash: cc17df0c73b276048f7c4b04bd9dc6644e828dc0
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949815"
---
# <a name="develop-project-templates-with-copy-project"></a>פיתוח תבניות פרוייקט בעזרת 'העתק פרוייקט'

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Dynamics 365 Project Operations תומך ביכולת להעתיק פרויקט ולהחזיר כל משימה למשאבים הגנריים המייצגים את התפקיד. לקוחות יכולים להשתמש בפונקציונליות זו לבניית תבניות פרוייקט בסיסיות.

כשבוחרים **העתק פרויקט**, מצב פרויקט היעד מתעדכן. השתמש ב **סיבת המצב** כדי לקבוע מתי הושלמה פעולת ההעתקה. בחירה ב **העתק פרויקט** מעדכן גם את תאריך ההתחלה של הפרויקט לתאריך ההתחלה הנוכחי אם לא מזוהה תאריך יעד בישות פרויקט היעד.

## <a name="copy-project-custom-action"></a>פעולה מותאמת אישית 'העתק פרויקט' 

### <a name="name"></a>שם 

**msdyn_CopyProjectV2**

### <a name="input-parameters"></a>פרמטרי קלט
ישנם ‏שלושה פרמטרי קלט:

| פרמטר          | סוג   | ערכים                                                   | 
|--------------------|--------|----------------------------------------------------------|
| ProjectCopyOption  | String | **{"removeNamedResources":true}** או **{"clearTeamsAndAssignments":true}** |
| SourceProject      | הפניית ישות | פרויקט מקור |
| יעד             | הפניית ישות | פרויקט יעד |


- **{"clearTeamsAndAssignments":true}**: התנהגות ברירת המחדל עבור Project באינטרנט ותסיר את כל ההקצאות וחברי הצוות..
- **{"removeNamedResources":true}** אופן הפעולה המהווה ברירת המחדל ב-Project Operations שיחזיר את ההקצאות למשאבים כלליים.

לקבלת מידע נוסף על פעולות ברירת מחדל נוספיות, ראה [שימוש בפולות Web API](/powerapps/developer/common-data-service/webapi/use-web-api-actions)

## <a name="specify-fields-to-copy"></a>ציון שדות להעתקה 
כאשר נקראת הפעולה, **העתק פרויקט** יבדק את תצוגת הפרויקט **העתק עמודות פרוייקט** כדי לקבוע אילו שדות יש להעתיק בעת העתקת הפרויקט.


### <a name="example"></a>דוגמה
הדוגמה הבאה מראה כיצד להתקשר לפעולה מותאמת אישית **CopyProject** עם ערכת הפרמטרים **removeNamedResources**.
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