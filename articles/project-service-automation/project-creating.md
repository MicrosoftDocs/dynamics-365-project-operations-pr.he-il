---
title: לוחות זמנים של פרוייקטים
description: נושא זה מספק מידע לגבי האופן שבו יוצרים לוח זמנים.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 3/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 10e8f8aa-ddfb-4626-b936-86f054808dc2
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: e6c259677fbc43e2e6087e013955f156ae2dac4e
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751785"
---
# <a name="project-schedules"></a><span data-ttu-id="23fde-103">לוחות זמנים של פרוייקטים</span><span class="sxs-lookup"><span data-stu-id="23fde-103">Project schedules</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="23fde-104">לוח הזמנים של הפרוייקט מציג את המטלות שיש להשלים, אילו משאבים יבצעו את העבודה ואת מסגרת הזמן שבה העבודה צריכה להסתיים.</span><span class="sxs-lookup"><span data-stu-id="23fde-104">A project schedule communicates what work must be completed, which resources will do the work, and the timeframe that the work must be finished in.</span></span> <span data-ttu-id="23fde-105">הוא משקף את כל העבודה שמשויכת למסירת הפרוייקט בזמן.</span><span class="sxs-lookup"><span data-stu-id="23fde-105">It reflects all the work that is associated with delivering the project on time.</span></span> <span data-ttu-id="23fde-106">ב- Dynamics 365 Project Service Automation, תוכל ליצור לוח זמנים לפרוייקט על-ידי פירוק עבודה אל משימות שניתנות לניהול, להעריך את הזמן הדרוש לביצוע כל משימה, להגדיר יחסי התלות בין המשימות, להגדיר משכי זמן למשימות ולהעריך את המשאבים הכלליים שיבצעו את המשימות.</span><span class="sxs-lookup"><span data-stu-id="23fde-106">In Dynamics 365 Project Service Automation, you create a project schedule by breaking the work down into manageable tasks, estimating the time that is required to do each task, setting task dependencies, setting task durations, and estimating the generic resources that will do the tasks.</span></span> <span data-ttu-id="23fde-107">לוח זמנים של פרוייקט נוצר בכרטיסיה **לוח זמנים** בדף הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="23fde-107">The project schedule is created on the **Schedule** tab of the project page.</span></span>
 
## <a name="tasks"></a><span data-ttu-id="23fde-108">משימות</span><span class="sxs-lookup"><span data-stu-id="23fde-108">Tasks</span></span>

<span data-ttu-id="23fde-109">השלב הראשון ביצירת לוח זמנים של פרוייקט הוא פירוק העבודה לחלקים הניתנים לניהול.</span><span class="sxs-lookup"><span data-stu-id="23fde-109">The first step in creating a project schedule is to break the work down into manageable portions.</span></span> <span data-ttu-id="23fde-110">לוח הזמנים ב- PSA תומך בתכונות הבאות:</span><span class="sxs-lookup"><span data-stu-id="23fde-110">The schedule in PSA supports the following features:</span></span>

- <span data-ttu-id="23fde-111">צומת הבסיס של פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="23fde-111">Project root node</span></span>
- <span data-ttu-id="23fde-112">משימות סיכום או גורם מכיל.</span><span class="sxs-lookup"><span data-stu-id="23fde-112">Summary or container tasks</span></span>
- <span data-ttu-id="23fde-113">משימות צומת עלה</span><span class="sxs-lookup"><span data-stu-id="23fde-113">Leaf node tasks</span></span>

### <a name="project-root-node"></a><span data-ttu-id="23fde-114">צומת הבסיס של פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="23fde-114">Project root node</span></span>

