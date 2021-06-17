---
title: הגדרת מחירון מכירות
description: נושא זה מספק מידע על מחירוני מוצרים לצורך תמחור פרויקט.
author: rumant
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
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
ms.openlocfilehash: 712dedb6766ff36181e261a66f3af99469449574
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004892"
---
# <a name="set-up-a-sales-price-list"></a><span data-ttu-id="91831-103">הגדרת מחירון מכירות</span><span class="sxs-lookup"><span data-stu-id="91831-103">Set up a sales price list</span></span>

<span data-ttu-id="91831-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="91831-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="91831-105">עבור הצעות מחיר וחוזים של פרויקט, למחירון פרויקט יש תבנית עקיפת מחיר שונה מאשר מחירון מוצר.</span><span class="sxs-lookup"><span data-stu-id="91831-105">For project quotes and contracts, a project price list has a different price override pattern than a product price list.</span></span> <span data-ttu-id="91831-106">בשורה בהצעת מחיר המבוססת על קטלוג מוצרים, באפשרותך לעקוף את המחיר לתפקידים ולקטגוריות ישירות בשורה בהצעת המחיר, משום שכל שורה בהצעת מחיר מצביעה על פריט קטלוג אחד בדיוק.</span><span class="sxs-lookup"><span data-stu-id="91831-106">On a product catalog–based quote line, you can override the price to roles and categories directly on the quote line, because each quote line points to exactly one catalog item.</span></span> <span data-ttu-id="91831-107">עם זאת, בשורה בהצעת מחיר המבוססת על פרויקט, אין באפשרותך לעקוף את המחיר לתפקידים ולקטגוריות ישירות בשורה בהצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="91831-107">However, on a project-based quote line, you can't override the price to roles and categories directly on the quote line.</span></span> <span data-ttu-id="91831-108">אתה יכול להשתמש במחירון הפרויקט כדי לעבוד עם שני דפוסי החלפה שונים.</span><span class="sxs-lookup"><span data-stu-id="91831-108">You can use the project price list to work with the two distinct override patterns.</span></span>

> [!NOTE]
> <span data-ttu-id="91831-109">מומלץ שיהיה לך מחירון נפרד עבור משאבי הפרויקט שלך ועבור פריטי הקטלוג, בשל ההבדלים באופן הפעולה בין השניים כאשר אתה עוקף תמחור.</span><span class="sxs-lookup"><span data-stu-id="91831-109">We recommend that you have a separate price list for your project resources and your catalog items, because of the behavior differences between the two when you override pricing.</span></span>

<span data-ttu-id="91831-110">לכל אחת מהיישויות הבאות יכול להיות מחירון מכירות משויך אחד או יותר עבור תמחור פרויקט:</span><span class="sxs-lookup"><span data-stu-id="91831-110">Each of the following entities can have one or more associated sales price lists for project pricing:</span></span>

- <span data-ttu-id="91831-111">לקוח (תיק לקוח)</span><span class="sxs-lookup"><span data-stu-id="91831-111">Customer (account)</span></span> 
- <span data-ttu-id="91831-112">הזדמנות</span><span class="sxs-lookup"><span data-stu-id="91831-112">Opportunity</span></span> 
- <span data-ttu-id="91831-113">הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="91831-113">Quote</span></span> 
- <span data-ttu-id="91831-114">חוזה הפרויקט</span><span class="sxs-lookup"><span data-stu-id="91831-114">Project Contract</span></span>

<span data-ttu-id="91831-115">השיוך של ישויות אלה למחירון מצוין על-ידי המחירונים של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="91831-115">The association of these entities with a price list is indicated by the project price lists.</span></span> <span data-ttu-id="91831-116">באפשרותך לשייך מחירון אחד או יותר לישויות המכירות 'לקוח', 'הזדמנות', 'הצעת מחיר' ו'חוזה פרויקט'.</span><span class="sxs-lookup"><span data-stu-id="91831-116">You can associate one or more price lists with the Customer, Opportunity, Quote, and Project Contract sales entities.</span></span>

