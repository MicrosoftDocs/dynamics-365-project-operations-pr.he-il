---
title: שימוש בשדה קיים ב- Project Service כממד תמחור
description: נושא זה מספק מידע על שימוש בשדות קיימים של Project Service כממדי תמחור.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/19/2018
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 8bc3a1df7669dac43b45d781448ed5c795a65be4
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5144159"
---
# <a name="use-an-existing-field-in-project-service-as-a-pricing-dimension"></a><span data-ttu-id="90145-103">שימוש בשדה קיים ב- Project Service כממד תמחור</span><span class="sxs-lookup"><span data-stu-id="90145-103">Use an existing field in Project Service as a pricing dimension</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="90145-104">ל- Project Service Automation ‏(PSA) יש שדות רבים בישות **נתונים בפועל** שניתן להשתמש בהם כממדי תמחור עבור תמחור מבוסס משאבים בארגוני פרויקטים.</span><span class="sxs-lookup"><span data-stu-id="90145-104">Project Service Automation (PSA) has many fields on the **Actuals** entity that can be used as pricing dimensions for resource-based pricing in project organizations.</span></span> <span data-ttu-id="90145-105">לדוגמה, שדה משותף אחד הוא **משאב ניתן להזמנה**.</span><span class="sxs-lookup"><span data-stu-id="90145-105">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="90145-106">חברות קטנות יותר, בעלות פחות מ- 20-30 משאבים הניתנים לחיוב, עשויות להחליט שהגישה הפשוטה ביותר היא להקצות תעריפי חיוב ועלות ספציפיים לכל משאב.</span><span class="sxs-lookup"><span data-stu-id="90145-106">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="90145-107">עם זאת, ככל שכוח העבודה לחיוב גדל, תעריפים מסוימים עשויים להיות בלתי מציאותיים כי תעריפי העלות והחיוב של המשאבים עשויים להשתנות בזמן שהמשאבים מקודמים לתפקידים חדשים, צוברים ניסיון נוסף או רוכשים מיומנויות שונות.</span><span class="sxs-lookup"><span data-stu-id="90145-107">However, as the billable workforce grows, specific rates could become unrealistic to maintain as resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different skill set.</span></span> <span data-ttu-id="90145-108">מאחר שגישה זו עדיין מתאימה לחברות בגודל מסוים, ראה [שימוש במשאב ניתן להזמנה כממד תמחור](bookable-resource-pricing-dimension.md) כדי להבין כיצד ניתן להשתמש בשדה קיים של Project Service כממד תמחור.</span><span class="sxs-lookup"><span data-stu-id="90145-108">Because this approach still works for companies of a certain size, see [Use a bookable resource as a pricing dimension](bookable-resource-pricing-dimension.md) to understand how an existing Project Service field can be used as a pricing dimension.</span></span>

<span data-ttu-id="90145-109">דוגמה נוספת היא קטגוריית עסקה.</span><span class="sxs-lookup"><span data-stu-id="90145-109">Another example is that of transaction category.</span></span> <span data-ttu-id="90145-110">לקוחות ומיישמים משתמשים בקטגוריית העסקה ב- PSA כדי לסווג את העבודה, ומשתמשים בשדה לקביעת המחיר והעלות בהתאם לקטגוריית העבודה.</span><span class="sxs-lookup"><span data-stu-id="90145-110">Customers and Implementers have used the transaction category in PSA to classify work and use the field to price and cost based on the category of work.</span></span> <span data-ttu-id="90145-111">לקבלת מידע נוסף, ראה [שימוש בקטגוריית עסקה כממד תמחור](transaction-category-pricing-dimension.md).</span><span class="sxs-lookup"><span data-stu-id="90145-111">For more information, see [Use transaction category as a pricing dimension](transaction-category-pricing-dimension.md).</span></span>
