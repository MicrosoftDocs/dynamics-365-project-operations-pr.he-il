---
title: מה חדש, מרץ 2021 - פריסה קלה של Project Operations
description: נושא זה מספק מידע על עדכוני האיכות הזמינים במהדורת מרץ 2021 עבור פריסה קלה של Project Operations.
author: sigitac
manager: tfehr
ms.date: 03/03/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: bd1518ef8f5645bace63a222b92cfd16d9c19a21
ms.sourcegitcommit: f78087174a8512199a1bcbd7e8610bbc80e64801
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "5500004"
---
# <a name="whats-new-march-2021---project-operations-lite-deployment"></a><span data-ttu-id="feffb-103">מה חדש, מרץ 2021 - פריסה קלה של Project Operations</span><span class="sxs-lookup"><span data-stu-id="feffb-103">What's new March 2021 - Project Operations lite deployment</span></span>

<span data-ttu-id="feffb-104">_חל על: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="feffb-104">_Applies To: Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="feffb-105">נושא זה חל על הרכיבים והגירסאות הבאים של Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="feffb-105">This topic applies to the following Dynamics 365 Project Operations components and versions:</span></span>

- <span data-ttu-id="feffb-106">Project Operations בסביבת Dataverse גרסה 4.8.0.91</span><span class="sxs-lookup"><span data-stu-id="feffb-106">Project Operations on Dataverse environment version 4.8.0.91</span></span> 

## <a name="quality-updates"></a><span data-ttu-id="feffb-107">עדכוני איכות</span><span class="sxs-lookup"><span data-stu-id="feffb-107">Quality updates</span></span>

