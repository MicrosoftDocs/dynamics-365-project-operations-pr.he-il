---
title: מה חדש, מרץ 2021 - Project Operations לתרחישים מבוססי משאבים/ללא מלאי
description: נושא זה מספק מידע על עדכוני האיכות הזמינים במהדורת מרץ 2021 של Project Operations לתרחישים מבוססי משאבים/לא מלאי.
author: sigitac
manager: tfehr
ms.date: 03/03/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4d114ee64bd26d3271a1c72a7404c0f7035c2b61
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948060"
---
# <a name="whats-new-march-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a><span data-ttu-id="d31fe-103">מה חדש, מרץ 2021 - Project Operations לתרחישים מבוססי משאבים/ללא מלאי</span><span class="sxs-lookup"><span data-stu-id="d31fe-103">What's new March 2021 - Project Operations for resource/non-stocked based scenarios</span></span>

<span data-ttu-id="d31fe-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="d31fe-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="d31fe-105">נושא זה חל על הרכיבים והגירסאות הבאים של Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="d31fe-105">This topic applies to the following Dynamics 365 Project Operations components and versions:</span></span>

- <span data-ttu-id="d31fe-106">Project Operations בסביבת Dataverse גרסה 4.8.0.91</span><span class="sxs-lookup"><span data-stu-id="d31fe-106">Project Operations on Dataverse environment version 4.8.0.91</span></span> 
- <span data-ttu-id="d31fe-107">ניהול פרויקטים וחשבונאות בסביבת Dynamics 365 Finance גרסה 10.0.16</span><span class="sxs-lookup"><span data-stu-id="d31fe-107">Project management and accounting on Dynamics 365 Finance environment version 10.0.16</span></span> 

## <a name="quality-updates"></a><span data-ttu-id="d31fe-108">עדכוני איכות</span><span class="sxs-lookup"><span data-stu-id="d31fe-108">Quality updates</span></span>

### <a name="project-operations-on-dataverse"></a><span data-ttu-id="d31fe-109">Project Operations ב- Dataverse</span><span class="sxs-lookup"><span data-stu-id="d31fe-109">Project Operations on Dataverse</span></span>


