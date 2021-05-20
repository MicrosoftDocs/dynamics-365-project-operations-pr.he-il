---
title: שימוש בממשקי API של לוח זמנים לביצוע פעולות דרך ישויות תזמון
description: נושא זה מספק מידע ודוגמאות לשימוש בממשקי API של לוח זמנים.
author: sigitac
manager: Annbe
ms.date: 04/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: e03f4e6c49a835206b23cade3fabe3fd26693441
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2021
ms.locfileid: "5950805"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="358d4-103">שימוש בממשקי API של לוח זמנים לביצוע פעולות דרך ישויות תזמון</span><span class="sxs-lookup"><span data-stu-id="358d4-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="358d4-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="358d4-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="358d4-105">כל הפונקציונליות או חלק ממנה המצוינת בנושא זה זמינה כחלק ממהדורת Preview.</span><span class="sxs-lookup"><span data-stu-id="358d4-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="358d4-106">התוכן והפונקציונליות כפופים לשינויים.</span><span class="sxs-lookup"><span data-stu-id="358d4-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="358d4-107">ישויות תזמון</span><span class="sxs-lookup"><span data-stu-id="358d4-107">Scheduling entities</span></span>

<span data-ttu-id="358d4-108">ממשקי API של לוח הזמנים מאפשרים לבצע פעולות יצירה, עדכון ומחיקה בעזרת **ישויות תזמון**.</span><span class="sxs-lookup"><span data-stu-id="358d4-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="358d4-109">ישויות אלה מנוהלות דרך מנוע התזמון ב- Project for the Web.</span><span class="sxs-lookup"><span data-stu-id="358d4-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="358d4-110">פעולות יצירה, עדכון ומחיקה בעזרת **ישויות תזמון** הוגבלו במהדרות הקודמות של Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="358d4-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="358d4-111">הטבלה הבאה מספקת רשימה מלאה של **ישויות התזמון**.</span><span class="sxs-lookup"><span data-stu-id="358d4-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="358d4-112">שם הישות</span><span class="sxs-lookup"><span data-stu-id="358d4-112">Entity name</span></span>  | <span data-ttu-id="358d4-113">שם לוגי של ישות</span><span class="sxs-lookup"><span data-stu-id="358d4-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="358d4-114">פרויקט</span><span class="sxs-lookup"><span data-stu-id="358d4-114">Project</span></span> | <span data-ttu-id="358d4-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="358d4-115">msdyn_project</span></span> |
| <span data-ttu-id="358d4-116">משימת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="358d4-116">Project Task</span></span>  | <span data-ttu-id="358d4-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="358d4-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="358d4-118">‏‫יחס תלות במשימת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="358d4-118">Project Task Dependency</span></span>  | <span data-ttu-id="358d4-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="358d4-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="358d4-120">הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="358d4-120">Resource Assignment</span></span> | <span data-ttu-id="358d4-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="358d4-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="358d4-122">מיכל של פרוייקט</span><span class="sxs-lookup"><span data-stu-id="358d4-122">Project Bucket</span></span>  | <span data-ttu-id="358d4-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="358d4-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="358d4-124">חבר צוות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="358d4-124">Project Team Member</span></span> | <span data-ttu-id="358d4-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="358d4-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="358d4-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="358d4-126">OperationSet</span></span>

<span data-ttu-id="358d4-127">OperationSet הוא דפוס יחידת עבודה שניתן להשתמש בו כאשר יש לעבד מספר בקשות המשפיעות על לוחות זמנים במסגרת עסקה.</span><span class="sxs-lookup"><span data-stu-id="358d4-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="358d4-128">ממשקי API של לוח זמנים</span><span class="sxs-lookup"><span data-stu-id="358d4-128">Schedule APIs</span></span>

<span data-ttu-id="358d4-129">להלן רשימה של ממשקי API נוכחיים של לוח זמנים.</span><span class="sxs-lookup"><span data-stu-id="358d4-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="358d4-130">**msdyn_CreateProjectV1** : ניתן להשתמש בממשק API זה ליצירת פרויקט.</span><span class="sxs-lookup"><span data-stu-id="358d4-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="358d4-131">הפרויקט ומיכל הפרויקט המוגדר כברירת מחדל נוצרים באופן מיידי.</span><span class="sxs-lookup"><span data-stu-id="358d4-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="358d4-132">**msdyn_CreateTeamMemberV1** : ניתן להשתמש בממשק API זה ליצירת חבר צוות פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="358d4-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="358d4-133">רשומת חבר הצוות נוצרת באופן מיידי.</span><span class="sxs-lookup"><span data-stu-id="358d4-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="358d4-134">**msdyn_CreateOperationSetV1** : ניתן להשתמש בממשק API זה לתזמון מספר בקשות שיש לבצע במסגרת עסקה.</span><span class="sxs-lookup"><span data-stu-id="358d4-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="358d4-135">**msdyn_PSSCreateV1** : ניתן להשתמש בממשק API זה ליצירת ישות.</span><span class="sxs-lookup"><span data-stu-id="358d4-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="358d4-136">הישות יכולה להיות כל אחת מיישויות התזמון התומכות בפעולת היצירה.</span><span class="sxs-lookup"><span data-stu-id="358d4-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="358d4-137">**msdyn_PSSUpdateV1**: ניתן להשתמש בממשק API זה לעדכון ישות.</span><span class="sxs-lookup"><span data-stu-id="358d4-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="358d4-138">הישות יכולה להיות כל אחת מיישויות התזמון התומכות בפעולת העדכון.</span><span class="sxs-lookup"><span data-stu-id="358d4-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="358d4-139">**msdyn_PSSDeleteV1**: ניתן להשתמש בממשק API זה למחיקת ישות.</span><span class="sxs-lookup"><span data-stu-id="358d4-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="358d4-140">הישות יכולה להיות כל אחת מיישויות התזמון התומכות בפעולת המחיקה.</span><span class="sxs-lookup"><span data-stu-id="358d4-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="358d4-141">**msdyn_ExecuteOperationSetV1** : ממשק API זה משמש לביצוע כל הפעולות במסגרת קבוצת הפעולות הנתונה.</span><span class="sxs-lookup"><span data-stu-id="358d4-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="358d4-142">שימוש בממשקי API של לוח זמנים עם OperationSet</span><span class="sxs-lookup"><span data-stu-id="358d4-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="358d4-143">מפני שהרשומות **CreateProjectV1** ו- **CreateTeamMemberV1** נוצרות באופן מיידי, לא ניתן להשתמש בממשקי API אלה ב- **OperationSet** ישירות.</span><span class="sxs-lookup"><span data-stu-id="358d4-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="358d4-144">עם זאת, ניתן להשתמש ב- API כדי ליצור רשומות נדרשות, ליצור **OperationSet** ולאחר מכן להשתמש ברשומות אלה שנוצרו מראש ב- **OperationSet**.</span><span class="sxs-lookup"><span data-stu-id="358d4-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="358d4-145">פעולות נתמכות</span><span class="sxs-lookup"><span data-stu-id="358d4-145">Supported operations</span></span>

