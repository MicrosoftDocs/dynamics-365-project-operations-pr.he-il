---
title: יצירת מבנה התפלגות עבודה
description: נושא זה מסביר כיצד ליצור מבנה התפלגות עבודה (WBS) כולל הפקדים הבסיסיים בממשק התזמון החדש.
author: ruhercul
manager: tfehr
ms.date: 01/07/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: d7fa645e78d2206e333d9f85fcec0f7a9c213c23
ms.sourcegitcommit: 260ce052fed760bb44c514517806049ca13a5459
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 01/08/2021
ms.locfileid: "4841346"
---
# <a name="create-a-work-breakdown-structure-wbs"></a><span data-ttu-id="bcc44-103">יצירת מבנה התפלגות עבודה (WBS)</span><span class="sxs-lookup"><span data-stu-id="bcc44-103">Create a work breakdown structure (WBS)</span></span>

<span data-ttu-id="bcc44-104">לוח הזמנים של הפרוייקט מציג את המטלות שיש להשלים, אילו משאבים יבצעו את העבודה ואת מסגרת הזמן שבה יש להשלים את העבודה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-104">A project schedule communicates what work must be completed, which resources will do the work, and the timeframe in which the work must be completed.</span></span> <span data-ttu-id="bcc44-105">לוח הזמנים משקף את כל העבודה הקשורה למסירת הפרוייקט בזמן.</span><span class="sxs-lookup"><span data-stu-id="bcc44-105">The schedule reflects all the work associated with delivering the project on time.</span></span> <span data-ttu-id="bcc44-106">ב- Dynamics 365 Project Operations, אתה יוצר לוח זמנים של פרוייקט על ידי:</span><span class="sxs-lookup"><span data-stu-id="bcc44-106">In Dynamics 365 Project Operations, you create a project schedule by:</span></span>

  - <span data-ttu-id="bcc44-107">חלוקת העבודה למשימות הניתנות לניהול.</span><span class="sxs-lookup"><span data-stu-id="bcc44-107">Breaking the work down into manageable tasks.</span></span>
  - <span data-ttu-id="bcc44-108">הערכת הזמן הנדרש לביצוע כל משימה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-108">Estimating the time that is required to do each task.</span></span>
  - <span data-ttu-id="bcc44-109">הגדרת ‏‫יחסי תלות של משימות.</span><span class="sxs-lookup"><span data-stu-id="bcc44-109">Setting task dependencies.</span></span>
  - <span data-ttu-id="bcc44-110">קביעת משכי זמן למשימה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-110">Setting task durations.</span></span>
  - <span data-ttu-id="bcc44-111">הערכת המשאבים הגנריים שיעשו את המשימות.</span><span class="sxs-lookup"><span data-stu-id="bcc44-111">Estimating the generic resources that will do the tasks.</span></span> 

<span data-ttu-id="bcc44-112">לוח זמנים של פרוייקט נוצר בכרטיסיה **לוח זמנים** בדף **פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="bcc44-112">The project schedule is created on the **Schedule** tab on the **Project** page.</span></span>

## <a name="tasks"></a><span data-ttu-id="bcc44-113">משימות</span><span class="sxs-lookup"><span data-stu-id="bcc44-113">Tasks</span></span>

<span data-ttu-id="bcc44-114">השלב הראשון ביצירת לוח זמנים של פרויקט הוא פירוק העבודה לחלקים הניתנים לניהול.</span><span class="sxs-lookup"><span data-stu-id="bcc44-114">The first step in creating a project schedule is to break the work down into manageable portions.</span></span> <span data-ttu-id="bcc44-115">לוח הזמנים ב- Project Operations תומך בתכונות הבאות:</span><span class="sxs-lookup"><span data-stu-id="bcc44-115">The schedule in Project Operations supports the following features:</span></span>

- <span data-ttu-id="bcc44-116">משימות סיכום או גורם מכיל.</span><span class="sxs-lookup"><span data-stu-id="bcc44-116">Summary or container tasks</span></span>
- <span data-ttu-id="bcc44-117">משימות צומת עלה</span><span class="sxs-lookup"><span data-stu-id="bcc44-117">Leaf node tasks</span></span>

### <a name="summary-tasks"></a><span data-ttu-id="bcc44-118">משימות סיכום</span><span class="sxs-lookup"><span data-stu-id="bcc44-118">Summary tasks</span></span>

