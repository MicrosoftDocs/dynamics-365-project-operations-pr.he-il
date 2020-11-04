---
title: פיתוח תבניות פרוייקט בעזרת 'העתק פרוייקט'
description: נושא זה מספק מידע על אופן יצירת תבניות פרוייקט באמצעות הפעולה המותאמת אישית העתק פרויקט.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: cb49109e8c199bc4569702ae844a19985534294d
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077248"
---
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="1f585-103">פיתוח תבניות פרוייקט בעזרת 'העתק פרוייקט'</span><span class="sxs-lookup"><span data-stu-id="1f585-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="1f585-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="1f585-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1f585-105">Dynamics 365 Project Operations תומך ביכולת להעתיק פרויקט ולהחזיר כל מטלה חזרה למשאבים הכלליים המייצגים את התפקיד.</span><span class="sxs-lookup"><span data-stu-id="1f585-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="1f585-106">לקוחות יכולים להשתמש בפונקציונליות זו לבניית תבניות פרוייקט בסיסיות.</span><span class="sxs-lookup"><span data-stu-id="1f585-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="1f585-107">כשבוחרים **העתק פרויקט** , מצב פרויקט היעד מתעדכן.</span><span class="sxs-lookup"><span data-stu-id="1f585-107">When you select **Copy Project** , the status of the target project is updated.</span></span> <span data-ttu-id="1f585-108">השתמש ב **סיבת המצב** כדי לקבוע מתי הושלמה פעולת ההעתקה.</span><span class="sxs-lookup"><span data-stu-id="1f585-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="1f585-109">בחירה ב **העתק פרויקט** מעדכן גם את תאריך ההתחלה של הפרויקט לתאריך ההתחלה הנוכחי אם לא מזוהה תאריך יעד בישות פרויקט היעד.</span><span class="sxs-lookup"><span data-stu-id="1f585-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="1f585-110">פעולה מותאמת אישית 'העתק פרויקט'</span><span class="sxs-lookup"><span data-stu-id="1f585-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="1f585-111">שם</span><span class="sxs-lookup"><span data-stu-id="1f585-111">Name</span></span> 

<span data-ttu-id="1f585-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="1f585-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="1f585-113">פרמטרי קלט</span><span class="sxs-lookup"><span data-stu-id="1f585-113">Input parameters</span></span>
<span data-ttu-id="1f585-114">ישנם ‏שלושה פרמטרי קלט:</span><span class="sxs-lookup"><span data-stu-id="1f585-114">There are three input parameters:</span></span>

| <span data-ttu-id="1f585-115">פרמטר</span><span class="sxs-lookup"><span data-stu-id="1f585-115">Parameter</span></span>          | <span data-ttu-id="1f585-116">סוג</span><span class="sxs-lookup"><span data-stu-id="1f585-116">Type</span></span>   | <span data-ttu-id="1f585-117">ערכים</span><span class="sxs-lookup"><span data-stu-id="1f585-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="1f585-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="1f585-118">ProjectCopyOption</span></span>  | <span data-ttu-id="1f585-119">String</span><span class="sxs-lookup"><span data-stu-id="1f585-119">String</span></span> | <span data-ttu-id="1f585-120">**{"removeNamedResources":true}** או **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="1f585-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="1f585-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="1f585-121">SourceProject</span></span>      | <span data-ttu-id="1f585-122">הפניית ישות</span><span class="sxs-lookup"><span data-stu-id="1f585-122">Entity Reference</span></span> | <span data-ttu-id="1f585-123">פרויקט מקור</span><span class="sxs-lookup"><span data-stu-id="1f585-123">Source Project</span></span> |
| <span data-ttu-id="1f585-124">יעד</span><span class="sxs-lookup"><span data-stu-id="1f585-124">Target</span></span>             | <span data-ttu-id="1f585-125">הפניית ישות</span><span class="sxs-lookup"><span data-stu-id="1f585-125">Entity Reference</span></span> | <span data-ttu-id="1f585-126">פרויקט יעד</span><span class="sxs-lookup"><span data-stu-id="1f585-126">Target Project</span></span> |


- <span data-ttu-id="1f585-127">**{"clearTeamsAndAssignments":true}** : התנהגות ברירת המחדל עבור Project באינטרנט ותסיר את כל ההקצאות וחברי הצוות..</span><span class="sxs-lookup"><span data-stu-id="1f585-127">**{"clearTeamsAndAssignments":true}** : Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="1f585-128">**{"removeNamedResources":true}** אופן הפעולה המהווה ברירת המחדל ב-Project Operations שיחזיר את ההקצאות למשאבים כלליים.</span><span class="sxs-lookup"><span data-stu-id="1f585-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="1f585-129">לקבלת מידע נוסף על פעולות ברירת מחדל נוספיות, ראה [שימוש בפולות Web API](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span><span class="sxs-lookup"><span data-stu-id="1f585-129">For more defaults on actions, see [Use Web API actions](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="1f585-130">ציון שדות להעתקה</span><span class="sxs-lookup"><span data-stu-id="1f585-130">Specify fields to copy</span></span> 
<span data-ttu-id="1f585-131">כאשר נקראת הפעולה, **העתק פרויקט** יבדק את תצוגת הפרויקט **העתק עמודות פרוייקט** כדי לקבוע אילו שדות יש להעתיק בעת העתקת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="1f585-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>
