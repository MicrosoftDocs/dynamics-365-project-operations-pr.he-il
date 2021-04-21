---
title: אישור חשבונית פרופורמה של פרוייקט
description: נושא זה מספק מידע על אישור חשבוניות פרופורמה‬ של פרויקט ב-Project Operations.
author: rumant
manager: Annbe
ms.date: 04/05/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 144c1b6a49951af8be0c619f41808e7617e59c92
ms.sourcegitcommit: ca0fc078d1a12484eca193fe051b8442c0559db8
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/07/2021
ms.locfileid: "5867087"
---
# <a name="confirm-a-proforma-project-invoice"></a><span data-ttu-id="c9c43-103">אישור חשבונית פרופורמה של פרוייקט</span><span class="sxs-lookup"><span data-stu-id="c9c43-103">Confirm a proforma project invoice</span></span> 

<span data-ttu-id="c9c43-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="c9c43-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="c9c43-105">לאחר אישור חשבונית פרופורמה, מצב חשבונית הפרויקט מתעדכן ל **מאושר**.</span><span class="sxs-lookup"><span data-stu-id="c9c43-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="c9c43-106">לאחר אישור חשבונית, היא תוגדר 'לקריאה בלבד'.</span><span class="sxs-lookup"><span data-stu-id="c9c43-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="c9c43-107">בהמשך, ניתן לתקן את החשבונית רק אם ישנם תיקונים או זיכויים ביוזמת הלקוח.</span><span class="sxs-lookup"><span data-stu-id="c9c43-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits.</span></span>

