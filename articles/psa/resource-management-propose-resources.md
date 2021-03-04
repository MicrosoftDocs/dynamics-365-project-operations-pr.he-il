---
title: הצע משאבי פרויקט
description: נושא זה מספק מידע לגבי הצעה של משאבי פרויקטים.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 0a3eaa9929770c91523831d92744d5084aa28cb8
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147519"
---
# <a name="propose-project-resources"></a><span data-ttu-id="6ea5d-103">הצע משאבי פרויקט</span><span class="sxs-lookup"><span data-stu-id="6ea5d-103">Propose project resources</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="6ea5d-104">מנהלי משאבים יכולים להציע משאב למנהל הפרויקט באמצעות בקשת משאב.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-104">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="6ea5d-105">מרשת הבקשה או מהבקשה עצמה, בחר **חפש משאבים**.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-105">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="6ea5d-106">בדף **מסייע לוח הזמנים‬**, בחר את המשאב ולאחר מכן בחלונית **צור הזמנת משאבים**, בשדה **מצב הזמנה**, בחר **הזמן**.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-106">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

    ![המשאב שהוצע נבחר](media/Resource-Management-image62.png)

<span data-ttu-id="6ea5d-108">עדכוני המצב הבאים מתרחשים:</span><span class="sxs-lookup"><span data-stu-id="6ea5d-108">The following status updates occur:</span></span>

- <span data-ttu-id="6ea5d-109">בדף **מסייע לוח הזמנים**, מחווני המצב מתעדכנים כדי לציין שההזמנה היא הזמנה מוצעת, לא הזמנה בטוחה.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>

    ![מחווני מצב עבור הזמנה מוצעת בדף 'מסייע לוח זמנים'](media/Resource-Management-image63.png)

- <span data-ttu-id="6ea5d-111">בבקשת המשאב, המצב משתנה ל **‏‫נחוצה סקירה‬**.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-111">On the resource request, the status is changed to **Needs Review**.</span></span>

    ![מצב בקשת המשאב משתנה ל'‏‫נחוצה סקירה‬'](media/Resource-Management-image64.png)

- <span data-ttu-id="6ea5d-113">בכרטיסיה **צוות** של הפרויקט, הערך **מצב בקשה** של חבר הצוות הכללי משתנה ל **‏‫נחוצה סקירה‬**.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-113">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

    ![מצב הבקשה של חבר צוות כללי משתנה ל'‏‫נחוצה סקירה‬' בכרטיסיה 'צוות'.](media/Resource-Management-image48.png)

<span data-ttu-id="6ea5d-115">מנהל הפרויקט יכול לקבל או לדחות את ההצעה.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-115">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="6ea5d-116">כאשר מנהלי משאבים מעבדים בקשות משאבים, הם יכולים להשתמש באחת מהגישות הבאות:</span><span class="sxs-lookup"><span data-stu-id="6ea5d-116">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="6ea5d-117">הצעת משאבים מרובים כדי לספק את הביקוש אם אין אפילו משאב אחד למימוש השעות הנדרשות.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-117">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="6ea5d-118">כעת השעות המוצעות מתחלקות בין משאבים מרובים שיכולים לספק את השעות הנדרשות.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-118">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="6ea5d-119">בתרחיש זה, השעות אינן יכולות להיות חופפות.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-119">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="6ea5d-120">הצעת פחות משאבים מן הנדרש.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-120">Propose fewer resources than are required.</span></span> <span data-ttu-id="6ea5d-121">בתרחיש זה, קיבולת המשאב המוצע נמוכה מהשעות הדרושות שהמבקש ציין.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-121">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="6ea5d-122">לכן, כאשר המבקש מקבל את המשאבים המוצעים, נוצרת דרישה למשאב שלא התמלא כדי ללכוד את הביקוש הנותר.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-122">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="6ea5d-123">הזמנת משאבים מרובים כדי לספק את הביקוש אם אין אפילו משאב אחד להשלמת העבודה.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-123">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="6ea5d-124">הזמנת פחות משאבים מן הנדרש.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-124">Book fewer resources than are required.</span></span> <span data-ttu-id="6ea5d-125">בתרחיש זה, מספר השעות שהוזמנו קטן יותר מן השעות הנדרשות.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-125">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="6ea5d-126">המערכת מנחה אותך להציע משאבים במקום הזמנות, כדי שהמבקש יוכל לאמת ולעקוב אחר הביקוש הנותר.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-126">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="billable-utilization"></a><span data-ttu-id="6ea5d-127">ניצול לחיוב</span><span class="sxs-lookup"><span data-stu-id="6ea5d-127">Billable utilization</span></span>