<span data-ttu-id="bcc44-119">משימות סיכום יכולות לאחסן משימות סיכום אחרות או משימות של צומת עלה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-119">Summary tasks can store other summary tasks or leaf node tasks.</span></span> <span data-ttu-id="bcc44-120">אין להן מאמץ עבודה או עלות משלהן.</span><span class="sxs-lookup"><span data-stu-id="bcc44-120">They have no work effort or cost of their own.</span></span> <span data-ttu-id="bcc44-121">במקום זאת, מאמצי העבודה והעלות שלהן הם סיכום של מאמץ העבודה והעלות של המשימות של הגורמים המכילים שלהן.</span><span class="sxs-lookup"><span data-stu-id="bcc44-121">Instead, their work effort and cost are a rollup of the work effort and cost of their container tasks.</span></span> <span data-ttu-id="bcc44-122">תאריך ההתחלה של פעילות הערסל הוא תאריך ההתחלה של פעילויות הגורמים המכילים, ותאריך הסיום הוא תאריך הסיום של פעילויות הגורמים המכילים.</span><span class="sxs-lookup"><span data-stu-id="bcc44-122">The start date of the summary task is the start date of the container tasks, and the end date is the end date of the container tasks.</span></span> <span data-ttu-id="bcc44-123">ניתן לערוך את שם פעילות הערסל, אך לא ניתן לערוך את מאפייני התזמון, כולל מאמץ, תאריכים ומשך זמן.</span><span class="sxs-lookup"><span data-stu-id="bcc44-123">The name of a summary task can be edited, but scheduling properties, including effort, dates, and duration, can't be edited.</span></span> <span data-ttu-id="bcc44-124">אם תמחק פעילות ערסל, תמחק גם את כל משימות הגורמים המכילים שלה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-124">If you delete a summary task, you also delete all its container tasks.</span></span>

### <a name="leaf-node-tasks"></a><span data-ttu-id="bcc44-125">משימות צומת עלה</span><span class="sxs-lookup"><span data-stu-id="bcc44-125">Leaf node tasks</span></span>

<span data-ttu-id="bcc44-126">משימות של צומת עלה מייצגות את העבודה המפורטת ביותר בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="bcc44-126">Leaf node tasks represent the most granular work on the project.</span></span> <span data-ttu-id="bcc44-127">יש להן הערכות של המאמץ, המשאבים, תאריכי התחלה וסיום מתוכננים ומשך הזמן.</span><span class="sxs-lookup"><span data-stu-id="bcc44-127">They have an estimated effort, resources, planned start and end dates, and a duration.</span></span>

## <a name="create-a-task-hierarchy"></a><span data-ttu-id="bcc44-128">יצירת הירארכיית פעילות</span><span class="sxs-lookup"><span data-stu-id="bcc44-128">Create a task hierarchy</span></span>

### <a name="add-a-task"></a><span data-ttu-id="bcc44-129">הוסף משימה</span><span class="sxs-lookup"><span data-stu-id="bcc44-129">Add a task</span></span>

<span data-ttu-id="bcc44-130">כדי להוסיף משימה אחת לפחות יש לבצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="bcc44-130">Complete the following steps to add one or more tasks.</span></span>

1. <span data-ttu-id="bcc44-131">עבור אל **פרוייקטים** ובחר ופתח את רשומת הפרוייקט שעבורה ברצונך ליצור לוח זמנים.</span><span class="sxs-lookup"><span data-stu-id="bcc44-131">Go to **Projects** and select and open the project record for which you want to create a schedule.</span></span> 
2. <span data-ttu-id="bcc44-132">בחר בכרטיסיה **משימות**.</span><span class="sxs-lookup"><span data-stu-id="bcc44-132">Select the **Tasks** tab.</span></span> 
3. <span data-ttu-id="bcc44-133">בחר **הוסף משימה חדשה**, הזן שם למשימה ולאחר מכן הקש Enter.</span><span class="sxs-lookup"><span data-stu-id="bcc44-133">Select **Add new task**, enter a name for the task, and then press Enter.</span></span>
2. <span data-ttu-id="bcc44-134">הזן שם משימה אחר ולחץ שוב על Enter עד שתהיה לך רשימה מלאה של משימות.</span><span class="sxs-lookup"><span data-stu-id="bcc44-134">Enter another task name and press Enter again until you have a full list of tasks.</span></span>

