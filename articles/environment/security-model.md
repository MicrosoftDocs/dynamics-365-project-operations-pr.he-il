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
ms.openlocfilehash: 8acaa86dec8ebca8f9850877d345e30be3e3a919
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2021
ms.locfileid: "5951210"
---
# <a name="security-model"></a><span data-ttu-id="17522-103">מודל האבטחה</span><span class="sxs-lookup"><span data-stu-id="17522-103">Security Model</span></span>

<span data-ttu-id="17522-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="17522-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="17522-105">Microsoft Dynamics 365 Project Operations מכיל מודל אבטחה ייחודי המאפשר מודל אבטחה עסקי שמבוסס על תפקידים ומשתף פעולה עם קבוצות Microsoft Office.</span><span class="sxs-lookup"><span data-stu-id="17522-105">Microsoft Dynamics 365 Project Operations contains a unique security model that allows for a role-based business security model that collaborates with Microsoft Office Groups.</span></span> 


## <a name="security-roles"></a><span data-ttu-id="17522-106">תפקידי אבטחה</span><span class="sxs-lookup"><span data-stu-id="17522-106">Security roles</span></span>
<span data-ttu-id="17522-107">יכולות החזית של Project Operations כוללות את התפקידים הבאים:</span><span class="sxs-lookup"><span data-stu-id="17522-107">Project Operations front-end capabilities include the following roles:</span></span>

| <span data-ttu-id="17522-108">תפקיד</span><span class="sxs-lookup"><span data-stu-id="17522-108">Role</span></span>                          | <span data-ttu-id="17522-109">תיאור</span><span class="sxs-lookup"><span data-stu-id="17522-109">Description</span></span>                                                                                                                                                                 | <span data-ttu-id="17522-110">Scope</span><span class="sxs-lookup"><span data-stu-id="17522-110">Scope</span></span> |
|-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|
| <span data-ttu-id="17522-111">מנהל שיטות עבודה</span><span class="sxs-lookup"><span data-stu-id="17522-111">Practice manager</span></span>              | <span data-ttu-id="17522-112">תומך בדיווח חוצה פרויקט.</span><span class="sxs-lookup"><span data-stu-id="17522-112">Supports cross-project reporting.</span></span>                                                                                                            | <span data-ttu-id="17522-113">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="17522-113">Business unit</span></span>              |
| <span data-ttu-id="17522-114">מאשר הפרויקט</span><span class="sxs-lookup"><span data-stu-id="17522-114">Project approver</span></span>              | <span data-ttu-id="17522-115">מאשר שעות והוצאות כנגד פרויקט.</span><span class="sxs-lookup"><span data-stu-id="17522-115">Approves time and expenses against a project.</span></span>                                                                                                                              | <span data-ttu-id="17522-116">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="17522-116">Business unit</span></span> |
| <span data-ttu-id="17522-117">מנהל חיוב פרויקט</span><span class="sxs-lookup"><span data-stu-id="17522-117">Project billing administrator</span></span> | <span data-ttu-id="17522-118">יוצר את הצעת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="17522-118">Creates the invoice proposal.</span></span>                                                                                                                                                 | <span data-ttu-id="17522-119">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="17522-119">Business unit</span></span> |
| <span data-ttu-id="17522-120">מנהל פרויקט</span><span class="sxs-lookup"><span data-stu-id="17522-120">Project manager</span></span>               | <span data-ttu-id="17522-121">יוצר את תוכנית הפרויקט ומבקש משאבים.</span><span class="sxs-lookup"><span data-stu-id="17522-121">Creates the project plan and requests resources.</span></span>                                                                                                                              | <span data-ttu-id="17522-122">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="17522-122">Business unit</span></span> |
| <span data-ttu-id="17522-123">משאב פרויקט</span><span class="sxs-lookup"><span data-stu-id="17522-123">Project resource</span></span>              | <span data-ttu-id="17522-124">חברי צוות שניתן להזמין אותם והם יכולים לדווח על שעות.</span><span class="sxs-lookup"><span data-stu-id="17522-124">Team members who can be booked and report time.</span></span>                                                                                                          | <span data-ttu-id="17522-125">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="17522-125">Business unit</span></span>|
| <span data-ttu-id="17522-126">מנהל משאבים</span><span class="sxs-lookup"><span data-stu-id="17522-126">Resource manager</span></span>              | <span data-ttu-id="17522-127">כל פונקציות ניהול המשאבים, כגון מילוי בקשות והזמנות של משאבים, מופרדות לתמיכה בתצורה היברידית של מנהל פרויקט + מנהל משאבים ובתפקיד מנהל משאבים יחיד ומרכזי.</span><span class="sxs-lookup"><span data-stu-id="17522-127">All resource management functions, such as fulfill resource requests and bookings, separated to support a hybrid Project manager + Resource manager configuration and a single and centralized Resource manager role.</span></span> | <span data-ttu-id="17522-128">יחידה עסקית</span><span class="sxs-lookup"><span data-stu-id="17522-128">Business unit</span></span> |


