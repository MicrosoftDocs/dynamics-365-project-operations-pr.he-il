---
title: אחזור ערכי זמן או הוצאה שאושרו
description: נושא זה מספק מידע אודות אופן האחזור של עסקת זמן או הוצאה שאושרה בעבר.
author: rumant
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 03/08/2019
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation 2.x and 3.x
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 74df6e196c9f060f957d79aebc9640a162fb2913
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751888"
---
# <a name="recall-approved-time-or-expense-entries"></a><span data-ttu-id="fc31f-103">אחזור ערכי זמן או הוצאה שאושרו</span><span class="sxs-lookup"><span data-stu-id="fc31f-103">Recall approved time or expense entries</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="fc31f-104">חבר צוות פרוייקט או אדם אחר השולח ערך זמן או הוצאה יכול לאחזר את ערך הזמן או ההוצאה לאחר אישורו.</span><span class="sxs-lookup"><span data-stu-id="fc31f-104">A project team member or an other person who submits a time or expense entry can recall that time or expense entry after it has been approved.</span></span> <span data-ttu-id="fc31f-105">התהליך לאחזור ערך זמן או הוצאה שאושר כולל שני שלבים:</span><span class="sxs-lookup"><span data-stu-id="fc31f-105">The process for recalling an approved time or expense entry has two steps:</span></span>

1. <span data-ttu-id="fc31f-106">שולח מבקש אחזור.</span><span class="sxs-lookup"><span data-stu-id="fc31f-106">A submitter requests a recall.</span></span>
2. <span data-ttu-id="fc31f-107">מאשר מאשר את האחזור.</span><span class="sxs-lookup"><span data-stu-id="fc31f-107">An approver approves the recall.</span></span>

## <a name="request-a-recall"></a><span data-ttu-id="fc31f-108">בקשה לאחזור</span><span class="sxs-lookup"><span data-stu-id="fc31f-108">Request a recall</span></span>

<span data-ttu-id="fc31f-109">בצע את השלבים הבאים כדי לבקש אחזור של ערך זמן או הוצאה שאושר.</span><span class="sxs-lookup"><span data-stu-id="fc31f-109">Follow these steps to request a recall of an approved time or expense entry.</span></span>

1. <span data-ttu-id="fc31f-110">עבור ערכי זמן, עבור אל **פרוייקטים** \> **העבודה שלי** \> **ערך זמן**.</span><span class="sxs-lookup"><span data-stu-id="fc31f-110">For time entries, go to **Projects** \> **My Work** \> **Time Entry**.</span></span>

    <span data-ttu-id="fc31f-111">-לחלופין-</span><span class="sxs-lookup"><span data-stu-id="fc31f-111">–or–</span></span>

    <span data-ttu-id="fc31f-112">עבור ערכי הוצאה, עבור אל **פרוייקטים** \> **העבודה שלי** \> **הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="fc31f-112">For expense entries, go to **Projects** \> **My Work** \> **Expenses**.</span></span>

2. <span data-ttu-id="fc31f-113">עבור ערכי זמן, בחר את כל ערכי הזמן עבור שילוב מסוים של פרוייקט ומשימה.</span><span class="sxs-lookup"><span data-stu-id="fc31f-113">For time entries, select all the time entries for a specific combination of a project and a task.</span></span> <span data-ttu-id="fc31f-114">לחלופין, ברשת, בחר את התאים הבודדים עבור זמן בתאריך מסוים, עבור פרוייקט ספציפי.</span><span class="sxs-lookup"><span data-stu-id="fc31f-114">Alternatively, in the grid, select the individual cells for time on a specific date for a specific project.</span></span>

    <span data-ttu-id="fc31f-115">-לחלופין-</span><span class="sxs-lookup"><span data-stu-id="fc31f-115">–or–</span></span>

    <span data-ttu-id="fc31f-116">עבור ערכי הוצאה, בחר את השורה עבור ערך ההוצאה לאחזור.</span><span class="sxs-lookup"><span data-stu-id="fc31f-116">For expense entries, select the row for the expense entry to recall.</span></span>

