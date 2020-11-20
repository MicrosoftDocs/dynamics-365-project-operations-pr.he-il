---
title: קביעת לוח זמנים לפרויקט עם מבנה התפלגות עבודה
description: כיצד לקבוע לוח זמנים לפרויקט עם מבנה התפלגות עבודה ב- Project Service
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: 04f30f2f2ed93dd1525f1c86a7521cdbf39a77bc
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127879"
---
# <a name="schedule-a-project-with-a-work-breakdown-structure-project-service"></a><span data-ttu-id="81f59-103">קביעת לוח זמנים לפרויקט עם מבנה התפלגות עבודה (Project Service)</span><span class="sxs-lookup"><span data-stu-id="81f59-103">Schedule a project with a work breakdown structure (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="81f59-104">לוח הזמנים של הפרויקט מציג את המטלות שיש לבצע, אילו משאבים יבצעו את העבודה ואת מסגרת הזמן שבה העבודה צריכה להסתיים.</span><span class="sxs-lookup"><span data-stu-id="81f59-104">A project schedule communicates what work needs to be performed, which resources will perform the work, and the timeframe in which that work needs to be completed.</span></span> <span data-ttu-id="81f59-105">לוח הזמנים של הפרויקט משקף את כל העבודה הקשורה למסירת הפרויקט בזמן.</span><span class="sxs-lookup"><span data-stu-id="81f59-105">The project schedule reflects all the work associated with delivering the project on time.</span></span> <span data-ttu-id="81f59-106">אחת הפעולות הראשונות בשלב האתחול של הפרויקט היא לקבוע לוח זמנים של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="81f59-106">One of the first steps in the initiation phase of the project is to come up with a project schedule.</span></span> <span data-ttu-id="81f59-107">כדי ליצור את לוח הזמנים של הפרויקט, עליך ליצור מבנה התפלגות עבודה.</span><span class="sxs-lookup"><span data-stu-id="81f59-107">To establish a project schedule, you need to create a work breakdown structure.</span></span>  
  
 <span data-ttu-id="81f59-108">צור את מבנה הפרויקט עם מבנה התפלגות עבודה, המסייע לך:</span><span class="sxs-lookup"><span data-stu-id="81f59-108">Create a project structure with a work breakdown structure, which helps you:</span></span>  
  
- <span data-ttu-id="81f59-109">לחלק את העבודה למשימות הניתנות לניהול</span><span class="sxs-lookup"><span data-stu-id="81f59-109">Break down work into manageable tasks</span></span>  
  
- <span data-ttu-id="81f59-110">להעריך את משך הזמן הנדרש להשלמת משימה</span><span class="sxs-lookup"><span data-stu-id="81f59-110">Estimate the time required to complete a task</span></span>  
  
- <span data-ttu-id="81f59-111">להגדיר את יחסי התלות בין משימות ואת משך המשימה</span><span class="sxs-lookup"><span data-stu-id="81f59-111">Set task dependencies and task duration</span></span>  
  
- <span data-ttu-id="81f59-112">לקבוע את התפקידים הנדרשים להשלמת כל משימה</span><span class="sxs-lookup"><span data-stu-id="81f59-112">Determine the roles required to complete each task</span></span>  
  
  <span data-ttu-id="81f59-113">ללוח הזמנים של הפרויקט במבנה התפלגות העבודה יש מראה ותחושה מוכרים, יחד עם תרשים גנט אינטראקטיבי.</span><span class="sxs-lookup"><span data-stu-id="81f59-113">The project schedule in the work breakdown structure has a familiar look and feel, complete with an interactive Gantt chart.</span></span>  
  
## <a name="create-a-work-breakdown-structure-for-a-project"></a><span data-ttu-id="81f59-114">יצירת מבנה התפלגות עבודה עבור פרויקט</span><span class="sxs-lookup"><span data-stu-id="81f59-114">Create a work breakdown structure for a project</span></span>  
 <span data-ttu-id="81f59-115">יצירת מבנה התפלגות עבודה המייצג את רצף הפעילויות בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="81f59-115">Create a work breakdown structure to represent the sequence of tasks in a project.</span></span> <span data-ttu-id="81f59-116">מבנה התפלגות העבודה כולל משימות, דרישות עבור כל משימה, ופרטי הכנסות ועלויות.</span><span class="sxs-lookup"><span data-stu-id="81f59-116">The work breakdown structure includes tasks, requirements for each task, and revenue and cost information.</span></span> <span data-ttu-id="81f59-117">במבנה התפלגות העבודה ניתן להוסיף:</span><span class="sxs-lookup"><span data-stu-id="81f59-117">In your work breakdown structure, you can add:</span></span>  
  
