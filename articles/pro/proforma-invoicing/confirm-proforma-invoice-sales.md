---
title: אישור חשבונית פרופורמה
description: נושא זה מספק מידע על אישור חשבוניות פרופורמה ב-Project Operations.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 4b67ee6848efdcb85cf732c1eaa3e40cdc51a2e2
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077216"
---
# <a name="confirming-a-proforma-invoice"></a><span data-ttu-id="12432-103">אישור חשבונית פרופורמה</span><span class="sxs-lookup"><span data-stu-id="12432-103">Confirming a proforma invoice</span></span>

<span data-ttu-id="12432-104">_**חל על** : פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="12432-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="12432-105">לאחר אישור חשבונית פרופורמה, מצב חשבונית הפרויקט מתעדכן ל **מאושר**.</span><span class="sxs-lookup"><span data-stu-id="12432-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="12432-106">לאחר אישור חשבונית, היא תוגדר 'לקריאה בלבד'.</span><span class="sxs-lookup"><span data-stu-id="12432-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="12432-107">בהמשך, ניתן לתקן את החשבונית רק אם ישנם תיקונים או זיכויים יזומים על ידי הלקוח, או אם החשבונית מסומנת כחשבונית ששולמה.</span><span class="sxs-lookup"><span data-stu-id="12432-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits, of if the invoice is marked as paid.</span></span>

