---
title: חשבוניות מתקנות מבוססות פרויקט
description: נושא זה מסביר כיצד ליצור ולאשר חשבוניות מתקנות מבוססות פרויקט ב-Project Operations.
author: rumant
ms.date: 03/29/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f6b6670f823577bf7f784443f97f0b77e1e9a6aa
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012272"
---
# <a name="corrective-project-based-invoices"></a><span data-ttu-id="dd7f0-103">חשבוניות מתקנות מבוססות פרויקט</span><span class="sxs-lookup"><span data-stu-id="dd7f0-103">Corrective project-based invoices</span></span>

<span data-ttu-id="dd7f0-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="dd7f0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="dd7f0-105">ניתן לתקן חשבונית פרויקט שאושרה כדי לעבד שינויים או זיכויים בהתאם למשא ומתן עם הלקוח ועם מנהל הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="dd7f0-106">כדי לערוך חשבונית שאושרה, פתח את החשבונית שאושרה ובחר באפשרות **תקן חשבונית זו**.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="dd7f0-107">אפשרות זו זמינה רק אם חשבונית הפרויקט אושרה או שבחשבונית מבוססת פרויקט יש מקדמות או ריטיינרים‬ או התאמות בין מקדמות או ריטיינרים‬.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-107">This selection isn't available unless a project invoice is confirmed or the project-based invoice has advances or retainers or reconciliations of advances or retainers.</span></span>

<span data-ttu-id="dd7f0-108">תיווצר חשבונית טיוטה חדשה מהחשבונית שאושרה.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="dd7f0-109">כל פרטי שורת החשבונית מהחשבונית שאושרה בעבר יועתקו לטיוטה החדשה.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="dd7f0-110">להלן כמה מנקודות המפתח שיש להבין לגבי פרטי השורה בחשבונית המתוקנת החדשה:</span><span class="sxs-lookup"><span data-stu-id="dd7f0-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="dd7f0-111">כל הכמויות מתעדכנות לאפס.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-111">All quantities are updated to zero.</span></span> <span data-ttu-id="dd7f0-112">Dynamics 365 Project Operations מניח שכל הפריטים המחויבים מזוכים במלואם.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-112">Dynamics 365 Project Operations assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="dd7f0-113">במידת הצורך, תוכל לעדכן כמויות אלה באופן ידני כדי לשקף את הכמות שמחויבת, ולא את הכמות שמזוכה.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="dd7f0-114">בהתבסס על הכמות שתזין, היישום יחשב את הכמות שיש לזכות.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="dd7f0-115">סכומים אלה באים לידי ביטוי בנתונים בפועל שנוצרים לאחר אישור החשבונית שתוקנה.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="dd7f0-116">אם אתה מבצע שינויים בסכום המס, עליך להזין את סכום המס הנכון ולא את סכום המס לזיכוי.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="dd7f0-117">תיקוני אבן דרך תמיד מעובדים כזיכויים מלאים.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-117">Milestone corrections are always processed as full credits.</span></span>


> [!IMPORTANT]
> <span data-ttu-id="dd7f0-118">עבור פרטי שורת החשבונית שהם תיקונים לחיובים אחרים שכבר בוצעו בחשבונית, השדה **תיקון** מוגדר בתור **כן**.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-118">For invoice line details that are corrections to other already invoiced charges, the **Correction** field is set to **Yes**.</span></span> <span data-ttu-id="dd7f0-119">עבור חשבוניות עם פרטים מתוקנים בשורת החשבונית, השדה **‏‫כולל תיקונים‬** מוגדר בתור **כן**.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-119">For invoices that have corrected invoice line details, the **Has corrections** field is set to **Yes**.</span></span>

## <a name="actuals-created-when-a-corrective-invoice-is-confirmed"></a><span data-ttu-id="dd7f0-120">נתונים בפועל שנוצרו בעת אישור החשבונית המתוקנת</span><span class="sxs-lookup"><span data-stu-id="dd7f0-120">Actuals created when a corrective invoice is confirmed</span></span>

