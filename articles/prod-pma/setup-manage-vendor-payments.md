---
title: הגדרה ושימוש בתשלומי ספק מסוג גב-אל-גב
description: נושא זה מסביר כיצד ליצור תנאי תשלום גב-אל-גב (PWP) כדי שתוכל לשחרר תשלומים חלקיים לספק, המבוססים על תשלומי לקוחות.
author: RadhikaRS
manager: AnnBe
ms.date: 03/30/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: e872c4a2d35cef4cddc6851615c6c4d73b4e9d9a
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077287"
---
# <a name="set-up-and-use-pay-when-paid-vendor-payments"></a><span data-ttu-id="c1726-103">הגדרה ושימוש בתשלומי ספק מסוג גב-אל-גב</span><span class="sxs-lookup"><span data-stu-id="c1726-103">Set up and use pay-when-paid vendor payments</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="c1726-104">כאשר אתה מאשר לספק לעבוד כקבלן משנה, ייתכן שתרצה לעכב את התשלום לספק עד שהלקוח ישלם לך עבור הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="c1726-104">When you approve a vendor to work as a subcontractor, you might want to withhold payment to the vendor until your customer pays you for the project.</span></span> <span data-ttu-id="c1726-105">כדי לתמוך בתרחיש זה, אתה יכול להגדיר תנאי תשלום גב-אל-גב (PWP) בעת הגדרת הזמנת הרכש (PO) מול הספק.</span><span class="sxs-lookup"><span data-stu-id="c1726-105">To support this scenario, you can set up pay-when-paid (PWP) terms when you set up the purchase order (PO) with the vendor.</span></span>

<span data-ttu-id="c1726-106">לדוגמה, כאשר לקוח משלם סכום בחשבונית פרויקט, אתה יכול לשחרר חלק מסכום חשבונית הספק או את כולו.</span><span class="sxs-lookup"><span data-stu-id="c1726-106">For example, when a customer pays an amount on a project invoice, you can release some or all of the vendor invoice amount.</span></span> <span data-ttu-id="c1726-107">פשוט הגדר תנאי גב-אל-גב המציינים כי תשלם לספק לאחר שתקבל מהלקוח אחוז מהתשלום הקשור.</span><span class="sxs-lookup"><span data-stu-id="c1726-107">Just set up PWP terms that specify that the vendor will be paid after you receive a percentage of the related payment from the customer.</span></span> <span data-ttu-id="c1726-108">אם אתה מקבל תשלום חלקי מלקוח, אתה יכול לשחרר ידנית חלק מחשבוניות הספק הקשורות לתשלום.</span><span class="sxs-lookup"><span data-stu-id="c1726-108">If you receive partial payment from a customer, you can manually release some of the related vendor invoices for payment.</span></span>

<span data-ttu-id="c1726-109">הדוגמה הבאה מתארת את התהליך כאשר משתמשים בתנאי גב-אל-גב.</span><span class="sxs-lookup"><span data-stu-id="c1726-109">The following example outlines the process when PWP terms are used.</span></span>

## <a name="example"></a><span data-ttu-id="c1726-110">דוגמה</span><span class="sxs-lookup"><span data-stu-id="c1726-110">Example</span></span>

<span data-ttu-id="c1726-111">הארגון שלך מסכים לספק ללקוח 100 מחשבים שמותקנת בהם תוכנה, במחיר של 150.00 דולר אמריקני (USD) למחשב.</span><span class="sxs-lookup"><span data-stu-id="c1726-111">Your organization agrees to provide a customer with 100 computers that have software installed, for a price of 150.00 US dollars (USD) per computer.</span></span> <span data-ttu-id="c1726-112">לאחר מכן אתה שוכר ספק שיספק לך את המחשבים שמותקנת בהם תוכנה.</span><span class="sxs-lookup"><span data-stu-id="c1726-112">You then hire a vendor to provide you with the computers that have software installed.</span></span> <span data-ttu-id="c1726-113">על פי ההסכם, הלקוח חייב לאשר את איכות המחשבים לפני שהוא משלם לארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="c1726-113">According to the agreement, the customer must approve the quality of the computers before it pays your organization.</span></span> <span data-ttu-id="c1726-114">המדיניות של הארגון שלך היא לעכב תשלום לספקים עד שהלקוח משלם לך.</span><span class="sxs-lookup"><span data-stu-id="c1726-114">Your organization's policy is to withhold payment to vendors until the customer has paid you.</span></span> <span data-ttu-id="c1726-115">לכן, אתה מגדיר את הפרויקט כך שיהיה לו 100 אחוז גב-אל-גב.</span><span class="sxs-lookup"><span data-stu-id="c1726-115">Therefore, you set up the project so that it has a PWP percentage of 100 percent.</span></span>