<span data-ttu-id="12432-108">הטבלה הבאה מפרטת את ניתונים בפועל שנוצרו על ידי המערכת.</span><span class="sxs-lookup"><span data-stu-id="12432-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="12432-109">ניתונים בפועל אלו נוצרים כאשר פעולות מסוימות מבוצעות בטיוטת חשבונית הפרויקט לפני אישורה.</span><span class="sxs-lookup"><span data-stu-id="12432-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="12432-110">
                    <strong>תרחיש</strong>
                </span><span class="sxs-lookup"><span data-stu-id="12432-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="12432-111">
                    <strong>ניתונים בפועל שנוצרו באישור</strong>
                </span><span class="sxs-lookup"><span data-stu-id="12432-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="12432-112">הפקת חשבונית עבור מקדמה או ריטיינר</span><span class="sxs-lookup"><span data-stu-id="12432-112">Invoicing an advance or retainer</span></span> </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-113">חיוב של נתונים בפועל של מכירות מסוג <strong>ריטיינר</strong> נוצר עבור הסכום של המקדמה או הריטיינר.</span><span class="sxs-lookup"><span data-stu-id="12432-113">A billed sales actual of type, <strong>Retainer</strong> is created for the amount on the advance or retainer.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-114">נתון בפועל של מכירות, בסכום שלילי, שלא חויב של הריטיינר או המקדמה, אשר ישמש להתאמה.</span><span class="sxs-lookup"><span data-stu-id="12432-114">An unbilled sales actual of a negative amount of the retainer or advance to be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="12432-115">לאחר תיאום מלא של ריטיינר או מקדמה על חשבונית.</span><span class="sxs-lookup"><span data-stu-id="12432-115">After fully reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-116">ביטול עסקת מכירה שלא חויבה, של הריטיינר או המקדמה, שנוצר למטרות התאמה.</span><span class="sxs-lookup"><span data-stu-id="12432-116">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="12432-117">סכום זה הוא סכום חיובי מכיוון שהוא נועד לבטל את הסכום השלילי שנוצר בעת הגשת החשבונית עובר הריטיינר או המקדמה.</span><span class="sxs-lookup"><span data-stu-id="12432-117">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-118">נתון מכירה בפועל שחויב, בסכום הרשום בחשבונית זו.</span><span class="sxs-lookup"><span data-stu-id="12432-118">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="12432-119">לאחר תיאום חלקי של ריטיינר או מקדמה בחשבונית.</span><span class="sxs-lookup"><span data-stu-id="12432-119">After partially reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-120">ביטול עסקת מכירה שלא חויבה, של הריטיינר או המקדמה, שנוצר למטרות התאמה.</span><span class="sxs-lookup"><span data-stu-id="12432-120">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="12432-121">סכום זה הוא סכום חיובי מכיוון שהוא נועד לבטל את הסכום השלילי שנוצר בעת הגשת החשבונית עובר הריטיינר או המקדמה.</span><span class="sxs-lookup"><span data-stu-id="12432-121">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-122">נתון מכירה בפועל שחויב, בסכום הרשום בחשבונית זו.</span><span class="sxs-lookup"><span data-stu-id="12432-122">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-123">נתון בפועל שלילי של מכירות, שלא חויב עבור סכום הריטיינר או המקדמה שנותר, שישמש להתאמה בחשבוניות עתידיות.</span><span class="sxs-lookup"><span data-stu-id="12432-123">A negative unbilled sales actual of the remaining retainer or advance amount to be used for reconciliation on future invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="12432-124">הפקת חשבונית עובר עסקת זמן ללא כל עריכות בטיוטת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="12432-124">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-125">ביטול עסקת מכירה שחויבה עבור השעות והסכום שבאישור הזמן המקורי.</span><span class="sxs-lookup"><span data-stu-id="12432-125">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-126">נתוני מכירות בפועל שחוייבו עבור השעות והסכום שבאישור הזמן המקורי.</span><span class="sxs-lookup"><span data-stu-id="12432-126">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="12432-127">הפקת חשבונית על עסקת זמן שנערכה כדי להפחית את הכמות.</span><span class="sxs-lookup"><span data-stu-id="12432-127">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-128">ביטול עסקת מכירה שחויבה עבור השעות והסכום שבאישור הזמן המקורי.</span><span class="sxs-lookup"><span data-stu-id="12432-128">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-129">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור השעות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של מכירות ונתון בפועל שווה ערך, של מכירה, שחויב.</span><span class="sxs-lookup"><span data-stu-id="12432-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-130">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר לא ניתן לחיוב עבור השעות והסכום לאחר ניכוי הנתונים שתוקנו בפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של מכירות ונתון בפועל שווה ערך, של מכירה, שחויב.</span><span class="sxs-lookup"><span data-stu-id="12432-130">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="12432-131">הפקת חשבונית על עסקת זמן שנערכה כדי להגדיל את הכמות.</span><span class="sxs-lookup"><span data-stu-id="12432-131">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-132">ביטול עסקת מכירה שחויבה עבור השעות והסכום שבאישור הזמן המקורי.</span><span class="sxs-lookup"><span data-stu-id="12432-132">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-133">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור השעות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של מכירות שלא חויב, ונתון בפועל שווה ערך, של מכירה, שחויב.</span><span class="sxs-lookup"><span data-stu-id="12432-133">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="12432-134">הפקת חשבונית עובר עסקת הוצאה ללא ביצוע עריכות כלשהן בטיוטת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="12432-134">Invoicing an expense transaction without any edits on draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-135">ביטול עסקת מכירה שלא חויבה עבור הכמות והסכום שבאישור ההוצאה המקורי.</span><span class="sxs-lookup"><span data-stu-id="12432-135">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-136">נתון בפועל של מכירה שחויב עבור הכמות והסכום שבאישור ההוצאה המקורי</span><span class="sxs-lookup"><span data-stu-id="12432-136">A billed sales actual for the quantity and amount on the original expense approval</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="12432-137">הפקת חשבונית עובר עסקת הוצאה שנערכה כדי להפחית את הכמות.</span><span class="sxs-lookup"><span data-stu-id="12432-137">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-138">ביטול עסקת מכירה שלא חויבה עבור הכמות והסכום שבאישור ההוצאה המקורי.</span><span class="sxs-lookup"><span data-stu-id="12432-138">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-139">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור הכמות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="12432-139">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-140">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר לא ניתן לחיוב עבור הכמות והסכום שנותרו לאחר ניכוי הנתונים שתוקנו בפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="12432-140">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="12432-141">הפקת חשבונית עובר עסקת הוצאה שנערכה כדי להגדיל את הכמות.</span><span class="sxs-lookup"><span data-stu-id="12432-141">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-142">ביטול עסקת מכירה שלא חויבה עבור הכמות והסכום שבאישור ההוצאה המקורי.</span><span class="sxs-lookup"><span data-stu-id="12432-142">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-143">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור הכמות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="12432-143">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="12432-144">הפקת חשבונית עובר עמלה.</span><span class="sxs-lookup"><span data-stu-id="12432-144">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-145">ביטול עסקת מכירות שלא חויבה עבור הסכום העמלה שבשורת היומן המקורית.</span><span class="sxs-lookup"><span data-stu-id="12432-145">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-146">נתון בפועל של מכירות שחויב עבור הכמות והסכום שבשורת יומן המקורית של העמלה.</span><span class="sxs-lookup"><span data-stu-id="12432-146">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="12432-147">הפקת חשבונית עבור אבן דרך.</span><span class="sxs-lookup"><span data-stu-id="12432-147">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-148">נתון מכירות בפועל שחויב עבור סכום אבן הדרך בשאבן הדרך המקורית בסעיף חוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="12432-148">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="12432-149">הפקת חשבונית עבור סעיף חוזה מבוסס מוצר.</span><span class="sxs-lookup"><span data-stu-id="12432-149">Invoicing a product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="12432-150">נתון מכירה בפועל שחויב עבור שורת המוצר והסכום המובאים מסעיף חוזה מבוסס מוצר.</span><span class="sxs-lookup"><span data-stu-id="12432-150">A billed sales actual for the product line with the quantity and amount coming from the product-based contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>
