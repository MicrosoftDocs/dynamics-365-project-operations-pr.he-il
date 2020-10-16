---
title: שורות הצעת מחיר המבוססות על מוצר תמחיר
description: נושא זה מספק מידע על החלת מחיר עלות לשורות הצעת מחיר מבוססות מוצר.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 17b377eab5bcbc1a2327cb3ff87cc75d8de40953
ms.sourcegitcommit: a0f80d024a5d3112a39781815bd31d0c05ddaf6f
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/30/2020
ms.locfileid: "3906182"
---
# <a name="costing-product-based-quote-lines"></a><span data-ttu-id="6a931-103">שורות הצעת מחיר המבוססות על מוצר תמחיר</span><span class="sxs-lookup"><span data-stu-id="6a931-103">Costing product-based quote lines</span></span>

<span data-ttu-id="6a931-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="6a931-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="6a931-105">לשורות הצעות מחיר מבוססות מוצר ב-Dynamics 365 Project Operations יש גם שדה של **מחיר עלות**.</span><span class="sxs-lookup"><span data-stu-id="6a931-105">Product-based quote lines in Dynamics 365 Project Operations also have a **Cost Price** field.</span></span> <span data-ttu-id="6a931-106">שדה זה משמש למעקב אחר מחיר העלות של המוצר בשורת הצעת המחיר ולחישובי רווחיות במורד הזרם.</span><span class="sxs-lookup"><span data-stu-id="6a931-106">This field is used to track the cost price for the product on the quote line and for downstream profitability calculations.</span></span>

<span data-ttu-id="6a931-107">כאשר נוצרת שורת הצעת מחיר מבוססת מוצר עבור מוצר קטלוג, עלות שורת הצעת המחיר מבוססת כברירת מחדל על השדה **עלות תקנית** בקטלוג המוצרים.</span><span class="sxs-lookup"><span data-stu-id="6a931-107">When a product-based quote line is created for a catalog product, the cost of the product-based quote line is defaulted from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="6a931-108">השדה 'עלות תקנית' בקטלוג המוצרים מוגדר במטבע הבסיס של הארגון.</span><span class="sxs-lookup"><span data-stu-id="6a931-108">The standard cost field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="6a931-109">עלות ברירת המחדל ליחידת בשורת הצעת מחיר מבוססת מוצר מומרת למטבע המכירה בהצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="6a931-109">The default unit cost on the product-based quote line is converted to the sales currency on the quote.</span></span>

## <a name="unit-cost-on-a-product-based-quote-line"></a><span data-ttu-id="6a931-110">עלות יחידה בשורת הצעת מחיר מבוססות מוצר</span><span class="sxs-lookup"><span data-stu-id="6a931-110">Unit cost on a product-based quote line</span></span>

<span data-ttu-id="6a931-111">המטרה של עלות יחידה בשורת הצעת מחיר מבוססת מוצר היא לאפשר עלויות שונות עבור מוצר בכל מכירה.</span><span class="sxs-lookup"><span data-stu-id="6a931-111">The purpose of having a unit cost on a product-based quote line is to allow for different costs for a product for each sale.</span></span> <span data-ttu-id="6a931-112">זהו לא תרחיש טיפוסי, אך לפעמים הספק עלול להוזיל את עלות המוצר בהתאם ללקוח של המכירה הסופית.</span><span class="sxs-lookup"><span data-stu-id="6a931-112">This is not a typical scenario, but sometimes the cost of the product may be discounted by the supplier depending on the customer of the final sale.</span></span>

<span data-ttu-id="6a931-113">לדוגמה:</span><span class="sxs-lookup"><span data-stu-id="6a931-113">For example:</span></span>

<span data-ttu-id="6a931-114">Fabrikam Robotics מתקין זרועות רובוטיות בקווי הייצור של חברת A Datum.</span><span class="sxs-lookup"><span data-stu-id="6a931-114">Fabrikam Robotics is installing robotic arms at A Datum Corporation's assembly lines.</span></span> <span data-ttu-id="6a931-115">Fabrikam מספקת שירותי התקנה אך הזרועות הרובוטיות נרכשות מחברת Trey Robotics.</span><span class="sxs-lookup"><span data-stu-id="6a931-115">Fabrikam provides installation services but the robotic arms are procured from Trey robotics.</span></span> <span data-ttu-id="6a931-116">אם התקנת הזרועות הרובוטיות בחברת A Datum תפתח קהילה אנכית חדשה עבור הזרועות הרובוטיות של Trey, חברת Trey עשויה להעניק ל-Fabrikam הנחה מיוחדת על עסקה זו.</span><span class="sxs-lookup"><span data-stu-id="6a931-116">If the installation of robotic arms at A Datum Corporation opens a new industry vertical for Trey's robotic arms, Trey could give a special discount for this deal to Fabrikam.</span></span>

<span data-ttu-id="6a931-117">במקרה זה, Fabrikam תיצור שורת הצעת מחיר מבוססת מוצר עבור זרועות רובוטיות ותזין עלות מיוחדת ליחידה עבור הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="6a931-117">In this case, Fabrikam will create product-based quote line for Robotic Arms and input a special per unit cost for this quote.</span></span> <span data-ttu-id="6a931-118">עלות זו שונה מהעלות התקנית של הזרועות הרובוטיות של Trey.</span><span class="sxs-lookup"><span data-stu-id="6a931-118">This cost is different from the standard cost of Trey Robotic Arms.</span></span>
