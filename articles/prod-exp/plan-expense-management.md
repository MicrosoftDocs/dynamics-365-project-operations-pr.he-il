---
title: קביעת תצורה של ניהול הוצאות
description: מאמר זה מתאר את השיקולים שעליך להביא בחשבון ואת ההחלטות שעליך לקבל במהלך תהליך התכנון לפני קביעת התצורה של ניהול ההוצאות ב- Microsoft Dynamics 365 Finance.
author: KimANelson
manager: AnnBe
ms.date: 08/29/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: GlobalCategory, ProjCategory, TrvLocations, TrvParameters, TrvPaymethod, TrvPerDiems
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 23001
ms.assetid: aa3fd14d-7e94-4603-985f-ca26d6f860ea
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: e2291515cc154fb5b34ca5802135791958bea1e5
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077456"
---
# <a name="configure-expense-management"></a><span data-ttu-id="49f5f-103">קביעת תצורה של ניהול הוצאות</span><span class="sxs-lookup"><span data-stu-id="49f5f-103">Configure expense management</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="49f5f-104">נושא זה מתאר את השיקולים שעליך להביא בחשבון ואת ההחלטות שעליך לקבל במהלך תהליך התכנון לפני קביעת התצורה של ניהול ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="49f5f-104">This topic describes the considerations and the decisions that you must make during the planning process before you configure Expense management.</span></span> <span data-ttu-id="49f5f-105">בניהול הוצאות, אתה יכול לאחסן מידע על אמצעי תשלום, דרישות נסיעה, דוחות הוצאות, מדיניות ועוד.</span><span class="sxs-lookup"><span data-stu-id="49f5f-105">In Expense management, you can store information about payment methods, travel requisitions, expense reports, policies, and so on.</span></span>

<span data-ttu-id="49f5f-106">מכיוון שרבות מההחלטות שתקבל בעת תכנון התצורה של ניהול ההוצאות מבוססות על המבנה ההיררכי והפיננסי של הארגון שלך, עליך לעיין במסמכי התכנון לתחומים אלה.</span><span class="sxs-lookup"><span data-stu-id="49f5f-106">Because many of the decisions that you make when you plan your configuration for Expense management are based on your organization’s hierarchy and financial structure, you must refer to the planning documents for those areas.</span></span>

## <a name="intercompany-expenses"></a><span data-ttu-id="49f5f-107">הוצאות בין-חברתיות</span><span class="sxs-lookup"><span data-stu-id="49f5f-107">Intercompany expenses</span></span>

<span data-ttu-id="49f5f-108">כאשר אתה מאפשר הוצאות בין-חברתיות, אתה מאפשר לישויות משפטיות ולעובדים לצבור הוצאות מטעם ישות משפטית אחרת ולגבות תשלום מהישות המשפטית של התעסוקה בתוך הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="49f5f-108">When you enable intercompany expenses, you allow legal entities and employees to incur expenses on behalf of another legal entity, and collect payment from the legal entity of employment within your organization.</span></span> <span data-ttu-id="49f5f-109">לדוגמה, עובד בישות משפטית א' משלים פרויקט עבור ישות משפטית ב', והפרויקט צובר הוצאות הקשורות לנסיעות.</span><span class="sxs-lookup"><span data-stu-id="49f5f-109">For example, an employee in legal entity A completes a project for legal entity B, and the project incurs travel related expenses.</span></span> <span data-ttu-id="49f5f-110">אם ההוצאות הבין-חברתיות זמינות, העובד יכול להגיש דוח הוצאות אשר ירשום את ההוצאה אצל ישות משפטית ב' וישות משפטית א' תצטרך לשלם את ההוצאה. אם לארגון שלך אין מספר ישויות משפטיות, אתה לא צריך להפוך את ההוצאות הבין-חברתיות לזמינות.</span><span class="sxs-lookup"><span data-stu-id="49f5f-110">If intercompany expenses are enabled, the employee can then file an expense report that will post the expense to legal entity B, and the expense must then be paid by legal entity A. If your organization doesn’t have multiple legal entities, you don’t have to enable intercompany expenses.</span></span>

