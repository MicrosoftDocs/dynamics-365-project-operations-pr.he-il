---
title: התקדמות הפרוייקט וצריכת העלות
description: נושא זו מספק מידע כיצד ניתן לעקוב אחר התקדמות הפרוייקט וצריכת העלות.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 0d742164-5469-421d-8917-63160a81f651
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8aa5814938129f30885d8161a7c86197ab013364
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751864"
---
# <a name="project-progress-and-cost-consumption"></a><span data-ttu-id="776a9-103">התקדמות הפרוייקט וצריכת העלות</span><span class="sxs-lookup"><span data-stu-id="776a9-103">Project progress and cost consumption</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="776a9-104">הצורך לעקוב אחר ההתקדמות מול לוח זמנים משתנה לפי ענף.</span><span class="sxs-lookup"><span data-stu-id="776a9-104">The need to track progress against a schedule varies by industry.</span></span> <span data-ttu-id="776a9-105">תעשיות מסוימות עוקבות ברמה מפורטת, ואילו תעשיות אחרות עוקבות ברמה גבוהה יותר.</span><span class="sxs-lookup"><span data-stu-id="776a9-105">Some industries track at a granular level, whereas other industries track at a higher level.</span></span> <span data-ttu-id="776a9-106">נושא זה מראה כיצד ליצור לוח זמנים שיעמוד בדרישות הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="776a9-106">This topic shows how to schedule in order to meet your organization's requirements.</span></span>

## <a name="effort-tracking-view"></a><span data-ttu-id="776a9-107">תצוגה של מעקב אחר המאמץ</span><span class="sxs-lookup"><span data-stu-id="776a9-107">Effort tracking view</span></span>

<span data-ttu-id="776a9-108">התצוגה **מעקב אחר מאמץ** עוקבת אחר ההתקדמות של משימות בלוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="776a9-108">The **Effort tracking** view tracks the progress of tasks in the schedule.</span></span> <span data-ttu-id="776a9-109">היא משווה בין שעות המאמץ בפועל שהושקעו במשימה לבין מספר שעות המאמץ המתוכננות במשימה.</span><span class="sxs-lookup"><span data-stu-id="776a9-109">It compares the actual effort hours that have been spent on a task to the planned effort hours for that task.</span></span> <span data-ttu-id="776a9-110">PSA משתמש בנוסחאות הבאות כדי לחשב את מדדי המעקב:</span><span class="sxs-lookup"><span data-stu-id="776a9-110">PSA uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="776a9-111">אחוז התקדמות = מאמץ בפועל שהושקע עד היום ÷ מאמץ מתוכנן עבור המשימה</span><span class="sxs-lookup"><span data-stu-id="776a9-111">Progress percentage = Actual effort spent to date ÷ Planned effort for the task</span></span> 
- <span data-ttu-id="776a9-112">הערכה לסיום (ETC) = מאמץ מתוכנן – מאמץ בפועל שהושקע עד היום</span><span class="sxs-lookup"><span data-stu-id="776a9-112">Estimate to complete (ETC) = Planned effort – Actual effort spent to date</span></span> 
- <span data-ttu-id="776a9-113">הערכה בעת סיום (EAC) = מאמץ שנותר + מאמץ בפועל שהושקע עד היום</span><span class="sxs-lookup"><span data-stu-id="776a9-113">Estimate at complete (EAC) = Remaining effort + Actual effort spent to date</span></span> 
- <span data-ttu-id="776a9-114">סטיית מאמץ חזוי = מאמץ מתוכנן – EAC</span><span class="sxs-lookup"><span data-stu-id="776a9-114">Projected effort variance = Planned effort – EAC</span></span>

<span data-ttu-id="776a9-115">PSA מציג תחזית לסטיית המאמץ במשימה.</span><span class="sxs-lookup"><span data-stu-id="776a9-115">PSA shows a projection of the effort variance on the task.</span></span> <span data-ttu-id="776a9-116">אם ה- EAC הוא יותר מהמאמץ המתוכנן, המשימה מתוכננת להימשך זמן רב יותר ממה שתוכנן במקור.</span><span class="sxs-lookup"><span data-stu-id="776a9-116">If the EAC is more than the planned effort, the task is projected to take more time than was originally planned.</span></span> <span data-ttu-id="776a9-117">לכן היא תפגר בלוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="776a9-117">Therefore, it's behind schedule.</span></span> <span data-ttu-id="776a9-118">אם ה- EAC הוא פחות מהמאמץ המתוכנן, המשימה מתוכננת להימשך פחות זמן ממה שתוכנן במקור.</span><span class="sxs-lookup"><span data-stu-id="776a9-118">If the EAC is less than the planned effort, the task is projected to take less time than was originally planned.</span></span> <span data-ttu-id="776a9-119">לכן היא מקדימה את לוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="776a9-119">Therefore, it's ahead of schedule.</span></span>