| <span data-ttu-id="feffb-108">**אזור תכונות**</span><span class="sxs-lookup"><span data-stu-id="feffb-108">**Feature area**</span></span> | <span data-ttu-id="feffb-109">**מספר אסמכתא**</span><span class="sxs-lookup"><span data-stu-id="feffb-109">**Reference number**</span></span> | <span data-ttu-id="feffb-110">**עדכון איכות**</span><span class="sxs-lookup"><span data-stu-id="feffb-110">**Quality update**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="feffb-111">חיוב ותמחור</span><span class="sxs-lookup"><span data-stu-id="feffb-111">Billing and pricing</span></span> | <span data-ttu-id="feffb-112">2133873</span><span class="sxs-lookup"><span data-stu-id="feffb-112">2133873</span></span> | <span data-ttu-id="feffb-113">תוקנה התצוגה של סמל מטבע **מחיר מכירות ליחידה** ברשת **אומדני הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="feffb-113">Fixed the display of **Unit Sales Price** currency symbol in the **Expense Estimates** grid.</span></span> |
| <span data-ttu-id="feffb-114">חיוב ותמחור</span><span class="sxs-lookup"><span data-stu-id="feffb-114">Billing and pricing</span></span> | <span data-ttu-id="feffb-115">2174616</span><span class="sxs-lookup"><span data-stu-id="feffb-115">2174616</span></span> | <span data-ttu-id="feffb-116">כאשר הצעת מחיר זוכה, יש התייחסות למחירון מותאם אישית של חוזה בסעיפי חוזה שמועתקים מהצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="feffb-116">When a quote is won, the contract custom pricelist is referenced on contract line details that are copied from the quote.</span></span> |
| <span data-ttu-id="feffb-117">ניהול הזדמנויות</span><span class="sxs-lookup"><span data-stu-id="feffb-117">Opportunity Management</span></span> | <span data-ttu-id="feffb-118">2167475</span><span class="sxs-lookup"><span data-stu-id="feffb-118">2167475</span></span> | <span data-ttu-id="feffb-119">סכום מס קבוע בחשבונית התיקון שמקורו ברישום בפועל שלא בוצע.</span><span class="sxs-lookup"><span data-stu-id="feffb-119">Fixed tax amount in the correction invoice that originated an unbilled actual entry.</span></span> |
| <span data-ttu-id="feffb-120">ניהול הזדמנויות</span><span class="sxs-lookup"><span data-stu-id="feffb-120">Opportunity Management</span></span> | <span data-ttu-id="feffb-121">2176285</span><span class="sxs-lookup"><span data-stu-id="feffb-121">2176285</span></span> | <span data-ttu-id="feffb-122">אין להעתיק סכום מס מפרטי חוזה מכירות/שורת הצעת מחיר לפרטי חוזה עלות/הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="feffb-122">Tax amount must not be copied from sales contract/quote line details to cost contract/quote line details.</span></span> |
| <span data-ttu-id="feffb-123">ניהול הזדמנויות</span><span class="sxs-lookup"><span data-stu-id="feffb-123">Opportunity Management</span></span> | <span data-ttu-id="feffb-124">2188079</span><span class="sxs-lookup"><span data-stu-id="feffb-124">2188079</span></span> | <span data-ttu-id="feffb-125">אין ליצור כלל חיוב מפוצל עבור חוזים שאינם מבוססים על עבודה.</span><span class="sxs-lookup"><span data-stu-id="feffb-125">Split billing rule must not be created for contracts that are not work-based.</span></span> |
| <span data-ttu-id="feffb-126">‏‫תכנון ומעקב</span><span class="sxs-lookup"><span data-stu-id="feffb-126">Planning and Tracking</span></span> | <span data-ttu-id="feffb-127">2138853</span><span class="sxs-lookup"><span data-stu-id="feffb-127">2138853</span></span> | <span data-ttu-id="feffb-128">פונקציית העתקת הפרויקט עודכנה כדי להבטיח ששורות אומדן הוצאות שמתייחסות להפניה מועתקות לפרויקט היעד.</span><span class="sxs-lookup"><span data-stu-id="feffb-128">Project copy function updated to ensure expense estimate lines that reference tasks are copied to the destination project.</span></span> |
| <span data-ttu-id="feffb-129">‏‫תכנון ומעקב</span><span class="sxs-lookup"><span data-stu-id="feffb-129">Planning and Tracking</span></span> | <span data-ttu-id="feffb-130">2173259</span><span class="sxs-lookup"><span data-stu-id="feffb-130">2173259</span></span> | <span data-ttu-id="feffb-131">פונקציית העתקת הפרויקט עודכנה כדי להבטיח שהיא לא מציגה את הודעת השגיאה **העתקת WBS** בתרחישים מסוימים.</span><span class="sxs-lookup"><span data-stu-id="feffb-131">Project copy function updated to ensure it doesn't display the **Copying WBS** error message in certain scenarios.</span></span> |
| <span data-ttu-id="feffb-132">זמן והוצאה</span><span class="sxs-lookup"><span data-stu-id="feffb-132">Time and Expense</span></span> | <span data-ttu-id="feffb-133">2148910</span><span class="sxs-lookup"><span data-stu-id="feffb-133">2148910</span></span> | <span data-ttu-id="feffb-134">תוקנה בעיה בתצוגה קבועה בדף **ערוך ערך** ברשת **ערכי זמן**.</span><span class="sxs-lookup"><span data-stu-id="feffb-134">Fixed display issue with the **Edit Entry** page in the **Time Entry** grid.</span></span> |
| <span data-ttu-id="feffb-135">זמן והוצאה</span><span class="sxs-lookup"><span data-stu-id="feffb-135">Time and Expense</span></span> | <span data-ttu-id="feffb-136">2159798</span><span class="sxs-lookup"><span data-stu-id="feffb-136">2159798</span></span> | <span data-ttu-id="feffb-137">בקרות טובות יותר כדי להבטיח שלא ניתן לערוך רשומות הוצאות שאושרו.</span><span class="sxs-lookup"><span data-stu-id="feffb-137">Tightened controls to ensure approved expense entries can't be edited.</span></span> |


