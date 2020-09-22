---
title: ביטול ערכי זמן והוצאה שאושרו בעבר
description: נושא זה מספק מידע אודות אופן הביטול של עסקת זמן והוצאה של פרוייקט שאושרה.
author: rumant
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 03/07/2019
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 2fc74aba2a837b7cdff55385ffa20d78c2678bb7
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751720"
---
# <a name="cancel-previously-approved-time-or-expense-entries"></a><span data-ttu-id="5d3f0-103">ביטול ערכי זמן או הוצאה שאושרו בעבר</span><span class="sxs-lookup"><span data-stu-id="5d3f0-103">Cancel previously approved time or expense entries</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="5d3f0-104">בגירסה העדכנית ביותר של Dynamics 365 Project Service Automation, מאשרים יכולים לבטל ערכי זמן או הוצאה שאושרו בעבר.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-104">In the latest version of Dynamics 365 Project Service Automation, approvers can cancel time or expense entries that they previously approved.</span></span>

## <a name="cancel-a-previously-approved-time-or-expense-entry"></a><span data-ttu-id="5d3f0-105">ביטול ערך זמן או הוצאה שאושר בעבר</span><span class="sxs-lookup"><span data-stu-id="5d3f0-105">Cancel a previously approved time or expense entry</span></span>

<span data-ttu-id="5d3f0-106">בצע את השלבים הבאים כדי לבטל ערך זמן או הוצאה שאישרת בעבר.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-106">Follow these steps to cancel a time or expense entry that you previously approved.</span></span>

1. <span data-ttu-id="5d3f0-107">עבור אל **פרוייקטים** \> **העבודה שלי** \> **אישורים**.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-107">Go to **Projects** \> **My Work** \> **Approvals**.</span></span>
2. <span data-ttu-id="5d3f0-108">בדף הרשימה **אישורים**, שנה את התצוגה ל**האישורים הקודמים שלי**.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-108">On the **Approvals** list page, change the view to **My past approvals**.</span></span> <span data-ttu-id="5d3f0-109">רשימה של ערכי הזמן וההוצאות שאישרת בעבר מוצגת.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-109">A list of the time and expense entries that you previously approved is shown.</span></span>
3. <span data-ttu-id="5d3f0-110">בחר ערך אחד או יותר, ולאחר מכן בחר **בטל אישור**.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-110">Select one or more entries, and then select **Cancel approval**.</span></span> <span data-ttu-id="5d3f0-111">תקבל הודעת אזהרה.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-111">You receive a warning message.</span></span>
4. <span data-ttu-id="5d3f0-112">בחר **אישור** כדי לבטל את האישור.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-112">Select **OK** to cancel the approval.</span></span>

## <a name="understand-the-impact-of-canceling-a-time-or-expense-entry-approval"></a><span data-ttu-id="5d3f0-113">הבנת ההשפעה של ביטול אישור של ערך זמן או הוצאה</span><span class="sxs-lookup"><span data-stu-id="5d3f0-113">Understand the impact of canceling a time or expense entry approval</span></span>

<span data-ttu-id="5d3f0-114">כאשר אישור מבוטל, יש לכך גם השפעה תפעולית וגם השפעה פיננסית.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-114">When an approval is canceled, there is both operational impact and financial impact.</span></span>

### <a name="operational-impact"></a><span data-ttu-id="5d3f0-115">השפעה תפעולית</span><span class="sxs-lookup"><span data-stu-id="5d3f0-115">Operational impact</span></span>

<span data-ttu-id="5d3f0-116">מבחינת התפעול, כאשר אישור מבוטל, מצב הרשומה מאופס ל**טיוטה**, והאישור אינו מופיע עוד בתצוגה **האישורים הקודמים שלי**.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-116">On the operations side, when an approval is canceled, the status of the record is reset to **Draft**, and the approval no longer appears in the **My past approvals** view.</span></span> <span data-ttu-id="5d3f0-117">במקום זאת, האישור המבוטל מופיע בתצוגה **ערכי זמן לאישור** או בתצוגה **ערכי הוצאות לאישור**, בהתאם לשאלה אם זה היה ערך זמן או ערך הוצאה.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-117">Instead, the canceled approval appears in either the **Time entries for approval** view or the **Expense entries for approval** view, depending on whether it was a time entry or an expense entry.</span></span> <span data-ttu-id="5d3f0-118">בנוסף, המצב של ערך הזמן או ערך ההוצאה הקשור משתנה ל**נשלח**, כך שהערך הקשור תואם לאישורים בעלי מצב **טיוטה**.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-118">Additionally, the status of the related time or expense entry is changed to **Submitted**, so that the related entry is consistent with approvals that have a status of **Draft**.</span></span>

