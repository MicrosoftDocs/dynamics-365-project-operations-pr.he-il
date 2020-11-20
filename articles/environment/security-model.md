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
ms.openlocfilehash: 3fc4101d0ea4b8e2a4ba8f1d43540d57239cf402
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4124369"
---
# <a name="security-model"></a><span data-ttu-id="e0782-103">מודל האבטחה</span><span class="sxs-lookup"><span data-stu-id="e0782-103">Security Model</span></span>

<span data-ttu-id="e0782-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="e0782-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e0782-105">Microsoft Dynamics 365 Project Operations מכיל מודל אבטחה ייחודי המאפשר מודל אבטחה עסקי מבוסס תפקיד המשתף פעולה עם קבוצות Microsoft Office.</span><span class="sxs-lookup"><span data-stu-id="e0782-105">Microsoft Dynamics 365 Project Operations contains a unique security model that allows for a role-based business security model that collaborates with Microsoft Office Groups.</span></span> 


## <a name="security-roles"></a><span data-ttu-id="e0782-106">תפקידי אבטחה</span><span class="sxs-lookup"><span data-stu-id="e0782-106">Security roles</span></span>
<span data-ttu-id="e0782-107">יכולות החזית של Project Operations כוללות את התפקידים הבאים:</span><span class="sxs-lookup"><span data-stu-id="e0782-107">Project Operations front-end capabilities include the following roles:</span></span>

| <span data-ttu-id="e0782-108">תפקיד</span><span class="sxs-lookup"><span data-stu-id="e0782-108">Role</span></span>                          | <span data-ttu-id="e0782-109">תיאור</span><span class="sxs-lookup"><span data-stu-id="e0782-109">Description</span></span>                                                                                                                                                                 | <span data-ttu-id="e0782-110">Scope</span><span class="sxs-lookup"><span data-stu-id="e0782-110">Scope</span></span> |
|-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|
| <span data-ttu-id="e0782-111">מנהל שיטות עבודה</span><span class="sxs-lookup"><span data-stu-id="e0782-111">Practice manager</span></span>              | <span data-ttu-id="e0782-112">תומך בדיווח חוצה פרויקט.</span><span class="sxs-lookup"><span data-stu-id="e0782-112">Supports cross-project reporting.</span></span>                                                                                                            | <span data-ttu-id="e0782-113">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="e0782-113">Business unit</span></span>              |
| <span data-ttu-id="e0782-114">מאשר הפרויקט</span><span class="sxs-lookup"><span data-stu-id="e0782-114">Project approver</span></span>              | <span data-ttu-id="e0782-115">מאשר שעות והוצאות כנגד פרויקט.</span><span class="sxs-lookup"><span data-stu-id="e0782-115">Approves time and expenses against a project.</span></span>                                                                                                                              | <span data-ttu-id="e0782-116">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="e0782-116">Business unit</span></span> |
| <span data-ttu-id="e0782-117">מנהל חיוב פרויקט</span><span class="sxs-lookup"><span data-stu-id="e0782-117">Project billing administrator</span></span> | <span data-ttu-id="e0782-118">יוצר את הצעת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="e0782-118">Creates the invoice proposal.</span></span>                                                                                                                                                 | <span data-ttu-id="e0782-119">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="e0782-119">Business unit</span></span> |
| <span data-ttu-id="e0782-120">מנהל פרויקט</span><span class="sxs-lookup"><span data-stu-id="e0782-120">Project manager</span></span>               | <span data-ttu-id="e0782-121">יוצר את תוכנית הפרויקט ומבקש משאבים.</span><span class="sxs-lookup"><span data-stu-id="e0782-121">Creates the project plan and requests resources.</span></span>                                                                                                                              | <span data-ttu-id="e0782-122">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="e0782-122">Business unit</span></span> |
| <span data-ttu-id="e0782-123">משאב פרויקט</span><span class="sxs-lookup"><span data-stu-id="e0782-123">Project resource</span></span>              | <span data-ttu-id="e0782-124">חברי צוות שניתן להזמין אותם והם יכולים לדווח על שעות.</span><span class="sxs-lookup"><span data-stu-id="e0782-124">Team members who can be booked and report time.</span></span>                                                                                                          | <span data-ttu-id="e0782-125">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="e0782-125">Business unit</span></span>|
| <span data-ttu-id="e0782-126">מנהל משאבים</span><span class="sxs-lookup"><span data-stu-id="e0782-126">Resource manager</span></span>              | <span data-ttu-id="e0782-127">כל פונקציות ניהול המשאבים, כגון מילוי בקשות והזמנות של משאבים, מופרדות לתמיכה בתצורה היברידית של מנהל פרויקט + מנהל משאבים ובתפקיד מנהל משאבים יחיד ומרכזי.</span><span class="sxs-lookup"><span data-stu-id="e0782-127">All resource management functions, such as fulfill resource requests and bookings, separated to support a hybrid Project manager + Resource manager configuration and a single and centralized Resource manager role.</span></span> | <span data-ttu-id="e0782-128">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="e0782-128">Business unit</span></span> |


