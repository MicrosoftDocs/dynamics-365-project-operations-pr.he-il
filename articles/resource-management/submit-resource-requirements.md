---
title: שליחת בקשת משאב
description: ניתן לשלוח דרישת משאב שנוצרה כבקשת משאב. לאחר מכן הבקשה נשלחת למנהל משאבים לצורך מימוש.
author: ruhercul
ms.date: 10/04/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 6ac0044a27d1e506c9c62c477014017fd0ca06cb
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6014027"
---
# <a name="submit-a-resource-request"></a><span data-ttu-id="a44b9-104">שליחת בקשת משאב</span><span class="sxs-lookup"><span data-stu-id="a44b9-104">Submit a resource request</span></span>

<span data-ttu-id="a44b9-105">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="a44b9-105">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a44b9-106">ניתן לשלוח דרישת משאב שנוצרה כבקשת משאב.</span><span class="sxs-lookup"><span data-stu-id="a44b9-106">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="a44b9-107">לאחר מכן הבקשה נשלחת למנהל משאבים לצורך מימוש.</span><span class="sxs-lookup"><span data-stu-id="a44b9-107">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="a44b9-108">ב- Dynamics 365 Project Operations, בדף **פרויקטים**, בחר את הכרטיסיה **צוות** כדי להציג רשימה של משאבים הניתנים להזמנה.</span><span class="sxs-lookup"><span data-stu-id="a44b9-108">In Dynamics 365 Project Operations, on the **Projects** page, select the **Team** tab to view a list of bookable resources.</span></span> 
2. <span data-ttu-id="a44b9-109">בחר ברשימה את המשאב הכללי בעל דרישת משאב ולחץ על **שלח בקשה**.</span><span class="sxs-lookup"><span data-stu-id="a44b9-109">Select the generic resource that has a resource requirement from the list, and then click **Submit Request**.</span></span>

<span data-ttu-id="a44b9-110">מצב הבקשה של חבר הצוות הכללי ישתנה ל **נשלח**.</span><span class="sxs-lookup"><span data-stu-id="a44b9-110">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="a44b9-111">לאחר מימוש הבקשה, המשאב הכללי מוחלף במשאב בעל שם אם מנהל המשאבים מממש את הבקשה על-ידי הזמנה של משאב בעל שם.</span><span class="sxs-lookup"><span data-stu-id="a44b9-111">After the request is fulfilled, the generic resource is replaced by a named resource if the resource manager fulfills the request by booking a named resource.</span></span> <span data-ttu-id="a44b9-112">אחרת, אם מנהל המשאבים מציע משאב בעל שם, המשאב הכללי נשאר בצוות ומצב הבקשה משתנה ל **נחוצה סקירה**.</span><span class="sxs-lookup"><span data-stu-id="a44b9-112">Otherwise, if the resource manager proposes a named resource, the generic resource remains on the team and the request status will change to **Needs Review**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]