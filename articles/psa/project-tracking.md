---
title: התקדמות בפרויקט וצריכת עלויות
description: נושא זו מספק מידע כיצד ניתן לעקוב אחר התקדמות הפרויקט וצריכת העלות.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 08/21/2020
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
ms.openlocfilehash: 0793ee0c75bcbdde0fd92a16634457f73f872b5e
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4120634"
---
# <a name="project-progress-and-cost-consumption"></a><span data-ttu-id="1eed6-103">התקדמות בפרויקט וצריכת עלויות</span><span class="sxs-lookup"><span data-stu-id="1eed6-103">Project progress and cost consumption</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="1eed6-104">הצורך לעקוב אחר ההתקדמות מול לוח זמנים משתנה לפי ענף.</span><span class="sxs-lookup"><span data-stu-id="1eed6-104">The need to track progress against a schedule varies by industry.</span></span> <span data-ttu-id="1eed6-105">תעשיות מסוימות עוקבות ברמה מפורטת, ואילו תעשיות אחרות עוקבות ברמה גבוהה יותר.</span><span class="sxs-lookup"><span data-stu-id="1eed6-105">Some industries track at a granular level, whereas other industries track at a higher level.</span></span> <span data-ttu-id="1eed6-106">נושא זה מראה כיצד ליצור לוח זמנים שיעמוד בדרישות הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="1eed6-106">This topic shows how to schedule in order to meet your organization's requirements.</span></span>

## <a name="effort-tracking-view"></a><span data-ttu-id="1eed6-107">תצוגה של מעקב אחר המאמץ</span><span class="sxs-lookup"><span data-stu-id="1eed6-107">Effort tracking view</span></span>

<span data-ttu-id="1eed6-108">התצוגה **מעקב אחר מאמץ** עוקבת אחר ההתקדמות של משימות בלוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="1eed6-108">The **Effort tracking** view tracks the progress of tasks in the schedule.</span></span> <span data-ttu-id="1eed6-109">היא משווה בין השעות בפועל שהושקעו בפעילות לבין מספר השעות המתוכננות של הפעילות.</span><span class="sxs-lookup"><span data-stu-id="1eed6-109">It compares the actual effort hours spent on a task to the task's planned effort hours.</span></span> <span data-ttu-id="1eed6-110">Project Service Automation משתמש בנוסחאות הבאות כדי לחשב את מדדי המעקב:</span><span class="sxs-lookup"><span data-stu-id="1eed6-110">Project Service Automation uses the following formulas to calculate the tracking metrics:</span></span>

<span data-ttu-id="1eed6-111">בתחילה ביצירת המשימות: העלות המתוכננת תוגדר לעלות המשוערת בסיום.</span><span class="sxs-lookup"><span data-stu-id="1eed6-111">Initially on the task creation: Planned cost will be set to the Estimated cost at complete.</span></span> <span data-ttu-id="1eed6-112">לאחר שנרשמו ‏‫נתונים בפועל‬ במשימה, הדבר הבא יהיה חישוב בתצוגת המעקב אחר מאמץ</span><span class="sxs-lookup"><span data-stu-id="1eed6-112">Once Actuals are recorded on the task, the following will be calculation on the Tracking view for Effort</span></span>

- <span data-ttu-id="1eed6-113">אחוזי התקדמות = מאמץ בפועל שנעשה עד היום + הערכה בעת סיום (EAC)</span><span class="sxs-lookup"><span data-stu-id="1eed6-113">Progress percentage = Actual effort spent to date ÷ Estimate at complete (EAC)</span></span> 
- <span data-ttu-id="1eed6-114">הערכה במלואה (ETC) = אומדן בהשלמה (EAC) - מאמץ בפועל שהושקע עד היום</span><span class="sxs-lookup"><span data-stu-id="1eed6-114">Estimate to complete (ETC) = Estimate at complete (EAC)  – Actual effort spent to date</span></span> 
- <span data-ttu-id="1eed6-115">EAC = מאמץ שנותר + מאמץ בפועל שהושקע עד היום</span><span class="sxs-lookup"><span data-stu-id="1eed6-115">EAC = Remaining effort + Actual effort spent to date</span></span> 
- <span data-ttu-id="1eed6-116">סטיית מאמץ חזוי = מאמץ מתוכנן – EAC</span><span class="sxs-lookup"><span data-stu-id="1eed6-116">Projected effort variance = Planned effort – EAC</span></span>

