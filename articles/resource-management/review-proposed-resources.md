---
title: סקירת משאבים מוצעים
description: נושא זה מספק מידע לגבי האופן שבו מציעים משאבי פרויקטים.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: ad5cbdeb5fe05e6115eb024833a8d58b626ea4c9
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077275"
---
# <a name="review-proposed-resources"></a><span data-ttu-id="de63d-103">סקירת משאבים מוצעים</span><span class="sxs-lookup"><span data-stu-id="de63d-103">Review proposed resources</span></span>

<span data-ttu-id="de63d-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="de63d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="de63d-105">מנהלי משאבים יכולים להציע משאב למנהל הפרויקט באמצעות בקשת משאב.</span><span class="sxs-lookup"><span data-stu-id="de63d-105">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="de63d-106">מרשת הבקשה או מהבקשה עצמה, בחר **חפש משאבים**.</span><span class="sxs-lookup"><span data-stu-id="de63d-106">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="de63d-107">בדף **מסייע לוח הזמנים‬** , בחר את המשאב ולאחר מכן בחלונית **צור הזמנת משאבים** , בשדה **מצב הזמנה** , בחר **הזמן**.</span><span class="sxs-lookup"><span data-stu-id="de63d-107">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

<span data-ttu-id="de63d-108">עדכוני המצב הבאים מתרחשים:</span><span class="sxs-lookup"><span data-stu-id="de63d-108">The following status updates occur:</span></span>

- <span data-ttu-id="de63d-109">בדף **מסייע לוח הזמנים** , מחווני המצב מתעדכנים כדי לציין שההזמנה היא הזמנה מוצעת, לא הזמנה בטוחה.</span><span class="sxs-lookup"><span data-stu-id="de63d-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>
- <span data-ttu-id="de63d-110">בבקשת המשאב, המצב משתנה ל **‏‫נחוצה סקירה‬**.</span><span class="sxs-lookup"><span data-stu-id="de63d-110">On the resource request, the status is changed to **Needs Review**.</span></span>
- <span data-ttu-id="de63d-111">בכרטיסיה **צוות** של הפרויקט, הערך **מצב בקשה** של חבר הצוות הכללי משתנה ל **‏‫נחוצה סקירה‬**.</span><span class="sxs-lookup"><span data-stu-id="de63d-111">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

<span data-ttu-id="de63d-112">מנהל הפרויקט יכול לקבל או לדחות את ההצעה.</span><span class="sxs-lookup"><span data-stu-id="de63d-112">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="de63d-113">כאשר מנהלי משאבים מעבדים בקשות משאבים, הם יכולים להשתמש באחת מהגישות הבאות:</span><span class="sxs-lookup"><span data-stu-id="de63d-113">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="de63d-114">הצעת משאבים מרובים כדי לספק את הביקוש אם אין אפילו משאב אחד למימוש השעות הנדרשות.</span><span class="sxs-lookup"><span data-stu-id="de63d-114">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="de63d-115">כעת השעות המוצעות מתחלקות בין משאבים מרובים שיכולים לספק את השעות הנדרשות.</span><span class="sxs-lookup"><span data-stu-id="de63d-115">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="de63d-116">בתרחיש זה, השעות אינן יכולות להיות חופפות.</span><span class="sxs-lookup"><span data-stu-id="de63d-116">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="de63d-117">הצעת פחות משאבים מן הנדרש.</span><span class="sxs-lookup"><span data-stu-id="de63d-117">Propose fewer resources than are required.</span></span> <span data-ttu-id="de63d-118">בתרחיש זה, קיבולת המשאב המוצע נמוכה מהשעות הדרושות שהמבקש ציין.</span><span class="sxs-lookup"><span data-stu-id="de63d-118">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="de63d-119">לכן, כאשר המבקש מקבל את המשאבים המוצעים, נוצרת דרישה למשאב שלא התמלא כדי ללכוד את הביקוש הנותר.</span><span class="sxs-lookup"><span data-stu-id="de63d-119">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="de63d-120">הזמנת משאבים מרובים כדי לספק את הביקוש אם אין אפילו משאב אחד להשלמת העבודה.</span><span class="sxs-lookup"><span data-stu-id="de63d-120">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="de63d-121">הזמנת פחות משאבים מן הנדרש.</span><span class="sxs-lookup"><span data-stu-id="de63d-121">Book fewer resources than are required.</span></span> <span data-ttu-id="de63d-122">בתרחיש זה, מספר השעות שהוזמנו קטן יותר מן השעות הנדרשות.</span><span class="sxs-lookup"><span data-stu-id="de63d-122">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="de63d-123">המערכת מנחה אותך להציע משאבים במקום הזמנות, כדי שהמבקש יוכל לאמת ולעקוב אחר הביקוש הנותר.</span><span class="sxs-lookup"><span data-stu-id="de63d-123">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="billable-utilization"></a><span data-ttu-id="de63d-124">ניצול לחיוב</span><span class="sxs-lookup"><span data-stu-id="de63d-124">Billable utilization</span></span>

