---
title: שיקולים לשדרוג עבור מבנה התפלגות העבודה
description: נושא זה מספק מידע לגבי שדרוג מבנה התפלגות העבודה מ- Project Service Automation 2.x ל- ‎3.x.
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
ms.prod: ''
ms.technology: Dynamics 365 Project Service Automation 2.x
author: ruhercul
ms.assetid: 9e43d5b5-ca5d-41f5-9012-c48f8e3080f9
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 9aa35dd8784bfa55737b0836e653afd0442b80c2
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751842"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a><span data-ttu-id="695ba-103">שיקולים לשדרוג עבור מבנה התפלגות העבודה</span><span class="sxs-lookup"><span data-stu-id="695ba-103">Upgrade considerations for the work breakdown structure</span></span>
<span data-ttu-id="695ba-104">נושא זה מספק מידע לגבי שדרוג מבנה התפלגות העבודה מ- Project Service Automation 2.x ל- ‎3.x.</span><span class="sxs-lookup"><span data-stu-id="695ba-104">This topic provides information about upgrading the work breakdown structure from Project Service Automation 2.x to 3.x.</span></span> <span data-ttu-id="695ba-105">נושא זה מגדיר את המצב התקין של פרוייקטים ב- Project Service Automation ‏(PSA) הנדרש לשדרוג מוצלח.</span><span class="sxs-lookup"><span data-stu-id="695ba-105">This topic defines the healthy state of a project in Project Service Automation (PSA) that is required for a successful upgrade.</span></span> <span data-ttu-id="695ba-106">הוא כולל גם מידע על תנאי החסימה הנפוצים שיגרמו לשדרוג להיכשל.</span><span class="sxs-lookup"><span data-stu-id="695ba-106">There is also information about the common blocking conditions that will cause upgrade to fail.</span></span> <span data-ttu-id="695ba-107">לקבלת מידע נוסף על הגדרת משימות פרוייקט והפונקציות שלהן במסגרת לוח זמנים של פרוייקט, ראה [לוחות זמנים של פרוייקטים](project-creating.md).</span><span class="sxs-lookup"><span data-stu-id="695ba-107">For more information about defining project tasks and their functions within a project schedule, see [Project schedules](project-creating.md).</span></span>

## <a name="key-entities"></a><span data-ttu-id="695ba-108">ישויות עיקריות</span><span class="sxs-lookup"><span data-stu-id="695ba-108">Key entities</span></span>
<span data-ttu-id="695ba-109">עבור מבנה התפלגות עבודה מדויק שכבר נטענו בו משאבים, הישויות הבאות נדרשות:</span><span class="sxs-lookup"><span data-stu-id="695ba-109">For an accurate work breakdown structure that is already loaded with resources, the following entities are required:</span></span>

- [<span data-ttu-id="695ba-110">פרוייקט</span><span class="sxs-lookup"><span data-stu-id="695ba-110">Project</span></span>](../developer/entities/msdyn_project.md)
- [<span data-ttu-id="695ba-111">צוות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="695ba-111">Project Team</span></span>](../developer/entities/msdyn_projectteam.md)
- [<span data-ttu-id="695ba-112">משימת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="695ba-112">Project Task</span></span>](../developer/entities/msdyn_projecttask.md)
- [<span data-ttu-id="695ba-113">הקצאות משאבים</span><span class="sxs-lookup"><span data-stu-id="695ba-113">Resource Assignments</span></span>](../developer/entities/msdyn_resourceassignment.md)
- [<span data-ttu-id="695ba-114">‏‫יחס תלות במשימת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="695ba-114">Project Task Dependency</span></span>](../developer/entities/msdyn_projecttaskdependency.md)
- [<span data-ttu-id="695ba-115">משאבים הניתנים להזמנה</span><span class="sxs-lookup"><span data-stu-id="695ba-115">Bookable Resources</span></span>](../developer/entities/bookableresource.md)

<span data-ttu-id="695ba-116">כדי להגדיר מבנה התפלגות עבודה שנטען במשאבים, עליך להשלים את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="695ba-116">To define a resource loaded work breakdown structure, you must complete the following steps:</span></span>