3. <span data-ttu-id="fc31f-117">בחר **אחזור**.</span><span class="sxs-lookup"><span data-stu-id="fc31f-117">Select **Recall**.</span></span> <span data-ttu-id="fc31f-118">תופיע תיבת הדו-שיח לאישור.</span><span class="sxs-lookup"><span data-stu-id="fc31f-118">A confirmation dialog box appears.</span></span> <span data-ttu-id="fc31f-119">אם ערכי הזמן וההוצאה שנבחרו כבר אושרו, תתבקש להזין סיבה לאחזור.</span><span class="sxs-lookup"><span data-stu-id="fc31f-119">If the selected time and expense entries were already approved, you're prompted to enter a reason for the recall.</span></span>
4. <span data-ttu-id="fc31f-120">הזן סיבה לאחזור, ולאחר מכן בחר **אישור** כדי לאשר את הפעולה.</span><span class="sxs-lookup"><span data-stu-id="fc31f-120">Enter a reason for the recall, and then select **OK** to confirm the operation.</span></span> <span data-ttu-id="fc31f-121">המערכת שולחת לאדם שאישר את הערכים בקשה לאישור האחזור.</span><span class="sxs-lookup"><span data-stu-id="fc31f-121">The system sends the person who approved the entries a request to approve the recall.</span></span>

> [!NOTE]
> <span data-ttu-id="fc31f-122">על אף שניתן לאחזר את ערכי הזמן וההוצאה שאושרו, אם כבר הוגשה חשבונית ללקוח עבור זמן או הוצאה שאושרו, לא ניתן ליצור בקשת אחזור.</span><span class="sxs-lookup"><span data-stu-id="fc31f-122">Although approved time and expense entries can be recalled, if an approved time or expense has already been invoiced to the customer, a recall request can't be created.</span></span> <span data-ttu-id="fc31f-123">משתמש שמנסה ליצור בקשה לאחזור יקבל הודעה המציינת שלא ניתן לאחזר את הזמן או ההוצאה מכיוון שכבר הוגשה עבורם חשבונית.</span><span class="sxs-lookup"><span data-stu-id="fc31f-123">A user who tries to create a recall request will receive a message that states that the time or expense can't be recalled because it was already invoiced.</span></span>

## <a name="approve-or-reject-a-recall-request"></a><span data-ttu-id="fc31f-124">אישור או דחייה של בקשת אחזור</span><span class="sxs-lookup"><span data-stu-id="fc31f-124">Approve or reject a recall request</span></span>

<span data-ttu-id="fc31f-125">בצע את השלבים הללו כדי לאשר או לדחות בקשת אחזור.</span><span class="sxs-lookup"><span data-stu-id="fc31f-125">Follow these steps to approve or reject a recall request.</span></span>

1. <span data-ttu-id="fc31f-126">עבור אל **פרוייקטים** \> **העבודה שלי** \> **אישורים**.</span><span class="sxs-lookup"><span data-stu-id="fc31f-126">Go to **Projects** \> **My Work** \> **Approvals**.</span></span>
2. <span data-ttu-id="fc31f-127">בדף הרשימה **אישורים**, שנה את התצוגה ל**בקשות אחזור לאישור**.</span><span class="sxs-lookup"><span data-stu-id="fc31f-127">On the **Approvals** list page, change the view to **Recall requests for approval**.</span></span> <span data-ttu-id="fc31f-128">מוצגת רשימה של בקשות אחזור שנשלחו.</span><span class="sxs-lookup"><span data-stu-id="fc31f-128">A list of submitted recall requests is shown.</span></span>
3. <span data-ttu-id="fc31f-129">בחר ערך אחד או יותר, ולאחר מכן בחר **אשר** או **דחה**.</span><span class="sxs-lookup"><span data-stu-id="fc31f-129">Select one or more entries, and then select either **Approve** or **Reject**.</span></span>
4. <span data-ttu-id="fc31f-130">אם בחרת **אשר**, תקבל הודעת אזהרה שמסבירה את השפעת האישור.</span><span class="sxs-lookup"><span data-stu-id="fc31f-130">If you selected **Approve**, you receive a warning message that explains the impact of the approval.</span></span> <span data-ttu-id="fc31f-131">‏‏בחר **אישור** כדי לאשר את הפעולה.</span><span class="sxs-lookup"><span data-stu-id="fc31f-131">Select **OK** to confirm the operation.</span></span> <span data-ttu-id="fc31f-132">הבקשה לאחזור מאושרת.</span><span class="sxs-lookup"><span data-stu-id="fc31f-132">The recall request is approved.</span></span>

    <span data-ttu-id="fc31f-133">-לחלופין-</span><span class="sxs-lookup"><span data-stu-id="fc31f-133">–or–</span></span>

    <span data-ttu-id="fc31f-134">אם בחרת **דחה**, הבקשה לאחזור נדחית.</span><span class="sxs-lookup"><span data-stu-id="fc31f-134">If you selected **Reject**, the recall request is rejected.</span></span>