| <span data-ttu-id="358d4-146">ישות תזמון</span><span class="sxs-lookup"><span data-stu-id="358d4-146">Scheduling entity</span></span> | <span data-ttu-id="358d4-147">צור</span><span class="sxs-lookup"><span data-stu-id="358d4-147">Create</span></span> | <span data-ttu-id="358d4-148">עדכון</span><span class="sxs-lookup"><span data-stu-id="358d4-148">Update</span></span> | <span data-ttu-id="358d4-149">DELETE</span><span class="sxs-lookup"><span data-stu-id="358d4-149">Delete</span></span> | <span data-ttu-id="358d4-150">שיקולים חשובים:</span><span class="sxs-lookup"><span data-stu-id="358d4-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="358d4-151">משימת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="358d4-151">Project task</span></span> | <span data-ttu-id="358d4-152">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="358d4-152">Yes</span></span> | <span data-ttu-id="358d4-153">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="358d4-153">Yes</span></span> | <span data-ttu-id="358d4-154">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="358d4-154">Yes</span></span> | <span data-ttu-id="358d4-155">ללא</span><span class="sxs-lookup"><span data-stu-id="358d4-155">None</span></span> |
| <span data-ttu-id="358d4-156">‏‫יחס תלות במשימת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="358d4-156">Project task dependency</span></span> | <span data-ttu-id="358d4-157">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="358d4-157">Yes</span></span> | <span data-ttu-id="358d4-158">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="358d4-158">Yes</span></span> | | <span data-ttu-id="358d4-159">רשומות יחס תלות במשימת פרוייקט אינן מעודכנות.</span><span class="sxs-lookup"><span data-stu-id="358d4-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="358d4-160">במקום זאת, ניתן למחוק רשומה ישנה וליצור רשומה חדשה.</span><span class="sxs-lookup"><span data-stu-id="358d4-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="358d4-161">הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="358d4-161">Resource assignment</span></span> | <span data-ttu-id="358d4-162">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="358d4-162">Yes</span></span> | <span data-ttu-id="358d4-163">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="358d4-163">Yes</span></span> | | <span data-ttu-id="358d4-164">פעולות עם השדות הבאים אינן נתמכות: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining** ו- **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="358d4-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="358d4-165">רשומות הקצאת משאבים אינן מעודכנות.</span><span class="sxs-lookup"><span data-stu-id="358d4-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="358d4-166">במקום זאת, ניתן למחוק את הרשומה הישנה וליצור רשומה חדשה.</span><span class="sxs-lookup"><span data-stu-id="358d4-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="358d4-167">מיכל של פרוייקט</span><span class="sxs-lookup"><span data-stu-id="358d4-167">Project bucket</span></span> | <span data-ttu-id="358d4-168">לא זמין</span><span class="sxs-lookup"><span data-stu-id="358d4-168">N/A</span></span> | <span data-ttu-id="358d4-169">לא זמין</span><span class="sxs-lookup"><span data-stu-id="358d4-169">N/A</span></span> | <span data-ttu-id="358d4-170">לא זמין</span><span class="sxs-lookup"><span data-stu-id="358d4-170">N/A</span></span> | <span data-ttu-id="358d4-171">מיכל ברירת המחדל נוצר באמצעות ממשק ה- API **CreateProjectV1**.</span><span class="sxs-lookup"><span data-stu-id="358d4-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="358d4-172">חבר צוות פרויקט</span><span class="sxs-lookup"><span data-stu-id="358d4-172">Project team member</span></span> | <span data-ttu-id="358d4-173">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="358d4-173">Yes</span></span> | <span data-ttu-id="358d4-174">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="358d4-174">Yes</span></span> | <span data-ttu-id="358d4-175">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="358d4-175">Yes</span></span> | <span data-ttu-id="358d4-176">לצורך פעולת היצירה, השתמש בממשק API **CreateTeamMemberV1**.</span><span class="sxs-lookup"><span data-stu-id="358d4-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="358d4-177">פרויקט</span><span class="sxs-lookup"><span data-stu-id="358d4-177">Project</span></span> | <span data-ttu-id="358d4-178">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="358d4-178">Yes</span></span> | <span data-ttu-id="358d4-179">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="358d4-179">Yes</span></span> | <span data-ttu-id="358d4-180">לא זמין</span><span class="sxs-lookup"><span data-stu-id="358d4-180">N/A</span></span> | <span data-ttu-id="358d4-181">פעולות עם השדות הבאים אינן נתמכות: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart** ו- **Duration**.</span><span class="sxs-lookup"><span data-stu-id="358d4-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="358d4-182">ניתן לקרוא לממשקי API אלה באמצעות אובייקטים של ישויות הכוללים שדות מותאמים אישית.</span><span class="sxs-lookup"><span data-stu-id="358d4-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="358d4-183">מאפיין המזהה הוא אופציונלי.</span><span class="sxs-lookup"><span data-stu-id="358d4-183">The ID property is optional.</span></span> <span data-ttu-id="358d4-184">אם הוא מסופק, המערכת מנסה להשתמש בו ומציגה חריגה אם לא ניתן להשתמש בו.</span><span class="sxs-lookup"><span data-stu-id="358d4-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="358d4-185">אם הוא לא מסופק, המערכת תיצור אותו.</span><span class="sxs-lookup"><span data-stu-id="358d4-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="358d4-186">שדות מוגבלים</span><span class="sxs-lookup"><span data-stu-id="358d4-186">Restricted fields</span></span>

