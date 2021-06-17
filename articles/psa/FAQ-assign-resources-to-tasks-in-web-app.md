---
title: כיצד להקצות משאב הניתן להזמנה למשימה ביישום האינטרנט
description: מבט כולל על הדרכים שבהן באפשרותך להקצות משאבים ניתנים להזמנה.
author: JohnPBurrows
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 32a04ddef901515cd77262b5ae6be2458cb6b00c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993296"
---
# <a name="how-do-i-assign-a-bookable-resource-to-a-task-in-the-web-app-project-service-app-v2x"></a><span data-ttu-id="9f491-103">כיצד להקצות משאב הניתן להזמנה למשימה ביישום אינטרנט (יישום Project Service גירסה 2.x)?</span><span class="sxs-lookup"><span data-stu-id="9f491-103">How do I assign a bookable resource to a task in the web app (Project Service app v2.x)?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="9f491-104">קיימות שתי דרכים להקצאת משאב למשימה ב- Project Service.</span><span class="sxs-lookup"><span data-stu-id="9f491-104">There are two ways to assign a resource to a task in Project Service.</span></span> <span data-ttu-id="9f491-105">באפשרותך להזמין משאב בתור חבר צוות ולאחר מכן להקצות אותו למשימה.</span><span class="sxs-lookup"><span data-stu-id="9f491-105">You can book a resource as a team member and then assign it to a task.</span></span> <span data-ttu-id="9f491-106">לחלופין, באפשרותך ליצור חבר צוות כללי דרך הקצאת תפקידים במשימות, ליצור צוות, ולאחר מכן למלא את דרישות הגיבוי עם משאב בעל שם.</span><span class="sxs-lookup"><span data-stu-id="9f491-106">Or, you can create a generic team member through role assignment on tasks, generate a team, and then fulfill the backing requirements with a named resource.</span></span>

<span data-ttu-id="9f491-107">שים לב כי אם ברצונך להקצות משאב הניתן להזמנה למשימה, לחבר צוות שמהווה משאב הניתן להזמנה חייבות להיות מספיק הזמנות זמינות.</span><span class="sxs-lookup"><span data-stu-id="9f491-107">Note that if you’d like to assign a bookable resource to a task, the bookable resource team member must have enough available bookings.</span></span> <span data-ttu-id="9f491-108">מצב ההזמנה חייב להיות הזמנה בטוחה‬ מסוג ביצוע ומצב מאושר.</span><span class="sxs-lookup"><span data-stu-id="9f491-108">The status of the booking must be Commit Type Hard Book and Status Committed.</span></span> <span data-ttu-id="9f491-109">אם אין מספיק הזמנות עבור המשאב, Project Service מסיר את ההקצאה ומציג את הודעת השגיאה הבאה:</span><span class="sxs-lookup"><span data-stu-id="9f491-109">If there aren’t enough bookings for the resource, Project Service removes the assignment and displays the following error message:</span></span>

<span data-ttu-id="9f491-110">*אין אפשרות להקצות משאבים למשימה - למשאבים הבאים אין מספיק שעות שהוזמנו כנגד פרוייקט*</span><span class="sxs-lookup"><span data-stu-id="9f491-110">*Unable to assign resource to task - Following resource(s) do not have sufficient hours booked against project*</span></span>

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a><span data-ttu-id="9f491-111">הזמנת משאב בתור חבר צוות ולאחר מכן הקצאת המשאב למשימה</span><span class="sxs-lookup"><span data-stu-id="9f491-111">Book a resource as a team member and then assign the resource to a task</span></span>

