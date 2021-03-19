---
title: סקירת משאבים מוצעים
description: נושא זה מספק מידע לגבי האופן שבו מציעים משאבי פרויקטים.
author: ruhercul
manager: AnnBe
ms.date: 11/05/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: fa0515b9d6a0023c05c37d2bcfa6a403f48927cb
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279274"
---
# <a name="review-proposed-resources"></a><span data-ttu-id="ba199-103">סקירת משאבים מוצעים</span><span class="sxs-lookup"><span data-stu-id="ba199-103">Review proposed resources</span></span>

<span data-ttu-id="ba199-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="ba199-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ba199-105">מנהלי משאבים יכולים להציע משאב למנהל הפרויקט באמצעות בקשת משאב.</span><span class="sxs-lookup"><span data-stu-id="ba199-105">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="ba199-106">מרשת הבקשה או מהבקשה עצמה, בחר **חפש משאבים**.</span><span class="sxs-lookup"><span data-stu-id="ba199-106">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="ba199-107">בדף **מסייע לוח הזמנים‬**, בחר את המשאב ולאחר מכן בחלונית **צור הזמנת משאבים**, בשדה **מצב הזמנה**, בחר **הזמן**.</span><span class="sxs-lookup"><span data-stu-id="ba199-107">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

<span data-ttu-id="ba199-108">עדכוני המצב הבאים מתרחשים:</span><span class="sxs-lookup"><span data-stu-id="ba199-108">The following status updates occur:</span></span>

- <span data-ttu-id="ba199-109">בדף **מסייע לוח הזמנים**, מחווני המצב מתעדכנים כדי לציין שההזמנה היא הזמנה מוצעת, לא הזמנה בטוחה.</span><span class="sxs-lookup"><span data-stu-id="ba199-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>
- <span data-ttu-id="ba199-110">בבקשת המשאב, המצב משתנה ל **‏‫נחוצה סקירה‬**.</span><span class="sxs-lookup"><span data-stu-id="ba199-110">On the resource request, the status is changed to **Needs Review**.</span></span>
- <span data-ttu-id="ba199-111">בכרטיסיה **צוות** של הפרויקט, הערך **מצב בקשה** של חבר הצוות הכללי משתנה ל **‏‫נחוצה סקירה‬**.</span><span class="sxs-lookup"><span data-stu-id="ba199-111">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

<span data-ttu-id="ba199-112">מנהל הפרויקט יכול לקבל או לדחות את ההצעה.</span><span class="sxs-lookup"><span data-stu-id="ba199-112">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="ba199-113">כאשר מנהלי משאבים מעבדים בקשות משאבים, הם יכולים להשתמש באחת מהגישות הבאות:</span><span class="sxs-lookup"><span data-stu-id="ba199-113">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="ba199-114">הצעת משאבים מרובים כדי לספק את הביקוש אם אין אפילו משאב אחד למימוש השעות הנדרשות.</span><span class="sxs-lookup"><span data-stu-id="ba199-114">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="ba199-115">כעת השעות המוצעות מתחלקות בין משאבים מרובים שיכולים לספק את השעות הנדרשות.</span><span class="sxs-lookup"><span data-stu-id="ba199-115">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="ba199-116">בתרחיש זה, השעות אינן יכולות להיות חופפות.</span><span class="sxs-lookup"><span data-stu-id="ba199-116">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="ba199-117">הצעת פחות משאבים מן הנדרש.</span><span class="sxs-lookup"><span data-stu-id="ba199-117">Propose fewer resources than are required.</span></span> <span data-ttu-id="ba199-118">בתרחיש זה, קיבולת המשאב המוצע נמוכה מהשעות הדרושות שהמבקש ציין.</span><span class="sxs-lookup"><span data-stu-id="ba199-118">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="ba199-119">לכן, כאשר המבקש מקבל את המשאבים המוצעים, נוצרת דרישה למשאב שלא התמלא כדי ללכוד את הביקוש הנותר.</span><span class="sxs-lookup"><span data-stu-id="ba199-119">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="ba199-120">הזמנת משאבים מרובים כדי לספק את הביקוש אם אין אפילו משאב אחד להשלמת העבודה.</span><span class="sxs-lookup"><span data-stu-id="ba199-120">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="ba199-121">הזמנת פחות משאבים מן הנדרש.</span><span class="sxs-lookup"><span data-stu-id="ba199-121">Book fewer resources than are required.</span></span> <span data-ttu-id="ba199-122">בתרחיש זה, מספר השעות שהוזמנו קטן יותר מן השעות הנדרשות.</span><span class="sxs-lookup"><span data-stu-id="ba199-122">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="ba199-123">המערכת מנחה אותך להציע משאבים במקום הזמנות, כדי שהמבקש יוכל לאמת ולעקוב אחר הביקוש הנותר.</span><span class="sxs-lookup"><span data-stu-id="ba199-123">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="ba199-124">זמינות משאב</span><span class="sxs-lookup"><span data-stu-id="ba199-124">Resource availability</span></span>