> [!NOTE]
> <span data-ttu-id="fc31f-135">בדומה לבקשה לאחזור, בעת אישור אחזור, המערכת בודקת אם קיימת פעילות להפקת חשבוניות לגבי ערכי הזמן או ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="fc31f-135">As when a recall is requested, when a recall is approved, the system checks for any invoicing activity on the time or expense entries.</span></span> <span data-ttu-id="fc31f-136">אם הוגשה כבר חשבונית לגבי ערך כלשהו, או אם הערך מופיע בחשבונית טיוטה, המאשר יקבל הודעת שגיאה המציינת שלא ניתן לאשר אחזור של הזמן או ההוצאה, מכיוון שכבר הוגשה עבורם חשבונית.</span><span class="sxs-lookup"><span data-stu-id="fc31f-136">If an entry was already invoiced, or if it's on a draft invoice, the approver will receive an error message that states that the time or expense can't be approved for recall, because it was already invoiced.</span></span>

## <a name="impact-of-a-recall-request"></a><span data-ttu-id="fc31f-137">השפעת הבקשה לאחזור</span><span class="sxs-lookup"><span data-stu-id="fc31f-137">Impact of a recall request</span></span>

<span data-ttu-id="fc31f-138">כאשר אישור מאוחזר, יש לכך גם השפעה תפעולית וגם השפעה פיננסית.</span><span class="sxs-lookup"><span data-stu-id="fc31f-138">When an approval is recalled, there is both operational impact and financial impact.</span></span>

### <a name="operational-impact"></a><span data-ttu-id="fc31f-139">השפעה תפעולית</span><span class="sxs-lookup"><span data-stu-id="fc31f-139">Operational impact</span></span>

<span data-ttu-id="fc31f-140">אם אושרה בקשת אחזור, רשומת האישור מסומנת כ**נדחה**.</span><span class="sxs-lookup"><span data-stu-id="fc31f-140">If a recall request is approved, the approval record is marked as **Rejected**.</span></span> <span data-ttu-id="fc31f-141">מצב הערך משתנה ל**הוחזר** או ל**נדחה**, תלוי אם מדובר בערך זמן או בערך הוצאה.</span><span class="sxs-lookup"><span data-stu-id="fc31f-141">The status of the entry is changed to either **Returned** or **Rejected**, depending on whether it's a time entry or an expense entry.</span></span>

<span data-ttu-id="fc31f-142">חבר צוות הפרוייקט יכול להציג ערכים, לערוך ולאחר מכן לשלוח מחדש ערכים, או למחוק ערכים באופן מלא.</span><span class="sxs-lookup"><span data-stu-id="fc31f-142">The project team member can view entries, edit and then resubmit entries, or delete entries entirely.</span></span>

<span data-ttu-id="fc31f-143">אם בקשת אחזור נדחתה, הערך נשאר במצב **אושר** וחבר צוות הפרוייקט או המאשר של הפרוייקט לא יכולים לערוך את הערך.</span><span class="sxs-lookup"><span data-stu-id="fc31f-143">If a recall request is rejected, the status of the entry remains **Approved**, and the entry can't be edited by the project team member or the approver for the project.</span></span>

### <a name="financial-impact"></a><span data-ttu-id="fc31f-144">השפעה פיננסית</span><span class="sxs-lookup"><span data-stu-id="fc31f-144">Financial impact</span></span>

<span data-ttu-id="fc31f-145">אם בקשת אחזור אושרה, הנתונים בפועל המתאימים עבור עלות ומכירות מתעדכנים באופן הבא:</span><span class="sxs-lookup"><span data-stu-id="fc31f-145">If a recall request is approved, the corresponding actuals for cost and sales are updated in the following manner:</span></span>