<span data-ttu-id="9f491-112">בשיטה זו אתה מוסיף משאב לצוות הפרוייקט ולאחר מכן מקצה משימות למשאב בלוח זמנים של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="9f491-112">With this method you add a resource to the project team and then assign tasks to the resource in the project schedule.</span></span> <span data-ttu-id="9f491-113">הנה כיצד לעשות זאת:</span><span class="sxs-lookup"><span data-stu-id="9f491-113">Here’s how you do this:</span></span>
1.  <span data-ttu-id="9f491-114">ברשת חבר צוות, הוסף חבר צוות חדש על-ידי בחירת **חדש**.</span><span class="sxs-lookup"><span data-stu-id="9f491-114">On the team member grid, add a new team member by selecting **New**.</span></span>
2.  <span data-ttu-id="9f491-115">במסך יצירה מהירה של חבר צוות, בחר את שם המשאב הניתן להזמנה והגדר תפקיד.</span><span class="sxs-lookup"><span data-stu-id="9f491-115">On the Team Member Quick Create screen, select the bookable resource name and set a role.</span></span>
3.  <span data-ttu-id="9f491-116">בחר את התאריכים **מ-** ו **עד**.</span><span class="sxs-lookup"><span data-stu-id="9f491-116">Select the **From** and **To** dates.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="9f491-117">![צילום מסך של הוספת חבר צוות](media/FAQ-Resources-to-Tasks2-1.png "צילום מסך של הוספת חבר צוות")</span><span class="sxs-lookup"><span data-stu-id="9f491-117">![Screenshot of adding team member](media/FAQ-Resources-to-Tasks2-1.png "Screenshot of adding team member")</span></span>
 
4.  <span data-ttu-id="9f491-118">בחר באחת משיטות ההקצאה הבאות להזמנת המשאב:</span><span class="sxs-lookup"><span data-stu-id="9f491-118">Select one of the following allocation methods for booking the resource:</span></span>
    - <span data-ttu-id="9f491-119">**קיבולת מלאה** מזמינה קיבולת מלאה של המשאב עבור התאריכים 'מ' ו'עד' שצוינו.</span><span class="sxs-lookup"><span data-stu-id="9f491-119">**Full Capacity** books the resource’s full capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="9f491-120">**קיבולת באחוזים** מזמינה את המשאב לאחוז הקיבולת של המשאב עבור התאריכים 'מ' ו'עד' שצוינו.</span><span class="sxs-lookup"><span data-stu-id="9f491-120">**Percentage Capacity** books the resource for a percentage of the resource's capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="9f491-121">**‏‫הפצת שעות באופן שווה‬** מזמינה את המשאב למספר מסוים של שעות, ומפיצה את הזמן באופן שווה בכל יום בטווח התאריכים 'מ' ו'עד' שצוינו.</span><span class="sxs-lookup"><span data-stu-id="9f491-121">**By Hours Distribute Evenly** books the resource for a specified number of hours, distributing it evenly per day over the specified from and to dates.</span></span>
    - <span data-ttu-id="9f491-122">**לפי ‏‫שעות עומס חזיתי‬** מזמינה את המשאב למספר מסוים של שעות, ומחלקת את השעות ביום לפי עומס חזיתי בטווח התאריכים 'מ' ו'עד' שצוינו.</span><span class="sxs-lookup"><span data-stu-id="9f491-122">**By Hours Front Load** books the resource for a specified number of hours, front-loading the per-day hours over the specified from and to dates.</span></span>

    <span data-ttu-id="9f491-123">אל תבחר באפשרות **ללא** מפני שהיא מוסיפה את המשאב בתור חבר בצוות הפרוייקט, אך אינה יוצרת הזמנות כלשהן אשר סופגות את קיבולת המשאב.</span><span class="sxs-lookup"><span data-stu-id="9f491-123">Don’t select **None** because it adds the resource to the team but doesn’t create any bookings that absorb the resource's capacity.</span></span>
5.  <span data-ttu-id="9f491-124">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="9f491-124">Select **Save**.</span></span>

    <span data-ttu-id="9f491-125">שים לב כי שעות ההזמנה חייבות להיות מספיקות כדי לכסות את שעות העבודה ואת טווחי התאריכים של משימות שאליהן אתה מקצה משאב זה.</span><span class="sxs-lookup"><span data-stu-id="9f491-125">Note that the hours of the booking must be enough to cover the effort hours and date ranges of the tasks that you assign this resource to.</span></span> <span data-ttu-id="9f491-126">אם אין התאמה ביניהם, אין באפשרותך להקצות את המשאב למשימה.</span><span class="sxs-lookup"><span data-stu-id="9f491-126">If they aren’t in alignment, you can’t assign the resource to the task.</span></span>