-   <span data-ttu-id="81f59-118">רצף המשימות בהירארכיה</span><span class="sxs-lookup"><span data-stu-id="81f59-118">The sequence of tasks in a hierarchy</span></span>  
  
-   <span data-ttu-id="81f59-119">משימות אחרות, אם יש, שחייבות להסתיים לפני שניתן להתחיל משימה</span><span class="sxs-lookup"><span data-stu-id="81f59-119">Other tasks, if any, that must be completed before a task can be started</span></span>  
  
-   <span data-ttu-id="81f59-120">מועד ההתחלה, מועד הסיום ומשך הפעילות</span><span class="sxs-lookup"><span data-stu-id="81f59-120">The starting date, ending date, and duration of a task</span></span>  
  
-   <span data-ttu-id="81f59-121">מספר השעות הנדרש עבור משימה</span><span class="sxs-lookup"><span data-stu-id="81f59-121">The number of hours required for a task</span></span>  
  
-   <span data-ttu-id="81f59-122">כל הכישורים הנדרשים מהעובדים וההשכלה הנדרשת</span><span class="sxs-lookup"><span data-stu-id="81f59-122">Any required worker skills and education</span></span>  
  
-   <span data-ttu-id="81f59-123">העובדים שהוקצו למשימה</span><span class="sxs-lookup"><span data-stu-id="81f59-123">The workers who are assigned to a task</span></span>  
  
-   <span data-ttu-id="81f59-124">הכנסה ועלויות משוערות</span><span class="sxs-lookup"><span data-stu-id="81f59-124">Estimated revenue and costs</span></span>  
  
## <a name="task-types"></a><span data-ttu-id="81f59-125">סוגי משימות</span><span class="sxs-lookup"><span data-stu-id="81f59-125">Task types</span></span>  
<span data-ttu-id="81f59-126">תשתמש בסוגים הבאים של משימות בעת יצירת מבנה התפלגות העבודה שלך:</span><span class="sxs-lookup"><span data-stu-id="81f59-126">You’ll use the following types of tasks when creating your work breakdown structure:</span></span>  

