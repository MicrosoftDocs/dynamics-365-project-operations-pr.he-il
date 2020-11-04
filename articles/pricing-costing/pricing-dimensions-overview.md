---
title: מבט כולל על ממדי תמחור
description: נושא זה מספק מידע על ממדי תמחור ב- Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 6b1ebdc97ec4704ba256acb521c0f2e7c474940b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077415"
---
# <a name="pricing-dimensions-overview"></a><span data-ttu-id="49146-103">מבט כולל על ממדי תמחור</span><span class="sxs-lookup"><span data-stu-id="49146-103">Pricing dimensions overview</span></span>

<span data-ttu-id="49146-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="49146-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="49146-105">הממדים שבהם נעשה שימוש במשאבי אנוש כדי להגדיר תמחור ועלויות מתחלקים לשתי קטגוריות:</span><span class="sxs-lookup"><span data-stu-id="49146-105">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="49146-106">אנשים</span><span class="sxs-lookup"><span data-stu-id="49146-106">People</span></span>
- <span data-ttu-id="49146-107">עבודה מתוכננת</span><span class="sxs-lookup"><span data-stu-id="49146-107">Planned work</span></span>

<span data-ttu-id="49146-108">עקב כך, קיימים שני סוגים של ערכים זמינים בממד תמחור הזמינים:</span><span class="sxs-lookup"><span data-stu-id="49146-108">Because of this, there are two types of pricing dimension values available:</span></span>

- <span data-ttu-id="49146-109">**קבוצות של אפשרויות** : ממדים שהם ספירות קבועות עבור קבוצת ערכים.</span><span class="sxs-lookup"><span data-stu-id="49146-109">**Option sets** : Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="49146-110">**ערכים מבוססי-ישות** : ממדים שיכולים להיות קבוצות שונות של ערכים.</span><span class="sxs-lookup"><span data-stu-id="49146-110">**Entity-based values** : Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="49146-111">ממדי תמחור</span><span class="sxs-lookup"><span data-stu-id="49146-111">Pricing dimensions</span></span>

<span data-ttu-id="49146-112">Dynamics 365 Project Operations מגיע עם סט ברירת מחדל של ממדי תמחור.</span><span class="sxs-lookup"><span data-stu-id="49146-112">Dynamics 365 Project Operations ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="49146-113">תוכל להציג את מדדי התמחור האלה על-ידי מעבר אל **Project Operations** > **פרמטרים**.</span><span class="sxs-lookup"><span data-stu-id="49146-113">You can view these pricing dimensions by going to **Project Operations** > **Parameters**.</span></span> <span data-ttu-id="49146-114">ברשומת הפרמטר, בכרטיסיה **‬‏‫ממדי תמחור מבוססי-כמות** , ודא שבתפקיד, **msdyn_resourcecategory** וביחידה הארגונית להקצאת משאבים, **msdyn_organizationalunit** השדה **‏‫חל על מכירות‬** והשדה **‏‫חל על עלות‬** מוגדרים בתור **כן**.</span><span class="sxs-lookup"><span data-stu-id="49146-114">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="49146-115">כאשר השדות האלה זמינים תוכל להגדיר את המחיר ואת העלות עבור כל שילוב של תפקיד ויחידה ארגונית.</span><span class="sxs-lookup"><span data-stu-id="49146-115">With these fields enabled, you can set up the price and cost for each role and organizational unit combination.</span></span>

<span data-ttu-id="49146-116">אם אתה צריך מחיר או עלות עבור המשאבים שלך באמצעות תכונות נוספות, תוכל ליצור שדות, ישויות וממדים מותאמים אישית.</span><span class="sxs-lookup"><span data-stu-id="49146-116">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span>

## <a name="pricing-human-resource-time"></a><span data-ttu-id="49146-117">תמחור זמן של משאב אנושי</span><span class="sxs-lookup"><span data-stu-id="49146-117">Pricing human resource time</span></span>
<span data-ttu-id="49146-118">כיצד ארגון מתמחר זמן של משאב אנושי הוא לרוב שיקול אסטרטגי חשוב שמשפיע ישירות על רווחיות הארגון.</span><span class="sxs-lookup"><span data-stu-id="49146-118">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="49146-119">עבוד עם הצוותים הפיננסיים וראשי אגפים כאשר הארגון שלך מוכן לזהות כיצד הוא מעוניין להגדיר את תעריפי עלויות וחיוב עבור הזמן של המשאב האנושי.</span><span class="sxs-lookup"><span data-stu-id="49146-119">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="49146-120">שיקולים אחרים לתמחור כוללים אם להשתמש מחדש בשדות או בישויות שאינם כרגע ממדי תמחור, אך מוחלים כממד תמחור עבור הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="49146-120">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="49146-121">שדות כמו **קטגוריית עסקה** ( **msdyn_transactioncategory** ) ו **משאב ניתן להזמנה** ( **bookableresource** ) הם דוגמאות לממדים מועמדים.</span><span class="sxs-lookup"><span data-stu-id="49146-121">Fields like **Transaction Category** ( **msdyn_transactioncategory** ) and **Bookable Resource** ( **bookableresource** ) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="49146-122">כדאי לשקול גם אם ממד התמחור שלך צריך להיות טבלה או קבוצת אפשרויות.</span><span class="sxs-lookup"><span data-stu-id="49146-122">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="49146-123">אם אתה צופה שינויים בערכים של ממד שיחרוג מ- 10 או 12 ואתה זקוק לתכונות נוספות בערכים אלה, תוכל ליצור ישות במקום קבוצת אפשרויות.</span><span class="sxs-lookup"><span data-stu-id="49146-123">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="49146-124">תחזוקה של קבוצת אפשרויות, כגון הוספה או הסרה של ערכים, מחייבת מנהל מערכת או מפתח בעוד שהוספת שורות חדשות לטבלה יכולה להתבצע על-ידי רוב המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="49146-124">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="49146-125">הדוגמה הבאה מציגה את תעריפי החיוב שמוגדרים בהתאם לתפקיד וליחידה הארגונית להקצאת משאבים שאליה המשאב שייך.</span><span class="sxs-lookup"><span data-stu-id="49146-125">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="49146-126">תעריפי עלויות מבוססים בדרך כלל על טווח השכר של העובד ועל היחידה הארגונית שאליה הוא שייך.</span><span class="sxs-lookup"><span data-stu-id="49146-126">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="49146-127">בדוגמה זו, הטבלאות של תעריף החיוב ותעריף העלויות ייראו כך.</span><span class="sxs-lookup"><span data-stu-id="49146-127">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="49146-128">**תעריפי חיוב לדוגמה**</span><span class="sxs-lookup"><span data-stu-id="49146-128">**Sample bill rates**</span></span>

