---
title: מחירוני מוצרים
description: נושא זה מספק מידע על המחירונים בתמחור הקטלוג המשמש להצעות מחיר וחוזים.
author: rumant
manager: AnnBe
ms.date: 04/05/2021
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
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: e37f0bf9eef946ab4ebd658cef4e1269cbaf686d
ms.sourcegitcommit: ac90be6106592f883a0de39a75836fb40255d65a
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/09/2021
ms.locfileid: "5877491"
---
# <a name="product-price-lists"></a><span data-ttu-id="fabee-103">מחירוני מוצרים</span><span class="sxs-lookup"><span data-stu-id="fabee-103">Product price lists</span></span>

<span data-ttu-id="fabee-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="fabee-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

 <span data-ttu-id="fabee-105">ב- Project Operations, **מחירוני מוצרים** וישויות קשורות של פריט מחירון תומכות בפונקציונליות לתמחור מוצרים בשורות הצעת מחיר ובסעיפי חוזה מבוססי מוצר.</span><span class="sxs-lookup"><span data-stu-id="fabee-105">In Project Operations, **Product price lists** and related price list item entities support functionality for pricing products on product-based quote and contract lines.</span></span> <span data-ttu-id="fabee-106">עבור מוצרים המשמשים בפרויקטים, נעשה שימוש ברשומות פריטי המחירון עבור מחירוני הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="fabee-106">For products used on projects, the price list item records for project price lists are used.</span></span> 

<span data-ttu-id="fabee-107">יש להגדיר מוצרים כך שיהיו להם עלות ומחירונים בברירת מחדל בקטלוג המוצרים.</span><span class="sxs-lookup"><span data-stu-id="fabee-107">Products should be set up so that they have default cost and price lists in the product catalog.</span></span> <span data-ttu-id="fabee-108">השתמש במחיר המחירון, בעלות הסטנדרטית ובעלות השוטפת כדי לקבוע את התצורה של העלות ומחירי המחירון בברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="fabee-108">Use the list price, standard cost, and current cost to configure default cost and list prices.</span></span> <span data-ttu-id="fabee-109">מחירי המחירון בברירת מחדל משמשים בשורת הצעת מחיר או בסעיף חוזה של פרויקט רק כאשר המערכת לא מוצאת שורת מחירון עבור אותו מוצר במחירון המוצר עבור הצעת המחיר או חוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="fabee-109">The default list prices are used on a quote line or a project contract line only when the system can't find a price list line for that product in the product price list for the quote or project contract.</span></span>

<span data-ttu-id="fabee-110">ניתן לשנות את מחיר העלות בשורות של קטלוג המוצרים בין הצעות מחיר.</span><span class="sxs-lookup"><span data-stu-id="fabee-110">The cost price of product catalog lines can be changed between quotes.</span></span> <span data-ttu-id="fabee-111">יכולת זו חשובה, מכיוון שאם לא תאתר באופן מדויק את העלויות, לא תוכל לקבוע רווחים תפעוליים בהתקשרויות הקשורות לפרויקטים.</span><span class="sxs-lookup"><span data-stu-id="fabee-111">This capability is important, because if you don't accurately track costs, you can't determine operational profits on project engagements.</span></span> <span data-ttu-id="fabee-112">כברירת מחדל, העלות הסטנדרטית של מוצר תשמש כמחיר העלות.</span><span class="sxs-lookup"><span data-stu-id="fabee-112">By default, the standard cost of the product is used as the cost price.</span></span> <span data-ttu-id="fabee-113">עם זאת, ניתן לעדכן את מחיר העלות בברירת מחדל בשורת הצעת המחיר אם יש מחיר עלות שונה עבור הצעת המחיר הזו.</span><span class="sxs-lookup"><span data-stu-id="fabee-113">However, the default cost price can be updated on the quote line if there's a different cost price for that quote.</span></span>

## <a name="price-list-items"></a><span data-ttu-id="fabee-114">פריטי מחירונים</span><span class="sxs-lookup"><span data-stu-id="fabee-114">Price list items</span></span>

<span data-ttu-id="fabee-115">באפשרותך להוסיף מוצרים מקטלוג מוצרים למחירונים שונים.</span><span class="sxs-lookup"><span data-stu-id="fabee-115">You can add products from a product catalog to different price lists.</span></span> <span data-ttu-id="fabee-116">שורות במחירונים עבור מוצרים תמיד יפנו ליחידה מסוימת.</span><span class="sxs-lookup"><span data-stu-id="fabee-116">Price list lines for products always reference a specific unit.</span></span> <span data-ttu-id="fabee-117">ניתן לקבוע את תצורת התמחור עבור מוצר בפריטי מחירון כסכום מטבע.</span><span class="sxs-lookup"><span data-stu-id="fabee-117">Pricing for a product on price list items can be configured as a currency amount.</span></span> <span data-ttu-id="fabee-118">לחלופין, ניתן להגדיר אותו כפונקציה של מחיר המחירון, העלות השוטפת או העלות הסטנדרטית.</span><span class="sxs-lookup"><span data-stu-id="fabee-118">Alternatively, it can be configured as a function of the list price, current cost, or standard cost.</span></span>

