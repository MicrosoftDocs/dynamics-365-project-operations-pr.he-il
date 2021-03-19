---
title: מודל האבטחה
description: נושא זה מספק מידע על מודל האבטחה ב- Dynamics 365 Project Operations.
author: stsporen
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 3f65d13809fef342be8bec682c11d95c4d9e9b19
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276799"
---
# <a name="security-model"></a><span data-ttu-id="f8a4d-103">מודל האבטחה</span><span class="sxs-lookup"><span data-stu-id="f8a4d-103">Security Model</span></span>

<span data-ttu-id="f8a4d-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="f8a4d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="f8a4d-105">Microsoft Dynamics 365 Project Operations מכיל מודל אבטחה ייחודי המאפשר מודל אבטחה עסקי שמבוסס על תפקידים ומשתף פעולה עם קבוצות Microsoft Office.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-105">Microsoft Dynamics 365 Project Operations contains a unique security model that allows for a role-based business security model that collaborates with Microsoft Office Groups.</span></span> 


## <a name="security-roles"></a><span data-ttu-id="f8a4d-106">תפקידי אבטחה</span><span class="sxs-lookup"><span data-stu-id="f8a4d-106">Security roles</span></span>
<span data-ttu-id="f8a4d-107">יכולות החזית של Project Operations כוללות את התפקידים הבאים:</span><span class="sxs-lookup"><span data-stu-id="f8a4d-107">Project Operations front-end capabilities include the following roles:</span></span>

| <span data-ttu-id="f8a4d-108">תפקיד</span><span class="sxs-lookup"><span data-stu-id="f8a4d-108">Role</span></span>                          | <span data-ttu-id="f8a4d-109">תיאור</span><span class="sxs-lookup"><span data-stu-id="f8a4d-109">Description</span></span>                                                                                                                                                                 | <span data-ttu-id="f8a4d-110">Scope</span><span class="sxs-lookup"><span data-stu-id="f8a4d-110">Scope</span></span> |
|-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|
| <span data-ttu-id="f8a4d-111">מנהל שיטות עבודה</span><span class="sxs-lookup"><span data-stu-id="f8a4d-111">Practice manager</span></span>              | <span data-ttu-id="f8a4d-112">תומך בדיווח חוצה פרויקט.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-112">Supports cross-project reporting.</span></span>                                                                                                            | <span data-ttu-id="f8a4d-113">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="f8a4d-113">Business unit</span></span>              |
| <span data-ttu-id="f8a4d-114">מאשר הפרויקט</span><span class="sxs-lookup"><span data-stu-id="f8a4d-114">Project approver</span></span>              | <span data-ttu-id="f8a4d-115">מאשר שעות והוצאות כנגד פרויקט.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-115">Approves time and expenses against a project.</span></span>                                                                                                                              | <span data-ttu-id="f8a4d-116">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="f8a4d-116">Business unit</span></span> |
| <span data-ttu-id="f8a4d-117">מנהל חיוב פרויקט</span><span class="sxs-lookup"><span data-stu-id="f8a4d-117">Project billing administrator</span></span> | <span data-ttu-id="f8a4d-118">יוצר את הצעת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-118">Creates the invoice proposal.</span></span>                                                                                                                                                 | <span data-ttu-id="f8a4d-119">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="f8a4d-119">Business unit</span></span> |
| <span data-ttu-id="f8a4d-120">מנהל פרויקט</span><span class="sxs-lookup"><span data-stu-id="f8a4d-120">Project manager</span></span>               | <span data-ttu-id="f8a4d-121">יוצר את תוכנית הפרויקט ומבקש משאבים.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-121">Creates the project plan and requests resources.</span></span>                                                                                                                              | <span data-ttu-id="f8a4d-122">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="f8a4d-122">Business unit</span></span> |
| <span data-ttu-id="f8a4d-123">משאב פרויקט</span><span class="sxs-lookup"><span data-stu-id="f8a4d-123">Project resource</span></span>              | <span data-ttu-id="f8a4d-124">חברי צוות שניתן להזמין אותם והם יכולים לדווח על שעות.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-124">Team members who can be booked and report time.</span></span>                                                                                                          | <span data-ttu-id="f8a4d-125">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="f8a4d-125">Business unit</span></span>|
| <span data-ttu-id="f8a4d-126">מנהל משאבים</span><span class="sxs-lookup"><span data-stu-id="f8a4d-126">Resource manager</span></span>              | <span data-ttu-id="f8a4d-127">כל פונקציות ניהול המשאבים, כגון מילוי בקשות והזמנות של משאבים, מופרדות לתמיכה בתצורה היברידית של מנהל פרויקט + מנהל משאבים ובתפקיד מנהל משאבים יחיד ומרכזי.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-127">All resource management functions, such as fulfill resource requests and bookings, separated to support a hybrid Project manager + Resource manager configuration and a single and centralized Resource manager role.</span></span> | <span data-ttu-id="f8a4d-128">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="f8a4d-128">Business unit</span></span> |