<span data-ttu-id="358d4-187">הטבלאות הבאות מגדירות את השדות שהאפשרויות **צור** ו **עריכה** מוגבלות בהם.</span><span class="sxs-lookup"><span data-stu-id="358d4-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="358d4-188">משימת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="358d4-188">Project task</span></span>

| <span data-ttu-id="358d4-189">**שם לוגי**</span><span class="sxs-lookup"><span data-stu-id="358d4-189">**Logical name**</span></span>                       | <span data-ttu-id="358d4-190">**אפשר ליצור**</span><span class="sxs-lookup"><span data-stu-id="358d4-190">**Can create**</span></span> | <span data-ttu-id="358d4-191">**יכול לערוך**</span><span class="sxs-lookup"><span data-stu-id="358d4-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="358d4-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="358d4-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="358d4-193">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-193">no</span></span>             | <span data-ttu-id="358d4-194">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-194">no</span></span>               |
| <span data-ttu-id="358d4-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="358d4-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="358d4-196">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-196">no</span></span>             | <span data-ttu-id="358d4-197">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-197">no</span></span>               |
| <span data-ttu-id="358d4-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="358d4-198">msdyn_actualend</span></span>                        | <span data-ttu-id="358d4-199">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-199">no</span></span>             | <span data-ttu-id="358d4-200">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-200">no</span></span>               |
| <span data-ttu-id="358d4-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="358d4-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="358d4-202">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-202">no</span></span>             | <span data-ttu-id="358d4-203">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-203">no</span></span>               |
| <span data-ttu-id="358d4-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="358d4-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="358d4-205">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-205">no</span></span>             | <span data-ttu-id="358d4-206">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-206">no</span></span>               |
| <span data-ttu-id="358d4-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="358d4-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="358d4-208">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-208">no</span></span>             | <span data-ttu-id="358d4-209">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-209">no</span></span>               |
| <span data-ttu-id="358d4-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="358d4-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="358d4-211">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-211">no</span></span>             | <span data-ttu-id="358d4-212">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-212">no</span></span>               |
| <span data-ttu-id="358d4-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="358d4-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="358d4-214">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-214">no</span></span>             | <span data-ttu-id="358d4-215">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-215">no</span></span>               |
| <span data-ttu-id="358d4-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="358d4-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="358d4-217">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-217">no</span></span>             | <span data-ttu-id="358d4-218">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-218">no</span></span>               |
| <span data-ttu-id="358d4-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="358d4-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="358d4-220">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-220">no</span></span>             | <span data-ttu-id="358d4-221">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-221">no</span></span>               |
| <span data-ttu-id="358d4-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="358d4-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="358d4-223">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-223">no</span></span>             | <span data-ttu-id="358d4-224">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-224">no</span></span>               |
| <span data-ttu-id="358d4-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="358d4-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="358d4-226">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-226">no</span></span>             | <span data-ttu-id="358d4-227">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-227">no</span></span>               |
| <span data-ttu-id="358d4-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="358d4-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="358d4-229">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-229">no</span></span>             | <span data-ttu-id="358d4-230">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-230">no</span></span>               |
| <span data-ttu-id="358d4-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="358d4-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="358d4-232">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-232">no</span></span>             | <span data-ttu-id="358d4-233">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-233">no</span></span>               |
| <span data-ttu-id="358d4-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="358d4-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="358d4-235">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-235">no</span></span>             | <span data-ttu-id="358d4-236">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-236">no</span></span>               |
| <span data-ttu-id="358d4-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="358d4-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="358d4-238">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-238">no</span></span>             | <span data-ttu-id="358d4-239">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-239">no</span></span>               |
| <span data-ttu-id="358d4-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="358d4-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="358d4-241">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-241">no</span></span>             | <span data-ttu-id="358d4-242">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-242">no</span></span>               |
| <span data-ttu-id="358d4-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="358d4-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="358d4-244">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-244">no</span></span>             | <span data-ttu-id="358d4-245">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-245">no</span></span>               |
| <span data-ttu-id="358d4-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="358d4-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="358d4-247">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-247">no</span></span>             | <span data-ttu-id="358d4-248">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-248">no</span></span>               |
| <span data-ttu-id="358d4-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="358d4-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="358d4-250">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-250">no</span></span>             | <span data-ttu-id="358d4-251">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-251">no</span></span>               |
| <span data-ttu-id="358d4-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="358d4-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="358d4-253">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-253">no</span></span>             | <span data-ttu-id="358d4-254">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-254">no</span></span>               |
| <span data-ttu-id="358d4-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="358d4-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="358d4-256">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-256">no</span></span>             | <span data-ttu-id="358d4-257">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-257">no</span></span>               |
| <span data-ttu-id="358d4-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="358d4-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="358d4-259">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-259">no</span></span>             | <span data-ttu-id="358d4-260">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-260">no</span></span>               |
| <span data-ttu-id="358d4-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="358d4-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="358d4-262">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-262">no</span></span>             | <span data-ttu-id="358d4-263">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-263">no</span></span>               |
| <span data-ttu-id="358d4-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="358d4-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="358d4-265">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-265">no</span></span>             | <span data-ttu-id="358d4-266">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-266">no</span></span>               |
| <span data-ttu-id="358d4-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="358d4-267">msdyn_progress</span></span>                         | <span data-ttu-id="358d4-268">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-268">no</span></span>             | <span data-ttu-id="358d4-269">לא (כן עבור P4W)</span><span class="sxs-lookup"><span data-stu-id="358d4-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="358d4-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="358d4-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="358d4-271">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-271">no</span></span>             | <span data-ttu-id="358d4-272">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-272">no</span></span>               |
| <span data-ttu-id="358d4-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="358d4-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="358d4-274">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-274">no</span></span>             | <span data-ttu-id="358d4-275">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-275">no</span></span>               |
| <span data-ttu-id="358d4-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="358d4-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="358d4-277">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-277">no</span></span>             | <span data-ttu-id="358d4-278">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-278">no</span></span>               |
| <span data-ttu-id="358d4-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="358d4-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="358d4-280">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-280">no</span></span>             | <span data-ttu-id="358d4-281">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-281">no</span></span>               |
| <span data-ttu-id="358d4-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="358d4-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="358d4-283">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-283">no</span></span>             | <span data-ttu-id="358d4-284">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-284">no</span></span>               |
| <span data-ttu-id="358d4-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="358d4-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="358d4-286">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-286">no</span></span>             | <span data-ttu-id="358d4-287">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-287">no</span></span>               |
| <span data-ttu-id="358d4-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="358d4-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="358d4-289">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-289">no</span></span>             | <span data-ttu-id="358d4-290">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-290">no</span></span>               |
| <span data-ttu-id="358d4-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="358d4-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="358d4-292">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-292">no</span></span>             | <span data-ttu-id="358d4-293">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-293">no</span></span>               |
| <span data-ttu-id="358d4-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="358d4-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="358d4-295">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-295">no</span></span>             | <span data-ttu-id="358d4-296">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-296">no</span></span>               |
| <span data-ttu-id="358d4-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="358d4-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="358d4-298">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-298">no</span></span>             | <span data-ttu-id="358d4-299">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-299">no</span></span>               |
| <span data-ttu-id="358d4-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="358d4-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="358d4-301">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-301">no</span></span>             | <span data-ttu-id="358d4-302">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-302">no</span></span>               |
| <span data-ttu-id="358d4-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="358d4-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="358d4-304">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-304">no</span></span>             | <span data-ttu-id="358d4-305">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-305">no</span></span>               |
| <span data-ttu-id="358d4-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="358d4-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="358d4-307">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-307">no</span></span>             | <span data-ttu-id="358d4-308">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-308">no</span></span>               |
| <span data-ttu-id="358d4-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="358d4-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="358d4-310">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-310">no</span></span>             | <span data-ttu-id="358d4-311">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-311">no</span></span>               |
| <span data-ttu-id="358d4-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="358d4-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="358d4-313">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-313">no</span></span>             | <span data-ttu-id="358d4-314">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-314">no</span></span>               |
| <span data-ttu-id="358d4-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="358d4-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="358d4-316">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-316">no</span></span>             | <span data-ttu-id="358d4-317">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-317">no</span></span>               |
| <span data-ttu-id="358d4-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="358d4-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="358d4-319">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-319">no</span></span>             | <span data-ttu-id="358d4-320">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-320">no</span></span>               |
| <span data-ttu-id="358d4-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="358d4-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="358d4-322">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-322">no</span></span>             | <span data-ttu-id="358d4-323">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-323">no</span></span>               |
| <span data-ttu-id="358d4-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="358d4-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="358d4-325">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-325">no</span></span>             | <span data-ttu-id="358d4-326">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-326">no</span></span>               |
| <span data-ttu-id="358d4-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="358d4-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="358d4-328">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-328">no</span></span>             | <span data-ttu-id="358d4-329">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-329">no</span></span>               |
| <span data-ttu-id="358d4-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="358d4-330">msdyn_summary</span></span>                          | <span data-ttu-id="358d4-331">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-331">no</span></span>             | <span data-ttu-id="358d4-332">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-332">no</span></span>               |
| <span data-ttu-id="358d4-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="358d4-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="358d4-334">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-334">no</span></span>             | <span data-ttu-id="358d4-335">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-335">no</span></span>               |
| <span data-ttu-id="358d4-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="358d4-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="358d4-337">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-337">no</span></span>             | <span data-ttu-id="358d4-338">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="358d4-339">‏‫יחס תלות במשימת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="358d4-339">Project task dependency</span></span>

