---
title: ניהול אזורי זמן
description: כאשר נוצר פרויקט, אזור הזמן שלו מבוסס על אזור הזמן שהוגדר בתבנית שעות העבודה שהוחלה.
author: ruhercul
ms.date: 10/05/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 1480d68105be1041e791de567b180178b330d71e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997737"
---
# <a name="manage-time-zones"></a><span data-ttu-id="1bde5-103">ניהול אזורי זמן</span><span class="sxs-lookup"><span data-stu-id="1bde5-103">Manage time zones</span></span>

<span data-ttu-id="1bde5-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="1bde5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


## <a name="projects"></a><span data-ttu-id="1bde5-105">פרויקטים</span><span class="sxs-lookup"><span data-stu-id="1bde5-105">Projects</span></span>

<span data-ttu-id="1bde5-106">כאשר נוצר פרויקט, אזור הזמן מבוסס על אזור הזמן שהוגדר בתבנית שעות העבודה שהוחלה.</span><span class="sxs-lookup"><span data-stu-id="1bde5-106">When a project is created, the time zone is based on the time zone defined in the applied work hour template.</span></span> <span data-ttu-id="1bde5-107">בטופס **פרויקט**, התאריכים תמיד מתיחסים לאזור הזמן של המשתמש המחובר בכל כרטיסיה, למעט בכרטיסיה **משימה**. כאשר מציגים את מבנה התפלגות העבודה, התאריכים תמיד יוצגו באזור הזמן של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="1bde5-107">On the **Project** for, the dates are always relative to the time zone of the user that is logged in on each tab, except the **Task** tab. When you view the work breakdown structure, the dates will always be displayed in the project’s time zone.</span></span>

## <a name="tasks"></a><span data-ttu-id="1bde5-108">משימות</span><span class="sxs-lookup"><span data-stu-id="1bde5-108">Tasks</span></span>

<span data-ttu-id="1bde5-109">כאשר נוצרת משימה, מועד ההתחלה, מועד הסיום והשעות/יום נשלטים על ידי שעות העבודה של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="1bde5-109">When a task is created, the start time, end time, and hours/day is controlled by the working hours of the project.</span></span> <span data-ttu-id="1bde5-110">לדוגמה, אם נוצרת משימה בפרויקט שאזור הזמן שלו הוא ‎-‎8‏PST ומוגדרות לו שעות העבודה הבאות: 09:00 עד 17:00 בימים שני עד שישי, כל משימה שנוצרת ללא הקצאה תכבד את מועד ההתחלה ואת מועד סיום של לוח השנה של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="1bde5-110">For example, if a task is created with a project whose time zone is -8 PST and has the following working hours: 9:00 AM to 5:00 PM Monday to Friday, any task created without an assignment will respect the start time and end time of the project calendar.</span></span>

## <a name="manage-resources-with-time-zones"></a><span data-ttu-id="1bde5-111">ניהל משאבים עם אזורי זמן</span><span class="sxs-lookup"><span data-stu-id="1bde5-111">Manage resources with time zones</span></span>

<span data-ttu-id="1bde5-112">לקבלת תוצאות מדויקות וניתנות לחיזוי בעת השימוש באפשרות **הארך ההזמנה**, ישנן שתי תנאים מקדימים שחייבים לעמוד בהם:</span><span class="sxs-lookup"><span data-stu-id="1bde5-112">For accurate and predictable results when using **Extend Booking**, there are two key prerequisites that must be met:</span></span>  

- <span data-ttu-id="1bde5-113">על המשתמש להגדיר את אזור הזמן של המכשיר כך שיתאים לאזור הזמן שהוגדר ב **הגדרות התאמה אישית** של המערכת.</span><span class="sxs-lookup"><span data-stu-id="1bde5-113">The user must configure their device's time zone to match the time zone defined in the system's **Personalization Settings**.</span></span>
 
  ![הגדרות אזור זמן ב- Windows 10](media/reconcile-assignments-03.png)

  ![הגדרות אזור זמן בהגדרות ההתאמה האישית](media/reconcile-assignments-04.png)
 
- <span data-ttu-id="1bde5-116">צריך שיהיה להמשאב הניתן להזמנה לפחות דקה של זמן עבודה שחופף לקווי המיתאר המשמשים להגדרת ההארכה המבוקשת.</span><span class="sxs-lookup"><span data-stu-id="1bde5-116">The bookable resource must have at least one minute of working time that overlaps with the contours that are used to define the requested extension.</span></span> <span data-ttu-id="1bde5-117">לדוגמה, למשאבים הבאים שעות עבודה שחלות בין 9:00 ל-19:00.</span><span class="sxs-lookup"><span data-stu-id="1bde5-117">For example, the following resources with working hours that fall between 9:00 AM and 7:00 PM.</span></span> 

  ![השוואה בין קווי המתאר של המשאבים](media/reconcile-assignments-05.png)

<span data-ttu-id="1bde5-119">בטבלה הבאה ניתן לראות:</span><span class="sxs-lookup"><span data-stu-id="1bde5-119">The following table shows:</span></span>

