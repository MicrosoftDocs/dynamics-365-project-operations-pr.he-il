---
title: מצבי תזמון
description: נושא זה מספק מידע על מצבי תזמון.
author: ruhercul
ms.date: 05/28/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 508ff1df8f7e31066712fab6f8871dfdb107a43b
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116708"
---
# <a name="scheduling-modes"></a><span data-ttu-id="91e22-103">מצבי תזמון</span><span class="sxs-lookup"><span data-stu-id="91e22-103">Scheduling modes</span></span>

<span data-ttu-id="91e22-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="91e22-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="91e22-105">Dynamics 365 Project Operations מספק לארגונים יכולת להגדיר כיצד הם מנהלים שינויים במשתני מפתח במשימות שבמבנה התפלגות העבודה.</span><span class="sxs-lookup"><span data-stu-id="91e22-105">Dynamics 365 Project Operations provides the ability for organizations to define how they manage changes to key variables in tasks within the work breakdown structure.</span></span> <span data-ttu-id="91e22-106">בהתבסס על הצרכים הספציפיים של הארגון, מנהלי פרויקטים יכולים לבצע שינויים במצב התזמון בעת יצירת פרויקט.</span><span class="sxs-lookup"><span data-stu-id="91e22-106">Based on the specific needs of the organization, Project Managers can make changes to the scheduling mode when a project is created.</span></span>

<span data-ttu-id="91e22-107">ישנם שלושה מצבי תזמון זמינים ב- Project Operations:</span><span class="sxs-lookup"><span data-stu-id="91e22-107">There are three scheduling modes available in Project Operations:</span></span>

  - <span data-ttu-id="91e22-108">משך קבוע (זהו מצב ברירת המחדל)</span><span class="sxs-lookup"><span data-stu-id="91e22-108">Fixed duration (this is the default mode)</span></span>
  - <span data-ttu-id="91e22-109">מאמץ קבוע (*עבודה*)</span><span class="sxs-lookup"><span data-stu-id="91e22-109">Fixed effort (*Work*)</span></span>
  - <span data-ttu-id="91e22-110">יחידות קבועות</span><span class="sxs-lookup"><span data-stu-id="91e22-110">Fixed units</span></span>

<span data-ttu-id="91e22-111">הערכים המושפעים מהגדרת מצב תזמון ספציפי נקבעים על ידי הנוסחה הבאה:</span><span class="sxs-lookup"><span data-stu-id="91e22-111">The values impacted by the definition of a specific scheduling mode are determined by the following formula:</span></span>

  <span data-ttu-id="91e22-112">מאמץ = משך x יחידות</span><span class="sxs-lookup"><span data-stu-id="91e22-112">Effort  = Duration x Units</span></span>

<span data-ttu-id="91e22-113">כשמגדירים את מצב התזמון של הפרויקט, מגדירים אחד מהערכים האלה, שלא ניתן לשנותם.</span><span class="sxs-lookup"><span data-stu-id="91e22-113">When you define a project’s scheduling mode, you are setting one of these values, which then can't be changed.</span></span> <span data-ttu-id="91e22-114">החזקת ערך זה כקבוע מציבה את ערך זה בעדיפות. פעולה זו מעדכנת את המערכת שלא לשנות אותו כאשר שני הערכים האחרים משתנים.</span><span class="sxs-lookup"><span data-stu-id="91e22-114">Holding this value as a constant places a priority on that value, which notifies the system not to change it when the other two values change.</span></span> <span data-ttu-id="91e22-115">הטבלה הבאה מספקת מידע על ההשפעות של בחירת מצב ספציפי.</span><span class="sxs-lookup"><span data-stu-id="91e22-115">The following table provides information about the impacts of selecting a specific mode.</span></span>

| <span data-ttu-id="91e22-116">**במשימה זו**</span><span class="sxs-lookup"><span data-stu-id="91e22-116">**In this task**</span></span>             | <span data-ttu-id="91e22-117">**אם משנים את היחידות**</span><span class="sxs-lookup"><span data-stu-id="91e22-117">**If you revise units**</span></span>   | <span data-ttu-id="91e22-118">**אם משנים את המשך**</span><span class="sxs-lookup"><span data-stu-id="91e22-118">**If you revise duration**</span></span> | <span data-ttu-id="91e22-119">**אם משנים את המאמץ**</span><span class="sxs-lookup"><span data-stu-id="91e22-119">**If you revise effort**</span></span>  |
|----------------------|---------------------------|----------------------------|---------------------------|
| <span data-ttu-id="91e22-120">משימת יחידות קבועות</span><span class="sxs-lookup"><span data-stu-id="91e22-120">Fixed units task</span></span>     | <span data-ttu-id="91e22-121">משך הזמן מחושב מחדש.</span><span class="sxs-lookup"><span data-stu-id="91e22-121">Duration is recalculated.</span></span> | <span data-ttu-id="91e22-122">המאמץ מחושב מחדש.</span><span class="sxs-lookup"><span data-stu-id="91e22-122">Effort is recalculated.</span></span>    | <span data-ttu-id="91e22-123">משך הזמן מחושב מחדש.</span><span class="sxs-lookup"><span data-stu-id="91e22-123">Duration is recalculated.</span></span> |
| <span data-ttu-id="91e22-124">משימה במאמץ קבוע</span><span class="sxs-lookup"><span data-stu-id="91e22-124">Fixed effort task</span></span>    | <span data-ttu-id="91e22-125">משך הזמן מחושב מחדש.</span><span class="sxs-lookup"><span data-stu-id="91e22-125">Duration is recalculated.</span></span> | <span data-ttu-id="91e22-126">יחידות מחושבות מחדש.</span><span class="sxs-lookup"><span data-stu-id="91e22-126">Units are recalculated.</span></span>    | <span data-ttu-id="91e22-127">משך הזמן מחושב מחדש.</span><span class="sxs-lookup"><span data-stu-id="91e22-127">Duration is recalculated.</span></span> |
| <span data-ttu-id="91e22-128">משימה במשך זמן קבוע</span><span class="sxs-lookup"><span data-stu-id="91e22-128">Fixed duration task</span></span>  | <span data-ttu-id="91e22-129">המאמץ מחושב מחדש.</span><span class="sxs-lookup"><span data-stu-id="91e22-129">Effort is recalculated.</span></span>   | <span data-ttu-id="91e22-130">המאמץ מחושב מחדש.</span><span class="sxs-lookup"><span data-stu-id="91e22-130">Effort is recalculated.</span></span>    | <span data-ttu-id="91e22-131">יחידות מחושבות מחדש.</span><span class="sxs-lookup"><span data-stu-id="91e22-131">Units are recalculated.</span></span>   |