<span data-ttu-id="23fde-115">צומת הבסיס של הפרוייקט הוא פעילות הערסל ברמה העליונה עבור הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="23fde-115">The project root node is the top-level summary task for the project.</span></span> <span data-ttu-id="23fde-116">כל המשימות האחרות של הפרוייקט ייווצרו תחתיה.</span><span class="sxs-lookup"><span data-stu-id="23fde-116">All other project tasks are created under it.</span></span> <span data-ttu-id="23fde-117">שם צומת הבסיס תמיד יוגדר כשם הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="23fde-117">The name of the root node is always set to the project name.</span></span> <span data-ttu-id="23fde-118">המאמץ, התאריכים ומשך הזמן של צומת הבסיס מסוכמים בהתאם לערכים בהירארכיה שמתחתיו.</span><span class="sxs-lookup"><span data-stu-id="23fde-118">The effort, dates, and duration of the root node are summarized based on the values in the hierarchy below it.</span></span> <span data-ttu-id="23fde-119">אינך יכול לערוך את המאפיינים של צומת הבסיס.</span><span class="sxs-lookup"><span data-stu-id="23fde-119">You can't edit the properties of the root node.</span></span> <span data-ttu-id="23fde-120">כמו כן, לא ניתן למחוק את צומת הבסיס.</span><span class="sxs-lookup"><span data-stu-id="23fde-120">You also can't delete the root node.</span></span>

### <a name="summary-or-container-tasks"></a><span data-ttu-id="23fde-121">משימות סיכום או גורם מכיל.</span><span class="sxs-lookup"><span data-stu-id="23fde-121">Summary or container tasks</span></span> 

<span data-ttu-id="23fde-122">פעילויות ערסל כוללות פעילויות משנה או משימות של גורמים מכילים מתחתיהן.</span><span class="sxs-lookup"><span data-stu-id="23fde-122">Summary tasks have sub-tasks or container tasks under them.</span></span> <span data-ttu-id="23fde-123">אין להן מאמץ עבודה או עלות משלהן.</span><span class="sxs-lookup"><span data-stu-id="23fde-123">They have no work effort or cost of their own.</span></span> <span data-ttu-id="23fde-124">במקום זאת, מאמצי העבודה והעלות שלהן הם סיכום של מאמץ העבודה והעלות של המשימות של הגורמים המכילים שלהן.</span><span class="sxs-lookup"><span data-stu-id="23fde-124">Instead, their work effort and cost are a rollup of the work effort and cost of their container tasks.</span></span> <span data-ttu-id="23fde-125">תאריך ההתחלה של פעילות הערסל הוא תאריך ההתחלה של פעילויות הגורמים המכילים, ותאריך הסיום הוא תאריך הסיום של פעילויות הגורמים המכילים.</span><span class="sxs-lookup"><span data-stu-id="23fde-125">The start date of the summary task is the start date of the container tasks, and the end date is the end date of the container tasks.</span></span> <span data-ttu-id="23fde-126">ניתן לערוך את שם פעילות הערסל, אך לא ניתן לערוך את מאפייני התזמון (מאמץ, תאריכים ומשך זמן).</span><span class="sxs-lookup"><span data-stu-id="23fde-126">The name of a summary task can be edited, but scheduling properties (effort, dates, and duration) can't be edited.</span></span> <span data-ttu-id="23fde-127">אם תמחק פעילות ערסל, תמחק גם את כל משימות הגורמים המכילים שלה.</span><span class="sxs-lookup"><span data-stu-id="23fde-127">If you delete a summary task, you also delete all its container tasks.</span></span>

### <a name="leaf-node-tasks"></a><span data-ttu-id="23fde-128">משימות צומת עלה</span><span class="sxs-lookup"><span data-stu-id="23fde-128">Leaf node tasks</span></span>

<span data-ttu-id="23fde-129">משימות של צומת עלה מייצגות את העבודה המפורטת ביותר בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="23fde-129">Leaf node tasks represent the most granular work on the project.</span></span> <span data-ttu-id="23fde-130">יש להן הערכות של המאמץ, המשאבים, תאריכי התחלה וסיום מתוכננים ומשך הזמן.</span><span class="sxs-lookup"><span data-stu-id="23fde-130">They have an estimated effort, resources, planned start and end dates, and a duration.</span></span>
 
## <a name="creating-a-task-hierarchy"></a><span data-ttu-id="23fde-131">יצירת הירארכיית פעילות</span><span class="sxs-lookup"><span data-stu-id="23fde-131">Creating a task hierarchy</span></span>

<span data-ttu-id="23fde-132">תוכל ליצור הירארכיית פעילות באמצעות האפשרויות הבאות:</span><span class="sxs-lookup"><span data-stu-id="23fde-132">You can create a task hierarchy by using the following options:</span></span>

