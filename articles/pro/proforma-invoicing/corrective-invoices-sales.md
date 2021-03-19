---
title: חשבוניות שתוקנו - לייט
description: נושא זה מספק מידע על חשבוניות שתוקנו ב- Project Operations.
author: rumant
manager: Annbe
ms.date: 10/15/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: eb949ff3a53bcba19d44e1c3d6fe08a6b368108d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274234"
---
# <a name="corrected-invoices---lite"></a><span data-ttu-id="12de8-103">חשבוניות שתוקנו - לייט</span><span class="sxs-lookup"><span data-stu-id="12de8-103">Corrected invoices - lite</span></span>

<span data-ttu-id="12de8-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="12de8-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="12de8-105">ניתן לתקן חשבונית פרויקט שאושרה כדי לעבד שינויים או זיכויים בהתאם למשא ומתן עם הלקוח ועם מנהל הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="12de8-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="12de8-106">כדי לערוך חשבונית שאושרה, פתח את החשבונית שאושרה ובחר באפשרות **תקן חשבונית זו**.</span><span class="sxs-lookup"><span data-stu-id="12de8-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="12de8-107">בחירה זו אינה זמינה אם חשבונית הפרויקט לא אושרה.</span><span class="sxs-lookup"><span data-stu-id="12de8-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="12de8-108">תיווצר חשבונית טיוטה חדשה מהחשבונית שאושרה.</span><span class="sxs-lookup"><span data-stu-id="12de8-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="12de8-109">כל פרטי שורת החשבונית מהחשבונית שאושרה בעבר יועתקו לטיוטה החדשה.</span><span class="sxs-lookup"><span data-stu-id="12de8-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="12de8-110">להלן כמה מנקודות המפתח שיש להבין לגבי פרטי השורה בחשבונית המתוקנת החדשה:</span><span class="sxs-lookup"><span data-stu-id="12de8-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="12de8-111">כל הכמויות מתעדכנות לאפס.</span><span class="sxs-lookup"><span data-stu-id="12de8-111">All quantities are updated to zero.</span></span> <span data-ttu-id="12de8-112">היישום מניח שכל הפריטים שהוגשה עבורם חשבונית מזוכים במלואם.</span><span class="sxs-lookup"><span data-stu-id="12de8-112">The application assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="12de8-113">במידת הצורך, תוכל לעדכן כמויות אלה באופן ידני כדי לשקף את הכמות שמחויבת, ולא את הכמות שמזוכה.</span><span class="sxs-lookup"><span data-stu-id="12de8-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="12de8-114">בהתבסס על הכמות שתזין, היישום יחשב את הכמות שיש לזכות.</span><span class="sxs-lookup"><span data-stu-id="12de8-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="12de8-115">סכומים אלה באים לידי ביטוי בנתונים בפועל שנוצרים לאחר אישור החשבונית שתוקנה.</span><span class="sxs-lookup"><span data-stu-id="12de8-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="12de8-116">אם אתה מבצע שינויים בסכום המס, עליך להזין את סכום המס הנכון ולא את סכום המס לזיכוי.</span><span class="sxs-lookup"><span data-stu-id="12de8-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="12de8-117">סעיפי חוזה מבוססי-מוצר שאושרו בעבר אינם מועתקים.</span><span class="sxs-lookup"><span data-stu-id="12de8-117">Previously confirmed product-based contract lines are not copied over.</span></span> <span data-ttu-id="12de8-118">אין תמיכה בעיבוד תיקונים בחשבונית של פרויקט מבוסס-מוצר.</span><span class="sxs-lookup"><span data-stu-id="12de8-118">Processing corrections on a product-based project invoice is not supported.</span></span>
- <span data-ttu-id="12de8-119">תיקוני אבן דרך תמיד מעובדים כזיכויים מלאים.</span><span class="sxs-lookup"><span data-stu-id="12de8-119">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="12de8-120">ניתן לתקן סכומי ריטיינר או מקדמה אם הוגשה ללקוח חשבונית בסכום שגוי.</span><span class="sxs-lookup"><span data-stu-id="12de8-120">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="12de8-121">ניתן לתקן התאמות של ריטיינרים ושל מקדמות אם נעשה שימוש בסכום שגוי ליצירת התאמה כנגד החיובים בחשבונית שאושרה בעבר.</span><span class="sxs-lookup"><span data-stu-id="12de8-121">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="12de8-122">פרטי שורה בחשבונית שהם תיקונים של חיובים אחרים שכבר הוגשה עבורם חשבונית מכילים את השדה **תיקון** מוגדר בתור **כן**.</span><span class="sxs-lookup"><span data-stu-id="12de8-122">Invoice line details that are corrections to other already invoiced charges have the field **Correction** set to **Yes**.</span></span> <span data-ttu-id="12de8-123">חשבוניות שיש בהן פרטי שורה בחשבונית שתוקנו מכילות את השדה **כולל תיקונים** שגם הוא מוגדר בתור **כן**.</span><span class="sxs-lookup"><span data-stu-id="12de8-123">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-on-confirmation-of-a-corrective-invoice"></a><span data-ttu-id="12de8-124">אישור תאריך יצירה של נתונים בפועל של חשבונית תיקון:</span><span class="sxs-lookup"><span data-stu-id="12de8-124">Actuals created on Confirmation of a corrective invoice:</span></span>

