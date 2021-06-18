---
title: אישור חשבונית פרופורמה מבוססת פרויקט
description: נושא זה מספק מידע על אישור חשבוניות פרופורמה‬ מבוססת פרויקט.
author: rumant
ms.date: 04/05/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 1e4591d97e9d895dade42b2bcce57f22208cba96
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012137"
---
# <a name="confirm-a-proforma-project-based-invoice"></a><span data-ttu-id="74bd9-103">אישור חשבונית פרופורמה מבוססת פרויקט</span><span class="sxs-lookup"><span data-stu-id="74bd9-103">Confirm a proforma project-based invoice</span></span>

<span data-ttu-id="74bd9-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="74bd9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="74bd9-105">לאחר אישור חשבונית פרופורמה, מצב חשבונית הפרויקט מתעדכן ל **מאושר**.</span><span class="sxs-lookup"><span data-stu-id="74bd9-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="74bd9-106">לאחר אישור חשבונית, היא תוגדר 'לקריאה בלבד'.</span><span class="sxs-lookup"><span data-stu-id="74bd9-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="74bd9-107">בהמשך, ניתן לתקן את החשבונית רק אם ישנם תיקונים או זיכויים ביוזמת הלקוח.</span><span class="sxs-lookup"><span data-stu-id="74bd9-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits.</span></span>

