---
title: הגדרת קטגוריות הוצאות
description: נושא זה מספק מידע על הדרך להגדרת קטגוריות הוצאות וקטגוריות משותפות עבור דוחות הוצאות.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: f051d70f3dfe3b241dc0a206c0cdfda000f87c76
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077198"
---
# <a name="set-up-expense-categories"></a><span data-ttu-id="51314-103">הגדרת קטגוריות הוצאות</span><span class="sxs-lookup"><span data-stu-id="51314-103">Set up expense categories</span></span>

<span data-ttu-id="51314-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="51314-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="51314-105">כאשר עובדים יוצרים דוחות הוצאות, כל הוצאה שהם רושמים חייבת להיות משויכת לקטגוריית הוצאות.</span><span class="sxs-lookup"><span data-stu-id="51314-105">When employees create expense reports, each expense that they record must be associated with an expense category.</span></span> <span data-ttu-id="51314-106">קטגוריות הוצאות נגזרות מקטגוריות משותפות הניתנות לשיתוף בין הגופים המשפטיים בארגון.</span><span class="sxs-lookup"><span data-stu-id="51314-106">Expense categories are derived from shared categories that can be shared across the legal entities in your organization.</span></span> <span data-ttu-id="51314-107">בהתאם להגדרת הארגון, ניתן לשתף קטגוריות הוצאות אלה גם בתחומים אחרים.</span><span class="sxs-lookup"><span data-stu-id="51314-107">Depending on how your organization is defined, these expense categories can also be shared in other areas.</span></span> <span data-ttu-id="51314-108">בהתבסס על הגדרת הארגון ועל ההנחיות מצוות היישום, עליך לקבוע אם הקטגוריות שנמצאות בשימוש לניהול הוצאות יהיו בשימוש רק בניהול הוצאות או שיש לשתף אותן בתחומים אחרים.</span><span class="sxs-lookup"><span data-stu-id="51314-108">Based on the definition of your organization and guidance from the implementation team, you must determine whether the categories that are used in Expense management will be used only in Expense management or should be shared in other areas.</span></span>

> [!NOTE]
> <span data-ttu-id="51314-109">ניתן לשתף קטגוריות אלה בין 'ניהול פרויקטים וחשבונאות' ו'ניהול הוצאות', או בין 'ניהול פרויקטים וחשבונאות' ו'ייצור'.</span><span class="sxs-lookup"><span data-stu-id="51314-109">These categories can be shared between Project management and accounting and Expense management, or between Project management and accounting and Production.</span></span> <span data-ttu-id="51314-110">עם זאת, לא ניתן לשתף אותן בין 'ניהול הוצאות' ו'ייצור'.</span><span class="sxs-lookup"><span data-stu-id="51314-110">However, they can't be shared between Expense management and Production.</span></span>

<span data-ttu-id="51314-111">לפני שמתחילים בתהליך ההגדרה, יש לקבל את ההחלטות הבאות עבור כל קטגוריית הוצאות:</span><span class="sxs-lookup"><span data-stu-id="51314-111">Before you can begin the setup process, the following decisions must be made for each expense category:</span></span>

