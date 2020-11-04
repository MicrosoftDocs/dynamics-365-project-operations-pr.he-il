---
title: הזמנות רכש לפרויקט
description: מאמר זה מתאר את השיטות השונות שבהן תוכל להשתמש כדי ליצור הזמנות רכש לפרויקט. השיטה שבה תשתמש תלויה במטרה של הזמנת הרכש ומתי יבוצעו הצריכה והחיוב של הפריטים שנרכשו לפרויקט.
author: Yowelle
manager: AnnBe
ms.date: 09/14/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 83972
ms.assetid: 247e4d72-610b-4fa5-9873-601ed0f4b2d6
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: bd891aec5bcab66c5801a5d9ca8abbbf632d662d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077296"
---
# <a name="purchase-orders-for-a-project"></a><span data-ttu-id="ec9fb-104">הזמנות רכש לפרויקט</span><span class="sxs-lookup"><span data-stu-id="ec9fb-104">Purchase orders for a project</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="ec9fb-105">מאמר זה מתאר את השיטות השונות שבהן תוכל להשתמש כדי ליצור הזמנות רכש לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-105">This article describes the various methods that you can use to create purchase orders for a project.</span></span> <span data-ttu-id="ec9fb-106">השיטה שבה תשתמש תלויה במטרה של הזמנת הרכש ומתי יבוצעו הצריכה והחיוב של הפריטים שנרכשו לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-106">The method that you use depends on the purpose of the purchase order, and when the purchased items are consumed and charged to a project.</span></span>

### <a name="methods-for-creating-a-purchase-order"></a><span data-ttu-id="ec9fb-107">שיטות ליצירת הזמנת רכש</span><span class="sxs-lookup"><span data-stu-id="ec9fb-107">Methods for creating a purchase order</span></span>

<span data-ttu-id="ec9fb-108">באפשרותך להשתמש באחת מהשיטות הבאות כדי ליצור הזמנת רכש בניהול פרויקטים וחשבונאות.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-108">You can use one of the following methods to create a purchase order in Project management and accounting.</span></span> <span data-ttu-id="ec9fb-109">מטרת הזמנת הרכש קובעת מתי נצרכת הזמנת הרכש, ולפיכך מתי מחויבים פריטים בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-109">The purpose of the purchase order determines when the purchase order is consumed and, therefore, when items are charged to a project.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="ec9fb-110">שיטה</span><span class="sxs-lookup"><span data-stu-id="ec9fb-110">Method</span></span></th>
<th><span data-ttu-id="ec9fb-111">מטרה</span><span class="sxs-lookup"><span data-stu-id="ec9fb-111">Purpose</span></span></th>
<th><span data-ttu-id="ec9fb-112">צריכת פריטים</span><span class="sxs-lookup"><span data-stu-id="ec9fb-112">Consumption of items</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="ec9fb-113">צור הזמנת רכש באופן ישיר מפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-113">Create a purchase order directly from a project.</span></span></td>
<td><span data-ttu-id="ec9fb-114">השתמש בשיטה זו כדי לרכוש פריטים מספק חיצוני לצריכה בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-114">Use this method to purchase items from an external vendor for consumption on a project.</span></span> <span data-ttu-id="ec9fb-115">ניתן ליצור את הזמנת הרכש בשתי דרכים:</span><span class="sxs-lookup"><span data-stu-id="ec9fb-115">You can create the purchase order in two ways:</span></span>
<ul>
<li><span data-ttu-id="ec9fb-116">מהפרויקט עצמו.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-116">From the project itself.</span></span> <span data-ttu-id="ec9fb-117">במקרה כזה, הפרויקט כבר מוגדר להזמנת הרכש.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-117">In this case, the project is already defined for the purchase order.</span></span></li>
<li><span data-ttu-id="ec9fb-118">על ידי ניווט להזמנת הרכש של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-118">By navigating to the project purchase order.</span></span> <span data-ttu-id="ec9fb-119">עליך לבחור גם את הספק וגם את הפרויקט שעבורו תיווצר הזמנת הרכש.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-119">You must select both the vendor and the project to create the purchase order for.</span></span></li>
</ul></td>
<td><span data-ttu-id="ec9fb-120">פריטים נצרכים כאשר חשבונית הספק מתעדכנת.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-120">Items are consumed when the vendor invoice is updated.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="ec9fb-121">צור הזמנת רכש מהזמנת מכירות.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-121">Create a purchase order from a sales order.</span></span></td>
<td><span data-ttu-id="ec9fb-122">השתמש בשיטה זו כדי לרכוש פריטים בעת יצירת הזמנת מכירות מפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-122">Use this method to purchase items when you create a sales order from a project.</span></span></td>
<td><span data-ttu-id="ec9fb-123">פריטים נצרכים כאשר מופקת חשבונית עבור הזמנת המכירות ללקוח.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-123">Items are consumed when the sales order is invoiced to the customer.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="ec9fb-124">צור הזמנת רכש מפריט נדרש.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-124">Create a purchase order from an item requirement.</span></span></td>
<td><span data-ttu-id="ec9fb-125">השתמש בשיטה זו כדי לרכוש פריטים בעת יצירת פריט נדרש מפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-125">Use this method to purchase items when you create an item requirement from a project.</span></span></td>
<td><span data-ttu-id="ec9fb-126">פריטים נצרכים בעת עדכון תעודת משלוח לפריט נדרש.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-126">Items are consumed when the item requirement packing slip is updated.</span></span></td>
</tr>
</tbody>
</table>

> [!NOTE] 
> <span data-ttu-id="ec9fb-127">בעת עדכון חשבונית הספק או תעודת המשלוח, תתבקש לעדכן את תעודת המשלוח בפריט הנדרש.</span><span class="sxs-lookup"><span data-stu-id="ec9fb-127">When you update the vendor invoice or packing slip, you're prompted to update the packing slip on the item requirement.</span></span>

<span data-ttu-id="ec9fb-128">לקבלת מידע נוסף, ראה [קבלת פריטים בהזמנת רכש מפריט נדרש](tasks/receive-items-purchase-order-item-requirement.md).</span><span class="sxs-lookup"><span data-stu-id="ec9fb-128">For more information, see [Receive items on purchase order from item requirement](tasks/receive-items-purchase-order-item-requirement.md).</span></span>