<span data-ttu-id="12de8-125">להלן הנתונים בפועל שנוצרים על ידי היישום לאחר אישור של תיקון על סמך הפעולות שבוצעו בטיוטת חשבונית התיקון לפני האישור.</span><span class="sxs-lookup"><span data-stu-id="12de8-125">Below are the actuals created by the application on confirmation of a corrective based on the operations performed on the draft corrective invoice before confirmation.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="12de8-126">
                    <strong>תרחיש</strong>
                </span><span class="sxs-lookup"><span data-stu-id="12de8-126">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="12de8-127">
                    <strong>ניתונים בפועל שנוצרו באישור</strong>
                </span><span class="sxs-lookup"><span data-stu-id="12de8-127">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="12de8-128">אשר את התיקון של המקדמה או של הריטיינר שהוגשה עבורם חשבונית.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="12de8-128">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-129">ביטול עסקת מכירה שלא חויבה, של הריטיינר או המקדמה, שנוצר למטרות התאמה.</span><span class="sxs-lookup"><span data-stu-id="12de8-129">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="12de8-130">סכום זה חיובי מכיוון שהוא נועד לבטל את הסכום השלילי שנוצר בעת הגשת החשבונית של הריטיינר או המקדמה.</span><span class="sxs-lookup"><span data-stu-id="12de8-130">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-131">נוצר נתון בפועל של ביטול מכירות שחויבו בסכום של הריטיינר או המקדמה, כדי לבטל את המכירות בפועל שחויבו.</span><span class="sxs-lookup"><span data-stu-id="12de8-131">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-132">נוצר נתון בפועל חדש של מכירות שחויבו עבור הסכום המתוקן בשורת החשבונית המתוקנת המבוססת על ריטיינר או מקדמה.</span><span class="sxs-lookup"><span data-stu-id="12de8-132">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-133">נתון בפועל של מכירות שלא חויבו בסכום שלילי של שורת החשבונית המתוקנת המבוססת על ריטיינר או מקדמה, שישמש להתאמה.</span><span class="sxs-lookup"><span data-stu-id="12de8-133">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="12de8-134">אישור של התיקון של הריטיינר או המקדמה שהותאמו בעבר.</span><span class="sxs-lookup"><span data-stu-id="12de8-134">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-135">ביטול עסקת מכירה שלא חויבה, של הריטיינר או המקדמה, שנוצר למטרות התאמה.</span><span class="sxs-lookup"><span data-stu-id="12de8-135">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="12de8-136">סכום זה חיובי והוא נועד לבטל את הסכום השלילי שנוצר בעת שאירעה ההתאמה הקודמת.</span><span class="sxs-lookup"><span data-stu-id="12de8-136">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-137">נתון בפועל של ביטול מכירות שחויבו בסכום של החשבונית הקודמת.</span><span class="sxs-lookup"><span data-stu-id="12de8-137">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-138">נתון בפועל חדש של מכירות שחויבו עבור סכום הריטיינר המתוקן מוחל בחשבונית המתוקנת.</span><span class="sxs-lookup"><span data-stu-id="12de8-138">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-139">נתון בפועל של מכירות שלא חויבו בסכום שלילי מהריטיינר או המקדמה הנותרים שתוקנו, שישמש להתאמה בחשבוניות עתידיות.</span><span class="sxs-lookup"><span data-stu-id="12de8-139">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="12de8-140">הפקת חשבונית לזיכוי המלא של עסקה בזמן שהוגשה עבורה חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="12de8-140">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-141">ביטול מכירות שחויבו עבור השעות והסכום בפרט של שורת החשבונית המקורית לזמן.</span><span class="sxs-lookup"><span data-stu-id="12de8-141">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-142">נתון בפועל חדש של מכירות שלא חויבו עבור השעות והסכום בפרט של שורת החשבונית המקורית לזמן.</span><span class="sxs-lookup"><span data-stu-id="12de8-142">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="12de8-143">הפקת חשבונית לזיכוי החלקי של עסקה בזמן.</span><span class="sxs-lookup"><span data-stu-id="12de8-143">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-144">ביטול מכירות שחויבו עבור השעות והסכום שהוגשה עבורם חשבונית בפרט של שורת החשבונית המקורית לזמן.</span><span class="sxs-lookup"><span data-stu-id="12de8-144">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-145">‏‫נתון בפועל חדש של מכירות שלא חויבו שניתן לחייב אותו עבור השעות והסכום בפרט שורת החשבונית הערוכה, ביטול שלו ונתון שווה ערך בפועל של מכירות שחויבו.</span><span class="sxs-lookup"><span data-stu-id="12de8-145">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-146">נתון בפועל חדש של מכירות שלא חויבו שניתן לחייב אותו עבור השעות והסכום הנותרים לאחר ניכוי של הנתונים המתוקנים בפרט שורת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="12de8-146">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="12de8-147">הפקת חשבונית לזיכוי המלא של עסקת הוצאה שהוגשה עבורה חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="12de8-147">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-148">ביטול מכירות שחויבו עבור הכמות והסכום בפרט של שורת החשבונית המקורית עבור ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="12de8-148">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-149">‏‫נתון בפועל חדש של מכירות שלא חויבו עבור הכמות והסכום בפרט של שורת החשבונית המקורית עבור ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="12de8-149">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="12de8-150">הפקת חשבונית לזיכוי החלקי של עסקת הוצאה שהוגשה עבורה חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="12de8-150">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-151">ביטול מכירות שחויבו עבור הכמות והסכום שהוגשה עבורם חשבונית בפרט של שורת החשבונית המקורית עבור ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="12de8-151">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-152">‏‫נתון בפועל חדש של מכירות שלא חויבו שניתן לחייב אותו עבור הכמות והסכום בפרט שורת החשבונית המתוקנת, ביטול שלו ונתון שווה ערך בפועל של מכירות שחויבו.</span><span class="sxs-lookup"><span data-stu-id="12de8-152">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-153">נתון בפועל חדש של מכירות שלא חויבו שניתן לחייב אותו עבור הכמות והסכום הנותרים לאחר ניכוי של הנתונים המתוקנים בפרט שורת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="12de8-153">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="12de8-154">הפקת חשבונית לזיכוי המלא של עסקת תשלום שהוגשה עבורה חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="12de8-154">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-155">ביטול מכירות שחויבו עבור הכמות והסכום בפרט של שורת החשבונית המקורית עבור התשלום.</span><span class="sxs-lookup"><span data-stu-id="12de8-155">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-156">‏‫נתון בפועל חדש של מכירות שלא חויבו עבור הכמות והסכום בפרט של שורת החשבונית המקורית עבור התשלום.</span><span class="sxs-lookup"><span data-stu-id="12de8-156">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="12de8-157">הפקת חשבונית לזיכוי החלקי של עסקת תשלום שהוגשה עבורה חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="12de8-157">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-158">ביטול מכירות שחויבו עבור הכמות והסכום שהוגשה עבורם חשבונית בפרט של שורת החשבונית המקורית עבור התשלום.</span><span class="sxs-lookup"><span data-stu-id="12de8-158">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-159">‏‫נתון בפועל חדש של מכירות שלא חויבו שניתן לחייב אותו עבור הכמות והסכום בפרט שורת חשבונית התיקון הערוכה, ביטול שלו ונתון שווה ערך בפועל של מכירות שחויבו.</span><span class="sxs-lookup"><span data-stu-id="12de8-159">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="12de8-160">הפקת חשבונית לזיכוי המלא של אבן דרך שהוגשה עבורו חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="12de8-160">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-161">ביטול מכירות שחויבו עבור הסכום בפרט של שורת החשבונית המקורית לאבן הדרך.</span><span class="sxs-lookup"><span data-stu-id="12de8-161">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="12de8-162">חשבונית אבן הדרך או מצב החיוב בסעיף החוזה של הפרויקט מתעדכנים למצב **מוכן להגיש חשבונית**.</span><span class="sxs-lookup"><span data-stu-id="12de8-162">The milestone invoice or billing status on the project contract line is updated to **Ready to Invoice**.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="12de8-163">הפקת חשבונית לזיכוי החלקי של אבן דרך שהוגשה עבורו חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="12de8-163">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-164">לא נתמך</span><span class="sxs-lookup"><span data-stu-id="12de8-164">Unsupported</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="12de8-165">זיכויים ותיקונים של סעיף חוזה המבוסס על מוצר שהוגשה עבורו חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="12de8-165">Credits and corrections of a previously invoiced product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12de8-166">לא נתמך</span><span class="sxs-lookup"><span data-stu-id="12de8-166">Unsupported</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]