<span data-ttu-id="91831-117">מחירון פרויקט המהווה ברירת מחדל אינו מוזן באופן אוטומטי ברשומת לקוח.</span><span class="sxs-lookup"><span data-stu-id="91831-117">A default project price list isn't automatically entered on a customer record.</span></span> <span data-ttu-id="91831-118">עם זאת, באפשרותך לצרף באופן ידני מחירון פרויקט לרשומת הלקוח.</span><span class="sxs-lookup"><span data-stu-id="91831-118">However, you can manually attach a project price list to the customer record.</span></span> <span data-ttu-id="91831-119">עם זאת, עליך לצרף באופן ידני מחירון פרויקט רק כאשר יש לך הסכם תמחור מותאם אישית עם הלקוח.</span><span class="sxs-lookup"><span data-stu-id="91831-119">Nevertheless, you should manually attach a project price list only when you have a custom pricing agreement with the customer.</span></span> 

<span data-ttu-id="91831-120">כאשר מחירון פרויקט מצורף לישות מכירות, מבוצע אימות של המידע הבא:</span><span class="sxs-lookup"><span data-stu-id="91831-120">When a project price list is attached to a sales entity, the following information is validated:</span></span>

- <span data-ttu-id="91831-121">למחירון יש הקשר של **מכירות**.</span><span class="sxs-lookup"><span data-stu-id="91831-121">The price list has a context of **Sales**.</span></span> 
- <span data-ttu-id="91831-122">מטבע המחירון מתאים למטבע הלקוח.</span><span class="sxs-lookup"><span data-stu-id="91831-122">The price list currency matches the customer currency.</span></span> 

<span data-ttu-id="91831-123">בחוזה של פרויקט, נעשה שימוש בסדר העדיפויות הבא כדי להגדיר באופן אוטומטי מחירונים קשורים של פרויקט:</span><span class="sxs-lookup"><span data-stu-id="91831-123">On a project contract, the following order of precedence is used to automatically set related project price lists:</span></span>

1. <span data-ttu-id="91831-124">הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="91831-124">Quote</span></span>
2. <span data-ttu-id="91831-125">הזדמנות</span><span class="sxs-lookup"><span data-stu-id="91831-125">Opportunity</span></span>
3. <span data-ttu-id="91831-126">לקוח</span><span class="sxs-lookup"><span data-stu-id="91831-126">Customer</span></span> 
4. <span data-ttu-id="91831-127">הגדרות כלליות</span><span class="sxs-lookup"><span data-stu-id="91831-127">Global settings</span></span> 

<span data-ttu-id="91831-128">כאשר מחירון של פרויקט מוזן כברירת מחדל, המערכת מאמתת שהמטבע תואם למטבע הלקוח ושהמחירונים המהווים ברירת מחדל שהוזנו הם בעלי הקשר של **מכירות**.</span><span class="sxs-lookup"><span data-stu-id="91831-128">When a project price list is entered by default, the system validates that the currency matches the customer’s currency, and that the default price lists that have been entered have a context of **Sales**.</span></span>

<span data-ttu-id="91831-129">באפשרותך לשייך מחירוני פרויקט מרובים לישויות 'לקוח', 'הזדמנות', 'הצעת מחיר' ו'חוזה פרויקט'.</span><span class="sxs-lookup"><span data-stu-id="91831-129">You can associate multiple project price lists with the Customer, Opportunity, Quote, and Project Contract entities.</span></span> <span data-ttu-id="91831-130">יכולת זו תומכת במחירי ברירת מחדל ספציפיים לתאריך עבור חוזה פרויקט לטווח הארוך, שבו אתה עשוי לדרוש יותר ממחירון אחד עבור עדכוני מחירים המתרחשים כתוצאה מאינפלציה.</span><span class="sxs-lookup"><span data-stu-id="91831-130">This capability supports date-specific default prices for a long-running project contract, where you might require more than one price list to account for price updates that occur because of inflation.</span></span> <span data-ttu-id="91831-131">עם זאת, אם המחירונים שאתה משייך לישות 'לקוח', 'הזדמנות', 'הצעת מחיר' או 'חוזה פרויקט' הם בעלי תוקף של תאריך חופף, מחירי ברירת המחדל עשויים להיות שגויים.</span><span class="sxs-lookup"><span data-stu-id="91831-131">However, if the price lists that you associate with the Customer, Opportunity, Quote, or Project Contract entity have overlapping date effectivity, the default prices might be incorrect.</span></span> <span data-ttu-id="91831-132">לכן, עליך לוודא שמחירוני הפרויקט בעלי תוקף של תאריך חופף אינם משויכים לישויות אלה.</span><span class="sxs-lookup"><span data-stu-id="91831-132">Therefore, you should make sure that project price lists that have overlapping date effectivity aren't associated with those entities.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]