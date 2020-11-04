---
title: אחזור ערכי זמן או הוצאה שאושרו
description: נושא זה מספק מידע אודות אופן האחזור של עסקת זמן או הוצאה שאושרה בעבר.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: ''
ms.author: rumant
ms.date: 03/08/2019
ms.topic: article
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 7bacd70881a6c463cc449a365173da5338a3d3fc
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077355"
---
# <a name="recall-approved-time-or-expense-entries"></a><span data-ttu-id="87a37-103">אחזור ערכי זמן או הוצאה שאושרו</span><span class="sxs-lookup"><span data-stu-id="87a37-103">Recall approved time or expense entries</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="87a37-104">חבר צוות פרויקט או אדם אחר השולח ערך זמן או הוצאה יכול לאחזר את ערך הזמן או ההוצאה לאחר אישורו.</span><span class="sxs-lookup"><span data-stu-id="87a37-104">A project team member or an other person who submits a time or expense entry can recall that time or expense entry after it has been approved.</span></span> <span data-ttu-id="87a37-105">התהליך לאחזור ערך זמן או הוצאה שאושר כולל שני שלבים:</span><span class="sxs-lookup"><span data-stu-id="87a37-105">The process for recalling an approved time or expense entry has two steps:</span></span>

1. <span data-ttu-id="87a37-106">שולח מבקש אחזור.</span><span class="sxs-lookup"><span data-stu-id="87a37-106">A submitter requests a recall.</span></span>
2. <span data-ttu-id="87a37-107">מאשר מאשר את האחזור.</span><span class="sxs-lookup"><span data-stu-id="87a37-107">An approver approves the recall.</span></span>

## <a name="request-a-recall"></a><span data-ttu-id="87a37-108">בקשה לאחזור</span><span class="sxs-lookup"><span data-stu-id="87a37-108">Request a recall</span></span>

<span data-ttu-id="87a37-109">בצע את השלבים הבאים כדי לבקש אחזור של ערך זמן או הוצאה שאושר.</span><span class="sxs-lookup"><span data-stu-id="87a37-109">Follow these steps to request a recall of an approved time or expense entry.</span></span>

1. <span data-ttu-id="87a37-110">עבור ערכי זמן, עבור אל **פרויקטים** \> **העבודה שלי** \> **ערך זמן**.</span><span class="sxs-lookup"><span data-stu-id="87a37-110">For time entries, go to **Projects** \> **My Work** \> **Time Entry**.</span></span>

    <span data-ttu-id="87a37-111">-לחלופין-</span><span class="sxs-lookup"><span data-stu-id="87a37-111">–or–</span></span>

    <span data-ttu-id="87a37-112">עבור ערכי הוצאה, עבור אל **פרויקטים** \> **העבודה שלי** \> **הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="87a37-112">For expense entries, go to **Projects** \> **My Work** \> **Expenses**.</span></span>

2. <span data-ttu-id="87a37-113">עבור ערכי זמן, בחר את כל ערכי הזמן עבור שילוב מסוים של פרויקט ומשימה.</span><span class="sxs-lookup"><span data-stu-id="87a37-113">For time entries, select all the time entries for a specific combination of a project and a task.</span></span> <span data-ttu-id="87a37-114">לחלופין, ברשת, בחר את התאים הבודדים עבור זמן בתאריך מסוים, עבור פרויקט ספציפי.</span><span class="sxs-lookup"><span data-stu-id="87a37-114">Alternatively, in the grid, select the individual cells for time on a specific date for a specific project.</span></span>

    <span data-ttu-id="87a37-115">-לחלופין-</span><span class="sxs-lookup"><span data-stu-id="87a37-115">–or–</span></span>

    <span data-ttu-id="87a37-116">עבור ערכי הוצאה, בחר את השורה עבור ערך ההוצאה לאחזור.</span><span class="sxs-lookup"><span data-stu-id="87a37-116">For expense entries, select the row for the expense entry to recall.</span></span>

