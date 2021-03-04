---
title: יצירת הצעות מחיר, תמחור וחיוב מתקדמים
description: נושא זה מספק מידע אודות יצירת הצעות מחיר, חיוב ותמחור ב- Project Service Automation.
author: kfend
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 2/14/2019
ms.topic: article
ms.author: kfend
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: ef2698b52bd5a89a10ff0be6aff3d98e6917e95c
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5149184"
---
# <a name="advanced-quoting-pricing-and-billing-guide"></a><span data-ttu-id="1d597-103">‏‫מדריך מתקדם ליצירת הצעות מחיר, תמחור וחיוב</span><span class="sxs-lookup"><span data-stu-id="1d597-103">Advanced quoting, pricing, and billing guide</span></span>

[!include [banner](../../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="1d597-104">היכולת למצוא את המשאבים הנכונים בזמן הנכון, להזמין משאבים אלה בפרוייקטים ולשמור על ניצול המשאבים עוזרת לארגונים לעמוד ביעדי ההכנסות וביעדי שביעות הרצון של הלקוחות.</span><span class="sxs-lookup"><span data-stu-id="1d597-104">The ability to find the right resources at the right time, book those resources on projects, and keep resources utilized helps organizations meet revenue targets and customer satisfaction goals.</span></span> 

<span data-ttu-id="1d597-105">קישור ה- PDF שהוזכר קודם לכן בנושא זה הוסר והתוכן הועבר לנושאים הבאים:</span><span class="sxs-lookup"><span data-stu-id="1d597-105">The PDF link that was previously in this topic has been removed and the content has been moved to the following topics:</span></span>

- [<span data-ttu-id="1d597-106">יצירת הצעות מחיר, תמחור וחיוב</span><span class="sxs-lookup"><span data-stu-id="1d597-106">Quoting, pricing, and billing</span></span>](../quote-bill-price.md)
- [<span data-ttu-id="1d597-107">תהליכי מכירות</span><span class="sxs-lookup"><span data-stu-id="1d597-107">Sales processes</span></span>](../basic-sales-process.md)
- [<span data-ttu-id="1d597-108">הצעות מחיר ושורות של הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="1d597-108">Quotes and quote lines</span></span>](../basic-quote-lines.md)
- [<span data-ttu-id="1d597-109">שורות הצעת מחיר מבוססות-פרוייקט</span><span class="sxs-lookup"><span data-stu-id="1d597-109">Product-based quote lines</span></span>](../product-based-quote-lines.md)
- [<span data-ttu-id="1d597-110">תמחור</span><span class="sxs-lookup"><span data-stu-id="1d597-110">Pricing</span></span>](../basic-pricing.md)
- [<span data-ttu-id="1d597-111">תמחור קטלוג מוצרים</span><span class="sxs-lookup"><span data-stu-id="1d597-111">Product catalog pricing</span></span>](../product-catalog-pricing.md)
- [<span data-ttu-id="1d597-112">עסקאות</span><span class="sxs-lookup"><span data-stu-id="1d597-112">Business transactions</span></span>](../basic-business-transactions.md)
- [<span data-ttu-id="1d597-113">הערכות</span><span class="sxs-lookup"><span data-stu-id="1d597-113">Estimates</span></span>](../estimates.md)
- [<span data-ttu-id="1d597-114">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="1d597-114">Actuals</span></span>](../actuals.md)
- [<span data-ttu-id="1d597-115">ניתוח הצעות מחיר לפרוייקט</span><span class="sxs-lookup"><span data-stu-id="1d597-115">Analyzing project quotes</span></span>](../basic-analyzing-quotes.md)
- [<span data-ttu-id="1d597-116">יחידות ארגוניות</span><span class="sxs-lookup"><span data-stu-id="1d597-116">Organizational units</span></span>](../advanced-organizational.md)
- [<span data-ttu-id="1d597-117">קבוצות יחידות ויחידות</span><span class="sxs-lookup"><span data-stu-id="1d597-117">Unit groups and units</span></span>](../advanced-units.md)
- [<span data-ttu-id="1d597-118">תרחישים מרובי מטבעות</span><span class="sxs-lookup"><span data-stu-id="1d597-118">Multi-currency scenarios</span></span>](../advanced-currency.md)
- [<span data-ttu-id="1d597-119">תיעוד נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="1d597-119">Recording actuals</span></span>](../advanced-actuals.md)

> [!NOTE]
> <span data-ttu-id="1d597-120">נושא זה יוסר בעדכון עתידי של תיעוד.</span><span class="sxs-lookup"><span data-stu-id="1d597-120">This topic will be removed in a future documentation update.</span></span> 