- <span data-ttu-id="23fde-133">לחצן **הוספת משימה**</span><span class="sxs-lookup"><span data-stu-id="23fde-133">**Add task** button</span></span>
- <span data-ttu-id="23fde-134">לחצן **הסט פעילות פנימה**</span><span class="sxs-lookup"><span data-stu-id="23fde-134">**Indent task** button</span></span>
- <span data-ttu-id="23fde-135">לחצן **הסט פעילות החוצה**</span><span class="sxs-lookup"><span data-stu-id="23fde-135">**Outdent task** button</span></span>
- <span data-ttu-id="23fde-136">לחצן **הזז למעלה** ולחצן **הזז למטה**</span><span class="sxs-lookup"><span data-stu-id="23fde-136">**Move up** and **Move down** buttons</span></span>
- <span data-ttu-id="23fde-137">נגישות וקיצורי מקשים</span><span class="sxs-lookup"><span data-stu-id="23fde-137">Accessibility and keyboard shortcuts</span></span>

### <a name="add-task"></a><span data-ttu-id="23fde-138">הוסף משימה</span><span class="sxs-lookup"><span data-stu-id="23fde-138">Add task</span></span>

<span data-ttu-id="23fde-139">הלחצן **הוסף משימה** מאפשר לך ליצור משימה חדשה בהירארכיה.</span><span class="sxs-lookup"><span data-stu-id="23fde-139">The **Add task** button lets you create a new task in the hierarchy.</span></span> <span data-ttu-id="23fde-140">אם לא תבחר מיקום, המשימה תיכנס לסוף.</span><span class="sxs-lookup"><span data-stu-id="23fde-140">If you don't select a position, the task is inserted at the end.</span></span> 

<span data-ttu-id="23fde-141">מזהה לוח זמנים מוקצה לכל משימה.</span><span class="sxs-lookup"><span data-stu-id="23fde-141">A schedule ID is assigned to every task.</span></span> <span data-ttu-id="23fde-142">מזהה לוח הזמנים מייצג את העומק והמיקום של המשימה בהירארכיה.</span><span class="sxs-lookup"><span data-stu-id="23fde-142">The schedule ID represents the task's depth and position in the hierarchy.</span></span> <span data-ttu-id="23fde-143">הוא משתמש במספור מיתאר.</span><span class="sxs-lookup"><span data-stu-id="23fde-143">It uses outline numbering.</span></span> <span data-ttu-id="23fde-144">במשימות ברמה הראשונה תחת צומת הבסיס של הפרוייקט, נעשה שימוש בסכימת מספור של 1, 2, 3 וכן הלאה.</span><span class="sxs-lookup"><span data-stu-id="23fde-144">For tasks in the first level under the project root node, a numbering scheme of 1, 2, 3, and so on, is used.</span></span> <span data-ttu-id="23fde-145">במשימות תחת הרמה הראשונה, נעשה שימוש בסכימת מספור של 1.1, 1.2, 1.3 וכן הלאה.</span><span class="sxs-lookup"><span data-stu-id="23fde-145">For tasks under the first level, a numbering scheme of 1.1, 1.2, 1.3, and so on, is used.</span></span>

### <a name="indent-task"></a><span data-ttu-id="23fde-146">הסט פעילות פנימה</span><span class="sxs-lookup"><span data-stu-id="23fde-146">Indent task</span></span>

<span data-ttu-id="23fde-147">כאשר פעילות מוסטת פנימה, היא הופכת לצאצא של הפעילות הנמצאת ישירות מעליה.</span><span class="sxs-lookup"><span data-stu-id="23fde-147">When a task is indented, it becomes a child of the task that is directly above it.</span></span> <span data-ttu-id="23fde-148">מזהה לוח הזמנים של הפעילות מחושב מחדש כך שהוא מבוסס על מזהה לוח הזמנים של האב החדש שלו ופועל לפי סכימת מספור המיתאר.</span><span class="sxs-lookup"><span data-stu-id="23fde-148">The schedule ID of the task is then recalculated so that it's based on the schedule ID of its new parent and follows the outline numbering scheme.</span></span> <span data-ttu-id="23fde-149">פעילות האב היא כעת פעילות ערסל או משימה של גורם מכיל.</span><span class="sxs-lookup"><span data-stu-id="23fde-149">The parent task is now a summary task or a container task.</span></span> <span data-ttu-id="23fde-150">לכן, היא הופכת לסיכום של משימות הצאצא שלה.</span><span class="sxs-lookup"><span data-stu-id="23fde-150">Therefore, it becomes a rollup of its child tasks.</span></span>