<span data-ttu-id="91e22-132">למידע נוסף אודות ההשלכות של מצב נתון, ראה [שנה את סוג המשימה לתזמון מדויק יותר](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span><span class="sxs-lookup"><span data-stu-id="91e22-132">For more information about the implications of a given mode, see [Change the task type for more accurate scheduling](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span></span> <span data-ttu-id="91e22-133">בנושא, המונח **עבודה** משמש במקום המונח **מאמץ**.</span><span class="sxs-lookup"><span data-stu-id="91e22-133">In the topic, the term **Work** is used instead of **Effort**.</span></span>

## <a name="change-the-organizations-scheduling-mode"></a><span data-ttu-id="91e22-134">שנה את מצב התזמון של הארגון</span><span class="sxs-lookup"><span data-stu-id="91e22-134">Change the organization’s scheduling mode</span></span>

<span data-ttu-id="91e22-135">השלם את השלבים הבאים להגדרת מצב התזמון של ארגון.</span><span class="sxs-lookup"><span data-stu-id="91e22-135">Complete the following steps to define the scheduling mode of an organization.</span></span>

1. <span data-ttu-id="91e22-136">עבור אל **הגדרות** \> **כללי** \> **פרמטרים** ולאחר מכן בחר בפרמטר הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="91e22-136">Go to **Settings** \> **General** \> **Parameters**, and then select the project parameter.</span></span> 
2. <span data-ttu-id="91e22-137">בדף **פרמטרים של הפרויקט**, בחר במצב תזמון ברירת המחדל עבור הארגון, ואז הגדר את היכולת של מנהל הפרויקט לעקוף את ההגדרה בעת יצירת פרויקט חדש.</span><span class="sxs-lookup"><span data-stu-id="91e22-137">On the **Project Parameters** page, select the default scheduling mode for the organization, and then define ability for the Project manager to override the setting when creating a new project.</span></span>

## <a name="change-the-scheduling-mode-setting-on-a-project"></a><span data-ttu-id="91e22-138">שנה את הגדרת מצב התזמון בפרויקט</span><span class="sxs-lookup"><span data-stu-id="91e22-138">Change the scheduling mode setting on a project</span></span>

<span data-ttu-id="91e22-139">אם ארגון מאפשר למנהל הפרויקט לעקוף את מצב תזמון ברירת המחדל, מנהל הפרויקט יכול לבצע את השינוי כאשר הוא יוצר פרויקט חדש.</span><span class="sxs-lookup"><span data-stu-id="91e22-139">If an organization allows the Project manager to override the default scheduling mode, the Project manager can make that change when they create a new project.</span></span> <span data-ttu-id="91e22-140">עם זאת, לאחר שמירת הפרויקט, לא ניתן לשנות את מצב התזמון.</span><span class="sxs-lookup"><span data-stu-id="91e22-140">However, after the project has been saved, the scheduling mode can't be changed.</span></span>

## <a name="copied-projects"></a><span data-ttu-id="91e22-141">הפרוייקטים מועתקים</span><span class="sxs-lookup"><span data-stu-id="91e22-141">Copied projects</span></span>

<span data-ttu-id="91e22-142">מכיוון שפרויקט נוצר בעת ביצוע פעולת ההעתקה של פרויקט, מנהל הפרויקט אינו יכול להגדיר את מצב התזמון.</span><span class="sxs-lookup"><span data-stu-id="91e22-142">Because a project is created when the copy project action is taken, the Project manager can't set the scheduling mode.</span></span> <span data-ttu-id="91e22-143">פרויקט היעד תמיד יהיה כברירת המחדל במצב שהוגדר ברמה הארגונית.</span><span class="sxs-lookup"><span data-stu-id="91e22-143">The destination project will always default to the mode defined at the organizational level.</span></span>

## <a name="copied-tasks"></a><span data-ttu-id="91e22-144">משימות שהועתקו</span><span class="sxs-lookup"><span data-stu-id="91e22-144">Copied tasks</span></span>

<span data-ttu-id="91e22-145">כאשר מועתקת משימה מפרויקט אחד למשנהו, המשימה יורשת את מצב התזמון של פרויקט היעד.</span><span class="sxs-lookup"><span data-stu-id="91e22-145">When a task is copied from one project to another, the task inherits the scheduling mode of the destination project.</span></span>
