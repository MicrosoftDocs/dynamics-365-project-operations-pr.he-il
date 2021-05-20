---
title: שיקולים לשדרוג עבור מבנה התפלגות העבודה
description: נושא זה מספק מידע לגבי שדרוג מבנה התפלגות העבודה מ- Project Service Automation 2.x ל- ‎3.x.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
author: ruhercul
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
ms.openlocfilehash: d31ca60b267063e9cadf544468ece501353950fa
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2021
ms.locfileid: "5951345"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a><span data-ttu-id="a488d-103">שיקולים לשדרוג עבור מבנה התפלגות העבודה</span><span class="sxs-lookup"><span data-stu-id="a488d-103">Upgrade considerations for the work breakdown structure</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="a488d-104">נושא זה מספק מידע לגבי שדרוג מבנה התפלגות העבודה מ- Project Service Automation 2.x ל- ‎3.x.</span><span class="sxs-lookup"><span data-stu-id="a488d-104">This topic provides information about upgrading the work breakdown structure from Project Service Automation 2.x to 3.x.</span></span> <span data-ttu-id="a488d-105">נושא זה מגדיר את המצב התקין של פרויקטים ב- Project Service Automation ‏(PSA) הנדרש לשדרוג מוצלח.</span><span class="sxs-lookup"><span data-stu-id="a488d-105">This topic defines the healthy state of a project in Project Service Automation (PSA) that is required for a successful upgrade.</span></span> <span data-ttu-id="a488d-106">הוא כולל גם מידע על תנאי החסימה הנפוצים שיגרמו לשדרוג להיכשל.</span><span class="sxs-lookup"><span data-stu-id="a488d-106">There is also information about the common blocking conditions that will cause upgrade to fail.</span></span> <span data-ttu-id="a488d-107">לקבלת מידע נוסף על הגדרת משימות פרויקט והפונקציות שלהן במסגרת לוח זמנים של פרויקט, ראה [לוחות זמנים של פרויקטים](project-creating.md).</span><span class="sxs-lookup"><span data-stu-id="a488d-107">For more information about defining project tasks and their functions within a project schedule, see [Project schedules](project-creating.md).</span></span>

## <a name="key-entities"></a><span data-ttu-id="a488d-108">ישויות עיקריות</span><span class="sxs-lookup"><span data-stu-id="a488d-108">Key entities</span></span>
<span data-ttu-id="a488d-109">עבור מבנה התפלגות עבודה מדויק שכבר נטענו בו משאבים, הישויות הבאות נדרשות:</span><span class="sxs-lookup"><span data-stu-id="a488d-109">For an accurate work breakdown structure that is already loaded with resources, the following entities are required:</span></span>

- [<span data-ttu-id="a488d-110">פרוייקט</span><span class="sxs-lookup"><span data-stu-id="a488d-110">Project</span></span>](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project)
- [<span data-ttu-id="a488d-111">צוות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="a488d-111">Project Team</span></span>](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam)
- [<span data-ttu-id="a488d-112">משימת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="a488d-112">Project Task</span></span>](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask)
- [<span data-ttu-id="a488d-113">הקצאות משאבים</span><span class="sxs-lookup"><span data-stu-id="a488d-113">Resource Assignments</span></span>](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment)
- [<span data-ttu-id="a488d-114">‏‫יחס תלות במשימת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="a488d-114">Project Task Dependency</span></span>](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency)
- [<span data-ttu-id="a488d-115">משאבים הניתנים להזמנה</span><span class="sxs-lookup"><span data-stu-id="a488d-115">Bookable Resources</span></span>](/dynamics365/customerengagement/on-premises/developer/entities/bookableresource)

<span data-ttu-id="a488d-116">כדי להגדיר מבנה התפלגות עבודה שנטען במשאבים, עליך להשלים את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="a488d-116">To define a resource loaded work breakdown structure, you must complete the following steps:</span></span>