<span data-ttu-id="6ea5d-128">המשאבים יכולים לכלול ניצול יעד לחיוב.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-128">Resources can have a target billable utilization.</span></span> <span data-ttu-id="6ea5d-129">ניצול יעד זה מוגדר כתכונה בתפקיד ברירת מחדל של משאב או מוגדר ברשומה של המשאב היחיד הניתן להזמנה.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-129">This target utilization is either defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="6ea5d-130">חישובי ניצול מבוססים על השעות בפועל שדיווחו המשאבים באמצעות ערכי זמן שאושרו.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-130">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="6ea5d-131">הנוסחאות הבאות משמשות לחישוב הניצול:</span><span class="sxs-lookup"><span data-stu-id="6ea5d-131">The following formulas are used to calculate utilization:</span></span>

- <span data-ttu-id="6ea5d-132">ניצול לחיוב = שעות בפועל הניתנות לחיוב ÷ קיבולת משאב</span><span class="sxs-lookup"><span data-stu-id="6ea5d-132">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
- <span data-ttu-id="6ea5d-133">ניצול שאינו לחיוב = זמן בפועל עם מזהה סוג חיוב = 'אינו לחיוב', 'משלים' או 'לא זמין' ÷ קיבולת משאב</span><span class="sxs-lookup"><span data-stu-id="6ea5d-133">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
- <span data-ttu-id="6ea5d-134">פנימי = זמן בפועל ללא חוזה מכירות ÷ קיבולת משאב</span><span class="sxs-lookup"><span data-stu-id="6ea5d-134">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
- <span data-ttu-id="6ea5d-135">קיבולת משאב = שעות עבודה של משאב – מחוץ למשרד – ימים שאינם ימי עבודה</span><span class="sxs-lookup"><span data-stu-id="6ea5d-135">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="6ea5d-136">ניתן למצוא את התצוגה **ניצול משאב** בחלונית **משאבים**.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-136">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

![תצוגת ניצול משאבים](media/Resource-Management-image65.png)

<span data-ttu-id="6ea5d-138">כל תא ברשת מייצג את אחוז הניצול לחיוב של המשאב בתקופה, כגון יום, שבוע או חודש.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-138">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="6ea5d-139">הנוסחאות הבאות משמשות לצביעת התאים:</span><span class="sxs-lookup"><span data-stu-id="6ea5d-139">The following formulas are used to color the cells:</span></span>

- <span data-ttu-id="6ea5d-140">**ירוק:** ניצול לחיוב \>= ניצול יעד של משאב</span><span class="sxs-lookup"><span data-stu-id="6ea5d-140">**Green:** Billable utilization \>= Resource target utilization</span></span>
- <span data-ttu-id="6ea5d-141">**צהוב:** יעד ניצול – 20 \<= ניצול לחיוב \< יעד ניצול</span><span class="sxs-lookup"><span data-stu-id="6ea5d-141">**Yellow:** Target utilization – 20 \<= Billable utilization \< Target utilization</span></span>
- <span data-ttu-id="6ea5d-142">**אדום:** ניצול לחיוב \< יעד ניצול – 20</span><span class="sxs-lookup"><span data-stu-id="6ea5d-142">**Red:** Billable utilization \< Target utilization – 20</span></span>

<span data-ttu-id="6ea5d-143">מכיוון שהתצוגה **ניצול משאבים** מבוססת על לוח הזמנים, ניתן להשתמש ביכולות הסינון של לוח הזמנים כדי לסנן את התוצאות.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-143">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="6ea5d-144">הרשת מחייבת הגדרה של ניצול יעד בתפקיד או במשאב הבודד.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-144">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="6ea5d-145">לצורך ביצוע ההגדרה, עבור אל **משאבים** \> **תפקידי משאבים**.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-145">To do this setup, go to **Resources** \> **Resource roles**.</span></span>

