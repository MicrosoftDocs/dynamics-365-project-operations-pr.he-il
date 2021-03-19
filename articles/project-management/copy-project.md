---
title: העתקת פרוייקט
description: נושא זו מספק מידע על העתקת פרויקטים ב- Dynamics 365 Project Operations.
author: ruhercul
manager: AnnBe
ms.date: 02/22/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: af1942e81691d9e13fdcbbf68599c1a8a4004582
ms.sourcegitcommit: 24528bb9c0ef8898077cb3bc672daa211c0e73aa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "5479520"
---
# <a name="copy-a-project"></a><span data-ttu-id="23a0b-103">העתקת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="23a0b-103">Copy a project</span></span>

<span data-ttu-id="23a0b-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="23a0b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="23a0b-105">עם Dynamics 365 Project Operations אפשר לבנות במהירות פרויקטים חדשים על ידי בחירה באפשרות **העתק פרויקט** בטופס **פרויקטים** .</span><span class="sxs-lookup"><span data-stu-id="23a0b-105">With Dynamics 365 Project Operations, you can quickly build new projects by selecting **Copy Project** on the **Projects** form.</span></span> <span data-ttu-id="23a0b-106">להעתקת פרויקט, פתח את הפרויקט שברצונך להעתיק ואז בחר **העתק פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="23a0b-106">To copy a project, open the project you want to copy, and then select **Copy project**.</span></span> <span data-ttu-id="23a0b-107">הפעולה תעתיק:</span><span class="sxs-lookup"><span data-stu-id="23a0b-107">The action will copy:</span></span>

- <span data-ttu-id="23a0b-108">מאפייני פרויקט (תאריך ההתחלה המשוער מועתק מפרויקט המקור)</span><span class="sxs-lookup"><span data-stu-id="23a0b-108">Project properties (The estimated start date is copied from the source project)</span></span>
- <span data-ttu-id="23a0b-109">מבנה התפלגות העבודה</span><span class="sxs-lookup"><span data-stu-id="23a0b-109">The Work breakdown structure</span></span>
- <span data-ttu-id="23a0b-110">חברי צוות בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="23a0b-110">Project team members</span></span>
- <span data-ttu-id="23a0b-111">הערכות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="23a0b-111">Project estimates</span></span>
- <span data-ttu-id="23a0b-112">הערכות הוצאה בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="23a0b-112">Project expense estimates</span></span>

## <a name="project-properties"></a><span data-ttu-id="23a0b-113">מאפייני פרויקט</span><span class="sxs-lookup"><span data-stu-id="23a0b-113">Project properties</span></span>

<span data-ttu-id="23a0b-114">כאשר הפרויקט מועתק, הערכים בשדות הבאים מועתקים:</span><span class="sxs-lookup"><span data-stu-id="23a0b-114">When the project is copied, the values in the following fields are copied:</span></span>

- <span data-ttu-id="23a0b-115">שם</span><span class="sxs-lookup"><span data-stu-id="23a0b-115">Name</span></span>
- <span data-ttu-id="23a0b-116">תיאור</span><span class="sxs-lookup"><span data-stu-id="23a0b-116">Description</span></span>
- <span data-ttu-id="23a0b-117">לקוח</span><span class="sxs-lookup"><span data-stu-id="23a0b-117">Customer</span></span>
- <span data-ttu-id="23a0b-118">תבנית לוח שנה</span><span class="sxs-lookup"><span data-stu-id="23a0b-118">Calendar Template</span></span>
- <span data-ttu-id="23a0b-119">מטבע</span><span class="sxs-lookup"><span data-stu-id="23a0b-119">Currency</span></span>
- <span data-ttu-id="23a0b-120">יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="23a0b-120">Contracting Unit</span></span>
- <span data-ttu-id="23a0b-121">מנהל פרויקט</span><span class="sxs-lookup"><span data-stu-id="23a0b-121">Project Manager</span></span>
- <span data-ttu-id="23a0b-122">סטאטוס</span><span class="sxs-lookup"><span data-stu-id="23a0b-122">Status</span></span>
- <span data-ttu-id="23a0b-123">מצב פרויקט כולל</span><span class="sxs-lookup"><span data-stu-id="23a0b-123">Overall Project Status</span></span>
- <span data-ttu-id="23a0b-124">הערות </span><span class="sxs-lookup"><span data-stu-id="23a0b-124">Comments</span></span>
- <span data-ttu-id="23a0b-125">הערכות</span><span class="sxs-lookup"><span data-stu-id="23a0b-125">Estimates</span></span>
- <span data-ttu-id="23a0b-126">תאריך התחלה משוער</span><span class="sxs-lookup"><span data-stu-id="23a0b-126">Estimated Start Date</span></span>
- <span data-ttu-id="23a0b-127">תאריך סיום</span><span class="sxs-lookup"><span data-stu-id="23a0b-127">Finish Date</span></span>
- <span data-ttu-id="23a0b-128">מאמץ (בשעות)</span><span class="sxs-lookup"><span data-stu-id="23a0b-128">Effort (Hours)</span></span>
- <span data-ttu-id="23a0b-129">עלות עבודה משוערת</span><span class="sxs-lookup"><span data-stu-id="23a0b-129">Estimated Labor Cost</span></span>
- <span data-ttu-id="23a0b-130">עלות הוצאות משוערת</span><span class="sxs-lookup"><span data-stu-id="23a0b-130">Estimated Expense Cost</span></span>