| <span data-ttu-id="d31fe-110">**אזור תכונות**</span><span class="sxs-lookup"><span data-stu-id="d31fe-110">**Feature area**</span></span> | <span data-ttu-id="d31fe-111">**מספר אסמכתא**</span><span class="sxs-lookup"><span data-stu-id="d31fe-111">**Reference number**</span></span> | <span data-ttu-id="d31fe-112">**עדכון איכות**</span><span class="sxs-lookup"><span data-stu-id="d31fe-112">**Quality update**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="d31fe-113">חיוב ותמחור</span><span class="sxs-lookup"><span data-stu-id="d31fe-113">Billing and pricing</span></span> | <span data-ttu-id="d31fe-114">2133873</span><span class="sxs-lookup"><span data-stu-id="d31fe-114">2133873</span></span> | <span data-ttu-id="d31fe-115">תוקנה התצוגה של סמל מטבע **מחיר מכירות ליחידה** ברשת **אומדני הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="d31fe-115">Fixed the display of **Unit Sales Price** currency symbol in the **Expense Estimates** grid.</span></span> |
| <span data-ttu-id="d31fe-116">חיוב ותמחור</span><span class="sxs-lookup"><span data-stu-id="d31fe-116">Billing and pricing</span></span> | <span data-ttu-id="d31fe-117">2174616</span><span class="sxs-lookup"><span data-stu-id="d31fe-117">2174616</span></span> | <span data-ttu-id="d31fe-118">כאשר הצעת מחיר זוכה, יש התייחסות למחירון מותאם אישית של חוזה בסעיפי חוזה שמועתקים מהצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d31fe-118">When a quote is won, the contract custom pricelist is referenced on contract line details that are copied from the quote.</span></span> |
| <span data-ttu-id="d31fe-119">ניהול הזדמנויות</span><span class="sxs-lookup"><span data-stu-id="d31fe-119">Opportunity Management</span></span> | <span data-ttu-id="d31fe-120">2167475</span><span class="sxs-lookup"><span data-stu-id="d31fe-120">2167475</span></span> | <span data-ttu-id="d31fe-121">סכום מס קבוע בחשבונית התיקון שמקורו ברישום בפועל שלא בוצע.</span><span class="sxs-lookup"><span data-stu-id="d31fe-121">Fixed tax amount in the correction invoice that originated an unbilled actual entry.</span></span> |
| <span data-ttu-id="d31fe-122">ניהול הזדמנויות</span><span class="sxs-lookup"><span data-stu-id="d31fe-122">Opportunity Management</span></span> | <span data-ttu-id="d31fe-123">2176285</span><span class="sxs-lookup"><span data-stu-id="d31fe-123">2176285</span></span> | <span data-ttu-id="d31fe-124">אין להעתיק סכום מס מפרטי חוזה מכירות/שורת הצעת מחיר לפרטי חוזה עלות/הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="d31fe-124">Tax amount must not be copied from sales contract/quote line details to cost contract/quote line details.</span></span> |
| <span data-ttu-id="d31fe-125">ניהול הזדמנויות</span><span class="sxs-lookup"><span data-stu-id="d31fe-125">Opportunity Management</span></span> | <span data-ttu-id="d31fe-126">2188079</span><span class="sxs-lookup"><span data-stu-id="d31fe-126">2188079</span></span> | <span data-ttu-id="d31fe-127">אין ליצור כלל חיוב מפוצל עבור חוזים שאינם מבוססים על עבודה.</span><span class="sxs-lookup"><span data-stu-id="d31fe-127">Split billing rule must not be created for contracts that are not work-based.</span></span> |
| <span data-ttu-id="d31fe-128">‏‫תכנון ומעקב</span><span class="sxs-lookup"><span data-stu-id="d31fe-128">Planning and Tracking</span></span> | <span data-ttu-id="d31fe-129">2125274</span><span class="sxs-lookup"><span data-stu-id="d31fe-129">2125274</span></span> | <span data-ttu-id="d31fe-130">התכונה **מפת פרוייקט בכתיבה כפולה** עבור **מיפוי תאריכי התחלה בפרויקט** עודכנה מ- **msdyn\_taskearlieststart‎** ל- **msdyn\_actualstart‎**.</span><span class="sxs-lookup"><span data-stu-id="d31fe-130">**Project Dual Write Map** attribute for **Project Start Date Mapping** updated from **msdyn\_taskearlieststart** to **msdyn\_actualstart**.</span></span> |
| <span data-ttu-id="d31fe-131">‏‫תכנון ומעקב</span><span class="sxs-lookup"><span data-stu-id="d31fe-131">Planning and Tracking</span></span> | <span data-ttu-id="d31fe-132">2138853</span><span class="sxs-lookup"><span data-stu-id="d31fe-132">2138853</span></span> | <span data-ttu-id="d31fe-133">פונקציית העתקת הפרויקט עודכנה כדי להבטיח ששורות אומדן הוצאות שמתייחסות להפניה מועתקות לפרויקט היעד.</span><span class="sxs-lookup"><span data-stu-id="d31fe-133">Project copy function updated to ensure expense estimate lines that reference tasks are copied to the destination project.</span></span> |
| <span data-ttu-id="d31fe-134">‏‫תכנון ומעקב</span><span class="sxs-lookup"><span data-stu-id="d31fe-134">Planning and Tracking</span></span> | <span data-ttu-id="d31fe-135">2154306</span><span class="sxs-lookup"><span data-stu-id="d31fe-135">2154306</span></span> | <span data-ttu-id="d31fe-136">תוקנו בעיות במחיקת אומדני הוצאות ב- Project Operations לתרחישים מבוססי משאבים.</span><span class="sxs-lookup"><span data-stu-id="d31fe-136">Fixed issues with deleting expense estimates in Project Operations for resource-based scenarios.</span></span> |
| <span data-ttu-id="d31fe-137">‏‫תכנון ומעקב</span><span class="sxs-lookup"><span data-stu-id="d31fe-137">Planning and Tracking</span></span> | <span data-ttu-id="d31fe-138">2173259</span><span class="sxs-lookup"><span data-stu-id="d31fe-138">2173259</span></span> | <span data-ttu-id="d31fe-139">פונקציית העתקת הפרויקט עודכנה כדי להבטיח שהיא לא מציגה הודעת שגיאה על **העתקת WBS** בתרחישים מסוימים.</span><span class="sxs-lookup"><span data-stu-id="d31fe-139">Project copy function updated to ensure it doesn't display **Copying WBS** error message in certain scenarios.</span></span> |
| <span data-ttu-id="d31fe-140">זמן והוצאה</span><span class="sxs-lookup"><span data-stu-id="d31fe-140">Time and Expense</span></span> | <span data-ttu-id="d31fe-141">2148910</span><span class="sxs-lookup"><span data-stu-id="d31fe-141">2148910</span></span> | <span data-ttu-id="d31fe-142">תוקנה בעיה בתצוגה קבועה בדף **ערוך ערך** ברשת **ערכי זמן**.</span><span class="sxs-lookup"><span data-stu-id="d31fe-142">Fixed display issue with the **Edit Entry** page in the **Time Entry** grid.</span></span> |
| <span data-ttu-id="d31fe-143">זמן והוצאה</span><span class="sxs-lookup"><span data-stu-id="d31fe-143">Time and Expense</span></span> | <span data-ttu-id="d31fe-144">2159798</span><span class="sxs-lookup"><span data-stu-id="d31fe-144">2159798</span></span> | <span data-ttu-id="d31fe-145">בקרות טובות יותר כדי להבטיח שלא ניתן לערוך רשומות הוצאות שאושרו.</span><span class="sxs-lookup"><span data-stu-id="d31fe-145">Tightened controls to ensure approved expense entries can't be edited.</span></span> |