1. <span data-ttu-id="a488d-117">צור פרויקט חדש.</span><span class="sxs-lookup"><span data-stu-id="a488d-117">Create a new project.</span></span> <span data-ttu-id="a488d-118">לקבלת מידע נוסף על יצירת פרוייקט חדש, ראה [msdyn_project](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).</span><span class="sxs-lookup"><span data-stu-id="a488d-118">For more information about how to create a new project, see [msdyn_project](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).</span></span>
2. <span data-ttu-id="a488d-119">צור משימה אחת או יותר.</span><span class="sxs-lookup"><span data-stu-id="a488d-119">Create one or more tasks.</span></span> <span data-ttu-id="a488d-120">לקבלת מידע נוסף על יצירת משימות, ראה [msdyn_projecttask](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).</span><span class="sxs-lookup"><span data-stu-id="a488d-120">For more information about how to create a task, see [msdyn_projecttask](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).</span></span>
3. <span data-ttu-id="a488d-121">הגדר את יחסי התלות בין המשימות.</span><span class="sxs-lookup"><span data-stu-id="a488d-121">Define the task dependencies.</span></span> <span data-ttu-id="a488d-122">למידע נוסף ראה [תלות במשימת פרוייקט](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).</span><span class="sxs-lookup"><span data-stu-id="a488d-122">For more information, see [Project Task Dependency](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).</span></span>
4. <span data-ttu-id="a488d-123">הקצה חברי צוות פרויקט לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a488d-123">Assign project team members to the project.</span></span> <span data-ttu-id="a488d-124">לקבלת מידע נוסף, ראה [msdyn_projectteam](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).</span><span class="sxs-lookup"><span data-stu-id="a488d-124">For more information, see [msdyn_projectteam](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).</span></span>
5. <span data-ttu-id="a488d-125">הקצה חברי צוות פרויקט למשימות.</span><span class="sxs-lookup"><span data-stu-id="a488d-125">Assign project team members to the tasks.</span></span> <span data-ttu-id="a488d-126">לקבלת מידע נוסף, ראה [msdyn_resourceassignment](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).</span><span class="sxs-lookup"><span data-stu-id="a488d-126">For more information, see [msdyn_resourceassignment](/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).</span></span>

## <a name="project-team-relationships"></a><span data-ttu-id="a488d-127">קשרי גומלין בצוות הפרויקט</span><span class="sxs-lookup"><span data-stu-id="a488d-127">Project team relationships</span></span>

<span data-ttu-id="a488d-128">כדי להבטיח שדרוג מוצלח, יש לשמור כראוי על קשרי הגומלין הבאים:</span><span class="sxs-lookup"><span data-stu-id="a488d-128">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>
- <span data-ttu-id="a488d-129">כל חברי צוות הפרויקט צריכים להיות משויכים למשאב הניתן להזמנה.</span><span class="sxs-lookup"><span data-stu-id="a488d-129">All project team members must be associated with a bookable resource.</span></span>
- <span data-ttu-id="a488d-130">כל חברי צוות הפרויקט צריכים להיות משויכים לאותו הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a488d-130">All project team members must be associated with the same project.</span></span> 

## <a name="project-task-relationships"></a><span data-ttu-id="a488d-131">קשרי גומלין במשימות הפרויקט</span><span class="sxs-lookup"><span data-stu-id="a488d-131">Project task relationships</span></span>
<span data-ttu-id="a488d-132">כדי להבטיח שדרוג מוצלח, יש לשמור כראוי על קשרי הגומלין הבאים:</span><span class="sxs-lookup"><span data-stu-id="a488d-132">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="a488d-133">כל המשימות הקשורות חייבות להיות משויכות לאותו הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a488d-133">Any related tasks must be associated with the same project.</span></span>
- <span data-ttu-id="a488d-134">כל משימת שורה צריכה משימת אב.</span><span class="sxs-lookup"><span data-stu-id="a488d-134">Every line task must have a parent task.</span></span>
- <span data-ttu-id="a488d-135">כל משימה צריכה פרויקט אב.</span><span class="sxs-lookup"><span data-stu-id="a488d-135">Every task must have a parent project.</span></span>