## <a name="re-projecting-effort"></a><span data-ttu-id="776a9-120">חיזוי מחדש למאמץ</span><span class="sxs-lookup"><span data-stu-id="776a9-120">Re-projecting effort</span></span>

<span data-ttu-id="776a9-121">מקובל שמנהל פרוייקט ישנה את ההערכות המקוריות במשימה.</span><span class="sxs-lookup"><span data-stu-id="776a9-121">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="776a9-122">חיזויים מחדש לפרוייקט הם תפיסות של מנהל הפרוייקט להערכות, בהינתן המצב הנוכחי של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="776a9-122">Project re-projections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="776a9-123">אולם, אנחנו לא ממליצים למנהל הפרוייקט לשנות את המספרים הבסיסיים, מכיוון שבסיס הפרוייקט מייצג את מקור האמת המבוסס של הערכת העלות ולוח הזמנים של הפרוייקט, וכל בעלי העניין של הפרוייקט הסכימו עליו.</span><span class="sxs-lookup"><span data-stu-id="776a9-123">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="776a9-124">קיימות שתי דרכים שבהן מנהל פרוייקט יכול לבצע חיזוי מחדש של מאמץ במשימות:</span><span class="sxs-lookup"><span data-stu-id="776a9-124">There are two ways that a project manager can re-project effort on tasks:</span></span>

- <span data-ttu-id="776a9-125">עקוף את ה- ETC שבברירת מחדל בעזרת הערכה חדשה של המאמץ בפועל שנותר במשימה.</span><span class="sxs-lookup"><span data-stu-id="776a9-125">Override the default ETC with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="776a9-126">עקוף את אחוז ההתקדמות שבברירת מחדל בעזרת הערכה חדשה של ההתקדמות האמיתית במשימה.</span><span class="sxs-lookup"><span data-stu-id="776a9-126">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="776a9-127">כל אחת מהגישות האלו גורמת לחישוב מחדש של ה- ETC, ‏EAC ואחוז ההתקדמות במשימה ושל סטיית המאמץ החזוי במשימה.</span><span class="sxs-lookup"><span data-stu-id="776a9-127">Each of these approaches cause a recalculation of the task's ETC, EAC, and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="776a9-128">ה- EAC, ‏ETC ואחוז ההתקדמות בפעילויות הערסל מחושבים גם כן, ומפיקים חיזוי חדש לסטיית המאמץ.</span><span class="sxs-lookup"><span data-stu-id="776a9-128">The EAC, ETC, and progress percentage on the summary tasks are also recalculated, and produce a new projection of effort variance.</span></span>

## <a name="re-projection-of-effort-on-summary-tasks"></a><span data-ttu-id="776a9-129">חיזוי מחדש של מאמץ בפעילויות ערסל</span><span class="sxs-lookup"><span data-stu-id="776a9-129">Re-projection of effort on summary tasks</span></span>

<span data-ttu-id="776a9-130">ניתן ליצור חיזוי מחדש למאמץ בפעילויות ערבול או במשימות של גורמים מכילים.</span><span class="sxs-lookup"><span data-stu-id="776a9-130">Effort on summary tasks or container tasks can be re-projected.</span></span> <span data-ttu-id="776a9-131">בין אם המשתמש מבצע חיזוי מחדש באמצעות המאמץ שנותר או אחוז ההתקדמות בפעילויות ערסל, קבוצת החישובים הבאה מתחילה:</span><span class="sxs-lookup"><span data-stu-id="776a9-131">Regardless of whether the user re-projects by using the remaining effort or the progress percentage on the summary tasks, the following set of calculations begins:</span></span>