<span data-ttu-id="49f5f-111">**החלטה:** האם אתה רוצה להפוך הוצאות בין-חברתיות לזמינות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-111">**Decision:** Do you want to enable intercompany expenses?</span></span>

## <a name="financial-management"></a><span data-ttu-id="49f5f-112">ניהול פיננסי</span><span class="sxs-lookup"><span data-stu-id="49f5f-112">Financial management</span></span>

<span data-ttu-id="49f5f-113">ניהול ההוצאות משולב היטב בניהול הפיננסי של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="49f5f-113">Expense management is tightly integrated with the financial management of your organization.</span></span> <span data-ttu-id="49f5f-114">הרבה מהתצורה של ניהול ההוצאות תתבסס על ההחלטות שקיבלת בנוגע לכספים של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="49f5f-114">Lots of your configuration for Expense management will be based on the decisions that you’ve made about your organization’s finances.</span></span> <span data-ttu-id="49f5f-115">הסעיפים הבאים מתארים את התחומים השונים הדורשים תכנון והחלטות, בהתבסס על ההחלטות הכספיות של הארגון ועל הדרכה מצוות המנהלים שלך.</span><span class="sxs-lookup"><span data-stu-id="49f5f-115">The following sections describe the various areas that require planning and decisions, based on your organization’s financial decisions and guidance from your leadership team.</span></span>

### <a name="per-diems"></a><span data-ttu-id="49f5f-116">אש"ל</span><span class="sxs-lookup"><span data-stu-id="49f5f-116">Per diems</span></span>

<span data-ttu-id="49f5f-117">עליך להגדיר את דמי האש"ל ליום שהארגון שלך מספק לעובדים.</span><span class="sxs-lookup"><span data-stu-id="49f5f-117">You must define the employee per diems that your organization provides.</span></span> <span data-ttu-id="49f5f-118">מכיוון שדמי האש"ל משמשים בדרך כלל לכיסוי הוצאות כגון ארוחות, לינה והוצאות נלוות אחרות, אתה יכול ליצור כללים לקצבאות דמי האש"ל שהארגון שלך מציע.</span><span class="sxs-lookup"><span data-stu-id="49f5f-118">Because per diems are typically used to cover expenses such as meals, lodging, and other incidental expenses, you can create rules for the per diem allowances that your organization offers.</span></span> <span data-ttu-id="49f5f-119">תעריפי אש"ל יכולים להתבסס על תקופת השנה, על יעד הנסיעה או על שניהם.</span><span class="sxs-lookup"><span data-stu-id="49f5f-119">per diem rates can be based on the time of year, the travel location, or both.</span></span> <span data-ttu-id="49f5f-120">כשמגדירים כלל לדמי אש"ל, אפשר לקבוע שאחוז מתעריף האש"ל ינוכה אם עובד מקבל ארוחות או שירותים בחינם.</span><span class="sxs-lookup"><span data-stu-id="49f5f-120">When you define a per diem rule, you can specify that a percentage of the per diem rate will be withheld if a worker receives complimentary meals or services.</span></span> <span data-ttu-id="49f5f-121">ניתן גם להגדיר רמות של תעריף אש"ל כדי להגדיר מספר שעות מינימלי ומקסימלי להחלת דמי אש"ל על נסיעה של עובד.</span><span class="sxs-lookup"><span data-stu-id="49f5f-121">You can also define per diem rate tiers to set the minimum and maximum number of hours that the per diem rate can be applied to a worker’s travel.</span></span>

<span data-ttu-id="49f5f-122">**החלטות:**</span><span class="sxs-lookup"><span data-stu-id="49f5f-122">**Decisions:**</span></span>

