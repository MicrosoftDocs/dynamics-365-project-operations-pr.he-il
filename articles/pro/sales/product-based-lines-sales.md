---
title: שורות בהזדמנות מבוססות מוצר
description: נושא זה מספק מידע על פרטים בשורות הזדמנות מבוססות מוצר ב-Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 17ffcf8dc94d42102115281d281d6b553cf1fa17
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077234"
---
# <a name="product-based-opportunity-lines"></a><span data-ttu-id="ac682-103">שורות בהזדמנות מבוססות מוצר</span><span class="sxs-lookup"><span data-stu-id="ac682-103">Product-based opportunity lines</span></span>

<span data-ttu-id="ac682-104">_**חל על** : פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="ac682-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ac682-105">שורות הזדמנות מבוססות מוצר הן פריטי שורה בהזדמנות.</span><span class="sxs-lookup"><span data-stu-id="ac682-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="ac682-106">שורות אלה מועברות ללקוח כפריטי שורה מובחנים בחשבונית הסופית ללא שירותים נוספים בעלי ערך מוסף.</span><span class="sxs-lookup"><span data-stu-id="ac682-106">These lines are delivered to the customer as distinct line items on the eventual invoice without any other value-added services.</span></span> <span data-ttu-id="ac682-107">ההוצאות והצריכה במשוייכים אינם נמצאים במעקב במשימות של פרויקטים קשורים כלשהם.</span><span class="sxs-lookup"><span data-stu-id="ac682-107">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="ac682-108">שורות מבוססות מוצר יכולים להיות פריטי קטלוג או מוצרים שאינם מופיעים ברשימה.</span><span class="sxs-lookup"><span data-stu-id="ac682-108">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="ac682-109">מרבית הפונקציונליות בשורות מבוססות מוצר של הזדמנות מבוססת על הפונקציונליות ביישום Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="ac682-109">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="ac682-110">לקבלת מידע נוסף אודות שורות הזדמנות מבוססות מוצר, ראה[הוספת מוצרים להזדמנות](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="ac682-110">For more information about product-based opportunity lines, see [Add products to an opportunity](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="ac682-111">מושג אחד הקשור לשורות הזדמנות מבוססות מוצר, שהוא ספציפי להזדמנויות מבוססות פרויקט, הוא **תקציב לקוח**.</span><span class="sxs-lookup"><span data-stu-id="ac682-111">One concept about product-based opportunity lines that is specific to project-based opportunities is **Customer Budget**.</span></span> <span data-ttu-id="ac682-112">השתמש בשדה זה כדי לעקוב אחר הסכום שהלקוח מוכן לשלם עבור פריט השורה.</span><span class="sxs-lookup"><span data-stu-id="ac682-112">Use this field to track the amount the customer is willing to pay for the line item.</span></span>

<span data-ttu-id="ac682-113">אם שיטת ההכנסות של סיכום ההזדמנות מוגדרת ל **מחושב על ידי המערכת** , ערכי תקציב הלקוח בכל השורות מבוססות המוצר ובכל השורות מבוססות הפרויקט מסוכמים כדי לחשב את ההכנסות המשוערות.</span><span class="sxs-lookup"><span data-stu-id="ac682-113">If the revenue method of the Opportunity summary is set to **System Calculated** , the customer budget values across product- and project-based lines are summarized to calculate the estimated revenue.</span></span>