### <a name="outdent-task"></a><span data-ttu-id="23fde-151">הסט פעילות החוצה</span><span class="sxs-lookup"><span data-stu-id="23fde-151">Outdent task</span></span> 

<span data-ttu-id="23fde-152">כאשר מסיטים פעילות החוצה, היא כבר לא צאצא של הפעילות שהיתה האב שלה.</span><span class="sxs-lookup"><span data-stu-id="23fde-152">When a task is outdented, it's no longer a child of the task that was its parent.</span></span> <span data-ttu-id="23fde-153">מזהה לוח הזמנים מחושב מחדש כך שהוא ישקף את המיקום והעומק המעודכנים של הפעילות בהירארכיה.</span><span class="sxs-lookup"><span data-stu-id="23fde-153">The schedule ID is then recalculated so that it reflects the task's updated depth and position in the hierarchy.</span></span> <span data-ttu-id="23fde-154">המאמץ, העלות והתאריכים של פעילות האב הקודמת מחושבים מחדש כך שלא יכללו בפעילות זו.</span><span class="sxs-lookup"><span data-stu-id="23fde-154">The effort, cost, and dates of the previous parent task are recalculated so that they don't include this task.</span></span>

### <a name="move-up-and-move-down"></a><span data-ttu-id="23fde-155">הזז למעלה והזז למטה</span><span class="sxs-lookup"><span data-stu-id="23fde-155">Move up and Move down</span></span> 

<span data-ttu-id="23fde-156">הלחצן **הזז למעלה** והלחצן **הזז למטה** משנים את מיקום הפעילות בתוך הירארכיית האב שלה.</span><span class="sxs-lookup"><span data-stu-id="23fde-156">The **Move up** and **Move down** buttons change the position of a task within its parent hierarchy.</span></span> <span data-ttu-id="23fde-157">שינויים מסוג זה אינם משפיעים על המאמץ, העלות, התאריכים או משך הזמן של הפעילות.</span><span class="sxs-lookup"><span data-stu-id="23fde-157">Changes of this type don't affect the task's effort, cost, dates, or duration.</span></span> <span data-ttu-id="23fde-158">רק מזהה לוח הזמנים של הפעילות מושפע.</span><span class="sxs-lookup"><span data-stu-id="23fde-158">Only the task's schedule ID is affected.</span></span> <span data-ttu-id="23fde-159">מזהה לוח הזמנים מחושב מחדש כך שהוא ישקף את המיקום והעומק החדשים של ברשימת פעילויות הצאצאים של פעילות האב.</span><span class="sxs-lookup"><span data-stu-id="23fde-159">The schedule ID is recalculated so that it reflects the task's new position in the parent's list of child tasks.</span></span>

### <a name="accessibility-and-keyboard-shortcuts"></a><span data-ttu-id="23fde-160">נגישות וקיצורי מקשים</span><span class="sxs-lookup"><span data-stu-id="23fde-160">Accessibility and keyboard shortcuts</span></span>

