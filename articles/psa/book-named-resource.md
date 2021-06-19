---
title: הזמנת משאבים בעלי שם מדרישות משאב
description: נושא זה מספק מידע אודות הזמנת משאבים בעלי שם עבור דרישת משאב כללי.
author: JohnPBurrows
ms.custom:
- dyn365-projectservice
ms.date: 12/11/2018
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
ms.openlocfilehash: c2f97107de938975491770ab4e2ed18a3145d0e3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013397"
---
# <a name="book-named-resources-from-resource-requirements"></a><span data-ttu-id="12345-103">הזמנת משאבים בעלי שם מדרישות משאב</span><span class="sxs-lookup"><span data-stu-id="12345-103">Book named resources from resource requirements</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="12345-104">באפשרותך להזמין משאב בעל שם כדי להחליף משאב כללי בעל דרישת משאב.</span><span class="sxs-lookup"><span data-stu-id="12345-104">You can book a named resource to replace generic resource that has a resource requirement.</span></span>

1. <span data-ttu-id="12345-105">ב- Project Service Automation‏ (PSA), בדף **פרוייקטים**, לחץ על הכרטיסיה **צוות**.</span><span class="sxs-lookup"><span data-stu-id="12345-105">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab.</span></span>
2. <span data-ttu-id="12345-106">בחר את המשאב הכללי בעל דרישת משאב מהרשימה ולאחר מכן לחץ על **הזמן**.</span><span class="sxs-lookup"><span data-stu-id="12345-106">Select the generic resource that has a resource requirement from the list and then click **Book**.</span></span> <span data-ttu-id="12345-107">לחלופין, פתח את דרישת המשאב ולאחר מכן לחץ על **הזמן**.</span><span class="sxs-lookup"><span data-stu-id="12345-107">Or, open the resource requirement and then click **Book**.</span></span>


![הזמנת חבר צוות כללי](media/RM-how-to-14.png)


3. <span data-ttu-id="12345-109">בדף **מסייע לוח הזמנים**, בחר משאב בעל שם כדי להזמין לצוות הפרוייקט שלך ולאחר מכן לחץ על **הזמן**.</span><span class="sxs-lookup"><span data-stu-id="12345-109">On the **Schedule Assistant** page, select a named resource to book onto your project team and then click **Book**.</span></span>

![הזמנת חבר צוות כללי באמצעות מסייע לוחות הזמנים](media/RM-how-to-15.png)

<span data-ttu-id="12345-111">לאחר שהזמנה הושלמה ומומשה על-ידי משאב בעל שם, המשאב הכללי מוחלף במשאב בעל שם.</span><span class="sxs-lookup"><span data-stu-id="12345-111">When the booking is complete and fulfilled by a named resource, the generic resource is replaced with the named resource.</span></span>

![חבר צוות בעל שם המחליף חבר צוות כללי](media/RM-how-to-16.png)

<span data-ttu-id="12345-113">ההקצאות בלוח הזמנים מתעדכנות גם במשאב בעל השם.</span><span class="sxs-lookup"><span data-stu-id="12345-113">The assignments on the schedule are updated with the named resource as well.</span></span>

![חבר צוות בעל שם המוקצה למשימות פרוייקט](media/RM-how-to-17.png)

## <a name="fulfill-a-generic-resource-with-multiple-named-resources"></a><span data-ttu-id="12345-115">מימוש משאב כללי עם משאבים מרובים בעלי שם</span><span class="sxs-lookup"><span data-stu-id="12345-115">Fulfill a generic resource with multiple named resources</span></span>
<span data-ttu-id="12345-116">מימוש דרישה עבור משאב כללי עם משאבים מרובים בעלי שם דומה להקצאת משאב יחיד בעל שם.</span><span class="sxs-lookup"><span data-stu-id="12345-116">Fulfilling a requirement for a generic resource with multiple named resources is similar to assigning a single named resource.</span></span> <span data-ttu-id="12345-117">לדוגמה, קיימת משימה עם משך של חמישה ימים ו- 120 שעות מאמץ.</span><span class="sxs-lookup"><span data-stu-id="12345-117">For example, there is a task with a duration of five days and 120 hours of effort.</span></span> <span data-ttu-id="12345-118">משאב אחד הפועל למשך שמונה שעות אופייניות ביום לאורך שבוע עבודה בן חמישה ימים לא יכול להשלים משימה זו.</span><span class="sxs-lookup"><span data-stu-id="12345-118">This task can't be completed by one resource that works a typical eight-hour day over a five day week.</span></span> 