- <span data-ttu-id="49f5f-123">כללי דמי אש"ל בברירת מחדל ליום הראשון והאחרון:</span><span class="sxs-lookup"><span data-stu-id="49f5f-123">Default per diem rules for the first and last days:</span></span>

    - <span data-ttu-id="49f5f-124">מהו מספר השעות המינימלי שעובד יכול להצהיר ביום ועדיין לקבל דמי אש"ל?</span><span class="sxs-lookup"><span data-stu-id="49f5f-124">What is the minimum number of hours that an employee can claim for a day and still receive a per diem?</span></span>
    - <span data-ttu-id="49f5f-125">האם יש הפחתה בסכום המוצע לארוחות ביום הראשון וביום האחרון?</span><span class="sxs-lookup"><span data-stu-id="49f5f-125">Is there a reduction in the amount that is offered for meals for the first day and last day?</span></span> <span data-ttu-id="49f5f-126">אם יש הפחתה, מה אחוז ההפחתה?</span><span class="sxs-lookup"><span data-stu-id="49f5f-126">If there is a reduction, what is the percentage of the reduction?</span></span>
    - <span data-ttu-id="49f5f-127">האם יש הפחתה בסכום המוצע לבית מלון ביום הראשון וביום האחרון?</span><span class="sxs-lookup"><span data-stu-id="49f5f-127">Is there a reduction in the amount that is offered for a hotel for the first day and last day?</span></span> <span data-ttu-id="49f5f-128">אם יש הפחתה, מה אחוז ההפחתה?</span><span class="sxs-lookup"><span data-stu-id="49f5f-128">If there is a reduction, what is the percentage of the reduction?</span></span>
    - <span data-ttu-id="49f5f-129">האם יש הפחתה בסכום המוצע להוצאות אחרות שנצברות ביום הראשון וביום האחרון?</span><span class="sxs-lookup"><span data-stu-id="49f5f-129">Is there a reduction in the amount that is offered for other expenses that are incurred on the first day and last day?</span></span> <span data-ttu-id="49f5f-130">אם יש הפחתה, מה אחוז ההפחתה?</span><span class="sxs-lookup"><span data-stu-id="49f5f-130">If there is a reduction, what is the percentage of the reduction?</span></span>

- <span data-ttu-id="49f5f-131">כללי דמי אש"ל בברירת מחדל:</span><span class="sxs-lookup"><span data-stu-id="49f5f-131">Default per diem rules:</span></span>

    - <span data-ttu-id="49f5f-132">האם יש הפחתה באחוזים של קצבת דמי האש"ל עבור כל ארוחה אם, למשל, הארוחה היא בחינם?</span><span class="sxs-lookup"><span data-stu-id="49f5f-132">Is there a percentage reduction in the per diem allowance for each meal if, for example, the meal is complimentary?</span></span> <span data-ttu-id="49f5f-133">אם יש הפחתה, מה אחוז ההפחתה לכל ארוחה?</span><span class="sxs-lookup"><span data-stu-id="49f5f-133">If there is a reduction, what is the reduction percentage for each meal?</span></span>
    - <span data-ttu-id="49f5f-134">האם ההפחתה עבור הארוחה מחושבת ליום, לנסיעה או לפי מספר הארוחות ביום?</span><span class="sxs-lookup"><span data-stu-id="49f5f-134">Is the meal reduction calculated per day, per trip, or by the number of meals per day?</span></span>
    - <span data-ttu-id="49f5f-135">האם יש לעגל סכומי אש"ל באופן רגיל או האם לעגל כלפי מעלה?</span><span class="sxs-lookup"><span data-stu-id="49f5f-135">Should per diem amounts be rounded in the regular manner or rounded up?</span></span>
    - <span data-ttu-id="49f5f-136">האם דמי האש"ל מחושבים לפי תקופה של 24 שעות או לפי יום קלנדרי?</span><span class="sxs-lookup"><span data-stu-id="49f5f-136">Are per diems calculated on a 24-hour period or on a calendar day?</span></span>