<span data-ttu-id="dd7f0-121">הטבלה הבאה מפרטת את הנתונים בפועל שנוצרים לאחר אישור החשבונית המתקנת.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-121">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="dd7f0-122">
                    <strong>תרחיש</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dd7f0-122">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="dd7f0-123">
                    <strong>ניתונים בפועל שנוצרו באישור</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dd7f0-123">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dd7f0-124">הפקת חשבונית לזיכוי המלא של עסקה בזמן שהוגשה עבורה חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-124">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-125">ביטול מכירות שחויבו עבור השעות והסכום בפרט של שורת החשבונית המקורית לזמן.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-125">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-126">נתון בפועל חדש של מכירות שלא חויבו עבור השעות והסכום בפרט של שורת החשבונית המקורית לזמן.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-126">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="dd7f0-127">הפקת חשבונית לזיכוי החלקי של עסקה בזמן.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-127">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-128">ביטול מכירות שחויבו עבור השעות והסכום שהוגשה עבורם חשבונית בפרט של שורת החשבונית המקורית לזמן.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-128">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-129">‏‫נתון בפועל חדש של מכירות שלא חויבו שניתן לחייב אותו עבור השעות והסכום בפרט שורת החשבונית הערוכה, ביטול שלו ונתון שווה ערך בפועל של מכירות שחויבו.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-130">נתון בפועל חדש של מכירות שלא חויבו שניתן לחייב אותו עבור השעות והסכום הנותרים לאחר ניכוי של הנתונים המתוקנים בפרט שורת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-130">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dd7f0-131">הפקת חשבונית לזיכוי המלא של עסקת הוצאה שהוגשה עבורה חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-131">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-132">ביטול מכירות שחויבו עבור הכמות והסכום בפרט של שורת החשבונית המקורית עבור ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-132">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-133">‏‫נתון בפועל חדש של מכירות שלא חויבו עבור הכמות והסכום בפרט של שורת החשבונית המקורית עבור ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-133">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="dd7f0-134">הפקת חשבונית לזיכוי החלקי של עסקת הוצאה שהוגשה עבורה חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-134">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-135">ביטול מכירות שחויבו עבור הכמות והסכום שהוגשה עבורם חשבונית בפרט של שורת החשבונית המקורית עבור ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-135">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-136">‏‫נתון בפועל חדש של מכירות שלא חויבו שניתן לחייב אותו עבור הכמות והסכום בפרט שורת החשבונית המתוקנת, ביטול שלו ונתון שווה ערך בפועל של מכירות שחויבו.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-136">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-137">נתון בפועל חדש של מכירות שלא חויבו שניתן לחייב אותו עבור הכמות והסכום הנותרים לאחר ניכוי של הנתונים המתוקנים בפרט שורת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-137">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
                <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dd7f0-138">חשבונית זיכוי מלא על עסקת חומר שחויבה בעבר.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-138">Invoicing the full credit of a previously invoiced material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-139">‏‫ביטול עסקת מכירות שחויבה‬ על הכמות והסכום בפרטי שורת החשבונית המקורית עבור חומר.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-139">A billed sales reversal for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-140">‏‫נתונים בפועל חדשים למכירות שלא חויבו‬ על הכמות והסכום בפרטי שורת החשבונית המקורית עבור חומר.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-140">A new unbilled sales actual for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="dd7f0-141">הפקת חשבונית זיכוי חלקי על עסקת חומר.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-141">Invoicing the partial credit on a material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-142">‏‫ביטול עסקת מכירות שחויבה‬ על הכמות והסכום שחויבו בפרטי שורת החשבונית המקורית עבור חומר.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-142">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-143">נתונים בפועל חדשים למכירות שלא חויבו הניתנות לחיוב‬ על הכמות והסכום בפירוט שורת החשבונית הערוכה, ביטול של פעולה זו ונתונים בפועל למכירות שחויבו שווי ערך.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-143">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-144">נתון בפועל חדש של מכירות שלא חויבו שניתן לחייב אותו עבור הכמות והסכום הנותרים לאחר ניכוי של הנתונים המתוקנים בפרט שורת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-144">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dd7f0-145">הפקת חשבונית לזיכוי המלא של עסקת תשלום שהוגשה עבורה חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-145">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-146">ביטול מכירות שחויבו עבור הכמות והסכום בפרט של שורת החשבונית המקורית עבור התשלום.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-147">‏‫נתון בפועל חדש של מכירות שלא חויבו עבור הכמות והסכום בפרט של שורת החשבונית המקורית עבור התשלום.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dd7f0-148">הפקת חשבונית לזיכוי החלקי של עסקת תשלום שהוגשה עבורה חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-148">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-149">ביטול מכירות שחויבו עבור הכמות והסכום שהוגשה עבורם חשבונית בפרט של שורת החשבונית המקורית עבור התשלום.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-150">‏‫נתון בפועל חדש של מכירות שלא חויבו שניתן לחייב אותו עבור הכמות והסכום בפרט שורת חשבונית התיקון הערוכה, ביטול שלו ונתון שווה ערך בפועל של מכירות שחויבו.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-150">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="dd7f0-151">הפקת חשבונית לזיכוי המלא של אבן דרך שהוגשה עבורו חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-151">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-152">ביטול מכירות שחויבו עבור הסכום בפרט של שורת החשבונית המקורית לאבן הדרך.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-152">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="dd7f0-153">מצב החשבונית של אבן דרך מתעדכן מ: <b>חשבונית הלקוח פורסמה</b> ל: <b>מוכן להגיש חשבונית</b>.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-153">The invoice status of the milestone is updated from <b>Customer Invoice Posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="dd7f0-154">הפקת חשבונית לזיכוי החלקי של אבן דרך שהוגשה עבורו חשבונית בעבר.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-154">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="dd7f0-155">תרחיש זה אינו נתמך.</span><span class="sxs-lookup"><span data-stu-id="dd7f0-155">This scenario isn't supported.</span></span>
                </p>
            </td>
        </tr>       
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
