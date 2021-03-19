---
title: שינויים בניהול משאבים (Project Service Automation 3.x)
description: נושא זה מספק מידע על השינויים בתחום ניהול המשאבים.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 03/18/2019
ms.topic: article
ms.service: business-applications
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 5f88d7309a5e1171629a72e749bfc01abb64c62a
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5284764"
---
# <a name="resource-management-changes-project-service-automation-3x"></a><span data-ttu-id="13f4d-103">שינויים בניהול משאבים (Project Service Automation 3.x)</span><span class="sxs-lookup"><span data-stu-id="13f4d-103">Resource management changes (Project Service Automation 3.x)</span></span>

[!include [banner](../../includes/psa-now-project-operations.md)]

<span data-ttu-id="13f4d-104">הסעיפים של נושא זה מספקים מידע על השינויים שבוצעו בתחום ניהול המשאבים של Dynamics 365 Project Service Automation גירסה ‎3.x.</span><span class="sxs-lookup"><span data-stu-id="13f4d-104">The sections of this topic provide information about the changes that have been made to the Resource management area of Dynamics 365 Project Service Automation version 3.x.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="13f4d-105">הערכות פרויקט</span><span class="sxs-lookup"><span data-stu-id="13f4d-105">Project estimates</span></span>

<span data-ttu-id="13f4d-106">במקום להתבסס על הישות **msdyn\_projecttask** (**משימת פרויקט‬**), הערכות הפרויקט מבוססות על הישות **msdyn\_resourceassignment** (**הקצאת משאבים‬**).</span><span class="sxs-lookup"><span data-stu-id="13f4d-106">Instead of being based on the **msdyn\_projecttask** entity (**Project Task**), project estimates are based on the **msdyn\_resourceassignment** entity (**Resource Assignment**).</span></span> <span data-ttu-id="13f4d-107">הקצאות המשאבים הפכו ל"מקור אמת" לתזמון ולתמחור של משימות.</span><span class="sxs-lookup"><span data-stu-id="13f4d-107">Resource assignments have become the "source of truth" for task scheduling and pricing.</span></span>

## <a name="line-tasks"></a><span data-ttu-id="13f4d-108">משימות שורה</span><span class="sxs-lookup"><span data-stu-id="13f4d-108">Line tasks</span></span>

<span data-ttu-id="13f4d-109">ב- PSA 3.x, משימות שורה הן מיושנות (לא בשימוש).</span><span class="sxs-lookup"><span data-stu-id="13f4d-109">In PSA 3.x, line tasks are obsolete (deprecated).</span></span> <span data-ttu-id="13f4d-110">ההקצאות מצביעות כעת על המשימה כולה, במקום על משימות השורה.</span><span class="sxs-lookup"><span data-stu-id="13f4d-110">Assignments now point to the whole task instead of the line tasks.</span></span>

<span data-ttu-id="13f4d-111">הדוגמה הבאה מראה כיצד משימה ששמה "משימת בדיקה" מוקצית לחברי הצוות A ו- B בגירסאות קודמות של PSA וב-PSA 3.x.</span><span class="sxs-lookup"><span data-stu-id="13f4d-111">The following example shows how a task that is named "Test task" is assigned to team members A and B in earlier versions of PSA and in PSA 3.x.</span></span>

- <span data-ttu-id="13f4d-112">**לפני PSA 3.x:**</span><span class="sxs-lookup"><span data-stu-id="13f4d-112">**Before PSA 3.x:**</span></span>

    - <span data-ttu-id="13f4d-113">משימת בדיקה</span><span class="sxs-lookup"><span data-stu-id="13f4d-113">Test task</span></span>

        - <span data-ttu-id="13f4d-114">משימת בדיקה - משימת שורה 1</span><span class="sxs-lookup"><span data-stu-id="13f4d-114">Test task – Line task 1</span></span>

            - <span data-ttu-id="13f4d-115">הקצאה ל- A</span><span class="sxs-lookup"><span data-stu-id="13f4d-115">Assignment to A</span></span>

        - <span data-ttu-id="13f4d-116">משימת בדיקה - משימת שורה 2</span><span class="sxs-lookup"><span data-stu-id="13f4d-116">Test task – Line task 2</span></span>

            - <span data-ttu-id="13f4d-117">הקצאה ל- B</span><span class="sxs-lookup"><span data-stu-id="13f4d-117">Assignment to B</span></span>

