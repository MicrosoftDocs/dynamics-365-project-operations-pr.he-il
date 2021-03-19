---
title: אישור חשבונית פרופורמה
description: נושא זה מספק מידע על אישור חשבונית פרופורמה.
author: rumant
manager: AnnBe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b2ed241509d2643d841ce55777e6e316612f70b8
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287869"
---
# <a name="confirm-a-proforma-invoice"></a><span data-ttu-id="1c8eb-103">אישור חשבונית פרופורמה</span><span class="sxs-lookup"><span data-stu-id="1c8eb-103">Confirm a proforma invoice</span></span>

<span data-ttu-id="1c8eb-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="1c8eb-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="1c8eb-105">לאחר אישור חשבונית פרופורמה, מצב חשבונית הפרויקט מתעדכן ל **מאושר**.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="1c8eb-106">לאחר אישור חשבונית, היא תוגדר 'לקריאה בלבד'.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="1c8eb-107">מכאן ואילך, ניתן לתקן את החשבונית רק אם ישנם תיקונים או זיכויים יזומים על ידי הלקוח, או כאשר החשבונית מסומנת כחשבונית ששולמה.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits, or when it's marked as paid.</span></span>

<span data-ttu-id="1c8eb-108">הטבלה הבאה מפרטת את ניתונים בפועל שנוצרו על ידי המערכת.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="1c8eb-109">ניתונים בפועל אלו נוצרים כאשר פעולות מסוימות מבוצעות בטיוטת חשבונית הפרויקט לפני אישורה.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="416" valign="top">
                <p><span data-ttu-id="1c8eb-110">
                    <strong>תרחיש</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1c8eb-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="608" valign="top">
                <p><span data-ttu-id="1c8eb-111">
                    <strong>ניתונים בפועל שנוצרו באישור</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1c8eb-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1c8eb-112">הפקת חשבונית עובר עסקת זמן ללא כל עריכות בטיוטת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-112">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-113">ביטול עסקת מכירה שחויבה עבור השעות והסכום שבאישור הזמן המקורי.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-113">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-114">נתוני מכירות בפועל שחוייבו עבור השעות והסכום שבאישור הזמן המקורי.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-114">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="1c8eb-115">הפקת חשבונית על עסקת זמן שנערכה כדי להפחית את הכמות.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-115">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-116">ביטול עסקת מכירה שחויבה עבור השעות והסכום שבאישור הזמן המקורי.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-116">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-117">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור השעות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של מכירות שלא חויב, ונתון בפועל שווה ערך, של מכירה, שחויב.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-117">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-118">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר לא ניתן לחיוב עבור השעות והסכום שנותרו לאחר ניכוי הנתונים שתוקנו בפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-118">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1c8eb-119">הפקת חשבונית על עסקת זמן שנערכה כדי להגדיל את הכמות.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-119">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-120">ביטול עסקת מכירה שחויבה עבור השעות והסכום שבאישור הזמן המקורי.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-120">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-121">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור השעות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של מכירות שלא חויב, ונתון בפועל שווה ערך, של מכירה, שחויב.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-121">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1c8eb-122">הפקת חשבונית עובר עסקת הוצאה ללא ביצוע עריכות כלשהן בטיוטת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-122">Invoicing an expense transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-123">ביטול עסקת מכירה שלא חויבה עבור הכמות והסכום שבאישור ההוצאה המקורי.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-123">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-124">נתון בפועל של מכירה שחויב עבור הכמות והסכום שבאישור ההוצאה המקורי.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-124">A billed sales actual for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="1c8eb-125">הפקת חשבונית עובר עסקת הוצאה שנערכה כדי להפחית את הכמות.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-125">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-126">ביטול עסקת מכירה שלא חויבה עבור הכמות והסכום שבאישור ההוצאה המקורי.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-126">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-127">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור הכמות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-127">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-128">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר לא ניתן לחיוב עבור הכמות והסכום שנותרו לאחר ניכוי הנתונים שתוקנו בפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-128">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent of the billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1c8eb-129">הפקת חשבונית עובר עסקת הוצאה שנערכה כדי להגדיל את הכמות.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-129">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-130">ביטול עסקת מכירה שלא חויבה עבור הכמות והסכום שבאישור ההוצאה המקורי.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-130">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-131">‏‫נתון בפועל חדש של מכירות שלא חויב, אשר ניתן לחיוב עבור הכמות והסכום שבפרט שורת החשבונית הערוכה, ביטול של הנתון בפועל של המכירות שלא חויב, ונתון בפועל שווה ערך, של מכירות, שחויב.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-131">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the untilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="1c8eb-132">הפקת חשבונית עובר עמלה.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-132">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-133">ביטול עסקת מכירות שלא חויבה עבור הסכום העמלה שבשורת היומן המקורית.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-133">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-134">נתון בפועל של מכירות שחויב עבור הכמות והסכום שבשורת יומן המקורית של העמלה.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-134">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="1c8eb-135">הפקת חשבונית עבור אבן דרך.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-135">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="1c8eb-136">נתון מכירות בפועל שחויב עבור סכום אבן הדרך בשאבן הדרך המקורית בסעיף חוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="1c8eb-136">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]