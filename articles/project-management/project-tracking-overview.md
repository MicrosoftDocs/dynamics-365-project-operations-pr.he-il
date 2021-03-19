---
title: מבט כולל על מעקב אחר פרויקט
description: נושא זו מספק מידע כיצד ניתן לעקוב אחר התקדמות הפרויקט וצריכת העלות.
author: ruhercul
manager: AnnBe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 14094d603be2834dc66abff2ff1faf5e940b1ffa
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286609"
---
# <a name="project-tracking-overview"></a><span data-ttu-id="d96e0-103">מבט כולל על מעקב אחר פרויקט</span><span class="sxs-lookup"><span data-stu-id="d96e0-103">Project tracking overview</span></span>

<span data-ttu-id="d96e0-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="d96e0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d96e0-105">הצורך לעקוב אחר ההתקדמות מול לוח זמנים משתנה לפי ענף.</span><span class="sxs-lookup"><span data-stu-id="d96e0-105">The need to track progress against a schedule varies by industry.</span></span> <span data-ttu-id="d96e0-106">תעשיות מסוימות עוקבות ברמה מפורטת, ואילו תעשיות אחרות עוקבות ברמה גבוהה יותר.</span><span class="sxs-lookup"><span data-stu-id="d96e0-106">Some industries track at a granular level, where other industries track at a higher level.</span></span> <span data-ttu-id="d96e0-107">נושא זה מראה כיצד ליצור לוח זמנים שיעמוד בדרישות הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="d96e0-107">This topic shows how to schedule in order to meet your organization's requirements.</span></span>

## <a name="effort-tracking-view"></a><span data-ttu-id="d96e0-108">תצוגה של מעקב אחר המאמץ</span><span class="sxs-lookup"><span data-stu-id="d96e0-108">Effort tracking view</span></span>

<span data-ttu-id="d96e0-109">התצוגה **מעקב אחר מאמץ** עוקבת אחר התקדמות המשימות בלוח הזמנים על-ידי השוואת שעות המאמץ בפועל שהושקעו במשימה לשעות המאמץ המתוכננות של המשימה.</span><span class="sxs-lookup"><span data-stu-id="d96e0-109">The **Effort tracking** view tracks the progress of tasks in the schedule by comparing the actual effort hours spent on a task to the task's planned effort hours.</span></span> <span data-ttu-id="d96e0-110">Dynamics 365 Project Operations משתמש בנוסחאות הבאות כדי לחשב את מדדי המעקב:</span><span class="sxs-lookup"><span data-stu-id="d96e0-110">Dynamics 365 Project Operations uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="d96e0-111">**אחוזי התקדמות**: מאמץ בפועל שנעשה עד היום ÷ הערכה בעת סיום (EAC)</span><span class="sxs-lookup"><span data-stu-id="d96e0-111">**Progress percentage**: Actual effort spent to date ÷ Estimate at complete (EAC)</span></span> 
- <span data-ttu-id="d96e0-112">**הערכה לסיום (ETC)**: מאמץ מתוכנן – מאמץ בפועל שהושקע עד היום</span><span class="sxs-lookup"><span data-stu-id="d96e0-112">**Estimate to complete (ETC)**: Planned effort – Actual effort spent to date</span></span> 
- <span data-ttu-id="d96e0-113">**EAC**: מאמץ שנותר + מאמץ בפועל שהושקע עד היום</span><span class="sxs-lookup"><span data-stu-id="d96e0-113">**EAC**: Remaining effort + Actual effort spent to date</span></span> 
- <span data-ttu-id="d96e0-114">**סטיית מאמץ חזוי**: מאמץ מתוכנן – EAC</span><span class="sxs-lookup"><span data-stu-id="d96e0-114">**Projected effort variance**: Planned effort – EAC</span></span>

<span data-ttu-id="d96e0-115">Project Operations מציג תחזית לסטיית המאמץ במשימה.</span><span class="sxs-lookup"><span data-stu-id="d96e0-115">Project Operations shows a projection of the effort variance on the task.</span></span> <span data-ttu-id="d96e0-116">אם ה- EAC הוא יותר מהמאמץ המתוכנן, המשימה מתוכננת להימשך זמן רב יותר ממה שתוכנן במקור והיא בפיגור אל מול לוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="d96e0-116">If the EAC is more than the planned effort, the task is projected to take more time than was originally planned and is behind schedule.</span></span> <span data-ttu-id="d96e0-117">אם ה- EAC הוא פחות מהמאמץ המתוכנן, המשימה מתוכננת להימשך זמן קצר יותר ממה שתוכנן במקור והיא מקדימה את לוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="d96e0-117">If the EAC is less than the planned effort, the task is projected to take less time than was originally planned and is ahead schedule.</span></span>