6.  <span data-ttu-id="9f491-127">במבנה התפלגות עבודה (WBS) עבור המשימה, לחץ על הרשימה הנפתחת של תאי משאבים.</span><span class="sxs-lookup"><span data-stu-id="9f491-127">On the work breakdown structure (WBS) for the task, click the resource cell dropdown.</span></span> <span data-ttu-id="9f491-128">אז:</span><span class="sxs-lookup"><span data-stu-id="9f491-128">Then:</span></span> 

    1. <span data-ttu-id="9f491-129">בחר **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="9f491-129">Select **Add**.</span></span>
    2. <span data-ttu-id="9f491-130">בחר את הרשימה הנפתחת תחת **משאבים** ובחר את חבר הצוות שהוספת לעיל.</span><span class="sxs-lookup"><span data-stu-id="9f491-130">Select the dropdown under **Resources** and select the team member you added above.</span></span>
    3. <span data-ttu-id="9f491-131">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="9f491-131">Select **OK**.</span></span> <span data-ttu-id="9f491-132">חבר הצוות מוקצה כעת למשימה.</span><span class="sxs-lookup"><span data-stu-id="9f491-132">The team member is now assigned to the task.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="9f491-133">![צילום מסך של הוספת משאבים באמצעות WBS](media/FAQ-Resources-to-Tasks2-2.png "צילום מסך של הוספת משאבים באמצעות WBS")</span><span class="sxs-lookup"><span data-stu-id="9f491-133">![Screenshot of adding resources with WBS](media/FAQ-Resources-to-Tasks2-2.png "Screenshot of adding resources with WBS")</span></span>
 
<span data-ttu-id="9f491-134">ברשת חבר צוות, תראה את הצבירה של שעות העבודה המוקצות למשאב תחת 'שעות שהוקצו'.</span><span class="sxs-lookup"><span data-stu-id="9f491-134">On the team member grid, you’ll see the aggregate of the resource’s assigned hours under Assigned Hours.</span></span> <span data-ttu-id="9f491-135">היא תהיה קטנה או שווה לשעות שהוזמנו עבור המשאב.</span><span class="sxs-lookup"><span data-stu-id="9f491-135">It will be less than or equal to the booked hours for the resource.</span></span> 

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="9f491-136">![צילום מסך של שעות שהוקצו למשאב](media/FAQ-Resources-to-Tasks2-3.png "צילום מסך של שעות שהוקצו למשאב")</span><span class="sxs-lookup"><span data-stu-id="9f491-136">![Screenshot of assigned hours for a resource](media/FAQ-Resources-to-Tasks2-3.png "Screenshot of assigned hours for a resource")</span></span>
 
<span data-ttu-id="9f491-137">אם המשימה שאתה מנסה להקצות למשאב מתחילה לאחר תאריך הסיום של הזמנות משאבים, המשאב לא יופיע ברשימה הנפתחת.</span><span class="sxs-lookup"><span data-stu-id="9f491-137">If the task you’re attempting to assign to the resource starts after the end date of the resources bookings, the resource won’t appear in the dropdown.</span></span>

<span data-ttu-id="9f491-138">שים לב כי באפשרותך להקצות משאב ליותר שעות מהשעות שבהזמנה שלו אם למשאב נותרה עוד קיבולת שלא הוקצתה.</span><span class="sxs-lookup"><span data-stu-id="9f491-138">Note that you can assign a resource to more hours than their booked hours if the resource has some remaining unassigned capacity.</span></span> <span data-ttu-id="9f491-139">במקרה זה המשאב יוקצה באופן חלקי בלבד עד ההזמנות שלו.</span><span class="sxs-lookup"><span data-stu-id="9f491-139">In this case the resource will only be partially assigned up to their bookings.</span></span> <span data-ttu-id="9f491-140">באפשרותך לראות את שעות המשימה הנותרות האלה שלא הוקצו על-ידי הוספת העמודה 'שעות לא מאוישות‬' למבנה התפלגות העבודה.</span><span class="sxs-lookup"><span data-stu-id="9f491-140">You can see these remaining unassigned task hours by adding the Unstaffed Hours column to the work breakdown structure.</span></span>

<span data-ttu-id="9f491-141">אם משאבים מוקצים לשעות ההזמנה שלהם (שעות ההזמנה שלהם שווות לשעות המוקצות שלהם), תראה את הודעת השגיאה הבאה בעת ניסיון להקצות להם עוד משימות:</span><span class="sxs-lookup"><span data-stu-id="9f491-141">If resources are assigned to their booked hours (their booked hours equals their assigned hours), you’ll see the following error message when you attempt to assign them further tasks:</span></span>

