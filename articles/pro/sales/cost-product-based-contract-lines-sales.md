---
title: סעיפי חוזה המבוססים על מוצר תמחיר
description: נושא זה מספק מידע אודות יצירת
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 7dfb9425174dddee52f9ee64f7a963e48a6bca70
ms.sourcegitcommit: 3a0c18823a7ad23df5aa3de272779313abe56c82
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/20/2020
ms.locfileid: "4077539"
---
# <a name="costing-product-based-contract-lines"></a><span data-ttu-id="98519-103">סעיפי חוזה המבוססים על מוצר תמחיר</span><span class="sxs-lookup"><span data-stu-id="98519-103">Costing product-based contract lines</span></span>

<span data-ttu-id="98519-104">_**חל על** : פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="98519-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="98519-105">סעיפי חוזה מבוססי מוצרים ב-Dynamics 365 Project Operations כוללים את השדה **מחיר עלות** , המאחסן את מחיר העלות של המוצר לצורך חישובי רווחיות במורד הזרם.</span><span class="sxs-lookup"><span data-stu-id="98519-105">Product-based contract lines in Dynamics 365 Project Operations include the **Cost Price** field, which stores the cost price of the product for downstream profitability calculations.</span></span>

<span data-ttu-id="98519-106">כאשר נוצר סעיף חוזה מבוסס מוצר עבור מוצר קטלוג, עלות סעיף החוזה מבוססת מוצר נקבע כברירת מחדל מהשדה **עלות סטנדרטית** שבקטלוג המוצרים.</span><span class="sxs-lookup"><span data-stu-id="98519-106">When a product-based contract line is created for a catalog product, the cost of the product-based contract line defaults from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="98519-107">השדה **עלות סטנדרטית** שבקטלוג המוצרים מוגדר במטבע הבסיס של הארגון.</span><span class="sxs-lookup"><span data-stu-id="98519-107">The **Standard Cost** field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="98519-108">כאשר ברירת המחדל של עלות היחידה נקבעת בסעיף החוזה, היא מומרת למטבע המכירות בחוזה.</span><span class="sxs-lookup"><span data-stu-id="98519-108">When the unit cost defaults on the contract line, it's converted into the sales currency on the contract.</span></span>

## <a name="unit-cost-on-a-product-based-contract-line"></a><span data-ttu-id="98519-109">עלות יחידה בסעיף חוזה מבוסס מוצר</span><span class="sxs-lookup"><span data-stu-id="98519-109">Unit cost on a product-based contract line</span></span>

<span data-ttu-id="98519-110">כאשר סעיף חוזה מבוסס מוצר כולל עלות יחידה, מתאפשרות עלויות מוצר שונות עבור כל מכירה של יחידה.</span><span class="sxs-lookup"><span data-stu-id="98519-110">Having a unit cost on a product-based contract line allows for different product costs for each sale of a unit.</span></span> <span data-ttu-id="98519-111">אמנם לא תמיד הכרחי, אך ישנם תרחישים מסוימים שבהם הספק עשוי להוזיל את עלות המוצר עבור הלקוח.</span><span class="sxs-lookup"><span data-stu-id="98519-111">While not always necessary, there are certain scenarios where the cost of the product may be discounted for the customer by the supplier.</span></span> <span data-ttu-id="98519-112">לפניך התרחיש הבא:</span><span class="sxs-lookup"><span data-stu-id="98519-112">Consider the following scenario:</span></span>

<span data-ttu-id="98519-113">Fabrikam Robotics מתקין זרועות רובוטיות בקווי הייצור של חברת Adatum.</span><span class="sxs-lookup"><span data-stu-id="98519-113">Fabrikam Robotics is installing robotic arms at Adatum Corporation's assembly lines.</span></span> <span data-ttu-id="98519-114">Fabrikam מספקת שירותי התקנה אך הזרועות הרובוטיות נרכשות מחברת Trey Research.</span><span class="sxs-lookup"><span data-stu-id="98519-114">Fabrikam provides installation services but the robotic arms are procured from Trey Research.</span></span> <span data-ttu-id="98519-115">אם התקנת הזרועות הרובוטיות בחברת Adatum תפתח קהילה אנכית חדשה עבור הזרועות הרובוטיות של Trey, היא עשויה להעניק ל-Fabrikam הנחה מיוחדת על עסקה זו.</span><span class="sxs-lookup"><span data-stu-id="98519-115">If the installation of robotic arms at Adatum Corporation opens a new industry vertical for Trey Research, they could offer a special discount for this deal to Fabrikam.</span></span> <span data-ttu-id="98519-116">במקרה זה, Fabrikam יוצרת סעיף חוזה מבוסס מוצרים עבור זרועות רובוטיות ומזינה עלות ליחידה עבור חוזה זה, שהיא שונה מהעלות הסטנדרטית של זרועות רובוטיות מחברת Trey Research.</span><span class="sxs-lookup"><span data-stu-id="98519-116">In this case, Fabrikam creates a product-based contract line for Robotic Arms and inputs a per unit cost for this contract that is different from the standard cost of robotic arms from Trey Research.</span></span>
