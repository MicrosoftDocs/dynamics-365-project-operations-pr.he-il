---
title: הזמנה לפרוייקט
description: נושא זה מספק מידע לגבי האופן שבו מבצעים הזמנה של משאב לפרויקטים.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 19128264ed3db7efeeba948155f0ddbdc806c2a0
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908195"
---
# <a name="book-to-a-project"></a><span data-ttu-id="eb535-103">הזמנה לפרוייקט</span><span class="sxs-lookup"><span data-stu-id="eb535-103">Book to a project</span></span>

<span data-ttu-id="eb535-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="eb535-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="eb535-105">ישנם מקרים בהם מנהל פרויקטים או מנהל משאבים יצטרכו להקצות משאב לפרויקט מבלי שהוגדרה דרישה ספציפית מחבר צוות כללי.</span><span class="sxs-lookup"><span data-stu-id="eb535-105">There are times where a Project manager or Resource manager will need to allocate a resource to project without a specific requirement being defined from a generic team member.</span></span> <span data-ttu-id="eb535-106">ניתן לבצע זאת באחת משלוש דרכים.</span><span class="sxs-lookup"><span data-stu-id="eb535-106">This can be achieved in one of three ways.</span></span>

- <span data-ttu-id="eb535-107">לבצע הזמנה דרך רשת חברי הצוות</span><span class="sxs-lookup"><span data-stu-id="eb535-107">Book from the team member grid</span></span>
- <span data-ttu-id="eb535-108">הזמנה מתוך לוח הזמנים</span><span class="sxs-lookup"><span data-stu-id="eb535-108">Book from the schedule board</span></span>
- <span data-ttu-id="eb535-109">לבצע הזמנה דרך הטופס **פרויקט**</span><span class="sxs-lookup"><span data-stu-id="eb535-109">Book from the **Project** form</span></span>

## <a name="book-from-the-team-member-grid"></a><span data-ttu-id="eb535-110">לבצע הזמנה דרך רשת חברי הצוות</span><span class="sxs-lookup"><span data-stu-id="eb535-110">Book from the team member grid</span></span>

<span data-ttu-id="eb535-111">אם הארגון שלך פועל במצב הקצאת משאבים היברידית, מנהל הפרויקט יכול להזמין משאב ישירות לפרויקט על ידי השלמת השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="eb535-111">If your organization is operating in hybrid Resource allocation mode, the Project manager can book a resource directly to the project by completing the following steps.</span></span>

1. <span data-ttu-id="eb535-112">מהפרויקט, עבור לרשת חברי הצוות ובחר **חדשׁ**.</span><span class="sxs-lookup"><span data-stu-id="eb535-112">From the project, go to the team member grid and select **New**.</span></span>
2. <span data-ttu-id="eb535-113">הגדר את שם העמדה והתפקיד של המשאב.</span><span class="sxs-lookup"><span data-stu-id="eb535-113">Define the position name and the role of the resource.</span></span>
3. <span data-ttu-id="eb535-114">בחר את המשאב שניתן להזמין מתוך בדיקת המידע הזמין.</span><span class="sxs-lookup"><span data-stu-id="eb535-114">Select the bookable resource from the available lookup.</span></span>
4. <span data-ttu-id="eb535-115">לאחר בחירת המשאב, הגדר את פרטי השדה הבאים להזמנת המשאב:</span><span class="sxs-lookup"><span data-stu-id="eb535-115">After you select the resource, define the following field information to book the resource:</span></span>

    - <span data-ttu-id="eb535-116">תאריך התחלה</span><span class="sxs-lookup"><span data-stu-id="eb535-116">Start date</span></span>
    - <span data-ttu-id="eb535-117">תאריך סיום</span><span class="sxs-lookup"><span data-stu-id="eb535-117">Finish date</span></span>
    - <span data-ttu-id="eb535-118">שיטת הקצאה</span><span class="sxs-lookup"><span data-stu-id="eb535-118">Allocation method</span></span>
    - <span data-ttu-id="eb535-119">שעות, אם רלוונטי</span><span class="sxs-lookup"><span data-stu-id="eb535-119">Hours, if applicable</span></span>
    - <span data-ttu-id="eb535-120">מאשר הפרויקט</span><span class="sxs-lookup"><span data-stu-id="eb535-120">Project approver</span></span>

6. <span data-ttu-id="eb535-121">בחר **שמור וסגור**</span><span class="sxs-lookup"><span data-stu-id="eb535-121">Select **Save and Close**</span></span>

## <a name="book-from-the-schedule-board"></a><span data-ttu-id="eb535-122">הזמנה מתוך לוח הזמנים</span><span class="sxs-lookup"><span data-stu-id="eb535-122">Book from the schedule board</span></span>