<span data-ttu-id="17522-129">Microsoft Project באינטרנט כולל את התפקידים הבאים:</span><span class="sxs-lookup"><span data-stu-id="17522-129">Microsoft Project for the Web includes the following roles:</span></span>

| <span data-ttu-id="17522-130">תפקיד</span><span class="sxs-lookup"><span data-stu-id="17522-130">Role</span></span>           | <span data-ttu-id="17522-131">תיאור</span><span class="sxs-lookup"><span data-stu-id="17522-131">Description</span></span>                                                                                                        | <span data-ttu-id="17522-132">Scope</span><span class="sxs-lookup"><span data-stu-id="17522-132">Scope</span></span>  |
|----------------|--------------------------------------------------------------------------------------------------------------------|--------|
| <span data-ttu-id="17522-133">משתמש בפרויקט</span><span class="sxs-lookup"><span data-stu-id="17522-133">Project user</span></span>   | <span data-ttu-id="17522-134">משתמש משותף של Project המסוגל ליצור פרויקטים משלו ולהציג את כל הפרויקטים המשותפים איתו.</span><span class="sxs-lookup"><span data-stu-id="17522-134">Collaborative user of Project   who is able to create their own projects and view any projects shared with   them.</span></span> | <span data-ttu-id="17522-135">משתמש</span><span class="sxs-lookup"><span data-stu-id="17522-135">User</span></span>   |
| <span data-ttu-id="17522-136">מערכת פרויקט</span><span class="sxs-lookup"><span data-stu-id="17522-136">Project system</span></span> | <span data-ttu-id="17522-137">תפקיד המשמש להקשר יישום.</span><span class="sxs-lookup"><span data-stu-id="17522-137">Role used for application   context.</span></span> <span data-ttu-id="17522-138">לקוחות לא אמורים להשתמש בתפקיד מערכת זה.</span><span class="sxs-lookup"><span data-stu-id="17522-138">Customers should not use this system role.</span></span>                                    | <span data-ttu-id="17522-139">כללי</span><span class="sxs-lookup"><span data-stu-id="17522-139">Global</span></span> |

## <a name="security-enforcement"></a><span data-ttu-id="17522-140">אכיפת אבטחה</span><span class="sxs-lookup"><span data-stu-id="17522-140">Security enforcement</span></span>
<span data-ttu-id="17522-141">פעולות המתבצעות ברמת הפרויקט מבוצעות בהקשר של המשתמש המחובר.</span><span class="sxs-lookup"><span data-stu-id="17522-141">Actions that are performed at the project level are performed in the context of the logged in user.</span></span> <span data-ttu-id="17522-142">המשמעות היא שכדי ליצור, לפתוח או למחוק פרויקט, למשתמש נדרשת גישה ל- CDS.</span><span class="sxs-lookup"><span data-stu-id="17522-142">This means that in order to create, open, or delete a project, the user is required to have access available in CDS.</span></span> <span data-ttu-id="17522-143">ניתן להעניק גישה ל- CDS באמצעות כל אחד מהמנגנונים האפשריים הכלולים בפלטפורמה.</span><span class="sxs-lookup"><span data-stu-id="17522-143">Access in CDS may be granted through any of the possible mechanisms included in the platform.</span></span> <span data-ttu-id="17522-144">לדוגמה, משתמש עם טווח גדול יותר רשאי לגשת לפרויקט או אם בוצעה פעולה מפורשת לשיתוף פרויקט המעניקה למשתמש גישה.</span><span class="sxs-lookup"><span data-stu-id="17522-144">For example, a user with a larger scope may access the project or if an explicit project share action has been performed which grants the user access.</span></span>

<span data-ttu-id="17522-145">חשוב להביא את זה בחשבון בעת יצירת פרויקטים ב- Project Operations.</span><span class="sxs-lookup"><span data-stu-id="17522-145">It's important to consider this when creating projects in Project Operations.</span></span>

## <a name="modern-group-collaboration-with-project-operations"></a><span data-ttu-id="17522-146">שיתוף פעולה מודרני בין קבוצות עם Project Operations</span><span class="sxs-lookup"><span data-stu-id="17522-146">Modern group collaboration with Project Operations</span></span>
<span data-ttu-id="17522-147">Project באינטרנט ו- Project Operations תומכים בקבוצות מודרניות לשיתוף פעולה.</span><span class="sxs-lookup"><span data-stu-id="17522-147">Project for the Web and Project Operations support modern groups for collaboration.</span></span> <span data-ttu-id="17522-148">משתמשים שנוספו לפרויקט באמצעות קבוצה יכולים לערוך את תוכנית הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="17522-148">Users added to the project through a group are able to edit the project plan.</span></span>

<span data-ttu-id="17522-149">Project באינטרנט מוסיף משתמשים לקבוצה באופן אוטומטי עם ההקצאה.</span><span class="sxs-lookup"><span data-stu-id="17522-149">Project for the Web adds users to the group automatically upon assignment.</span></span>