### <a name="manage-hierarchy-of-a-task"></a><span data-ttu-id="bcc44-135">נהל הירארכיה של משימה</span><span class="sxs-lookup"><span data-stu-id="bcc44-135">Manage hierarchy of a task</span></span>

<span data-ttu-id="bcc44-136">כאשר פעילות מוסטת פנימה, היא הופכת לצאצא של הפעילות הנמצאת ישירות מעליה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-136">When a task is indented, it becomes a child of the task that is directly above it.</span></span> <span data-ttu-id="bcc44-137">מזהה לוח הזמנים של הפעילות מחושב מחדש כך שהוא מבוסס על מזהה לוח הזמנים של האב החדש שלו ופועל לפי סכימת מספור המיתאר.</span><span class="sxs-lookup"><span data-stu-id="bcc44-137">The schedule ID of the task is then recalculated so that it's based on the schedule ID of its new parent and follows the outline numbering scheme.</span></span> <span data-ttu-id="bcc44-138">משימת ההורה היא כעת משימת סיכום.</span><span class="sxs-lookup"><span data-stu-id="bcc44-138">The parent task is now a summary task.</span></span> <span data-ttu-id="bcc44-139">לכן, היא הופכת לסיכום של משימות הצאצא שלה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-139">Therefore, it becomes a rollup of its child tasks.</span></span> <span data-ttu-id="bcc44-140">כאשר מקדמים פעילות, היא כבר לא צאצא של הפעילות שהיתה האב שלה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-140">When a task is promoted, it's no longer a child of the task that was its parent.</span></span> <span data-ttu-id="bcc44-141">מזהה לוח הזמנים מחושב מחדש כך שהוא ישקף את המיקום והעומק המעודכנים של הפעילות בהירארכיה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-141">The schedule ID is then recalculated so that it reflects the task's updated depth and position in the hierarchy.</span></span> <span data-ttu-id="bcc44-142">המאמץ, העלות והתאריכים של פעילות האב הקודמת מחושבים מחדש כך שלא יכללו בפעילות זו.</span><span class="sxs-lookup"><span data-stu-id="bcc44-142">The effort, cost, and dates of the previous parent task are recalculated so that they don't include this task.</span></span>

<span data-ttu-id="bcc44-143">כדי להזיז או לקדם משימה יש לבצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="bcc44-143">Complete the following steps to indent or promote a task.</span></span>

1. <span data-ttu-id="bcc44-144">בדף **פרוייקט**, בכרטיסיה **משימות**, תחת **משימות סיכום**, בחר את סמל שלוש הנקודות האנכיות לפי שם המשימה, ואז בחר **הפוך למשימת משנה**.</span><span class="sxs-lookup"><span data-stu-id="bcc44-144">On the **Project** page, on the **Tasks** tab, under **Summary tasks**, select the three vertical dots by the task name, and then select **Make subtask**.</span></span> 
2. <span data-ttu-id="bcc44-145">בחר במשימה להזזה או לקידום.</span><span class="sxs-lookup"><span data-stu-id="bcc44-145">Select the task to indent or promote.</span></span> <span data-ttu-id="bcc44-146">לבחירת יותר ממשימה אחת, בחר משימה, לחץ והחזק את מקש Ctrl ולאחר מכן בחר משימות אחרות.</span><span class="sxs-lookup"><span data-stu-id="bcc44-146">To select more than one task, select a task, press and hold Ctrl, and then select additional tasks.</span></span>
2. <span data-ttu-id="bcc44-147">בחר **‏‫הסט פנימה** או **קדם משימת משנה** כדי להעביר משימות מתחת למשימות סיכום או מחוץ להם.</span><span class="sxs-lookup"><span data-stu-id="bcc44-147">Select **Indent** or **Promote subtask**  to move tasks under or out from under summary tasks.</span></span>

### <a name="move-tasks-up-and-down"></a><span data-ttu-id="bcc44-148">הזזת משימות למעלה ולמטה</span><span class="sxs-lookup"><span data-stu-id="bcc44-148">Move tasks up and down</span></span>

<span data-ttu-id="bcc44-149">משימות יכולות לעבור לכל רמה במבנה התפלגות העבודה באחת משתי דרכים:</span><span class="sxs-lookup"><span data-stu-id="bcc44-149">Tasks can me moved to any level in the work breakdown structure in one of two ways:</span></span>