<span data-ttu-id="eb535-123">כאשר מנהל משאבים צריך להזמין משאב ישירות לפרויקט, הוא יכול להשתמש בלוח הזמנים ובדרישת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="eb535-123">When a Resource manager needs to book a resource directly to a project, they can use the schedule board and the project requirement.</span></span> <span data-ttu-id="eb535-124">דרישת הפרויקט היא דרישת משאבים שתמיד ניתן להזמין כנגדה.</span><span class="sxs-lookup"><span data-stu-id="eb535-124">The project requirement is a resource requirement that is always available to be booked against.</span></span> <span data-ttu-id="eb535-125">בצע את השלבים הבאים כדי להזמין ישירות לפרויקט מלוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="eb535-125">To book directly to a project form the schedule board, complete the following steps.</span></span>

1. <span data-ttu-id="eb535-126">נווט ללוח הזמנים ובעמוד הימני, סנן את המשאבים אותם אתה שוקל עובר הדרישה.</span><span class="sxs-lookup"><span data-stu-id="eb535-126">Navigate to the schedule board and on the left page, filter for the resources you are considering for the requirement.</span></span>
2. <span data-ttu-id="eb535-127">בחלונית התחתונה בחר את הכרטיסיה **פרויקט** כדי להציג את רשימת דרישות הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="eb535-127">In the bottom pane, select the **Project** tab to view a list of project requirements.</span></span>
3. <span data-ttu-id="eb535-128">גרור את הדרישה אל משאב והגדר את המידע הבא:</span><span class="sxs-lookup"><span data-stu-id="eb535-128">Drag the requirement onto a resource and define the following information:</span></span>

    - <span data-ttu-id="eb535-129">תאריך התחלה</span><span class="sxs-lookup"><span data-stu-id="eb535-129">Start date</span></span>
    - <span data-ttu-id="eb535-130">תאריך סיום</span><span class="sxs-lookup"><span data-stu-id="eb535-130">Finish date</span></span>
    - <span data-ttu-id="eb535-131">מצב הזמנה</span><span class="sxs-lookup"><span data-stu-id="eb535-131">Booking status</span></span>
    - <span data-ttu-id="eb535-132">שיטת הזמנה</span><span class="sxs-lookup"><span data-stu-id="eb535-132">Booking method</span></span>
    - <span data-ttu-id="eb535-133">משך הזמן</span><span class="sxs-lookup"><span data-stu-id="eb535-133">Duration</span></span>

## <a name="book-from-the-project-form"></a><span data-ttu-id="eb535-134">ביצוע הזמנה דרך הטופס הפרויקט</span><span class="sxs-lookup"><span data-stu-id="eb535-134">Book from the Project form</span></span>

<span data-ttu-id="eb535-135">כמנהל פרויקט, ייתכן שתצטרך להזמין משאב לפרויקט, אך יודע רק את הקריטריונים ולא את שם המשאב.</span><span class="sxs-lookup"><span data-stu-id="eb535-135">As a Project manager, you might need to book a resource to a project, but only know the criteria rather than the name of the resource.</span></span> <span data-ttu-id="eb535-136">בצע את השלבים הבאים כדי להשתמש במסייע לוח הזמנים כדי למצוא משאב על סמך תכונות זמינות של המשאב.</span><span class="sxs-lookup"><span data-stu-id="eb535-136">Complete the following steps to use the schedule assistant to find a resource based on any available attributes of the resource.</span></span> 

1. <span data-ttu-id="eb535-137">נווט לפרויקט ובחר **הזמן** כדי לפתוח את 'מסייע לוח הזמנים'.</span><span class="sxs-lookup"><span data-stu-id="eb535-137">Navigate to the project and select **Book** to open the Schedule Assistant.</span></span>
2. <span data-ttu-id="eb535-138">בעזרת המסננים שבצד ימין של 'מסייע לוח הזמנים', צמצם את הקריטריונים ובחר **חיפוש.**</span><span class="sxs-lookup"><span data-stu-id="eb535-138">Using the filters on the left side of the Schedule Assistant, narrow the criteria and select **Search.**</span></span>
3. <span data-ttu-id="eb535-139">בהתבסס על משאבים שהוחזרו בתוצאות, ניתן להזמין משאב.</span><span class="sxs-lookup"><span data-stu-id="eb535-139">Based on resources returned in the results, you can book a resource.</span></span>

> [!NOTE]
> <span data-ttu-id="eb535-140">שיטה זו אינה יוצרת הזמנות עבור המשאב.</span><span class="sxs-lookup"><span data-stu-id="eb535-140">This method doesn't create any bookings for the resource.</span></span> <span data-ttu-id="eb535-141">במקום זאת, היא מוסיפה את משאב לצוות הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="eb535-141">Instead, it adds the resource to the team.</span></span> <span data-ttu-id="eb535-142">לאחר שחבר הצוות נוסף לפרויקט, מנהל הפרויקט יכול להשתמש באפשרויות 'השאר הזמנות' או 'הארכת הזמנות' כדי להוסיף את ההזמנות הנדרשות למשאב.</span><span class="sxs-lookup"><span data-stu-id="eb535-142">After the team member has been added to the project, the project manager can use maintain bookings or extend bookings to add the required bookings to the resource.</span></span>