<span data-ttu-id="e0782-129">Microsoft Project באינטרנט כולל את התפקידים הבאים:</span><span class="sxs-lookup"><span data-stu-id="e0782-129">Microsoft Project for the Web includes the following roles:</span></span>

| <span data-ttu-id="e0782-130">תפקיד</span><span class="sxs-lookup"><span data-stu-id="e0782-130">Role</span></span>           | <span data-ttu-id="e0782-131">תיאור</span><span class="sxs-lookup"><span data-stu-id="e0782-131">Description</span></span>                                                                                                        | <span data-ttu-id="e0782-132">Scope</span><span class="sxs-lookup"><span data-stu-id="e0782-132">Scope</span></span>  |
|----------------|--------------------------------------------------------------------------------------------------------------------|--------|
| <span data-ttu-id="e0782-133">משתמש בפרויקט</span><span class="sxs-lookup"><span data-stu-id="e0782-133">Project user</span></span>   | <span data-ttu-id="e0782-134">משתמש משותף של Project המסוגל ליצור פרויקטים משלו ולהציג את כל הפרויקטים המשותפים איתו.</span><span class="sxs-lookup"><span data-stu-id="e0782-134">Collaborative user of Project   who is able to create their own projects and view any projects shared with   them.</span></span> | <span data-ttu-id="e0782-135">משתמש</span><span class="sxs-lookup"><span data-stu-id="e0782-135">User</span></span>   |
| <span data-ttu-id="e0782-136">מערכת פרויקט</span><span class="sxs-lookup"><span data-stu-id="e0782-136">Project system</span></span> | <span data-ttu-id="e0782-137">תפקיד המשמש להקשר יישום.</span><span class="sxs-lookup"><span data-stu-id="e0782-137">Role used for application   context.</span></span> <span data-ttu-id="e0782-138">לקוחות לא אמורים להשתמש בתפקיד מערכת זה.</span><span class="sxs-lookup"><span data-stu-id="e0782-138">Customers should not use this system role.</span></span>                                    | <span data-ttu-id="e0782-139">כללי</span><span class="sxs-lookup"><span data-stu-id="e0782-139">Global</span></span> |