<span data-ttu-id="1eed6-117">Project Service Automation מציג תחזית לשונות של המאמצים במשימה.</span><span class="sxs-lookup"><span data-stu-id="1eed6-117">Project Service Automation shows a projection of the effort variance on the task.</span></span> <span data-ttu-id="1eed6-118">אם ה- EAC הוא יותר מהמאמץ המתוכנן, המשימה מתוכננת להימשך זמן רב יותר ממה שתוכנן במקור.</span><span class="sxs-lookup"><span data-stu-id="1eed6-118">If the EAC is more than the planned effort, the task is projected to take more time than was originally planned.</span></span> <span data-ttu-id="1eed6-119">לכן היא תפגר בלוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="1eed6-119">Therefore, it's behind schedule.</span></span> <span data-ttu-id="1eed6-120">אם ה- EAC הוא פחות מהמאמץ המתוכנן, המשימה מתוכננת להימשך פחות זמן ממה שתוכנן במקור.</span><span class="sxs-lookup"><span data-stu-id="1eed6-120">If the EAC is less than the planned effort, the task is projected to take less time than was originally planned.</span></span> <span data-ttu-id="1eed6-121">לכן היא מקדימה את לוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="1eed6-121">Therefore, it's ahead of schedule.</span></span>

## <a name="reprojecting-effort"></a><span data-ttu-id="1eed6-122">חיזוי מחדש למאמץ</span><span class="sxs-lookup"><span data-stu-id="1eed6-122">Reprojecting effort</span></span>

<span data-ttu-id="1eed6-123">מקובל שמנהל פרויקט ישנה את ההערכות המקוריות במשימה.</span><span class="sxs-lookup"><span data-stu-id="1eed6-123">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="1eed6-124">חיזויים מחדש של פרויקט הם תפיסות של מנהל הפרויקט להערכות, בהינתן המצב הנוכחי של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="1eed6-124">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="1eed6-125">אולם, אנחנו לא ממליצים למנהל הפרויקט לשנות את המספרים הבסיסיים, מכיוון שבסיס הפרויקט מייצג את מקור האמת המבוסס של הערכת העלות ולוח הזמנים של הפרויקט, וכל בעלי העניין של הפרויקט הסכימו עליו.</span><span class="sxs-lookup"><span data-stu-id="1eed6-125">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="1eed6-126">קיימות שתי דרכים שבהן מנהל פרויקט יכול לבצע חיזוי מחדש של מאמץ במשימות:</span><span class="sxs-lookup"><span data-stu-id="1eed6-126">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="1eed6-127">עקוף את ה- ETC שבברירת מחדל בעזרת הערכה חדשה של המאמץ בפועל שנותר במשימה.</span><span class="sxs-lookup"><span data-stu-id="1eed6-127">Override the default ETC with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="1eed6-128">עקוף את אחוז ההתקדמות שבברירת מחדל בעזרת הערכה חדשה של ההתקדמות האמיתית במשימה.</span><span class="sxs-lookup"><span data-stu-id="1eed6-128">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="1eed6-129">כל אחת מהגישות האלו גורמת לחישוב מחדש של ה- ETC, ‏EAC ואחוז ההתקדמות במשימה ושל סטיית המאמץ החזוי במשימה.</span><span class="sxs-lookup"><span data-stu-id="1eed6-129">Each of these approaches cause a recalculation of the task's ETC, EAC, and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="1eed6-130">ה- EAC, ‏ETC ואחוז ההתקדמות בפעילויות הערסל מחושבים גם כן, ומפיקים חיזוי חדש לסטיית המאמץ.</span><span class="sxs-lookup"><span data-stu-id="1eed6-130">The EAC, ETC, and progress percentage on the summary tasks are also recalculated, and produce a new projection of effort variance.</span></span>