| <span data-ttu-id="358d4-340">**שם לוגי**</span><span class="sxs-lookup"><span data-stu-id="358d4-340">**Logical name**</span></span>              | <span data-ttu-id="358d4-341">**אפשר ליצור**</span><span class="sxs-lookup"><span data-stu-id="358d4-341">**Can create**</span></span> | <span data-ttu-id="358d4-342">**יכול לערוך**</span><span class="sxs-lookup"><span data-stu-id="358d4-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="358d4-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="358d4-343">msdyn_linktype</span></span>                | <span data-ttu-id="358d4-344">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-344">no</span></span>             | <span data-ttu-id="358d4-345">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-345">no</span></span>           |
| <span data-ttu-id="358d4-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="358d4-346">msdyn_linktypename</span></span>            | <span data-ttu-id="358d4-347">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-347">no</span></span>             | <span data-ttu-id="358d4-348">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-348">no</span></span>           |
| <span data-ttu-id="358d4-349">msdyn_predcessortask</span><span class="sxs-lookup"><span data-stu-id="358d4-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="358d4-350">כן</span><span class="sxs-lookup"><span data-stu-id="358d4-350">yes</span></span>            | <span data-ttu-id="358d4-351">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-351">no</span></span>           |
| <span data-ttu-id="358d4-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="358d4-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="358d4-353">כן</span><span class="sxs-lookup"><span data-stu-id="358d4-353">yes</span></span>            | <span data-ttu-id="358d4-354">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-354">no</span></span>           |
| <span data-ttu-id="358d4-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="358d4-355">msdyn_project</span></span>                 | <span data-ttu-id="358d4-356">כן</span><span class="sxs-lookup"><span data-stu-id="358d4-356">yes</span></span>            | <span data-ttu-id="358d4-357">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-357">no</span></span>           |
| <span data-ttu-id="358d4-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="358d4-358">msdyn_projectname</span></span>             | <span data-ttu-id="358d4-359">כן</span><span class="sxs-lookup"><span data-stu-id="358d4-359">yes</span></span>            | <span data-ttu-id="358d4-360">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-360">no</span></span>           |
| <span data-ttu-id="358d4-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="358d4-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="358d4-362">כן</span><span class="sxs-lookup"><span data-stu-id="358d4-362">yes</span></span>            | <span data-ttu-id="358d4-363">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-363">no</span></span>           |
| <span data-ttu-id="358d4-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="358d4-364">msdyn_successortask</span></span>           | <span data-ttu-id="358d4-365">כן</span><span class="sxs-lookup"><span data-stu-id="358d4-365">yes</span></span>            | <span data-ttu-id="358d4-366">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-366">no</span></span>           |
| <span data-ttu-id="358d4-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="358d4-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="358d4-368">כן</span><span class="sxs-lookup"><span data-stu-id="358d4-368">yes</span></span>            | <span data-ttu-id="358d4-369">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="358d4-370">הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="358d4-370">Resource assignment</span></span>