## <a name="security-enforcement"></a><span data-ttu-id="e0782-140">אכיפת אבטחה</span><span class="sxs-lookup"><span data-stu-id="e0782-140">Security enforcement</span></span>
<span data-ttu-id="e0782-141">פעולות המתבצעות ברמת הפרויקט מבוצעות בהקשר של המשתמש המחובר.</span><span class="sxs-lookup"><span data-stu-id="e0782-141">Actions that are performed at the project level are performed in the context of the logged in user.</span></span> <span data-ttu-id="e0782-142">המשמעות היא שכדי ליצור, לפתוח או למחוק פרויקט, למשתמש נדרשת גישה ל- CDS.</span><span class="sxs-lookup"><span data-stu-id="e0782-142">This means that in order to create, open, or delete a project, the user is required to have access available in CDS.</span></span> <span data-ttu-id="e0782-143">ניתן להעניק גישה ל- CDS באמצעות כל אחד מהמנגנונים האפשריים הכלולים בפלטפורמה.</span><span class="sxs-lookup"><span data-stu-id="e0782-143">Access in CDS may be granted through any of the possible mechanisms included in the platform.</span></span> <span data-ttu-id="e0782-144">לדוגמה, משתמש עם טווח גדול יותר רשאי לגשת לפרויקט או אם בוצעה פעולה מפורשת לשיתוף פרויקט המעניקה למשתמש גישה.</span><span class="sxs-lookup"><span data-stu-id="e0782-144">For example, a user with a larger scope may access the project or if an explicit project share action has been performed which grants the user access.</span></span>

<span data-ttu-id="e0782-145">חשוב להביא את זה בחשבון בעת יצירת פרויקטים ב- Project Operations.</span><span class="sxs-lookup"><span data-stu-id="e0782-145">It's important to consider this when creating projects in Project Operations.</span></span>

## <a name="modern-group-collaboration-with-project-operations"></a><span data-ttu-id="e0782-146">שיתוף פעולה מודרני בין קבוצות עם Project Operations</span><span class="sxs-lookup"><span data-stu-id="e0782-146">Modern group collaboration with Project Operations</span></span>
<span data-ttu-id="e0782-147">Project באינטרנט ו- Project Operations תומכים בקבוצות מודרניות לשיתוף פעולה.</span><span class="sxs-lookup"><span data-stu-id="e0782-147">Project for the Web and Project Operations support modern groups for collaboration.</span></span> <span data-ttu-id="e0782-148">משתמשים שנוספו לפרויקט באמצעות קבוצה יכולים לערוך את תוכנית הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="e0782-148">Users added to the project through a group are able to edit the project plan.</span></span>

<span data-ttu-id="e0782-149">Project באינטרנט מוסיף משתמשים לקבוצה באופן אוטומטי עם ההקצאה.</span><span class="sxs-lookup"><span data-stu-id="e0782-149">Project for the Web adds users to the group automatically upon assignment.</span></span>

<span data-ttu-id="e0782-150">הקבוצות מאפשרות לעבוד בשיתוף פעולה על ההרשאות לפרויקט ועל תוצרים נתמכים של שיתוף הפעולה.</span><span class="sxs-lookup"><span data-stu-id="e0782-150">Groups allow the permissions of the project and supporting collaboration artifacts to be worked on collaboratively.</span></span> <span data-ttu-id="e0782-151">התרשים הבא מתאר את האירועים ומציין שינויים שקורים במהלך תהליך הקצאת הקבוצה.</span><span class="sxs-lookup"><span data-stu-id="e0782-151">The following diagram depicts the events and state changes that happen during the group assignment process.</span></span>

<span data-ttu-id="e0782-152">Project Operations לא יוצר קבוצה באמצעות פעולה משתמעת ועושה זאת רק באמצעות פעולה מפורשת של קבוצות הדורשות זאת.</span><span class="sxs-lookup"><span data-stu-id="e0782-152">Project Operations does not create a group through implicit action and only does so through the explicit action of pressing groups.</span></span>

<span data-ttu-id="e0782-153">חיפוש חבר קבוצה בדו-שיח **ניהול קבוצה** מוגבל לאלה המוגדרים כחלק מקבוצת האבטחה של הסביבה.</span><span class="sxs-lookup"><span data-stu-id="e0782-153">Group member search in the **Group management** dialog, is limited to those who are set as part of the environment's security group.</span></span> <span data-ttu-id="e0782-154">למידע נוסף, ראה [בקרה על גישת משתמשים לסביבות: קבוצות אבטחה ורשיונות](https://docs.microsoft.com/power-platform/admin/control-user-access).</span><span class="sxs-lookup"><span data-stu-id="e0782-154">For more information, see [Control user access to environments: security groups and licenses](https://docs.microsoft.com/power-platform/admin/control-user-access).</span></span>