<span data-ttu-id="74bd9-108">הטבלה הבאה מפרטת את ניתונים בפועל שנוצרו על ידי המערכת.</span><span class="sxs-lookup"><span data-stu-id="74bd9-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="74bd9-109">ניתונים בפועל אלו נוצרים כאשר פעולות מסוימות מבוצעות בטיוטת חשבונית הפרויקט לפני אישורה.</span><span class="sxs-lookup"><span data-stu-id="74bd9-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="74bd9-110">
                    <strong>תרחיש</strong>
                </span><span class="sxs-lookup"><span data-stu-id="74bd9-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="74bd9-111">
                    <strong>ניתונים בפועל שנוצרו באישור</strong>
                </span><span class="sxs-lookup"><span data-stu-id="74bd9-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74bd9-112">הפקת חשבונית עבור מקדמה או ריטיינר</span><span class="sxs-lookup"><span data-stu-id="74bd9-112">Invoicing an advance or retainer</span></span> </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-113">חיוב של נתונים בפועל של מכירות מסוג <strong>ריטיינר</strong> נוצר עבור הסכום של המקדמה או הריטיינר.</span><span class="sxs-lookup"><span data-stu-id="74bd9-113">A billed sales actual of type, <strong>Retainer</strong> is created for the amount on the advance or retainer.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-114">‏‫נתונים בפועל למכירות שלא חויבו עם סכום שלילי של הריטיינר או המקדמה שישמשו להתאמה.</span><span class="sxs-lookup"><span data-stu-id="74bd9-114">An unbilled sales actual with a negative amount of the retainer or advance to be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74bd9-115">לאחר תיאום מלא של ריטיינר או מקדמה על חשבונית.</span><span class="sxs-lookup"><span data-stu-id="74bd9-115">After fully reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-116">ביטול עסקת מכירה שלא חויבה, של הריטיינר או המקדמה, שנוצר למטרות התאמה.</span><span class="sxs-lookup"><span data-stu-id="74bd9-116">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="74bd9-117">סכום זה הוא סכום חיובי מכיוון שהוא נועד לבטל את הסכום השלילי שנוצר בעת הגשת החשבונית עובר הריטיינר או המקדמה.</span><span class="sxs-lookup"><span data-stu-id="74bd9-117">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-118">נתון מכירה בפועל שחויב, בסכום הרשום בחשבונית זו.</span><span class="sxs-lookup"><span data-stu-id="74bd9-118">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="74bd9-119">לאחר תיאום חלקי של ריטיינר או מקדמה בחשבונית.</span><span class="sxs-lookup"><span data-stu-id="74bd9-119">After partially reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-120">ביטול עסקת מכירה שלא חויבה, של הריטיינר או המקדמה, שנוצר למטרות התאמה.</span><span class="sxs-lookup"><span data-stu-id="74bd9-120">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="74bd9-121">סכום זה הוא סכום חיובי מכיוון שהוא נועד לבטל את הסכום השלילי שנוצר בעת הגשת החשבונית עובר הריטיינר או המקדמה.</span><span class="sxs-lookup"><span data-stu-id="74bd9-121">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-122">נתון מכירה בפועל שחויב, בסכום הרשום בחשבונית זו.</span><span class="sxs-lookup"><span data-stu-id="74bd9-122">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-123">נתון בפועל שלילי של מכירות, שלא חויב עבור סכום הריטיינר או המקדמה שנותר, שישמש להתאמה בחשבוניות עתידיות.</span><span class="sxs-lookup"><span data-stu-id="74bd9-123">A negative unbilled sales actual of the remaining retainer or advance amount to be used for reconciliation on future invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74bd9-124">הפקת חשבונית עובר עסקת זמן ללא כל עריכות בטיוטת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="74bd9-124">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-125">ביטול עסקת מכירה שחויבה עבור השעות והסכום שבאישור הזמן המקורי.</span><span class="sxs-lookup"><span data-stu-id="74bd9-125">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-126">נתוני מכירות בפועל שחוייבו עבור השעות והסכום שבאישור הזמן המקורי.</span><span class="sxs-lookup"><span data-stu-id="74bd9-126">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="74bd9-127">הפקת חשבונית על עסקת זמן שנערכה כדי להפחית את הכמות.</span><span class="sxs-lookup"><span data-stu-id="74bd9-127">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-128">ביטול עסקת מכירה שחויבה עבור השעות והסכום שבאישור הזמן המקורי.</span><span class="sxs-lookup"><span data-stu-id="74bd9-128">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-129">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור השעות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של מכירות ונתון בפועל שווה ערך, של מכירה, שחויב.</span><span class="sxs-lookup"><span data-stu-id="74bd9-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-130">נתונים בפועל חדשים למכירות שלא חויבו ושאינן ניתנות לחיוב עבור השעות והסכום הנותרים לאחר ניכוי הנתונים המתוקנים בפירוט שורת החשבונית הערוכה, ביטול נתוני המכירות בפועל ו‏‫נתונים בפועל למכירות שחויבו שווי ערך.</span><span class="sxs-lookup"><span data-stu-id="74bd9-130">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74bd9-131">הפקת חשבונית על עסקת זמן שנערכה כדי להגדיל את הכמות.</span><span class="sxs-lookup"><span data-stu-id="74bd9-131">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-132">ביטול עסקת מכירה שחויבה עבור השעות והסכום שבאישור הזמן המקורי.</span><span class="sxs-lookup"><span data-stu-id="74bd9-132">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-133">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור השעות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של מכירות שלא חויב, ונתון בפועל שווה ערך, של מכירה, שחויב.</span><span class="sxs-lookup"><span data-stu-id="74bd9-133">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74bd9-134">הפקת חשבונית עובר עסקת הוצאה ללא ביצוע עריכות כלשהן בטיוטת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="74bd9-134">Invoicing an expense transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-135">ביטול עסקת מכירה שלא חויבה עבור הכמות והסכום שבאישור ההוצאה המקורי.</span><span class="sxs-lookup"><span data-stu-id="74bd9-135">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-136">נתון בפועל של מכירה שחויב עבור הכמות והסכום שבאישור ההוצאה המקורי.</span><span class="sxs-lookup"><span data-stu-id="74bd9-136">A billed sales actual for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="74bd9-137">הפקת חשבונית עובר עסקת הוצאה שנערכה כדי להפחית את הכמות.</span><span class="sxs-lookup"><span data-stu-id="74bd9-137">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-138">ביטול עסקת מכירה שלא חויבה עבור הכמות והסכום שבאישור ההוצאה המקורי.</span><span class="sxs-lookup"><span data-stu-id="74bd9-138">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-139">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור הכמות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="74bd9-139">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-140">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר לא ניתן לחיוב עבור הכמות והסכום שנותרו לאחר ניכוי הנתונים שתוקנו בפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="74bd9-140">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74bd9-141">הפקת חשבונית עובר עסקת הוצאה שנערכה כדי להגדיל את הכמות.</span><span class="sxs-lookup"><span data-stu-id="74bd9-141">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-142">ביטול עסקת מכירה שלא חויבה עבור הכמות והסכום שבאישור ההוצאה המקורי.</span><span class="sxs-lookup"><span data-stu-id="74bd9-142">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-143">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור הכמות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="74bd9-143">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74bd9-144">הפקת חשבונית לעסקת חומר ללא כל עריכה בחשבונית הטיוטה.</span><span class="sxs-lookup"><span data-stu-id="74bd9-144">Invoicing a material transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-145">‏‫ביטול עסקת מכירות שלא חויבה‬ על הכמות והסכום באישור המקורי של שימוש בחומרים.</span><span class="sxs-lookup"><span data-stu-id="74bd9-145">An unbilled sales reversal for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-146">‏‫נתונים בפועל למכירות על הכמות והסכום באישור המקורי של שימוש בחומרים.</span><span class="sxs-lookup"><span data-stu-id="74bd9-146">A billed sales actual for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="74bd9-147">הפקת חשבונית לעסקת חומר שנערכה כדי להפחית את הכמות.</span><span class="sxs-lookup"><span data-stu-id="74bd9-147">Invoicing a material transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-148">‏‫ביטול עסקת מכירות שלא חויבה‬ על הכמות והסכום באישור המקורי של זמן.</span><span class="sxs-lookup"><span data-stu-id="74bd9-148">An unbilled sales reversal for the quantity and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-149">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור הכמות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="74bd9-149">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-150">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר לא ניתן לחיוב עבור הכמות והסכום שנותרו לאחר ניכוי הנתונים שתוקנו בפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="74bd9-150">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74bd9-151">הפקת חשבונית לעסקת חומר שנערכה כדי להגדיל את הכמות.</span><span class="sxs-lookup"><span data-stu-id="74bd9-151">Invoicing a material transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-152">‏‫ביטול עסקת מכירות שלא חויבה‬ על הכמות והסכום באישור המקורי של שימוש בחומרים.</span><span class="sxs-lookup"><span data-stu-id="74bd9-152">An unbilled sales reversal for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-153">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור הכמות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="74bd9-153">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="74bd9-154">הפקת חשבונית עובר עמלה.</span><span class="sxs-lookup"><span data-stu-id="74bd9-154">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-155">ביטול עסקת מכירות שלא חויבה עבור הסכום העמלה שבשורת היומן המקורית.</span><span class="sxs-lookup"><span data-stu-id="74bd9-155">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-156">נתון בפועל של מכירות שחויב עבור הכמות והסכום שבשורת יומן המקורית של העמלה.</span><span class="sxs-lookup"><span data-stu-id="74bd9-156">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="74bd9-157">הפקת חשבונית עבור אבן דרך.</span><span class="sxs-lookup"><span data-stu-id="74bd9-157">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="74bd9-158">נתון מכירות בפועל שחויב עבור סכום אבן הדרך בשאבן הדרך המקורית בסעיף חוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="74bd9-158">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
       
    </tbody>
</table>

[!INCLUDE[footer-include](../includes/footer-banner.md)]
