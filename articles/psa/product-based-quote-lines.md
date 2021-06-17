---
title: שורות הצעת מחיר מבוססות-מוצר
description: נושא זה מספק מידע על שורות הצעת מחיר מבוססות מוצר.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 1bd789f4ee4d5b4603093be24aa25addafa9e8e8
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998502"
---
# <a name="product-based-quote-lines"></a><span data-ttu-id="5d3cc-103">שורות הצעת מחיר מבוססות-מוצר</span><span class="sxs-lookup"><span data-stu-id="5d3cc-103">Product-based quote lines</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]


<span data-ttu-id="5d3cc-104">באפשרותך ליצור שורות הצעות מחיר מבוססות מוצר ב- Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-104">You can create product-based quote lines in Dynamics 365 Project Service Automation.</span></span> <span data-ttu-id="5d3cc-105">שורות הצעת מחיר מבוססות-מוצר יכולות להיות שורות "שאינן ברשימה", או שהן יכולות להיות פריטים מקטלוג המוצרים.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-105">Product-based quote lines can be "write-in" lines, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="5d3cc-106">קטלוג מוצרים</span><span class="sxs-lookup"><span data-stu-id="5d3cc-106">Product catalog</span></span>

<span data-ttu-id="5d3cc-107">המוצרים בקטלוג מוצרים של Dynamics 365 כוללים יחידה בברירת מחדל וקבוצת יחידות.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-107">The products in a Dynamics 365 product catalog have a default unit and unit group.</span></span> <span data-ttu-id="5d3cc-108">אם כמה מוצרים חולקים את אותה קבוצת תכונות, תוכל ליצור משפחת מוצרים שגם לה יש את התכונות האלו.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-108">If several products share the same set of attributes, you can create a product family that also has those attributes.</span></span> <span data-ttu-id="5d3cc-109">כל המוצרים במשפחת מוצרים אחת יורשים את אותה קבוצת תכונות.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-109">All the products in one product family inherit the same set of attributes.</span></span>

<span data-ttu-id="5d3cc-110">לדוגמה, חברה מוכרת רשיונות מנוי עבור מגוון תוכנות.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-110">For example, a company sells subscription licenses for a variety of software.</span></span> <span data-ttu-id="5d3cc-111">כל תוכנת מנוי כוללת את שתי התכונות הבאות:</span><span class="sxs-lookup"><span data-stu-id="5d3cc-111">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="5d3cc-112">מספר המשתמשים</span><span class="sxs-lookup"><span data-stu-id="5d3cc-112">Number of users</span></span> 
- <span data-ttu-id="5d3cc-113">משך המנוי (בחודשים)</span><span class="sxs-lookup"><span data-stu-id="5d3cc-113">Subscription duration (in months)</span></span>

<span data-ttu-id="5d3cc-114">דרך טובה לשמור על סוג זה של קטלוג היא לשמור משפחת מוצרים בשם **תוכנת מנוי**, וכלולים בה **מספר המשתמשים** ו **משך המנוי** כתכונות.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-114">A good way to maintain this type of catalog is to create a product family that is named **Subscription Software**, and that has **Number of users** and **Subscription duration** as attributes.</span></span> <span data-ttu-id="5d3cc-115">תוכל לאחר מכן להוסיף מוצרים בודדים, כגון **Dynamics 365 Sales** או **Dynamics 365 Field Service** למשפחת המוצרים של **תוכנת מנוי**.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-115">You can then add individual products, such as **Dynamics 365 Sales** or **Dynamics 365 Field Service** to the **Subscription Software** product family.</span></span>

## <a name="adding-product-catalog-items-to-a-project-quote"></a><span data-ttu-id="5d3cc-116">הוספת פריטים בקטלוג מוצרים להצעת מחיר של פרויקט</span><span class="sxs-lookup"><span data-stu-id="5d3cc-116">Adding product catalog items to a project quote</span></span>

<span data-ttu-id="5d3cc-117">להצעת מחיר של פרויקט ולדפי חוזה של פרויקט יש מקטעים עבור שני סוגי שורות: שורות מבוססות פרויקט ושורות מבוססות מוצר.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-117">Project quote and project contract pages have sections for two types of lines: project-based lines and product-based lines.</span></span> <span data-ttu-id="5d3cc-118">עבור שורות מבוססות מוצר, Dynamics 365 משמש להוספת פריטים מקטלוג מוצרים להצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-118">For product-based lines, Dynamics 365 is used to add items from a product catalog to a quote.</span></span> <span data-ttu-id="5d3cc-119">הרשימה הנפתחת בשורת הצעת המחיר או בסעיף החוזה של הפרויקט כוללת את כל המוצרים והיחידות במחירון המוצר שמצורף להצעת מחיר או לחוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-119">The drop-down list on the quote line or project contract line includes all the products and units in the product price list that is attached to the quote or project contract.</span></span> <span data-ttu-id="5d3cc-120">באפשרותך גם להוסיף מוצרים שאינם חלק ממחירון המוצר של הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-120">You can also add products that aren't part of quote's product price list.</span></span>

