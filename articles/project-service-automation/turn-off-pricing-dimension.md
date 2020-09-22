---
title: ביטול ממד תמחור
description: נושא זה מראה כיצד להגדיר ממדי תמחור בפתרון של Project Service.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/06/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 689e5a8d-e39a-471d-a6c4-7e2fc3bb5590
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 5cf2cd86fb1eba50c8e08b2bd624669ab0b1deb3
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751844"
---
# <a name="turn-off-a-pricing-dimension"></a><span data-ttu-id="d66a2-103">ביטול ממד תמחור</span><span class="sxs-lookup"><span data-stu-id="d66a2-103">Turn off a pricing dimension</span></span>

<span data-ttu-id="d66a2-104">ייתכן שתצטרך לסקור ולעדכן את אסטרטגיית התמחור שלך כל כמה שנים.</span><span class="sxs-lookup"><span data-stu-id="d66a2-104">You may need to review and update your pricing strategy every few years.</span></span> <span data-ttu-id="d66a2-105">כל העדכונים שאתה מבצע עשויים לדרוש ממך לבטל את ממד התמחור הקיים וליצור ממד חדש.</span><span class="sxs-lookup"><span data-stu-id="d66a2-105">Any updates you make might require that you turn off an existing pricing dimension and create a new one.</span></span> <span data-ttu-id="d66a2-106">לדוגמה, ייתכן שתמחרת בעבר לפי **תפקיד**, אבל עכשיו החלטת לתמחר לפי **ניסיון בעבודה**.</span><span class="sxs-lookup"><span data-stu-id="d66a2-106">For example, you may have previously priced by **Role**, but now you have decided to price by **Work Experience**.</span></span> <span data-ttu-id="d66a2-107">כתוצאה מכך, ייתכן שתידרש לבטל את **תפקיד** בתור ממד תמחור וליצור את **ניסיון בעבודה** בתור ממד תמחור חדש.</span><span class="sxs-lookup"><span data-stu-id="d66a2-107">This may require you to turn off **Role** as a pricing dimension and create **Work Expereince** as a new pricing dimension.</span></span> 

<span data-ttu-id="d66a2-108">ניתן לבטל ממד תמחור, אם הוא מוגדר מראש או מותאם אישית, על-ידי הגדרת השדות **חל על עלות** ו**חל על מכירות** בממד התמחור לערך **לא**.</span><span class="sxs-lookup"><span data-stu-id="d66a2-108">Turning off a pricing dimension, regardless if it is out-of-the-box or custom, can be done by setting the **Applicable to Cost** and **Applicable to Sales** fields of the Pricing Dimension to **No**.</span></span>

<span data-ttu-id="d66a2-109">עם זאת, כשתעשה זאת, ייתכן שתקבל את הודעת השגיאה הבאה.</span><span class="sxs-lookup"><span data-stu-id="d66a2-109">However, when you do this, you might receive the following error message.</span></span>

![שגיאת תהליך עסקי עלולה לקרות בעת ביטול ממד תמחור](media/Business-Process-Error.png)


<span data-ttu-id="d66a2-111">הודעת שגיאה זו מציינת שקיימות רשומות מחיר שהוגדרו קודם לכן עבור הממד שמבוטל.</span><span class="sxs-lookup"><span data-stu-id="d66a2-111">This error message indicates that there are price records that were previously set up for the dimension that is being turned off.</span></span> <span data-ttu-id="d66a2-112">כל הרשומות של **מחיר תפקיד** ו**ייקור מחיר תפקיד** המפנות לממד חייבות להימחק לפני שניתן יהיה להגדיר את ישימות הממד לערך **לא**.</span><span class="sxs-lookup"><span data-stu-id="d66a2-112">All **Role Price** and **Role Price Markup** records that refer to a dimension must be deleted before the dimension’s applicability can be to set to **No**.</span></span> <span data-ttu-id="d66a2-113">כלל זה חל על ממדי תמחור מוגדרים מראש ועל ממדי תמחור מותאמים אישית שיצרת.</span><span class="sxs-lookup"><span data-stu-id="d66a2-113">This rule applies to both out-of-the-box pricing dimensions and any custom pricing dimensions that you may have created.</span></span> <span data-ttu-id="d66a2-114">הסיבה לאימות זה היא ש- Project Service כולל אילוץ שלפיו לכל רשומת **מחיר תפקיד** חייב להיות שילוב ייחודי של ממדים.</span><span class="sxs-lookup"><span data-stu-id="d66a2-114">The reason for this validation is because Project Service has a constraint that each **Role Price** record must have a unique combination of dimensions.</span></span> <span data-ttu-id="d66a2-115">לדוגמה, במחירון הנקרא **תעריפי עלויות בארה"ב 2018**, מופיעות השורות הבאות של **מחיר תפקיד**.</span><span class="sxs-lookup"><span data-stu-id="d66a2-115">For example, on a price list called **US Cost Rates 2018**, you have the following **Role price** rows.</span></span> 