<span data-ttu-id="fabee-119">פונקציונליות התמחור תומכת באפשרויות עיגול שונות כאשר מחירי המוצרים מוגדרים כפונקציה של מחיר המחירון, העלות הסטנדרטית או העלות השוטפת.</span><span class="sxs-lookup"><span data-stu-id="fabee-119">Pricing functionality supports various rounding options when product prices are configured as a function of the list price, standard cost, or current cost.</span></span> <span data-ttu-id="fabee-120">בנוסף לניצול שיטות תמחור ואפשרויות עיגול מרובות, באפשרותך לשייך רשימות של הנחות לפריטי מחירון.</span><span class="sxs-lookup"><span data-stu-id="fabee-120">In addition to taking advantage of multiple pricing methods and rounding options, you can associate discount lists with price list items.</span></span> 

 
## <a name="default-product-price-list"></a><span data-ttu-id="fabee-121">מחירון מוצרים בברירת המחדל</span><span class="sxs-lookup"><span data-stu-id="fabee-121">Default product price list</span></span>
<span data-ttu-id="fabee-122">לכל רשומת לקוח יש שדה **מחירון בברירת מחדל** שבו תוכל לציין מחירון שתואם למטבע של הלקוח.</span><span class="sxs-lookup"><span data-stu-id="fabee-122">Each customer record has a **Default Price List** field, where you can specify a price list that matches the currency of the customer.</span></span> <span data-ttu-id="fabee-123">ערך ברירת מחדל אינו מוזן באופן אוטומטי בשדה זה.</span><span class="sxs-lookup"><span data-stu-id="fabee-123">A default value isn't automatically entered in this field.</span></span> <span data-ttu-id="fabee-124">כאשר קיים הסכם תמחור מותאם אישית עם לקוח ספציפי, תוכל להשתמש בשדה זה כדי לשייך מחירון ללקוח הזה.</span><span class="sxs-lookup"><span data-stu-id="fabee-124">When a custom pricing agreement with a specific customer exists, you can use this field to associate a price list with that customer.</span></span>

<span data-ttu-id="fabee-125">הישויות 'הזדמנות', 'הצעת מחיר' ו'חוזה פרויקט' משתמשות בסדר הבא כדי להזין מחירוני מוצרים בברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="fabee-125">The Opportunity, Quote, and Project Contract entities use the following order to enter default product price lists.</span></span> <span data-ttu-id="fabee-126">אותו סדר משמש עבור מחירונים של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="fabee-126">The same order is used for project price lists.</span></span>

1.  <span data-ttu-id="fabee-127">הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="fabee-127">Quote</span></span>
2.  <span data-ttu-id="fabee-128">הזדמנות</span><span class="sxs-lookup"><span data-stu-id="fabee-128">Opportunity</span></span>
3.  <span data-ttu-id="fabee-129">לקוח</span><span class="sxs-lookup"><span data-stu-id="fabee-129">Customer</span></span>
4.  <span data-ttu-id="fabee-130">הגדרות כלליות</span><span class="sxs-lookup"><span data-stu-id="fabee-130">Global settings</span></span> 

<span data-ttu-id="fabee-131">כברירת מחדל, השדה **מוצר** בשורת הצעת מחיר מונה את כל המוצרים הפעילים במחירון המוצר של הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="fabee-131">By default, the **Product** field on the quote line lists all the active products in the product price list of the quote.</span></span> <span data-ttu-id="fabee-132">אם מוצר לא הופעל, או אם מדובר במוצר טיוטה, הוא אינו מופיע ברשימה, גם אם הוא במחירון.</span><span class="sxs-lookup"><span data-stu-id="fabee-132">If a product has been inactivated, or if it's a draft product, it isn't listed, even if it's in the price list.</span></span> 

<span data-ttu-id="fabee-133">שורות של קטלוג מוצרים מתווספות כשורות בחשבוניות בחשבונית הראשונה שנוצרת עבור חוזה פרויקט.</span><span class="sxs-lookup"><span data-stu-id="fabee-133">Product catalog lines are added as invoice lines on the first invoice that is created for a project contract.</span></span> <span data-ttu-id="fabee-134">בטיוטת חשבונית, ניתן למחוק את השורות בחשבונית הזו.</span><span class="sxs-lookup"><span data-stu-id="fabee-134">On a draft invoice, those invoice lines can be deleted.</span></span> <span data-ttu-id="fabee-135">במקרה כזה, השורות יופיעו בחשבונית העוקבת עד שהחשבונית יופקו, או עד שהחשבונית תישלח ללקוח.</span><span class="sxs-lookup"><span data-stu-id="fabee-135">In that case, the lines will appear on a subsequent invoice until they are invoiced, or until the invoice is sent to the customer.</span></span> <span data-ttu-id="fabee-136">אין באפשרותך להפיק חשבונית לכמות חלקית של שורת חשבונית מוצר.</span><span class="sxs-lookup"><span data-stu-id="fabee-136">You can't invoice a partial quantity of a product invoice line.</span></span> <span data-ttu-id="fabee-137">כאשר מפיקים חשבונית לשורות המוצר מחוזה הפרויקט, נוצרים נתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="fabee-137">When the product lines from the project contract are invoiced, actuals are created.</span></span> <span data-ttu-id="fabee-138">אולם, נתונים בפועל אלה אינם מקושרים לישות הפרויקט הקשורה.</span><span class="sxs-lookup"><span data-stu-id="fabee-138">However, those actuals aren't linked to the related project entity.</span></span> <span data-ttu-id="fabee-139">במילים אחרות, סעיפי חוזה של פרויקט שמבוסס על מוצר לא תלויים בכל שימוש מבוסס פרויקט.</span><span class="sxs-lookup"><span data-stu-id="fabee-139">In other words, product-based project contract lines are independent of any project-based use.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]