### <a name="valid-conditions"></a><span data-ttu-id="a488d-136">תנאים חוקיים</span><span class="sxs-lookup"><span data-stu-id="a488d-136">Valid conditions</span></span>

- <span data-ttu-id="a488d-137">כל משכי הזמן של המשימות חייבים להיות גדולים משעה אחת או שווים לה (>=) וקטנים מ- 1,800,000 דקות (1,250 ימים).\*</span><span class="sxs-lookup"><span data-stu-id="a488d-137">All task durations must be greater than or equal to (>=) one hour and less than 1,800,000 minutes (1,250 days).\*</span></span>
- <span data-ttu-id="a488d-138">תאריך ההתחלה של כל המשימות חייב להתקיים ב- 01/01/2000 או לאחר מכן.\*</span><span class="sxs-lookup"><span data-stu-id="a488d-138">All tasks must have a start date no earlier than 2000/01/01.\*</span></span>
- <span data-ttu-id="a488d-139">תאריך ההתחלה של כל המשימות חייב להתקיים 17 שנה לכל היותר מהתאריך הנוכחי.\*</span><span class="sxs-lookup"><span data-stu-id="a488d-139">All tasks must have a start date no later than 17 years from the present day.\*</span></span>
- <span data-ttu-id="a488d-140">תאריך ההתחלה של כל המשימות חייב להתקיים לפני תאריך הסיום או בתאריך הסיום.</span><span class="sxs-lookup"><span data-stu-id="a488d-140">All tasks must have a start date earlier or equal to their finish date.</span></span>
- <span data-ttu-id="a488d-141">כל סוגי העסקאות בסיווגים ('הוצאה', 'חומר', 'מס' ו'זמן') חייבים להכיל ערכים של **יחידת ברירת מחדל** ו **קבוצת יחידות**.</span><span class="sxs-lookup"><span data-stu-id="a488d-141">All transaction types on classifications (Expense, Material, Tax, and Time) must have values for **Default Unit** and **Unit Group**.</span></span>
- <span data-ttu-id="a488d-142">יש להימנע מתבניות תאריך הכוללות אותיות.</span><span class="sxs-lookup"><span data-stu-id="a488d-142">Date formats with letters should be avoided.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="a488d-143">שלבים פוטנציאליים לצמצום סיכונים</span><span class="sxs-lookup"><span data-stu-id="a488d-143">Potential mitigation steps</span></span>
- <span data-ttu-id="a488d-144">השתמש בחיפוש מתקדם כדי לזהות משימות פרויקט שאינן מכילות מזהה פרויקט.</span><span class="sxs-lookup"><span data-stu-id="a488d-144">Use Advanced Find to identify Project tasks that do not contain a Project ID.</span></span>
- <span data-ttu-id="a488d-145">השתמש בחיפוש מתקדם כדי לזהות משימות פרויקט שבהן משך הזמן המתוזמן גדול מ- 1,800,000.</span><span class="sxs-lookup"><span data-stu-id="a488d-145">Use Advanced Find to identify Project tasks where the scheduled duration is greater than > 1,800,000.</span></span>
- <span data-ttu-id="a488d-146">לפני ביצוע שינויים בנתונים, עליך לבדוק התאמות אישיות הקשורות לישות שעלולות לפגוע במצב הנתונים.</span><span class="sxs-lookup"><span data-stu-id="a488d-146">Prior to making any data changes, you should investigate any customizations associated with the entity that may have led to getting the data into a bad state.</span></span> <span data-ttu-id="a488d-147">יש להתייחס להתאמות אישיות אלה לפני שתמשיך בעדכונים הקשורים לנתונים.</span><span class="sxs-lookup"><span data-stu-id="a488d-147">These customizations should be addressed before proceeding with any data-related updates.</span></span>
- <span data-ttu-id="a488d-148">עבור המשימות שזוהו שהתייתמו, שקול למחוק משימות אלה אם אין בהן צורך יותר או אם יש לשייך אותן לפרויקט ההורה הנכון.</span><span class="sxs-lookup"><span data-stu-id="a488d-148">For the identified tasks that have been orphaned, consider deleting these tasks if they are not needed or if they should be associated with the correct parent project.</span></span>
- <span data-ttu-id="a488d-149">עבור משימות שבהן משך הזמן הוא מעל 1,250 יום, שקול להוסיף משימות מרובות כדי לייצג את משך הזמן הכולל, אם הדבר אפשרי.</span><span class="sxs-lookup"><span data-stu-id="a488d-149">For any tasks where the duration is greater than 1,250 days, consider adding multiple tasks to represent the total duration, if feasible.</span></span>