<span data-ttu-id="f8a4d-129">Microsoft Project באינטרנט כולל את התפקידים הבאים:</span><span class="sxs-lookup"><span data-stu-id="f8a4d-129">Microsoft Project for the Web includes the following roles:</span></span>

| <span data-ttu-id="f8a4d-130">תפקיד</span><span class="sxs-lookup"><span data-stu-id="f8a4d-130">Role</span></span>           | <span data-ttu-id="f8a4d-131">תיאור</span><span class="sxs-lookup"><span data-stu-id="f8a4d-131">Description</span></span>                                                                                                        | <span data-ttu-id="f8a4d-132">Scope</span><span class="sxs-lookup"><span data-stu-id="f8a4d-132">Scope</span></span>  |
|----------------|--------------------------------------------------------------------------------------------------------------------|--------|
| <span data-ttu-id="f8a4d-133">משתמש בפרויקט</span><span class="sxs-lookup"><span data-stu-id="f8a4d-133">Project user</span></span>   | <span data-ttu-id="f8a4d-134">משתמש משותף של Project המסוגל ליצור פרויקטים משלו ולהציג את כל הפרויקטים המשותפים איתו.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-134">Collaborative user of Project   who is able to create their own projects and view any projects shared with   them.</span></span> | <span data-ttu-id="f8a4d-135">משתמש</span><span class="sxs-lookup"><span data-stu-id="f8a4d-135">User</span></span>   |
| <span data-ttu-id="f8a4d-136">מערכת פרויקט</span><span class="sxs-lookup"><span data-stu-id="f8a4d-136">Project system</span></span> | <span data-ttu-id="f8a4d-137">תפקיד המשמש להקשר יישום.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-137">Role used for application   context.</span></span> <span data-ttu-id="f8a4d-138">לקוחות לא אמורים להשתמש בתפקיד מערכת זה.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-138">Customers should not use this system role.</span></span>                                    | <span data-ttu-id="f8a4d-139">כללי</span><span class="sxs-lookup"><span data-stu-id="f8a4d-139">Global</span></span> |

## <a name="security-enforcement"></a><span data-ttu-id="f8a4d-140">אכיפת אבטחה</span><span class="sxs-lookup"><span data-stu-id="f8a4d-140">Security enforcement</span></span>
<span data-ttu-id="f8a4d-141">פעולות המתבצעות ברמת הפרויקט מבוצעות בהקשר של המשתמש המחובר.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-141">Actions that are performed at the project level are performed in the context of the logged in user.</span></span> <span data-ttu-id="f8a4d-142">המשמעות היא שכדי ליצור, לפתוח או למחוק פרויקט, למשתמש נדרשת גישה ל- CDS.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-142">This means that in order to create, open, or delete a project, the user is required to have access available in CDS.</span></span> <span data-ttu-id="f8a4d-143">ניתן להעניק גישה ל- CDS באמצעות כל אחד מהמנגנונים האפשריים הכלולים בפלטפורמה.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-143">Access in CDS may be granted through any of the possible mechanisms included in the platform.</span></span> <span data-ttu-id="f8a4d-144">לדוגמה, משתמש עם טווח גדול יותר רשאי לגשת לפרויקט או אם בוצעה פעולה מפורשת לשיתוף פרויקט המעניקה למשתמש גישה.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-144">For example, a user with a larger scope may access the project or if an explicit project share action has been performed which grants the user access.</span></span>

<span data-ttu-id="f8a4d-145">חשוב להביא את זה בחשבון בעת יצירת פרויקטים ב- Project Operations.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-145">It's important to consider this when creating projects in Project Operations.</span></span>

## <a name="modern-group-collaboration-with-project-operations"></a><span data-ttu-id="f8a4d-146">שיתוף פעולה מודרני בין קבוצות עם Project Operations</span><span class="sxs-lookup"><span data-stu-id="f8a4d-146">Modern group collaboration with Project Operations</span></span>
<span data-ttu-id="f8a4d-147">Project באינטרנט ו- Project Operations תומכים בקבוצות מודרניות לשיתוף פעולה.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-147">Project for the Web and Project Operations support modern groups for collaboration.</span></span> <span data-ttu-id="f8a4d-148">משתמשים שנוספו לפרויקט באמצעות קבוצה יכולים לערוך את תוכנית הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-148">Users added to the project through a group are able to edit the project plan.</span></span>

<span data-ttu-id="f8a4d-149">Project באינטרנט מוסיף משתמשים לקבוצה באופן אוטומטי עם ההקצאה.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-149">Project for the Web adds users to the group automatically upon assignment.</span></span>