## <a name="reprojection-of-effort-on-summary-tasks"></a><span data-ttu-id="1eed6-131">חיזוי מחדש של מאמץ בפעילויות ערסל</span><span class="sxs-lookup"><span data-stu-id="1eed6-131">Reprojection of effort on summary tasks</span></span>

<span data-ttu-id="1eed6-132">ניתן ליצור חיזוי מחדש למאמץ בפעילויות ערבול או במשימות של גורמים מכילים.</span><span class="sxs-lookup"><span data-stu-id="1eed6-132">Effort on summary tasks or container tasks can be reprojected.</span></span> <span data-ttu-id="1eed6-133">בין אם המשתמש מבצע חיזוי מחדש באמצעות המאמץ שנותר או אחוז ההתקדמות בפעילויות ערסל, קבוצת החישובים הבאה מתחילה:</span><span class="sxs-lookup"><span data-stu-id="1eed6-133">Regardless of whether the user reprojects by using the remaining effort or the progress percentage on the summary tasks, the following set of calculations begins:</span></span>

- <span data-ttu-id="1eed6-134">מתבצע חישוב ל- EAC,‏‏ ל- ETC ולאחוז ההתקדמות במשימה.</span><span class="sxs-lookup"><span data-stu-id="1eed6-134">The EAC, ETC, and progress percentage on the task are calculated.</span></span>
- <span data-ttu-id="1eed6-135">ה- EAC החדש מופץ לפעילויות הצאצא ביחס זהה לזה שהיה ב- EAC המקורי בפעילות.</span><span class="sxs-lookup"><span data-stu-id="1eed6-135">The new EAC is distributed down to the child tasks in the same proportion as the original EAC was on the task.</span></span>
- <span data-ttu-id="1eed6-136">ה- EAC החדש מחושב בכל אחת מהפעילויות הבודדות עד לפעילויות של צומת העלה.</span><span class="sxs-lookup"><span data-stu-id="1eed6-136">The new EAC on each of the individual tasks down to the leaf node tasks is calculated.</span></span> 
- <span data-ttu-id="1eed6-137">החישוב מחדש של ETC ואחוז התקדמות בפעילויות הצאצא המושפעות עד לצמתי העלה מתבסס על ערך ה- EAC.</span><span class="sxs-lookup"><span data-stu-id="1eed6-137">The affected child tasks down to the leaf nodes have their ETC and progress percentage recalculated based on the EAC value.</span></span> <span data-ttu-id="1eed6-138">התוצאה היא חיזוי חדש עבור סטיית המאמץ של הפעילות.</span><span class="sxs-lookup"><span data-stu-id="1eed6-138">This results in a new projection for the effort variance of the task.</span></span> 
- <span data-ttu-id="1eed6-139">מתבצע חישוב מחדש להערכות ה- EAC של פעילויות הערסל ועד לצומת הבסיס.</span><span class="sxs-lookup"><span data-stu-id="1eed6-139">The EACs of the summary tasks all the way to the root node are recalculated.</span></span>

### <a name="cost-tracking-view"></a><span data-ttu-id="1eed6-140">תצוגת מעקב עלות</span><span class="sxs-lookup"><span data-stu-id="1eed6-140">Cost tracking view</span></span> 

<span data-ttu-id="1eed6-141">התצוגה **מעקב עלות** משווה בין העלות בפועל שהושקעה לעלות המתוכננת.</span><span class="sxs-lookup"><span data-stu-id="1eed6-141">The **Cost tracking** view compares the actual cost that was spent on a task to the planned cost.</span></span> 