- <span data-ttu-id="49f5f-137">כללים לדמי אש"ל המבוססים על מיקום:</span><span class="sxs-lookup"><span data-stu-id="49f5f-137">Per diem rules that are based on location:</span></span>

    - <span data-ttu-id="49f5f-138">האם תעריפי האש"ל משתנים בהתאם למיקום?</span><span class="sxs-lookup"><span data-stu-id="49f5f-138">Do per diem rates vary according to location?</span></span> <span data-ttu-id="49f5f-139">אילו מיקומים כלולים?</span><span class="sxs-lookup"><span data-stu-id="49f5f-139">What locations are included?</span></span>
    - <span data-ttu-id="49f5f-140">אם תעריפי האש"ל משתנים בהתאם למיקום, עבור כל מיקום, איזה סכום באחוזים ניתן עבור סוגי ההוצאות הבאים:</span><span class="sxs-lookup"><span data-stu-id="49f5f-140">If per diem rates vary according to location, for each location, what percentage amount is provided for the following types of expenses:</span></span>

        - <span data-ttu-id="49f5f-141">ארוחות</span><span class="sxs-lookup"><span data-stu-id="49f5f-141">Meals</span></span>
        - <span data-ttu-id="49f5f-142">בתי מלון</span><span class="sxs-lookup"><span data-stu-id="49f5f-142">Hotel</span></span>
        - <span data-ttu-id="49f5f-143">הוצאות אחרות</span><span class="sxs-lookup"><span data-stu-id="49f5f-143">Other expenses</span></span>

### <a name="expense-management-journals-and-accounts"></a><span data-ttu-id="49f5f-144">יומנים וחשבונות של ניהול הוצאות</span><span class="sxs-lookup"><span data-stu-id="49f5f-144">Expense management journals and accounts</span></span>

<span data-ttu-id="49f5f-145">ניהול הוצאות מחייב שימוש במספר יומנים וחשבונות.</span><span class="sxs-lookup"><span data-stu-id="49f5f-145">Expense management requires that you use multiple journals and accounts.</span></span> <span data-ttu-id="49f5f-146">עליך להחליט, למשל, האם אותו חשבון משמש גם למקדמות במזומן וגם למחלוקות בנוגע לכרטיסי אשראי.</span><span class="sxs-lookup"><span data-stu-id="49f5f-146">You must decide, for example, whether the same account is used for cash advances and credit card disputes.</span></span>

<span data-ttu-id="49f5f-147">**החלטות:**</span><span class="sxs-lookup"><span data-stu-id="49f5f-147">**Decisions:**</span></span>

- <span data-ttu-id="49f5f-148">באיזה יומן ספר ראשי מדווחים על דוחות הוצאות שאושרו?</span><span class="sxs-lookup"><span data-stu-id="49f5f-148">Which ledger journal are approved expense reports posted to?</span></span>
- <span data-ttu-id="49f5f-149">איזה חשבון משמש למקדמות במזומן?</span><span class="sxs-lookup"><span data-stu-id="49f5f-149">Which account is used for cash advances?</span></span>
- <span data-ttu-id="49f5f-150">האם יש לרשום מקדמות במזומן באופן מיידי?</span><span class="sxs-lookup"><span data-stu-id="49f5f-150">Should cash advances be posted immediately?</span></span>

### <a name="payment-methods"></a><span data-ttu-id="49f5f-151">שיטות תשלום</span><span class="sxs-lookup"><span data-stu-id="49f5f-151">Payment methods</span></span>

<span data-ttu-id="49f5f-152">כאשר אתה מאפשר לעובדים לצבור הוצאות מטעם העסק שלך, עליך להגדיר את אמצעי התשלום בהם העובדים רשאים להשתמש.</span><span class="sxs-lookup"><span data-stu-id="49f5f-152">When you allow employees to incur expenses on behalf of your business, you must define the payment methods that employees are allowed to use.</span></span> <span data-ttu-id="49f5f-153">לדוגמה, אתה יכול לאפשר לעובדים להשתמש במזומן או בכרטיס אשראי ארגוני.</span><span class="sxs-lookup"><span data-stu-id="49f5f-153">For example, you might allow employees to use cash or a corporate credit card.</span></span> <span data-ttu-id="49f5f-154">אתה יכול גם לאפשר לעובדים להשתמש בכרטיסי אשראי אישיים ואז לתת להם החזר.</span><span class="sxs-lookup"><span data-stu-id="49f5f-154">You might also allow employees to use personal credit cards, and then reimburse the employees.</span></span> <span data-ttu-id="49f5f-155">עליך לקבל את ההחלטות הבאות עבור כל אמצעי תשלום שאתה מאפשר.</span><span class="sxs-lookup"><span data-stu-id="49f5f-155">You must make the following decisions for each payment method that you allow.</span></span>