- <span data-ttu-id="bcc44-150">בחר משימות נוספות וגרור אותן למיקום הרצוי.</span><span class="sxs-lookup"><span data-stu-id="bcc44-150">Select one more tasks and drag them to the desired location.</span></span>
- <span data-ttu-id="bcc44-151">בחר מטלה אחת או יותר, לחץ באמצעות לחצן העכבר הימני ובחר **גזירה**, בחר בתא היעד בלוח הזמנים, ואז לחץ באמצעות לחצן העכבר הימני ובחר **הדבק**.</span><span class="sxs-lookup"><span data-stu-id="bcc44-151">Select one or more tasks, right-click and select **Cut**, select the destination cell in the schedule, and then right-click and select **Paste**.</span></span>

## <a name="task-attributes"></a><span data-ttu-id="bcc44-152">תכונות המשימה</span><span class="sxs-lookup"><span data-stu-id="bcc44-152">Task attributes</span></span>

<span data-ttu-id="bcc44-153">שם המשימה מתאר את העבודה שיש להשלים.</span><span class="sxs-lookup"><span data-stu-id="bcc44-153">A task's name describes the work that must be completed.</span></span> <span data-ttu-id="bcc44-154">ב- Project Operations, התכונות המשויכות לפעילות מתארות את לוח הזמנים של הפעילות ואת הדרישות של האיוש.</span><span class="sxs-lookup"><span data-stu-id="bcc44-154">In Project Operations, the attributes associated with a task describe the schedule of the task and its staffing requirements.</span></span>

## <a name="schedule-attributes"></a><span data-ttu-id="bcc44-155">תכונות של לוח זמנים</span><span class="sxs-lookup"><span data-stu-id="bcc44-155">Schedule attributes</span></span>

<span data-ttu-id="bcc44-156">התכונות **מאמץ**, **תאריך התחלה**, **תאריך סיום** ו **משך** מגדירות את לוח הזמנים של המשימה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-156">The **Effort**, **Start date**, **End date**, and **Duration** attributes define the schedule for the task.</span></span>

<span data-ttu-id="bcc44-157">הטבלה הבאה מציגה מאפייני לוח זמנים נוספים.</span><span class="sxs-lookup"><span data-stu-id="bcc44-157">The following table shows additional schedule attributes.</span></span>

| <span data-ttu-id="bcc44-158">**שם תצוגה סופי**</span><span class="sxs-lookup"><span data-stu-id="bcc44-158">**Final display name**</span></span> | <span data-ttu-id="bcc44-159">**תיאור סופי**</span><span class="sxs-lookup"><span data-stu-id="bcc44-159">**Final description**</span></span> |
| --- | --- |
| <span data-ttu-id="bcc44-160">מאמץ שהושלם (בשעות)</span><span class="sxs-lookup"><span data-stu-id="bcc44-160">Effort Completed (Hours)</span></span> | <span data-ttu-id="bcc44-161">עבודה שהושלמה עבור המשימה בשעות.</span><span class="sxs-lookup"><span data-stu-id="bcc44-161">Completed work for the task in hours.</span></span> |
| <span data-ttu-id="bcc44-162">משך הזמן</span><span class="sxs-lookup"><span data-stu-id="bcc44-162">Duration</span></span> | <span data-ttu-id="bcc44-163">מציג את משך המשימה בימים.</span><span class="sxs-lookup"><span data-stu-id="bcc44-163">Displays the duration in days for the task.</span></span> |
| <span data-ttu-id="bcc44-164">מאמץ כולל</span><span class="sxs-lookup"><span data-stu-id="bcc44-164">Total Effort</span></span> | <span data-ttu-id="bcc44-165">סה"כ עבודה למשימה בשעות.</span><span class="sxs-lookup"><span data-stu-id="bcc44-165">Total work for the task in hours.</span></span> |
| <span data-ttu-id="bcc44-166">סיום</span><span class="sxs-lookup"><span data-stu-id="bcc44-166">Finish</span></span> | <span data-ttu-id="bcc44-167">תאריך ושעת סיום.</span><span class="sxs-lookup"><span data-stu-id="bcc44-167">Finish date and time.</span></span> |
| <span data-ttu-id="bcc44-168">% הושלם</span><span class="sxs-lookup"><span data-stu-id="bcc44-168">% Complete</span></span> | <span data-ttu-id="bcc44-169">אחוז המשימה שהושלמה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-169">The percentage of the task that is complete.</span></span> |
| <span data-ttu-id="bcc44-170">מיכל של פרוייקט</span><span class="sxs-lookup"><span data-stu-id="bcc44-170">Project Bucket</span></span> | <span data-ttu-id="bcc44-171">ניתן לקבץ את לוח הפעילויות לפי Bucket כך שלכל Bucket יש עמודה משלו.</span><span class="sxs-lookup"><span data-stu-id="bcc44-171">The task board can be grouped by bucket so each bucket has its own column.</span></span> |
| <span data-ttu-id="bcc44-172">מאמץ שנותר (בשעות)</span><span class="sxs-lookup"><span data-stu-id="bcc44-172">Effort Remaining (Hours)</span></span> | <span data-ttu-id="bcc44-173">העבודה שנותרה למשימה בשעות.</span><span class="sxs-lookup"><span data-stu-id="bcc44-173">The remaining work for the task in hours.</span></span> |
| <span data-ttu-id="bcc44-174">התחל</span><span class="sxs-lookup"><span data-stu-id="bcc44-174">Start</span></span> | <span data-ttu-id="bcc44-175">תאריך התחלה ושעת התחלה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-175">Start date and time.</span></span> |
| <span data-ttu-id="bcc44-176">שם</span><span class="sxs-lookup"><span data-stu-id="bcc44-176">Name</span></span> | <span data-ttu-id="bcc44-177">שם המשימה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-177">The name of the task.</span></span> |
| <span data-ttu-id="bcc44-178">מזהה</span><span class="sxs-lookup"><span data-stu-id="bcc44-178">ID</span></span> | <span data-ttu-id="bcc44-179">מזהה המשימה במבנה התפלגות העבודה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-179">The ID of the task in the work breakdown structure.</span></span> |