<span data-ttu-id="23fde-161">הרשת **לוח זמנים** נגישה לחלוטין וניתן להשתמש בה עם קוראי מסך כמו 'קורא טקסטים', JAWS או NVDA.</span><span class="sxs-lookup"><span data-stu-id="23fde-161">The **Schedule** grid is fully accessible and can be used with screen readers such as Narrator, JAWS, or NVDA.</span></span> <span data-ttu-id="23fde-162">תוכל לזוז באזור הרשת באמצעות מקשי החצים (כמו ב- Microsoft Excel), תוכל להשתמש במקש ה- Tab כדי להתקדם באמצעות רכיבי ממשק משתמש אינטראקטיביים ותוכל להשתמש במקש החץ למטה, במקש ה- Enter או במקש הרווח כדי לבחור ולהפעיל תפריטים נפתחים.</span><span class="sxs-lookup"><span data-stu-id="23fde-162">You can move through the grid area by using arrow keys (as in Microsoft Excel), you can use the Tab key to advance through the interactive UI elements, and you can use the Down arrow key, the Enter key, or the Spacebar to select and invoke the drop-down menus.</span></span> <span data-ttu-id="23fde-163">כותרות העמודות הן גם אינטראקטיביות.</span><span class="sxs-lookup"><span data-stu-id="23fde-163">The column headers are also interactive.</span></span> <span data-ttu-id="23fde-164">באפשרותך להסתיר ולהציג עמודות, להשתמש במקש ה- Tab ובמקשי החצים כדי לעבור בין כותרות העמודות ולהשתמש בלחצני הפעולה בסרגל הכלים.</span><span class="sxs-lookup"><span data-stu-id="23fde-164">You can hide and show columns, use the Tab key and arrow keys to move through the column headers, and use the action buttons on the toolbar.</span></span> <span data-ttu-id="23fde-165">בנוסף, באפשרותך להשתמש בקיצורי המקשים הבאים:</span><span class="sxs-lookup"><span data-stu-id="23fde-165">In addition, you can use the following keyboard shortcuts:</span></span>

- <span data-ttu-id="23fde-166">**רענון**: ‏ALT+SHIFT+F5</span><span class="sxs-lookup"><span data-stu-id="23fde-166">**Refresh**: ALT+SHIFT+F5</span></span>
- <span data-ttu-id="23fde-167">**הוספה**:‏ ALT+SHIFT+Insert</span><span class="sxs-lookup"><span data-stu-id="23fde-167">**Add**: ALT+SHIFT+Insert</span></span>
- <span data-ttu-id="23fde-168">**מחיקה**: ‏ALT+SHIFT+Delete</span><span class="sxs-lookup"><span data-stu-id="23fde-168">**Delete**: ALT+SHIFT+Delete</span></span>
- <span data-ttu-id="23fde-169">**הזזה למעלה/למטה**: ‏ALT+SHIFT+חצים למעלה/למטה</span><span class="sxs-lookup"><span data-stu-id="23fde-169">**Move up/down**: ALT+SHIFT+Up/Down arrows</span></span>
- <span data-ttu-id="23fde-170">**הסטה פנימה/החוצה**: ‏ALT_SHIFT+חצים לימין/לשמאל</span><span class="sxs-lookup"><span data-stu-id="23fde-170">**Indent/Outdent**: ALT_SHIFT+Left/Right arrows</span></span>
- <span data-ttu-id="23fde-171">**הרחבה/צמצום הירארכיות**:‏ ALT+SHIFT+מקשי פלוס/מינוס</span><span class="sxs-lookup"><span data-stu-id="23fde-171">**Expand/Collapse Hierarchies**: ALT+SHIFT+Plus/Minus keys</span></span>

## <a name="task-attributes"></a><span data-ttu-id="23fde-172">תכונות המשימה</span><span class="sxs-lookup"><span data-stu-id="23fde-172">Task attributes</span></span>

<span data-ttu-id="23fde-173">שם המשימה מתאר את העבודה שיש להשלים.</span><span class="sxs-lookup"><span data-stu-id="23fde-173">A task's name describes the work that must be completed.</span></span> <span data-ttu-id="23fde-174">ב- PSA, התכונות המשויכות לפעילות מתארות את לוח הזמנים של הפעילות ואת הדרישות של האיוש.</span><span class="sxs-lookup"><span data-stu-id="23fde-174">In PSA, the attributes that are associated with a task describe the schedule of the task and its staffing requirements.</span></span>

> ![תכונות המשימה](media/project-2.png)
 
### <a name="schedule-attributes"></a><span data-ttu-id="23fde-176">תכונות של לוח זמנים</span><span class="sxs-lookup"><span data-stu-id="23fde-176">Schedule attributes</span></span>

<span data-ttu-id="23fde-177">התכונות **מאמץ**, **תאריך התחלה**, **תאריך סיום** ו**משך** מגדירות את לוח הזמנים של המשימה.</span><span class="sxs-lookup"><span data-stu-id="23fde-177">The **Effort**, **Start date**, **End date**, and **Duration** attributes define the schedule for the task.</span></span>

