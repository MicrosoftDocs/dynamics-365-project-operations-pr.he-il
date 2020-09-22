---
title: מדוע ברירת המחדל למחיר היא אפס עבור עלות ההוצאות בפועל?
description: פתרון בעיות בנושא מדוע ברירת המחדל למחיר היא אפס עבור עלות ההוצאות בפועל.
author: rumant
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 8/22/2018
ms.topic: article
ms.prod: Project Service
ms.technology: ''
ms.assetid: bc1ebc58-c733-4310-8435-572ed9a9fef9
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 3fb678822877a61d141de75aea29b7d5cdf292c4
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751798"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="a8361-103">מדוע ברירת המחדל למחיר היא אפס עבור עלות ההוצאות בפועל?</span><span class="sxs-lookup"><span data-stu-id="a8361-103">Why is the price defaulting to zero on expense cost actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a8361-104">שאלות נפוצות אלה דנות בנושא ההוצאות בפועל כאשר מחלקת התנועות מוגדרת כ'הוצאה' וסוג התנועה הוא 'עלות'.</span><span class="sxs-lookup"><span data-stu-id="a8361-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="a8361-105">פתרון בעיות בנושא תעריפים עבור עלות הוצאות בפועל</span><span class="sxs-lookup"><span data-stu-id="a8361-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="a8361-106">עבור להוצאה הקשורה וודא כי קיים סכום בשדה ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="a8361-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="a8361-107">אם בהוצאה המקורית שדה הסכום ריק, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="a8361-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="a8361-108">כדי לפתור בעיה זו, צור מחדש את ההוצאה עם סכום חוקי ואשר אותו.</span><span class="sxs-lookup"><span data-stu-id="a8361-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>