| <span data-ttu-id="358d4-371">**שם לוגי**</span><span class="sxs-lookup"><span data-stu-id="358d4-371">**Logical name**</span></span>             | <span data-ttu-id="358d4-372">**אפשר ליצור**</span><span class="sxs-lookup"><span data-stu-id="358d4-372">**Can create**</span></span> | <span data-ttu-id="358d4-373">**יכול לערוך**</span><span class="sxs-lookup"><span data-stu-id="358d4-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="358d4-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="358d4-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="358d4-375">כן</span><span class="sxs-lookup"><span data-stu-id="358d4-375">yes</span></span>            | <span data-ttu-id="358d4-376">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-376">no</span></span>           |
| <span data-ttu-id="358d4-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="358d4-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="358d4-378">כן</span><span class="sxs-lookup"><span data-stu-id="358d4-378">yes</span></span>            | <span data-ttu-id="358d4-379">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-379">no</span></span>           |
| <span data-ttu-id="358d4-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="358d4-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="358d4-381">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-381">no</span></span>             | <span data-ttu-id="358d4-382">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-382">no</span></span>           |
| <span data-ttu-id="358d4-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="358d4-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="358d4-384">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-384">no</span></span>             | <span data-ttu-id="358d4-385">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-385">no</span></span>           |
| <span data-ttu-id="358d4-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="358d4-386">msdyn_committype</span></span>             | <span data-ttu-id="358d4-387">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-387">no</span></span>             | <span data-ttu-id="358d4-388">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-388">no</span></span>           |
| <span data-ttu-id="358d4-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="358d4-389">msdyn_committypename</span></span>         | <span data-ttu-id="358d4-390">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-390">no</span></span>             | <span data-ttu-id="358d4-391">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-391">no</span></span>           |
| <span data-ttu-id="358d4-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="358d4-392">msdyn_effort</span></span>                 | <span data-ttu-id="358d4-393">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-393">no</span></span>             | <span data-ttu-id="358d4-394">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-394">no</span></span>           |
| <span data-ttu-id="358d4-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="358d4-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="358d4-396">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-396">no</span></span>             | <span data-ttu-id="358d4-397">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-397">no</span></span>           |
| <span data-ttu-id="358d4-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="358d4-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="358d4-399">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-399">no</span></span>             | <span data-ttu-id="358d4-400">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-400">no</span></span>           |
| <span data-ttu-id="358d4-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="358d4-401">msdyn_finish</span></span>                 | <span data-ttu-id="358d4-402">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-402">no</span></span>             | <span data-ttu-id="358d4-403">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-403">no</span></span>           |
| <span data-ttu-id="358d4-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="358d4-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="358d4-405">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-405">no</span></span>             | <span data-ttu-id="358d4-406">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-406">no</span></span>           |
| <span data-ttu-id="358d4-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="358d4-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="358d4-408">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-408">no</span></span>             | <span data-ttu-id="358d4-409">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-409">no</span></span>           |
| <span data-ttu-id="358d4-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="358d4-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="358d4-411">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-411">no</span></span>             | <span data-ttu-id="358d4-412">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-412">no</span></span>           |
| <span data-ttu-id="358d4-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="358d4-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="358d4-414">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-414">no</span></span>             | <span data-ttu-id="358d4-415">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-415">no</span></span>           |
| <span data-ttu-id="358d4-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="358d4-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="358d4-417">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-417">no</span></span>             | <span data-ttu-id="358d4-418">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-418">no</span></span>           |
| <span data-ttu-id="358d4-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="358d4-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="358d4-420">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-420">no</span></span>             | <span data-ttu-id="358d4-421">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-421">no</span></span>           |
| <span data-ttu-id="358d4-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="358d4-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="358d4-423">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-423">no</span></span>             | <span data-ttu-id="358d4-424">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-424">no</span></span>           |
| <span data-ttu-id="358d4-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="358d4-425">msdyn_projectid</span></span>              | <span data-ttu-id="358d4-426">כן</span><span class="sxs-lookup"><span data-stu-id="358d4-426">yes</span></span>            | <span data-ttu-id="358d4-427">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-427">no</span></span>           |
| <span data-ttu-id="358d4-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="358d4-428">msdyn_projectidname</span></span>          | <span data-ttu-id="358d4-429">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-429">no</span></span>             | <span data-ttu-id="358d4-430">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-430">no</span></span>           |
| <span data-ttu-id="358d4-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="358d4-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="358d4-432">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-432">no</span></span>             | <span data-ttu-id="358d4-433">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-433">no</span></span>           |
| <span data-ttu-id="358d4-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="358d4-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="358d4-435">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-435">no</span></span>             | <span data-ttu-id="358d4-436">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-436">no</span></span>           |
| <span data-ttu-id="358d4-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="358d4-437">msdyn_start</span></span>                  | <span data-ttu-id="358d4-438">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-438">no</span></span>             | <span data-ttu-id="358d4-439">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-439">no</span></span>           |
| <span data-ttu-id="358d4-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="358d4-440">msdyn_taskid</span></span>                 | <span data-ttu-id="358d4-441">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-441">no</span></span>             | <span data-ttu-id="358d4-442">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-442">no</span></span>           |
| <span data-ttu-id="358d4-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="358d4-443">msdyn_taskidname</span></span>             | <span data-ttu-id="358d4-444">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-444">no</span></span>             | <span data-ttu-id="358d4-445">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-445">no</span></span>           |
| <span data-ttu-id="358d4-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="358d4-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="358d4-447">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-447">no</span></span>             | <span data-ttu-id="358d4-448">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="358d4-449">חבר צוות פרויקט</span><span class="sxs-lookup"><span data-stu-id="358d4-449">Project team member</span></span>