<span data-ttu-id="23fde-178">תכונות נוספות של לוח הזמנים כוללות:</span><span class="sxs-lookup"><span data-stu-id="23fde-178">Additional schedule attributes include:</span></span>

- <span data-ttu-id="23fde-179">**שעות מאמץ**: הזן הערכה של השעות הדרושות להשלמת המשימה.</span><span class="sxs-lookup"><span data-stu-id="23fde-179">**Effort hours**: Enter an estimate of the hours that are required to complete the task.</span></span> 
- <span data-ttu-id="23fde-180">**משך**: ציין את מספר ימי העבודה הדרושים להשלמת המשימה.</span><span class="sxs-lookup"><span data-stu-id="23fde-180">**Duration**: Specify the number of workdays that are required to complete the task.</span></span>
- <span data-ttu-id="23fde-181">**מזהה לוח הזמנים**: מזהה זה שנוצר באופן אוטומטי משמש כדי למיין משימות בהירארכיה.</span><span class="sxs-lookup"><span data-stu-id="23fde-181">**Schedule ID**: This automatically generated ID is used to order tasks in the hierarchy.</span></span> <span data-ttu-id="23fde-182">יחסי התלות בין המשימות מנהלים את הסדר בפועל שבו מעובדות המשימות.</span><span class="sxs-lookup"><span data-stu-id="23fde-182">Dependencies between the tasks manage the actual order in which the tasks are worked on.</span></span>
 
### <a name="staffing-attributes"></a><span data-ttu-id="23fde-183">תכונות איוש</span><span class="sxs-lookup"><span data-stu-id="23fde-183">Staffing attributes</span></span>

<span data-ttu-id="23fde-184">ניתן לגשת לתכונות איוש באמצעות השדה **משאבים** בלוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="23fde-184">Staffing attributes are accessed through the **Resources** field in the schedule.</span></span> <span data-ttu-id="23fde-185">תוכל לחפש משאב קיים או ללחוץ על **צור** ובחלונית **יצירה מהירה**, הוסף חבר צוות פרוייקט כמשאב חדש.</span><span class="sxs-lookup"><span data-stu-id="23fde-185">You can either search for an existing resource, or click **Create** and in the **Quick Create** pane, add a project team member as a new resource.</span></span>

<span data-ttu-id="23fde-186">השדות **תפקיד**, **‏‫יחידת הקצאת משאבים‬**, ו**שם עמדה‬** משמשים לתיאור דרישות האיוש עבור המשימה.</span><span class="sxs-lookup"><span data-stu-id="23fde-186">The **Role**, **Resourcing Unit**, and **Position Name** fields are used to describe the staffing requirements for the task.</span></span> <span data-ttu-id="23fde-187">תכונות איוש אלה יחד עם לוח הזמנים של המשימה משמשים לחיפוש משאבים זמינים לביצוע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="23fde-187">These staffing attributes together with the task schedule are used to find available resources to do this task.</span></span>

<span data-ttu-id="23fde-188">**תפקיד** - ציין את סוג המשאב הדרוש לביצוע המשימה.</span><span class="sxs-lookup"><span data-stu-id="23fde-188">**Role** - Specify the type of resource that is required to do the task.</span></span>

<span data-ttu-id="23fde-189">**יחידת הקצאת משאבים** - ציין את היחידה שממנה יש להקצות משאבים עבור המשימה.</span><span class="sxs-lookup"><span data-stu-id="23fde-189">**Resourcing unit** - Specify the unit that resources for the task should be assigned from.</span></span> <span data-ttu-id="23fde-190">תכונה זו משפיעה על הערכת העלות והמכירות עבור המשימה אם תעריף העלות והחיוב עבור המשאב מוגדרים בהתאם ל‏‫יחידות של הקצאת משאבים‬.</span><span class="sxs-lookup"><span data-stu-id="23fde-190">This attribute affects the cost and sales estimate for the task if the cost and bill rate for the resource are set based on resourcing units.</span></span>