<span data-ttu-id="c1726-116">הספק שולח לך את 100 המחשבים שמותקנת בהם תוכנה, יחד עם חשבונית על סך 10,000.00 USD.</span><span class="sxs-lookup"><span data-stu-id="c1726-116">The vendor sends you the 100 computers that have software installed, together with an invoice for 10,000.00 USD.</span></span> <span data-ttu-id="c1726-117">מכיוון שמוגדרים תנאי גב-אל-גב בפרויקט, אינך משלם לספק עם קבלת המחשבים.</span><span class="sxs-lookup"><span data-stu-id="c1726-117">Because PWP terms are set up for your project, you don't pay the vendor upon receipt of the computers.</span></span> <span data-ttu-id="c1726-118">במקום, אתה שולח את המחשבים ללקוח, יחד עם חשבונית על סך 15,000.00.</span><span class="sxs-lookup"><span data-stu-id="c1726-118">Instead, you send the computers to the customer, together with an invoice for 15,000.00.</span></span> <span data-ttu-id="c1726-119">הלקוח בודק את המחשבים ומאשר את הסכום המלא של חשבונית הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="c1726-119">The customer inspects the computers and approves the full amount of the project invoice.</span></span>

<span data-ttu-id="c1726-120">לאחר קבלת התשלום המלא מהלקוח, אתה משלם לספק 10,000.00, הסכום המלא של חשבונית הספק.</span><span class="sxs-lookup"><span data-stu-id="c1726-120">After you receive the full payment from the customer, you pay the vendor 10,000.00, the full amount of the vendor invoice.</span></span>

## <a name="set-up-pwp-terms-for-a-project"></a><span data-ttu-id="c1726-121">הגדרת תנאי גב-אל-גב לפרויקט</span><span class="sxs-lookup"><span data-stu-id="c1726-121">Set up PWP terms for a project</span></span>

<span data-ttu-id="c1726-122">כאשר אתה מגדיר תנאי גב-אל-גב לפרויקט, עליך לציין באחוזים את הסכום המינימלי שעל הלקוח לשלם לך עבור הפרויקט לפני התשלום לספק.</span><span class="sxs-lookup"><span data-stu-id="c1726-122">When you set up PWP terms for a project, you must specify, as a percentage, the minimum amount that a customer must pay you for the project before you will pay the vendor.</span></span> <span data-ttu-id="c1726-123">סכום הסף מחושב באופן אוטומטי בחשבוניות הלקוח לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="c1726-123">The threshold amount is automatically calculated on the customer invoices for the project.</span></span> <span data-ttu-id="c1726-124">בצע את השלבים הבאים להגדרת אחוז הסף עבור תנאי גב-אל-גב.</span><span class="sxs-lookup"><span data-stu-id="c1726-124">Follow these steps to set up the threshold percentage for PWP terms.</span></span>

1. <span data-ttu-id="c1726-125">עבור אל **ניהול פרויקטים וחשבונאות** \> **פרויקטים** \> **כל הפרויקטים**.</span><span class="sxs-lookup"><span data-stu-id="c1726-125">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="c1726-126">חפש ופתח את הפרויקט שעבורו אתה רוצה להגדיר תנאי גב-אל-גב.</span><span class="sxs-lookup"><span data-stu-id="c1726-126">Find and open the project that you want to set up PWP terms for.</span></span>
3. <span data-ttu-id="c1726-127">ב- FastTab **הסכמי ספק** , בחר באפשרות **הוסף שורה**.</span><span class="sxs-lookup"><span data-stu-id="c1726-127">On the **Vendor agreements** FastTab, select **Add line**.</span></span>
3. <span data-ttu-id="c1726-128">בשדה **‏‫קוד תיק לקוח‬** , בחר אחת מהאפשרויות הבאות:</span><span class="sxs-lookup"><span data-stu-id="c1726-128">In the **Account code** field, select one of the following options:</span></span>

    - <span data-ttu-id="c1726-129">**טבלה** – תנאי הגב-אל-גב חלים על ספק יחיד.</span><span class="sxs-lookup"><span data-stu-id="c1726-129">**Table** – The PWP terms apply to a single vendor.</span></span>
    - <span data-ttu-id="c1726-130">**קבוצה** – תנאי הגב-אל-גב חלים על כל הספקים בקבוצת ספקים.</span><span class="sxs-lookup"><span data-stu-id="c1726-130">**Group** – The PWP terms apply to all vendors in a vendor group.</span></span>
    - <span data-ttu-id="c1726-131">**כולם** – תנאי הגב-אל-גב חלים על כל הספקים.</span><span class="sxs-lookup"><span data-stu-id="c1726-131">**All** – The PWP terms apply to all vendors.</span></span>

