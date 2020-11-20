---
title: ניתוח של הצעות מחיר לפרוייקט
description: נושא זו מספק מידע אודות הניתוח של הצעות מחיר לפרוייקט.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
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
ms.openlocfilehash: 6ed900620f92e76d293f6b533b101be94b25cff3
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127024"
---
# <a name="analysis-of-project-quotes"></a><span data-ttu-id="0f263-103">ניתוח של הצעות מחיר לפרוייקט</span><span class="sxs-lookup"><span data-stu-id="0f263-103">Analysis of project quotes</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="0f263-104">Dynamics 365 Project Service Automation מנתח הצעות מחיר לפרוייקט כדי להעריך רווחיות.</span><span class="sxs-lookup"><span data-stu-id="0f263-104">Dynamics 365 Project Service Automation analyzes project quotes to estimate profitability.</span></span> <span data-ttu-id="0f263-105">הוא מנתח גם באיזו מידה הצעת המחיר מותאמת לציפיות הלקוח לגבי תאריך המסירה או תאריך ההשלמה, ולגבי התקציב.</span><span class="sxs-lookup"><span data-stu-id="0f263-105">It also analyzes how well the quote is aligned with customer expectations about the delivery date or completion date, and about the budget.tions.</span></span>

## <a name="profitability-analysis"></a><span data-ttu-id="0f263-106">ניתוח רווחיות</span><span class="sxs-lookup"><span data-stu-id="0f263-106">Profitability analysis</span></span>

<span data-ttu-id="0f263-107">Project Service Automation מנתח רווחיות באמצעות שולי הרווח הגולמי ושולי הרווי הגולמי המותאמים.</span><span class="sxs-lookup"><span data-stu-id="0f263-107">Project Service Automation analyzes profitability by using the gross margin and the adjusted gross margin.</span></span>

- <span data-ttu-id="0f263-108">שולי הרווח הגולמי מחושבים באמצעות הנוסחה הבאה:</span><span class="sxs-lookup"><span data-stu-id="0f263-108">Gross margins are calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of estimated chargeable costs) x 100
  `
- <span data-ttu-id="0f263-109">שולי הרווח הגולמי המותאמים מחושבים באמצעות הנוסחה הבאה:</span><span class="sxs-lookup"><span data-stu-id="0f263-109">The adjusted gross margin is calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of all estimated costs) x 100
  `

<span data-ttu-id="0f263-110">אם קיים הבדל בין הערכים עבור שולי הרווח הגולמי ושולי הרווח הגולמי המותאמים של שוליים רחבים, רוב העבודה בהצעת המחיר מסווגת כלא לחיוב.</span><span class="sxs-lookup"><span data-stu-id="0f263-110">If the values for gross margin and adjusted gross margin differ by a wide margin, much of the work in the quote is classified as non-chargeable.</span></span>

## <a name="analysis-of-customer-expectations"></a><span data-ttu-id="0f263-111">ניתוח של ציפיות הלקוח</span><span class="sxs-lookup"><span data-stu-id="0f263-111">Analysis of customer expectations</span></span>

<span data-ttu-id="0f263-112">באפשרותך לנתח הצעות מחיר וליצור תרשימים עבור ציפיות של לקוחות לגבי לוח הזמנים והתקציב אם תזין ערכים עבור השדות הבאים:</span><span class="sxs-lookup"><span data-stu-id="0f263-112">You can analyze quotes and generate charts for customer expectations about the schedule and budget if you enter values for the following fields:</span></span>

- <span data-ttu-id="0f263-113">השדה **תאריך מסירה מבוקש** בכותרת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="0f263-113">The **Requested delivery date** field on the quote header.</span></span>
- <span data-ttu-id="0f263-114">השדה **תקציב הלקוח** עבור כל שורת הצעת מחיר (עבור שורות מבוססות-פרוייקט ושורות מבוססות-מוצר).</span><span class="sxs-lookup"><span data-stu-id="0f263-114">The **Customer budget** field for each quote line (for project-based lines and product-based lines).</span></span>

<span data-ttu-id="0f263-115">ניתוח של ציפיות הלקוח לגבי לוח הזמנים מתבצע על-ידי השוואת תאריך הסיום המאוחר ביתר של הפרט בשורת הצעת המחיר לתאריך המסירה המבוקש בכל שורות הצעת המחיר בהצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="0f263-115">Analysis of customer expectations about the schedule is done by comparing the latest end date of the quote line detail with the requested delivery date across all quote lines in the quote.</span></span>

<span data-ttu-id="0f263-116">ניתוח של ציפיות הלקוח לגבי התקציב מתבצע על-ידי השוואת הסכום של תקציב הלקוח הכולל לסכום המופיע בהצעת המחיר בכל שורות הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="0f263-116">Analysis of customer expectations about the budget is done by comparing the sum of the total customer budget with the quoted amount across all quote lines.</span></span>