## <a name="reprojecting-effort"></a><span data-ttu-id="d96e0-118">חיזוי מחדש למאמץ</span><span class="sxs-lookup"><span data-stu-id="d96e0-118">Reprojecting effort</span></span>

<span data-ttu-id="d96e0-119">מנהלי פרויקטים משנים לעיתים קרובות את ההערכות המקוריות במשימה.</span><span class="sxs-lookup"><span data-stu-id="d96e0-119">Project managers often revise the original estimates on a task.</span></span> <span data-ttu-id="d96e0-120">חיזויים מחדש של פרויקט הם תפיסות של מנהל הפרויקט להערכות, בהינתן המצב הנוכחי של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="d96e0-120">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="d96e0-121">עם זאת, איננו ממליצים למנהלי פרויקטים לשנות את המספרים הבסיסיים.</span><span class="sxs-lookup"><span data-stu-id="d96e0-121">However, we don't recommend that project managers change the baseline numbers.</span></span> <span data-ttu-id="d96e0-122">זאת מכיוון שבסיס הפרויקט מייצג את מקור האמת המבוסס של הערכת העלות ולוח הזמנים של הפרויקט, וכל בעלי העניין של הפרויקט הסכימו עליו.</span><span class="sxs-lookup"><span data-stu-id="d96e0-122">This is because the project baseline represents the established source of truth for the project schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="d96e0-123">קיימות שתי דרכים שבהן מנהל פרויקט יכול לבצע חיזוי מחדש של מאמץ במשימות:</span><span class="sxs-lookup"><span data-stu-id="d96e0-123">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="d96e0-124">עקוף את ה- ETC שבברירת מחדל בעזרת הערכה חדשה של המאמץ בפועל שנותר במשימה.</span><span class="sxs-lookup"><span data-stu-id="d96e0-124">Override the default ETC with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="d96e0-125">עקוף את אחוז ההתקדמות שבברירת מחדל בעזרת הערכה חדשה של ההתקדמות האמיתית במשימה.</span><span class="sxs-lookup"><span data-stu-id="d96e0-125">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="d96e0-126">כל גישה גורמת לחישוב מחדש של ה- ETC, ה- ‏EAC, אחוז ההתקדמות במשימה ושל סטיית המאמץ החזוי במשימה.</span><span class="sxs-lookup"><span data-stu-id="d96e0-126">Each approach causes a recalculation of the task's ETC, EAC, progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="d96e0-127">ה- EAC, ה- ‏ETC ואחוז ההתקדמות בפעילויות הערסל מחושבים גם כן, ומפיקים חיזוי חדש לסטיית המאמץ.</span><span class="sxs-lookup"><span data-stu-id="d96e0-127">The EAC, ETC, and progress percentage on the summary tasks are also recalculated and produce a new projection of effort variance.</span></span>

## <a name="reprojection-of-effort-on-summary-tasks"></a><span data-ttu-id="d96e0-128">חיזוי מחדש של מאמץ בפעילויות ערסל</span><span class="sxs-lookup"><span data-stu-id="d96e0-128">Reprojection of effort on summary tasks</span></span>

<span data-ttu-id="d96e0-129">ניתן ליצור חיזוי מחדש למאמץ בפעילויות ערבול או במשימות של גורמים מכילים.</span><span class="sxs-lookup"><span data-stu-id="d96e0-129">Effort on summary tasks or container tasks can be reprojected.</span></span> <span data-ttu-id="d96e0-130">בין אם המשתמש מבצע חיזוי מחדש באמצעות המאמץ שנותר או אחוז ההתקדמות בפעילויות ערסל, קבוצת החישובים הבאה מתחילה:</span><span class="sxs-lookup"><span data-stu-id="d96e0-130">Regardless of whether the user reprojects by using the remaining effort or the progress percentage on the summary tasks, the following set of calculations begins:</span></span>