- <span data-ttu-id="776a9-132">מתבצע חישוב ל- EAC,‏‏ ל- ETC ולאחוז ההתקדמות במשימה.</span><span class="sxs-lookup"><span data-stu-id="776a9-132">The EAC, ETC, and progress percentage on the task are calculated.</span></span>
- <span data-ttu-id="776a9-133">ה- EAC החדש מופץ לפעילויות הצאצא ביחס זהה לזה שהיה ב- EAC המקורי בפעילות.</span><span class="sxs-lookup"><span data-stu-id="776a9-133">The new EAC is distributed down to the child tasks in the same proportion as the original EAC was on the task.</span></span>
- <span data-ttu-id="776a9-134">ה- EAC החדש מחושב בכל אחת מהפעילויות הבודדות עד לפעילויות של צומת העלה.</span><span class="sxs-lookup"><span data-stu-id="776a9-134">The new EAC on each of the individualt tasks down to the leaf node tasks is calculated.</span></span> 
- <span data-ttu-id="776a9-135">החישוב מחדש של ETC ואחוז התקדמות בפעילויות הצאצא המושפעות עד לצמתי העלה מתבסס על ערך ה- EAC.</span><span class="sxs-lookup"><span data-stu-id="776a9-135">The affected child tasks down to the leaf nodes have their ETC and progress percentage recalculated based on the EAC value.</span></span> <span data-ttu-id="776a9-136">התוצאה היא חיזוי חדש עבור סטיית המאמץ של הפעילות.</span><span class="sxs-lookup"><span data-stu-id="776a9-136">This results in a new projection for the effort variance of the task.</span></span> 
- <span data-ttu-id="776a9-137">מתבצע חישוב מחדש להערכות ה- EAC של פעילויות הערסל ועד לצומת הבסיס.</span><span class="sxs-lookup"><span data-stu-id="776a9-137">The EACs of the summary tasks all the way to the root node are recalculated.</span></span>

### <a name="cost-tracking-view"></a><span data-ttu-id="776a9-138">תצוגת מעקב עלות</span><span class="sxs-lookup"><span data-stu-id="776a9-138">Cost tracking view</span></span> 

<span data-ttu-id="776a9-139">התצוגה **מעקב עלות** משווה בין העלות בפועל שהושקעה לעלות המתוכננת במשימה.</span><span class="sxs-lookup"><span data-stu-id="776a9-139">The **Cost tracking** view compares the actual cost that was spent on a task to the planned cost on a task.</span></span> 

> [!NOTE]
> <span data-ttu-id="776a9-140">תצוגה זו מציגה רק עלויות עבודה ואינה כוללת עלויות מהערכת ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="776a9-140">This view shows only labor costs and doesn’t include costs from the expense estimates.</span></span> 

<span data-ttu-id="776a9-141">PSA משתמש בנוסחאות הבאות כדי לחשב את מדדי המעקב:</span><span class="sxs-lookup"><span data-stu-id="776a9-141">PSA uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="776a9-142">אחוז העלות הנצרכת = עלות בפועל שהושקעה עד היום ÷ עלות מתוכננת עבור המשימה</span><span class="sxs-lookup"><span data-stu-id="776a9-142">Percentage of cost consumed = Actual cost spent to date ÷ Planned cost for the task</span></span>
- <span data-ttu-id="776a9-143">עלות לסיום (CTC) = עלות מתוכננת – עלות בפועל שהושקעה עד היום</span><span class="sxs-lookup"><span data-stu-id="776a9-143">Cost to complete (CTC) = Planned cost – Actual cost spent to date</span></span>
- <span data-ttu-id="776a9-144">EAC‏ = CTC + עלות בפועל שהושקעה עד היום</span><span class="sxs-lookup"><span data-stu-id="776a9-144">EAC = CTC + Actual cost spent to date</span></span>
- <span data-ttu-id="776a9-145">סטיית עלות חזויה = עלות מתוכננת – EAC</span><span class="sxs-lookup"><span data-stu-id="776a9-145">Projected cost variance = Planned cost – EAC</span></span>

<span data-ttu-id="776a9-146">תחזית לסטיית העלות מוצגת במשימה.</span><span class="sxs-lookup"><span data-stu-id="776a9-146">A projection of the cost variance is shown on the task.</span></span> <span data-ttu-id="776a9-147">אם ה- EAC הוא יותר מהעלות המתוכננת, המשימה מתוכננת לעלות יותר ממה שתוכנן במקור.</span><span class="sxs-lookup"><span data-stu-id="776a9-147">If the EAC is more than the planned cost, the task is projected to cost more than was originally planned.</span></span> <span data-ttu-id="776a9-148">לכן היא חורגת מהתקציב.</span><span class="sxs-lookup"><span data-stu-id="776a9-148">Therefore, it's trending over budget.</span></span> <span data-ttu-id="776a9-149">אם ה- EAC הוא פחות מהעלות המתוכננת, המשימה מתוכננת לעלות פחות ממה שתוכנן במקור.</span><span class="sxs-lookup"><span data-stu-id="776a9-149">If the EAC is less than the planned cost, the task is projected to cost less than was originally planned.</span></span> <span data-ttu-id="776a9-150">לכן היא מתחת לתקציב.</span><span class="sxs-lookup"><span data-stu-id="776a9-150">Therefore, it's trending under budget.</span></span>

