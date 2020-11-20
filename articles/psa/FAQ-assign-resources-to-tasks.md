---
title: הקצאת משאב למשימה
description: נושא זה מספק מידע אודות אופן הקצאת משאבים למשימות.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/27/2019
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
ms.openlocfilehash: b7aef799ec4b90d602a6f3641cbac06264664f00
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4125134"
---
# <a name="assign-a-resource-to-a-task"></a><span data-ttu-id="7f6a5-103">הקצאת משאב למשימה</span><span class="sxs-lookup"><span data-stu-id="7f6a5-103">Assign a resource to a task</span></span>

<span data-ttu-id="7f6a5-104">קיימות שלוש דרכים להקצאת משאב למשימה ב- Microsoft Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-104">There are three ways to assign a resource to a task in Microsoft Dynamics 365 Project Service Automation.</span></span>

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a><span data-ttu-id="7f6a5-105">הזמנת משאב בתור חבר צוות ולאחר מכן הקצאת המשאב למשימה</span><span class="sxs-lookup"><span data-stu-id="7f6a5-105">Book a resource as a team member, and then assign the resource to a task</span></span>

<span data-ttu-id="7f6a5-106">באפשרותך להוסיף משאב לצוות הפרוייקט ולאחר מכן להקצות את המשאב למשימות בלוח זמנים של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-106">You can add a resource to the project team, and then assign the resource to tasks in the project schedule.</span></span>

1. <span data-ttu-id="7f6a5-107">בכרטיסיה **חבר צוות**, הוסף חבר צוות חדש על-ידי בחירת **חדש**.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-107">On the **Team Member** tab, add a new team member by selecting **New**.</span></span> 

2. <span data-ttu-id="7f6a5-108">החלונית **יצירה מהירה של חבר צוות** תיפתח ובה תוכל לבחור את שם המשאב הניתן להזמנה ולהגדיר תפקיד.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-108">The **Team Member Quick Create** panel opens, where you can select the bookable resource name and set a role.</span></span> 

    <span data-ttu-id="7f6a5-109">בחר באחת משיטות ההקצאה הבאות להזמנת המשאב:</span><span class="sxs-lookup"><span data-stu-id="7f6a5-109">Select one of the following allocation methods for the resource’s booking:</span></span>

    - <span data-ttu-id="7f6a5-110">**קיבולת מלאה** מזמינה קיבולת מלאה של המשאב עבור התאריכים 'מ' ו'עד' שצוינו.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-110">**Full Capacity** books the resource’s full capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="7f6a5-111">**קיבולת באחוזים** מזמינה את המשאב לאחוז הקיבולת של המשאב עבור התאריכים 'מ' ו'עד' שצוינו.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-111">**Percentage Capacity** books the resource for a percentage of the resource's capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="7f6a5-112">**‏‫הפצת שעות באופן שווה‬** מזמינה את המשאב למספר מסוים של שעות, ומפיצה אותן באופן שווה בכל יום בטווח התאריכים 'מ'/'עד' שצוינו.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-112">**By Hours Distribute Evenly** books the resource for a specified number of hours, distributing them evenly per day over the specified from and to dates.</span></span>
    - <span data-ttu-id="7f6a5-113">**לפי ‏‫שעות עומס חזיתי‬** מזמינה את המשאב למספר מסוים של שעות, ומחלקת את השעות ביום לפי עומס חזיתי בטווח התאריכים 'מ' ו'עד' שצוינו.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-113">**By Hours Front Load** books the resource for a specified number of hours, front-loading the per-day hours over the specified from and to dates.</span></span>
    - <span data-ttu-id="7f6a5-114">**ללא** מוסיפה את המשאב לצוות, אך אינה יוצרת הזמנות כלשהן אשר סופגות את הקיבולת שלו.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-114">**None** adds the resource to the team but doesn’t create any bookings that absorb their capacity.</span></span>