<span data-ttu-id="9f491-142">*אין אפשרות להקצות משאב למשימה - למשאבים הבאים אין מספיק שעות שהוזמנו כנגד פרוייקט.*</span><span class="sxs-lookup"><span data-stu-id="9f491-142">*Unable to assign resource to task - Following resource(s) do not have sufficient hours booked against project.*</span></span>

<span data-ttu-id="9f491-143">בנוסף, חבר הצוות שהוא מנהל פרוייקט בברירת המחדל שמתווסף לצוות בעת יצירת הפרוייקט מתווסף ללא כל הזמנות ולא ניתן להקצות אותו לאף משימה.</span><span class="sxs-lookup"><span data-stu-id="9f491-143">Additionally, the default project manager team member that is added to the team when you create the project is added without any bookings and can’t be assigned to any task.</span></span> <span data-ttu-id="9f491-144">הוא לא יוצג ברשימה הנפתחת של משאבים עבור משימות.</span><span class="sxs-lookup"><span data-stu-id="9f491-144">They won’t show up in the resource dropdown for tasks.</span></span>

<span data-ttu-id="9f491-145">אם ברצונך להקצות משאב זה, עליך להסיר אותו מהצוות ולאחר מכן להוסיף אותו מחדש עם שיטת הקצאה שאינה 'ללא'.</span><span class="sxs-lookup"><span data-stu-id="9f491-145">If you want to assign this resource, you need to remove them from the team and then re-add them with an allocation method other than None.</span></span> <span data-ttu-id="9f491-146">הסיבה שהוא מתווסף לצוות בעת יצירת הפרוייקט היא כדי שלפרוייקט יהיה לפחות מאשר פרוייקט אחד כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="9f491-146">The reason they’re added to the team when the project is created is so that a project has at least one project approver by default.</span></span>

## <a name="create-a-generic-team-member-through-role-assignment-on-tasks"></a><span data-ttu-id="9f491-147">יצירת חבר צוות כללי באמצעות הקצאת תפקידים במשימות</span><span class="sxs-lookup"><span data-stu-id="9f491-147">Create a generic team member through role assignment on tasks</span></span>

<span data-ttu-id="9f491-148">שיטה זו מבטיחה שלמשאבים יש מספיק הזמנות עבור משימות.</span><span class="sxs-lookup"><span data-stu-id="9f491-148">This method assures that resources have enough bookings for tasks.</span></span> <span data-ttu-id="9f491-149">תחילה, עליך ליצור מציין מיקום או משאב כללי המתאר את המאפיינים של משאב בעל שם, שברצונך שיעבוד על המשימות, על-ידי יצירת צוות לאחר הקצאת תפקידים למשימות.</span><span class="sxs-lookup"><span data-stu-id="9f491-149">First, you create a placeholder or generic resource that describes the characteristics of the named resource you ultimately want to work on the tasks by generating a team after assigning roles to tasks.</span></span> <span data-ttu-id="9f491-150">הנה כיצד לעשות זאת:</span><span class="sxs-lookup"><span data-stu-id="9f491-150">Here’s how you do this:</span></span>

1. <span data-ttu-id="9f491-151">במבנה התפלגות עבודה, בחר משימה.</span><span class="sxs-lookup"><span data-stu-id="9f491-151">On the work breakdown structure, select a task.</span></span>
2. <span data-ttu-id="9f491-152">בחר בסמל הרשימה הנפתחת **תפקיד מוקצה** בתא המשאב.</span><span class="sxs-lookup"><span data-stu-id="9f491-152">Select the **Assigned Role** dropdown icon in the resource cell.</span></span>
3. <span data-ttu-id="9f491-153">בחר את הרשימה הנפתחת **תפקיד** ובחר את התפקיד עבור המשאב הכללי.</span><span class="sxs-lookup"><span data-stu-id="9f491-153">Select the **Role** dropdown and select the role for the generic resource.</span></span>
4. <span data-ttu-id="9f491-154">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="9f491-154">Select **OK**.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="9f491-155">![צילום מסך של שימוש ב- WBS להוספת משאב](media/FAQ-Resources-to-Tasks2-4.png "צילום מסך של שימוש ב- WBS להוספת משאב")</span><span class="sxs-lookup"><span data-stu-id="9f491-155">![Screenshot of using WBS to add resource](media/FAQ-Resources-to-Tasks2-4.png "Screenshot of using WBS to add resource")</span></span>
 
