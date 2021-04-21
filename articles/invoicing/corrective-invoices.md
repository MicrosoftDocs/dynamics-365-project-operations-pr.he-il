---
title: יצירת חשבוניות מתקנות מבוססות פרויקט
description: נושא זה מספק מידע על חשבוניות מתקנות ב-Project Operations.
author: rumant
manager: Annbe
ms.date: 03/29/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 32772d64b3fc77f0af9618edff40e3b295593454
ms.sourcegitcommit: 504c09365bf404c1f1aa9b5034c1e1e5bc9d0d54
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/31/2021
ms.locfileid: "5788860"
---
# <a name="create-corrective-project-based-invoices"></a><span data-ttu-id="9ae18-103">יצירת חשבוניות מתקנות מבוססות פרויקט</span><span class="sxs-lookup"><span data-stu-id="9ae18-103">Create corrective project-based invoices</span></span> 

<span data-ttu-id="9ae18-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="9ae18-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="9ae18-105">ניתן לתקן חשבונית פרויקט שאושרה כדי לעבד שינויים או זיכויים בהתאם למשא ומתן עם הלקוח ועם מנהל הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="9ae18-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="9ae18-106">כדי לערוך חשבונית שאושרה, פתח את החשבונית שאושרה ובחר באפשרות **תקן חשבונית זו**.</span><span class="sxs-lookup"><span data-stu-id="9ae18-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="9ae18-107">בחירה זו אינה זמינה אם חשבונית הפרויקט לא אושרה.</span><span class="sxs-lookup"><span data-stu-id="9ae18-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="9ae18-108">תיווצר חשבונית טיוטה חדשה מהחשבונית שאושרה.</span><span class="sxs-lookup"><span data-stu-id="9ae18-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="9ae18-109">כל פרטי שורת החשבונית מהחשבונית שאושרה בעבר יועתקו לטיוטה החדשה.</span><span class="sxs-lookup"><span data-stu-id="9ae18-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="9ae18-110">להלן מספר נקודות מפתח שיעזרו לך להבין יותר את פרטי השורה בחשבונית המתוקנת החדשה:</span><span class="sxs-lookup"><span data-stu-id="9ae18-110">The following are some key points to help you understand more about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="9ae18-111">כל הכמויות מתעדכנות לאפס.</span><span class="sxs-lookup"><span data-stu-id="9ae18-111">All quantities are updated to zero.</span></span> <span data-ttu-id="9ae18-112">זה מניח שכל הפריטים המחויבים מזוכים במלואם.</span><span class="sxs-lookup"><span data-stu-id="9ae18-112">This assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="9ae18-113">במידת הצורך, תוכל לעדכן כמויות אלה באופן ידני כדי לשקף את הכמות שמחויבת, ולא את הכמות שמזוכה.</span><span class="sxs-lookup"><span data-stu-id="9ae18-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="9ae18-114">בהתבסס על הכמות שתזין, היישום יחשב את הכמות שיש לזכות.</span><span class="sxs-lookup"><span data-stu-id="9ae18-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="9ae18-115">סכומים אלה באים לידי ביטוי בנתונים בפועל שנוצרים לאחר אישור החשבונית שתוקנה.</span><span class="sxs-lookup"><span data-stu-id="9ae18-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="9ae18-116">אם אתה מבצע שינויים בסכום המס, עליך להזין את סכום המס הנכון ולא את סכום המס לזיכוי.</span><span class="sxs-lookup"><span data-stu-id="9ae18-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="9ae18-117">תיקוני אבן דרך תמיד מעובדים כזיכויים מלאים.</span><span class="sxs-lookup"><span data-stu-id="9ae18-117">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="9ae18-118">ניתן לתקן סכומי ריטיינר או מקדמה אם הוגשה ללקוח חשבונית בסכום שגוי.</span><span class="sxs-lookup"><span data-stu-id="9ae18-118">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="9ae18-119">ניתן לתקן התאמות של ריטיינרים ושל מקדמות אם נעשה שימוש בסכום שגוי ליצירת התאמה כנגד החיובים בחשבונית שאושרה בעבר.</span><span class="sxs-lookup"><span data-stu-id="9ae18-119">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9ae18-120">בפרטי שורת החשבונית שהם תיקונים לחיובים אחרים שכבר בוצעו בחשבונית, השדה **תיקון** מוגדר בתור **כן**.</span><span class="sxs-lookup"><span data-stu-id="9ae18-120">Invoice line details that are corrections to other already invoiced charges have the **Correction** field set to **Yes**.</span></span> <span data-ttu-id="9ae18-121">חשבוניות שיש בהן פרטי שורה בחשבונית שתוקנו מכילות את השדה **כולל תיקונים** שגם הוא מוגדר בתור **כן**.</span><span class="sxs-lookup"><span data-stu-id="9ae18-121">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-on-confirmation-of-a-corrective-invoice"></a><span data-ttu-id="9ae18-122">נתונים בפועל שנוצרו בעת אישור החשבונית המתוקנת</span><span class="sxs-lookup"><span data-stu-id="9ae18-122">Actuals created on confirmation of a corrective invoice</span></span>