| | | 
|---------------------------------------|-----------------------------------------------------------------| 
| <span data-ttu-id="81f59-127">**צומת הבסיס של פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="81f59-127">**Project root node**</span></span> | <span data-ttu-id="81f59-128">פעילות הערסל ברמה העליונה עבור הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="81f59-128">The top-level summary task for the project.</span></span> <span data-ttu-id="81f59-129">כל המשימות האחרות של הפרויקט ייווצרו תחתיה.</span><span class="sxs-lookup"><span data-stu-id="81f59-129">All other project tasks are created under it.</span></span> <span data-ttu-id="81f59-130">שם פעילות הבסיס הוא שם הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="81f59-130">The name of the root task is the project name.</span></span> <span data-ttu-id="81f59-131">המאמץ, התאריכים ומשך צומת הבסיס מבוססים על הערכים בהירארכיה שמתחתיו.</span><span class="sxs-lookup"><span data-stu-id="81f59-131">The effort, dates, and duration of the root node are based on the values on the hierarchy below it.</span></span> <span data-ttu-id="81f59-132">אי אפשר לערוך מאפיינים של צומת הבסיס או למחוק את צומת הבסיס.</span><span class="sxs-lookup"><span data-stu-id="81f59-132">You can’t edit root node properties or delete the root node.</span></span> | 
| <span data-ttu-id="81f59-133">**משימות סיכום או גורם מכיל**.</span><span class="sxs-lookup"><span data-stu-id="81f59-133">**Summary or container tasks**</span></span> | <span data-ttu-id="81f59-134">פעילות ערסל היא פעילות שיש משימות משנה מתחת לה.</span><span class="sxs-lookup"><span data-stu-id="81f59-134">A summary task is a task that has sub-tasks under it.</span></span> <span data-ttu-id="81f59-135">לפעילות ערסל אין עבודה או עלות משלה.</span><span class="sxs-lookup"><span data-stu-id="81f59-135">A summary task doesn’t have any work effort or cost of its own.</span></span> <span data-ttu-id="81f59-136">העבודה והעלות שלה הם אוסף של משימות המשנה שלה.</span><span class="sxs-lookup"><span data-stu-id="81f59-136">Its work effort and cost are a rollup of its sub-tasks.</span></span> <span data-ttu-id="81f59-137">ניתן לשנות את השם של פעילות הערסל, אך אי אפשר לשנות את המאמץ, התאריכים או משך הזמן, מכיוון שאלה מחושבים באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="81f59-137">You can change the name of a summary task, but you can’t change the effort, dates, or duration, because those are automatically calculated.</span></span> <span data-ttu-id="81f59-138">מחיקה של פעילות ערסל מוחקת את הפעילות ואת כל משימות המשנה שלה.</span><span class="sxs-lookup"><span data-stu-id="81f59-138">Deleting a summary task deletes the task and all of its sub-tasks.</span></span>|  
| <span data-ttu-id="81f59-139">**משימות צומת עלה**</span><span class="sxs-lookup"><span data-stu-id="81f59-139">**Leaf node tasks**</span></span> | <span data-ttu-id="81f59-140">משימת צומת עלה מייצגת את העבודה המפורטת ביותר בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="81f59-140">A leaf node task represents the most detailed work on the project.</span></span> <span data-ttu-id="81f59-141">יש לה הערכות של כמות העבודה, מספר משאבים מתוכנן, תאריכי התחלה וסיום ומשך פעילות מתוכננים.</span><span class="sxs-lookup"><span data-stu-id="81f59-141">It has an estimated effort, a planned number of resources, planned start and end dates, and a duration.</span></span>|

  
## <a name="task-hierarchy"></a><span data-ttu-id="81f59-142">הירארכיית הפעילויות</span><span class="sxs-lookup"><span data-stu-id="81f59-142">Task hierarchy</span></span>  
 <span data-ttu-id="81f59-143">עומדות בפניך האפשרויות הבאות בעת יצירת היררכיה של פעילות:</span><span class="sxs-lookup"><span data-stu-id="81f59-143">You have the following options when creating a task hierarchy:</span></span>  
  
- <span data-ttu-id="81f59-144">**הוסף משימה**.</span><span class="sxs-lookup"><span data-stu-id="81f59-144">**Add task**.</span></span>   <span data-ttu-id="81f59-145">ניתן להוסיף משימה במיקום שתבחר בהירארכיה של המשימה.</span><span class="sxs-lookup"><span data-stu-id="81f59-145">You can add a task at a position you choose in the task hierarchy.</span></span> <span data-ttu-id="81f59-146">אם לא תבחר מיקום, המשימה החדשה שלך תופיע בסוף.</span><span class="sxs-lookup"><span data-stu-id="81f59-146">If you don’t select a position, your new task appears at the end.</span></span>  
  
- <span data-ttu-id="81f59-147">**הסטה פנימה של משימה**.</span><span class="sxs-lookup"><span data-stu-id="81f59-147">**Indent task**.</span></span>   <span data-ttu-id="81f59-148">הסט פנימה את המשימש כדי להפוך אותה לצאצא של המשימה שנמצאת ישירות מעליה.</span><span class="sxs-lookup"><span data-stu-id="81f59-148">Indent a task to make it a child of the task directly above it.</span></span>  
  
- <span data-ttu-id="81f59-149">**הסטה החוצה של משימה**</span><span class="sxs-lookup"><span data-stu-id="81f59-149">**Outdent task**.</span></span>   <span data-ttu-id="81f59-150">הסט החוצה את המשימה כדי שהיא כבר לא תהיה פעילות משנה של משימת האב המקורית.</span><span class="sxs-lookup"><span data-stu-id="81f59-150">Outdent a task to make it so it’s no longer a sub-task of its original parent task.</span></span>  
  
