---
title: פיתוח תבניות פרוייקט בעזרת 'העתק פרוייקט'
description: נושא זה מספק מידע על אופן יצירת תבניות פרוייקט באמצעות הפעולה המותאמת אישית העתק פרויקט.
author: stsporen
ms.date: 03/10/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 72aa2db7c717eeab85ada448c673bf702087baeb
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8590899"
---
# <a name="develop-project-templates-with-copy-project"></a>פיתוח תבניות פרוייקט בעזרת 'העתק פרוייקט'

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

Dynamics 365 Project Operations תומך ביכולת להעתיק פרויקט ולהחזיר כל משימה למשאבים הגנריים המייצגים את התפקיד. לקוחות יכולים להשתמש בפונקציונליות זו לבניית תבניות פרוייקט בסיסיות.

כשבוחרים **העתק פרויקט**, מצב פרויקט היעד מתעדכן. השתמש ב **סיבת המצב** כדי לקבוע מתי הושלמה פעולת ההעתקה. בחירה ב **העתק פרויקט** מעדכן גם את תאריך ההתחלה של הפרויקט לתאריך ההתחלה הנוכחי אם לא מזוהה תאריך יעד בישות פרויקט היעד.

## <a name="copy-project-custom-action"></a>פעולה מותאמת אישית 'העתק פרויקט'

### <a name="name"></a>Name 

msdyn \_CopyProjectV3

### <a name="input-parameters"></a>פרמטרי קלט

ישנם ‏שלושה פרמטרי קלט:

- **ReplaceNamedResources** או **ClearTeamsAndAssignments** – הגדר רק אחת מהאפשרויות. אל תגדיר את שניהם.

    - **\{"ReplaceNamedResources":true\}** - אופן הפעולה המהווה ברירת המחדל עבור Project Operations. כל משאב בעל שם מוחלף על ידי משאבים כלליים
    - **\{"‎‏ClearTeamsAndAssignments‏‎": ‏true\}** – אופן פעולה המהווה ברירת המחדל עבור Project for the Web. כל המשימות וחברי הצוות מוסרים.

- **SourceProject** – הפניה לישות של פרויקט המקור שיש להעתיק ממנו. הפרמטר אינו יכול להיות Null.
- **יעד** – הפניה לישות של פרויקט היעד שיש להעתיק אליו. הפרמטר אינו יכול להיות Null.

הטבלה הבאה מספקת סיכום של שלושת הפרמטרים.

| פרמטר                | Type             | ערך                 |
|--------------------------|------------------|-----------------------|
| ReplaceNamedResources    | בוליאני‬          | **True** או **false** |
| ClearTeamsAndAssignments | בוליאני‬          | **True** או **false** |
| SourceProject            | הפניית ישות | פרויקט המקור    |
| יעד                   | הפניית ישות | פרוייקט היעד    |

לקבלת מידע על פעולות ברירת מחדל נוספיות, ראה [שימוש בפולות Web API](/powerapps/developer/common-data-service/webapi/use-web-api-actions).

### <a name="validations"></a>אימותים

מתבצעים האימותים הבאים.

1. Null בודק ומחאזר את פרויקט המקור והיעד כדי לאשר את קיומם של שני הפרויקטים בארגון.
2. המערכת מאמתת שפרויקט היעד תקף להעתקה על ידי אימות התנאים הבאים:

    - אין פעילות קודמת בפרויקט (כולל בחירת הכרטיסיה **משימות**), והפרויקט נוצר לאחרונה.
    - אין עותק קודם, לא התבקש ייבוא לפרויקט זה, ולפרויקט אין מצב של **נכשל**.

3. הפעולה לא נקראת באמצעות HTTP.

## <a name="specify-fields-to-copy"></a>ציון שדות להעתקה

כאשר נקראת הפעולה, **העתק פרויקט** יבדק את תצוגת הפרויקט **העתק עמודות פרוייקט** כדי לקבוע אילו שדות יש להעתיק בעת העתקת הפרויקט.

### <a name="example"></a>דוגמה

הדוגמה הבאה מראה כיצד לקרוא לפעולה המותאמת אישית **CopyProjectV3** באמצעות ערכת הפרמטרים **removeNamedResources**.

```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

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
            targetProject["msdyn_subject"] = "Example Project - Copy";
            targetProject.Id = organizationService.Create(targetProject);

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption, true, false);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, bool replaceNamedResources = true, bool clearTeamsAndAssignments = false)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV3");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;

            if (replaceNamedResources)
            {
                req["ReplaceNamedResources"] = true;
            }
            else
            {
                req["ClearTeamsAndAssignments"] = true;
            }

            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```

[!INCLUDE[footer-include](../includes/footer-banner.md)]
