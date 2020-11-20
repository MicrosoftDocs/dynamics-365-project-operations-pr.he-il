---
title: הזנת הוצאות (לייט)
description: נושא זה מספק מידע על אופן העבודה עם הזנת הוצאות בפריסה בגרסת לייט.
author: stsporen
manager: AnnBe
ms.date: 10/06/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 536c961593599df8e7e2986f92259b0e690eae8b
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121084"
---
# <a name="expense-entry-lite"></a><span data-ttu-id="57dd6-103">הזנת הוצאות (לייט)</span><span class="sxs-lookup"><span data-stu-id="57dd6-103">Expense entry (lite)</span></span>

<span data-ttu-id="57dd6-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="57dd6-104">_**Applies to:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="57dd6-105">ניהול הוצאות בסיסי, או לייט, הוא היכולת לרשום הוצאות פשוטות.</span><span class="sxs-lookup"><span data-stu-id="57dd6-105">Basic, or lite, expense management is the capability to record simple expenses.</span></span> <span data-ttu-id="57dd6-106">ניתן לרשום הוצאות כנגד פרויקט, ולאחר מכן מאשר הפרויקט יבדוק ויאשר אותן.</span><span class="sxs-lookup"><span data-stu-id="57dd6-106">You can record expenses against a project, and then the project approver will review and approve them.</span></span>