## <a name="project-managers-re-projection-of-cost"></a><span data-ttu-id="776a9-151">חיזוי עלות מחדש של מנהל הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="776a9-151">Project manager’s re-projection of cost</span></span>

<span data-ttu-id="776a9-152">כאשר מבצעים חיזוי מחדש למאמץ, ה- CTC,‏ EAC, אחוז העלות שנצרכה וסטיית העלות החזויה מחושבים מחדש בתצוגה **מעקב עלות**.</span><span class="sxs-lookup"><span data-stu-id="776a9-152">When effort is re-projected, the CTC, EAC, percentage of cost consumed, and projected cost variance are all recalculated in the **Cost tracking** view.</span></span>

## <a name="project-status-summary"></a><span data-ttu-id="776a9-153">סיכום מצב פרוייקט</span><span class="sxs-lookup"><span data-stu-id="776a9-153">Project status summary</span></span>

<span data-ttu-id="776a9-154">מעקב אחר נתונים בתצוגה **מעקב מאמץ** ובתצוגה **מעקב עלות** מראה את ההתקדמות ואת צריכת העלות בצומת הבסיס של הפרוייקט, פעילויות ערסל ורמות של משימות צומת עלה.</span><span class="sxs-lookup"><span data-stu-id="776a9-154">Tracking data in the **Effort tracking** and **Cost tracking** views shows the progress and cost consumption at the project root node, summary tasks, and leaf node tasks levels.</span></span> <span data-ttu-id="776a9-155">המקטע **מצב** בדף **ישות פרוייקט** מציג סיכום של מצב רמת הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="776a9-155">The **Status** section on the **Project entity** page shows a summary of project-level status.</span></span>

## <a name="status-summary-fields"></a><span data-ttu-id="776a9-156">שדות סיכום מצב</span><span class="sxs-lookup"><span data-stu-id="776a9-156">Status summary fields</span></span>

<span data-ttu-id="776a9-157">השדה **מצב פרוייקט כולל‬** הוא שדה שניתן לערוך אותו ושמציג את המצב הכולל של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="776a9-157">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="776a9-158">הוא משתמש בקידוד צבעים, כגון ירוק, צהוב ואדום, כדי לציין סיכון שמתגבר.</span><span class="sxs-lookup"><span data-stu-id="776a9-158">It uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> <span data-ttu-id="776a9-159">השדה **הערות** מאפשר למנהל הפרוייקט להזין הערות ספציפיות לגבי המצב.</span><span class="sxs-lookup"><span data-stu-id="776a9-159">The **Comments** field lets the project manager enter specific comments about the status.</span></span> <span data-ttu-id="776a9-160">לא ניתן לערוך את השדה **‏‫המצב עודכן בתאריך** והערך הוא חותמת זמן שמציינת מתי המצב עודכן לאחרונה.</span><span class="sxs-lookup"><span data-stu-id="776a9-160">The **Status updated on** field is not editable and the value is a timestamp that indicates when the status was last updated.</span></span>

<span data-ttu-id="776a9-161">השדה **‏‫ביצועי לוח זמנים‬** והשדה **‏‫ביצועי עלות‬** נקבעים מתאריך המעקב.</span><span class="sxs-lookup"><span data-stu-id="776a9-161">The **Schedule performance** and **Cost performance** fields are set from the tracking date.</span></span> <span data-ttu-id="776a9-162">כאשר לוח הזמנים וסטיית העלות עבור צומת הבסיס בתצוגה **מעקב מאמץ** חיוביים, תוכל להגדיר שדות אלו בתור **הקדמה‬**.</span><span class="sxs-lookup"><span data-stu-id="776a9-162">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, you can set these fields to **Ahead**.</span></span> <span data-ttu-id="776a9-163">כאשר לוח הזמנים וסטיית העלות עבור צומת הבסיס שליליים, תוכל להגדיר אותם בתור **עיכוב**.</span><span class="sxs-lookup"><span data-stu-id="776a9-163">When the schedule and cost variance for the root node are negative, you can set them to **Behind**.</span></span>