| <span data-ttu-id="358d4-450">**שם לוגי**</span><span class="sxs-lookup"><span data-stu-id="358d4-450">**Logical name**</span></span>                                 | <span data-ttu-id="358d4-451">**אפשר ליצור**</span><span class="sxs-lookup"><span data-stu-id="358d4-451">**Can create**</span></span> | <span data-ttu-id="358d4-452">**יכול לערוך**</span><span class="sxs-lookup"><span data-stu-id="358d4-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="358d4-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="358d4-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="358d4-454">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-454">no</span></span>             | <span data-ttu-id="358d4-455">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-455">no</span></span>           |
| <span data-ttu-id="358d4-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="358d4-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="358d4-457">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-457">no</span></span>             | <span data-ttu-id="358d4-458">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-458">no</span></span>           |
| <span data-ttu-id="358d4-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="358d4-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="358d4-460">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-460">no</span></span>             | <span data-ttu-id="358d4-461">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-461">no</span></span>           |
| <span data-ttu-id="358d4-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="358d4-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="358d4-463">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-463">no</span></span>             | <span data-ttu-id="358d4-464">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-464">no</span></span>           |
| <span data-ttu-id="358d4-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="358d4-465">msdyn_effort</span></span>                                     | <span data-ttu-id="358d4-466">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-466">no</span></span>             | <span data-ttu-id="358d4-467">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-467">no</span></span>           |
| <span data-ttu-id="358d4-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="358d4-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="358d4-469">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-469">no</span></span>             | <span data-ttu-id="358d4-470">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-470">no</span></span>           |
| <span data-ttu-id="358d4-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="358d4-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="358d4-472">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-472">no</span></span>             | <span data-ttu-id="358d4-473">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-473">no</span></span>           |
| <span data-ttu-id="358d4-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="358d4-474">msdyn_finish</span></span>                                     | <span data-ttu-id="358d4-475">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-475">no</span></span>             | <span data-ttu-id="358d4-476">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-476">no</span></span>           |
| <span data-ttu-id="358d4-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="358d4-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="358d4-478">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-478">no</span></span>             | <span data-ttu-id="358d4-479">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-479">no</span></span>           |
| <span data-ttu-id="358d4-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="358d4-480">msdyn_hours</span></span>                                      | <span data-ttu-id="358d4-481">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-481">no</span></span>             | <span data-ttu-id="358d4-482">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-482">no</span></span>           |
| <span data-ttu-id="358d4-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="358d4-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="358d4-484">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-484">no</span></span>             | <span data-ttu-id="358d4-485">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-485">no</span></span>           |
| <span data-ttu-id="358d4-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="358d4-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="358d4-487">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-487">no</span></span>             | <span data-ttu-id="358d4-488">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-488">no</span></span>           |
| <span data-ttu-id="358d4-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="358d4-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="358d4-490">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-490">no</span></span>             | <span data-ttu-id="358d4-491">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-491">no</span></span>           |
| <span data-ttu-id="358d4-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="358d4-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="358d4-493">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-493">no</span></span>             | <span data-ttu-id="358d4-494">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-494">no</span></span>           |
| <span data-ttu-id="358d4-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="358d4-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="358d4-496">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-496">no</span></span>             | <span data-ttu-id="358d4-497">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-497">no</span></span>           |
| <span data-ttu-id="358d4-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="358d4-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="358d4-499">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-499">no</span></span>             | <span data-ttu-id="358d4-500">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-500">no</span></span>           |
| <span data-ttu-id="358d4-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="358d4-501">msdyn_start</span></span>                                      | <span data-ttu-id="358d4-502">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-502">no</span></span>             | <span data-ttu-id="358d4-503">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="358d4-504">פרויקט</span><span class="sxs-lookup"><span data-stu-id="358d4-504">Project</span></span>