<span data-ttu-id="57dd6-107">לקבלת מידע נוסף אודות יכולות הוצאות ב-Dynamics 365 Project Operations, ראה [מבט כולל על הוצאות](expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="57dd6-107">For more information about expense capabilities in Dynamics 365 Project Operations, see [Expense overview](expense-overview.md).</span></span>

## <a name="capture-a-basic-expense"></a><span data-ttu-id="57dd6-108">לכידת הוצאה בסיסית</span><span class="sxs-lookup"><span data-stu-id="57dd6-108">Capture a basic expense</span></span>

<span data-ttu-id="57dd6-109">ניתן יכול ללכוד את ההוצאות כדי שתוכל להגיש אותן למאשר.</span><span class="sxs-lookup"><span data-stu-id="57dd6-109">You can capture your expenses so that you can submit them to the approver.</span></span>

1. <span data-ttu-id="57dd6-110">עבור אל **הוצאות**, ובחר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="57dd6-110">Go to **Expenses**, and select **New**.</span></span>
2. <span data-ttu-id="57dd6-111">בדף **הוצאה חדשה**, הזן את פרטים הנדרשים על ההוצאה ולאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="57dd6-111">On the **New Expense** page, enter the required expense information, and then select **Save**.</span></span>

## <a name="submit-a-basic-expense"></a><span data-ttu-id="57dd6-112">הגשת הוצאה בסיסית</span><span class="sxs-lookup"><span data-stu-id="57dd6-112">Submit a basic expense</span></span>

<span data-ttu-id="57dd6-113">לאחר שסיימת ללכוד את כל ההוצאות שלך, ואתה מוכן שיאשרו אותן, עליך להגיש אותן לאישור.</span><span class="sxs-lookup"><span data-stu-id="57dd6-113">After you've finished capturing all your expenses, and you're ready to have them approved, you must submit them.</span></span>

1. <span data-ttu-id="57dd6-114">עבור אל **הוצאות**, ובחר בהוצאה.</span><span class="sxs-lookup"><span data-stu-id="57dd6-114">Go to **Expenses**, and select an expense.</span></span> <span data-ttu-id="57dd6-115">לחלופין, בחר בכול ההוצאות באמצעות תיבת הסימון שבכותרת העליונה.</span><span class="sxs-lookup"><span data-stu-id="57dd6-115">Or, select all the expenses by using the check box on the header.</span></span>
2. <span data-ttu-id="57dd6-116">בחר **שלח**.</span><span class="sxs-lookup"><span data-stu-id="57dd6-116">Select **Submit**.</span></span> <span data-ttu-id="57dd6-117">המערכת מעבדת את הערכים שנבחרו ואז יוצרת בקשות לאישור הוצאות.</span><span class="sxs-lookup"><span data-stu-id="57dd6-117">The system processes the selected entries and then creates expense approval requests.</span></span>

## <a name="recall-a-basic-expense"></a><span data-ttu-id="57dd6-118">אחזור של הוצאה בסיסית</span><span class="sxs-lookup"><span data-stu-id="57dd6-118">Recall a basic expense</span></span>

<span data-ttu-id="57dd6-119">כשאתה מגיש הוצאה בטעות, אתה יכול לאחזר אותה.</span><span class="sxs-lookup"><span data-stu-id="57dd6-119">When you submit an expense by mistake, you can recall it.</span></span> <span data-ttu-id="57dd6-120">הזמן הנדרש לצורך אחזור ערך הוצאה תלוי בשלב האישור שלו.</span><span class="sxs-lookup"><span data-stu-id="57dd6-120">The time that is required to recall an expense entry depends on its approval stage.</span></span>  <span data-ttu-id="57dd6-121">אם המאשר עדיין לא אישר את הערך, האחזור יכול להתרחש באופן מיידי.</span><span class="sxs-lookup"><span data-stu-id="57dd6-121">If the approver hasn't yet approved the entry, the recall can occur immediately.</span></span> <span data-ttu-id="57dd6-122">אך אם הערך כבר אושר, המאשר יתבקש לאשר את אחזור ולבטל את העסקאות.</span><span class="sxs-lookup"><span data-stu-id="57dd6-122">However, if the entry has already been approved, the approver is asked to approve the recall and reverse the transactions.</span></span>

1. <span data-ttu-id="57dd6-123">עבור אל **הוצאות** ולאחר מכן, ברשימת ההוצאות, בחר את ההוצאה לאחזור.</span><span class="sxs-lookup"><span data-stu-id="57dd6-123">Go to **Expenses**, and then, in the list of expenses, select the expense to recall.</span></span>
2. <span data-ttu-id="57dd6-124">בחר **אחזור**.</span><span class="sxs-lookup"><span data-stu-id="57dd6-124">Select **Recall**.</span></span> <span data-ttu-id="57dd6-125">אם ערך ההוצאה טרם אושר, המערכת תאחזר אותו מיד.</span><span class="sxs-lookup"><span data-stu-id="57dd6-125">If the expense entry hasn't yet been approved, the system immediately recalls it.</span></span> <span data-ttu-id="57dd6-126">אם ערך ההוצאה כבר אושר, נוצרת בקשת אחזור כדי להודיע למאושר שברצונך לבטל את ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="57dd6-126">If the expense entry has already been approved, a recall request is created to notify the approver that you want to reverse the expense.</span></span> <span data-ttu-id="57dd6-127">בשלב זה המאשר יאשר שניתן לבצע את הביטול, והערך יוחזר.</span><span class="sxs-lookup"><span data-stu-id="57dd6-127">The approver will then confirm that the reversal can be done, and the entry will be returned.</span></span>

## <a name="delete-a-basic-expense"></a><span data-ttu-id="57dd6-128">מחיקת הוצאה בסיסית</span><span class="sxs-lookup"><span data-stu-id="57dd6-128">Delete a basic expense</span></span>

<span data-ttu-id="57dd6-129">ניתן למחוק הוצאות שטרם הוגשו.</span><span class="sxs-lookup"><span data-stu-id="57dd6-129">Expenses that haven't yet been submitted can be deleted.</span></span> <span data-ttu-id="57dd6-130">כדי למחוק הוצאה שכבר הוגשה, תחילה עליך לאחזר אותה.</span><span class="sxs-lookup"><span data-stu-id="57dd6-130">To delete an expense that has already been submitted, you must first recall it.</span></span>

## <a name="see-also"></a><span data-ttu-id="57dd6-131">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="57dd6-131">See also</span></span>

- [<span data-ttu-id="57dd6-132">מבט כולל על אישורים</span><span class="sxs-lookup"><span data-stu-id="57dd6-132">Approvals overview</span></span>](../approvals/approvals-overview.md)
