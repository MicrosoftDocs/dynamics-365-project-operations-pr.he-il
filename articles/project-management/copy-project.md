---
title: העתקת פרוייקט
description: נושא זו מספק מידע על העתקת פרויקטים ב- Dynamics 365 Project Operations.
author: ruhercul
ms.date: 05/21/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: c3055ab5b8c07faa2bc9167956d283e2a66029dd
ms.sourcegitcommit: 173f2b1f4e063c440a5f78d76d456c62aadbd89e
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/24/2021
ms.locfileid: "6091255"
---
# <a name="copy-a-project"></a><span data-ttu-id="845b8-103">העתקת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="845b8-103">Copy a project</span></span>

<span data-ttu-id="845b8-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="845b8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="845b8-105">עם Dynamics 365 Project Operations אפשר לבנות במהירות פרויקטים חדשים על ידי בחירה באפשרות **העתק פרויקט** בטופס **פרויקטים** .</span><span class="sxs-lookup"><span data-stu-id="845b8-105">With Dynamics 365 Project Operations, you can quickly build new projects by selecting **Copy Project** on the **Projects** form.</span></span> <span data-ttu-id="845b8-106">להעתקת פרויקט, פתח את הפרויקט שברצונך להעתיק ואז בחר **העתק פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="845b8-106">To copy a project, open the project you want to copy, and then select **Copy project**.</span></span> <span data-ttu-id="845b8-107">הפעולה תעתיק את הפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="845b8-107">The action will copy the following:</span></span>

- <span data-ttu-id="845b8-108">מאפייני פרויקט</span><span class="sxs-lookup"><span data-stu-id="845b8-108">Project properties</span></span> 
- <span data-ttu-id="845b8-109">מבנה התפלגות העבודה</span><span class="sxs-lookup"><span data-stu-id="845b8-109">Work breakdown structure</span></span>
- <span data-ttu-id="845b8-110">חברי צוות בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="845b8-110">Project team members</span></span>
- <span data-ttu-id="845b8-111">הערכות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="845b8-111">Project estimates</span></span>
- <span data-ttu-id="845b8-112">הערכות הוצאה בפרויקט</span><span class="sxs-lookup"><span data-stu-id="845b8-112">Project expense estimates</span></span>
- <span data-ttu-id="845b8-113">הערכות חומרים בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="845b8-113">Project material estimates</span></span>

## <a name="project-properties"></a><span data-ttu-id="845b8-114">מאפייני פרויקט</span><span class="sxs-lookup"><span data-stu-id="845b8-114">Project properties</span></span>

<span data-ttu-id="845b8-115">כאשר הפרויקט מועתק, הערכים בשדות הבאים מועתקים:</span><span class="sxs-lookup"><span data-stu-id="845b8-115">When the project is copied, the values in the following fields are copied:</span></span>

- <span data-ttu-id="845b8-116">שם</span><span class="sxs-lookup"><span data-stu-id="845b8-116">Name</span></span>
- <span data-ttu-id="845b8-117">תיאור</span><span class="sxs-lookup"><span data-stu-id="845b8-117">Description</span></span>
- <span data-ttu-id="845b8-118">לקוח</span><span class="sxs-lookup"><span data-stu-id="845b8-118">Customer</span></span>
- <span data-ttu-id="845b8-119">תבנית לוח שנה</span><span class="sxs-lookup"><span data-stu-id="845b8-119">Calendar Template</span></span>
- <span data-ttu-id="845b8-120">מטבע</span><span class="sxs-lookup"><span data-stu-id="845b8-120">Currency</span></span>
- <span data-ttu-id="845b8-121">יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="845b8-121">Contracting Unit</span></span>
- <span data-ttu-id="845b8-122">מנהל פרויקט</span><span class="sxs-lookup"><span data-stu-id="845b8-122">Project Manager</span></span>
- <span data-ttu-id="845b8-123">סטאטוס</span><span class="sxs-lookup"><span data-stu-id="845b8-123">Status</span></span>
- <span data-ttu-id="845b8-124">מצב פרוייקט כולל</span><span class="sxs-lookup"><span data-stu-id="845b8-124">Overall Project Status</span></span>
- <span data-ttu-id="845b8-125">הערות </span><span class="sxs-lookup"><span data-stu-id="845b8-125">Comments</span></span>
- <span data-ttu-id="845b8-126">הערכות</span><span class="sxs-lookup"><span data-stu-id="845b8-126">Estimates</span></span>
- <span data-ttu-id="845b8-127">תאריך התחלה משוער: זהו התאריך שבו הפרוייקט נוצר מהעותק.</span><span class="sxs-lookup"><span data-stu-id="845b8-127">Estimated Start Date: This is the date that the project is created from the copy.</span></span>
- <span data-ttu-id="845b8-128">תאריך סיום משוער: תאריך זה מותאם לפי תאריך ההתחלה של הפרוייקט החדש שנוצר מהעותק.</span><span class="sxs-lookup"><span data-stu-id="845b8-128">Estimated Finish Date: This date is adjusted based on the start date of the new project that was made from the copy.</span></span>
- <span data-ttu-id="845b8-129">מאמץ (בשעות)</span><span class="sxs-lookup"><span data-stu-id="845b8-129">Effort (Hours)</span></span>
- <span data-ttu-id="845b8-130">עלות עבודה משוערת</span><span class="sxs-lookup"><span data-stu-id="845b8-130">Estimated Labor Cost</span></span>
- <span data-ttu-id="845b8-131">עלות הוצאות משוערת</span><span class="sxs-lookup"><span data-stu-id="845b8-131">Estimated Expense Cost</span></span>
- <span data-ttu-id="845b8-132">עלות חומרים משוערת</span><span class="sxs-lookup"><span data-stu-id="845b8-132">Estimated Material Cost</span></span>