<span data-ttu-id="5d3cc-121">בנוסף, תוכל לבחור מוצרים ממחירונים אחרים, או לבחור מוצרים ישירות מקטלוג המוצרים.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-121">Additionally, you can select products from other price lists, or you can select products directly from the product catalog.</span></span> <span data-ttu-id="5d3cc-122">בעת בחירת מוצרים ישירות מקטלוג המוצרים, המחירון בברירת המחדל של מוצר זה ישמש לקבלת מחיר המכירה של המוצר.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-122">When you select products directly from a product catalog, the default price list of that product is used to get the product's sales price.</span></span> <span data-ttu-id="5d3cc-123">אם לא מוגדר מחירון בברירת מחדל, המחיר מוגדר כ-0 (אפס).</span><span class="sxs-lookup"><span data-stu-id="5d3cc-123">If a default price list isn't set, the price is set to 0 (zero).</span></span>

<span data-ttu-id="5d3cc-124">אם שורת הצעת מחיר מבוססת על קטלוג מוצרים, באפשרותך לעקוף את מחיר המכירה ישירות בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-124">If a quote line is based on a product catalog, you can override the sales price directly on the quote line.</span></span> <span data-ttu-id="5d3cc-125">שים לב, לשורת הצעת המחיר ב- Dynamics 365 יש שדה **תמחור**.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-125">Note that a quote line in Dynamics 365 has a **Pricing** field.</span></span> <span data-ttu-id="5d3cc-126">קיימים שני ערכים זמינים:</span><span class="sxs-lookup"><span data-stu-id="5d3cc-126">Two values are available:</span></span>

- <span data-ttu-id="5d3cc-127">עקוף את התמחור</span><span class="sxs-lookup"><span data-stu-id="5d3cc-127">Override pricing</span></span>  
- <span data-ttu-id="5d3cc-128">השתמש בברירת המחדל</span><span class="sxs-lookup"><span data-stu-id="5d3cc-128">Use default</span></span>

<span data-ttu-id="5d3cc-129">אם תגדיר את השדה הזה בתור **עקוף את התמחור**‏, Dynamics 365 לא קובע מחיר בברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-129">If you set this field to **Override pricing**, Dynamics 365 doesn't set a default price.</span></span> <span data-ttu-id="5d3cc-130">עליך להזין מחיר עבור המוצר בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-130">You must enter a price for the product on the quote line.</span></span> <span data-ttu-id="5d3cc-131">אם תגדיר שדה זה בתור **‏‫השתמש בברירת המחדל**‏, Dynamics 365 ישתמש במחיר המכירה שבברירת המחדל וינעל את השדה כדי למנוע עריכה.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-131">If you set this field to **Use default**, Dynamics 365 uses the default sales price and locks the field to prevent editing.</span></span>

<span data-ttu-id="5d3cc-132">לאחר התקנה של PSA, מחירי המכירות שבברירת מחדל מוזנים בשורות שמבוססות על המוצר בהצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-132">After you install PSA, default sales prices are entered on the product-based lines on a quote.</span></span> <span data-ttu-id="5d3cc-133">השדה **תמחור** מוגדר לאחר מכן בתור **עקוף את התמחור** כדי שתוכל לערוך את המחיר שבברירת המחדל בשורות של הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-133">The **Pricing** field is then set to **Override pricing** so that you can edit the default price on the quote lines.</span></span>

> ![הגדרת עקיפת תמחור](media/basic-guide-10.png)
 
## <a name="quantity-factors-for-products"></a><span data-ttu-id="5d3cc-135">גורמי כמות למוצרים</span><span class="sxs-lookup"><span data-stu-id="5d3cc-135">Quantity factors for products</span></span>

