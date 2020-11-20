---
title: הזמנת משאבים בעלי שם הניתנים להזמנה לצוות פרוייקט והקצאת משימות
description: נושא זה מספק מידע על אופן הזמנת משאבים בעלי שם לצוותי פרוייקט והקצאתם למשימות.
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 11/28/2018
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
ms.openlocfilehash: 0300c494a3294b26e2de6bbfa1dd50a76bb72651
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130174"
---
# <a name="book-named-bookable-resources-to-a-project-team-and-assign-tasks"></a><span data-ttu-id="477eb-103">הזמנת משאבים בעלי שם הניתנים להזמנה לצוות פרוייקט והקצאת משימות</span><span class="sxs-lookup"><span data-stu-id="477eb-103">Book named bookable resources to a project team and assign tasks</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="477eb-104">באפשרותך להוסיף משאב בעל שם לצוות הפרוייקט שלך על-ידי הזמנתו ישירות אל הצוות.</span><span class="sxs-lookup"><span data-stu-id="477eb-104">You can  add a named resource to your project team by booking them directly onto the team.</span></span> <span data-ttu-id="477eb-105">לשם כך, בצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="477eb-105">To do this, complete the following steps.</span></span>

1. <span data-ttu-id="477eb-106">ב- Project Service Automation, עבור אל **פרוייקטים**, ובחר לפתוח את הפרוייקט שאתה מזמין עבורו.</span><span class="sxs-lookup"><span data-stu-id="477eb-106">In  Project Service Automation, go to **Projects**, and select the open the project that you are booking for.</span></span>
2. <span data-ttu-id="477eb-107">בדף **פרוייקט**, בכרטיסיה **צוות**, לחץ על **חדש**.</span><span class="sxs-lookup"><span data-stu-id="477eb-107">On the **Project** page, on the **Team** tab, click **New**.</span></span> 

![הוספת חבר צוות מהכרטיסיה 'צוות'](media/RM-how-to-1.png)

3. <span data-ttu-id="477eb-109">בתיבת הדו-שיח **יצירה מהירה של חבר צוות**, בחר את המשאב הניתן להזמנה.</span><span class="sxs-lookup"><span data-stu-id="477eb-109">In the **Quick Create Project Team Member** dialog box, select the bookable resource.</span></span> <span data-ttu-id="477eb-110">השדה **תפקיד** יאוכלס בתפקיד ברירת המחדל של המשאב, אם יש תפקיד שהוקצה לו.</span><span class="sxs-lookup"><span data-stu-id="477eb-110">The **Role** field will populate with the resource's default role if they have one assigned.</span></span> <span data-ttu-id="477eb-111">באפשרותך לשנות את התפקיד במידת הצורך.</span><span class="sxs-lookup"><span data-stu-id="477eb-111">You can change the role if needed.</span></span> 
4. <span data-ttu-id="477eb-112">בחר את תאריכי מ- ועד שהמשאב יזדקק להם ובחר את שיטת ההקצאה של קיבולת המשאב.</span><span class="sxs-lookup"><span data-stu-id="477eb-112">Select the from and to dates that the resource will be needed and select the allocation method of the resource's capacity.</span></span> 
5. <span data-ttu-id="477eb-113">אם ברצונך שחבר הצוות יהיה מאשר פרוייקט, בחר **כן** בשדה **מאשר פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="477eb-113">If you want the team member to be a project approver, select **Yes** in the **Project Approver** field.</span></span> <span data-ttu-id="477eb-114">משמעות הדבר היא שחבר הצוות יוכל לאשר ערכי זמן והוצאה שנשלחו עבור הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="477eb-114">This will mean that the team member can approve submitted time and expense entries for this project.</span></span> 
6. <span data-ttu-id="477eb-115">לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="477eb-115">Click **Save**.</span></span>

![הוספת חבר צוות בטופס היצירה המהירה](media/RM-how-to-2.png)