<span data-ttu-id="17522-150">הקבוצות מאפשרות לעבוד בשיתוף פעולה על ההרשאות לפרויקט ועל תוצרים נתמכים של שיתוף הפעולה.</span><span class="sxs-lookup"><span data-stu-id="17522-150">Groups allow the permissions of the project and supporting collaboration artifacts to be worked on collaboratively.</span></span> <span data-ttu-id="17522-151">התרשים הבא מתאר את האירועים ומציין שינויים שקורים במהלך תהליך הקצאת הקבוצה.</span><span class="sxs-lookup"><span data-stu-id="17522-151">The following diagram depicts the events and state changes that happen during the group assignment process.</span></span>

<span data-ttu-id="17522-152">Project Operations לא יוצר קבוצה באמצעות פעולה משתמעת ועושה זאת רק באמצעות פעולה מפורשת של קבוצות הדורשות זאת.</span><span class="sxs-lookup"><span data-stu-id="17522-152">Project Operations does not create a group through implicit action and only does so through the explicit action of pressing groups.</span></span>

<span data-ttu-id="17522-153">חיפוש חבר קבוצה בדו-שיח **ניהול קבוצה** מוגבל לאלה המוגדרים כחלק מקבוצת האבטחה של הסביבה.</span><span class="sxs-lookup"><span data-stu-id="17522-153">Group member search in the **Group management** dialog, is limited to those who are set as part of the environment's security group.</span></span> <span data-ttu-id="17522-154">למידע נוסף, ראה [בקרה על גישת משתמשים לסביבות: קבוצות אבטחה ורשיונות](/power-platform/admin/control-user-access).</span><span class="sxs-lookup"><span data-stu-id="17522-154">For more information, see [Control user access to environments: security groups and licenses](/power-platform/admin/control-user-access).</span></span>

![מצב הקבוצה](./media/groupsmode.png)

1. <span data-ttu-id="17522-156">הפרויקט נוצר על-ידי המשתמש היוצר והוא בבעלותו.</span><span class="sxs-lookup"><span data-stu-id="17522-156">The Project is created and owned by the creating User.</span></span>
2. <span data-ttu-id="17522-157">הבעלים של הפרויקט מעודכן בצוות.</span><span class="sxs-lookup"><span data-stu-id="17522-157">The Project owner is updated to the team.</span></span>
3. <span data-ttu-id="17522-158">צוות הבעלים ממופה לקבוצת Office שצוינה או שנוצרה.</span><span class="sxs-lookup"><span data-stu-id="17522-158">The Owner team is mapped to the specified or created Office Group.</span></span>
4. <span data-ttu-id="17522-159">הבעלים המקורי של הפרויקט מתווסף לקבוצת Office.</span><span class="sxs-lookup"><span data-stu-id="17522-159">The original owner of the Project is added to the Office Group.</span></span>

## <a name="deployment-recommendation"></a><span data-ttu-id="17522-160">המלצת פריסה</span><span class="sxs-lookup"><span data-stu-id="17522-160">Deployment recommendation</span></span>
<span data-ttu-id="17522-161">ככל שמודל שיתוף הפעולה של קבוצת Office יתפתח, תתווסף פונקציונליות כדי לספק בקרה מפורטת יותר לאורך זמן.</span><span class="sxs-lookup"><span data-stu-id="17522-161">As the Office group collaboration model evolves, functionality will be added to provide more detailed control over time.</span></span> <span data-ttu-id="17522-162">לקוחות הפורשים Project Operations היום מוזמנים להתמקד במודל האבטחה המסורתי של Microsoft Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="17522-162">Customers that deploy Project Operations today are encouraged to focus on a traditional Microsoft Dynamics 365 security model.</span></span>

<span data-ttu-id="17522-163">למידע נוסף, ראה [אבטחה ב- Common Data Service](/power-platform/admin/wp-security)</span><span class="sxs-lookup"><span data-stu-id="17522-163">For more information, see [Security in Common Data Service](/power-platform/admin/wp-security).</span></span>

## <a name="project-operations-and-microsoft-dynamics-365-finance-security"></a><span data-ttu-id="17522-164">Project Operations ואבטחה של Microsoft Dynamics 365 Finance</span><span class="sxs-lookup"><span data-stu-id="17522-164">Project Operations and Microsoft Dynamics 365 Finance security</span></span>
<span data-ttu-id="17522-165">Project Operations כולל את התפקידים הבאים:</span><span class="sxs-lookup"><span data-stu-id="17522-165">Project Operations includes the following roles:</span></span>

- <span data-ttu-id="17522-166">מנהל פרויקט</span><span class="sxs-lookup"><span data-stu-id="17522-166">Project manager</span></span>
- <span data-ttu-id="17522-167">רואה חשבון של פרויקט</span><span class="sxs-lookup"><span data-stu-id="17522-167">Project accountant</span></span>

<span data-ttu-id="17522-168">למידע נוסף על אבטחה ב- Finance, ראה [אבטחה מבוססת תפקידים](/dynamics365/fin-ops-core/dev-itpro/sysadmin/role-based-security).</span><span class="sxs-lookup"><span data-stu-id="17522-168">For more information about security in Finance, see [Role-based security](/dynamics365/fin-ops-core/dev-itpro/sysadmin/role-based-security).</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]