3. <span data-ttu-id="87a37-117">בחר **אחזור**.</span><span class="sxs-lookup"><span data-stu-id="87a37-117">Select **Recall**.</span></span> <span data-ttu-id="87a37-118">תופיע תיבת הדו-שיח לאישור.</span><span class="sxs-lookup"><span data-stu-id="87a37-118">A confirmation dialog box appears.</span></span> <span data-ttu-id="87a37-119">אם ערכי הזמן וההוצאה שנבחרו כבר אושרו, תתבקש להזין סיבה לאחזור.</span><span class="sxs-lookup"><span data-stu-id="87a37-119">If the selected time and expense entries were already approved, you're prompted to enter a reason for the recall.</span></span>
4. <span data-ttu-id="87a37-120">הזן סיבה לאחזור, ולאחר מכן בחר **אישור** כדי לאשר את הפעולה.</span><span class="sxs-lookup"><span data-stu-id="87a37-120">Enter a reason for the recall, and then select **OK** to confirm the operation.</span></span> <span data-ttu-id="87a37-121">המערכת שולחת לאדם שאישר את הערכים בקשה לאישור האחזור.</span><span class="sxs-lookup"><span data-stu-id="87a37-121">The system sends the person who approved the entries a request to approve the recall.</span></span>

> [!NOTE]
> <span data-ttu-id="87a37-122">על אף שניתן לאחזר את ערכי הזמן וההוצאה שאושרו, אם כבר הוגשה חשבונית ללקוח עבור זמן או הוצאה שאושרו, לא ניתן ליצור בקשת אחזור.</span><span class="sxs-lookup"><span data-stu-id="87a37-122">Although approved time and expense entries can be recalled, if an approved time or expense has already been invoiced to the customer, a recall request can't be created.</span></span> <span data-ttu-id="87a37-123">משתמש שמנסה ליצור בקשה לאחזור יקבל הודעה המציינת שלא ניתן לאחזר את הזמן או ההוצאה מכיוון שכבר הוגשה עבורם חשבונית.</span><span class="sxs-lookup"><span data-stu-id="87a37-123">A user who tries to create a recall request will receive a message that states that the time or expense can't be recalled because it was already invoiced.</span></span>

## <a name="approve-or-reject-a-recall-request"></a><span data-ttu-id="87a37-124">אישור או דחייה של בקשת אחזור</span><span class="sxs-lookup"><span data-stu-id="87a37-124">Approve or reject a recall request</span></span>

<span data-ttu-id="87a37-125">בצע את השלבים הללו כדי לאשר או לדחות בקשת אחזור.</span><span class="sxs-lookup"><span data-stu-id="87a37-125">Follow these steps to approve or reject a recall request.</span></span>

1. <span data-ttu-id="87a37-126">עבור אל **פרויקטים** \> **העבודה שלי** \> **אישורים**.</span><span class="sxs-lookup"><span data-stu-id="87a37-126">Go to **Projects** \> **My Work** \> **Approvals**.</span></span>
2. <span data-ttu-id="87a37-127">בדף הרשימה **אישורים** , שנה את התצוגה ל **בקשות אחזור לאישור**.</span><span class="sxs-lookup"><span data-stu-id="87a37-127">On the **Approvals** list page, change the view to **Recall requests for approval**.</span></span> <span data-ttu-id="87a37-128">מוצגת רשימה של בקשות אחזור שנשלחו.</span><span class="sxs-lookup"><span data-stu-id="87a37-128">A list of submitted recall requests is shown.</span></span>
3. <span data-ttu-id="87a37-129">בחר ערך אחד או יותר, ולאחר מכן בחר **אשר** או **דחה**.</span><span class="sxs-lookup"><span data-stu-id="87a37-129">Select one or more entries, and then select either **Approve** or **Reject**.</span></span>
4. <span data-ttu-id="87a37-130">אם בחרת **אשר** , תקבל הודעת אזהרה שמסבירה את השפעת האישור.</span><span class="sxs-lookup"><span data-stu-id="87a37-130">If you selected **Approve** , you receive a warning message that explains the impact of the approval.</span></span> <span data-ttu-id="87a37-131">‏‏בחר **אישור** כדי לאשר את הפעולה.</span><span class="sxs-lookup"><span data-stu-id="87a37-131">Select **OK** to confirm the operation.</span></span> <span data-ttu-id="87a37-132">הבקשה לאחזור מאושרת.</span><span class="sxs-lookup"><span data-stu-id="87a37-132">The recall request is approved.</span></span>

    <span data-ttu-id="87a37-133">-לחלופין-</span><span class="sxs-lookup"><span data-stu-id="87a37-133">–or–</span></span>

    <span data-ttu-id="87a37-134">אם בחרת **דחה** , הבקשה לאחזור נדחית.</span><span class="sxs-lookup"><span data-stu-id="87a37-134">If you selected **Reject** , the recall request is rejected.</span></span>