<span data-ttu-id="de63d-125">המשאבים יכולים לכלול ניצול יעד לחיוב.</span><span class="sxs-lookup"><span data-stu-id="de63d-125">Resources can have a target billable utilization.</span></span> <span data-ttu-id="de63d-126">ניצול יעד זה מוגדר כתכונה בתפקיד ברירת מחדל של משאב או מוגדר ברשומה של המשאב היחיד הניתן להזמנה.</span><span class="sxs-lookup"><span data-stu-id="de63d-126">This target utilization is either defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="de63d-127">חישובי ניצול מבוססים על השעות בפועל שדיווחו המשאבים באמצעות ערכי זמן שאושרו.</span><span class="sxs-lookup"><span data-stu-id="de63d-127">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="de63d-128">הנוסחאות הבאות משמשות לחישוב הניצול:</span><span class="sxs-lookup"><span data-stu-id="de63d-128">The following formulas are used to calculate utilization:</span></span>

- <span data-ttu-id="de63d-129">ניצול לחיוב = שעות בפועל הניתנות לחיוב ÷ קיבולת משאב</span><span class="sxs-lookup"><span data-stu-id="de63d-129">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
- <span data-ttu-id="de63d-130">ניצול שאינו לחיוב = זמן בפועל עם מזהה סוג חיוב = 'אינו לחיוב', 'משלים' או 'לא זמין' ÷ קיבולת משאב</span><span class="sxs-lookup"><span data-stu-id="de63d-130">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
- <span data-ttu-id="de63d-131">פנימי = זמן בפועל ללא חוזה מכירות ÷ קיבולת משאב</span><span class="sxs-lookup"><span data-stu-id="de63d-131">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
- <span data-ttu-id="de63d-132">קיבולת משאב = שעות עבודה של משאב – מחוץ למשרד – ימים שאינם ימי עבודה</span><span class="sxs-lookup"><span data-stu-id="de63d-132">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="de63d-133">ניתן למצוא את התצוגה **ניצול משאב** בחלונית **משאבים**.</span><span class="sxs-lookup"><span data-stu-id="de63d-133">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

<span data-ttu-id="de63d-134">כל תא ברשת מייצג את אחוז הניצול לחיוב של המשאב בתקופה, כגון יום, שבוע או חודש.</span><span class="sxs-lookup"><span data-stu-id="de63d-134">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="de63d-135">הנוסחאות הבאות משמשות לצביעת התאים:</span><span class="sxs-lookup"><span data-stu-id="de63d-135">The following formulas are used to color the cells:</span></span>

- <span data-ttu-id="de63d-136">**ירוק:** ניצול לחיוב \>= ניצול יעד של משאב</span><span class="sxs-lookup"><span data-stu-id="de63d-136">**Green:** Billable utilization \>= Resource target utilization</span></span>
- <span data-ttu-id="de63d-137">**צהוב:** יעד ניצול – 20 \<= ניצול לחיוב \< יעד ניצול</span><span class="sxs-lookup"><span data-stu-id="de63d-137">**Yellow:** Target utilization – 20 \<= Billable utilization \< Target utilization</span></span>
- <span data-ttu-id="de63d-138">**אדום:** ניצול לחיוב \< יעד ניצול – 20</span><span class="sxs-lookup"><span data-stu-id="de63d-138">**Red:** Billable utilization \< Target utilization – 20</span></span>

<span data-ttu-id="de63d-139">מכיוון שהתצוגה **ניצול משאבים** מבוססת על לוח הזמנים, ניתן להשתמש ביכולות הסינון של לוח הזמנים כדי לסנן את התוצאות.</span><span class="sxs-lookup"><span data-stu-id="de63d-139">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="de63d-140">הרשת מחייבת הגדרה של ניצול יעד בתפקיד או במשאב הבודד.</span><span class="sxs-lookup"><span data-stu-id="de63d-140">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="de63d-141">לצורך ביצוע ההגדרה, עבור אל **משאבים** \> **תפקידי משאבים**.</span><span class="sxs-lookup"><span data-stu-id="de63d-141">To do this setup, go to **Resources** \> **Resource roles**.</span></span>