<span data-ttu-id="c9c43-108">הטבלה הבאה מפרטת את ניתונים בפועל שנוצרו על ידי המערכת.</span><span class="sxs-lookup"><span data-stu-id="c9c43-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="c9c43-109">ניתונים בפועל אלו נוצרים כאשר פעולות מסוימות מבוצעות בטיוטת חשבונית הפרויקט לפני אישורה.</span><span class="sxs-lookup"><span data-stu-id="c9c43-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="c9c43-110">
                    <strong>תרחיש</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c9c43-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="c9c43-111">
                    <strong>ניתונים בפועל שנוצרו באישור</strong>
                </span><span class="sxs-lookup"><span data-stu-id="c9c43-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c9c43-112">הפקת חשבונית עבור מקדמה או ריטיינר</span><span class="sxs-lookup"><span data-stu-id="c9c43-112">Invoicing an advance or retainer</span></span> </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-113">חיוב של נתונים בפועל של מכירות מסוג <strong>ריטיינר</strong> נוצר עבור הסכום של המקדמה או הריטיינר.</span><span class="sxs-lookup"><span data-stu-id="c9c43-113">A billed sales actual of type, <strong>Retainer</strong> is created for the amount on the advance or retainer.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-114">נתון בפועל של מכירות, בסכום שלילי, שלא חויב של הריטיינר או המקדמה, אשר ישמש להתאמה.</span><span class="sxs-lookup"><span data-stu-id="c9c43-114">An unbilled sales actual of a negative amount of the retainer or advance to be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c9c43-115">לאחר תיאום מלא של ריטיינר או מקדמה על חשבונית.</span><span class="sxs-lookup"><span data-stu-id="c9c43-115">After fully reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-116">ביטול עסקת מכירה שלא חויבה, של הריטיינר או המקדמה, שנוצר למטרות התאמה.</span><span class="sxs-lookup"><span data-stu-id="c9c43-116">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="c9c43-117">סכום זה הוא סכום חיובי מכיוון שהוא נועד לבטל את הסכום השלילי שנוצר בעת הגשת החשבונית עובר הריטיינר או המקדמה.</span><span class="sxs-lookup"><span data-stu-id="c9c43-117">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-118">נתון מכירה בפועל שחויב, בסכום הרשום בחשבונית זו.</span><span class="sxs-lookup"><span data-stu-id="c9c43-118">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="c9c43-119">לאחר תיאום חלקי של ריטיינר או מקדמה בחשבונית.</span><span class="sxs-lookup"><span data-stu-id="c9c43-119">After partially reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-120">ביטול עסקת מכירה שלא חויבה, של הריטיינר או המקדמה, שנוצר למטרות התאמה.</span><span class="sxs-lookup"><span data-stu-id="c9c43-120">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="c9c43-121">סכום זה הוא סכום חיובי מכיוון שהוא נועד לבטל את הסכום השלילי שנוצר בעת הגשת החשבונית עובר הריטיינר או המקדמה.</span><span class="sxs-lookup"><span data-stu-id="c9c43-121">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-122">נתון מכירה בפועל שחויב, בסכום הרשום בחשבונית זו.</span><span class="sxs-lookup"><span data-stu-id="c9c43-122">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-123">נתון בפועל שלילי של מכירות, שלא חויב עבור סכום הריטיינר או המקדמה שנותר, שישמש להתאמה בחשבוניות עתידיות.</span><span class="sxs-lookup"><span data-stu-id="c9c43-123">A negative unbilled sales actual of the remaining retainer or advance amount to be used for reconciliation on future invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c9c43-124">הפקת חשבונית עובר עסקת זמן ללא כל עריכות בטיוטת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="c9c43-124">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-125">ביטול עסקת מכירה שחויבה עבור השעות והסכום שבאישור הזמן המקורי.</span><span class="sxs-lookup"><span data-stu-id="c9c43-125">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-126">נתוני מכירות בפועל שחוייבו עבור השעות והסכום שבאישור הזמן המקורי.</span><span class="sxs-lookup"><span data-stu-id="c9c43-126">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="c9c43-127">הפקת חשבונית על עסקת זמן שנערכה כדי להפחית את הכמות.</span><span class="sxs-lookup"><span data-stu-id="c9c43-127">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-128">ביטול עסקת מכירה שחויבה עבור השעות והסכום שבאישור הזמן המקורי.</span><span class="sxs-lookup"><span data-stu-id="c9c43-128">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-129">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור השעות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של מכירות ונתון בפועל שווה ערך, של מכירה, שחויב.</span><span class="sxs-lookup"><span data-stu-id="c9c43-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-130">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר לא ניתן לחיוב עבור השעות והסכום לאחר ניכוי הנתונים שתוקנו בפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של מכירות ונתון בפועל שווה ערך, של מכירה, שחויב.</span><span class="sxs-lookup"><span data-stu-id="c9c43-130">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c9c43-131">הפקת חשבונית על עסקת זמן שנערכה כדי להגדיל את הכמות.</span><span class="sxs-lookup"><span data-stu-id="c9c43-131">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-132">ביטול עסקת מכירה שחויבה עבור השעות והסכום שבאישור הזמן המקורי.</span><span class="sxs-lookup"><span data-stu-id="c9c43-132">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-133">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור השעות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של מכירות שלא חויב, ונתון בפועל שווה ערך, של מכירה, שחויב.</span><span class="sxs-lookup"><span data-stu-id="c9c43-133">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c9c43-134">הפקת חשבונית עובר עסקת הוצאה ללא ביצוע עריכות כלשהן בטיוטת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="c9c43-134">Invoicing an expense transaction without any edits on draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-135">ביטול עסקת מכירה שלא חויבה עבור הכמות והסכום שבאישור ההוצאה המקורי.</span><span class="sxs-lookup"><span data-stu-id="c9c43-135">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-136">נתון בפועל של מכירה שחויב עבור הכמות והסכום שבאישור ההוצאה המקורי</span><span class="sxs-lookup"><span data-stu-id="c9c43-136">A billed sales actual for the quantity and amount on the original expense approval</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="c9c43-137">הפקת חשבונית עובר עסקת הוצאה שנערכה כדי להפחית את הכמות.</span><span class="sxs-lookup"><span data-stu-id="c9c43-137">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-138">ביטול עסקת מכירה שלא חויבה עבור הכמות והסכום שבאישור ההוצאה המקורי.</span><span class="sxs-lookup"><span data-stu-id="c9c43-138">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-139">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור הכמות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="c9c43-139">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-140">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר לא ניתן לחיוב עבור הכמות והסכום שנותרו לאחר ניכוי הנתונים שתוקנו בפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="c9c43-140">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c9c43-141">הפקת חשבונית עובר עסקת הוצאה שנערכה כדי להגדיל את הכמות.</span><span class="sxs-lookup"><span data-stu-id="c9c43-141">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-142">ביטול עסקת מכירה שלא חויבה עבור הכמות והסכום שבאישור ההוצאה המקורי.</span><span class="sxs-lookup"><span data-stu-id="c9c43-142">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-143">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור הכמות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="c9c43-143">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c9c43-144">הפקת חשבונית לעסקת חומר ללא כל עריכה בחשבונית הטיוטה.</span><span class="sxs-lookup"><span data-stu-id="c9c43-144">Invoicing a material transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-145">‏‫ביטול עסקת מכירות שלא חויבה‬ על הכמות והסכום באישור המקורי של שימוש בחומרים.</span><span class="sxs-lookup"><span data-stu-id="c9c43-145">An unbilled sales reversal for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-146">‏‫נתונים בפועל למכירות על הכמות והסכום באישור המקורי של שימוש בחומרים.</span><span class="sxs-lookup"><span data-stu-id="c9c43-146">A billed sales actual for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="c9c43-147">הפקת חשבונית לעסקת חומר שנערכה כדי להפחית את הכמות.</span><span class="sxs-lookup"><span data-stu-id="c9c43-147">Invoicing a material transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-148">‏‫ביטול עסקת מכירות שלא חויבה‬ על הכמות והסכום באישור המקורי של זמן.</span><span class="sxs-lookup"><span data-stu-id="c9c43-148">An unbilled sales reversal for the quantity and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-149">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור הכמות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="c9c43-149">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-150">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר לא ניתן לחיוב עבור הכמות והסכום שנותרו לאחר ניכוי הנתונים שתוקנו בפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="c9c43-150">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c9c43-151">הפקת חשבונית לעסקת חומר שנערכה כדי להגדיל את הכמות.</span><span class="sxs-lookup"><span data-stu-id="c9c43-151">Invoicing a material transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-152">‏‫ביטול עסקת מכירות שלא חויבה‬ על הכמות והסכום באישור המקורי של שימוש בחומרים.</span><span class="sxs-lookup"><span data-stu-id="c9c43-152">An unbilled sales reversal for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-153">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור הכמות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="c9c43-153">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="c9c43-154">הפקת חשבונית עובר עמלה.</span><span class="sxs-lookup"><span data-stu-id="c9c43-154">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-155">ביטול עסקת מכירות שלא חויבה עבור הסכום העמלה שבשורת היומן המקורית.</span><span class="sxs-lookup"><span data-stu-id="c9c43-155">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-156">נתון בפועל של מכירות שחויב עבור הכמות והסכום שבשורת יומן המקורית של העמלה.</span><span class="sxs-lookup"><span data-stu-id="c9c43-156">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="c9c43-157">הפקת חשבונית עבור אבן דרך.</span><span class="sxs-lookup"><span data-stu-id="c9c43-157">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-158">נתון מכירות בפועל שחויב עבור סכום אבן הדרך בשאבן הדרך המקורית בסעיף חוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="c9c43-158">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="c9c43-159">הפקת חשבונית עבור סעיף חוזה מבוסס מוצר.</span><span class="sxs-lookup"><span data-stu-id="c9c43-159">Invoicing a product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="c9c43-160">נתון מכירה בפועל שחויב עבור שורת המוצר והסכום המובאים מסעיף חוזה מבוסס מוצר.</span><span class="sxs-lookup"><span data-stu-id="c9c43-160">A billed sales actual for the product line with the quantity and amount coming from the product-based contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