> [!NOTE]
> <span data-ttu-id="a488d-150">לפריטים שצוינו בכוכבית (\*) יש מגבלות הקשורות לכך שניהול קשרי לקוחות (CRM) תומך רק ב- 7,320 הרחבות מופע חוזר.</span><span class="sxs-lookup"><span data-stu-id="a488d-150">Items noted with an asterisk (\*) have limits that are due to the fact that customer relationship management (CRM) supports only 7,320 recurrence expansions.</span></span> <span data-ttu-id="a488d-151">יש להישאר מתחת למגבלה זו.</span><span class="sxs-lookup"><span data-stu-id="a488d-151">You must stay below this limit.</span></span>

## <a name="resource-assignment-relationships"></a><span data-ttu-id="a488d-152">קשרי גומלין של הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="a488d-152">Resource Assignment relationships</span></span>
<span data-ttu-id="a488d-153">כדי להבטיח שדרוג מוצלח, יש לשמור כראוי על קשרי הגומלין הבאים:</span><span class="sxs-lookup"><span data-stu-id="a488d-153">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="a488d-154">כל הקצאות המשאבים במבנה התפלגות העבודה חייבות להיות קשורות לאותו הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a488d-154">All Resource Assignments in a work breakdown structure must be related to the same project.</span></span>
- <span data-ttu-id="a488d-155">כל הקצאות המשאבים במבנה התפלגות העבודה חייבות להיות משויכות לחברי צוות הפרויקט באותו הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a488d-155">All Resource Assignments in a work breakdown structure must be associated to project team members in the same project.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="a488d-156">שלבים פוטנציאליים לצמצום סיכונים</span><span class="sxs-lookup"><span data-stu-id="a488d-156">Potential mitigation steps</span></span>
- <span data-ttu-id="a488d-157">זהה את כל המשימות שאינן תואמות לתנאים המתוארים לעיל.</span><span class="sxs-lookup"><span data-stu-id="a488d-157">Identify all tasks that fall outside the conditions described above.</span></span>  
- <span data-ttu-id="a488d-158">יש למחוק את כל מטלות המשאבים שאינן תקפות עוד.</span><span class="sxs-lookup"><span data-stu-id="a488d-158">Any Resource Assignments that are no longer valid should be deleted.</span></span>

## <a name="project-task-dependency-relationships"></a><span data-ttu-id="a488d-159">קשרי גומלין של יחסי תלות של משימות הפרויקט</span><span class="sxs-lookup"><span data-stu-id="a488d-159">Project task dependency relationships</span></span>
<span data-ttu-id="a488d-160">כדי להבטיח שדרוג מוצלח, יש לשמור כראוי על קשרי הגומלין הבאים:</span><span class="sxs-lookup"><span data-stu-id="a488d-160">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="a488d-161">כל יחסי התלות של משימות הפרויקט חייבים להיות קשורים לאותו הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a488d-161">All project task dependencies must be related to the same project.</span></span>
- <span data-ttu-id="a488d-162">לא ניתן להפנות לאותם יחסי תלות של משימות יותר מפעם אחת.</span><span class="sxs-lookup"><span data-stu-id="a488d-162">A task can't have the same dependency referenced more than once.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]