4. <span data-ttu-id="c1726-132">אם בחרת **טבלה** או **קבוצה** בשלב הקודם, בשדה **ספק / קבוצת ספקים** , בחר את הספק או את קבוצת הספקים שתנאי הגב-אל-גב חלים עליהם.</span><span class="sxs-lookup"><span data-stu-id="c1726-132">If you selected **Table** or **Group** in the previous step, in the **Vendor/Vendor group** field, select the vendor or vendor group that the PWP terms apply to.</span></span> <span data-ttu-id="c1726-133">אם בחרת **כולם** בשלב הקודם, לא ניתן לערוך את השדה **ספק / קבוצת ספקים**.</span><span class="sxs-lookup"><span data-stu-id="c1726-133">If you selected **All** in the previous step, the **Vendor/Vendor group** field can't be edited.</span></span>
5. <span data-ttu-id="c1726-134">אם מוגדרים תנאי שמירה של ספק עבור הספק בפרויקט, בשדה **תנאי שמירה של ספק** , בחר את מזהה הכלל לתנאי השמירה.</span><span class="sxs-lookup"><span data-stu-id="c1726-134">If vendor retention terms are set up for the vendor in the project, in the **Vendor retention terms** field, select the rule ID for the retention terms.</span></span>
6. <span data-ttu-id="c1726-135">בשדה **אחוז הסף של גב-אל-גב** , הזן את אחוז הסף עבור הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="c1726-135">In the **PWP threshold percentage** field, enter the threshold percentage for the project.</span></span> <span data-ttu-id="c1726-136">האחוז שהזנת לפרויקט מגדיר את הסכום המינימלי שעל הלקוח לשלם לך לפני שתשלם לספק.</span><span class="sxs-lookup"><span data-stu-id="c1726-136">The percentage that you enter for the project defines the minimum amount that the customer must pay you before you will pay the vendor.</span></span>

## <a name="create-a-po-that-has-pwp-terms"></a><span data-ttu-id="c1726-137">יצירת הזמנת רכש עם תנאי גב-אל-גב</span><span class="sxs-lookup"><span data-stu-id="c1726-137">Create a PO that has PWP terms</span></span>

<span data-ttu-id="c1726-138">כאשר אתה מפרסם חשבונית מספק, אם הספק כפוף לתנאי גב-אל-גב, תנאים אלה מוצגים בשורות הזמנת הרכש.</span><span class="sxs-lookup"><span data-stu-id="c1726-138">When you post an invoice from a vendor, if the vendor is subject to PWP terms, those terms are shown on the PO lines.</span></span> <span data-ttu-id="c1726-139">כדי ליצור הזמנת רכש עם תנאי גב-אל-גב, בצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="c1726-139">To create a PO that has PWP terms, follow these steps.</span></span>

1. <span data-ttu-id="c1726-140">עבור אל **רכש ומיקור** \> **הזמנות רכש** \> **כל הזמנות הרכש**.</span><span class="sxs-lookup"><span data-stu-id="c1726-140">Go to **Procurement and sourcing** \> **Purchase orders** \> **All purchase orders**.</span></span>
2. <span data-ttu-id="c1726-141">בחלונית הפעולות בחר באפשרות **חדש**.</span><span class="sxs-lookup"><span data-stu-id="c1726-141">On the Action Pane, select **New**.</span></span> <span data-ttu-id="c1726-142">לאחר מכן, בתיבת הדו-שיח **צור הזמנת רכש** , הזן את המידע הדרוש ובחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="c1726-142">Then, in the **Create purchase order** dialog box, enter the required information, and select **OK**.</span></span>

    <span data-ttu-id="c1726-143">לחלופין, פתח הזמנת רכש קיימת בדף הרשימה **כל הזמנות הרכש**.</span><span class="sxs-lookup"><span data-stu-id="c1726-143">Alternatively, open an existing PO on the **All purchase orders** list page.</span></span>

