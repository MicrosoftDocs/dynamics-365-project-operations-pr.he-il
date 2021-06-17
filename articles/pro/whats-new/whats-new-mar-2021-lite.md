---
title: מה חדש, מרץ 2021 - פריסה קלה של Project Operations
description: נושא זה מספק מידע על עדכוני האיכות הזמינים במהדורת מרץ 2021 עבור פריסה קלה של Project Operations.
author: sigitac
ms.date: 03/03/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: efddb96b2cb428b9dc0488c32eb5670d01322bcb
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993867"
---
# <a name="whats-new-march-2021---project-operations-lite-deployment"></a><span data-ttu-id="6a149-103">מה חדש, מרץ 2021 - פריסה קלה של Project Operations</span><span class="sxs-lookup"><span data-stu-id="6a149-103">What's new March 2021 - Project Operations lite deployment</span></span>

<span data-ttu-id="6a149-104">_חל על: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="6a149-104">_Applies To: Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="6a149-105">נושא זה חל על הרכיבים והגירסאות הבאים של Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="6a149-105">This topic applies to the following Dynamics 365 Project Operations components and versions:</span></span>

- <span data-ttu-id="6a149-106">Project Operations בסביבת Dataverse גרסה 4.8.0.91</span><span class="sxs-lookup"><span data-stu-id="6a149-106">Project Operations on Dataverse environment version 4.8.0.91</span></span> 

## <a name="quality-updates"></a><span data-ttu-id="6a149-107">עדכוני איכות</span><span class="sxs-lookup"><span data-stu-id="6a149-107">Quality updates</span></span>