> [!NOTE]
> <span data-ttu-id="1eed6-142">תצוגה זו מציגה רק עלויות עבודה ואינה כוללת עלויות מהערכת ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="1eed6-142">This view shows only labor costs and doesn’t include costs from the expense estimates.</span></span> 

<span data-ttu-id="1eed6-143">Project Service Automation משתמש בנוסחאות הבאות כדי לחשב את מדדי המעקב:</span><span class="sxs-lookup"><span data-stu-id="1eed6-143">Project Service Automation uses the following formulas to calculate the tracking metrics:</span></span>

<span data-ttu-id="1eed6-144">כאשר נוצרת משימה, העלות המתוכננת שווה לעלות המשוערת בסיום.</span><span class="sxs-lookup"><span data-stu-id="1eed6-144">When a task is created, the planned cost is equal to the estimated cost at complete.</span></span> <span data-ttu-id="1eed6-145">לאחר רישום ‏‫נתונים בפועל‬ במשימה, הנתונים הבאים מחושבים בתצוגת **מעקב** אחר עלות:</span><span class="sxs-lookup"><span data-stu-id="1eed6-145">After actuals are recorded on the task, the following is calculated on the **Tracking** view for cost:</span></span>

 - <span data-ttu-id="1eed6-146">אחוז העלות הנצרכת = עלות בפועל שהושקעה עד היום ÷ אומדן עלות בעת השלמת המשימה</span><span class="sxs-lookup"><span data-stu-id="1eed6-146">Percentage of cost consumed = Actual cost spent to date ÷ Estimated cost at complete for the task</span></span>
 - <span data-ttu-id="1eed6-147">עלות לסיום (CTC) = אומדן עלות בזמן ההשלמה – עלות בפועל שהושקעה עד היום</span><span class="sxs-lookup"><span data-stu-id="1eed6-147">Cost to complete (CTC) = Estimated cost at complete – Actual cost spent to date</span></span>
 - <span data-ttu-id="1eed6-148">הערכה בעת סיום = CTC + עלות בפועל שהושקעה עד היום</span><span class="sxs-lookup"><span data-stu-id="1eed6-148">Estimated cost at complete = CTC + Actual cost spent to date</span></span>
 - <span data-ttu-id="1eed6-149">שונות העלות החזויה = עלות מתוכננת - עלות משוערת בהשלמה</span><span class="sxs-lookup"><span data-stu-id="1eed6-149">Projected cost variance = Planned cost – Estimated cost at complete</span></span>

<span data-ttu-id="1eed6-150">תחזית לסטיית העלות מוצגת במשימה.</span><span class="sxs-lookup"><span data-stu-id="1eed6-150">A projection of the cost variance is shown on the task.</span></span> <span data-ttu-id="1eed6-151">אם ההערכה בעת סיום היא יותר מהעלות המתוכננת, המשימה מתוכננת לעלות יותר ממה שתוכנן במקור.</span><span class="sxs-lookup"><span data-stu-id="1eed6-151">If the estimated cost at complete is more than the planned cost, the task is projected to cost more than was originally planned.</span></span> <span data-ttu-id="1eed6-152">לכן היא חורגת מהתקציב.</span><span class="sxs-lookup"><span data-stu-id="1eed6-152">Therefore, it's trending over budget.</span></span> <span data-ttu-id="1eed6-153">אם אומדן העלות קטן מהעלות המתוכננת, המשימה מתוכננת לעלות פחות ממה שתוכנן במקור והיא במסגרת התקציב.</span><span class="sxs-lookup"><span data-stu-id="1eed6-153">If the Estimated cost at complete is less than the planned cost, the task is projected to cost less than was originally planned and is trending under budget.</span></span>

## <a name="project-managers-reprojection-of-cost"></a><span data-ttu-id="1eed6-154">חיזוי עלות מחדש של מנהל הפרויקט</span><span class="sxs-lookup"><span data-stu-id="1eed6-154">Project manager’s reprojection of cost</span></span>