### <a name="project-management-and-accounting-on-dynamics-365-finance"></a><span data-ttu-id="d31fe-146">ניהול פרויקטים וחשבונאות ב- Dynamics 365 Finance</span><span class="sxs-lookup"><span data-stu-id="d31fe-146">Project management and accounting on Dynamics 365 Finance</span></span>

<span data-ttu-id="d31fe-147">למידע נוסף, ראה [מה חדש, ינואר 2021 - Project Operations לתרחישים המבוססים על משאבים/ללא מלאי](whats-new-jan-2021-resource-based.md).</span><span class="sxs-lookup"><span data-stu-id="d31fe-147">For more information, see [What's new January 2021 - Project Operations for resource/non-stocked based scenarios](whats-new-jan-2021-resource-based.md).</span></span>

## <a name="regulatory-updates"></a><span data-ttu-id="d31fe-148">עדכוני רגולציה</span><span class="sxs-lookup"><span data-stu-id="d31fe-148">Regulatory updates</span></span>

<span data-ttu-id="d31fe-149">למידע על עדכונים רגולטוריים עבור יישומי Finance and Operations, ראה [עדכוני רגולציה](/dynamics365/finance/localizations/regulatory-updates).</span><span class="sxs-lookup"><span data-stu-id="d31fe-149">For information about regulatory updates for Finance and Operations apps, see [Regulatory updates](/dynamics365/finance/localizations/regulatory-updates).</span></span> <span data-ttu-id="d31fe-150">דרך נוספת ללמוד על עדכונים רגולטוריים היא להיכנס אל LCS ולהציג את עדכוני הרגולציה המתוכננים באמצעות כלי חיפוש הבעיות.</span><span class="sxs-lookup"><span data-stu-id="d31fe-150">Another way to learn about regulatory updates is to sign in to LCS and view the planned regulatory updates using the issue search tool.</span></span> <span data-ttu-id="d31fe-151">חיפוש בעיות מאפשר לך לחפש לפי מדינה, סוג תכונה והפצה.</span><span class="sxs-lookup"><span data-stu-id="d31fe-151">Issue search lets you search by country, type of feature, and release.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]