> [!NOTE]
> <span data-ttu-id="87a37-135">בדומה לבקשה לאחזור, בעת אישור אחזור, המערכת בודקת אם קיימת פעילות להפקת חשבוניות לגבי ערכי הזמן או ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="87a37-135">As when a recall is requested, when a recall is approved, the system checks for any invoicing activity on the time or expense entries.</span></span> <span data-ttu-id="87a37-136">אם הוגשה כבר חשבונית לגבי ערך כלשהו, או אם הערך מופיע בחשבונית טיוטה, המאשר יקבל הודעת שגיאה המציינת שלא ניתן לאשר אחזור של הזמן או ההוצאה, מכיוון שכבר הוגשה עבורם חשבונית.</span><span class="sxs-lookup"><span data-stu-id="87a37-136">If an entry was already invoiced, or if it's on a draft invoice, the approver will receive an error message that states that the time or expense can't be approved for recall, because it was already invoiced.</span></span>

## <a name="impact-of-a-recall-request"></a><span data-ttu-id="87a37-137">השפעת הבקשה לאחזור</span><span class="sxs-lookup"><span data-stu-id="87a37-137">Impact of a recall request</span></span>

<span data-ttu-id="87a37-138">כאשר אישור מאוחזר, יש לכך גם השפעה תפעולית וגם השפעה פיננסית.</span><span class="sxs-lookup"><span data-stu-id="87a37-138">When an approval is recalled, there is both operational impact and financial impact.</span></span>

### <a name="operational-impact"></a><span data-ttu-id="87a37-139">השפעה תפעולית</span><span class="sxs-lookup"><span data-stu-id="87a37-139">Operational impact</span></span>

<span data-ttu-id="87a37-140">אם אושרה בקשת אחזור, רשומת האישור מסומנת כ **נדחה**.</span><span class="sxs-lookup"><span data-stu-id="87a37-140">If a recall request is approved, the approval record is marked as **Rejected**.</span></span> <span data-ttu-id="87a37-141">מצב הערך משתנה ל **הוחזר** או ל **נדחה** , תלוי אם מדובר בערך זמן או בערך הוצאה.</span><span class="sxs-lookup"><span data-stu-id="87a37-141">The status of the entry is changed to either **Returned** or **Rejected** , depending on whether it's a time entry or an expense entry.</span></span>

<span data-ttu-id="87a37-142">חבר צוות הפרויקט יכול להציג ערכים, לערוך ולאחר מכן לשלוח מחדש ערכים, או למחוק ערכים באופן מלא.</span><span class="sxs-lookup"><span data-stu-id="87a37-142">The project team member can view entries, edit and then resubmit entries, or delete entries entirely.</span></span>

<span data-ttu-id="87a37-143">אם בקשת אחזור נדחתה, הערך נשאר במצב **אושר** וחבר צוות הפרויקט או המאשר של הפרויקט לא יכולים לערוך את הערך.</span><span class="sxs-lookup"><span data-stu-id="87a37-143">If a recall request is rejected, the status of the entry remains **Approved** , and the entry can't be edited by the project team member or the approver for the project.</span></span>

### <a name="financial-impact"></a><span data-ttu-id="87a37-144">השפעה פיננסית</span><span class="sxs-lookup"><span data-stu-id="87a37-144">Financial impact</span></span>

<span data-ttu-id="87a37-145">אם בקשת אחזור אושרה, הנתונים בפועל המתאימים עבור עלות ומכירות מתעדכנים באופן הבא:</span><span class="sxs-lookup"><span data-stu-id="87a37-145">If a recall request is approved, the corresponding actuals for cost and sales are updated in the following manner:</span></span>