## <a name="staffing-attributes"></a><span data-ttu-id="bcc44-180">תכונות איוש</span><span class="sxs-lookup"><span data-stu-id="bcc44-180">Staffing attributes</span></span>

<span data-ttu-id="bcc44-181">ניתן לגשת לתכונות איוש באמצעות השדה **משאבים** בלוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="bcc44-181">Staffing attributes are accessed through the **Resources** field in the schedule.</span></span> <span data-ttu-id="bcc44-182">תוכל לחפש משאב קיים או לבחור **צור** ובחלונית **יצירה מהירה**, הוסף חבר צוות פרוייקט כמשאב חדש.</span><span class="sxs-lookup"><span data-stu-id="bcc44-182">You can either search for an existing resource, or select **Create**, and in the **Quick Create** pane, add a project team member as a new resource.</span></span>

<span data-ttu-id="bcc44-183">השדות **תפקיד**, **‏‫יחידת הקצאת משאבים‬**, ו **שם עמדה‬** משמשים לתיאור דרישות האיוש עבור המשימה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-183">The **Role**, **Resourcing Unit**, and **Position Name** fields are used to describe the staffing requirements for the task.</span></span> <span data-ttu-id="bcc44-184">תכונות איוש אלה, יחד עם לוח הזמנים של המשימה, משמשים לחיפוש משאבים זמינים לביצוע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="bcc44-184">These staffing attributes, together with the task schedule are used to find available resources to do this task.</span></span>

   - <span data-ttu-id="bcc44-185">**תפקיד**: ציין את סוג המשאב הדרוש לביצוע המשימה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-185">**Role**: Specify the type of resource that is required to do the task.</span></span>
   - <span data-ttu-id="bcc44-186">**יחידת הקצאת משאבים**: ציין את היחידה שממנה יש להקצות משאבים עבור המשימה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-186">**Resourcing unit**: Specify the unit that resources for the task should be assigned from.</span></span> <span data-ttu-id="bcc44-187">תכונה זו משפיעה על הערכת העלות והמכירות עבור המשימה אם תעריף העלות והחיוב עבור המשאב מוגדרים בהתאם ל‏‫יחידות של הקצאת משאבים‬.</span><span class="sxs-lookup"><span data-stu-id="bcc44-187">This attribute affects the cost and sales estimate for the task if the cost and bill rate for the resource are set based on resourcing units.</span></span>
   - <span data-ttu-id="bcc44-188">**שם עמדה**: הזן שם ידידותי עבור המשאב הכללי שמשרת כמציין מיקום עבור המשאב שבסופו של דבר יבצע את העבודה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-188">**Position name**: Enter a name for the generic resource that serves as a placeholder for the resource that will ultimately do the work.</span></span>