- <span data-ttu-id="d96e0-131">מתבצע חישוב ל- EAC,‏‏ ל- ETC ולאחוז ההתקדמות במשימה.</span><span class="sxs-lookup"><span data-stu-id="d96e0-131">The EAC, ETC, and progress percentage on the task are calculated.</span></span>
- <span data-ttu-id="d96e0-132">ה- EAC החדש מופץ לפעילויות הצאצא ביחס זהה לזה שהיה ב- EAC המקורי בפעילות.</span><span class="sxs-lookup"><span data-stu-id="d96e0-132">The new EAC is distributed down to the child tasks in the same proportion as the original EAC was on the task.</span></span>
- <span data-ttu-id="d96e0-133">ה- EAC החדש מחושב בכל אחת מהפעילויות הבודדות עד לפעילויות של צומת העלה.</span><span class="sxs-lookup"><span data-stu-id="d96e0-133">The new EAC on each of the individual tasks down to the leaf node tasks is calculated.</span></span> 
- <span data-ttu-id="d96e0-134">החישוב מחדש של ETC ואחוז התקדמות בפעילויות הצאצא המושפעות עד לצמתי העלה מתבסס על ערך ה- EAC.</span><span class="sxs-lookup"><span data-stu-id="d96e0-134">The affected child tasks down to the leaf nodes have their ETC and progress percentage recalculated based on the EAC value.</span></span> <span data-ttu-id="d96e0-135">התוצאה היא חיזוי חדש עבור סטיית המאמץ של הפעילות.</span><span class="sxs-lookup"><span data-stu-id="d96e0-135">This results in a new projection for the effort variance of the task.</span></span> 
- <span data-ttu-id="d96e0-136">מתבצע חישוב מחדש להערכות ה- EAC של פעילויות הערסל ועד לצומת הבסיס.</span><span class="sxs-lookup"><span data-stu-id="d96e0-136">The EACs of the summary tasks all the way to the root node are recalculated.</span></span>

### <a name="cost-tracking-view"></a><span data-ttu-id="d96e0-137">תצוגת מעקב עלות</span><span class="sxs-lookup"><span data-stu-id="d96e0-137">Cost tracking view</span></span> 

<span data-ttu-id="d96e0-138">התצוגה **מעקב עלות** משווה בין העלות בפועל שהושקעה לעלות המתוכננת במשימה.</span><span class="sxs-lookup"><span data-stu-id="d96e0-138">The **Cost tracking** view compares the actual cost that was spent on a task to the planned cost on a task.</span></span> 

> [!NOTE]
> <span data-ttu-id="d96e0-139">תצוגה זו מציגה רק עלויות עבודה ואינה כוללת עלויות מהערכת ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="d96e0-139">This view shows only labor costs and doesn’t include costs from the expense estimates.</span></span> <span data-ttu-id="d96e0-140">Project Operations משתמש בנוסחאות הבאות כדי לחשב את מדדי המעקב:</span><span class="sxs-lookup"><span data-stu-id="d96e0-140">Project Operations uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="d96e0-141">**אחוז העלות הנצרכת**: עלות בפועל שהושקעה עד היום ÷ אומדן עלות בעת השלמת המשימה</span><span class="sxs-lookup"><span data-stu-id="d96e0-141">**Percentage of cost consumed**: Actual cost spent to date ÷ Estimated cost at completion</span></span>
- <span data-ttu-id="d96e0-142">**עלות לסיום (CTC)**: עלות מתוכננת – עלות בפועל שהושקעה עד היום</span><span class="sxs-lookup"><span data-stu-id="d96e0-142">**Cost to complete (CTC)**: Planned cost – Actual cost spent to date</span></span>
- <span data-ttu-id="d96e0-143">**EAC**: עלות נותרת + סכום עלות בפועל עד היום</span><span class="sxs-lookup"><span data-stu-id="d96e0-143">**EAC**: Remaining cost + Actual cost spent to date</span></span>
- <span data-ttu-id="d96e0-144">**סטיית עלות חזויה**: עלות מתוכננת – EAC</span><span class="sxs-lookup"><span data-stu-id="d96e0-144">**Projected cost variance**: Planned cost – EAC</span></span>

<span data-ttu-id="d96e0-145">תחזית לסטיית העלות מוצגת במשימה.</span><span class="sxs-lookup"><span data-stu-id="d96e0-145">A projection of the cost variance is shown on the task.</span></span> <span data-ttu-id="d96e0-146">אם ה- EAC הוא יותר מהעלות המתוכננת, המשימה מתוכננת לעלות יותר ממה שתוכנן במקור.</span><span class="sxs-lookup"><span data-stu-id="d96e0-146">If the EAC is more than the planned cost, the task is projected to cost more than was originally planned.</span></span> <span data-ttu-id="d96e0-147">לכן היא חורגת מהתקציב.</span><span class="sxs-lookup"><span data-stu-id="d96e0-147">Therefore, it's trending over budget.</span></span> <span data-ttu-id="d96e0-148">אם ה- EAC הוא פחות מהעלות המתוכננת, המשימה מתוכננת לעלות פחות ממה שתוכנן במקור.</span><span class="sxs-lookup"><span data-stu-id="d96e0-148">If the EAC is less than the planned cost, the task is projected to cost less than was originally planned.</span></span> <span data-ttu-id="d96e0-149">לכן היא מתחת לתקציב.</span><span class="sxs-lookup"><span data-stu-id="d96e0-149">Therefore, it's trending under budget.</span></span>

