---
title: העתקת פרוייקט
description: נושא זה מספק מידע על העתקת פרוייקטים ב-Dynamics 365 Project operations.
author: ruhercul
manager: AnnBe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: cf80f2a1cd27aae33d123e45dee70d94ea4d01a9
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077249"
---
# <a name="copy-a-project"></a><span data-ttu-id="ac2fb-103">העתקת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ac2fb-103">Copy a project</span></span>

<span data-ttu-id="ac2fb-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="ac2fb-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ac2fb-105">באמצעות Dynamics 365 Project Operations, ניתן לבנות במהירות פרויקטים חדשים באמצעות בחירה באפשרות **העתק פרויקט** בטופס **פרויקטים**.</span><span class="sxs-lookup"><span data-stu-id="ac2fb-105">With Dynamics 365 Project Operations, you can quickly build new projects by selecting **Copy Project** on the **Projects** form.</span></span> <span data-ttu-id="ac2fb-106">להעתקת פרויקט, פתח את הפרויקט שברצונך להעתיק ואז בחר **העתק פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="ac2fb-106">To copy a project, open the project you want to copy, and then select **Copy project**.</span></span> <span data-ttu-id="ac2fb-107">הפעולה תעתיק:</span><span class="sxs-lookup"><span data-stu-id="ac2fb-107">The action will copy:</span></span>

- <span data-ttu-id="ac2fb-108">מאפייני פרויקט</span><span class="sxs-lookup"><span data-stu-id="ac2fb-108">Project properties</span></span>
- <span data-ttu-id="ac2fb-109">מבנה התפלגות העבודה</span><span class="sxs-lookup"><span data-stu-id="ac2fb-109">The Work breakdown structure</span></span>
- <span data-ttu-id="ac2fb-110">חברי צוות בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="ac2fb-110">Project team members</span></span>
- <span data-ttu-id="ac2fb-111">הערכות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ac2fb-111">Project estimates</span></span>
- <span data-ttu-id="ac2fb-112">הערכות הוצאה בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="ac2fb-112">Project expense estimates</span></span>

## <a name="project-properties"></a><span data-ttu-id="ac2fb-113">מאפייני פרויקט</span><span class="sxs-lookup"><span data-stu-id="ac2fb-113">Project properties</span></span>

<span data-ttu-id="ac2fb-114">כאשר הפרויקט מועתק, הערכים בשדות הבאים מועתקים:</span><span class="sxs-lookup"><span data-stu-id="ac2fb-114">When the project is copied, the values in the following fields are copied:</span></span>

- <span data-ttu-id="ac2fb-115">שם</span><span class="sxs-lookup"><span data-stu-id="ac2fb-115">Name</span></span>
- <span data-ttu-id="ac2fb-116">תיאור</span><span class="sxs-lookup"><span data-stu-id="ac2fb-116">Description</span></span>
- <span data-ttu-id="ac2fb-117">לקוח</span><span class="sxs-lookup"><span data-stu-id="ac2fb-117">Customer</span></span>
- <span data-ttu-id="ac2fb-118">תבנית לוח שנה</span><span class="sxs-lookup"><span data-stu-id="ac2fb-118">Calendar Template</span></span>
- <span data-ttu-id="ac2fb-119">מטבע</span><span class="sxs-lookup"><span data-stu-id="ac2fb-119">Currency</span></span>
- <span data-ttu-id="ac2fb-120">יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="ac2fb-120">Contracting Unit</span></span>
- <span data-ttu-id="ac2fb-121">מנהל פרויקט</span><span class="sxs-lookup"><span data-stu-id="ac2fb-121">Project Manager</span></span>
- <span data-ttu-id="ac2fb-122">סטאטוס</span><span class="sxs-lookup"><span data-stu-id="ac2fb-122">Status</span></span>
- <span data-ttu-id="ac2fb-123">מצב פרויקט כולל</span><span class="sxs-lookup"><span data-stu-id="ac2fb-123">Overall Project Status</span></span>
- <span data-ttu-id="ac2fb-124">הערות </span><span class="sxs-lookup"><span data-stu-id="ac2fb-124">Comments</span></span>
- <span data-ttu-id="ac2fb-125">הערכות</span><span class="sxs-lookup"><span data-stu-id="ac2fb-125">Estimates</span></span>
- <span data-ttu-id="ac2fb-126">תאריך התחלה משוער</span><span class="sxs-lookup"><span data-stu-id="ac2fb-126">Estimated Start Date</span></span>
- <span data-ttu-id="ac2fb-127">תאריך סיום</span><span class="sxs-lookup"><span data-stu-id="ac2fb-127">Finish Date</span></span>
- <span data-ttu-id="ac2fb-128">מאמץ (בשעות)</span><span class="sxs-lookup"><span data-stu-id="ac2fb-128">Effort (Hours)</span></span>
- <span data-ttu-id="ac2fb-129">עלות עבודה משוערת</span><span class="sxs-lookup"><span data-stu-id="ac2fb-129">Estimated Labor Cost</span></span>
- <span data-ttu-id="ac2fb-130">עלות הוצאות משוערת</span><span class="sxs-lookup"><span data-stu-id="ac2fb-130">Estimated Expense Cost</span></span>