![מצב הקבוצה](./media/groupsmode.png)

1. <span data-ttu-id="e0782-156">הפרויקט נוצר על-ידי המשתמש היוצר והוא בבעלותו.</span><span class="sxs-lookup"><span data-stu-id="e0782-156">The Project is created and owned by the creating User.</span></span>
2. <span data-ttu-id="e0782-157">הבעלים של הפרויקט מעודכן בצוות.</span><span class="sxs-lookup"><span data-stu-id="e0782-157">The Project owner is updated to the team.</span></span>
3. <span data-ttu-id="e0782-158">צוות הבעלים ממופה לקבוצת Office שצוינה או שנוצרה.</span><span class="sxs-lookup"><span data-stu-id="e0782-158">The Owner team is mapped to the specified or created Office Group.</span></span>
4. <span data-ttu-id="e0782-159">הבעלים המקורי של הפרויקט מתווסף לקבוצת Office.</span><span class="sxs-lookup"><span data-stu-id="e0782-159">The original owner of the Project is added to the Office Group.</span></span>

## <a name="deployment-recommendation"></a><span data-ttu-id="e0782-160">המלצת פריסה</span><span class="sxs-lookup"><span data-stu-id="e0782-160">Deployment recommendation</span></span>
<span data-ttu-id="e0782-161">ככל שמודל שיתוף הפעולה של קבוצת Office יתפתח, תתווסף פונקציונליות כדי לספק בקרה מפורטת יותר לאורך זמן.</span><span class="sxs-lookup"><span data-stu-id="e0782-161">As the Office group collaboration model evolves, functionality will be added to provide more detailed control over time.</span></span> <span data-ttu-id="e0782-162">לקוחות הפורשים Project Operations היום מוזמנים להתמקד במודל האבטחה המסורתי של Microsoft Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="e0782-162">Customers that deploy Project Operations today are encouraged to focus on a traditional Microsoft Dynamics 365 security model.</span></span>

<span data-ttu-id="e0782-163">למידע נוסף, ראה [אבטחה ב- Common Data Service](https://docs.microsoft.com/power-platform/admin/wp-security)</span><span class="sxs-lookup"><span data-stu-id="e0782-163">For more information, see [Security in Common Data Service](https://docs.microsoft.com/power-platform/admin/wp-security).</span></span>

## <a name="project-operations-and-microsoft-dynamics-365-finance-security"></a><span data-ttu-id="e0782-164">Project Operations ואבטחה של Microsoft Dynamics 365 Finance</span><span class="sxs-lookup"><span data-stu-id="e0782-164">Project Operations and Microsoft Dynamics 365 Finance security</span></span>
<span data-ttu-id="e0782-165">Project Operations כולל את התפקידים הבאים:</span><span class="sxs-lookup"><span data-stu-id="e0782-165">Project Operations includes the following roles:</span></span>

- <span data-ttu-id="e0782-166">מנהל פרויקט</span><span class="sxs-lookup"><span data-stu-id="e0782-166">Project manager</span></span>
- <span data-ttu-id="e0782-167">רואה חשבון של פרויקט</span><span class="sxs-lookup"><span data-stu-id="e0782-167">Project accountant</span></span>

<span data-ttu-id="e0782-168">למידע נוסף על אבטחה ב- Finance, ראה [אבטחה מבוססת תפקידים](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/role-based-security).</span><span class="sxs-lookup"><span data-stu-id="e0782-168">For more information about security in Finance, see [Role-based security](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/role-based-security).</span></span>


