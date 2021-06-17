---
title: סעיפי חוזה מבוססי מוצר של עלות - לייט
description: נושא זה מספק מידע אודות יצירת
author: rumant
ms.date: 10/19/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 9458a57863244a68359f57185325c03a46bd6569
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003542"
---
# <a name="cost-product-based-contract-lines---lite"></a><span data-ttu-id="3c2d3-103">סעיפי חוזה מבוססי מוצר של עלות - לייט</span><span class="sxs-lookup"><span data-stu-id="3c2d3-103">Cost product-based contract lines - lite</span></span>

<span data-ttu-id="3c2d3-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="3c2d3-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="3c2d3-105">סעיפי חוזה שמבוססים על מוצר ב- Dynamics 365 Project Operations כוללים את השדה **מחיר עלות**, המאחסן את מחיר העלות של המוצר לצורך חישובי רווחיות במורד הזרם.</span><span class="sxs-lookup"><span data-stu-id="3c2d3-105">Product-based contract lines in Dynamics 365 Project Operations include the **Cost Price** field, which stores the cost price of the product for downstream profitability calculations.</span></span>

<span data-ttu-id="3c2d3-106">כאשר נוצר סעיף חוזה שמבוסס על מוצר עבור מוצר קטלוג, עלות הסעיף היא ברירת המחדל מהשדה **מחיר רגיל** בקטלוג המוצרים.</span><span class="sxs-lookup"><span data-stu-id="3c2d3-106">When a product-based contract line is created for a catalog product, the cost of the line defaults from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="3c2d3-107">השדה **עלות סטנדרטית** שבקטלוג המוצרים מוגדר במטבע הבסיס של הארגון.</span><span class="sxs-lookup"><span data-stu-id="3c2d3-107">The **Standard Cost** field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="3c2d3-108">כאשר ברירת המחדל של עלות היחידה נקבעת בסעיף החוזה, היא מומרת למטבע המכירות בחוזה.</span><span class="sxs-lookup"><span data-stu-id="3c2d3-108">When the unit cost defaults on the contract line, it's converted into the sales currency on the contract.</span></span>

## <a name="unit-cost-on-a-product-based-contract-line"></a><span data-ttu-id="3c2d3-109">עלות יחידה בסעיף חוזה מבוסס מוצר</span><span class="sxs-lookup"><span data-stu-id="3c2d3-109">Unit cost on a product-based contract line</span></span>

<span data-ttu-id="3c2d3-110">כאשר סעיף חוזה מבוסס מוצר כולל עלות יחידה, מתאפשרות עלויות מוצר שונות עבור כל מכירה של יחידה.</span><span class="sxs-lookup"><span data-stu-id="3c2d3-110">Having a unit cost on a product-based contract line allows for different product costs for each sale of a unit.</span></span> <span data-ttu-id="3c2d3-111">אמנם לא תמיד הכרחי, אך ישנם תרחישים מסוימים שבהם הספק עשוי להוזיל את עלות המוצר עבור הלקוח.</span><span class="sxs-lookup"><span data-stu-id="3c2d3-111">While not always necessary, there are certain scenarios where the cost of the product may be discounted for the customer by the supplier.</span></span> <span data-ttu-id="3c2d3-112">לפניך התרחיש הבא:</span><span class="sxs-lookup"><span data-stu-id="3c2d3-112">Consider the following scenario:</span></span>

<span data-ttu-id="3c2d3-113">Fabrikam Robotics מתקין זרועות רובוטיות בקווי הייצור של חברת Adatum.</span><span class="sxs-lookup"><span data-stu-id="3c2d3-113">Fabrikam Robotics is installing robotic arms at Adatum Corporation's assembly lines.</span></span> <span data-ttu-id="3c2d3-114">Fabrikam מספקת שירותי התקנה אך הזרועות הרובוטיות הן של Trey Research.</span><span class="sxs-lookup"><span data-stu-id="3c2d3-114">Fabrikam provides installation services but the robotic arms are from Trey Research.</span></span> <span data-ttu-id="3c2d3-115">אם התקנת הזרועות הרובוטיות בחברת Adatum תפתח קהילה אנכית חדשה עבור הזרועות הרובוטיות של Trey, היא עשויה להעניק ל-Fabrikam הנחה מיוחדת על עסקה זו.</span><span class="sxs-lookup"><span data-stu-id="3c2d3-115">If the installation of robotic arms at Adatum Corporation opens a new industry vertical for Trey Research, they could offer a special discount for this deal to Fabrikam.</span></span> <span data-ttu-id="3c2d3-116">במקרה זה, Fabrikam יוצר סעיף חוזה מבוסס מוצרים עבור Robotic Arms.</span><span class="sxs-lookup"><span data-stu-id="3c2d3-116">In this case, Fabrikam creates a product-based contract line for Robotic Arms.</span></span> <span data-ttu-id="3c2d3-117">עלות ליחידה מוזנת עבור חוזה זה.</span><span class="sxs-lookup"><span data-stu-id="3c2d3-117">A per unit cost is entered for this contract.</span></span> <span data-ttu-id="3c2d3-118">העלות שונה מעלות הזרועות הרובוטיות מ- Robotic Arms.</span><span class="sxs-lookup"><span data-stu-id="3c2d3-118">The cost is different from the cost of robotic arms from Trey Research.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]