<span data-ttu-id="49f5f-156">**החלטות:**</span><span class="sxs-lookup"><span data-stu-id="49f5f-156">**Decisions:**</span></span>

- <span data-ttu-id="49f5f-157">אילו אמצעי תשלום מותרים?</span><span class="sxs-lookup"><span data-stu-id="49f5f-157">What payment methods are allowed?</span></span>
- <span data-ttu-id="49f5f-158">בבעלות מי ההוצאות של אמצעי התשלום?</span><span class="sxs-lookup"><span data-stu-id="49f5f-158">Who owns the payment method expenses?</span></span>
- <span data-ttu-id="49f5f-159">האם יש סוג חשבון קיזוז?</span><span class="sxs-lookup"><span data-stu-id="49f5f-159">Is there an offset account type?</span></span> <span data-ttu-id="49f5f-160">אם יש סוג חשבון קיזוז, מה הסוג?</span><span class="sxs-lookup"><span data-stu-id="49f5f-160">If there is an offset account type, what is it?</span></span>
- <span data-ttu-id="49f5f-161">אם יש חשבון קיזוז, מה החשבון?</span><span class="sxs-lookup"><span data-stu-id="49f5f-161">If there is an offset account, what is the account?</span></span>
- <span data-ttu-id="49f5f-162">אם אמצעי התשלום הוא כרטיס אשראי, האם להשתמש באמצעי התשלום רק בעסקאות שיובאו?</span><span class="sxs-lookup"><span data-stu-id="49f5f-162">If the payment method is a credit card, should the payment method be used only with imported transactions?</span></span>

### <a name="expense-categories-and-shared-categories"></a><span data-ttu-id="49f5f-163">קטגוריות הוצאה וקטגוריות משותפות</span><span class="sxs-lookup"><span data-stu-id="49f5f-163">Expense categories and shared categories</span></span>

<span data-ttu-id="49f5f-164">כאשר עובדים יוצרים דוח הוצאות, כל הוצאה שהם רושמים חייבת להיות משויכת לקטגוריית הוצאות.</span><span class="sxs-lookup"><span data-stu-id="49f5f-164">When employees create an expense report, each expense that they record must be associated with an expense category.</span></span> <span data-ttu-id="49f5f-165">קטגוריות הוצאות נגזרות מקטגוריות משותפות הניתנות לשיתוף בין הגופים המשפטיים בארגון.</span><span class="sxs-lookup"><span data-stu-id="49f5f-165">Expense categories are derived from shared categories that can be shared across the legal entities in your organization.</span></span> <span data-ttu-id="49f5f-166">ניתן גם לשתף קטגוריות אלה בניהול פרויקטים ובחשבונאות, בהתאם לאופן ההגדרה של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="49f5f-166">These categories can also be shared in Project management and accounting, depending on the way that your organization is defined.</span></span> <span data-ttu-id="49f5f-167">בהתבסס על הגדרת הארגון ועל ההנחיות מצוות היישום, עליך לקבוע אם הקטגוריות שנמצאות בשימוש לניהול הוצאות יהיו בשימוש רק בניהול הוצאות או שיש לשתף אותן בין ניהול פרויקטים וחשבונאות לבין ניהול הוצאות.</span><span class="sxs-lookup"><span data-stu-id="49f5f-167">Based on the definition of your organization and guidance from the implementation team, determine whether the categories that are used in Expense management will be used only in Expense management, or whether they should be shared between Project management and accounting and Expense management.</span></span> <span data-ttu-id="49f5f-168">שים לב שניתן לשתף קטגוריות אלה בין פרויקט והוצאות או בין פרויקט וייצור, אבל לא בין הוצאות וייצור.</span><span class="sxs-lookup"><span data-stu-id="49f5f-168">Note that these categories can be shared between Project and Expense or Project and Production, but not between Expense and Production.</span></span> <span data-ttu-id="49f5f-169">עליך לקבל את ההחלטות הבאות עבור כל קטגוריית הוצאה.</span><span class="sxs-lookup"><span data-stu-id="49f5f-169">You must make the following decisions for each expense category.</span></span>