<span data-ttu-id="de63d-142">בנוסף, יש להקצות תפקיד ברירת מחדל לכל משאב הניתן להזמנה.</span><span class="sxs-lookup"><span data-stu-id="de63d-142">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="de63d-143">עבור אל **משאבים** \> **משאבים**.</span><span class="sxs-lookup"><span data-stu-id="de63d-143">Go to **Resources** \> **Resources**.</span></span> <span data-ttu-id="de63d-144">בכרטיסיה **Project Service** , הקפד להגדיר תפקיד משאב וודא שהשדה **מהווה ברירת מחדל** עבורו מוגדר ל **כן**.</span><span class="sxs-lookup"><span data-stu-id="de63d-144">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field for it is set to **Yes**.</span></span> <span data-ttu-id="de63d-145">ניתן להוסיף תפקידים נוספים כאשר **מהווה ברירת מחדל = לא**.</span><span class="sxs-lookup"><span data-stu-id="de63d-145">You can add additional roles where **Is Default = No**.</span></span> <span data-ttu-id="de63d-146">התפקיד שבו **מהווה ברירת מחדל = כן** משמש להערכה של ניצול המשאב כנגד היעד עבור אותו תפקיד.</span><span class="sxs-lookup"><span data-stu-id="de63d-146">The role where the **Is Default = Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

<span data-ttu-id="de63d-147">בכרטיסיה **Project Service** , ניתן גם להגדיר ניצול יעד בודד עבור המשאב.</span><span class="sxs-lookup"><span data-stu-id="de63d-147">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="de63d-148">כעת, חישוב הניצול משתמש בניצול היעד כדי להעריך את היעד של המשאב במקום את היעד של תפקיד ברירת המחדל של המשאב.</span><span class="sxs-lookup"><span data-stu-id="de63d-148">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="de63d-149">הניצול מוצג עבור משאב רק אם משאב זה אישר זמן הניתן לחיוב במהלך התקופה המופיעה ברשת.</span><span class="sxs-lookup"><span data-stu-id="de63d-149">Utilization is shown for a resource only if that resource has approved, chargeable time during the period that is shown in the grid.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="de63d-150">זמינות משאב</span><span class="sxs-lookup"><span data-stu-id="de63d-150">Resource availability</span></span>

<span data-ttu-id="de63d-151">חשוב שמנהלי משאבים יוכלו להציג זמינות של משאבים ולעדכן הזמנות.</span><span class="sxs-lookup"><span data-stu-id="de63d-151">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="de63d-152">במקרים מסוימים, אין ביקוש רשמי (בקשת משאב), אך מנהל משאבים חייב להגיב לביקוש לא מתוכנן שמגיע דרך ערוצים כגון דואר, שיחת טלפון או הודעה מיידית.</span><span class="sxs-lookup"><span data-stu-id="de63d-152">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="de63d-153">מנהלי משאבים משתמשים בלוח הזמנים כדי לעדכן משאבים והזמנות.</span><span class="sxs-lookup"><span data-stu-id="de63d-153">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="de63d-154">שעות עבודה של משאב משמשות כבסיס לחישוב הזמינות של משאב.</span><span class="sxs-lookup"><span data-stu-id="de63d-154">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="de63d-155">הזמנות של משאבים צורכות את הקיבולת של המשאבים.</span><span class="sxs-lookup"><span data-stu-id="de63d-155">Resource bookings consume the capacity of the resources.</span></span>

<span data-ttu-id="de63d-156">לוח הזמנים משתמש בצבעים ובהצללה כדי להציג הזמנות, זמינות והזמנות יתר וכן את מצב ההזמנות.</span><span class="sxs-lookup"><span data-stu-id="de63d-156">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="de63d-157">הגדרה בהגדרות לוח הזמנים מאפשרת לך להציג מקרא.</span><span class="sxs-lookup"><span data-stu-id="de63d-157">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="de63d-158">אם מופיע חץ המצביע ימינה ליד משאב בודד הניתן להזמנה בלוח הזמנים, ניתן להרחיב את המשאב כך שיציג פרטים של העבודה שהמשאב הוזמן עבורה.</span><span class="sxs-lookup"><span data-stu-id="de63d-158">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

<span data-ttu-id="de63d-159">מכיוון ש- Dynamics 365 Project Operations משתמש במנגנון Universal Resource Scheduling, אם במחשב שלך מותקן גם Dynamics 365 Field Service, תוכל להציג את פרטי הזמנות המשאבים עבור פרויקטים, הזמנות עבודה וכל ישות אחרת שהארכת את התזמון שלה.</span><span class="sxs-lookup"><span data-stu-id="de63d-159">Because Dynamics 365 Project Operations uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

<span data-ttu-id="de63d-160">כדי להציג פרטים נוספים אודות משאב בודד, לחץ עליו באמצעות לחצן העכבר הימני כדי לפתוח את כרטיס המשאב.</span><span class="sxs-lookup"><span data-stu-id="de63d-160">To view more details about an individual resource, right-click it to open the resource card.</span></span>