<span data-ttu-id="bcc44-189">השדה **משאבים** שומר על שם העמדה של המשאב הכללי או משאב בעל שם, כאשר הוא יימצא.</span><span class="sxs-lookup"><span data-stu-id="bcc44-189">The **Resources** field holds the position name of the generic resource or named resource when one is found.</span></span>

<span data-ttu-id="bcc44-190">השדה **קטגוריה** שומר על הערכים שמציינים סוג עבודה רחב יותר שאליו ניתן לקבץ את המשימה.</span><span class="sxs-lookup"><span data-stu-id="bcc44-190">The **Category** field holds the values that indicate a broader type of work that the task can be grouped into.</span></span> <span data-ttu-id="bcc44-191">שדה זה אינו משפיע על תזמון או על איוש.</span><span class="sxs-lookup"><span data-stu-id="bcc44-191">This field doesn't affect scheduling or staffing.</span></span> <span data-ttu-id="bcc44-192">במקום זאת, השדה משמש לדיווח בלבד.</span><span class="sxs-lookup"><span data-stu-id="bcc44-192">Instead, the field is used only for reporting.</span></span>

## <a name="task-dependencies"></a><span data-ttu-id="bcc44-193">יחסי תלות בין משימות</span><span class="sxs-lookup"><span data-stu-id="bcc44-193">Task dependencies</span></span>

<span data-ttu-id="bcc44-194">באפשרותך להשתמש בלוח הזמנים ב- Project Operations כדי ליצור קשרי פעילויות קדם בין משימות.</span><span class="sxs-lookup"><span data-stu-id="bcc44-194">You can use the schedule in Project Operations to create predecessor relationships between tasks.</span></span> <span data-ttu-id="bcc44-195">השדה **‏‫‏‏פעילות קדם‬** משתמש בערך אחד או יותר כדי לציין את המשימות שמשימה תלויה בהן.</span><span class="sxs-lookup"><span data-stu-id="bcc44-195">The **Predecessor** field uses one or more values to indicate the tasks that a task depends on.</span></span> <span data-ttu-id="bcc44-196">בעת הקצאת ערכים לפעילות קדם, המשימה תוכל להתחיל רק לאחר השלמת כל המשימות של פעילויות הקדם.</span><span class="sxs-lookup"><span data-stu-id="bcc44-196">When predecessor values are assigned to a task, the task can start only after all of the predecessor tasks have been completed.</span></span> <span data-ttu-id="bcc44-197">בשל התלות, תאריך ההתחלה המתוכנן של הפעילות מאופס לתאריך שבו הושלמו המשימות של פעילויות הקדם.</span><span class="sxs-lookup"><span data-stu-id="bcc44-197">Because of the dependency, the planned start date of the task is reset to the date when the predecessor tasks are completed.</span></span>

<span data-ttu-id="bcc44-198">למצב המשימה אין שום השפעה על עדכונים שמתבצעים לתאריכי ההתחלה או הסוף של משימות תלויות/פעילויות קדם.</span><span class="sxs-lookup"><span data-stu-id="bcc44-198">The task mode has no effect on updates that are made to the start and end dates of predecessor/dependent tasks.</span></span>

## <a name="accessibility-and-keyboard-shortcuts"></a><span data-ttu-id="bcc44-199">נגישות וקיצורי מקשים</span><span class="sxs-lookup"><span data-stu-id="bcc44-199">Accessibility and keyboard shortcuts</span></span>

<span data-ttu-id="bcc44-200">הרשת **לוח זמנים** נגישה לחלוטין וניתן להשתמש בה עם קוראי מסך כמו 'קורא טקסטים', JAWS או NVDA.</span><span class="sxs-lookup"><span data-stu-id="bcc44-200">The **Schedule** grid is fully accessible and can be used with screen readers such as Narrator, JAWS, or NVDA.</span></span> <span data-ttu-id="bcc44-201">תוכל לזוז באזור הרשת באמצעות מקשי החצים (כמו ב- Microsoft Excel), תוכל להשתמש במקש ה- Tab כדי להתקדם באמצעות רכיבי ממשק משתמש אינטראקטיביים ותוכל להשתמש במקש החץ למטה, במקש ה- Enter או במקש הרווח כדי לבחור ולפתוח תפריטים נפתחים.</span><span class="sxs-lookup"><span data-stu-id="bcc44-201">You can move through the grid area by using arrow keys (as in Microsoft Excel), you can use the Tab key to advance through the interactive user interface elements, and you can use the Down arrow key, the Enter key, or the Spacebar to select and open the drop-down menus.</span></span>