<span data-ttu-id="23fde-191">**שם עמדה** – הזן שם ידידותי עבור המשאב הכללי שמשרת כמציין מיקום עבור המשאב שבסופו של דבר יבצע את העבודה.</span><span class="sxs-lookup"><span data-stu-id="23fde-191">**Position name** – Enter a friendly name for the generic resource that serves as a placeholder for the resource that will ultimately do the work.</span></span>

<span data-ttu-id="23fde-192">השדה **משאבים** שומר על שם העמדה של המשאב הכללי או משאב בעל שם, כאשר הוא יימצא.</span><span class="sxs-lookup"><span data-stu-id="23fde-192">The **Resources** field holds the position name of the generic resource or named resource when one is found.</span></span>

<span data-ttu-id="23fde-193">השדה **קטגוריה** שומר על הערכים שמציינים סוג עבודה רחב יותר שאליו ניתן לקבץ את המשימה.</span><span class="sxs-lookup"><span data-stu-id="23fde-193">The **Category** field holds the values that indicate a broader type of work that the task can be grouped into.</span></span> <span data-ttu-id="23fde-194">שדה זה אינו משפיע על תזמון או על איוש.</span><span class="sxs-lookup"><span data-stu-id="23fde-194">This field doesn't affect scheduling or staffing.</span></span> <span data-ttu-id="23fde-195">הוא משמש רק לדיווח.</span><span class="sxs-lookup"><span data-stu-id="23fde-195">It's used only for reporting.</span></span>

### <a name="task-dependencies"></a><span data-ttu-id="23fde-196">יחסי תלות בין משימות</span><span class="sxs-lookup"><span data-stu-id="23fde-196">Task dependencies</span></span> 

<span data-ttu-id="23fde-197">באפשרותך להשתמש בלוח הזמנים ב- PSA כדי ליצור קשרי פעילויות קדם בין משימות.</span><span class="sxs-lookup"><span data-stu-id="23fde-197">You can use the schedule in PSA to create predecessor relationships between tasks.</span></span> <span data-ttu-id="23fde-198">השדה **‏‫‏‏פעילות קדם‬** תחת **משימות** משתמש בערך אחד או יותר כדי לציין את המשימות שמשימה תלויה בהן.</span><span class="sxs-lookup"><span data-stu-id="23fde-198">The **Predecessor** field under **Tasks** takes one or more values to indicate the tasks that a task depends on.</span></span> <span data-ttu-id="23fde-199">בעת הקצאת ערכים לפעילות קדם, המשימה תוכל להתחיל רק לאחר השלמת כל המשימות של פעילויות הקדם.</span><span class="sxs-lookup"><span data-stu-id="23fde-199">When predecessor values are assigned to a task, the task can start only after all the predecessor tasks have been completed.</span></span> <span data-ttu-id="23fde-200">בשל התלות, תאריך ההתחלה המתוכנן של הפעילות מאופס לתאריך שבו הושלמו המשימות של פעילויות הקדם.</span><span class="sxs-lookup"><span data-stu-id="23fde-200">Because of the dependency, the planned start date of the task is reset to the date when the predecessor tasks are completed.</span></span>

<span data-ttu-id="23fde-201">למצב המשימה אין שום השפעה על עדכונים שמתבצעים לתאריכי ההתחלה או הסוף של משימות תלויות/פעילויות קדם.</span><span class="sxs-lookup"><span data-stu-id="23fde-201">The task mode has no effect on updates that are made to the start and end dates of predecessor/dependent tasks.</span></span>

## <a name="task-mode"></a><span data-ttu-id="23fde-202">מצב משימה</span><span class="sxs-lookup"><span data-stu-id="23fde-202">Task mode</span></span> 

<span data-ttu-id="23fde-203">מצב המשימה קובע את התזמון של משימות צומת עלה.</span><span class="sxs-lookup"><span data-stu-id="23fde-203">The task mode determines the scheduling of leaf node tasks.</span></span> <span data-ttu-id="23fde-204">PSA תומך בשני מצבי משימה עבור כל משימה: תזמון אוטומטי ותזמון ידני.</span><span class="sxs-lookup"><span data-stu-id="23fde-204">PSA supports two task modes for every task: automatic scheduling and manual scheduling.</span></span>