<span data-ttu-id="5d3f0-119">כמאשר, באפשרותך לערוך חלק משדות האישור בעל מצב **טיוטה**.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-119">As an approver, you can edit some of the fields of an approval that has a status of **Draft**.</span></span> <span data-ttu-id="5d3f0-120">שדות אלה כוללים את **סוג חיוב** ואת **שעות לחיוב עבור ערכי זמן**.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-120">These fields include **Billing Type** and **Billable Hours for Time Entries**.</span></span> <span data-ttu-id="5d3f0-121">לאחר ביצוע שינויים, באפשרותך לאשר שוב את הרשומה.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-121">After you make changes, you can approve the record again.</span></span> <span data-ttu-id="5d3f0-122">לחלופין, באפשרותך לדחות את הערך.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-122">Alternatively, you can reject the entry.</span></span> <span data-ttu-id="5d3f0-123">אם תדחה את האישור של ערך זמן, מצב הערך ישתנה ל**הוחזר**.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-123">If you reject the approval of a time entry, the status of the entry is changed to **Returned**.</span></span> <span data-ttu-id="5d3f0-124">אם תדחה את האישור של ערך הוצאה, המצב ישתנה ל**נדחה**.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-124">If you reject the approval of an expense entry, the status is changed to **Rejected**.</span></span> <span data-ttu-id="5d3f0-125">מבחינה פונקציונלית, הן הערכים שהוחזרו והן הערכים שנדחו מתנהגים כמו ערך בעל מצב של **טיוטה**.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-125">Functionally, both returned and rejected entries behave the same as an entry that has a status of **Draft**.</span></span> <span data-ttu-id="5d3f0-126">חבר צוות של פרוייקט יכול לבצע שינויים נדרשים בערך ולאחר מכן לשלוח אותו מחדש לאישור, או למחוק את הערך לחלוטין.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-126">A project team member can either make any required changes to the entry and then resubmit it for approval, or delete the entry entirely.</span></span>

### <a name="financial-impact"></a><span data-ttu-id="5d3f0-127">השפעה פיננסית</span><span class="sxs-lookup"><span data-stu-id="5d3f0-127">Financial impact</span></span>

<span data-ttu-id="5d3f0-128">פרוייקט מושפע גם מבחינה פיננסית כאשר אישור מבוטל.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-128">A project is also affected financially when an approval is canceled.</span></span> <span data-ttu-id="5d3f0-129">ראשית, הנתונים בפועל המתאימים עבור עלות ומכירות מתעדכנים באופן הבא:</span><span class="sxs-lookup"><span data-stu-id="5d3f0-129">First, the corresponding actuals for cost and sales are updated in the following manner:</span></span>

- <span data-ttu-id="5d3f0-130">מצב ההתאמה מוגדר ל**מותאם**.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-130">The adjustment status is set to **Adjusted**.</span></span>
- <span data-ttu-id="5d3f0-131">מצב החיוב מוגדר ל**בוטל**.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-131">The billing status is set to **Canceled**.</span></span>

<span data-ttu-id="5d3f0-132">בשלב הבא, ערכי ביטול נוצרים בטבלה 'נתונים בפועל'.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-132">Next, reversal entries are created in the Actuals table.</span></span> <span data-ttu-id="5d3f0-133">כדי ליצור ערכי ביטול, המערכת מעתיקה את ערכי השדה מהנתונים בפועל המקוריים.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-133">To create reversal entries, the system copies over the field values from the original actuals.</span></span> <span data-ttu-id="5d3f0-134">הערכים היחידים שאינם מועתקים הם ערכי הכמות.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-134">The only values that aren't copied over are the quantity values.</span></span> <span data-ttu-id="5d3f0-135">ערכים אלה חוזרים לקדמותם במקום זאת.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-135">These values are reversed instead.</span></span> <span data-ttu-id="5d3f0-136">נתונים בפועל שבוטלו נוצרים הן עבור נתונים בפועל של **עלות** והן עבור נתונים בפועל של **מכירות שלא חויבו**.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-136">Reversed actuals are created for both **Cost** and **Unbilled Sales** actuals.</span></span> <span data-ttu-id="5d3f0-137">השדה **מצב התאמה** של הנתונים בפועל שהתבטלו מוגדר ל**לא ניתן להתאמה** ומצב החיוב מוגדר ל**בוטל**.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-137">The **Adjustment Status** field on the reversed actuals is set to **Unadjustable**, and the billing status is set to **Canceled**.</span></span>

<span data-ttu-id="5d3f0-138">לאחר ששינויים אלה מתבצעים, הסכום שמתועד כסכום שהושקע בפרוייקט ומצבור ההכנסות בפרוייקט לא ייחשבו עוד לסכומים שנתונים בפועל אלה מייצגים.</span><span class="sxs-lookup"><span data-stu-id="5d3f0-138">After these changes are made, the amount that is recorded as spent on the project and the revenue backlog on the project will longer account for the amounts that these actuals represent.</span></span>