<span data-ttu-id="1eed6-155">כאשר מבצעים חיזוי מחדש של המאמץ, ה- CTC,‏ ההערכה בעת סיום, אחוז העלות שנצרכה וסטיית העלות החזויה מחושבים מחדש בתצוגה **מעקב עלות**.</span><span class="sxs-lookup"><span data-stu-id="1eed6-155">When effort is reprojected, the CTC, Estimated cost at complete, percentage of cost consumed, and projected cost variance are all recalculated in the **Cost tracking** view.</span></span>

## <a name="project-status-summary"></a><span data-ttu-id="1eed6-156">סיכום מצב פרויקט</span><span class="sxs-lookup"><span data-stu-id="1eed6-156">Project status summary</span></span>

<span data-ttu-id="1eed6-157">מעקב אחר נתונים בתצוגה **מעקב מאמץ** ובתצוגה **מעקב עלות** מראה את ההתקדמות ואת צריכת העלות בצומת הבסיס של הפרויקט, פעילויות ערסל ורמות של משימות צומת עלה.</span><span class="sxs-lookup"><span data-stu-id="1eed6-157">Tracking data in the **Effort tracking** and **Cost tracking** views shows the progress and cost consumption at the project root node, summary tasks, and leaf node tasks levels.</span></span> <span data-ttu-id="1eed6-158">המקטע **מצב** בדף **ישות פרויקט** מציג סיכום של מצב רמת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="1eed6-158">The **Status** section on the **Project entity** page shows a summary of project-level status.</span></span>

## <a name="status-summary-fields"></a><span data-ttu-id="1eed6-159">שדות סיכום מצב</span><span class="sxs-lookup"><span data-stu-id="1eed6-159">Status summary fields</span></span>

<span data-ttu-id="1eed6-160">השדה **מצב פרויקט כולל‬** הוא שדה שניתן לערוך אותו ושמציג את המצב הכולל של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="1eed6-160">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="1eed6-161">הוא משתמש בקידוד צבעים, כגון ירוק, צהוב ואדום, כדי לציין סיכון שמתגבר.</span><span class="sxs-lookup"><span data-stu-id="1eed6-161">It uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> <span data-ttu-id="1eed6-162">השדה **הערות** מאפשר למנהל הפרויקט להזין הערות ספציפיות לגבי המצב.</span><span class="sxs-lookup"><span data-stu-id="1eed6-162">The **Comments** field lets the project manager enter specific comments about the status.</span></span> <span data-ttu-id="1eed6-163">לא ניתן לערוך את השדה **‏‫המצב עודכן בתאריך** והערך הוא חותמת זמן שמציינת מתי המצב עודכן לאחרונה.</span><span class="sxs-lookup"><span data-stu-id="1eed6-163">The **Status updated on** field is not editable and the value is a timestamp that indicates when the status was last updated.</span></span>

<span data-ttu-id="1eed6-164">השדה **‏‫ביצועי לוח זמנים‬** והשדה **‏‫ביצועי עלות‬** נקבעים מתאריך המעקב.</span><span class="sxs-lookup"><span data-stu-id="1eed6-164">The **Schedule performance** and **Cost performance** fields are set from the tracking date.</span></span> <span data-ttu-id="1eed6-165">כאשר לוח הזמנים וסטיית העלות עבור צומת הבסיס בתצוגה **מעקב מאמץ** חיוביים, תוכל להגדיר שדות אלו בתור **הקדמה‬**.</span><span class="sxs-lookup"><span data-stu-id="1eed6-165">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, you can set these fields to **Ahead**.</span></span> <span data-ttu-id="1eed6-166">כאשר לוח הזמנים וסטיית העלות עבור צומת הבסיס שליליים, תוכל להגדיר אותם בתור **עיכוב**.</span><span class="sxs-lookup"><span data-stu-id="1eed6-166">When the schedule and cost variance for the root node are negative, you can set them to **Behind**.</span></span>