1. <span data-ttu-id="695ba-117">צור פרוייקט חדש.</span><span class="sxs-lookup"><span data-stu-id="695ba-117">Create a new project.</span></span> <span data-ttu-id="695ba-118">לקבלת מידע נוסף על יצירת פרוייקט חדש, ראה [msdyn_project](../developer/entities/msdyn_project.md).</span><span class="sxs-lookup"><span data-stu-id="695ba-118">For more information about how to create a new project, see [msdyn_project](../developer/entities/msdyn_project.md).</span></span>
2. <span data-ttu-id="695ba-119">צור משימה אחת או יותר.</span><span class="sxs-lookup"><span data-stu-id="695ba-119">Create one or more tasks.</span></span> <span data-ttu-id="695ba-120">לקבלת מידע נוסף על יצירת משימות, ראה [msdyn_projecttask](../developer/entities/msdyn_projecttask.md).</span><span class="sxs-lookup"><span data-stu-id="695ba-120">For more information about how to create a task, see [msdyn_projecttask](../developer/entities/msdyn_projecttask.md).</span></span>
3. <span data-ttu-id="695ba-121">הגדר את יחסי התלות בין המשימות.</span><span class="sxs-lookup"><span data-stu-id="695ba-121">Define the task dependencies.</span></span> <span data-ttu-id="695ba-122">למידע נוסף ראה [תלות במשימת פרוייקט](../developer/entities/msdyn_projecttaskdependency.md).</span><span class="sxs-lookup"><span data-stu-id="695ba-122">For more information, see [Project Task Dependency](../developer/entities/msdyn_projecttaskdependency.md).</span></span>
4. <span data-ttu-id="695ba-123">הקצה חברי צוות פרוייקט לפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="695ba-123">Assign project team members to the project.</span></span> <span data-ttu-id="695ba-124">לקבלת מידע נוסף, ראה [msdyn_projectteam](../developer/entities/msdyn_projectteam.md).</span><span class="sxs-lookup"><span data-stu-id="695ba-124">For more information, see [msdyn_projectteam](../developer/entities/msdyn_projectteam.md).</span></span>
5. <span data-ttu-id="695ba-125">הקצה חברי צוות פרוייקט למשימות.</span><span class="sxs-lookup"><span data-stu-id="695ba-125">Assign project team members to the tasks.</span></span> <span data-ttu-id="695ba-126">לקבלת מידע נוסף, ראה [msdyn_resourceassignment](../developer/entities/msdyn_resourceassignment.md).</span><span class="sxs-lookup"><span data-stu-id="695ba-126">For more information, see [msdyn_resourceassignment](../developer/entities/msdyn_resourceassignment.md).</span></span>

## <a name="project-team-relationships"></a><span data-ttu-id="695ba-127">קשרי גומלין בצוות הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="695ba-127">Project team relationships</span></span>

<span data-ttu-id="695ba-128">כדי להבטיח שדרוג מוצלח, יש לשמור כראוי על קשרי הגומלין הבאים:</span><span class="sxs-lookup"><span data-stu-id="695ba-128">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>
- <span data-ttu-id="695ba-129">כל חברי צוות הפרוייקט צריכים להיות משויכים למשאב הניתן להזמנה.</span><span class="sxs-lookup"><span data-stu-id="695ba-129">All project team members must be associated with a bookable resource.</span></span>
- <span data-ttu-id="695ba-130">כל חברי צוות הפרוייקט צריכים להיות משויכים לאותו הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="695ba-130">All project team members must be associated with the same project.</span></span> 

## <a name="project-task-relationships"></a><span data-ttu-id="695ba-131">קשרי גומלין במשימות הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="695ba-131">Project task relationships</span></span>
<span data-ttu-id="695ba-132">כדי להבטיח שדרוג מוצלח, יש לשמור כראוי על קשרי הגומלין הבאים:</span><span class="sxs-lookup"><span data-stu-id="695ba-132">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="695ba-133">כל המשימות הקשורות חייבות להיות משויכות לאותו הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="695ba-133">Any related tasks must be associated with the same project.</span></span>
- <span data-ttu-id="695ba-134">כל משימת שורה צריכה משימת אב.</span><span class="sxs-lookup"><span data-stu-id="695ba-134">Every line task must have a parent task.</span></span>
- <span data-ttu-id="695ba-135">כל משימה צריכה פרוייקט אב.</span><span class="sxs-lookup"><span data-stu-id="695ba-135">Every task must have a parent project.</span></span>

