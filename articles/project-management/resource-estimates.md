---
title: הערכות משאבים
description: נושא זה מספק מידע על אופן החישוב של הערכות משאבים ב-Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 2ebde2b3c5bcfb5faa02ee476065ac34b1953432
ms.sourcegitcommit: f255b2cbf290973ce62fe2c1c121bd1df15a7392
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/01/2020
ms.locfileid: "3928570"
---
# <a name="resource-estimates"></a><span data-ttu-id="4a51b-103">הערכות משאבים</span><span class="sxs-lookup"><span data-stu-id="4a51b-103">Resource estimates</span></span>

<span data-ttu-id="4a51b-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="4a51b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="4a51b-105">הערכות המשאבים מגיעות ממאמץ שמחולק ליחידות זמן עבודה המוגדר במבנה התפלגות העבודה יחד עם ממדי תמחור ישימים.</span><span class="sxs-lookup"><span data-stu-id="4a51b-105">Resource estimates come from time-phased effort that is defined in the work breakdown structure along with applicable pricing dimensions.</span></span> <span data-ttu-id="4a51b-106">בדרך כלל, החישוב הוא **תעריף לשעה לכל תפקיד x שעות.**</span><span class="sxs-lookup"><span data-stu-id="4a51b-106">Typically, the calculation is **rate/hr for each role x hours.**</span></span> <span data-ttu-id="4a51b-107">המאמץ שמחולק ליחידות זמן עבודה של כל משאב נשמר ברשומת הקצאת המשאבים.</span><span class="sxs-lookup"><span data-stu-id="4a51b-107">The time-phased effort for each resource is stored in the resource assignment record.</span></span> <span data-ttu-id="4a51b-108">התמחור נשמר במחירון שהוגדר מראש.</span><span class="sxs-lookup"><span data-stu-id="4a51b-108">The pricing is stored in a pre-defined price list.</span></span> <span data-ttu-id="4a51b-109">המרת יחידות מיושמת על סמך המחירון הרלוונטי.</span><span class="sxs-lookup"><span data-stu-id="4a51b-109">Unit conversion is applied based on the applicable price list.</span></span>

![הערכות משאבים](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a><span data-ttu-id="4a51b-111">ברירות מחדל של מחיר עלות ושל מטבע עלות</span><span class="sxs-lookup"><span data-stu-id="4a51b-111">Default cost price and cost currency</span></span>

<span data-ttu-id="4a51b-112">מחירי העלות מוגדרים כברירת מחדל מהיחידה הארגונית.</span><span class="sxs-lookup"><span data-stu-id="4a51b-112">Cost prices are defaulted from the Organizational Unit.</span></span>

## <a name="default-bill-rate-and-sales-currency"></a><span data-ttu-id="4a51b-113">ברירות מחדל של תעריף חיוב ושל מטבע מכירות</span><span class="sxs-lookup"><span data-stu-id="4a51b-113">Default bill rate and sales currency</span></span>

<span data-ttu-id="4a51b-114">מחירי מכירה מוחלים פעם אחת בכל עסקה.</span><span class="sxs-lookup"><span data-stu-id="4a51b-114">Sales prices are applied once per deal.</span></span> <span data-ttu-id="4a51b-115">ההירארכיה לברירת המחדל של מחירון המכירה היא כדלקמן:</span><span class="sxs-lookup"><span data-stu-id="4a51b-115">The hierarchy for sale price list defaulting is as follows:</span></span>

1. <span data-ttu-id="4a51b-116">הארגון</span><span class="sxs-lookup"><span data-stu-id="4a51b-116">Organization</span></span>
2. <span data-ttu-id="4a51b-117">לקוח</span><span class="sxs-lookup"><span data-stu-id="4a51b-117">Customer</span></span>
3. <span data-ttu-id="4a51b-118">הצעת מחיר / חוזה</span><span class="sxs-lookup"><span data-stu-id="4a51b-118">Quote/contract</span></span>
