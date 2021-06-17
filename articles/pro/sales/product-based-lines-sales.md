---
title: שורות הזדמנות מבוססות מוצר - לייט
description: נושא זה מספק מידע על פרטים בשורות הזדמנות מבוססות מוצר ב-Project Operations.
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 7865da682ae607f017bf59ce1ae1addc9fefa60b
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994497"
---
# <a name="product-based-opportunity-lines---lite"></a><span data-ttu-id="b32b6-103">שורות הזדמנות מבוססות מוצר - לייט</span><span class="sxs-lookup"><span data-stu-id="b32b6-103">Product-based opportunity lines - lite</span></span>

<span data-ttu-id="b32b6-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="b32b6-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b32b6-105">שורות הזדמנות מבוססות מוצר הן פריטי שורה בהזדמנות.</span><span class="sxs-lookup"><span data-stu-id="b32b6-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="b32b6-106">פריטי שורה נפרדים אלה נמצאים בחשבונית הסופית שמסופקת ללקוח.</span><span class="sxs-lookup"><span data-stu-id="b32b6-106">These distinct line items are on the eventual invoice that is provided to the customer.</span></span> <span data-ttu-id="b32b6-107">החשבונית אינה כוללת שירותים נוספים אחרים.</span><span class="sxs-lookup"><span data-stu-id="b32b6-107">The invoice doesn't include any other additional services.</span></span> <span data-ttu-id="b32b6-108">ההוצאות והצריכה במשוייכים אינם נמצאים במעקב במשימות של פרויקטים קשורים כלשהם.</span><span class="sxs-lookup"><span data-stu-id="b32b6-108">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="b32b6-109">שורות מבוססות מוצר יכולים להיות פריטי קטלוג או מוצרים שאינם מופיעים ברשימה.</span><span class="sxs-lookup"><span data-stu-id="b32b6-109">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="b32b6-110">מרבית הפונקציונליות בשורות מבוססות מוצר של הזדמנות מבוססת על הפונקציונליות ביישום Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="b32b6-110">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="b32b6-111">לקבלת מידע נוסף אודות שורות הזדמנות מבוססות מוצר, ראה[הוספת מוצרים להזדמנות](/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="b32b6-111">For more information about product-based opportunity lines, see [Add products to an opportunity](/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="b32b6-112">**תקציב הלקוח** הוא מושג ספציפי לשורות הזדמנויות מבוססות פרוייקטים.</span><span class="sxs-lookup"><span data-stu-id="b32b6-112">**Customer budget** is a concept that is specific to project-based opportunity lines.</span></span> <span data-ttu-id="b32b6-113">השדה **תקציב לקוח** עוקב אחר הסכום שהלקוח מוכן לשלם עבור הפריט.</span><span class="sxs-lookup"><span data-stu-id="b32b6-113">The **Customer budget** field tracks the amount the customer is willing to pay for the item.</span></span>

<span data-ttu-id="b32b6-114">כאשר שיטת ההכנסות של סיכום ההזדמנויות היא **מחושב על ידי המערכת**, ערכי תקציב הלקוח בכל שורות ההזדמנות מסוכמים לחישוב ההכנסות המשוערות.</span><span class="sxs-lookup"><span data-stu-id="b32b6-114">When the revenue method of the Opportunity summary is **System Calculated**, the customer budget values across the opportunity lines are summarized to calculate the estimated revenue.</span></span> 



[!INCLUDE[footer-include](../../includes/footer-banner.md)]