### <a name="valid-conditions"></a><span data-ttu-id="695ba-136">תנאים חוקיים</span><span class="sxs-lookup"><span data-stu-id="695ba-136">Valid conditions</span></span>

- <span data-ttu-id="695ba-137">כל משכי הזמן של המשימות חייבים להיות גדולים משעה אחת או שווים לה (>=) וקטנים מ- 1,800,000 דקות (1,250 ימים).\*</span><span class="sxs-lookup"><span data-stu-id="695ba-137">All task durations must be greater than or equal to (>=) one hour and less than 1,800,000 minutes (1,250 days).\*</span></span>
- <span data-ttu-id="695ba-138">תאריך ההתחלה של כל המשימות חייב להתקיים ב- 01/01/2000 או לאחר מכן.\*</span><span class="sxs-lookup"><span data-stu-id="695ba-138">All tasks must have a start date no earlier than 2000/01/01.\*</span></span>
- <span data-ttu-id="695ba-139">תאריך ההתחלה של כל המשימות חייב להתקיים 17 שנה לכל היותר מהתאריך הנוכחי.\*</span><span class="sxs-lookup"><span data-stu-id="695ba-139">All tasks must have a start date no later than 17 years from the present day.\*</span></span>
- <span data-ttu-id="695ba-140">תאריך ההתחלה של כל המשימות חייב להתקיים לפני תאריך הסיום או בתאריך הסיום.</span><span class="sxs-lookup"><span data-stu-id="695ba-140">All tasks must have a start date earlier or equal to their finish date.</span></span>
- <span data-ttu-id="695ba-141">כל סוגי העסקאות בסיווגים ('הוצאה', 'חומר', 'מס' ו'זמן') חייבים להכיל ערכים של **יחידת ברירת מחדל** ו**קבוצת יחידות**.</span><span class="sxs-lookup"><span data-stu-id="695ba-141">All transaction types on classifications (Expense, Material, Tax, and Time) must have values for **Default Unit** and **Unit Group**.</span></span>
- <span data-ttu-id="695ba-142">יש להימנע מתבניות תאריך הכוללות אותיות.</span><span class="sxs-lookup"><span data-stu-id="695ba-142">Date formats with letters should be avoided.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="695ba-143">שלבים פוטנציאליים לצמצום סיכונים</span><span class="sxs-lookup"><span data-stu-id="695ba-143">Potential mitigation steps</span></span>
- <span data-ttu-id="695ba-144">השתמש בחיפוש מתקדם כדי לזהות משימות פרוייקט שאינן מכילות מזהה פרויקט.</span><span class="sxs-lookup"><span data-stu-id="695ba-144">Use Advanced Find to identify Project tasks that do not contain a Project ID.</span></span>
- <span data-ttu-id="695ba-145">השתמש בחיפוש מתקדם כדי לזהות משימות פרויקט שבהן משך הזמן המתוזמן גדול מ- 1,800,000.</span><span class="sxs-lookup"><span data-stu-id="695ba-145">Use Advanced Find to identify Project tasks where the scheduled duration is greater than > 1,800,000.</span></span>
- <span data-ttu-id="695ba-146">לפני ביצוע שינויים בנתונים, עליך לבדוק התאמות אישיות הקשורות לישות שעלולות לפגוע במצב הנתונים.</span><span class="sxs-lookup"><span data-stu-id="695ba-146">Prior to making any data changes, you should investigate any customizations associated with the entity that may have led to getting the data into a bad state.</span></span> <span data-ttu-id="695ba-147">יש להתייחס להתאמות אישיות אלה לפני שתמשיך בעדכונים הקשורים לנתונים.</span><span class="sxs-lookup"><span data-stu-id="695ba-147">These customizations should be addressed before proceeding with any data-related updates.</span></span>
- <span data-ttu-id="695ba-148">עבור המשימות שזוהו שהתייתמו, שקול למחוק משימות אלה אם אין בהן צורך יותר או אם יש לשייך אותן לפרוייקט ההורה הנכון.</span><span class="sxs-lookup"><span data-stu-id="695ba-148">For the identified tasks that have been orphaned, consider deleting these tasks if they are not needed or if they should be associated with the correct parent project.</span></span>
- <span data-ttu-id="695ba-149">עבור משימות שבהן משך הזמן הוא מעל 1,250 יום, שקול להוסיף משימות מרובות כדי לייצג את משך הזמן הכולל, אם הדבר אפשרי.</span><span class="sxs-lookup"><span data-stu-id="695ba-149">For any tasks where the duration is greater than 1,250 days, consider adding multiple tasks to represent the total duration, if feasible.</span></span>