### <a name="auto-scheduling"></a><span data-ttu-id="23fde-205">תזמון אוטומטי</span><span class="sxs-lookup"><span data-stu-id="23fde-205">Auto-scheduling</span></span> 
 
<span data-ttu-id="23fde-206">בעת הגדרת מצב המשימה בתור **‏‫מתוזמן אוטומטית‬**, מנוע תזמון המשימות משתמש בכללי תזמון על תכונות המשימה כדי לקבוע את לוח הזמנים עבור המשימה.</span><span class="sxs-lookup"><span data-stu-id="23fde-206">When task mode is set to **Automatically Scheduled** for a task, the task scheduling engine uses the scheduling rules on task attributes to determine the schedule for the task.</span></span>

#### <a name="scheduling-rules"></a><span data-ttu-id="23fde-207">כללי תזמון</span><span class="sxs-lookup"><span data-stu-id="23fde-207">Scheduling rules</span></span>

<span data-ttu-id="23fde-208">כברירת מחדל, אם למשימה של צומת עלה אין פעילויות קדם, תאריך ההתחלה שלה נקבע לתאריך ההתחלה המתוזמן של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="23fde-208">By default, if a leaf node task doesn't have predecessors, its start date is set to the project's scheduled start date.</span></span> <span data-ttu-id="23fde-209">משך פעילות צומת עלה תמיד מחושב כמספר ימי העבודה בין תאריכי ההתחלה והסיום שלו.</span><span class="sxs-lookup"><span data-stu-id="23fde-209">The duration of a leaf node task is always calculated as the number of working days between its start and end dates.</span></span> <span data-ttu-id="23fde-210">כאשר פעילות מתוזמנת אוטומטית, מנוע התזמון פועל לפי הכללים האלו:</span><span class="sxs-lookup"><span data-stu-id="23fde-210">When a task is automatically scheduled, the scheduling engine follows these rules:</span></span>

- <span data-ttu-id="23fde-211">תאריכי ההתחלה והסיום של המשימה חייבים להיות ימי עבודה לפי לוח השנה לתזמון הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="23fde-211">The start and end dates of the task must be working days, according to the project's scheduling calendar.</span></span> 
- <span data-ttu-id="23fde-212">עבור משימות שיש להן פעילויות קדם, תאריך ההתחלה נקבע אוטומטית לתאריך הסיום האחרון של פעילויות הקדם שלה.</span><span class="sxs-lookup"><span data-stu-id="23fde-212">For any task that has predecessor tasks, the start date is automatically set to the latest end date of its predecessors.</span></span>
- <span data-ttu-id="23fde-213">המאמץ מחושב באמצעות הנוסחה הזו: מספר האנשים × משך × שעות ביום עבודה רגיל בלוח השנה של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="23fde-213">Effort is calculated by using this formula: Number of people × Duration × Hours in a standard workday in the project calendar.</span></span>

### <a name="manual-scheduling"></a><span data-ttu-id="23fde-214">תזמון ידני</span><span class="sxs-lookup"><span data-stu-id="23fde-214">Manual scheduling</span></span>

<span data-ttu-id="23fde-215">אם הכללים של תזמון אוטומטי לא עונים על הדרישות שלך, תוכל לקבוע את מצב המשימה בתור **תזמון ידני**.</span><span class="sxs-lookup"><span data-stu-id="23fde-215">If the rules of automatic scheduling don't meet your requirements, you can set the task mode for the task to **Manually Scheduled**.</span></span> <span data-ttu-id="23fde-216">הגדרה זו מפסיקה את מנוע התזמון המחשב את הערכים של תכונות תזמון אחרות.</span><span class="sxs-lookup"><span data-stu-id="23fde-216">This setting stops the scheduling engine from calculating the values of other scheduling attributes.</span></span> <span data-ttu-id="23fde-217">ללא קשר למצב המשימה, אם תגדיר פעילויות קדם בפעילויות, תמיד תשפיע על תאריך ההתחלה של המשימה התלויה.</span><span class="sxs-lookup"><span data-stu-id="23fde-217">Regardless of the task mode, if you set predecessors on tasks, you always affect the dependent task's start date.</span></span>