<span data-ttu-id="49f5f-170">**החלטות:**</span><span class="sxs-lookup"><span data-stu-id="49f5f-170">**Decisions:**</span></span>

- <span data-ttu-id="49f5f-171">מהי קטגוריית ההוצאות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-171">What is the expense category?</span></span> <span data-ttu-id="49f5f-172">דוגמאות לקטגוריות הוצאות כוללות טיסות, בתי מלון או קילומטראז'.</span><span class="sxs-lookup"><span data-stu-id="49f5f-172">Examples include categories for flights, hotel, or mileage.</span></span>
- <span data-ttu-id="49f5f-173">האם ניתן להשתמש בקטגוריית ההוצאות גם בניהול פרוייקטים וחשבונאות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-173">Can the expense category also be used in Project management and accounting?</span></span>
- <span data-ttu-id="49f5f-174">מהו סוג ההוצאה?</span><span class="sxs-lookup"><span data-stu-id="49f5f-174">What is the expense type?</span></span>
- <span data-ttu-id="49f5f-175">מהו אמצעי התשלום המוגדר כברירת מחדל עבור קטגוריית ההוצאות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-175">What is the default payment method for the expense category?</span></span>
- <span data-ttu-id="49f5f-176">האם יש לפרט את ההוצאות בקטגוריית ההוצאות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-176">Do expenses in the expense category have to be itemized?</span></span>
- <span data-ttu-id="49f5f-177">מהו החשבון הראשי המוגדר כברירת מחדל עבור קטגוריית ההוצאות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-177">What is the main default account for the expense category?</span></span>
- <span data-ttu-id="49f5f-178">מהי קבוצת המע"מ לפריט המוגדרת כברירת מחדל עבור קטגוריית ההוצאות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-178">What is the default item sales tax group for the expense category?</span></span>
- <span data-ttu-id="49f5f-179">האם מותר להשתמש באמצעי תשלום נוספים עבור קטגוריית ההוצאות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-179">Are additional payment methods allowed for the expense category?</span></span> <span data-ttu-id="49f5f-180">אם מותר להשתמש באמצעי תשלום נוספים, מה הם?</span><span class="sxs-lookup"><span data-stu-id="49f5f-180">If additional payment methods are allowed, what are they?</span></span>
- <span data-ttu-id="49f5f-181">האם יש קטגוריות משנה בקטגוריית הוצאות זו?</span><span class="sxs-lookup"><span data-stu-id="49f5f-181">Are there subcategories in this expense category?</span></span> <span data-ttu-id="49f5f-182">אם כן, יש לקבל גם את ההחלטות הבאות:</span><span class="sxs-lookup"><span data-stu-id="49f5f-182">If there are subcategories, you must also make the following decisions:</span></span>

    - <span data-ttu-id="49f5f-183">האם קטגוריות משנה כלשהן לא נכללות בהשבת מס?</span><span class="sxs-lookup"><span data-stu-id="49f5f-183">Are any of the subcategories excluded from tax recovery?</span></span>
    - <span data-ttu-id="49f5f-184">מהי קבוצת המע"מ לפריט של קטגוריות המשנה?</span><span class="sxs-lookup"><span data-stu-id="49f5f-184">What is the item sales tax group of the subcategories?</span></span>

<span data-ttu-id="49f5f-185">אם נעשה שימוש בקטגוריית ההוצאה גם בניהול פרויקטים ובחשבונאות, ענה על השאלות הנותרות.</span><span class="sxs-lookup"><span data-stu-id="49f5f-185">If the expense category is also used in Project management and accounting, answer the remaining questions.</span></span> <span data-ttu-id="49f5f-186">אם לא, עבור לסעיף הבא.</span><span class="sxs-lookup"><span data-stu-id="49f5f-186">Otherwise, move on to the next section.</span></span>