- <span data-ttu-id="1bde5-120">תבנית לוח שנה של פרויקט</span><span class="sxs-lookup"><span data-stu-id="1bde5-120">A project calendar template</span></span>
- <span data-ttu-id="1bde5-121">משאב א': למשאב זה יש אותו לוח שנה והוא נמצא באותו אזור זמן כמו הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="1bde5-121">Resource A: This resource has the same calendar and is in the same time zone as the project.</span></span> <span data-ttu-id="1bde5-122">זמן ההתחלה של ההזמנות יהיה 9:00 בבוקר.</span><span class="sxs-lookup"><span data-stu-id="1bde5-122">The start time of the bookings will be 9:00 AM.</span></span>
- <span data-ttu-id="1bde5-123">משאב ב': משאב זה ממוקם באזור זמן שונה מהפרויקט ומתחיל בשעה 7:00 בבוקר באזור הזמן שלו.</span><span class="sxs-lookup"><span data-stu-id="1bde5-123">Resource B: This resource is located in a different time zone than the project and starts at 7:00 AM in their time zone.</span></span> <span data-ttu-id="1bde5-124">עם זאת, ההזמנות יחלו בשעה 9:00 בבוקר מכיוון שזהו זמן ההתחלה המוקדם ביותר של מתאר ההקצאה.</span><span class="sxs-lookup"><span data-stu-id="1bde5-124">However, the bookings will begin at 9:00 AM as that is the earliest start time of the assignment contour.</span></span>
- <span data-ttu-id="1bde5-125">משאבים ג' וד': המשאבים ממוקמים באזורי זמן שונים, ששניהם שונים זה מזה ומהפרויקט, וההזמנות שלהם אינן מתחילות לפני זמני ההתחלה הזמינים שלהם בהתאמה.</span><span class="sxs-lookup"><span data-stu-id="1bde5-125">Resources C and D: The resources are located in different time zones, both different from each other and the project, and their bookings start no earlier than their respective available start times.</span></span>

|<span data-ttu-id="1bde5-126">ישות</span><span class="sxs-lookup"><span data-stu-id="1bde5-126">Entity</span></span>  |<span data-ttu-id="1bde5-127">לוח שנה</span><span class="sxs-lookup"><span data-stu-id="1bde5-127">Calendar</span></span>  |
|-|-|
|<span data-ttu-id="1bde5-128">תבנית לוח שנה של פרויקט</span><span class="sxs-lookup"><span data-stu-id="1bde5-128">Project calendar template</span></span>   | ![לוח השנה של הפרויקט](media/reconcile-assignments-06.png) |
|<span data-ttu-id="1bde5-130">משאב א'</span><span class="sxs-lookup"><span data-stu-id="1bde5-130">Resource A</span></span>  | ![לוח שנה של משאב א'](media/reconcile-assignments-06.png) |
|<span data-ttu-id="1bde5-132">משאב ב'</span><span class="sxs-lookup"><span data-stu-id="1bde5-132">Resource B</span></span>  |  ![לוח שנה של משאב ב'](media/reconcile-assignments-07.png) |
|<span data-ttu-id="1bde5-134">משאב ג'</span><span class="sxs-lookup"><span data-stu-id="1bde5-134">Resource C</span></span>  |  ![לוח שנה של משאב ג'](media/reconcile-assignments-08.png) |
|<span data-ttu-id="1bde5-136">משאב ד'</span><span class="sxs-lookup"><span data-stu-id="1bde5-136">Resource D</span></span>  | ![לוח שנה של משאב ד'](media/reconcile-assignments-09.png)  |
 
<span data-ttu-id="1bde5-138">כשמנווטים אל התצוגה **התאמה**, מוצגים הקצאות המשאבים ומחסור ההזמנות המשוייכים מוצגים.</span><span class="sxs-lookup"><span data-stu-id="1bde5-138">When you navigate to the **Reconciliation** view, the resource assignments and the associated booking shortages are displayed.</span></span>

![תצוגת התאמה לפני הרחבה](media/reconcile-assignments-10.png)

<span data-ttu-id="1bde5-140">לאחר שנעשה שימוש בפונקציונליות 'הארך הזמנה' עבור כל משאב, הזמנות מאורכות בהצלחה עבור כל משאב מכיוון ששעות העבודה של כל משאב חופפות לקווי המתאר של המחסור.</span><span class="sxs-lookup"><span data-stu-id="1bde5-140">After the extend booking functionality has been used for each resource, bookings are successfully extended for each resource because each resource’s working hours overlapped with the contours of the shortage.</span></span>

![תצוגת ההתאמה לאחר הארכת ההזמנה](media/reconcile-assignments-11.png) 

<span data-ttu-id="1bde5-142">שימו לב שמבט מקרוב על פרטי ההזמנות מראה הבדלים מועדי התחלת של ההזמנות.</span><span class="sxs-lookup"><span data-stu-id="1bde5-142">Notice that a closer look at the details of the bookings shows differences in the start time of the bookings.</span></span> <span data-ttu-id="1bde5-143">ההזמנות אינן מתחילות לפני מועד ההתחלה של קו המיתאר של ההקצאה ולא לפני מועד ההתחלה הזמין של המשאב.</span><span class="sxs-lookup"><span data-stu-id="1bde5-143">The bookings start no earlier than the start time of the assignment contour and no earlier than the available start time of the resource.</span></span>

![הזמנות חדשות של משאבים בלוח הזמנים](media/reconcile-assignments-12.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]