<span data-ttu-id="9f491-156">לאחר שהשלמת את הקצאת התפקידים למשימות ב- WBS, בחר **צור צוות פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="9f491-156">Once you’ve completed assigning roles to the tasks in the WBS, select **Generate Project Team**.</span></span> <span data-ttu-id="9f491-157">Project Service יוצר את המספר המינימלי של חברי צוות כלליים בהתבסס על התפקידים, יחידות הקצאת משאבים ארגוניות ולוח תאריכים של הפרוייקט על-ידי צבירת הקצאות המשימות.</span><span class="sxs-lookup"><span data-stu-id="9f491-157">Project Service creates the minimum number of generic team members based on the roles, resourcing organization units, and project calendar by aggregating the task assignments.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="9f491-158">![צילום מסך של יצירת צוות פרוייקט](media/FAQ-Resources-to-Tasks2-5.png "צילום מסך של יצירת צוות פרוייקט")</span><span class="sxs-lookup"><span data-stu-id="9f491-158">![Screenshot of generating project team](media/FAQ-Resources-to-Tasks2-5.png "Screenshot of generating project team")</span></span>
 
<span data-ttu-id="9f491-159">ברשת חבר צוות, תראה משאבים מסוג 'משאב כללי' עם שם התפקיד והמיקום.</span><span class="sxs-lookup"><span data-stu-id="9f491-159">On the Team Member grid, you’ll see resources of the Generic Resource type with the role and position name.</span></span> <span data-ttu-id="9f491-160">אם נדרשים שני משאבים עבור תפקיד להשלמת העבודה, התכונה של יצירת צוות יוצרת שני חברי צוות ומשתמשת בשם מיקום כדי להבחין ביניהם.</span><span class="sxs-lookup"><span data-stu-id="9f491-160">If two resources are needed for a role to complete the work, the Generate Team feature creates two team members and uses position name to set them apart.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="9f491-161">![צילום מסך של הוספת שני משאבים כלליים](media/FAQ-Resources-to-Tasks2-6.png "צילום מסך של הוספת שני משאבים כלליים")</span><span class="sxs-lookup"><span data-stu-id="9f491-161">![Screenshot of adding two generic resources](media/FAQ-Resources-to-Tasks2-6.png "Screenshot of adding two generic resources")</span></span>
 
<span data-ttu-id="9f491-162">באפשרותך לפתוח את הדרישה למשאב גיבוי עבור חבר הצוות הכללי על-ידי בחירת הקישור תחת 'דרישת משאב'.</span><span class="sxs-lookup"><span data-stu-id="9f491-162">You can open the backing resource requirement for the generic team member by selecting the link under Resource Requirement.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="9f491-163">![צילום מסך של פתיחת דרישת משאב לגיבוי](media/FAQ-Resources-to-Tasks2-7.png "צילום מסך של פתיחת דרישת משאב לגיבוי")</span><span class="sxs-lookup"><span data-stu-id="9f491-163">![Screenshot of opening backing resource requirement](media/FAQ-Resources-to-Tasks2-7.png "Screenshot of opening backing resource requirement")</span></span>

<span data-ttu-id="9f491-164">בחר **הזמנה** עבור המשאב הכללי, ולאחר מכן תוכל להשתמש בלוח הזמנים כדי למצוא ולהזמין משאב אמיתי.</span><span class="sxs-lookup"><span data-stu-id="9f491-164">Select **Book** for the generic resource, and then you can use the schedule board to find and book a real resource.</span></span> <span data-ttu-id="9f491-165">באפשרותך גם לשלוח את הדרישה למימוש על-ידי מנהל משאבים באמצעות בחירה באפשרות **שלח בקשה**.</span><span class="sxs-lookup"><span data-stu-id="9f491-165">You can also submit the requirement for fulfillment by a resource manager by selecting **Submit Request**.</span></span>

<span data-ttu-id="9f491-166">בעת מימוש משאב כללי עם משאב בעל שם, המשאב הכללי מוסר מהצוות, והקצאות המשימות עבור המשאב הכללי מוקצות למשאב בעל שם שמילא את דרישת המשאב של המשאב הכללי.</span><span class="sxs-lookup"><span data-stu-id="9f491-166">When the generic resource is fulfilled with a named resource, the generic resource is removed from the team and the task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>
 



[!INCLUDE[footer-include](../includes/footer-banner.md)]