- <span data-ttu-id="81f59-151">**הזז למעלה והזז למטה**.</span><span class="sxs-lookup"><span data-stu-id="81f59-151">**Move up and Move down**.</span></span>   <span data-ttu-id="81f59-152">העבר משימות למעלה או למטה בהירארכיה של משימת האב.</span><span class="sxs-lookup"><span data-stu-id="81f59-152">Move tasks up and down in the hierarchy of its parent task.</span></span> <span data-ttu-id="81f59-153">להעברת משימה למעלה או למטה אין השפעה על המאמץ, העלות, התאריכים או משך הזמן שלה.</span><span class="sxs-lookup"><span data-stu-id="81f59-153">Moving a task up or down has no effect on its effort, cost, dates, or duration.</span></span>  
  
## <a name="task-attributes"></a><span data-ttu-id="81f59-154">תכונות המשימה</span><span class="sxs-lookup"><span data-stu-id="81f59-154">Task attributes</span></span>  
 <span data-ttu-id="81f59-155">שם המשימה מתאר את העבודה שיש להשלים.</span><span class="sxs-lookup"><span data-stu-id="81f59-155">A task’s name describes the work that needs to be completed.</span></span> <span data-ttu-id="81f59-156">השתמש בתכונות שונות של המשימה כדי לתאר את לוח הזמנים ואת דרישות כוח האדם עבור המשימה.</span><span class="sxs-lookup"><span data-stu-id="81f59-156">You use various task attributes to describe the schedule and staffing requirements for the task.</span></span>  
  
### <a name="schedule-attributes"></a><span data-ttu-id="81f59-157">תכונות של לוח זמנים</span><span class="sxs-lookup"><span data-stu-id="81f59-157">Schedule attributes</span></span>

 - <span data-ttu-id="81f59-158">הקצאת ערכים עבור **שעות מאמץ**, **מספר משאבים**, **תאריך התחלה**, **תאריך סיום**, ו- **משך** כדי לקבוע את לוח הזמנים עבור המשימה.</span><span class="sxs-lookup"><span data-stu-id="81f59-158">Assign values to **Effort hours**, **Number of resources**, **Start date**, **End date**, and **Duration** to determine the schedule for the task.</span></span> 
 - <span data-ttu-id="81f59-159">**מאמץ** הוא הערכה של השעות הנדרשות כדי להשלים את המשימה.</span><span class="sxs-lookup"><span data-stu-id="81f59-159">**Effort** is an estimate of the hours it takes to complete the task.</span></span>
 - <span data-ttu-id="81f59-160">**מספר משאבים** הוא הערכה שמנהל הפרויקט מוסיף למשימה כדי לסייע בקביעת לוח הזמנים הטוב ביותר שאפשר.</span><span class="sxs-lookup"><span data-stu-id="81f59-160">**Number of resources** is an estimate that the project manager puts in the task to help come up with the best possible schedule.</span></span> 
 - <span data-ttu-id="81f59-161">**משך** (בימים) מציין את מספר ימי העבודה שיידרש כדי להשלים את המשימה.</span><span class="sxs-lookup"><span data-stu-id="81f59-161">**Duration** (in days) indicates the number of work days it will take to complete the task.</span></span>  
  
### <a name="staffing-attributes"></a><span data-ttu-id="81f59-162">תכונות איוש</span><span class="sxs-lookup"><span data-stu-id="81f59-162">Staffing attributes</span></span>

 - <span data-ttu-id="81f59-163">**תפקיד**, **יחידה ארגונית של המשאב**, **מספר משאבים**, ו- **משאבים** מתארים את דרישות כוח האדם עבור המשימה.</span><span class="sxs-lookup"><span data-stu-id="81f59-163">**Role**, **Resource organizational unit**, **Number of resources**, and **Resources** describe the staffing requirements for the task.</span></span> 
 - <span data-ttu-id="81f59-164">**תפקיד** מתאר את סוג המשאב הדרוש כדי לבצע את המשימה.</span><span class="sxs-lookup"><span data-stu-id="81f59-164">**Role** describes the type of resource needed to perform the task.</span></span> 
 - <span data-ttu-id="81f59-165">**היחידה הארגונית של המשאב** מציין את היחידה הארגונית שממנה נעשה איוש המשאבים עבור המשימה; הדבר משפיע גם על העלות ועל הערכת המכירות של המשימה, שכן זה כלול בעת קביעת מחיר המכירה ליחידה עבור המשאב.</span><span class="sxs-lookup"><span data-stu-id="81f59-165">**Resource organizational unit** indicates the organizational unit from which resources should be staffed for that task; this also impacts the cost and sales estimate of the task, since this is accounted for when determining the unit sales price for the resource.</span></span> 
 - <span data-ttu-id="81f59-166">**משאבים** כולל משאב כללי או משאב בעל שם כאשר הוא נמצא.</span><span class="sxs-lookup"><span data-stu-id="81f59-166">**Resources** holds a generic resource or a named resource when one is found.</span></span>  
  