<span data-ttu-id="477eb-117">כעת באפשרותך להקצות את המשאב שהוזמן למשימות בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="477eb-117">You can now assign the booked resource to tasks on the project.</span></span> <span data-ttu-id="477eb-118">בדף **פרוייקט**, לחץ על הכרטיסיה **תזמון** כדי להקצות משימות למשאב החדש.</span><span class="sxs-lookup"><span data-stu-id="477eb-118">On the **Project** page, click the **Schedule** tab to assign tasks to the new resource.</span></span> <span data-ttu-id="477eb-119">בורר המשאבים שמופעל מהשדה **משאבים** ברשת המשימה יציג את חברי הצוות שבאפשרותך לבחור.</span><span class="sxs-lookup"><span data-stu-id="477eb-119">The resource picker that is launched from the **Resources** field in the task grid will show the team members that you can select.</span></span>

![הקצאת חבר צוות למשימה בכרטיסיה 'תזמון'](media/RM-how-to-3.png)

<span data-ttu-id="477eb-121">בגירסה 3 עבור Project Service Automation‏ (PSA), הזמנות משאבים והקצאות משימות אינן משולבות באופן הדוק.</span><span class="sxs-lookup"><span data-stu-id="477eb-121">In version 3 for Project Service Automation (PSA), resource bookings and task assignments are not tightly coupled.</span></span> <span data-ttu-id="477eb-122">משמעות הדבר היא שכאשר אתה משתמש בבורר המשאבים בלוח הזמנים, באפשרותך להקצות משימות לחברי צוות עבור מספר שעות גדול יותר מכפי שההזמנות שלהם מכסות בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="477eb-122">This means that when you use the resource picker in the schedule, you can assign tasks to team members for more hours than their bookings cover on the project.</span></span>
<span data-ttu-id="477eb-123">באפשרותך לראות את ההבדלים בין הזמנות של חברי צוות והקצאות בכרטיסיה **צוות** או בכרטיסיה **התאמת משאבים**. באפשרותך גם ליישב את ההבדלים בין הזמנות והקצאות עבור משאבים ברמה מפורטת יותר.</span><span class="sxs-lookup"><span data-stu-id="477eb-123">You can see the differences between team member bookings and assignments on the **Team** tab or on the **Resource Reconciliation** tab. You can also reconcile the differences between bookings and assignments for resources at a more detailed level.</span></span>

![הכרטיסיה 'התאמת משאבים'](media/RM-how-to-4.png)

<span data-ttu-id="477eb-125">תוכל גם להשתמש בבורר המשאבים בכרטיסיה **תזמון** כדי לחפש ולבחור משאבים הניתנים להזמנה שאינם עדיין חלק מצוות הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="477eb-125">You can also use the resource picker on the **Schedule** tab to search for and select bookable resources that are not already part of the project team.</span></span> <span data-ttu-id="477eb-126">הם מוצגים בבורר המשאבים כ **משאבים אחרים**.</span><span class="sxs-lookup"><span data-stu-id="477eb-126">These are shown in the resource picker as **Other Resources**.</span></span>

![הקצאת משאב שאינו חבר צוות למשימה](media/RM-how-to-5.png)

<span data-ttu-id="477eb-128">כאשר אתה עושה זאת, המשאב מתווסף לצוות הפרוייקט ומוקצה למשימה, אבל לא נוצרות הזמנות.</span><span class="sxs-lookup"><span data-stu-id="477eb-128">When you do this, the resource is added to the project team and assigned to the task, but no bookings are generated.</span></span>

![חבר צוות עם הקצאות וללא הזמנות](media/RM-how-to-6.png)

<span data-ttu-id="477eb-130">באפשרותך להשתמש ביכולת הארכת ההזמנה של הכרטיסיה  **פיוס** או ב **לוח זמנים** כדי להזמין את קיבולת המשאב לפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="477eb-130">You can use the **Reconciliation** tab’s extend booking capability or the **Schedule Board** to book the resource’s capacity to the project.</span></span>

![הארכת הזמנות עבור חבר צוות בכרטיסיה 'התאמת משאבים'](media/RM-how-to-7.png)

<span data-ttu-id="477eb-132">לאחר שחבר צוות מוזמן לפרוייקט, באפשרותך להשתמש בשמירת הזמנות או להשתמש בלוח הזמנים ישירות כדי לנהל את ההזמנות שלו.</span><span class="sxs-lookup"><span data-stu-id="477eb-132">After a team member is booked on your project, you can use maintain bookings or use the Schedule Board directly to manage their bookings.</span></span>
