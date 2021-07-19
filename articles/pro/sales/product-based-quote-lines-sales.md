---
title: מבט כולל על שורות הצעות מחיר מבוססות מוצר - לייט
description: נושא זה מספק מידע על עבודה עם שרות הצעות מחיר מבוססות מוצר.
author: rumant
ms.date: 10/30/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: 8b904f9abd3d2505c5397906f63a5ae8ff4be41b
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 07/07/2021
ms.locfileid: "6369827"
---
# <a name="product-based-quote-lines-overview---lite"></a><span data-ttu-id="ed566-103">מבט כולל על שורות הצעות מחיר מבוססות מוצר - לייט</span><span class="sxs-lookup"><span data-stu-id="ed566-103">Product-based quote lines overview - lite</span></span>

<span data-ttu-id="ed566-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="ed566-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ed566-105">באפשרותך ליצור שורות הצעות מחיר מבוססות מוצר ב- Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="ed566-105">You can create product-based quote lines in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="ed566-106">שורות הצעת מחיר מבוססות מוצר יכולות להיווסף באופן ידיני, או שהן יכולות להיות פריטים מקטלוג המוצרים.</span><span class="sxs-lookup"><span data-stu-id="ed566-106">Product-based quote lines can be manually added, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="ed566-107">קטלוג מוצרים</span><span class="sxs-lookup"><span data-stu-id="ed566-107">Product catalog</span></span>

<span data-ttu-id="ed566-108">לכל מוצר בקטלוג מוצרים יש יחידת בברירת מחדל וקבוצת יחידות.</span><span class="sxs-lookup"><span data-stu-id="ed566-108">Each product in the product catalog has a default unit and unit group.</span></span> <span data-ttu-id="ed566-109">אם כמה מוצרים חולקים את אותה קבוצת תכונות, ניתן ליצור משפחת מוצרים שגם לה יש את התכונות האלו.</span><span class="sxs-lookup"><span data-stu-id="ed566-109">If multiple products share the same set of attributes, you can create a product family that share those attributes.</span></span> 

<span data-ttu-id="ed566-110">לדוגמה, חברה מוכרת רשיונות מנוי עבור סוגים שונים של תוכנות.</span><span class="sxs-lookup"><span data-stu-id="ed566-110">For example, a company sells subscription licenses for different kinds of software.</span></span> <span data-ttu-id="ed566-111">כל תוכנת מנוי כוללת את שתי התכונות הבאות:</span><span class="sxs-lookup"><span data-stu-id="ed566-111">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="ed566-112">מספר המשתמשים</span><span class="sxs-lookup"><span data-stu-id="ed566-112">Number of users</span></span>
- <span data-ttu-id="ed566-113">משך המנוי הנמדד בחודשים</span><span class="sxs-lookup"><span data-stu-id="ed566-113">A subscription duration measured in months</span></span>

<span data-ttu-id="ed566-114">לשמירה על סוג זה של קטלוג, צור משפחת מוצרים בשם **תוכנה במנוי**, והוסף אליה את מספר המשתמשים ומשך המנוי כתכונות.</span><span class="sxs-lookup"><span data-stu-id="ed566-114">To maintain this type of catalog, create a product family named **Subscription Software** and add the number of users and the subscription duration as attributes.</span></span> <span data-ttu-id="ed566-115">לאחר מכן, אפשר להוסיף מוצרים בודדים למשפחת המוצרים **תוכנה במנוי**.</span><span class="sxs-lookup"><span data-stu-id="ed566-115">Next, you can add individual products to the **Subscription Software** product family.</span></span>

## <a name="add-product-catalog-items-to-a-project-quote"></a><span data-ttu-id="ed566-116">הוספת פריטים מקטלוג מוצרים להצעת מחיר של פרויקט</span><span class="sxs-lookup"><span data-stu-id="ed566-116">Add product catalog items to a project quote</span></span>