| <span data-ttu-id="6a149-108">**אזור תכונות**</span><span class="sxs-lookup"><span data-stu-id="6a149-108">**Feature area**</span></span> | <span data-ttu-id="6a149-109">**מספר אסמכתא**</span><span class="sxs-lookup"><span data-stu-id="6a149-109">**Reference number**</span></span> | <span data-ttu-id="6a149-110">**עדכון איכות**</span><span class="sxs-lookup"><span data-stu-id="6a149-110">**Quality update**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="6a149-111">חיוב ותמחור</span><span class="sxs-lookup"><span data-stu-id="6a149-111">Billing and pricing</span></span> | <span data-ttu-id="6a149-112">2133873</span><span class="sxs-lookup"><span data-stu-id="6a149-112">2133873</span></span> | <span data-ttu-id="6a149-113">תוקנה התצוגה של סמל מטבע **מחיר מכירות ליחידה** ברשת **אומדני הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="6a149-113">Fixed the display of **Unit Sales Price** currency symbol in the **Expense Estimates** grid.</span></span> |
| <span data-ttu-id="6a149-114">חיוב ותמחור</span><span class="sxs-lookup"><span data-stu-id="6a149-114">Billing and pricing</span></span> | <span data-ttu-id="6a149-115">2174616</span><span class="sxs-lookup"><span data-stu-id="6a149-115">2174616</span></span> | <span data-ttu-id="6a149-116">כאשר הצעת מחיר זוכה, יש התייחסות למחירון מותאם אישית של חוזה בסעיפי חוזה שמועתקים מהצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="6a149-116">When a quote is won, the contract custom pricelist is referenced on contract line details that are copied from the quote.</span></span> |
| <span data-ttu-id="6a149-117">ניהול הזדמנויות</span><span class="sxs-lookup"><span data-stu-id="6a149-117">Opportunity Management</span></span> | <span data-ttu-id="6a149-118">2167475</span><span class="sxs-lookup"><span data-stu-id="6a149-118">2167475</span></span> | <span data-ttu-id="6a149-119">סכום מס קבוע בחשבונית התיקון שמקורו ברישום בפועל שלא בוצע.</span><span class="sxs-lookup"><span data-stu-id="6a149-119">Fixed tax amount in the correction invoice that originated an unbilled actual entry.</span></span> |
| <span data-ttu-id="6a149-120">ניהול הזדמנויות</span><span class="sxs-lookup"><span data-stu-id="6a149-120">Opportunity Management</span></span> | <span data-ttu-id="6a149-121">2176285</span><span class="sxs-lookup"><span data-stu-id="6a149-121">2176285</span></span> | <span data-ttu-id="6a149-122">אין להעתיק סכום מס מפרטי חוזה מכירות/שורת הצעת מחיר לפרטי חוזה עלות/הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="6a149-122">Tax amount must not be copied from sales contract/quote line details to cost contract/quote line details.</span></span> |
| <span data-ttu-id="6a149-123">ניהול הזדמנויות</span><span class="sxs-lookup"><span data-stu-id="6a149-123">Opportunity Management</span></span> | <span data-ttu-id="6a149-124">2188079</span><span class="sxs-lookup"><span data-stu-id="6a149-124">2188079</span></span> | <span data-ttu-id="6a149-125">אין ליצור כלל חיוב מפוצל עבור חוזים שאינם מבוססים על עבודה.</span><span class="sxs-lookup"><span data-stu-id="6a149-125">Split billing rule must not be created for contracts that are not work-based.</span></span> |
| <span data-ttu-id="6a149-126">‏‫תכנון ומעקב</span><span class="sxs-lookup"><span data-stu-id="6a149-126">Planning and Tracking</span></span> | <span data-ttu-id="6a149-127">2138853</span><span class="sxs-lookup"><span data-stu-id="6a149-127">2138853</span></span> | <span data-ttu-id="6a149-128">פונקציית העתקת הפרויקט עודכנה כדי להבטיח ששורות אומדן הוצאות שמתייחסות להפניה מועתקות לפרויקט היעד.</span><span class="sxs-lookup"><span data-stu-id="6a149-128">Project copy function updated to ensure expense estimate lines that reference tasks are copied to the destination project.</span></span> |
| <span data-ttu-id="6a149-129">‏‫תכנון ומעקב</span><span class="sxs-lookup"><span data-stu-id="6a149-129">Planning and Tracking</span></span> | <span data-ttu-id="6a149-130">2173259</span><span class="sxs-lookup"><span data-stu-id="6a149-130">2173259</span></span> | <span data-ttu-id="6a149-131">פונקציית העתקת הפרויקט עודכנה כדי להבטיח שהיא לא מציגה את הודעת השגיאה **העתקת WBS** בתרחישים מסוימים.</span><span class="sxs-lookup"><span data-stu-id="6a149-131">Project copy function updated to ensure it doesn't display the **Copying WBS** error message in certain scenarios.</span></span> |
| <span data-ttu-id="6a149-132">זמן והוצאה</span><span class="sxs-lookup"><span data-stu-id="6a149-132">Time and Expense</span></span> | <span data-ttu-id="6a149-133">2148910</span><span class="sxs-lookup"><span data-stu-id="6a149-133">2148910</span></span> | <span data-ttu-id="6a149-134">תוקנה בעיה בתצוגה קבועה בדף **ערוך ערך** ברשת **ערכי זמן**.</span><span class="sxs-lookup"><span data-stu-id="6a149-134">Fixed display issue with the **Edit Entry** page in the **Time Entry** grid.</span></span> |
| <span data-ttu-id="6a149-135">זמן והוצאה</span><span class="sxs-lookup"><span data-stu-id="6a149-135">Time and Expense</span></span> | <span data-ttu-id="6a149-136">2159798</span><span class="sxs-lookup"><span data-stu-id="6a149-136">2159798</span></span> | <span data-ttu-id="6a149-137">בקרות טובות יותר כדי להבטיח שלא ניתן לערוך רשומות הוצאות שאושרו.</span><span class="sxs-lookup"><span data-stu-id="6a149-137">Tightened controls to ensure approved expense entries can't be edited.</span></span> |