| <span data-ttu-id="49146-129">תפקיד</span><span class="sxs-lookup"><span data-stu-id="49146-129">Role</span></span>        | <span data-ttu-id="49146-130">יחידה ארגונית</span><span class="sxs-lookup"><span data-stu-id="49146-130">Org Unit</span></span>    |<span data-ttu-id="49146-131">יחידה</span><span class="sxs-lookup"><span data-stu-id="49146-131">Unit</span></span>      |<span data-ttu-id="49146-132">מחיר</span><span class="sxs-lookup"><span data-stu-id="49146-132">Price</span></span>      |<span data-ttu-id="49146-133">מטבע</span><span class="sxs-lookup"><span data-stu-id="49146-133">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="49146-134">מפתח</span><span class="sxs-lookup"><span data-stu-id="49146-134">Developer</span></span>   | <span data-ttu-id="49146-135">Contoso US</span><span class="sxs-lookup"><span data-stu-id="49146-135">Contoso US</span></span>  |<span data-ttu-id="49146-136">Hour</span><span class="sxs-lookup"><span data-stu-id="49146-136">Hour</span></span> | <span data-ttu-id="49146-137">200</span><span class="sxs-lookup"><span data-stu-id="49146-137">200</span></span>|<span data-ttu-id="49146-138">USD</span><span class="sxs-lookup"><span data-stu-id="49146-138">USD</span></span>     |
| <span data-ttu-id="49146-139">מפתח</span><span class="sxs-lookup"><span data-stu-id="49146-139">Developer</span></span>   | <span data-ttu-id="49146-140">Contoso India</span><span class="sxs-lookup"><span data-stu-id="49146-140">Contoso India</span></span> |<span data-ttu-id="49146-141">Hour</span><span class="sxs-lookup"><span data-stu-id="49146-141">Hour</span></span>|   <span data-ttu-id="49146-142">112</span><span class="sxs-lookup"><span data-stu-id="49146-142">112</span></span>|<span data-ttu-id="49146-143">USD</span><span class="sxs-lookup"><span data-stu-id="49146-143">USD</span></span>     |


<span data-ttu-id="49146-144">**תעריפי עלויות לדוגמה**</span><span class="sxs-lookup"><span data-stu-id="49146-144">**Sample cost rates**</span></span>

| <span data-ttu-id="49146-145">טווח שכר</span><span class="sxs-lookup"><span data-stu-id="49146-145">Salary Band</span></span>     | <span data-ttu-id="49146-146">יחידה ארגונית</span><span class="sxs-lookup"><span data-stu-id="49146-146">Org Unit</span></span>    |<span data-ttu-id="49146-147">יחידה</span><span class="sxs-lookup"><span data-stu-id="49146-147">Unit</span></span>      |<span data-ttu-id="49146-148">מחיר</span><span class="sxs-lookup"><span data-stu-id="49146-148">Price</span></span>      |<span data-ttu-id="49146-149">מטבע</span><span class="sxs-lookup"><span data-stu-id="49146-149">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="49146-150">טווח1_של החברה שלי</span><span class="sxs-lookup"><span data-stu-id="49146-150">My company_Band1</span></span> | <span data-ttu-id="49146-151">Contoso US</span><span class="sxs-lookup"><span data-stu-id="49146-151">Contoso US</span></span>  |<span data-ttu-id="49146-152">Hour</span><span class="sxs-lookup"><span data-stu-id="49146-152">Hour</span></span> | <span data-ttu-id="49146-153">145</span><span class="sxs-lookup"><span data-stu-id="49146-153">145</span></span>|<span data-ttu-id="49146-154">USD</span><span class="sxs-lookup"><span data-stu-id="49146-154">USD</span></span>     |
| <span data-ttu-id="49146-155">טווח2_של החברה שלי</span><span class="sxs-lookup"><span data-stu-id="49146-155">My company_Band2</span></span> | <span data-ttu-id="49146-156">Contoso India</span><span class="sxs-lookup"><span data-stu-id="49146-156">Contoso India</span></span> |<span data-ttu-id="49146-157">Hour</span><span class="sxs-lookup"><span data-stu-id="49146-157">Hour</span></span>|   <span data-ttu-id="49146-158">67</span><span class="sxs-lookup"><span data-stu-id="49146-158">67</span></span>|<span data-ttu-id="49146-159">USD</span><span class="sxs-lookup"><span data-stu-id="49146-159">USD</span></span>     |