- <span data-ttu-id="49f5f-187">אילו חשבונות עלות יהיו בשימוש עבור ההוצאות הבאות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-187">Which cost accounts will be used for the following expenses?</span></span>

    - <span data-ttu-id="49f5f-188">עלות</span><span class="sxs-lookup"><span data-stu-id="49f5f-188">Cost</span></span>
    - <span data-ttu-id="49f5f-189">הקצאת שכר</span><span class="sxs-lookup"><span data-stu-id="49f5f-189">Payroll allocation</span></span>
    - <span data-ttu-id="49f5f-190">WIP-ערך עלות</span><span class="sxs-lookup"><span data-stu-id="49f5f-190">WIP-cost value</span></span>
    - <span data-ttu-id="49f5f-191">פריט-עלות</span><span class="sxs-lookup"><span data-stu-id="49f5f-191">Cost-item</span></span>
    - <span data-ttu-id="49f5f-192">WIP-ערך עלות-פריט</span><span class="sxs-lookup"><span data-stu-id="49f5f-192">WIP-cost value-item</span></span>
    - <span data-ttu-id="49f5f-193">הפסד נצבר</span><span class="sxs-lookup"><span data-stu-id="49f5f-193">Accrued loss</span></span>
    - <span data-ttu-id="49f5f-194">WIP-הפסד נצבר</span><span class="sxs-lookup"><span data-stu-id="49f5f-194">WIP-accrued loss</span></span>

- <span data-ttu-id="49f5f-195">אילו חשבונות של הכנסות יהיו בשימוש עבור ההכנסות הבאות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-195">Which revenue accounts will be used for the following?</span></span>

    - <span data-ttu-id="49f5f-196">הכנסה שחויבה</span><span class="sxs-lookup"><span data-stu-id="49f5f-196">Invoiced revenue</span></span>
    - <span data-ttu-id="49f5f-197">הכנסה נצברת-ערך מכירה</span><span class="sxs-lookup"><span data-stu-id="49f5f-197">Accrued revenue-sales value</span></span>
    - <span data-ttu-id="49f5f-198">WIP-ערך מכירה</span><span class="sxs-lookup"><span data-stu-id="49f5f-198">WIP-sales value</span></span>
    - <span data-ttu-id="49f5f-199">הכנסה נצברת-ייצור</span><span class="sxs-lookup"><span data-stu-id="49f5f-199">Accrued revenue-production</span></span>
    - <span data-ttu-id="49f5f-200">WIP-ייצור</span><span class="sxs-lookup"><span data-stu-id="49f5f-200">WIP-production</span></span>
    - <span data-ttu-id="49f5f-201">הכנסה נצברת-רווח</span><span class="sxs-lookup"><span data-stu-id="49f5f-201">Accrued revenue-profit</span></span>
    - <span data-ttu-id="49f5f-202">WIP-רווח</span><span class="sxs-lookup"><span data-stu-id="49f5f-202">WIP-profit</span></span>
    - <span data-ttu-id="49f5f-203">הכנסה נצברת-מנוי</span><span class="sxs-lookup"><span data-stu-id="49f5f-203">Accrued revenue-subscription</span></span>
    - <span data-ttu-id="49f5f-204">WIP-מנוי</span><span class="sxs-lookup"><span data-stu-id="49f5f-204">WIP-subscription</span></span>

### <a name="taxes"></a><span data-ttu-id="49f5f-205">מסים</span><span class="sxs-lookup"><span data-stu-id="49f5f-205">Taxes</span></span>

<span data-ttu-id="49f5f-206">עבור מיסים הקשורים להוצאות, עליך לקבוע מה נכלל או זמין בדוחות ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="49f5f-206">For expense-related taxes, you must determine what is included or enabled on expense reports.</span></span>

<span data-ttu-id="49f5f-207">**החלטות:**</span><span class="sxs-lookup"><span data-stu-id="49f5f-207">**Decisions:**</span></span>