- <span data-ttu-id="13f4d-118">**PSA 3.x:**</span><span class="sxs-lookup"><span data-stu-id="13f4d-118">**PSA 3.x:**</span></span>

    - <span data-ttu-id="13f4d-119">משימת בדיקה</span><span class="sxs-lookup"><span data-stu-id="13f4d-119">Test task</span></span>

        - <span data-ttu-id="13f4d-120">הקצאה ל- A</span><span class="sxs-lookup"><span data-stu-id="13f4d-120">Assignment to A</span></span>
        - <span data-ttu-id="13f4d-121">הקצאה ל- B</span><span class="sxs-lookup"><span data-stu-id="13f4d-121">Assignment to B</span></span>

## <a name="unassigned-assignment"></a><span data-ttu-id="13f4d-122">הקצאה לא מוקצית</span><span class="sxs-lookup"><span data-stu-id="13f4d-122">Unassigned assignment</span></span>

<span data-ttu-id="13f4d-123">ב- PSA 3.x, הקצאה לא מוקצית היא הקצאה המוקצית לחבר צוות **NULL** ולמשאב **NULL**.</span><span class="sxs-lookup"><span data-stu-id="13f4d-123">In PSA 3.x, an unassigned assignment is an assignment that is assigned to a **NULL** team member and a **NULL** resource.</span></span> <span data-ttu-id="13f4d-124">הקצאות לא מוקצות יכולות להתרחש במספר תרחישים:</span><span class="sxs-lookup"><span data-stu-id="13f4d-124">Unassigned assignments can occur in a couple of scenarios:</span></span>

- <span data-ttu-id="13f4d-125">אם נוצרה משימה, אך היא עדיין לא הוקצתה לאף חבר צוות, נוצרת תמיד הקצאה לא מוקצית.</span><span class="sxs-lookup"><span data-stu-id="13f4d-125">If a task has been created, but it hasn't yet been assigned to any team member, an unassigned assignment is always created.</span></span> 
- <span data-ttu-id="13f4d-126">אם הוסרו כל מקבלי ההקצאות במשימה, הקצאה לא מוקצית נוצרת מחדש עבור אותה משימה.</span><span class="sxs-lookup"><span data-stu-id="13f4d-126">If all assignees on a task are removed, an unassigned assignment is re-created for that task.</span></span>

## <a name="scheduling-fields-on-the-project-task-entity"></a><span data-ttu-id="13f4d-127">תזמון שדות בישות 'משימת פרויקט'</span><span class="sxs-lookup"><span data-stu-id="13f4d-127">Scheduling fields on the Project Task entity</span></span>

<span data-ttu-id="13f4d-128">השדות בישות **msdyn\_projecttask** הוצאו משימוש או הועברו לישות **msdyn\_resourceassignment**, או שכעת מתבצעת אליהם הפניה מהישות **msdyn\_projectteam** (**חבר צוות פרויקט**).</span><span class="sxs-lookup"><span data-stu-id="13f4d-128">The fields on the **msdyn\_projecttask** entity have been deprecated or moved to the **msdyn\_resourceassignment** entity, or they are now referenced from the **msdyn\_projectteam** entity (**Project Team Member**).</span></span>

| <span data-ttu-id="13f4d-129">שדה לא בשימוש ב- msdyn\_projecttask (משימת פרויקט)</span><span class="sxs-lookup"><span data-stu-id="13f4d-129">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="13f4d-130">שדה חדש ב- msdyn\_resourceassignment (הקצאת משאבים)</span><span class="sxs-lookup"><span data-stu-id="13f4d-130">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> | <span data-ttu-id="13f4d-131">הערה</span><span class="sxs-lookup"><span data-stu-id="13f4d-131">Comment</span></span> |
|---|---|---|
| <span data-ttu-id="13f4d-132">msdyn\_assignedresources</span><span class="sxs-lookup"><span data-stu-id="13f4d-132">msdyn\_assignedresources</span></span> | <span data-ttu-id="13f4d-133">ללא</span><span class="sxs-lookup"><span data-stu-id="13f4d-133">None</span></span> | |
| <span data-ttu-id="13f4d-134">msdyn\_assignedteammembers</span><span class="sxs-lookup"><span data-stu-id="13f4d-134">msdyn\_assignedteammembers</span></span> | <span data-ttu-id="13f4d-135">ללא</span><span class="sxs-lookup"><span data-stu-id="13f4d-135">None</span></span> | |
| <span data-ttu-id="13f4d-136">msdyn\_numberofresources</span><span class="sxs-lookup"><span data-stu-id="13f4d-136">msdyn\_numberofresources</span></span> | <span data-ttu-id="13f4d-137">ללא</span><span class="sxs-lookup"><span data-stu-id="13f4d-137">None</span></span> | |
| <span data-ttu-id="13f4d-138">msdyn\_scheduledhours</span><span class="sxs-lookup"><span data-stu-id="13f4d-138">msdyn\_scheduledhours</span></span> | <span data-ttu-id="13f4d-139">ללא</span><span class="sxs-lookup"><span data-stu-id="13f4d-139">None</span></span> | |
| <span data-ttu-id="13f4d-140">msdyn\_effortcontour</span><span class="sxs-lookup"><span data-stu-id="13f4d-140">msdyn\_effortcontour</span></span> | <span data-ttu-id="13f4d-141">msdyn\_plannedwork</span><span class="sxs-lookup"><span data-stu-id="13f4d-141">msdyn\_plannedwork</span></span> | <span data-ttu-id="13f4d-142">התבנית של מבנה הנתונים JavaScript Object Notation ‏(JSON) המאוחסן בשדה שונתה.</span><span class="sxs-lookup"><span data-stu-id="13f4d-142">The format of the JavaScript Object Notation (JSON) data structure that is stored in the field has been changed.</span></span> |