## <a name="work-breakdown-structure"></a><span data-ttu-id="23a0b-131">מבנה התפלגות העבודה</span><span class="sxs-lookup"><span data-stu-id="23a0b-131">Work breakdown structure</span></span>

<span data-ttu-id="23a0b-132">כאשר הפרויקט מועתק, כל מבנה התפלגות העבודה של המשאב שנטען מועתק.</span><span class="sxs-lookup"><span data-stu-id="23a0b-132">When the project is copied, the entire resource-loaded work breakdown structure is copied.</span></span> <span data-ttu-id="23a0b-133">משאבים בעלי שם מוחלפים במשאבים כלליים.</span><span class="sxs-lookup"><span data-stu-id="23a0b-133">Named resources are replaced with generic resources.</span></span> <span data-ttu-id="23a0b-134">אם למשאבים בעלי השם אין את אותן שעות עבודה כמו למשאב הכללי, לוח הזמנים יחושב מחדש ומשך המשימות עשוי להשתנות.</span><span class="sxs-lookup"><span data-stu-id="23a0b-134">If the named resources don't have the same working hours as the generic resource, the schedule will be recalculated and task durations may change.</span></span>

## <a name="project-team-members"></a><span data-ttu-id="23a0b-135">חברי צוות בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="23a0b-135">Project team members</span></span>

<span data-ttu-id="23a0b-136">כאשר צוות פרויקט מועתק מפרויקט המקור, המשאבים הכלליים מועתקים.</span><span class="sxs-lookup"><span data-stu-id="23a0b-136">When a project team is copied from the source project, the generic resources are copied.</span></span> <span data-ttu-id="23a0b-137">הקצאות של המשאבים הכלליים נשארות כפי השהיו בפרוייקט המקור.</span><span class="sxs-lookup"><span data-stu-id="23a0b-137">Generic resource assignments are also maintained as they were in the source project.</span></span> <span data-ttu-id="23a0b-138">משאבים בעלי שם יומרו לחברי צוות כלליים.</span><span class="sxs-lookup"><span data-stu-id="23a0b-138">Named resources will be converted to generic team members.</span></span>

## <a name="estimates"></a><span data-ttu-id="23a0b-139">הערכות</span><span class="sxs-lookup"><span data-stu-id="23a0b-139">Estimates</span></span>

<span data-ttu-id="23a0b-140">כאשר מועתק הפרויקט, מעותקות גם שורות הערכת המשאבים וההוצאות מפרויקט המקור.</span><span class="sxs-lookup"><span data-stu-id="23a0b-140">When the project is copied, both resource and expense estimate lines are copied from the source project.</span></span> 

<span data-ttu-id="23a0b-141">למידע על אופן הגישה הפרוגרמטית אל 'העתק פוריקט', ראה [פיתוח תבניות פרוייקט באמצעות 'העתקת פוריקט'](dev-copy-project.md).</span><span class="sxs-lookup"><span data-stu-id="23a0b-141">For information on how to programmatically access Copy Project, see [Develop project templates with Copy Project](dev-copy-project.md).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
