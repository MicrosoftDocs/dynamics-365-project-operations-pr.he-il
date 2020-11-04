---
title: שליחה של בקשת משאב
description: נושא זה מספק מידע על שליחת בקשה עבור משאב פרויקט.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 12/1/2018
ms.topic: article
author: JohnPBurrows
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: bcea3d640d7e9ee2b071c55bff9ade3268edb319
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077401"
---
# <a name="submitting-a-resource-request"></a><span data-ttu-id="d85d8-103">שליחה של בקשת משאב</span><span class="sxs-lookup"><span data-stu-id="d85d8-103">Submitting a resource request</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="d85d8-104">ניתן לשלוח דרישת משאב שנוצרה כבקשת משאב.</span><span class="sxs-lookup"><span data-stu-id="d85d8-104">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="d85d8-105">לאחר מכן הבקשה נשלחת למנהל משאבים לצורך מימוש.</span><span class="sxs-lookup"><span data-stu-id="d85d8-105">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="d85d8-106">ב- Project Service Automation‏ (PSA), בדף **פרויקטים** , לחץ על הכרטיסיה **צוות** כדי להציג רשימה של משאבים הניתנים להזמנה.</span><span class="sxs-lookup"><span data-stu-id="d85d8-106">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab to view a list bookable resources.</span></span> 
2. <span data-ttu-id="d85d8-107">בחר את המשאב הכללי בעל דרישת משאב מהרשימה ולאחר מכן לחץ על **שלח בקשה**.</span><span class="sxs-lookup"><span data-stu-id="d85d8-107">Select the generic resource that has a resource requirement from the list and then click **Submit Request**.</span></span>

![שליחה של בקשת משאב](media/RM-how-to-18.png)

<span data-ttu-id="d85d8-109">מצב הבקשה של חבר הצוות הכללי ישתנה ל **נשלח**.</span><span class="sxs-lookup"><span data-stu-id="d85d8-109">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="d85d8-110">לאחר שהבקשה מומשה על-ידי מנהל המשאבים, המשאב הכללי יוחלף במשאב בעל שם אם מנהל המשאבים מממש את הבקשה בהזמנה של משאב בעל שם.</span><span class="sxs-lookup"><span data-stu-id="d85d8-110">After the request is fulfilled by the resource manager, the generic resource will be replaced by a named resource if the resource manager fulfills the request with the booking of a named resource.</span></span> <span data-ttu-id="d85d8-111">אחרת, המשאב הכללי יישאר בצוות ומצב הבקשה ישתנה ל **נחוצה סקירה** , אם מנהל המשאבים הציע משאב בעל שם.</span><span class="sxs-lookup"><span data-stu-id="d85d8-111">Otherwise, the generic resource will remain on the team and the request status will change to **Needs Review** , if the resource manager has proposed a named resource.</span></span>