> [!NOTE]
> <span data-ttu-id="695ba-150">לפריטים שצוינו בכוכבית (\*) יש מגבלות הקשורות לכך שניהול קשרי לקוחות (CRM) תומך רק ב- 7,320 הרחבות מופע חוזר.</span><span class="sxs-lookup"><span data-stu-id="695ba-150">Items noted with an asterisk (\*) have limits that are due to the fact that customer relationship management (CRM) supports only 7,320 recurrence expansions.</span></span> <span data-ttu-id="695ba-151">יש להישאר מתחת למגבלה זו.</span><span class="sxs-lookup"><span data-stu-id="695ba-151">You must stay below this limit.</span></span>

## <a name="resource-assignment-relationships"></a><span data-ttu-id="695ba-152">קשרי גומלין של הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="695ba-152">Resource Assignment relationships</span></span>
<span data-ttu-id="695ba-153">כדי להבטיח שדרוג מוצלח, יש לשמור כראוי על קשרי הגומלין הבאים:</span><span class="sxs-lookup"><span data-stu-id="695ba-153">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="695ba-154">כל הקצאות המשאבים במבנה התפלגות העבודה חייבות להיות קשורות לאותו הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="695ba-154">All Resource Assignments in a work breakdown structure must be related to the same project.</span></span>
- <span data-ttu-id="695ba-155">כל הקצאות המשאבים במבנה התפלגות העבודה חייבות להיות משויכות לחברי צוות הפרוייקט באותו הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="695ba-155">All Resource Assignments in a work breakdown structure must be associated to project team members in the same project.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="695ba-156">שלבים פוטנציאליים לצמצום סיכונים</span><span class="sxs-lookup"><span data-stu-id="695ba-156">Potential mitigation steps</span></span>
- <span data-ttu-id="695ba-157">זהה את כל המשימות שאינן תואמות לתנאים המתוארים לעיל.</span><span class="sxs-lookup"><span data-stu-id="695ba-157">Identify all tasks that fall outside the conditions described above.</span></span>  
- <span data-ttu-id="695ba-158">יש למחוק את כל מטלות המשאבים שאינן תקפות עוד.</span><span class="sxs-lookup"><span data-stu-id="695ba-158">Any Resource Assignments that are no longer valid should be deleted.</span></span>

## <a name="project-task-dependency-relationships"></a><span data-ttu-id="695ba-159">קשרי גומלין של יחסי תלות של משימות הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="695ba-159">Project task dependency relationships</span></span>
<span data-ttu-id="695ba-160">כדי להבטיח שדרוג מוצלח, יש לשמור כראוי על קשרי הגומלין הבאים:</span><span class="sxs-lookup"><span data-stu-id="695ba-160">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="695ba-161">כל יחסי התלות של משימות הפרוייקט חייבים להיות קשורים לאותו הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="695ba-161">All project task dependencies must be related to the same project.</span></span>
- <span data-ttu-id="695ba-162">לא ניתן להפנות לאותם יחסי תלות של משימות יותר מפעם אחת.</span><span class="sxs-lookup"><span data-stu-id="695ba-162">A task can't have the same dependency referenced more than once.</span></span>