## <a name="task-dependencies"></a><span data-ttu-id="81f59-167">יחסי תלות בין משימות</span><span class="sxs-lookup"><span data-stu-id="81f59-167">Task dependencies</span></span>  
 <span data-ttu-id="81f59-168">באפשרותך ליצור קשרי פעילויות קדם בין משימה אחת או יותר במבנה התפלגות העבודה.</span><span class="sxs-lookup"><span data-stu-id="81f59-168">You can create predecessor relationships between one or more tasks in the work breakdown structure.</span></span> <span data-ttu-id="81f59-169">ניתן להגדיר ערך אחד או יותר עבור השדה של פעילויות הקדם כדי לציין את המשימות שבהן היא תלויה.</span><span class="sxs-lookup"><span data-stu-id="81f59-169">You can set one or more values for the predecessor field on tasks to indicate the tasks that it will be dependent on.</span></span> <span data-ttu-id="81f59-170">בעת הקצאת ערך לפעילות הקדם, המשימה תוכל להתחיל רק לאחר השלמת כל פעילויות הקדם.</span><span class="sxs-lookup"><span data-stu-id="81f59-170">When you assign a predecessor value to a task, the task can only start when all the predecessor tasks have completed.</span></span> <span data-ttu-id="81f59-171">הגדרה של תלות בפעילות תגרום לחישוב מחדש של תאריך ההתחלה המתוכנן של המשימה וקביעתו לתאריך הסיום העדכני ביותר של כל פעילויות הקדם שלה.</span><span class="sxs-lookup"><span data-stu-id="81f59-171">Setting this dependency on a task will result in the recalculation of the planned start date of the task as the latest end of all of its predecessors.</span></span> <span data-ttu-id="81f59-172">ההשפעות הקשורות לפעילויות הקדם בלוח הזמנים אינן מוגבלות למצב המשימה המוגדר במשימה.</span><span class="sxs-lookup"><span data-stu-id="81f59-172">Predecessor-related impacts on a schedule are not limited by the task mode defined on the task.</span></span>  
  
## <a name="task-mode"></a><span data-ttu-id="81f59-173">מצב משימה</span><span class="sxs-lookup"><span data-stu-id="81f59-173">Task mode</span></span>  
 <span data-ttu-id="81f59-174">מצב משימה הוא אחד הגורמים החשובים הקובעים את התזמון של משימות צומת עלה.</span><span class="sxs-lookup"><span data-stu-id="81f59-174">Task mode is one of the important factors that determine scheduling leaf node tasks.</span></span> <span data-ttu-id="81f59-175">ישנם שני מצבי משימה עבור כל משימה: מצב תזמון אוטומטי ומצב תזמון ידני.</span><span class="sxs-lookup"><span data-stu-id="81f59-175">There are two task modes for every task: auto scheduling mode and manual scheduling mode.</span></span>  
  
-   <span data-ttu-id="81f59-176">**תזמון אוטומטי**.</span><span class="sxs-lookup"><span data-stu-id="81f59-176">**Auto scheduling**.</span></span>   <span data-ttu-id="81f59-177">בעת הגדרת מצב המשימה בתור 'תזמון אוטומטי', מנוע תזמון המשימות משתמש בכללי תזמון על התכונות הבאות של המשימה כדי לקבוע את לוח הזמנים עבור המשימה:</span><span class="sxs-lookup"><span data-stu-id="81f59-177">When you set the task mode to Automatically Scheduled, the task scheduling engine uses the scheduling rules on the following task attributes to determine the schedule for the task:</span></span>  
  
    -   <span data-ttu-id="81f59-178">‏‏פעילויות קדם</span><span class="sxs-lookup"><span data-stu-id="81f59-178">Predecessors</span></span>  
  
    -   <span data-ttu-id="81f59-179">מאמץ</span><span class="sxs-lookup"><span data-stu-id="81f59-179">Effort</span></span>  
  
    -   <span data-ttu-id="81f59-180">מספר משאבים</span><span class="sxs-lookup"><span data-stu-id="81f59-180">Number of resources</span></span>  
  
    -   <span data-ttu-id="81f59-181">תאריכי ההתחלה והסיום</span><span class="sxs-lookup"><span data-stu-id="81f59-181">Start and end dates</span></span>  
  