| <span data-ttu-id="358d4-505">**שם לוגי**</span><span class="sxs-lookup"><span data-stu-id="358d4-505">**Logical name**</span></span>                       | <span data-ttu-id="358d4-506">**אפשר ליצור**</span><span class="sxs-lookup"><span data-stu-id="358d4-506">**Can create**</span></span> | <span data-ttu-id="358d4-507">**יכול לערוך**</span><span class="sxs-lookup"><span data-stu-id="358d4-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="358d4-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="358d4-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="358d4-509">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-509">no</span></span>             | <span data-ttu-id="358d4-510">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-510">no</span></span>           |
| <span data-ttu-id="358d4-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="358d4-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="358d4-512">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-512">no</span></span>             | <span data-ttu-id="358d4-513">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-513">no</span></span>           |
| <span data-ttu-id="358d4-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="358d4-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="358d4-515">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-515">no</span></span>             | <span data-ttu-id="358d4-516">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-516">no</span></span>           |
| <span data-ttu-id="358d4-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="358d4-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="358d4-518">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-518">no</span></span>             | <span data-ttu-id="358d4-519">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-519">no</span></span>           |
| <span data-ttu-id="358d4-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="358d4-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="358d4-521">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-521">no</span></span>             | <span data-ttu-id="358d4-522">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-522">no</span></span>           |
| <span data-ttu-id="358d4-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="358d4-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="358d4-524">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-524">no</span></span>             | <span data-ttu-id="358d4-525">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-525">no</span></span>           |
| <span data-ttu-id="358d4-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="358d4-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="358d4-527">כן</span><span class="sxs-lookup"><span data-stu-id="358d4-527">yes</span></span>            | <span data-ttu-id="358d4-528">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-528">no</span></span>           |
| <span data-ttu-id="358d4-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="358d4-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="358d4-530">כן</span><span class="sxs-lookup"><span data-stu-id="358d4-530">yes</span></span>            | <span data-ttu-id="358d4-531">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-531">no</span></span>           |
| <span data-ttu-id="358d4-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="358d4-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="358d4-533">כן</span><span class="sxs-lookup"><span data-stu-id="358d4-533">yes</span></span>            | <span data-ttu-id="358d4-534">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-534">no</span></span>           |
| <span data-ttu-id="358d4-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="358d4-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="358d4-536">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-536">no</span></span>             | <span data-ttu-id="358d4-537">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-537">no</span></span>           |
| <span data-ttu-id="358d4-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="358d4-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="358d4-539">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-539">no</span></span>             | <span data-ttu-id="358d4-540">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-540">no</span></span>           |
| <span data-ttu-id="358d4-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="358d4-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="358d4-542">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-542">no</span></span>             | <span data-ttu-id="358d4-543">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-543">no</span></span>           |
| <span data-ttu-id="358d4-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="358d4-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="358d4-545">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-545">no</span></span>             | <span data-ttu-id="358d4-546">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-546">no</span></span>           |
| <span data-ttu-id="358d4-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="358d4-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="358d4-548">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-548">no</span></span>             | <span data-ttu-id="358d4-549">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-549">no</span></span>           |
| <span data-ttu-id="358d4-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="358d4-550">msdyn_duration</span></span>                         | <span data-ttu-id="358d4-551">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-551">no</span></span>             | <span data-ttu-id="358d4-552">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-552">no</span></span>           |
| <span data-ttu-id="358d4-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="358d4-553">msdyn_effort</span></span>                           | <span data-ttu-id="358d4-554">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-554">no</span></span>             | <span data-ttu-id="358d4-555">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-555">no</span></span>           |
| <span data-ttu-id="358d4-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="358d4-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="358d4-557">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-557">no</span></span>             | <span data-ttu-id="358d4-558">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-558">no</span></span>           |
| <span data-ttu-id="358d4-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="358d4-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="358d4-560">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-560">no</span></span>             | <span data-ttu-id="358d4-561">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-561">no</span></span>           |
| <span data-ttu-id="358d4-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="358d4-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="358d4-563">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-563">no</span></span>             | <span data-ttu-id="358d4-564">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-564">no</span></span>           |
| <span data-ttu-id="358d4-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="358d4-565">msdyn_finish</span></span>                           | <span data-ttu-id="358d4-566">כן</span><span class="sxs-lookup"><span data-stu-id="358d4-566">yes</span></span>            | <span data-ttu-id="358d4-567">כן</span><span class="sxs-lookup"><span data-stu-id="358d4-567">yes</span></span>          |
| <span data-ttu-id="358d4-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="358d4-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="358d4-569">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-569">no</span></span>             | <span data-ttu-id="358d4-570">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-570">no</span></span>           |
| <span data-ttu-id="358d4-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="358d4-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="358d4-572">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-572">no</span></span>             | <span data-ttu-id="358d4-573">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-573">no</span></span>           |
| <span data-ttu-id="358d4-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="358d4-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="358d4-575">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-575">no</span></span>             | <span data-ttu-id="358d4-576">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-576">no</span></span>           |
| <span data-ttu-id="358d4-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="358d4-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="358d4-578">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-578">no</span></span>             | <span data-ttu-id="358d4-579">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-579">no</span></span>           |
| <span data-ttu-id="358d4-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="358d4-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="358d4-581">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-581">no</span></span>             | <span data-ttu-id="358d4-582">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-582">no</span></span>           |
| <span data-ttu-id="358d4-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="358d4-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="358d4-584">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-584">no</span></span>             | <span data-ttu-id="358d4-585">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-585">no</span></span>           |
| <span data-ttu-id="358d4-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="358d4-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="358d4-587">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-587">no</span></span>             | <span data-ttu-id="358d4-588">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-588">no</span></span>           |
| <span data-ttu-id="358d4-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="358d4-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="358d4-590">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-590">no</span></span>             | <span data-ttu-id="358d4-591">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-591">no</span></span>           |
| <span data-ttu-id="358d4-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="358d4-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="358d4-593">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-593">no</span></span>             | <span data-ttu-id="358d4-594">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-594">no</span></span>           |
| <span data-ttu-id="358d4-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="358d4-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="358d4-596">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-596">no</span></span>             | <span data-ttu-id="358d4-597">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-597">no</span></span>           |
| <span data-ttu-id="358d4-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="358d4-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="358d4-599">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-599">no</span></span>             | <span data-ttu-id="358d4-600">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-600">no</span></span>           |
| <span data-ttu-id="358d4-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="358d4-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="358d4-602">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-602">no</span></span>             | <span data-ttu-id="358d4-603">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-603">no</span></span>           |
| <span data-ttu-id="358d4-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="358d4-604">msdyn_progress</span></span>                         | <span data-ttu-id="358d4-605">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-605">no</span></span>             | <span data-ttu-id="358d4-606">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-606">no</span></span>           |
| <span data-ttu-id="358d4-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="358d4-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="358d4-608">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-608">no</span></span>             | <span data-ttu-id="358d4-609">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-609">no</span></span>           |
| <span data-ttu-id="358d4-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="358d4-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="358d4-611">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-611">no</span></span>             | <span data-ttu-id="358d4-612">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-612">no</span></span>           |
| <span data-ttu-id="358d4-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="358d4-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="358d4-614">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-614">no</span></span>             | <span data-ttu-id="358d4-615">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-615">no</span></span>           |
| <span data-ttu-id="358d4-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="358d4-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="358d4-617">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-617">no</span></span>             | <span data-ttu-id="358d4-618">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-618">no</span></span>           |
| <span data-ttu-id="358d4-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="358d4-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="358d4-620">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-620">no</span></span>             | <span data-ttu-id="358d4-621">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-621">no</span></span>           |
| <span data-ttu-id="358d4-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="358d4-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="358d4-623">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-623">no</span></span>             | <span data-ttu-id="358d4-624">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-624">no</span></span>           |
| <span data-ttu-id="358d4-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="358d4-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="358d4-626">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-626">no</span></span>             | <span data-ttu-id="358d4-627">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-627">no</span></span>           |
| <span data-ttu-id="358d4-628">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="358d4-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="358d4-629">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-629">no</span></span>             | <span data-ttu-id="358d4-630">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-630">no</span></span>           |
| <span data-ttu-id="358d4-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="358d4-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="358d4-632">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-632">no</span></span>             | <span data-ttu-id="358d4-633">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-633">no</span></span>           |
| <span data-ttu-id="358d4-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="358d4-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="358d4-635">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-635">no</span></span>             | <span data-ttu-id="358d4-636">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-636">no</span></span>           |
| <span data-ttu-id="358d4-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="358d4-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="358d4-638">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-638">no</span></span>             | <span data-ttu-id="358d4-639">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-639">no</span></span>           |
| <span data-ttu-id="358d4-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="358d4-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="358d4-641">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-641">no</span></span>             | <span data-ttu-id="358d4-642">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-642">no</span></span>           |
| <span data-ttu-id="358d4-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="358d4-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="358d4-644">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-644">no</span></span>             | <span data-ttu-id="358d4-645">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-645">no</span></span>           |
| <span data-ttu-id="358d4-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="358d4-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="358d4-647">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-647">no</span></span>             | <span data-ttu-id="358d4-648">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-648">no</span></span>           |
| <span data-ttu-id="358d4-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="358d4-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="358d4-650">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-650">no</span></span>             | <span data-ttu-id="358d4-651">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-651">no</span></span>           |
| <span data-ttu-id="358d4-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="358d4-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="358d4-653">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-653">no</span></span>             | <span data-ttu-id="358d4-654">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-654">no</span></span>           |
| <span data-ttu-id="358d4-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="358d4-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="358d4-656">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-656">no</span></span>             | <span data-ttu-id="358d4-657">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-657">no</span></span>           |
| <span data-ttu-id="358d4-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="358d4-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="358d4-659">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-659">no</span></span>             | <span data-ttu-id="358d4-660">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-660">no</span></span>           |
| <span data-ttu-id="358d4-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="358d4-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="358d4-662">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-662">no</span></span>             | <span data-ttu-id="358d4-663">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-663">no</span></span>           |
| <span data-ttu-id="358d4-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="358d4-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="358d4-665">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-665">no</span></span>             | <span data-ttu-id="358d4-666">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-666">no</span></span>           |
| <span data-ttu-id="358d4-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="358d4-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="358d4-668">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-668">no</span></span>             | <span data-ttu-id="358d4-669">לא</span><span class="sxs-lookup"><span data-stu-id="358d4-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="358d4-670">בעיות ומגבלות ידועות</span><span class="sxs-lookup"><span data-stu-id="358d4-670">Limitations and known issues</span></span>
<span data-ttu-id="358d4-671">להלן רשימה של מגבלות ובעיות ידועות:</span><span class="sxs-lookup"><span data-stu-id="358d4-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="358d4-672">רק **משתמשים עם רישיון ל-Microsoft Project License** יכולים להשתמש בממשקי API של לוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="358d4-672">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="358d4-673">המשתמשים שיכולים להשתמש בהם:</span><span class="sxs-lookup"><span data-stu-id="358d4-673">They can't be used by:</span></span>
    - <span data-ttu-id="358d4-674">משתמשים ביישום</span><span class="sxs-lookup"><span data-stu-id="358d4-674">Application users</span></span>
    - <span data-ttu-id="358d4-675">משתמשי מערכת</span><span class="sxs-lookup"><span data-stu-id="358d4-675">System users</span></span>
    - <span data-ttu-id="358d4-676">משתמשי שילוב</span><span class="sxs-lookup"><span data-stu-id="358d4-676">Integration users</span></span>
    - <span data-ttu-id="358d4-677">משתמשים אחרים שאין להם את הרישיון הנדרש</span><span class="sxs-lookup"><span data-stu-id="358d4-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="358d4-678">כל **OperationSet** יכולה לבצע מקסימום 100 פעולות.</span><span class="sxs-lookup"><span data-stu-id="358d4-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="358d4-679">לכל משתמש יכולות להיות עד 10 **OperationSets** פתוחות.</span><span class="sxs-lookup"><span data-stu-id="358d4-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="358d4-680">Project Operations תומך כיום במקסימום 500 משימות בסה"כ לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="358d4-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="358d4-681">מצב כשל של **OperationSet** ויומני כשל אינם זמינים כרגע.</span><span class="sxs-lookup"><span data-stu-id="358d4-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- <span data-ttu-id="358d4-682">ממשקי API של לוח זמנים הם כרגע במהדורת Public Preview.</span><span class="sxs-lookup"><span data-stu-id="358d4-682">Schedule APIs are in Public preview.</span></span> <span data-ttu-id="358d4-683">השימוש בממשקי API אלה בסביבת ייצור אינו נתמך על ידי Microsoft.</span><span class="sxs-lookup"><span data-stu-id="358d4-683">Using these APIs in a Production environment isn't supported by Microsoft.</span></span>