## <a name="schedule-contour"></a><span data-ttu-id="13f4d-143">מתאר לוח זמנים</span><span class="sxs-lookup"><span data-stu-id="13f4d-143">Schedule contour</span></span>

<span data-ttu-id="13f4d-144">מתאר לוח הזמנים מאוחסן בשדה **עבודה מתוכננת‬** (**msdyn\_plannedwork**) של כל ישות **הקצאת משאבים** (**msdyn\_resourceassignment**).</span><span class="sxs-lookup"><span data-stu-id="13f4d-144">The schedule contour is stored in the **Planned Work** field (**msdyn\_plannedwork**) of each **Resource Assignment** entity (**msdyn\_resourceassignment**).</span></span>

### <a name="structure"></a><span data-ttu-id="13f4d-145">מבנה</span><span class="sxs-lookup"><span data-stu-id="13f4d-145">Structure</span></span>

<span data-ttu-id="13f4d-146">המבנה החדש של מתאר לוח הזמנים מורכב מפרוסות זמן גמישות המוגדרות עבור כל יום בלוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="13f4d-146">The new structure of the schedule contour consists of flexible time slices that are defined for each day of the schedule.</span></span> <span data-ttu-id="13f4d-147">כל פרוסת זמן כוללת את המאפיינים הבאים:</span><span class="sxs-lookup"><span data-stu-id="13f4d-147">Each time slice has the following properties:</span></span>

- <span data-ttu-id="13f4d-148">**התחלה** - תחילת שעות העבודה באותו יום, לפי לוח השנה של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="13f4d-148">**Start** – The start of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="13f4d-149">**סיום** - סיום שעות העבודה באותו יום, לפי לוח השנה של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="13f4d-149">**End** – The end of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="13f4d-150">**שעות** - מספר השעות המוקצות ביום.</span><span class="sxs-lookup"><span data-stu-id="13f4d-150">**Hours** – The number of hours that are assigned on the day.</span></span>

<span data-ttu-id="13f4d-151">**דוגמה**</span><span class="sxs-lookup"><span data-stu-id="13f4d-151">**Example**</span></span>

<span data-ttu-id="13f4d-152">דוגמה זו משתמשת בלוח שנה של פרויקט שבו יום העבודה מתקיים בין השעות 09:00 ל- 17:00 באזור הזמן UTC-8.</span><span class="sxs-lookup"><span data-stu-id="13f4d-152">This example uses a project calendar where the workday is from 9 AM to 5 PM in the UTC-8 time zone.</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

### <a name="auto-scheduling-and-manual-scheduling"></a><span data-ttu-id="13f4d-153">תזמון אוטומטי ותזמון ידני</span><span class="sxs-lookup"><span data-stu-id="13f4d-153">Auto-scheduling and manual scheduling</span></span>

<span data-ttu-id="13f4d-154">אם משימה מתוזמנת באופן אוטומטי, השעות נטענות מראש וייתכן שמשך המשימה יתקצר.</span><span class="sxs-lookup"><span data-stu-id="13f4d-154">If a task is auto-scheduled, the hours are front-loaded, and the task duration might be reduced.</span></span>

<span data-ttu-id="13f4d-155">**דוגמה**</span><span class="sxs-lookup"><span data-stu-id="13f4d-155">**Example**</span></span>

