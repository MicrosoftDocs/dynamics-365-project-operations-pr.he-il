---
title: מבט כולל על סעיפי חוזה מבוססי מוצר - לייט
description: נושא זה מספק מידע על סעיפי חוזה מבוססי מוצר.
author: rumant
ms.date: 10/07/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: 8464eefbce9ba266360e10039e2a0be78982d8fa
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 07/07/2021
ms.locfileid: "6369737"
---
# <a name="product-based-contract-lines-overview---lite"></a><span data-ttu-id="510c6-103">מבט כולל על סעיפי חוזה מבוססי מוצר - לייט</span><span class="sxs-lookup"><span data-stu-id="510c6-103">Product-based contract lines overview - lite</span></span>

<span data-ttu-id="510c6-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="510c6-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="510c6-105">באפשרותך ליצור שורות חוזה מבוססות מוצר ב- Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="510c6-105">You can create product-based contract lines in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="510c6-106">סעיפי חוזה מבוססי-מוצר יכולים להיות סעיפים שנוצרו ידנית, או פריטים מקטלוג המוצרים.</span><span class="sxs-lookup"><span data-stu-id="510c6-106">Product-based contract lines can be manually created lines, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="510c6-107">קטלוג מוצרים</span><span class="sxs-lookup"><span data-stu-id="510c6-107">Product catalog</span></span>

<span data-ttu-id="510c6-108">המוצרים בקטלוג מוצרים כוללים יחידה בברירת מחדל וקבוצת יחידות.</span><span class="sxs-lookup"><span data-stu-id="510c6-108">The products in the product catalog have a default unit and unit group.</span></span> <span data-ttu-id="510c6-109">אם כמה מוצרים חולקים את אותה קבוצת תכונות, תוכל ליצור משפחת מוצרים שגם לה יש את התכונות האלו.</span><span class="sxs-lookup"><span data-stu-id="510c6-109">If several products share the same set of attributes, you can create a product family that also has those attributes.</span></span> <span data-ttu-id="510c6-110">כל המוצרים במשפחת מוצרים אחת יורשים את אותה קבוצת תכונות.</span><span class="sxs-lookup"><span data-stu-id="510c6-110">All the products in one product family inherit the same set of attributes.</span></span>

<span data-ttu-id="510c6-111">לדוגמה, חברה מוכרת רשיונות מנוי עבור סוגים שונים של תוכנות.</span><span class="sxs-lookup"><span data-stu-id="510c6-111">For example, a company sells subscription licenses for different kinds of software.</span></span> <span data-ttu-id="510c6-112">כל תוכנת מנוי כוללת את שתי התכונות הבאות:</span><span class="sxs-lookup"><span data-stu-id="510c6-112">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="510c6-113">מספר המשתמשים</span><span class="sxs-lookup"><span data-stu-id="510c6-113">Number of users</span></span>
- <span data-ttu-id="510c6-114">משך המנוי (בחודשים)</span><span class="sxs-lookup"><span data-stu-id="510c6-114">Subscription duration (in months)</span></span>

<span data-ttu-id="510c6-115">כדי לשמור על קטלוג מסוג זה, צור משפחת מוצרים בשם **תוכנה עם מנוי**.</span><span class="sxs-lookup"><span data-stu-id="510c6-115">To maintain this type of catalog, create a product family that is named **Subscription Software**.</span></span> <span data-ttu-id="510c6-116">הוסף את התכונות **מספר משתמשים** ו **משך המנוי** למשפחת המוצרים.</span><span class="sxs-lookup"><span data-stu-id="510c6-116">Add the attributes, **Number of users** and **Subscription duration** to the product family.</span></span> <span data-ttu-id="510c6-117">לאחר מכן, הוסף מוצרים בודדים למוצר משפחתי של **תוכנה עם מנוי**.</span><span class="sxs-lookup"><span data-stu-id="510c6-117">Then, add individual products to the **Subscription Software** product family.</span></span>

## <a name="add-product-catalog-items-to-a-project-contract"></a><span data-ttu-id="510c6-118">הוסף פריטים בקטלוג מוצרים לחוזה של פרויקט</span><span class="sxs-lookup"><span data-stu-id="510c6-118">Add product catalog items to a project Contract</span></span>