<span data-ttu-id="6ea5d-146">בנוסף, יש להקצות תפקיד ברירת מחדל לכל משאב הניתן להזמנה.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-146">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="6ea5d-147">עבור אל **משאבים** \> **משאבים**.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-147">Go to **Resources** \> **Resources**.</span></span> <span data-ttu-id="6ea5d-148">בכרטיסיה **Project Service**, הקפד להגדיר תפקיד משאב וודא שהשדה **מהווה ברירת מחדל** עבורו מוגדר ל **כן**.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-148">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field for it is set to **Yes**.</span></span> <span data-ttu-id="6ea5d-149">ניתן להוסיף תפקידים נוספים כאשר **מהווה ברירת מחדל = לא**.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-149">You can add additional roles where **Is Default = No**.</span></span> <span data-ttu-id="6ea5d-150">התפקיד שבו **מהווה ברירת מחדל = כן** משמש להערכה של ניצול המשאב כנגד היעד עבור אותו תפקיד.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-150">The role where the **Is Default = Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

![תפקיד ברירת המחדל שהוגדר](media/Resource-Management-image67.png)

<span data-ttu-id="6ea5d-152">בכרטיסיה **Project Service**, ניתן גם להגדיר ניצול יעד בודד עבור המשאב.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-152">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="6ea5d-153">כעת, חישוב הניצול משתמש בניצול היעד כדי להעריך את היעד של המשאב במקום את היעד של תפקיד ברירת המחדל של המשאב.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-153">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="6ea5d-154">הניצול מוצג עבור משאב רק אם משאב זה אישר זמן הניתן לחיוב במהלך התקופה המופיעה ברשת.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-154">Utilization is shown for a resource only if that resource has approved, chargeable time during the period that is shown in the grid.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="6ea5d-155">זמינות משאב</span><span class="sxs-lookup"><span data-stu-id="6ea5d-155">Resource availability</span></span>

<span data-ttu-id="6ea5d-156">חשוב שמנהלי משאבים יוכלו להציג זמינות של משאבים ולעדכן הזמנות.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-156">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="6ea5d-157">במקרים מסוימים, אין ביקוש רשמי (בקשת משאב), אך מנהל משאבים חייב להגיב לביקוש לא מתוכנן שמגיע דרך ערוצים כגון דואר, שיחת טלפון או הודעה מיידית.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-157">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="6ea5d-158">מנהלי משאבים משתמשים בלוח הזמנים כדי לעדכן משאבים והזמנות.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-158">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="6ea5d-159">שעות עבודה של משאב משמשות כבסיס לחישוב הזמינות של משאב.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-159">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="6ea5d-160">הזמנות של משאבים צורכות את הקיבולת של המשאבים.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-160">Resource bookings consume the capacity of the resources.</span></span>

![לוח זמנים](media/Resource-Management-image68.png)

<span data-ttu-id="6ea5d-162">לוח הזמנים משתמש בצבעים ובהצללה כדי להציג הזמנות, זמינות והזמנות יתר וכן את מצב ההזמנות.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-162">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="6ea5d-163">הגדרה בהגדרות לוח הזמנים מאפשרת לך להציג מקרא.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-163">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="6ea5d-164">אם מופיע חץ המצביע ימינה ליד משאב בודד הניתן להזמנה בלוח הזמנים, ניתן להרחיב את המשאב כך שיציג פרטים של העבודה שהמשאב הוזמן עבורה.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-164">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

![משאב הניתן להזמנה שהורחב בלוח הזמנים](media/Resource-Management-image69.png)

<span data-ttu-id="6ea5d-166">מכיוון ש- Dynamics 365 Project Service Automation משתמש במנגנון Universal Resource Scheduling, אם במחשב שלך מותקן גם Dynamics 365 Field Service, תוכל להציג את פרטי הזמנות המשאבים עבור פרויקטים, הזמנות עבודה וכל ישות אחרת שהארכת את התזמון שלה.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-166">Because Dynamics 365 Project Service Automation uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

![פרטים של הזמנות משאבים עבור פרויקטים והזמנות עבודה](media/Resource-Management-image70.png)

<span data-ttu-id="6ea5d-168">כדי להציג פרטים נוספים אודות משאב בודד, לחץ עליו באמצעות לחצן העכבר הימני כדי לפתוח את כרטיס המשאב.</span><span class="sxs-lookup"><span data-stu-id="6ea5d-168">To view more details about an individual resource, right-click it to open the resource card.</span></span>

![כרטיס משאב](media/Resource-Management-image71.png)