![משימה שזקוקה ל- 120 שעות מאמץ במשך חמישה ימים](media/RM-how-to-21.png)

<span data-ttu-id="12345-120">הדרישה היא עבור 120 שעות של הנדסת רובוטיקה למשך חמישה ימים, כלומר 24 שעות ביום.</span><span class="sxs-lookup"><span data-stu-id="12345-120">The requirement is for 120 hours of robotics engineering over five days, which is 24 hours per day.</span></span>

![דרישה ליום](media/RM-how-to-22.png)

<span data-ttu-id="12345-122">זוהי דוגמה למועד שבו נחוצים משאבים מרובים בעלי שם למימוש בקשת משאב כללי.</span><span class="sxs-lookup"><span data-stu-id="12345-122">This is an example of when multiple named resources are needed to fulfill a generic resource request.</span></span> <span data-ttu-id="12345-123">יהיה עליך להזמין משאבים מרובים למימוש הדרישה.</span><span class="sxs-lookup"><span data-stu-id="12345-123">You will need to book multiple resources to fulfill the requirement.</span></span>

![הזמנת משאבים מרובים למימוש הדרישה](media/RM-how-to-23.png)

<span data-ttu-id="12345-125">ההבדל העיקרי בתרחיש זה הוא שהמשאב הכללי נשאר בצוות המוקצה למשימה, וחברי הצוות של המשאב בעל השם המוזמן אינם מוקצים כחלק מהמשרה.</span><span class="sxs-lookup"><span data-stu-id="12345-125">The main difference in this scenario is that the generic resource remains on the team assigned to the task, and the booked named resource team members are not assigned as part of the position.</span></span> <span data-ttu-id="12345-126">מנהל הפרויקט יכול להקצות את העבודה בהתאם למשאבים בעלי השם.</span><span class="sxs-lookup"><span data-stu-id="12345-126">The project manager can assign the work as appropriate to the named resources.</span></span> <span data-ttu-id="12345-127">התצוגה **פיוס** יכולה לסייע למנהל פרויקט בפירוט של ההזמנות במשאבים המרובים להקצאות משימות.</span><span class="sxs-lookup"><span data-stu-id="12345-127">The **Reconciliation** view can assist a project manager in breaking up the bookings across multiple resources to task assignments.</span></span> <span data-ttu-id="12345-128">פעולה זו אינה מתבצעת באופן אוטומטי משום שבכל תרחיש המורכב יותר מהדוגמה הפשוטה לעיל, כגון מקרים שבהם יש חבילת משימות המרכיבה את הדרישה, המערכת צריכה להניח מהי הכוונה שעומדת מאחורי צורת ההקצאה הרצויה של מנהל הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="12345-128">This is not done automatically because in any scenario more complicated than the simple example above, such as where you have a bundle of tasks making up the requirement, the intent of how the project manager wants to assign, needs to be assumed by the system.</span></span> <span data-ttu-id="12345-129">כיוון שהמערכת אינה יכולה להבין כוונות, רוב הסיכויים שההנחות יהיו שונות מהכוונה ועלולה להתקבל תוצאה שגויה או בלתי צפויה.</span><span class="sxs-lookup"><span data-stu-id="12345-129">Because the system can't understand intent, chances are that the assumptions will be different than intended and an incorrect or unpredictable result will happen.</span></span> <span data-ttu-id="12345-130">התוצאה הצפויה היא שהמשאב הכללי יישאר מוקצה עד שמנהל הפרוייקט ייצור במכוון הקצאות, בסיוע התצוגה **פיוס**.</span><span class="sxs-lookup"><span data-stu-id="12345-130">The predictable outcome is that the generic resource remains assigned until the project manager deliberately creates assignments, with the assistance of the **Reconciliation** view.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]