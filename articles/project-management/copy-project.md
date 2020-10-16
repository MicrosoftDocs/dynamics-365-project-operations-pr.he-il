---
title: העתקת פרוייקט
description: נושא זה מספק מידע על העתקת פרוייקטים ב-Dynamics 365 Project operations.
author: ruhercul
manager: AnnBe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: e35dc725e7938e9f59f7151dd1b37500fabf77a4
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908187"
---
# <a name="copy-a-project"></a><span data-ttu-id="93d39-103">העתקת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="93d39-103">Copy a project</span></span>

<span data-ttu-id="93d39-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="93d39-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="93d39-105">באמצעות Dynamics 365 Project Operations, תוכל לבנות במהירות פרויקטים חדשים באמצעות הפעולה **העתק פרויקט** בטופס **פרויקטים**.</span><span class="sxs-lookup"><span data-stu-id="93d39-105">With Dynamics 365 Project Operations, you can quickly build new projects by using the **Copy Project** action on the **Projects** from.</span></span> <span data-ttu-id="93d39-106">להעתקת פרויקט, בחר פרויקט ולאחר מכן בחר **העתק**.</span><span class="sxs-lookup"><span data-stu-id="93d39-106">To copy a project, select a project, and then select **Copy**.</span></span> <span data-ttu-id="93d39-107">הפעולה תעתיק:</span><span class="sxs-lookup"><span data-stu-id="93d39-107">The action will copy:</span></span>

- <span data-ttu-id="93d39-108">מאפייני פרויקט</span><span class="sxs-lookup"><span data-stu-id="93d39-108">Project properties</span></span>
- <span data-ttu-id="93d39-109">מבנה התפלגות העבודה</span><span class="sxs-lookup"><span data-stu-id="93d39-109">The Work breakdown structure</span></span>
- <span data-ttu-id="93d39-110">חברי צוות בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="93d39-110">Project team members</span></span>
- <span data-ttu-id="93d39-111">הערכות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="93d39-111">Project estimates</span></span>
- <span data-ttu-id="93d39-112">הערכות הוצאה בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="93d39-112">Project expense estimates</span></span>

## <a name="project-properties"></a><span data-ttu-id="93d39-113">מאפייני פרויקט</span><span class="sxs-lookup"><span data-stu-id="93d39-113">Project properties</span></span>

<span data-ttu-id="93d39-114">כאשר הפרויקט מועתק, הערכים בשדות הבאים מועתקים:</span><span class="sxs-lookup"><span data-stu-id="93d39-114">When the project is copied, the values in the following fields are copied:</span></span>

- <span data-ttu-id="93d39-115">שם</span><span class="sxs-lookup"><span data-stu-id="93d39-115">Name</span></span>
- <span data-ttu-id="93d39-116">תיאור</span><span class="sxs-lookup"><span data-stu-id="93d39-116">Description</span></span>
- <span data-ttu-id="93d39-117">לקוח</span><span class="sxs-lookup"><span data-stu-id="93d39-117">Customer</span></span>
- <span data-ttu-id="93d39-118">תבנית לוח שנה</span><span class="sxs-lookup"><span data-stu-id="93d39-118">Calendar Template</span></span>
- <span data-ttu-id="93d39-119">מטבע</span><span class="sxs-lookup"><span data-stu-id="93d39-119">Currency</span></span>
- <span data-ttu-id="93d39-120">יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="93d39-120">Contracting Unit</span></span>
- <span data-ttu-id="93d39-121">מנהל פרויקט</span><span class="sxs-lookup"><span data-stu-id="93d39-121">Project Manager</span></span>
- <span data-ttu-id="93d39-122">סטאטוס</span><span class="sxs-lookup"><span data-stu-id="93d39-122">Status</span></span>
- <span data-ttu-id="93d39-123">מצב פרויקט כולל</span><span class="sxs-lookup"><span data-stu-id="93d39-123">Overall Project Status</span></span>
- <span data-ttu-id="93d39-124">הערות </span><span class="sxs-lookup"><span data-stu-id="93d39-124">Comments</span></span>
- <span data-ttu-id="93d39-125">הערכות</span><span class="sxs-lookup"><span data-stu-id="93d39-125">Estimates</span></span>
- <span data-ttu-id="93d39-126">תאריך התחלה משוער</span><span class="sxs-lookup"><span data-stu-id="93d39-126">Estimated Start Date</span></span>
- <span data-ttu-id="93d39-127">תאריך סיום</span><span class="sxs-lookup"><span data-stu-id="93d39-127">Finish Date</span></span>
- <span data-ttu-id="93d39-128">מאמץ (בשעות)</span><span class="sxs-lookup"><span data-stu-id="93d39-128">Effort (Hours)</span></span>
- <span data-ttu-id="93d39-129">עלות עבודה משוערת</span><span class="sxs-lookup"><span data-stu-id="93d39-129">Estimated Labor Cost</span></span>
- <span data-ttu-id="93d39-130">עלות הוצאות משוערת</span><span class="sxs-lookup"><span data-stu-id="93d39-130">Estimated Expense Cost</span></span>

## <a name="work-breakdown-structure"></a><span data-ttu-id="93d39-131">מבנה התפלגות העבודה</span><span class="sxs-lookup"><span data-stu-id="93d39-131">Work breakdown structure</span></span>

<span data-ttu-id="93d39-132">כאשר הפרויקט מועתק, כל מבנה התפלגות העבודה של המשאב שנטען מועתק.</span><span class="sxs-lookup"><span data-stu-id="93d39-132">When the project is copied, the entire resource-loaded work breakdown structure is copied.</span></span> <span data-ttu-id="93d39-133">משאבים בעלי שם מוחלפים במשאבים כלליים.</span><span class="sxs-lookup"><span data-stu-id="93d39-133">Named resources are replaced with generic resources.</span></span> <span data-ttu-id="93d39-134">אם למשאבים בעלי השם אין את אותן שעות עבודה כמו למשאב הכללי, לוח הזמנים יחושב מחדש ומשך המשימות עשוי להשתנות.</span><span class="sxs-lookup"><span data-stu-id="93d39-134">If the named resources don't have the same working hours as the generic resource, the schedule will be recalculated and task durations may change.</span></span>

## <a name="project-team-members"></a><span data-ttu-id="93d39-135">חברי צוות בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="93d39-135">Project team members</span></span>

<span data-ttu-id="93d39-136">כאשר צוות פרויקט מועתק מפרויקט המקור, המשאבים הכלליים מועתקים.</span><span class="sxs-lookup"><span data-stu-id="93d39-136">When a project team is copied from the source project, the generic resources are copied.</span></span> <span data-ttu-id="93d39-137">הקצאות של המשאבים הכלליים נשארות כפי השהיו בפרוייקט המקור.</span><span class="sxs-lookup"><span data-stu-id="93d39-137">Generic resource assignments are also maintained as they were in the source project.</span></span> <span data-ttu-id="93d39-138">משאבים בעלי שם יומרו לחברי צוות כלליים.</span><span class="sxs-lookup"><span data-stu-id="93d39-138">Named resources will be converted to generic team members.</span></span>

## <a name="estimates"></a><span data-ttu-id="93d39-139">הערכות</span><span class="sxs-lookup"><span data-stu-id="93d39-139">Estimates</span></span>

<span data-ttu-id="93d39-140">כאשר מועתק הפרויקט, מעותקות גם שורות הערכת המשאבים וההוצאות מפרויקט המקור.</span><span class="sxs-lookup"><span data-stu-id="93d39-140">When the project is copied, both resource and expense estimate lines are copied from the source project.</span></span>