## <a name="project-managers-reprojection-of-cost"></a><span data-ttu-id="d96e0-150">חיזוי עלות מחדש של מנהל הפרויקט</span><span class="sxs-lookup"><span data-stu-id="d96e0-150">Project manager’s reprojection of cost</span></span>

<span data-ttu-id="d96e0-151">כאשר מבצעים חיזוי מחדש למאמץ, ה- CTC,‏ EAC, אחוז העלות שנצרכה וסטיית העלות החזויה מחושבים מחדש בתצוגה **מעקב עלות**.</span><span class="sxs-lookup"><span data-stu-id="d96e0-151">When effort is reprojected, the CTC, EAC, percentage of cost consumed, and projected cost variance are all recalculated in the **Cost tracking** view.</span></span>

## <a name="project-status-summary"></a><span data-ttu-id="d96e0-152">סיכום מצב פרויקט</span><span class="sxs-lookup"><span data-stu-id="d96e0-152">Project status summary</span></span>

<span data-ttu-id="d96e0-153">מעקב אחר נתונים בתצוגה **מעקב מאמץ** ובתצוגה **מעקב עלות** מראה את ההתקדמות ואת צריכת העלות בצומת הבסיס של הפרויקט, פעילויות ערסל ורמות של משימות צומת עלה.</span><span class="sxs-lookup"><span data-stu-id="d96e0-153">Tracking data in the **Effort tracking** and **Cost tracking** views shows the progress and cost consumption at the project root node, summary tasks, and leaf node tasks levels.</span></span> <span data-ttu-id="d96e0-154">המקטע **מצב** בדף **ישות פרויקט** מציג סיכום של מצב רמת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="d96e0-154">The **Status** section on the **Project entity** page shows a summary of project-level status.</span></span>

## <a name="status-summary-fields"></a><span data-ttu-id="d96e0-155">שדות סיכום מצב</span><span class="sxs-lookup"><span data-stu-id="d96e0-155">Status summary fields</span></span>

<span data-ttu-id="d96e0-156">השדה **מצב פרויקט כולל‬** הוא שדה שניתן לערוך אותו ושמציג את המצב הכולל של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="d96e0-156">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="d96e0-157">הוא משתמש בקידוד צבעים, כגון ירוק, צהוב ואדום, כדי לציין סיכון שמתגבר.</span><span class="sxs-lookup"><span data-stu-id="d96e0-157">It uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> <span data-ttu-id="d96e0-158">השדה **הערות** מאפשר למנהל הפרויקט להזין הערות ספציפיות לגבי המצב.</span><span class="sxs-lookup"><span data-stu-id="d96e0-158">The **Comments** field lets the project manager enter specific comments about the status.</span></span> <span data-ttu-id="d96e0-159">לא ניתן לערוך את השדה **‏‫המצב עודכן בתאריך** והערך הוא חותמת זמן שמציינת מתי המצב עודכן לאחרונה.</span><span class="sxs-lookup"><span data-stu-id="d96e0-159">The **Status updated on** field is not editable and the value is a timestamp that indicates when the status was last updated.</span></span>

<span data-ttu-id="d96e0-160">השדה **‏‫ביצועי לוח זמנים‬** והשדה **‏‫ביצועי עלות‬** נקבעים מתאריך המעקב.</span><span class="sxs-lookup"><span data-stu-id="d96e0-160">The **Schedule performance** and **Cost performance** fields are set from the tracking date.</span></span> <span data-ttu-id="d96e0-161">כאשר לוח הזמנים וסטיית העלות עבור צומת הבסיס בתצוגה **מעקב מאמץ** חיוביים, תוכל להגדיר שדות אלו בתור **הקדמה‬**.</span><span class="sxs-lookup"><span data-stu-id="d96e0-161">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, you can set these fields to **Ahead**.</span></span> <span data-ttu-id="d96e0-162">כאשר לוח הזמנים וסטיית העלות עבור צומת הבסיס שליליים, תוכל להגדיר אותם בתור **עיכוב**.</span><span class="sxs-lookup"><span data-stu-id="d96e0-162">When the schedule and cost variance for the root node are negative, you can set them to **Behind**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]