> [!NOTE]
> <span data-ttu-id="845b8-133">העתקת פרוייקט יכולה להיות פעולה ארוכת טווח.</span><span class="sxs-lookup"><span data-stu-id="845b8-133">Copy project is a long running operation.</span></span> <span data-ttu-id="845b8-134">מועתקים גם רשומות הפרוייקט, המאפיינים הרלוונטיים שלו וישויות קשורות רבות.</span><span class="sxs-lookup"><span data-stu-id="845b8-134">Project records, their relevant attributes, and many related entities are also copied.</span></span> <span data-ttu-id="845b8-135">בגלל אופי הפעולה הארוכה, לאחר תחילת ההעתקה, דף פרוייקט היעד נעול לעריכה עד להשלמת פעולת ההעתקה.</span><span class="sxs-lookup"><span data-stu-id="845b8-135">Because of the long running nature of the operation, after the copy starts, the target project page is locked for editing until the copy operation is complete.</span></span>

## <a name="work-breakdown-structure"></a><span data-ttu-id="845b8-136">מבנה התפלגות העבודה</span><span class="sxs-lookup"><span data-stu-id="845b8-136">Work breakdown structure</span></span>

<span data-ttu-id="845b8-137">כאשר הפרויקט מועתק, כל מבנה התפלגות העבודה של המשאב שנטען מועתק.</span><span class="sxs-lookup"><span data-stu-id="845b8-137">When the project is copied, the entire resource-loaded work breakdown structure is copied.</span></span> <span data-ttu-id="845b8-138">משאבים בעלי שם מוחלפים במשאבים כלליים.</span><span class="sxs-lookup"><span data-stu-id="845b8-138">Named resources are replaced with generic resources.</span></span> <span data-ttu-id="845b8-139">אם למשאבים בעלי השם אין את אותן שעות עבודה כמו למשאב הכללי, לוח הזמנים יחושב מחדש ומשך המשימות עשוי להשתנות.</span><span class="sxs-lookup"><span data-stu-id="845b8-139">If the named resources don't have the same working hours as the generic resource, the schedule will be recalculated and task durations may change.</span></span>

## <a name="project-team-members"></a><span data-ttu-id="845b8-140">חברי צוות בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="845b8-140">Project team members</span></span>

<span data-ttu-id="845b8-141">כאשר צוות פרויקט מועתק מפרויקט המקור, המשאבים הכלליים מועתקים.</span><span class="sxs-lookup"><span data-stu-id="845b8-141">When a project team is copied from the source project, the generic resources are copied.</span></span> <span data-ttu-id="845b8-142">הקצאות של המשאבים הכלליים נשארות כפי השהיו בפרוייקט המקור.</span><span class="sxs-lookup"><span data-stu-id="845b8-142">Generic resource assignments are also maintained as they were in the source project.</span></span> <span data-ttu-id="845b8-143">משאבים בעלי שם יומרו לחברי צוות כלליים.</span><span class="sxs-lookup"><span data-stu-id="845b8-143">Named resources will be converted to generic team members.</span></span>

## <a name="estimates"></a><span data-ttu-id="845b8-144">הערכות</span><span class="sxs-lookup"><span data-stu-id="845b8-144">Estimates</span></span>

<span data-ttu-id="845b8-145">כאשר מועתק הפרוייקט, מועתקים שורות המשאבים, ההוצאות והערכות החומר מפרוייקט המקור.</span><span class="sxs-lookup"><span data-stu-id="845b8-145">When the project is copied, resource, expense and material estimate lines are copied from the source project.</span></span> 

<span data-ttu-id="845b8-146">למידע על אופן הגישה הפרוגרמטית אל 'העתק פוריקט', ראה [פיתוח תבניות פרוייקט באמצעות 'העתקת פוריקט'](dev-copy-project.md).</span><span class="sxs-lookup"><span data-stu-id="845b8-146">For information on how to programmatically access Copy Project, see [Develop project templates with Copy Project](dev-copy-project.md).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
