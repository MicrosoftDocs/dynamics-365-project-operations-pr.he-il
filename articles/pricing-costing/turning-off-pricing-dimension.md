---
title: השבתת ממד תמחור
description: נושא זה מספק מידע על אופן ההשבתה של ממדי תמחור.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
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
ms.openlocfilehash: ffeff2ab465f37b8a4e40f4e64b118e3bb412cb8
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4119284"
---
# <a name="turning-off-a-pricing-dimension"></a><span data-ttu-id="f8065-103">השבתת ממד תמחור</span><span class="sxs-lookup"><span data-stu-id="f8065-103">Turning off a pricing dimension</span></span>

<span data-ttu-id="f8065-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="f8065-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f8065-105">ייתכן שתצטרך לסקור ולעדכן את אסטרטגיית התמחור שלך כל כמה שנים.</span><span class="sxs-lookup"><span data-stu-id="f8065-105">You may need to review and update your pricing strategy every few years.</span></span> <span data-ttu-id="f8065-106">כל העדכונים שאתה מבצע עשויים לדרוש ממך לבטל את ממד התמחור הקיים וליצור ממד חדש.</span><span class="sxs-lookup"><span data-stu-id="f8065-106">Any updates you make might require that you turn off an existing pricing dimension and create a new one.</span></span> <span data-ttu-id="f8065-107">לדוגמה, ייתכן שתמחרת בעבר לפי **תפקיד**, אבל עכשיו החלטת לתמחר לפי **ניסיון בעבודה**.</span><span class="sxs-lookup"><span data-stu-id="f8065-107">For example, you may have previously priced by **Role**, but now you have decided to price by **Work Experience**.</span></span> <span data-ttu-id="f8065-108">כתוצאה מכך, ייתכן שתידרש לבטל את **תפקיד** בתור ממד תמחור וליצור את **ניסיון בעבודה** בתור ממד תמחור חדש.</span><span class="sxs-lookup"><span data-stu-id="f8065-108">This may require you to turn off **Role** as a pricing dimension and create **Work Experience** as a new pricing dimension.</span></span> 

<span data-ttu-id="f8065-109">ניתן לבטל ממד תמחור, אם הוא מוגדר מראש או מותאם אישית, על-ידי הגדרת השדות **חל על עלות** ו **חל על מכירות** בממד התמחור לערך **לא**.</span><span class="sxs-lookup"><span data-stu-id="f8065-109">Turning off a pricing dimension, regardless if it is out-of-the-box or custom, can be done by setting the **Applicable to Cost** and **Applicable to Sales** fields of the Pricing Dimension to **No**.</span></span>

<span data-ttu-id="f8065-110">עם זאת, כאשר תעשה זאת, ייתכן שתקבל את הודעת השגיאה, **לא ניתן לעדכן או למחוק את ממד התמחור אם יש רשומות מחירים משויכות.**</span><span class="sxs-lookup"><span data-stu-id="f8065-110">However, when you do this, you might receive the error message, **Pricing dimension cannot be updated or deleted if there are associated price records.**</span></span>

<span data-ttu-id="f8065-111">הודעת שגיאה זו מציינת שקיימות רשומות מחיר שהוגדרו קודם לכן עבור הממד שמבוטל.</span><span class="sxs-lookup"><span data-stu-id="f8065-111">This error message indicates that there are price records that were previously set up for the dimension that is being turned off.</span></span> <span data-ttu-id="f8065-112">כל הרשומות של **מחיר תפקיד** ו **ייקור מחיר תפקיד** המפנות לממד חייבות להימחק לפני שניתן יהיה להגדיר את ישימות הממד לערך **לא**.</span><span class="sxs-lookup"><span data-stu-id="f8065-112">All **Role Price** and **Role Price Markup** records that refer to a dimension must be deleted before the dimension’s applicability can be to set to **No**.</span></span> <span data-ttu-id="f8065-113">כלל זה חל על ממדי תמחור מוגדרים מראש ועל ממדי תמחור מותאמים אישית שיצרת.</span><span class="sxs-lookup"><span data-stu-id="f8065-113">This rule applies to both out-of-the-box pricing dimensions and any custom pricing dimensions that you may have created.</span></span> <span data-ttu-id="f8065-114">הסיבה לאימות זה היא שלרשומה **מחיר תפקיד** חייב להיות שילוב ייחודי של ממדים.</span><span class="sxs-lookup"><span data-stu-id="f8065-114">The reason for this validation is because each **Role Price** record must have a unique combination of dimensions.</span></span> <span data-ttu-id="f8065-115">לדוגמה, במחירון הנקרא **תעריפי עלויות בארה"ב 2018**, מופיעות השורות הבאות של **מחיר תפקיד**.</span><span class="sxs-lookup"><span data-stu-id="f8065-115">For example, on a price list called **US Cost Rates 2018**, you have the following **Role price** rows.</span></span> 

