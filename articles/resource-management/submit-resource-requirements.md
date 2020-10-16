---
title: שליחת בקשת משאב
description: ניתן לשלוח דרישת משאב שנוצרה כבקשת משאב. לאחר מכן הבקשה נשלחת למנהל משאבים לצורך מימוש.
author: ruhercul
manager: Annbe
ms.date: 10/04/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 94cf0f0d88e9be2522936b45122ed0037434d4f3
ms.sourcegitcommit: 2cf93d8bf0be5b61a739195a41334c34d910e9ba
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961710"
---
# <a name="submit-a-resource-request"></a><span data-ttu-id="64d97-104">שליחת בקשת משאב</span><span class="sxs-lookup"><span data-stu-id="64d97-104">Submit a resource request</span></span>

<span data-ttu-id="64d97-105">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="64d97-105">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="64d97-106">ניתן לשלוח דרישת משאב שנוצרה כבקשת משאב.</span><span class="sxs-lookup"><span data-stu-id="64d97-106">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="64d97-107">לאחר מכן הבקשה נשלחת למנהל משאבים לצורך מימוש.</span><span class="sxs-lookup"><span data-stu-id="64d97-107">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="64d97-108">ב- Dynamics 365 Project Operations, בדף **פרוייקטים**, בחר בכרטיסיה **צוות** כדי להציג רשימה של משאבים הניתנים להזמנה.</span><span class="sxs-lookup"><span data-stu-id="64d97-108">In Dynamics 365 Project Operations, on the **Projects** page, select the **Team** tab to view a list of bookable resources.</span></span> 
2. <span data-ttu-id="64d97-109">בחר ברשימה את המשאב הכללי בעל דרישת משאב ולחץ על **שלח בקשה**.</span><span class="sxs-lookup"><span data-stu-id="64d97-109">Select the generic resource that has a resource requirement from the list, and then click **Submit Request**.</span></span>

<span data-ttu-id="64d97-110">מצב הבקשה של חבר הצוות הכללי ישתנה ל**נשלח**.</span><span class="sxs-lookup"><span data-stu-id="64d97-110">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="64d97-111">לאחר מימוש הבקשה, המשאב הכללי מוחלף במשאב בעל שם אם מנהל המשאבים מממש את הבקשה על-ידי הזמנה של משאב בעל שם.</span><span class="sxs-lookup"><span data-stu-id="64d97-111">After the request is fulfilled, the generic resource is replaced by a named resource if the resource manager fulfills the request by booking a named resource.</span></span> <span data-ttu-id="64d97-112">אחרת, אם מנהל המשאבים מציע משאב בעל שם, המשאב הכללי נשאר בצוות ומצב הבקשה משתנה ל**נחוצה סקירה**.</span><span class="sxs-lookup"><span data-stu-id="64d97-112">Otherwise, if the resource manager proposes a named resource, the generic resource remains on the team and the request status will change to **Needs Review**.</span></span>