4. <span data-ttu-id="c1726-144">בדף **הזמנת רכש** , ב- FastTab **שורות הזמנת רכש** , עיין בפרטי שורת הזמנת הרכש עבור הספק.</span><span class="sxs-lookup"><span data-stu-id="c1726-144">On the **Purchase order** page, on the **Purchase order lines** FastTab, review the details of the PO line for the vendor.</span></span> <span data-ttu-id="c1726-145">האפשרות **גב-אל-גב** נבחרת באופן אוטומטי, והערך בשדה **אחוז הסף של גב-אל-גב** מועתק אוטומטית מהשדה **אחוז הסף של גב-אל-גב** אל הדף **פרויקטים**.</span><span class="sxs-lookup"><span data-stu-id="c1726-145">The **Pay when paid** option is automatically selected, and the value in the **PWP threshold percentage** field is automatically copied from the **PWP threshold percentage** field on the **Projects** page.</span></span>
6. <span data-ttu-id="c1726-146">אם אינך רוצה להחיל תנאי גב-אל-גב על הספק עבור שורת הזמנת הרכש, נקה את הסימון של האפשרות **גב-אל-גב**.</span><span class="sxs-lookup"><span data-stu-id="c1726-146">If you don't want to apply PWP terms to the vendor for a PO line, clear the **Pay when paid** option.</span></span> <span data-ttu-id="c1726-147">במקרה זה, השדה **אחוז הסף של גב-אל-גב** עבור שורת הזמנת הרכש יאופס ל- 0 (אפס).</span><span class="sxs-lookup"><span data-stu-id="c1726-147">In this case, the **PWP threshold percentage** field for the PO line will be reset to 0 (zero).</span></span>

## <a name="update-a-customer-payment-and-pay-the-vendor"></a><span data-ttu-id="c1726-148">עדכון תשלום של לקוח ומתן תשלום לספק</span><span class="sxs-lookup"><span data-stu-id="c1726-148">Update a customer payment and pay the vendor</span></span>

<span data-ttu-id="c1726-149">כאשר ספק משלים את עבודתו בפרויקט ושולח אליך חשבונית, עליך לבדוק את מצב הפרויקט ואת חשבוניות הלקוח כדי לקבוע אם מולאו הקריטריונים של תנאי הגב-אל-גב לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="c1726-149">When a vendor completes its work on a project and sends you an invoice, you must review the project status and customer invoices to determine whether the PWP terms have been met for the project.</span></span> <span data-ttu-id="c1726-150">אם הם מולאו עבור הספק, תוכל לקבוע אילו שורות יש לשלם בחשבונית הספק, בהתבסס על תשלומי הלקוח עבור הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="c1726-150">If the PWP terms for the vendor were met, you can determine which lines on the vendor invoice to pay, based on the customer payments for the project.</span></span> <span data-ttu-id="c1726-151">אם תחליט לשלם לספק למרות שהקריטריונים של תנאי הגב-אל-גב לא מולאו, תוכל לעקוף את תנאי הגב-אל-גב בדף **חשבונית ספק עם גב-אל-גב**.</span><span class="sxs-lookup"><span data-stu-id="c1726-151">If you decide to pay the vendor even though the PWP terms weren't met, you can override the PWP terms on the **Vendor invoice with pay when paid** page.</span></span>

1. <span data-ttu-id="c1726-152">עבור אל **ניהול פרויקטים וחשבונאות** \> **בירורים ודוחות** \> **בירורים בנוגע לשמירה** \> **חשבונית ספק עם גב-אל-גב**.</span><span class="sxs-lookup"><span data-stu-id="c1726-152">Go to **Project management and accounting** \> **Inquiries and reports** \> **Retention inquiries** \> **Vendor invoice with pay when paid**.</span></span>
2. <span data-ttu-id="c1726-153">בדף **חשבוניות ספק עם גב-אל-גב** , בשדה החיפוש, הזן ערכים כדי למצוא את חשבונית הספק שברצונך לבדוק, ואז בחר **חפש**.</span><span class="sxs-lookup"><span data-stu-id="c1726-153">On the **Vendor invoices with pay when paid** page, in the search field, enter values to find the vendor invoice that you want to review, and then select **Search**.</span></span>
3. <span data-ttu-id="c1726-154">ב- FastTab **שורות חשבונית ספק** , בחר את השורות שאתה רוצה לשנות.</span><span class="sxs-lookup"><span data-stu-id="c1726-154">On the **Vendor invoice lines** FastTab, select the lines that you want to change.</span></span>
4. <span data-ttu-id="c1726-155">אם התנאים של **גב-אל-גב** התקיימו עבור שורת החשבונית, בחר **שחרר את תשלום הספק**.</span><span class="sxs-lookup"><span data-stu-id="c1726-155">If the **Pay when paid** conditions are met for the invoice line, select **Release vendor payment**.</span></span> <span data-ttu-id="c1726-156">האפשרות **גב-אל-גב** תנוקה, והערך של השדה **מוכן לתשלום** ישתנה ל **כן**.</span><span class="sxs-lookup"><span data-stu-id="c1726-156">The **Pay when paid** option is cleared, and the value of the **Ready for payment** field is changed to **Yes**.</span></span>