-   <span data-ttu-id="81f59-182">**כללי תזמון**.</span><span class="sxs-lookup"><span data-stu-id="81f59-182">**Scheduling rules**.</span></span>   <span data-ttu-id="81f59-183">תאריך ההתחלה של משימת צומת עלה שאין לה פעילויות קדם נקבע כברירת מחדל לתאריך ההתחלה של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="81f59-183">The start date of a leaf node task that does not have predecessors defaults to the project’s scheduling start date.</span></span> <span data-ttu-id="81f59-184">משך פעילות צומת עלה תמיד מחושב כמספר ימי העבודה בין תאריכי ההתחלה והסיום שלו.</span><span class="sxs-lookup"><span data-stu-id="81f59-184">The duration of a leaf node task is always calculated as the number of working days between its start and end dates.</span></span> <span data-ttu-id="81f59-185">כאשר פעילות מתוזמנת אוטומטית, מנוע התזמון פועל לפי הכללים שלהלן:</span><span class="sxs-lookup"><span data-stu-id="81f59-185">When a task is automatically scheduled, the scheduling engine follows the rules below:</span></span>  
  
    -   <span data-ttu-id="81f59-186">תאריכי ההתחלה והסיום של המשימה חייבים תמיד להיות ימי עבודה לפי לוח השנה והתזמון של הפרויקט</span><span class="sxs-lookup"><span data-stu-id="81f59-186">Start and end dates of a task must always be working days according to the project’s scheduling calendar</span></span>  
  
    -   <span data-ttu-id="81f59-187">תאריך ההתחלה של משימה שיש לה פעילות קדם נקבע לתאריך הסיום האחרון של פעילויות הקדם שלה</span><span class="sxs-lookup"><span data-stu-id="81f59-187">The start date of a task that has predecessors defaults to the latest end date of its predecessors</span></span>  
  
    -   <span data-ttu-id="81f59-188">מאמץ = מספר אנשים \* משך \* שעות ביום עבודה רגיל בלוח שנה של הפרויקט</span><span class="sxs-lookup"><span data-stu-id="81f59-188">Effort = Number of people \* Duration \* hours in a standard work day of the project calendar</span></span>  
  
-   <span data-ttu-id="81f59-189">**תזמון ידני**.</span><span class="sxs-lookup"><span data-stu-id="81f59-189">**Manual scheduling**.</span></span>   <span data-ttu-id="81f59-190">במקרים מסוימים, ייתכן שתרצה לסטות מכללים אלה.</span><span class="sxs-lookup"><span data-stu-id="81f59-190">In some cases, you might want to deviate from these rules.</span></span> <span data-ttu-id="81f59-191">במקרים אלה, באפשרותך להגדיר את מצב המשימה שיהיה מתוזמן באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="81f59-191">In these cases, you can set the task mode for the task to be manually scheduled.</span></span> <span data-ttu-id="81f59-192">פעולה זו מפסיקה את מנוע התזמון המחשב את הערכים עבור תכונות אחרות של התזמון.</span><span class="sxs-lookup"><span data-stu-id="81f59-192">This stops the scheduling engine from calculating the values for other scheduling attributes.</span></span> <span data-ttu-id="81f59-193">הגדרת פעילויות קדם למשימות משפיע תמיד על תאריך ההתחלה של המשימה המקושרת.</span><span class="sxs-lookup"><span data-stu-id="81f59-193">Setting predecessors on tasks always impacts the dependent task’s start date.</span></span>  
  
## <a name="create-a-work-breakdown-structure"></a><span data-ttu-id="81f59-194">יצירה של מבנה התפלגות עבודה</span><span class="sxs-lookup"><span data-stu-id="81f59-194">Create a work breakdown structure</span></span>  
  