<span data-ttu-id="f8a4d-150">הקבוצות מאפשרות לעבוד בשיתוף פעולה על ההרשאות לפרויקט ועל תוצרים נתמכים של שיתוף הפעולה.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-150">Groups allow the permissions of the project and supporting collaboration artifacts to be worked on collaboratively.</span></span> <span data-ttu-id="f8a4d-151">התרשים הבא מתאר את האירועים ומציין שינויים שקורים במהלך תהליך הקצאת הקבוצה.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-151">The following diagram depicts the events and state changes that happen during the group assignment process.</span></span>

<span data-ttu-id="f8a4d-152">Project Operations לא יוצר קבוצה באמצעות פעולה משתמעת ועושה זאת רק באמצעות פעולה מפורשת של קבוצות הדורשות זאת.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-152">Project Operations does not create a group through implicit action and only does so through the explicit action of pressing groups.</span></span>

<span data-ttu-id="f8a4d-153">חיפוש חבר קבוצה בדו-שיח **ניהול קבוצה** מוגבל לאלה המוגדרים כחלק מקבוצת האבטחה של הסביבה.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-153">Group member search in the **Group management** dialog, is limited to those who are set as part of the environment's security group.</span></span> <span data-ttu-id="f8a4d-154">למידע נוסף, ראה [בקרה על גישת משתמשים לסביבות: קבוצות אבטחה ורשיונות](https://docs.microsoft.com/power-platform/admin/control-user-access).</span><span class="sxs-lookup"><span data-stu-id="f8a4d-154">For more information, see [Control user access to environments: security groups and licenses](https://docs.microsoft.com/power-platform/admin/control-user-access).</span></span>

![מצב הקבוצה](./media/groupsmode.png)

1. <span data-ttu-id="f8a4d-156">הפרויקט נוצר על-ידי המשתמש היוצר והוא בבעלותו.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-156">The Project is created and owned by the creating User.</span></span>
2. <span data-ttu-id="f8a4d-157">הבעלים של הפרויקט מעודכן בצוות.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-157">The Project owner is updated to the team.</span></span>
3. <span data-ttu-id="f8a4d-158">צוות הבעלים ממופה לקבוצת Office שצוינה או שנוצרה.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-158">The Owner team is mapped to the specified or created Office Group.</span></span>
4. <span data-ttu-id="f8a4d-159">הבעלים המקורי של הפרויקט מתווסף לקבוצת Office.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-159">The original owner of the Project is added to the Office Group.</span></span>

## <a name="deployment-recommendation"></a><span data-ttu-id="f8a4d-160">המלצת פריסה</span><span class="sxs-lookup"><span data-stu-id="f8a4d-160">Deployment recommendation</span></span>
<span data-ttu-id="f8a4d-161">ככל שמודל שיתוף הפעולה של קבוצת Office יתפתח, תתווסף פונקציונליות כדי לספק בקרה מפורטת יותר לאורך זמן.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-161">As the Office group collaboration model evolves, functionality will be added to provide more detailed control over time.</span></span> <span data-ttu-id="f8a4d-162">לקוחות הפורשים Project Operations היום מוזמנים להתמקד במודל האבטחה המסורתי של Microsoft Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="f8a4d-162">Customers that deploy Project Operations today are encouraged to focus on a traditional Microsoft Dynamics 365 security model.</span></span>

<span data-ttu-id="f8a4d-163">למידע נוסף, ראה [אבטחה ב- Common Data Service](https://docs.microsoft.com/power-platform/admin/wp-security)</span><span class="sxs-lookup"><span data-stu-id="f8a4d-163">For more information, see [Security in Common Data Service](https://docs.microsoft.com/power-platform/admin/wp-security).</span></span>

## <a name="project-operations-and-microsoft-dynamics-365-finance-security"></a><span data-ttu-id="f8a4d-164">Project Operations ואבטחה של Microsoft Dynamics 365 Finance</span><span class="sxs-lookup"><span data-stu-id="f8a4d-164">Project Operations and Microsoft Dynamics 365 Finance security</span></span>
<span data-ttu-id="f8a4d-165">Project Operations כולל את התפקידים הבאים:</span><span class="sxs-lookup"><span data-stu-id="f8a4d-165">Project Operations includes the following roles:</span></span>

- <span data-ttu-id="f8a4d-166">מנהל פרויקט</span><span class="sxs-lookup"><span data-stu-id="f8a4d-166">Project manager</span></span>
- <span data-ttu-id="f8a4d-167">רואה חשבון של פרויקט</span><span class="sxs-lookup"><span data-stu-id="f8a4d-167">Project accountant</span></span>

<span data-ttu-id="f8a4d-168">למידע נוסף על אבטחה ב- Finance, ראה [אבטחה מבוססת תפקידים](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/role-based-security).</span><span class="sxs-lookup"><span data-stu-id="f8a4d-168">For more information about security in Finance, see [Role-based security](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/role-based-security).</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]