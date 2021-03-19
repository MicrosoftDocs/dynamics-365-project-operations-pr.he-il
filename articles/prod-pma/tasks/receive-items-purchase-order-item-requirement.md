---
title: קבלת פריטים בהזמנת רכש מפריט נדרש
description: נושא זה מסביר כיצד לקבל פריטים בהזמנת רכש מפריט נדרש.
author: Yowelle
manager: AnnBe
ms.date: 08/06/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage, ProjTable, ProjSalesItemReq, InventItemIdLookupSimple, PurchCreateFromSalesOrder, VendAccountItemLookup, PurchTable, PurchEditLines
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: c2083516ff929113fd6db377acfe5aeb104666dd
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288229"
---
# <a name="receive-items-on-purchase-order-from-item-requirement"></a><span data-ttu-id="ad1c8-103">קבלת פריטים בהזמנת רכש מפריט נדרש</span><span class="sxs-lookup"><span data-stu-id="ad1c8-103">Receive items on purchase order from item requirement</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="ad1c8-104">נושא זה מסביר כיצד לקבל פריטים בהזמנת רכש מפריט נדרש.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-104">This topic explains how to receive items on a purchase order from an item requirement.</span></span>

<span data-ttu-id="ad1c8-105">על ידי שימוש בפריט נדרש במקום בעסקת פריט, תוכל לתכנן מסירה ממש לפני השימוש בפועל בפריט, ליצור הזמנת רכש, לכלול את הפריט במסגרת הסכם הסחר ולכלול את הפריט הנדרש בתכנון הייצור.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-105">By using an item requirement instead of an item transaction, you can plan for delivery just before the item is actually used, create a purchase order, include the item in the trade-agreement framework, and include the item requirement in production planning.</span></span> 

<span data-ttu-id="ad1c8-106">משימה זו משתמשת בערכת נתונים של USSI.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-106">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="ad1c8-107">בחלונית הניווט, עבור אל **מודולים > ניהול פרויקטים וחשבונאות > פרויקטים > כל הפרויקטים**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-107">In the navigation pane, go to **Modules > Project management and accounting > Projects > All projects**.</span></span>
2. <span data-ttu-id="ad1c8-108">מתוך הרשימה בחר את הקישור בשורה הרצויה.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-108">In the list, select the link in the desired row.</span></span>
3. <span data-ttu-id="ad1c8-109">בחלונית הפעולות בחר **תכנון**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-109">On the Action Pane, select **Plan**.</span></span>
4. <span data-ttu-id="ad1c8-110">בחר **פריט נדרשים**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-110">Select **Item requirements**.</span></span>
5. <span data-ttu-id="ad1c8-111">בחר **New**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-111">Select **New**.</span></span>
6. <span data-ttu-id="ad1c8-112">בשורה החדשה, הזן או בחר ערך בשדה **מספר פריט**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-112">In the new row, enter or select a value in the **Item number** field.</span></span>
7. <span data-ttu-id="ad1c8-113">הזן מספר בשדה **כמות**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-113">In the **Quantity** field, enter a number.</span></span>
8. <span data-ttu-id="ad1c8-114">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-114">Select **Save**.</span></span>
9. <span data-ttu-id="ad1c8-115">בחלונית הפעולות בחר **נהל**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-115">On the Action Pane, select **Manage**.</span></span>
10. <span data-ttu-id="ad1c8-116">בחר **פונקציות**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-116">Select **Functions**.</span></span>
11. <span data-ttu-id="ad1c8-117">בחר **יצירת הזמנת רכש**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-117">Select **Create purchase order**.</span></span>
12. <span data-ttu-id="ad1c8-118">סמן את תיבת הסימון **כלול הכל**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-118">Select the **Include all** check box.</span></span>
13. <span data-ttu-id="ad1c8-119">בשדה **חשבון ספק**, הזן או בחר ערך.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-119">In the **Vendor account** field, enter or select a value.</span></span>
14. <span data-ttu-id="ad1c8-120">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-120">Select **OK**.</span></span>
15. <span data-ttu-id="ad1c8-121">בחלונית הניווט, עבור אל **מודולים > חשבונות זכאים > הזמנות רכש > כל הזמנות הרכש**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-121">In the navigation pane, go to **Modules > Accounts payable > Purchase orders > All purchase orders**.</span></span>
16. <span data-ttu-id="ad1c8-122">מתוך הרשימה בחר את הקישור בשורה הרצויה.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-122">In the list, select the link in the desired row.</span></span>
17. <span data-ttu-id="ad1c8-123">בחלונית הפעולות בחר **רכש**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-123">On the Action Pane, select **Purchase**.</span></span>
18. <span data-ttu-id="ad1c8-124">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-124">Select **Confirm**.</span></span>
19. <span data-ttu-id="ad1c8-125">בחלונית הפעולות בחר **קבל**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-125">On the Action Pane, select **Receive**.</span></span>
20. <span data-ttu-id="ad1c8-126">בחר **קבלת מוצר**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-126">Select **Product receipt**.</span></span>
21. <span data-ttu-id="ad1c8-127">הקלד ערך בשדה **קבלת מוצר**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-127">In the **Product receipt** field, type a value.</span></span>
22. <span data-ttu-id="ad1c8-128">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="ad1c8-128">Select **OK**.</span></span>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]