- <span data-ttu-id="87a37-146">השדה **מצב התאמה** מתעדכן ל **מותאם**.</span><span class="sxs-lookup"><span data-stu-id="87a37-146">The **Adjustment Status** field is updated to **Adjusted**.</span></span>
- <span data-ttu-id="87a37-147">השדה **מצב חיוב** מתעדכן ל **בוטל**.</span><span class="sxs-lookup"><span data-stu-id="87a37-147">The **Billing Status** field is updated to **Canceled**.</span></span>

<span data-ttu-id="87a37-148">בשלב הבא, ערכי ביטול נוצרים בטבלה 'נתונים בפועל'.</span><span class="sxs-lookup"><span data-stu-id="87a37-148">Next, reversal entries are created in the Actuals table.</span></span> <span data-ttu-id="87a37-149">כדי ליצור ערכי ביטול, המערכת מעתיקה את ערכי השדה מהנתונים בפועל המקוריים.</span><span class="sxs-lookup"><span data-stu-id="87a37-149">To create reversal entries, the system copies over the field values from the original actuals.</span></span> <span data-ttu-id="87a37-150">הערכים היחידים שאינם מועתקים הם ערכי הכמות.</span><span class="sxs-lookup"><span data-stu-id="87a37-150">The only values that aren't copied over are the quantity values.</span></span> <span data-ttu-id="87a37-151">ערכים אלה חוזרים לקדמותם במקום זאת.</span><span class="sxs-lookup"><span data-stu-id="87a37-151">These values are reversed instead.</span></span> <span data-ttu-id="87a37-152">נתונים בפועל שבוטלו נוצרים הן עבור נתונים בפועל של **עלות** והן עבור נתונים בפועל של **מכירות שלא חויבו**.</span><span class="sxs-lookup"><span data-stu-id="87a37-152">Reversed actuals are created for both **Cost** and **Unbilled Sales** actuals.</span></span> <span data-ttu-id="87a37-153">השדה **מצב התאמה** של הנתונים בפועל שהתבטלו מוגדר ל **לא ניתן להתאמה** והשדה **מצב חיוב** מוגדר ל **בוטל**.</span><span class="sxs-lookup"><span data-stu-id="87a37-153">The **Adjustment Status** field on the reversed actuals is set to **Unadjustable** , and the **Billing status** field is set to **Canceled**.</span></span> <span data-ttu-id="87a37-154">בגלל שינויים אלה, הסכום שמתועד כסכום שהושקע ומצבור ההכנסות בפרויקט לא ייחשבו עוד לסכומים שנתונים בפועל אלה מייצגים.</span><span class="sxs-lookup"><span data-stu-id="87a37-154">Because of these changes, the recorded spending and the revenue backlog on the project will no longer account for the amounts that these actuals represent.</span></span>

<span data-ttu-id="87a37-155">אם בקשת אחזור נדחית, אין לכך השפעה פיננסית על הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="87a37-155">If a recall request is rejected, there is no financial impact on the project.</span></span>

## <a name="changes-to-time-entry-records"></a><span data-ttu-id="87a37-156">שינויים ברשומות של ערכי זמן</span><span class="sxs-lookup"><span data-stu-id="87a37-156">Changes to time entry records</span></span>

<span data-ttu-id="87a37-157">האיור הבא מציג את השינויים המתרחשים עבור ערכי זמן שאושרו בזמן האחזור שלהם.</span><span class="sxs-lookup"><span data-stu-id="87a37-157">The following illustration shows the changes that occur for approved time entries when they are recalled.</span></span>

![מעברים בין מצבים של ערכי זמן](media/TimeEntryStateTransitions.png)

## <a name="changes-to-expense-entry-records"></a><span data-ttu-id="87a37-159">שינויים ברשומות של ערכי הוצאה</span><span class="sxs-lookup"><span data-stu-id="87a37-159">Changes to expense entry records</span></span>

<span data-ttu-id="87a37-160">האיור הבא מציג את השינויים המתרחשים עבור ערכי הוצאה שאושרו בזמן האחזור שלהם.</span><span class="sxs-lookup"><span data-stu-id="87a37-160">The following illustration shows the changes that occur for approved expense entries when they are recalled.</span></span>

![מעברים בין מצבים של ערכי הוצאה](media/ExpenseEntryStateTransitions.png)