3. <span data-ttu-id="7f6a5-115">ברשת **לוח זמנים** עבור משימה, בחר בסמל **משאב** בתא המשאב, ולאחר מכן תחת **חברי צוות**, בחר את חבר הצוות שהוספת זה עתה.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-115">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell, and then under **Team Members**, select the team member you just added.</span></span> 

> [!NOTE]
> <span data-ttu-id="7f6a5-116">גם בכרטיסיה **חבר צוות** וגם בכרטיסיה **פיוס**, המשאב מציג את השעות שהוזמנו והשעות שהוקצו.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-116">On the **Team Member** and **Reconciliation** tabs, the resource shows booked and assigned hours.</span></span> <span data-ttu-id="7f6a5-117">השעות אמורות להיות זהות, אך אין זו חובה מפני שהזמנות והקצאות אינן משולבות באופן הדוק.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-117">The hours should be the same, but it isn't required as bookings and assignments are not tightly coupled.</span></span> <span data-ttu-id="7f6a5-118">הכרטיסיה **פיוס** מספקת פרטים כאשר השעות שונות, למשל כאשר אתה מקצה למשאב יותר שעות ממה שהזמנת.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-118">The **Reconciliation** tab gives you details when they are different, such as when you assign a resource more hours than you have booked.</span></span> <span data-ttu-id="7f6a5-119">בעת הצורך, באפשרותך לתקן את המידע על-ידי הרחבת הזמנות המשאב או שינוי ההקצאה.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-119">If needed, you can correct the information by extending the resource's bookings or changing the assignment.</span></span>

## <a name="create-a-generic-team-member-through-task-assignment"></a><span data-ttu-id="7f6a5-120">יצירת חבר צוות כללי באמצעות הקצאת משימות</span><span class="sxs-lookup"><span data-stu-id="7f6a5-120">Create a generic team member through task assignment</span></span>

<span data-ttu-id="7f6a5-121">כאשר אתה יוצר חבר צוות כללי דרך הקצאת המשימה, עליך ליצור מציין מיקום או משאב כללי המתאר את המאפיינים של המשאב בעל השם, שברצונך שיעבוד על המשימות בסופו של דבר.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-121">When you create a generic team member through task assignment, you create a placeholder or generic resource that describes the characteristics of the named resource you ultimately want to work on the tasks.</span></span> <span data-ttu-id="7f6a5-122">לאחר מכן צור דרישה (או הגש בקשה באמצעות הדרישה) המשמשת לחיפוש ולהזמנה של משאב בעל שם.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-122">You then generate a requirement (or submit a request using the requirement) that is used to search for and book the named resource.</span></span>

1. <span data-ttu-id="7f6a5-123">ברשת **לוח זמנים** עבור משימה, בחר בסמל **משאב** בתא המשאב.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-123">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell.</span></span>

2. <span data-ttu-id="7f6a5-124">הקלד שם שישמש כשם המשאב מציין המיקום.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-124">Type a name to serve as the placeholder resource’s name.</span></span> <span data-ttu-id="7f6a5-125">לדוגמה, מנהל תוכנית.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-125">For example, Program Manager.</span></span>

3. <span data-ttu-id="7f6a5-126">בחר **צור** ובשדה **יצירה מהירה של חבר צוות פרוייקט**, הגדר את התפקיד עבור המשאב הכללי.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-126">Select **Create**, and in the **Quick Create Project Team Member** field, set the role for the generic resource.</span></span>

4. <span data-ttu-id="7f6a5-127">באפשרותך להמשיך להקצות משימות למשאב מציין מיקום זה על-ידי בחירת המשאב ב **בורר המשאבים** עבור המשימה.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-127">You can continue to assign tasks to this placeholder resource by selecting the resource on the **Resource Selector** for the task.</span></span> <span data-ttu-id="7f6a5-128">הם מופיעים ברשימה תחת **חברי צוות**.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-128">They’re listed under **Team Members**.</span></span>