- [<span data-ttu-id="358d4-684">מגבלות וגבולות בפרויקטים ובמשימות</span><span class="sxs-lookup"><span data-stu-id="358d4-684">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="358d4-685">טיפול בשגיאות</span><span class="sxs-lookup"><span data-stu-id="358d4-685">Error handling</span></span>

   - <span data-ttu-id="358d4-686">כדי לסקור שגיאות שנוצרו מערכי תפעול, עבור אל **גדרות** \> **שילוב תזמון** \> **מערכי תפעול**.</span><span class="sxs-lookup"><span data-stu-id="358d4-686">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="358d4-687">כדי לבדוק שגיאות שנוצרו משירות תזמון הפרויקט, עבור אל **הגדרות** \> **תזמון שילוב** \> **יומני שגיאה של PSS**.</span><span class="sxs-lookup"><span data-stu-id="358d4-687">To review errors generated from the Project Scheduling Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="358d4-688">תרחיש לדוגמה</span><span class="sxs-lookup"><span data-stu-id="358d4-688">Sample scenario</span></span>

<span data-ttu-id="358d4-689">בתרחיש זה, תיצור פרויקט, חבר צוות, ארבע משימות ושתי הקצאות משאבים.</span><span class="sxs-lookup"><span data-stu-id="358d4-689">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="358d4-690">לאחר מכן, תעדכן משימה אחת, תעדכן את הפרויקט, תמחק משימה אחת, תמחק הקצאת משאבים אחת ותיצור תלות במשימה.</span><span class="sxs-lookup"><span data-stu-id="358d4-690">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

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

## <a name="additional-samples"></a><span data-ttu-id="358d4-691">דוגמאות נוספות</span><span class="sxs-lookup"><span data-stu-id="358d4-691">Additional samples</span></span>

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
    task["msdyn_progress"] = 0.34m;
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