- <span data-ttu-id="49f5f-208">האם מס מכירות נכלל בסכומי ההוצאות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-208">Is sales tax included in the expense amounts?</span></span>
- <span data-ttu-id="49f5f-209">האם החזר מס צריך להיות זמין בהוצאות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-209">Should tax recovery be enabled on expenses?</span></span>

    > [!NOTE]
    > <span data-ttu-id="49f5f-210">כאשר תכננת את ספר החשבונות הראשי, אם החלטת להחיל מס מכירות של ארה"ב ולהשתמש בכללי המס, אינך יכול להפוך את החזר המס על הוצאות לזמין.</span><span class="sxs-lookup"><span data-stu-id="49f5f-210">When you were planning the general ledger, if you decided to apply U.S. sales tax and use tax rules, you can’t enable tax recovery on expenses.</span></span> <span data-ttu-id="49f5f-211">(להחלת מס מכירות של ארה"ב ולשימוש בכללי המס, הגדר את האפשרות **החל כללי מיסוי של מס מכירות** ל **כן** ).</span><span class="sxs-lookup"><span data-stu-id="49f5f-211">(To apply U.S. sales tax and use tax rules, set the **Apply sales tax taxations rules** option to **Yes**.)</span></span>

## <a name="policies"></a><span data-ttu-id="49f5f-212">כללי מדיניות</span><span class="sxs-lookup"><span data-stu-id="49f5f-212">Policies</span></span>

<span data-ttu-id="49f5f-213">על ידי יצירת מדיניות של דוח הוצאות, אתה יכול לעזור לארגון שלך לחסוך זמן וכסף כאשר עובדים צוברים הוצאות מטעמו.</span><span class="sxs-lookup"><span data-stu-id="49f5f-213">By creating expense report policies, you can help your organization save time and money when employees incur expenses on its behalf.</span></span> <span data-ttu-id="49f5f-214">מדיניות מסייעת להבטיח שהעובדים יישארו במסגרת התקציב, יספקו את כל המידע הנדרש ויבזבזו כסף רק אם זה נדרש.</span><span class="sxs-lookup"><span data-stu-id="49f5f-214">Policies help guarantee that employees stay in budget, provide all required information, and spend money only as they require it.</span></span> <span data-ttu-id="49f5f-215">עליך לקבל את ההחלטות הבאות עבור כל מדיניות של דוח הוצאות ועבור כל מדיניות אישור של דוח הוצאות שאתה יוצר.</span><span class="sxs-lookup"><span data-stu-id="49f5f-215">You must make the following decisions for each expense report policy and each expense report approval policy that you create.</span></span>

<span data-ttu-id="49f5f-216">**החלטות:**</span><span class="sxs-lookup"><span data-stu-id="49f5f-216">**Decisions:**</span></span>

- <span data-ttu-id="49f5f-217">מה שם המדיניות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-217">What is the name of the policy?</span></span>
- <span data-ttu-id="49f5f-218">לשם מה נועדה מדיניות ההוצאות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-218">What is the expense policy for?</span></span>
- <span data-ttu-id="49f5f-219">אם החלטת בעבר להפוך הוצאות בין-חברתיות לזמינות, על אילו חברות בארגון שלך תחול מדיניות זו?</span><span class="sxs-lookup"><span data-stu-id="49f5f-219">If you previously decided to enable intercompany expenses, which companies in your organization will this policy apply to?</span></span>
- <span data-ttu-id="49f5f-220">מתי המדיניות נכנסת לתוקף?</span><span class="sxs-lookup"><span data-stu-id="49f5f-220">When does the policy become effective?</span></span>
- <span data-ttu-id="49f5f-221">מתי פג תוקף המדיניות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-221">When does the policy expire?</span></span>
- <span data-ttu-id="49f5f-222">מהו כלל המדיניות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-222">What is the policy rule?</span></span>
- <span data-ttu-id="49f5f-223">מה התוצאה של כלל המדיניות?</span><span class="sxs-lookup"><span data-stu-id="49f5f-223">What is the outcome of the policy rule?</span></span>