<span data-ttu-id="ed566-117">בדפים **הצעת מחיר של פרויקט** ו **חוזה פרויקט** יש מקטעים עבור שורות מבוססות פרויקט ושורות מבוססות מוצר.</span><span class="sxs-lookup"><span data-stu-id="ed566-117">The **Project Quote** and **Project Contract** pages have sections for project-based lines and product-based lines.</span></span> <span data-ttu-id="ed566-118">עבור שורות מבוססות מוצר, הרשימה הנפתחת בשורת הצעת המחיר או בסעיף החוזה של הפרויקט כוללת את כל המוצרים והיחידות במחירון המוצר.</span><span class="sxs-lookup"><span data-stu-id="ed566-118">For product-based lines, the drop-down list on the quote line or project contract line includes all the products and units in the product price list.</span></span> <span data-ttu-id="ed566-119">באפשרותך גם להוסיף מוצרים שאינם חלק ממחירון המוצר.</span><span class="sxs-lookup"><span data-stu-id="ed566-119">You can also add products that aren't part of the product price list.</span></span>

<span data-ttu-id="ed566-120">בנוסף, תוכל לבחור מוצרים ממחירונים אחרים, או ישירות מקטלוג המוצרים.</span><span class="sxs-lookup"><span data-stu-id="ed566-120">Additionally, you can select products from other price lists or directly from the product catalog.</span></span> <span data-ttu-id="ed566-121">בעת בחירת מוצרים ישירות מקטלוג המוצרים, המחירון בברירת המחדל של מוצר זה ישמש לקבלת מחיר המכירה של המוצר.</span><span class="sxs-lookup"><span data-stu-id="ed566-121">When you select products directly from a product catalog, the default price list of that product is used to get the product's sales price.</span></span> <span data-ttu-id="ed566-122">אם לא מוגדר מחירון בברירת מחדל, המחיר מוגדר כאפס (0).</span><span class="sxs-lookup"><span data-stu-id="ed566-122">If a default price list isn't set, the price is set to zero (0).</span></span>

<span data-ttu-id="ed566-123">כאשר שורת הצעת מחיר מבוססת על קטלוג מוצרים, באפשרותך לעקוף את מחיר המכירה ישירות בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="ed566-123">When a quote line is based on a product catalog, you can override the sales price directly on the quote line.</span></span> <span data-ttu-id="ed566-124">שורת הצעת מחיר בשדה **תמחור** עם שני ערכים זמינים:</span><span class="sxs-lookup"><span data-stu-id="ed566-124">A quote line in **Pricing** field with two available values:</span></span>

- <span data-ttu-id="ed566-125">**עקוף את התמחור**</span><span class="sxs-lookup"><span data-stu-id="ed566-125">**Override Pricing**</span></span>
- <span data-ttu-id="ed566-126">**השתמש בברירת מחדל**</span><span class="sxs-lookup"><span data-stu-id="ed566-126">**Use Default**</span></span>

<span data-ttu-id="ed566-127">אם תבחר באפשרות **עקוף את התמחור** מחיר ברירת המחדל לא יוגדר.</span><span class="sxs-lookup"><span data-stu-id="ed566-127">If you select **Override Pricing**, the default price isn't set.</span></span> <span data-ttu-id="ed566-128">במקום זאת, עליך להזין מחיר עבור המוצר בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="ed566-128">Instead, you must enter a price for the product on the quote line.</span></span> <span data-ttu-id="ed566-129">אם תבחר באפשרות **השתמש בברית המחדל**, נעשה שימוש במחיר המכירה המוגדר כברירת מחדל והשדה נעול לעריכה.</span><span class="sxs-lookup"><span data-stu-id="ed566-129">If you select **Use Default**, the default sales price is used and the field is locked for editing.</span></span>

<span data-ttu-id="ed566-130">מחירי מכירה ברירת מחדל מוזנים בשורות מבוססות מוצר של הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="ed566-130">Default sales prices are entered on the product-based lines of a quote.</span></span> <span data-ttu-id="ed566-131">אחר כך, השדה **תמחור** מוגדר כ **עקוף את התמחור** כדי שתוכל לערוך את המחיר ברירת המחדל בשורות הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="ed566-131">The **Pricing** field is then set to **Override Pricing** so that you can edit the default price on the quote lines.</span></span> <span data-ttu-id="ed566-132">זוהי עקיפה ספציפית של Project Operations לאופן הפעולה של שורות מבוססות המוצר ב-Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="ed566-132">This is a Project Operations-specific override to the product-based lines behavior in Dynamics 365 Sales.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]