- <span data-ttu-id="fc31f-146">השדה **מצב התאמה** מתעדכן ל**מותאם**.</span><span class="sxs-lookup"><span data-stu-id="fc31f-146">The **Adjustment Status** field is updated to **Adjusted**.</span></span>
- <span data-ttu-id="fc31f-147">השדה **מצב חיוב** מתעדכן ל**בוטל**.</span><span class="sxs-lookup"><span data-stu-id="fc31f-147">The **Billing Status** field is updated to **Canceled**.</span></span>

<span data-ttu-id="fc31f-148">בשלב הבא, ערכי ביטול נוצרים בטבלה 'נתונים בפועל'.</span><span class="sxs-lookup"><span data-stu-id="fc31f-148">Next, reversal entries are created in the Actuals table.</span></span> <span data-ttu-id="fc31f-149">כדי ליצור ערכי ביטול, המערכת מעתיקה את ערכי השדה מהנתונים בפועל המקוריים.</span><span class="sxs-lookup"><span data-stu-id="fc31f-149">To create reversal entries, the system copies over the field values from the original actuals.</span></span> <span data-ttu-id="fc31f-150">הערכים היחידים שאינם מועתקים הם ערכי הכמות.</span><span class="sxs-lookup"><span data-stu-id="fc31f-150">The only values that aren't copied over are the quantity values.</span></span> <span data-ttu-id="fc31f-151">ערכים אלה חוזרים לקדמותם במקום זאת.</span><span class="sxs-lookup"><span data-stu-id="fc31f-151">These values are reversed instead.</span></span> <span data-ttu-id="fc31f-152">נתונים בפועל שבוטלו נוצרים הן עבור נתונים בפועל של **עלות** והן עבור נתונים בפועל של **מכירות שלא חויבו**.</span><span class="sxs-lookup"><span data-stu-id="fc31f-152">Reversed actuals are created for both **Cost** and **Unbilled Sales** actuals.</span></span> <span data-ttu-id="fc31f-153">השדה **מצב התאמה** של הנתונים בפועל שהתבטלו מוגדר ל**לא ניתן להתאמה** והשדה **מצב חיוב** מוגדר ל**בוטל**.</span><span class="sxs-lookup"><span data-stu-id="fc31f-153">The **Adjustment Status** field on the reversed actuals is set to **Unadjustable**, and the **Billing status** field is set to **Canceled**.</span></span> <span data-ttu-id="fc31f-154">בגלל שינויים אלה, הסכום שמתועד כסכום שהושקע ומצבור ההכנסות בפרוייקט לא ייחשבו עוד לסכומים שנתונים בפועל אלה מייצגים.</span><span class="sxs-lookup"><span data-stu-id="fc31f-154">Because of these changes, the recorded spending and the revenue backlog on the project will no longer account for the amounts that these actuals represent.</span></span>

<span data-ttu-id="fc31f-155">אם בקשת אחזור נדחית, אין לכך השפעה פיננסית על הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="fc31f-155">If a recall request is rejected, there is no financial impact on the project.</span></span>

## <a name="changes-to-time-entry-records"></a><span data-ttu-id="fc31f-156">שינויים ברשומות של ערכי זמן</span><span class="sxs-lookup"><span data-stu-id="fc31f-156">Changes to time entry records</span></span>

<span data-ttu-id="fc31f-157">האיור הבא מציג את השינויים המתרחשים עבור ערכי זמן שאושרו בזמן האחזור שלהם.</span><span class="sxs-lookup"><span data-stu-id="fc31f-157">The following illustration shows the changes that occur for approved time entries when they are recalled.</span></span>

![מעברים בין מצבים של ערכי זמן](media/TimeEntryStateTransitions.png)

## <a name="changes-to-expense-entry-records"></a><span data-ttu-id="fc31f-159">שינויים ברשומות של ערכי הוצאה</span><span class="sxs-lookup"><span data-stu-id="fc31f-159">Changes to expense entry records</span></span>

<span data-ttu-id="fc31f-160">האיור הבא מציג את השינויים המתרחשים עבור ערכי הוצאה שאושרו בזמן האחזור שלהם.</span><span class="sxs-lookup"><span data-stu-id="fc31f-160">The following illustration shows the changes that occur for approved expense entries when they are recalled.</span></span>

![מעברים בין מצבים של ערכי הוצאה](media/ExpenseEntryStateTransitions.png)