- <span data-ttu-id="51314-112">מהי קטגוריית ההוצאות?</span><span class="sxs-lookup"><span data-stu-id="51314-112">What is the expense category?</span></span> <span data-ttu-id="51314-113">דוגמאות לקטגוריות הוצאות כוללות טיסות, בתי מלון או קילומטראז'.</span><span class="sxs-lookup"><span data-stu-id="51314-113">Examples include categories for flights, hotel, or mileage.</span></span>
- <span data-ttu-id="51314-114">האם ניתן להשתמש בקטגוריית ההוצאות גם בניהול פרויקטים וחשבונאות?</span><span class="sxs-lookup"><span data-stu-id="51314-114">Can the expense category also be used in Project management and accounting?</span></span> <span data-ttu-id="51314-115">אם כן, יש לקבל גם את ההחלטות הבאות:</span><span class="sxs-lookup"><span data-stu-id="51314-115">If it can, you must also make the following decisions:</span></span>

    - <span data-ttu-id="51314-116">אילו חשבונות עלות יהיו בשימוש עבור ההוצאות הבאות?</span><span class="sxs-lookup"><span data-stu-id="51314-116">Which cost accounts will be used for the following expenses?</span></span>

        - <span data-ttu-id="51314-117">עלות</span><span class="sxs-lookup"><span data-stu-id="51314-117">Cost</span></span>
        - <span data-ttu-id="51314-118">הקצאת שכר</span><span class="sxs-lookup"><span data-stu-id="51314-118">Payroll allocation</span></span>
        - <span data-ttu-id="51314-119">WIP-ערך עלות</span><span class="sxs-lookup"><span data-stu-id="51314-119">WIP-cost value</span></span>
        - <span data-ttu-id="51314-120">פריט-עלות</span><span class="sxs-lookup"><span data-stu-id="51314-120">Cost-item</span></span>
        - <span data-ttu-id="51314-121">WIP-ערך עלות-פריט</span><span class="sxs-lookup"><span data-stu-id="51314-121">WIP-cost value-item</span></span>
        - <span data-ttu-id="51314-122">הפסד נצבר</span><span class="sxs-lookup"><span data-stu-id="51314-122">Accrued loss</span></span>
        - <span data-ttu-id="51314-123">WIP-הפסד נצבר</span><span class="sxs-lookup"><span data-stu-id="51314-123">WIP-accrued loss</span></span>

    - <span data-ttu-id="51314-124">אילו חשבונות הכנסות ישמשו למקורות ההכנסה הבאים?</span><span class="sxs-lookup"><span data-stu-id="51314-124">Which revenue accounts will be used for the following sources of revenue?</span></span>

        - <span data-ttu-id="51314-125">הכנסה שחויבה</span><span class="sxs-lookup"><span data-stu-id="51314-125">Invoiced revenue</span></span>
        - <span data-ttu-id="51314-126">הכנסה נצברת-ערך מכירה</span><span class="sxs-lookup"><span data-stu-id="51314-126">Accrued revenue-sales value</span></span>
        - <span data-ttu-id="51314-127">WIP-ערך מכירה</span><span class="sxs-lookup"><span data-stu-id="51314-127">WIP-sales value</span></span>
        - <span data-ttu-id="51314-128">הכנסה נצברת-ייצור</span><span class="sxs-lookup"><span data-stu-id="51314-128">Accrued revenue-production</span></span>
        - <span data-ttu-id="51314-129">WIP-ייצור</span><span class="sxs-lookup"><span data-stu-id="51314-129">WIP-production</span></span>
        - <span data-ttu-id="51314-130">הכנסה נצברת-רווח</span><span class="sxs-lookup"><span data-stu-id="51314-130">Accrued revenue-profit</span></span>
        - <span data-ttu-id="51314-131">WIP-רווח</span><span class="sxs-lookup"><span data-stu-id="51314-131">WIP-profit</span></span>
        - <span data-ttu-id="51314-132">הכנסה נצברת-מנוי</span><span class="sxs-lookup"><span data-stu-id="51314-132">Accrued revenue-subscription</span></span>
        - <span data-ttu-id="51314-133">WIP-מנוי</span><span class="sxs-lookup"><span data-stu-id="51314-133">WIP-subscription</span></span>

- <span data-ttu-id="51314-134">מהו סוג ההוצאה?</span><span class="sxs-lookup"><span data-stu-id="51314-134">What is the expense type?</span></span>
- <span data-ttu-id="51314-135">מהו אמצעי התשלום המוגדר כברירת מחדל עבור קטגוריית ההוצאות?</span><span class="sxs-lookup"><span data-stu-id="51314-135">What is the default payment method for the expense category?</span></span>
- <span data-ttu-id="51314-136">האם יש לפרט את ההוצאות בקטגוריית ההוצאות?</span><span class="sxs-lookup"><span data-stu-id="51314-136">Do expenses in the expense category have to be itemized?</span></span>
- <span data-ttu-id="51314-137">מהו החשבון הראשי המוגדר כברירת מחדל עבור קטגוריית ההוצאות?</span><span class="sxs-lookup"><span data-stu-id="51314-137">What is the main default account for the expense category?</span></span>
- <span data-ttu-id="51314-138">מהי קבוצת המע"מ לפריט המוגדרת כברירת מחדל עבור קטגוריית ההוצאות?</span><span class="sxs-lookup"><span data-stu-id="51314-138">What is the default item sales tax group for the expense category?</span></span>
- <span data-ttu-id="51314-139">האם מותר להשתמש באמצעי תשלום נוספים עבור קטגוריית ההוצאות?</span><span class="sxs-lookup"><span data-stu-id="51314-139">Are additional payment methods allowed for the expense category?</span></span> <span data-ttu-id="51314-140">אם כן, מה הם?</span><span class="sxs-lookup"><span data-stu-id="51314-140">If so, what are they?</span></span>
- <span data-ttu-id="51314-141">האם יש קטגוריות משנה בקטגוריית הוצאות זו?</span><span class="sxs-lookup"><span data-stu-id="51314-141">Are there subcategories in this expense category?</span></span> <span data-ttu-id="51314-142">אם כן, יש לקבל גם את ההחלטות הבאות:</span><span class="sxs-lookup"><span data-stu-id="51314-142">If there are subcategories, you must also make the following decisions:</span></span>

    - <span data-ttu-id="51314-143">האם קטגוריות משנה כלשהן לא נכללות בהשבת מס?</span><span class="sxs-lookup"><span data-stu-id="51314-143">Are any of the subcategories excluded from tax recovery?</span></span>
    - <span data-ttu-id="51314-144">מהי קבוצת המע"מ לפריט של קטגוריות המשנה?</span><span class="sxs-lookup"><span data-stu-id="51314-144">What is the item sales tax group of the subcategories?</span></span>