5. <span data-ttu-id="7f6a5-129">כאשר תסיים להקצות את המשאב הכללי, בחר את המשאב הכללי בכרטיסיה **צוות** ובחר **צור דרישה** כדי ליצור דרישת משאב עבור המשאב הכללי.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-129">When you’re done assigning the generic resource, select the generic resource on the **Team** tab, and then select **Generate Requirement** to create a resource requirement for the generic resource.</span></span>

6. <span data-ttu-id="7f6a5-130">בחר **הזמנה** עבור המשאב הכללי.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-130">Select **Book** for the generic resource.</span></span> <span data-ttu-id="7f6a5-131">לאחר מכן באפשרותך להשתמש בלוח זמנים כדי למצוא ולהזמין משאב אמיתי.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-131">You can then use the Schedule board to find and book a real resource.</span></span> <span data-ttu-id="7f6a5-132">באפשרותך גם לשלוח את הדרישה למימוש על-ידי מנהל משאבים.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-132">You can also submit the requirement for fulfillment by a resource manager.</span></span>

7. <span data-ttu-id="7f6a5-133">בעת מימוש משאב כללי עם משאב בעל שם, המשאב הכללי מוסר מהצוות, והקצאות המשימות עבור המשאב הכללי מוקצות למשאב בעל שם שמילא את דרישת המשאב של המשאב הכללי.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-133">When the generic resource is fulfilled with a named resource, the generic resource is removed from the team and the task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>

## <a name="assign-a-named-resource-from-the-list-of-all-bookable-resources"></a><span data-ttu-id="7f6a5-134">הקצאת משאב בעל שם מתוך רשימת כל המשאבים הניתנים להזמנה</span><span class="sxs-lookup"><span data-stu-id="7f6a5-134">Assign a named resource from the list of all bookable resources</span></span>

<span data-ttu-id="7f6a5-135">באפשרותך להשתמש בתיבת החיפוש של **בורר המשאבים** כדי לחפש את כל המשאבים הניתנים להזמנה ולהקצות אותם למשימה.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-135">You can use the search box in the **Resource Selector** to search all bookable resources and assign them to a task.</span></span>

<span data-ttu-id="7f6a5-136">משאבים שהוקצו בדרך זו יתווספו לצוות ללא הזמנות.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-136">Resources assigned this way are added to the team without any bookings.</span></span> <span data-ttu-id="7f6a5-137">הדבר דומה להוספת חבר צוות ובחירת 'ללא' כשיטת ההקצאה.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-137">This is similar to adding a team member and selecting None as the allocation method.</span></span> <span data-ttu-id="7f6a5-138">המשאב מוצג בכרטיסיות **צוות** ו **פיוס** כמשאב עם הקצאות בלבד וגירעון של הזמנות.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-138">The resource is displayed in the **Team** and **Reconciliation** tabs as resources with only assignments and a booking deficit.</span></span> <span data-ttu-id="7f6a5-139">הזמן אותם אם ברצונך להשתמש בזמינות שלהם.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-139">Book them if you want to use their availability.</span></span>

1. <span data-ttu-id="7f6a5-140">ברשת **לוח זמנים** עבור משימה, בחר בסמל **משאב** בתא המשאב.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-140">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell.</span></span>

2. <span data-ttu-id="7f6a5-141">התחל להקליד שם.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-141">Start typing a name.</span></span> <span data-ttu-id="7f6a5-142">תוצאות החיפוש עבור השם מוצגות ב **בורר המשאבים** תחת **משאבים אחרים**.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-142">The search results for the name are displayed in the **Resource Selector** under **Other Resources**.</span></span>

3. <span data-ttu-id="7f6a5-143">בחר את המשאב שברצונך להקצות למשימה.</span><span class="sxs-lookup"><span data-stu-id="7f6a5-143">Select the resource that you want to assign to the task.</span></span>