| <span data-ttu-id="d66a2-116">כותרת סטנדרטית</span><span class="sxs-lookup"><span data-stu-id="d66a2-116">Standard Title</span></span>         | <span data-ttu-id="d66a2-117">יחידה ארגונית</span><span class="sxs-lookup"><span data-stu-id="d66a2-117">Org Unit</span></span>    |<span data-ttu-id="d66a2-118">יחידה</span><span class="sxs-lookup"><span data-stu-id="d66a2-118">Unit</span></span>   |<span data-ttu-id="d66a2-119">מחיר</span><span class="sxs-lookup"><span data-stu-id="d66a2-119">Price</span></span>  |<span data-ttu-id="d66a2-120">מטבע</span><span class="sxs-lookup"><span data-stu-id="d66a2-120">Currency</span></span>  |
| -----------------------|-------------|-------|-------|----------|
| <span data-ttu-id="d66a2-121">מהנדס מערכות</span><span class="sxs-lookup"><span data-stu-id="d66a2-121">Systems Engineer</span></span>|<span data-ttu-id="d66a2-122">Contoso US</span><span class="sxs-lookup"><span data-stu-id="d66a2-122">Contoso US</span></span>|<span data-ttu-id="d66a2-123">שעה</span><span class="sxs-lookup"><span data-stu-id="d66a2-123">Hour</span></span>| <span data-ttu-id="d66a2-124">100</span><span class="sxs-lookup"><span data-stu-id="d66a2-124">100</span></span>|<span data-ttu-id="d66a2-125">USD</span><span class="sxs-lookup"><span data-stu-id="d66a2-125">USD</span></span>|
| <span data-ttu-id="d66a2-126">מהנדס מערכות בכיר</span><span class="sxs-lookup"><span data-stu-id="d66a2-126">Senior Systems Engineer</span></span>|<span data-ttu-id="d66a2-127">Contoso US</span><span class="sxs-lookup"><span data-stu-id="d66a2-127">Contoso US</span></span>|<span data-ttu-id="d66a2-128">שעה</span><span class="sxs-lookup"><span data-stu-id="d66a2-128">Hour</span></span>| <span data-ttu-id="d66a2-129">150</span><span class="sxs-lookup"><span data-stu-id="d66a2-129">150</span></span>| <span data-ttu-id="d66a2-130">USD</span><span class="sxs-lookup"><span data-stu-id="d66a2-130">USD</span></span>|


<span data-ttu-id="d66a2-131">כאשר אתה מבטל את הכותרת הסטנדרטית בתור **ממד התמחור**, ומנגנון התמחור של Project Service מחפש מחיר, הוא ישתמש רק בערך של **היחידה הארגונית** מתוך הקשר הקלט.</span><span class="sxs-lookup"><span data-stu-id="d66a2-131">When you turn off **Standard Title** as the pricing dimension, and the Project Service pricing engine searches for a price, it will only use the **Org Unit** value from the input context.</span></span> <span data-ttu-id="d66a2-132">אם **היחידה הארגונית** של הקשר הקלט היא "Contoso US", התוצאה תהיה לא דטרמיניסטית כיוון ששתי השורות יתאימו.</span><span class="sxs-lookup"><span data-stu-id="d66a2-132">If the **Org Unit** of the input context is “Contoso US”, the result will be non-deterministic because both the rows will match.</span></span> <span data-ttu-id="d66a2-133">כדי להימנע מתרחיש זה, בעת יצירת רשומות **מחיר תפקיד**, Project Service מאמת ששילוב הממדים הוא ייחודי.</span><span class="sxs-lookup"><span data-stu-id="d66a2-133">To avoid this scenario, when you create **Role Price** records, Project Service validates that the combination of dimensions is unique.</span></span> <span data-ttu-id="d66a2-134">אם הממד מבוטל לאחר שנוצרו רשומות **מחיר התפקיד**, ניתן להפר אילוץ זה.</span><span class="sxs-lookup"><span data-stu-id="d66a2-134">If the dimension is turned off after the **Role Price** records are created, this constraint can be violated.</span></span> <span data-ttu-id="d66a2-135">לפיכך, לפני ביטול הממד, עליך למחוק את כל השורות של **מחיר תפקיד** ו**ייקור מחיר תפקיד** שערך ממד זה מאוכלס אצלן.</span><span class="sxs-lookup"><span data-stu-id="d66a2-135">Therefore, it is required that before you turn off a dimension, you delete all **Role Price** and **Role Price Markup** rows that have that dimension value populated.</span></span>