<span data-ttu-id="510c6-119">בחוזי פרויקט יש קטעים לשני סוגים של סעיפים, מבוססי פרויקטים ומבוססי מוצרים.</span><span class="sxs-lookup"><span data-stu-id="510c6-119">Project contracts have sections for two types of lines, project-based and product-based.</span></span> <span data-ttu-id="510c6-120">סעיפים מבוססי מוצרים כוללים את כל המוצרים והיחידות במחירון המוצרים בחוזה.</span><span class="sxs-lookup"><span data-stu-id="510c6-120">Product-based lines include all of the products and units in the product price list on the contract.</span></span> <span data-ttu-id="510c6-121">ניתן להוסיף מוצרים שאינם חלק ממחירון המוצרים של החוזה.</span><span class="sxs-lookup"><span data-stu-id="510c6-121">Products that aren't part of contract's product price list can be added.</span></span>

<span data-ttu-id="510c6-122">ניתן לבחור מוצרים ממחירונים אחרים, או ישירות מקטלוג המוצרים.</span><span class="sxs-lookup"><span data-stu-id="510c6-122">You can select products from other price lists, or directly from the product catalog.</span></span> <span data-ttu-id="510c6-123">בעת בחירת מוצרים ישירות מקטלוג המוצרים, המחירון בברירת המחדל של מוצר זה ישמש עבור מחיר המכירה של המוצר.</span><span class="sxs-lookup"><span data-stu-id="510c6-123">When you select products directly from a product catalog, the default price list of that product is used for the product's sales price.</span></span> <span data-ttu-id="510c6-124">אם לא מוגדר מחירון בברירת מחדל, המחיר מוגדר כ-0 (אפס).</span><span class="sxs-lookup"><span data-stu-id="510c6-124">If a default price list isn't set, the price is set to 0 (zero).</span></span>

<span data-ttu-id="510c6-125">אם סעיף החוזה מבוסס על קטלוג מוצרים, באפשרותך לעקוף את מחיר המכירה ישירות בסעיף החוזה.</span><span class="sxs-lookup"><span data-stu-id="510c6-125">If a contract line is based on a product catalog, you can override the sales price directly on the line.</span></span> <span data-ttu-id="510c6-126">סעיף חוזה כולל את השדה **תמחור** עם שני הערכים:</span><span class="sxs-lookup"><span data-stu-id="510c6-126">A contract line has the **Pricing** field with the two values:</span></span>

- <span data-ttu-id="510c6-127">**עקוף את התמחור**</span><span class="sxs-lookup"><span data-stu-id="510c6-127">**Override pricing**</span></span>
- <span data-ttu-id="510c6-128">**השתמש בברירת המחדל**</span><span class="sxs-lookup"><span data-stu-id="510c6-128">**Use default**</span></span>

<span data-ttu-id="510c6-129">אם תגדיר את השדה **תמחור** שיהיה **תמחור ידני**, מחיר ברירת המחדל לא מוגדר.</span><span class="sxs-lookup"><span data-stu-id="510c6-129">If you set the **Pricing** field to **Override pricing**, the default price isn't set.</span></span> <span data-ttu-id="510c6-130">הזן מחיר עבור המוצר בסעיף החוזה.</span><span class="sxs-lookup"><span data-stu-id="510c6-130">Enter a price for the product on the contract line.</span></span> <span data-ttu-id="510c6-131">אם אתה מגדיר את השדה **השתמש בברית המחדל**, נעשה שימוש במחיר המכירה המוגדר כברירת מחדל ולא ניתן לערוך את השדה.</span><span class="sxs-lookup"><span data-stu-id="510c6-131">If you set the field to **Use default**, the default sales price is used and the field can't be edited.</span></span>

<span data-ttu-id="510c6-132">לאחר התקנה של Project Operations, מחירי המכירות שבברירת מחדל מוזנים בשורות שמבוססות על המוצר בחוזה.</span><span class="sxs-lookup"><span data-stu-id="510c6-132">After you install Project Operations, default sales prices are entered on the product-based lines on a contract.</span></span> <span data-ttu-id="510c6-133">השדה **תמחור** מוגדר **עקוף את התמחור** כדי שתוכל לערוך את המחיר שבברירת המחדל בסעיפי החוזה.</span><span class="sxs-lookup"><span data-stu-id="510c6-133">The **Pricing** field is set to **Override pricing** so that you can edit the default price on the contract lines.</span></span> <span data-ttu-id="510c6-134">זוהי עקיפה ספציפית ל- Project Operations להתנהגות של סעיפים מבוססי מוצר ב- Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="510c6-134">This is a Project Operations-specific override to product-based lines behavior in Dynamics 365 Sales.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]