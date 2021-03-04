---
title: שורות הזדמנות מבוססות מוצר - לייט
description: נושא זה מספק מידע על פרטים בשורות הזדמנות מבוססות מוצר ב-Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b826bf3a1320eee2758af7a094e9f1c2eac6a119
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764955"
---
# <a name="product-based-opportunity-lines---lite"></a><span data-ttu-id="db513-103">שורות הזדמנות מבוססות מוצר - לייט</span><span class="sxs-lookup"><span data-stu-id="db513-103">Product-based opportunity lines - lite</span></span>

<span data-ttu-id="db513-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="db513-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="db513-105">שורות הזדמנות מבוססות מוצר הן פריטי שורה בהזדמנות.</span><span class="sxs-lookup"><span data-stu-id="db513-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="db513-106">פריטי שורה נפרדים אלה נמצאים בחשבונית הסופית שמסופקת ללקוח.</span><span class="sxs-lookup"><span data-stu-id="db513-106">These distinct line items are on the eventual invoice that is provided to the customer.</span></span> <span data-ttu-id="db513-107">החשבונית אינה כוללת שירותים נוספים אחרים.</span><span class="sxs-lookup"><span data-stu-id="db513-107">The invoice doesn't include any other additional services.</span></span> <span data-ttu-id="db513-108">ההוצאות והצריכה במשוייכים אינם נמצאים במעקב במשימות של פרויקטים קשורים כלשהם.</span><span class="sxs-lookup"><span data-stu-id="db513-108">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="db513-109">שורות מבוססות מוצר יכולים להיות פריטי קטלוג או מוצרים שאינם מופיעים ברשימה.</span><span class="sxs-lookup"><span data-stu-id="db513-109">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="db513-110">מרבית הפונקציונליות בשורות מבוססות מוצר של הזדמנות מבוססת על הפונקציונליות ביישום Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="db513-110">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="db513-111">לקבלת מידע נוסף אודות שורות הזדמנות מבוססות מוצר, ראה[הוספת מוצרים להזדמנות](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="db513-111">For more information about product-based opportunity lines, see [Add products to an opportunity](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="db513-112">**תקציב הלקוח** הוא מושג ספציפי לשורות הזדמנויות מבוססות פרוייקטים.</span><span class="sxs-lookup"><span data-stu-id="db513-112">**Customer budget** is a concept that is specific to project-based opportunity lines.</span></span> <span data-ttu-id="db513-113">השדה **תקציב לקוח** עוקב אחר הסכום שהלקוח מוכן לשלם עבור הפריט.</span><span class="sxs-lookup"><span data-stu-id="db513-113">The **Customer budget** field tracks the amount the customer is willing to pay for the item.</span></span>

<span data-ttu-id="db513-114">כאשר שיטת ההכנסות של סיכום ההזדמנויות היא **מחושב על ידי המערכת**, ערכי תקציב הלקוח בכל שורות ההזדמנות מסוכמים לחישוב ההכנסות המשוערות.</span><span class="sxs-lookup"><span data-stu-id="db513-114">When the revenue method of the Opportunity summary is **System Calculated**, the customer budget values across the opportunity lines are summarized to calculate the estimated revenue.</span></span> 