| <span data-ttu-id="f8065-116">כותרת סטנדרטית</span><span class="sxs-lookup"><span data-stu-id="f8065-116">Standard Title</span></span>         | <span data-ttu-id="f8065-117">יחידה ארגונית</span><span class="sxs-lookup"><span data-stu-id="f8065-117">Org Unit</span></span>    |<span data-ttu-id="f8065-118">יחידה</span><span class="sxs-lookup"><span data-stu-id="f8065-118">Unit</span></span>   |<span data-ttu-id="f8065-119">מחיר</span><span class="sxs-lookup"><span data-stu-id="f8065-119">Price</span></span>  |<span data-ttu-id="f8065-120">מטבע</span><span class="sxs-lookup"><span data-stu-id="f8065-120">Currency</span></span>  |
| -----------------------|-------------|-------|-------|----------|
| <span data-ttu-id="f8065-121">מהנדס מערכות</span><span class="sxs-lookup"><span data-stu-id="f8065-121">Systems Engineer</span></span>|<span data-ttu-id="f8065-122">Contoso US</span><span class="sxs-lookup"><span data-stu-id="f8065-122">Contoso US</span></span>|<span data-ttu-id="f8065-123">שעה</span><span class="sxs-lookup"><span data-stu-id="f8065-123">Hour</span></span>| <span data-ttu-id="f8065-124">100</span><span class="sxs-lookup"><span data-stu-id="f8065-124">100</span></span>|<span data-ttu-id="f8065-125">USD</span><span class="sxs-lookup"><span data-stu-id="f8065-125">USD</span></span>|
| <span data-ttu-id="f8065-126">מהנדס מערכות בכיר</span><span class="sxs-lookup"><span data-stu-id="f8065-126">Senior Systems Engineer</span></span>|<span data-ttu-id="f8065-127">Contoso US</span><span class="sxs-lookup"><span data-stu-id="f8065-127">Contoso US</span></span>|<span data-ttu-id="f8065-128">שעה</span><span class="sxs-lookup"><span data-stu-id="f8065-128">Hour</span></span>| <span data-ttu-id="f8065-129">150</span><span class="sxs-lookup"><span data-stu-id="f8065-129">150</span></span>| <span data-ttu-id="f8065-130">USD</span><span class="sxs-lookup"><span data-stu-id="f8065-130">USD</span></span>|


<span data-ttu-id="f8065-131">כאשר אתה מבטל את הכותרת הסטנדרטית בתור **ממד התמחור**, ומנגנון התמחור מחפש מחיר, הוא ישתמש רק בערך של **היחידה הארגונית** מתוך הקשר הקלט.</span><span class="sxs-lookup"><span data-stu-id="f8065-131">When you turn off **Standard Title** as the pricing dimension, and the pricing engine searches for a price, it will only use the **Org Unit** value from the input context.</span></span> <span data-ttu-id="f8065-132">אם **היחידה הארגונית** של הקשר הקלט היא "Contoso US", התוצאה תהיה לא דטרמיניסטית כיוון ששתי השורות יתאימו.</span><span class="sxs-lookup"><span data-stu-id="f8065-132">If the **Org Unit** of the input context is “Contoso US”, the result will be non-deterministic because both the rows will match.</span></span> <span data-ttu-id="f8065-133">כדי להימנע מתרחיש זה, בעת יצירת רשומות **מחיר תפקיד**, המערכת מאמתת ששילוב הממדים הוא ייחודי.</span><span class="sxs-lookup"><span data-stu-id="f8065-133">To avoid this scenario, when you create **Role Price** records, the system validates that the combination of dimensions is unique.</span></span> <span data-ttu-id="f8065-134">אם הממד מבוטל לאחר שנוצרו רשומות **מחיר התפקיד**, ניתן להפר אילוץ זה.</span><span class="sxs-lookup"><span data-stu-id="f8065-134">If the dimension is turned off after the **Role Price** records are created, this constraint can be violated.</span></span> <span data-ttu-id="f8065-135">לפיכך, לפני ביטול הממד, עליך למחוק את כל השורות של **מחיר תפקיד** ו **ייקור מחיר תפקיד** שערך ממד זה מאוכלס אצלן.</span><span class="sxs-lookup"><span data-stu-id="f8065-135">Therefore, it is required that before you turn off a dimension, you delete all **Role Price** and **Role Price Markup** rows that have that dimension value populated.</span></span>