<span data-ttu-id="5d3cc-136">PSA משתמש בגורמי כמות כדי לתמוך במכירה של מוצרים מבוססי מנוי.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-136">PSA uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="5d3cc-137">עבור מוצרים מבוססי מנוי, הכמות בהצעת המחיר או בסעיף החוזה של הפרויקט מבוטאת כמספר החודשים של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-137">For subscription-based products, the quantity on the quote or project contract line is expressed as the number of user months.</span></span>

<span data-ttu-id="5d3cc-138">בדרך כלל, המחיר של תוכנת המנוי מאוחסן בקטלוג כמחיר לכל משתמש בחודש.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-138">Usually, the price of subscription software is stored in the catalog as the price per user per month.</span></span> <span data-ttu-id="5d3cc-139">אולם, תוכל להשתמש בתיאורי זמן אחרים במקום זאת.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-139">However, you can use other time descriptions instead.</span></span> <span data-ttu-id="5d3cc-140">במהלך תהליך המכירה, המחיר בשורת הצעת המחיר הוא בדרך כלל מחיר לפי משתמש, לפי חודש, בתאם למשא ומתן שנוהל על-ידי סוכן מכירות של מחלקת ה- IT.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-140">During the sales process, the price on the quote line is usually the per-user, per-month price that was negotiated and discounted by the IT sales agent.</span></span> <span data-ttu-id="5d3cc-141">לכל עסקה יש מספר שונה של משתמשים ומספר שונה של חודשי מנוי.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-141">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="5d3cc-142">הכמות המשמשת לחישוב הסכום בשורת הצעת המחיר היא תוצר של מספר המשתמשים ומספר חודשי המנוי.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-142">The quantity that is used to compute the amount of the quote line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="5d3cc-143">כדי לתמוך בסוג זה של מכירה, PSA הציג את המושג של גורמי כמות.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-143">To support this type of sale, PSA introduced the concept of quantity factors.</span></span> <span data-ttu-id="5d3cc-144">גורמי כמות מסתמכים על תכונות המוצר ב- Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-144">Quantity factors rely on the product attributes in Dynamics 365.</span></span> <span data-ttu-id="5d3cc-145">בעת קביעת תצורה של מאפיינים מסוימים עבור מוצר, PSA מאפשר לך לסמן קבוצת משנה של מאפיינים אלה, או את כל המאפיינים, כגורמי כמות.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-145">When you configure specific properties for a product, PSA lets you flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="5d3cc-146">PSA מוודא שרק מאפיינים מספריים או מאפייני מוצר בעלי סוג נתונים מספרי מסומנים כגורמי כמות.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-146">PSA validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="5d3cc-147">כאשר למוצר מוגדרים גורמי כמות והוא מתווסף לשורת הצעת מחיר, השדה **כמות** בשורת הצעת מחיר הופך לשדה לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-147">When a product that quantity factors are configured for is added to a quote line, the **Quantity** field on the quote line becomes a read-only field.</span></span> <span data-ttu-id="5d3cc-148">לאחר הזנת ערכים עבור מאפייני מוצר שהם גורמי כמות, PSA מחשב את הכמות בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-148">After you enter values for product properties that are quantity factors, PSA computes the quantity of the quote line.</span></span>

<span data-ttu-id="5d3cc-149">לדוגמה, ייתכן שב- Dynamics 365 יהיו המאפיינים הבאים:</span><span class="sxs-lookup"><span data-stu-id="5d3cc-149">For example, Dynamics 365 might have the following properties:</span></span> 

- <span data-ttu-id="5d3cc-150">**מס' המשתמשים** - מספר המשתמשים</span><span class="sxs-lookup"><span data-stu-id="5d3cc-150">**No of users** - The number of users</span></span> 
- <span data-ttu-id="5d3cc-151">**מס' החודשים** - מספר חודשי המנוי</span><span class="sxs-lookup"><span data-stu-id="5d3cc-151">**No of Months** - The number of subscription months</span></span>
- <span data-ttu-id="5d3cc-152">**SKU של מוצר**</span><span class="sxs-lookup"><span data-stu-id="5d3cc-152">**Product SKU**</span></span> 

<span data-ttu-id="5d3cc-153">ניתן לסמן את המאפיין **מס' המשתמשים** ואת המאפיין **מס' החודשים** כגורמי כמות על-ידי עריכת המאפיינים של שורת המוצר.</span><span class="sxs-lookup"><span data-stu-id="5d3cc-153">Tne **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span> 

> ![סימון 'מס' משתמשים' ו'מס' החודשים' כגורמי כמות.](media/basic-guide-11.png)
 


[!INCLUDE[footer-include](../includes/footer-banner.md)]