1.  <span data-ttu-id="81f59-195">עבור אל **Project Service > פרויקטים**.</span><span class="sxs-lookup"><span data-stu-id="81f59-195">Go to **Project Service > Projects**.</span></span>  
  
2.  <span data-ttu-id="81f59-196">לחץ על הפרויקט שברצונך לעבוד עליו.</span><span class="sxs-lookup"><span data-stu-id="81f59-196">Click the project you want to work on.</span></span>  
  
3.  <span data-ttu-id="81f59-197">בסרגל שלרוחב חלקו העליון של המסך, בחר את החץ למטה לצד שם הפרויקט, ולאחר מכן לחץ על מבנה התפלגות עבודה.</span><span class="sxs-lookup"><span data-stu-id="81f59-197">In the bar across the top of the screen, select the down arrow next to the project name, and then click Work breakdown structure.</span></span>  
  
4.  <span data-ttu-id="81f59-198">כדי להוסיף משימה, לחץ על **הוסף משימה**.</span><span class="sxs-lookup"><span data-stu-id="81f59-198">To add a task, click **Add Task**.</span></span> <span data-ttu-id="81f59-199">מלא את השדות של המשימה ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="81f59-199">Fill in the fields for the task, and then click **Save**.</span></span>  
  
5.  <span data-ttu-id="81f59-200">המשך להוסיף משימות עד להשלמת מבנה התפלגות העבודה.</span><span class="sxs-lookup"><span data-stu-id="81f59-200">Continue adding tasks until your work breakdown structure is complete.</span></span> <span data-ttu-id="81f59-201">בעת יצירת מבנה התפלגות העבודה, באפשרותך לבצע את הפעולות הבאות כדי לארגן את המשימות:</span><span class="sxs-lookup"><span data-stu-id="81f59-201">While creating your work breakdown structure, you can do the following to organize your tasks:</span></span>  
  
    -   <span data-ttu-id="81f59-202">בחר משימה ולחץ על **הסטה פנימה** כדי להעביר אותה מתחת למשימה אחרת או לחץ על 'הסטה החוצה' כדי להזיז אותה החוצה.</span><span class="sxs-lookup"><span data-stu-id="81f59-202">Select a task and click **Indent** to move it under another task or click Outdent to move it out a level.</span></span>  
  
    -   <span data-ttu-id="81f59-203">בחר משימה ולחץ על **העבר למעלה** או **העבר למטה** כדי להעביר אותה למעלה או למטה ברשימה.</span><span class="sxs-lookup"><span data-stu-id="81f59-203">Select a task and click **Move Up** or **Move Down** to move it up or down in the list.</span></span>  
  
    -   <span data-ttu-id="81f59-204">לחץ על **הסתר גנט** כדי להסתיר את תרשים הגנט, ולחץ על **הצג גנט** כדי להציגו שוב.</span><span class="sxs-lookup"><span data-stu-id="81f59-204">Click **Hide Gantt** to hide the Gantt chart, and click **Show Gantt** to display it again.</span></span>  
  
    -   <span data-ttu-id="81f59-205">בחר פרק זמן אחר בתרשים הגנט בתוך **ציר הזמן**.</span><span class="sxs-lookup"><span data-stu-id="81f59-205">Select a different period of time for the Gantt chart in **Time Scale**.</span></span>  
  
6.  <span data-ttu-id="81f59-206">כדי להוסיף את התפקידים שציינת במבנה התפלגות העבודה לחברי צוות הפרויקט שלך, לחץ על **יצירת צוות פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="81f59-206">To add the roles you specified in your work breakdown structure to your project’s team members, click **Generate Project Team**.</span></span>  
  
7.  <span data-ttu-id="81f59-207">לחץ על **שמור** בפינה הימנית התחתונה של המסך לאחר שתסיים לבצע שינויים.</span><span class="sxs-lookup"><span data-stu-id="81f59-207">Click **Save** at the bottom right corner of the screen when you’re done making changes.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="81f59-208">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="81f59-208">See Also</span></span>  
 [<span data-ttu-id="81f59-209">מדריך למנהל פרויקט</span><span class="sxs-lookup"><span data-stu-id="81f59-209">Project manager guide</span></span>](../psa/project-manager-guide.md)