## <a name="work-breakdown-structure"></a><span data-ttu-id="ac2fb-131">מבנה התפלגות העבודה</span><span class="sxs-lookup"><span data-stu-id="ac2fb-131">Work breakdown structure</span></span>

<span data-ttu-id="ac2fb-132">כאשר הפרויקט מועתק, כל מבנה התפלגות העבודה של המשאב שנטען מועתק.</span><span class="sxs-lookup"><span data-stu-id="ac2fb-132">When the project is copied, the entire resource-loaded work breakdown structure is copied.</span></span> <span data-ttu-id="ac2fb-133">משאבים בעלי שם מוחלפים במשאבים כלליים.</span><span class="sxs-lookup"><span data-stu-id="ac2fb-133">Named resources are replaced with generic resources.</span></span> <span data-ttu-id="ac2fb-134">אם למשאבים בעלי השם אין את אותן שעות עבודה כמו למשאב הכללי, לוח הזמנים יחושב מחדש ומשך המשימות עשוי להשתנות.</span><span class="sxs-lookup"><span data-stu-id="ac2fb-134">If the named resources don't have the same working hours as the generic resource, the schedule will be recalculated and task durations may change.</span></span>

## <a name="project-team-members"></a><span data-ttu-id="ac2fb-135">חברי צוות בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="ac2fb-135">Project team members</span></span>

<span data-ttu-id="ac2fb-136">כאשר צוות פרויקט מועתק מפרויקט המקור, המשאבים הכלליים מועתקים.</span><span class="sxs-lookup"><span data-stu-id="ac2fb-136">When a project team is copied from the source project, the generic resources are copied.</span></span> <span data-ttu-id="ac2fb-137">הקצאות של המשאבים הכלליים נשארות כפי השהיו בפרוייקט המקור.</span><span class="sxs-lookup"><span data-stu-id="ac2fb-137">Generic resource assignments are also maintained as they were in the source project.</span></span> <span data-ttu-id="ac2fb-138">משאבים בעלי שם יומרו לחברי צוות כלליים.</span><span class="sxs-lookup"><span data-stu-id="ac2fb-138">Named resources will be converted to generic team members.</span></span>

## <a name="estimates"></a><span data-ttu-id="ac2fb-139">הערכות</span><span class="sxs-lookup"><span data-stu-id="ac2fb-139">Estimates</span></span>

<span data-ttu-id="ac2fb-140">כאשר מועתק הפרויקט, מעותקות גם שורות הערכת המשאבים וההוצאות מפרויקט המקור.</span><span class="sxs-lookup"><span data-stu-id="ac2fb-140">When the project is copied, both resource and expense estimate lines are copied from the source project.</span></span> 

<span data-ttu-id="ac2fb-141">למידע על אופן הגישה הפרוגרמטית אל 'העתק פוריקט', ראה [פיתוח תבניות פרוייקט באמצעות 'העתקת פוריקט'](dev-copy-project.md).</span><span class="sxs-lookup"><span data-stu-id="ac2fb-141">For information on how to programmatically access Copy Project, see [Develop project templates with Copy Project](dev-copy-project.md).</span></span>