<span data-ttu-id="9ae18-123">הטבלה הבאה מפרטת את הנתונים בפועל שנוצרים לאחר אישור החשבונית המתקנת.</span><span class="sxs-lookup"><span data-stu-id="9ae18-123">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="9ae18-124">
                    <strong>תרחיש</strong>
                </span><span class="sxs-lookup"><span data-stu-id="9ae18-124">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="9ae18-125">
                    <strong>ניתונים בפועל שנוצרו באישור</strong>
                </span><span class="sxs-lookup"><span data-stu-id="9ae18-125">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="9ae18-126">אשר את התיקון של המקדמה או של הריטיינר שהוגשה עבורם חשבונית.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="9ae18-126">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-127">ביטול עסקת מכירה שלא חויבה, של הריטיינר או המקדמה, שנוצר למטרות התאמה.</span><span class="sxs-lookup"><span data-stu-id="9ae18-127">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="9ae18-128">סכום זה חיובי מכיוון שהוא נועד לבטל את הסכום השלילי שנוצר בעת הגשת החשבונית של הריטיינר או המקדמה.</span><span class="sxs-lookup"><span data-stu-id="9ae18-128">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-129">נוצר נתון בפועל של ביטול מכירות שחויבו בסכום של הריטיינר או המקדמה, כדי לבטל את המכירות בפועל שחויבו.</span><span class="sxs-lookup"><span data-stu-id="9ae18-129">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-130">נוצר נתון בפועל חדש של מכירות שחויבו עבור הסכום המתוקן בשורת החשבונית המתוקנת המבוססת על ריטיינר או מקדמה.</span><span class="sxs-lookup"><span data-stu-id="9ae18-130">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-131">נתון בפועל של מכירות שלא חויבו בסכום שלילי של שורת החשבונית המתוקנת המבוססת על ריטיינר או מקדמה, שישמש להתאמה.</span><span class="sxs-lookup"><span data-stu-id="9ae18-131">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="9ae18-132">אישור של התיקון של הריטיינר או המקדמה שהותאמו בעבר.</span><span class="sxs-lookup"><span data-stu-id="9ae18-132">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-133">ביטול עסקת מכירה שלא חויבה, של הריטיינר או המקדמה, שנוצר למטרות התאמה.</span><span class="sxs-lookup"><span data-stu-id="9ae18-133">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="9ae18-134">סכום זה חיובי והוא נועד לבטל את הסכום השלילי שנוצר בעת שאירעה ההתאמה הקודמת.</span><span class="sxs-lookup"><span data-stu-id="9ae18-134">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-135">נתון בפועל של ביטול מכירות שחויבו בסכום של החשבונית הקודמת.</span><span class="sxs-lookup"><span data-stu-id="9ae18-135">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-136">נתון בפועל חדש של מכירות שחויבו עבור סכום הריטיינר המתוקן מוחל בחשבונית המתוקנת.</span><span class="sxs-lookup"><span data-stu-id="9ae18-136">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-137">נתון בפועל של מכירות שלא חויבו בסכום שלילי מהריטיינר או המקדמה הנותרים שתוקנו, שישמש להתאמה בחשבוניות עתידיות.</span><span class="sxs-lookup"><span data-stu-id="9ae18-137">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="9ae18-138">הפקת חשבונית לזיכוי המלא של עסקה בזמן שהוגשה עבורה חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="9ae18-138">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-139">ביטול מכירות שחויבו עבור השעות והסכום בפרט של שורת החשבונית המקורית לזמן.</span><span class="sxs-lookup"><span data-stu-id="9ae18-139">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-140">נתון בפועל חדש של מכירות שלא חויבו עבור השעות והסכום בפרט של שורת החשבונית המקורית לזמן.</span><span class="sxs-lookup"><span data-stu-id="9ae18-140">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="9ae18-141">הפקת חשבונית לזיכוי החלקי של עסקה בזמן.</span><span class="sxs-lookup"><span data-stu-id="9ae18-141">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-142">ביטול מכירות שחויבו עבור השעות והסכום שהוגשה עבורם חשבונית בפרט של שורת החשבונית המקורית לזמן.</span><span class="sxs-lookup"><span data-stu-id="9ae18-142">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-143">‏‫נתון בפועל חדש של מכירות שלא חויבו שניתן לחייב אותו עבור השעות והסכום בפרט שורת החשבונית הערוכה, ביטול שלו ונתון שווה ערך בפועל של מכירות שחויבו.</span><span class="sxs-lookup"><span data-stu-id="9ae18-143">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-144">נתון בפועל חדש של מכירות שלא חויבו שניתן לחייב אותו עבור השעות והסכום הנותרים לאחר ניכוי של הנתונים המתוקנים בפרט שורת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="9ae18-144">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="9ae18-145">הפקת חשבונית לזיכוי המלא של עסקת הוצאה שהוגשה עבורה חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="9ae18-145">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-146">ביטול מכירות שחויבו עבור הכמות והסכום בפרט של שורת החשבונית המקורית עבור ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="9ae18-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-147">‏‫נתון בפועל חדש של מכירות שלא חויבו עבור הכמות והסכום בפרט של שורת החשבונית המקורית עבור ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="9ae18-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="9ae18-148">הפקת חשבונית לזיכוי החלקי של עסקת הוצאה שהוגשה עבורה חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="9ae18-148">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-149">ביטול מכירות שחויבו עבור הכמות והסכום שהוגשה עבורם חשבונית בפרט של שורת החשבונית המקורית עבור ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="9ae18-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-150">‏‫נתון בפועל חדש של מכירות שלא חויבו שניתן לחייב אותו עבור הכמות והסכום בפרט שורת החשבונית המתוקנת, ביטול שלו ונתון שווה ערך בפועל של מכירות שחויבו.</span><span class="sxs-lookup"><span data-stu-id="9ae18-150">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-151">נתון בפועל חדש של מכירות שלא חויבו שניתן לחייב אותו עבור הכמות והסכום הנותרים לאחר ניכוי של הנתונים המתוקנים בפרט שורת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="9ae18-151">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="9ae18-152">הפקת חשבונית לזיכוי המלא של עסקת תשלום שהוגשה עבורה חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="9ae18-152">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-153">ביטול מכירות שחויבו עבור הכמות והסכום בפרט של שורת החשבונית המקורית עבור התשלום.</span><span class="sxs-lookup"><span data-stu-id="9ae18-153">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-154">‏‫נתון בפועל חדש של מכירות שלא חויבו עבור הכמות והסכום בפרט של שורת החשבונית המקורית עבור התשלום.</span><span class="sxs-lookup"><span data-stu-id="9ae18-154">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="9ae18-155">הפקת חשבונית לזיכוי החלקי של עסקת תשלום שהוגשה עבורה חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="9ae18-155">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-156">ביטול מכירות שחויבו עבור הכמות והסכום שהוגשה עבורם חשבונית בפרט של שורת החשבונית המקורית עבור התשלום.</span><span class="sxs-lookup"><span data-stu-id="9ae18-156">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-157">‏‫נתון בפועל חדש של מכירות שלא חויבו שניתן לחייב אותו עבור הכמות והסכום בפרט שורת חשבונית התיקון הערוכה, ביטול שלו ונתון שווה ערך בפועל של מכירות שחויבו.</span><span class="sxs-lookup"><span data-stu-id="9ae18-157">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="9ae18-158">הפקת חשבונית לזיכוי המלא של אבן דרך שהוגשה עבורו חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="9ae18-158">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-159">ביטול מכירות שחויבו עבור הסכום בפרט של שורת החשבונית המקורית לאבן הדרך.</span><span class="sxs-lookup"><span data-stu-id="9ae18-159">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="9ae18-160">מצב החשבונית באבן דרך מתעדכן מ: <b>חשבונית הלקוח פורסמה</b> ל: <b>מוכן להגיש חשבונית</b>.</span><span class="sxs-lookup"><span data-stu-id="9ae18-160">The invoice status on the milestone is updated from <b>Customer invoice posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="9ae18-161">הפקת חשבונית לזיכוי החלקי של אבן דרך שהוגשה עבורו חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="9ae18-161">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="9ae18-162">לא נתמך</span><span class="sxs-lookup"><span data-stu-id="9ae18-162">Unsupported</span></span> </p>
            </td>
        </tr>        
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