<span data-ttu-id="13f4d-156">המשימה הבאה מתוזמנת באופן אוטומטי במשך 18 שעות על-פני שלושה ימים (3 בדצמבר 2018 עד 5 בדצמבר 2018).</span><span class="sxs-lookup"><span data-stu-id="13f4d-156">The following task is auto-scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

<span data-ttu-id="13f4d-157">אם משימה מתוזמנת באופן ידני, השעות מתחלקות באופן שווה בין כל התאריכים.</span><span class="sxs-lookup"><span data-stu-id="13f4d-157">If a task is manually scheduled, the hours are evenly distributed to all the dates.</span></span>

<span data-ttu-id="13f4d-158">**דוגמה**</span><span class="sxs-lookup"><span data-stu-id="13f4d-158">**Example**</span></span>

<span data-ttu-id="13f4d-159">המשימה הבאה מתוזמנת באופן ידני במשך 18 שעות על-פני שלושה ימים (3 בדצמבר 2018 עד 5 בדצמבר 2018).</span><span class="sxs-lookup"><span data-stu-id="13f4d-159">The following task is manually scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":6},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":6},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":6}]
```

### <a name="assignment-unit"></a><span data-ttu-id="13f4d-160">יחידת הקצאה</span><span class="sxs-lookup"><span data-stu-id="13f4d-160">Assignment unit</span></span>

<span data-ttu-id="13f4d-161">יחידת ההקצאה הוצאה משימוש ב- PSA 3.x.</span><span class="sxs-lookup"><span data-stu-id="13f4d-161">The assignment unit has been deprecated in PSA 3.x.</span></span> <span data-ttu-id="13f4d-162">שעות המאמץ הדרושות למשימה מחולקות כעת באופן שווה, לכל יום, בין כל המשאבים שהוקצו.</span><span class="sxs-lookup"><span data-stu-id="13f4d-162">The task effort hours are now equally divided, per day, among all the assigned resources.</span></span>

<span data-ttu-id="13f4d-163">**דוגמה**</span><span class="sxs-lookup"><span data-stu-id="13f4d-163">**Example**</span></span>

<span data-ttu-id="13f4d-164">בדוגמה זו, המשימה מוקצית לשני משאבים ומתוזמנת באופן אוטומטי עבור 36 שעות על-פני שלושה ימים (3 בדצמבר 2018 עד 5 בדצמבר 2018).</span><span class="sxs-lookup"><span data-stu-id="13f4d-164">In this example, the task is is assigned to two resources and is auto-scheduled for 36 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

- <span data-ttu-id="13f4d-165">הקצאה 1:</span><span class="sxs-lookup"><span data-stu-id="13f4d-165">Assignment 1:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

- <span data-ttu-id="13f4d-166">הקצאה 2:</span><span class="sxs-lookup"><span data-stu-id="13f4d-166">Assignment 2:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

## <a name="pricing-dimensions"></a><span data-ttu-id="13f4d-167">ממדי תמחור</span><span class="sxs-lookup"><span data-stu-id="13f4d-167">Pricing dimensions</span></span>

<span data-ttu-id="13f4d-168">ב- PSA 3.x, שדות ממד תמחור ספציפיים למשאבים (כגון **תפקיד** ו **יחידה ארגונית**) הוסרו מהישות **msdyn‎\_projecttask‎**.</span><span class="sxs-lookup"><span data-stu-id="13f4d-168">In PSA 3.x, resource-specific pricing dimension fields (such as **Role** and **Organizational Unit**) have been removed from the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="13f4d-169">כעת ניתן לאחזר שדות אלה מחבר צוות הפרויקט המתאים (**msdyn\_projectteam**) של הקצאת המשאב (**msdyn\_resourceassignment**) כאשר הערכות הפרויקט נוצרות.</span><span class="sxs-lookup"><span data-stu-id="13f4d-169">These fields can now be retrieved from the corresponding project team member (**msdyn\_projectteam**) of the resource assignment (**msdyn\_resourceassignment**) when project estimates are generated.</span></span> <span data-ttu-id="13f4d-170">שדה חדש, **msdyn\_organizationalunit**, נוסף לישות **msdyn\_projectteam**.</span><span class="sxs-lookup"><span data-stu-id="13f4d-170">A new field, **msdyn\_organizationalunit**, has been added to the **msdyn\_projectteam** entity.</span></span>

| <span data-ttu-id="13f4d-171">שדה לא בשימוש ב- msdyn\_projecttask (משימת פרויקט)</span><span class="sxs-lookup"><span data-stu-id="13f4d-171">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="13f4d-172">שדה מ- msdyn\_projectteam (חבר צוות פרויקט) המשמש במקום זאת</span><span class="sxs-lookup"><span data-stu-id="13f4d-172">Field from msdyn\_projectteam (Project Team Member) that is used instead</span></span> |
|---|---|
| <span data-ttu-id="13f4d-173">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="13f4d-173">msdyn\_resourcecategory</span></span> | <span data-ttu-id="13f4d-174">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="13f4d-174">msdyn\_resourcecategory</span></span> |
| <span data-ttu-id="13f4d-175">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="13f4d-175">msdyn\_organizationalunit</span></span> | <span data-ttu-id="13f4d-176">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="13f4d-176">msdyn\_organizationalunit</span></span> |

## <a name="contours"></a><span data-ttu-id="13f4d-177">מתארים</span><span class="sxs-lookup"><span data-stu-id="13f4d-177">Contours</span></span>

<span data-ttu-id="13f4d-178">שדות המתאר של התמחור וההערכה הוצאו משימוש בישות **msdyn\_projecttask**.</span><span class="sxs-lookup"><span data-stu-id="13f4d-178">The pricing and estimation contour fields have been deprecated on the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="13f4d-179">הם הועברו לישות **msdyn\_resourceassignment**.</span><span class="sxs-lookup"><span data-stu-id="13f4d-179">They have been moved to the **msdyn\_resourceassignment** entity.</span></span>

| <span data-ttu-id="13f4d-180">שדה לא בשימוש ב- msdyn\_projecttask (משימת פרויקט)</span><span class="sxs-lookup"><span data-stu-id="13f4d-180">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="13f4d-181">שדה חדש ב- msdyn\_resourceassignment (הקצאת משאבים)</span><span class="sxs-lookup"><span data-stu-id="13f4d-181">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> |
|---|---|
| <span data-ttu-id="13f4d-182">msdyn\_costestimatecontour</span><span class="sxs-lookup"><span data-stu-id="13f4d-182">msdyn\_costestimatecontour</span></span> | <span data-ttu-id="13f4d-183">msdyn\_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="13f4d-183">msdyn\_plannedcostcontour</span></span> |
| <span data-ttu-id="13f4d-184">msdyn\_salesestimatecontour</span><span class="sxs-lookup"><span data-stu-id="13f4d-184">msdyn\_salesestimatecontour</span></span> | <span data-ttu-id="13f4d-185">msdyn\_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="13f4d-185">msdyn\_plannedsalescontour</span></span> |

<span data-ttu-id="13f4d-186">השדות הבאים נוספו לישות **msdyn\_resourceassignment**:</span><span class="sxs-lookup"><span data-stu-id="13f4d-186">The following fields have been added to the **msdyn\_resourceassignment** entity:</span></span>

* <span data-ttu-id="13f4d-187">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="13f4d-187">msdyn\_plannedcost</span></span>
* <span data-ttu-id="13f4d-188">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="13f4d-188">msdyn\_plannedsales</span></span>

<span data-ttu-id="13f4d-189">השדות הבאים עבור עלות ומכירות 'מתוכננות', 'בפועל' ו'נותרו' לא השתנו בישות **msdyn\_projecttask**:</span><span class="sxs-lookup"><span data-stu-id="13f4d-189">The following fields for planned, actual, and remaining cost and sales are unchanged on the **msdyn\_projecttask** entity:</span></span>

* <span data-ttu-id="13f4d-190">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="13f4d-190">msdyn\_plannedcost</span></span>
* <span data-ttu-id="13f4d-191">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="13f4d-191">msdyn\_plannedsales</span></span>
* <span data-ttu-id="13f4d-192">msdyn\_actualcost</span><span class="sxs-lookup"><span data-stu-id="13f4d-192">msdyn\_actualcost</span></span>
* <span data-ttu-id="13f4d-193">msdyn\_actualsales</span><span class="sxs-lookup"><span data-stu-id="13f4d-193">msdyn\_actualsales</span></span>
* <span data-ttu-id="13f4d-194">msdyn\_remainingcost</span><span class="sxs-lookup"><span data-stu-id="13f4d-194">msdyn\_remainingcost</span></span>
* <span data-ttu-id="13f4d-195">msdyn\_remainingsales</span><span class="sxs-lookup"><span data-stu-id="13f4d-195">msdyn\_remainingsales</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]