<span data-ttu-id="ba199-125">חשוב שמנהלי משאבים יוכלו להציג זמינות של משאבים ולעדכן הזמנות.</span><span class="sxs-lookup"><span data-stu-id="ba199-125">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="ba199-126">במקרים מסוימים, אין ביקוש רשמי (בקשת משאב), אך מנהל משאבים חייב להגיב לביקוש לא מתוכנן שמגיע דרך ערוצים כגון דואר, שיחת טלפון או הודעה מיידית.</span><span class="sxs-lookup"><span data-stu-id="ba199-126">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="ba199-127">מנהלי משאבים משתמשים בלוח הזמנים כדי לעדכן משאבים והזמנות.</span><span class="sxs-lookup"><span data-stu-id="ba199-127">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="ba199-128">שעות עבודה של משאב משמשות כבסיס לחישוב הזמינות של משאב.</span><span class="sxs-lookup"><span data-stu-id="ba199-128">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="ba199-129">הזמנות של משאבים צורכות את הקיבולת של המשאבים.</span><span class="sxs-lookup"><span data-stu-id="ba199-129">Resource bookings consume the capacity of the resources.</span></span>

<span data-ttu-id="ba199-130">לוח הזמנים משתמש בצבעים ובהצללה כדי להציג הזמנות, זמינות והזמנות יתר וכן את מצב ההזמנות.</span><span class="sxs-lookup"><span data-stu-id="ba199-130">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="ba199-131">הגדרה בהגדרות לוח הזמנים מאפשרת לך להציג מקרא.</span><span class="sxs-lookup"><span data-stu-id="ba199-131">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="ba199-132">אם מופיע חץ המצביע ימינה ליד משאב בודד הניתן להזמנה בלוח הזמנים, ניתן להרחיב את המשאב כך שיציג פרטים של העבודה שהמשאב הוזמן עבורה.</span><span class="sxs-lookup"><span data-stu-id="ba199-132">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

<span data-ttu-id="ba199-133">מכיוון ש- Dynamics 365 Project Operations משתמש במנגנון Universal Resource Scheduling, אם במחשב שלך מותקן גם Dynamics 365 Field Service, תוכל להציג את פרטי הזמנות המשאבים עבור פרויקטים, הזמנות עבודה וכל ישות אחרת שהארכת את התזמון שלה.</span><span class="sxs-lookup"><span data-stu-id="ba199-133">Because Dynamics 365 Project Operations uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

<span data-ttu-id="ba199-134">כדי להציג פרטים נוספים אודות משאב בודד, לחץ עליו באמצעות לחצן העכבר הימני כדי לפתוח את כרטיס המשאב.</span><span class="sxs-lookup"><span data-stu-id="ba199-134">To view more details about an individual resource, right-click it to open the resource card.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]