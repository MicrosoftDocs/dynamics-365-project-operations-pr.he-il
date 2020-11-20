---
title: מדוע ברירת המחדל למחיר היא אפס עבור עלות ההוצאות בפועל?
description: פתרון בעיות בנושא מדוע ברירת המחדל למחיר היא אפס עבור עלות ההוצאות בפועל.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/22/2018
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
ms.openlocfilehash: 306f169ee25d42ac3c9e63fa70956b9c50315829
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122119"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="a6034-103">מדוע ברירת המחדל למחיר היא אפס עבור עלות ההוצאות בפועל?</span><span class="sxs-lookup"><span data-stu-id="a6034-103">Why is the price defaulting to zero on expense cost actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a6034-104">שאלות נפוצות אלה דנות בנושא ההוצאות בפועל כאשר מחלקת התנועות מוגדרת כ'הוצאה' וסוג התנועה הוא 'עלות'.</span><span class="sxs-lookup"><span data-stu-id="a6034-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="a6034-105">פתרון בעיות בנושא תעריפים עבור עלות הוצאות בפועל</span><span class="sxs-lookup"><span data-stu-id="a6034-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="a6034-106">עבור להוצאה הקשורה וודא כי קיים סכום בשדה ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="a6034-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="a6034-107">אם בהוצאה המקורית שדה הסכום ריק, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="a6034-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="a6034-108">כדי לפתור בעיה זו, צור מחדש את ההוצאה עם סכום חוקי ואשר אותו.</span><span class="sxs-lookup"><span data-stu-id="a6034-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>
