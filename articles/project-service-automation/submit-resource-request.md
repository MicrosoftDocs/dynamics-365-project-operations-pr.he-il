---
title: שלח בקשת משאב
description: נושא זה מספק מידע על שליחת בקשה עבור משאב פרוייקט.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 12/1/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
author: JohnPBurrows
ms.assetid: 9f4a6315-3905-4b15-8d06-e5dae30ccbb8
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 2b706ae25af5ba85647c98353b5950663fafc292
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751851"
---
# <a name="submit-a-resource-request"></a><span data-ttu-id="50525-103">שלח בקשת משאב</span><span class="sxs-lookup"><span data-stu-id="50525-103">Submit a resource request</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="50525-104">ניתן לשלוח דרישת משאב שנוצרה כבקשת משאב.</span><span class="sxs-lookup"><span data-stu-id="50525-104">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="50525-105">לאחר מכן הבקשה נשלחת למנהל משאבים לצורך מימוש.</span><span class="sxs-lookup"><span data-stu-id="50525-105">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="50525-106">ב- Project Service Automation‏ (PSA), בדף **פרוייקטים**, לחץ על הכרטיסיה **צוות** כדי להציג רשימה של משאבים הניתנים להזמנה.</span><span class="sxs-lookup"><span data-stu-id="50525-106">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab to view a list bookable resources.</span></span> 
2. <span data-ttu-id="50525-107">בחר את המשאב הכללי בעל דרישת משאב מהרשימה ולאחר מכן לחץ על **שלח בקשה**.</span><span class="sxs-lookup"><span data-stu-id="50525-107">Select the generic resource that has a resource requirement from the list and then click **Submit Request**.</span></span>

![שליחה של בקשת משאב](media/RM-how-to-18.png)

<span data-ttu-id="50525-109">מצב הבקשה של חבר הצוות הכללי ישתנה ל**נשלח**.</span><span class="sxs-lookup"><span data-stu-id="50525-109">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="50525-110">לאחר שהבקשה מומשה על-ידי מנהל המשאבים, המשאב הכללי יוחלף במשאב בעל שם אם מנהל המשאבים מממש את הבקשה בהזמנה של משאב בעל שם.</span><span class="sxs-lookup"><span data-stu-id="50525-110">After the request is fulfilled by the resource manager, the generic resource will be replaced by a named resource if the resource manager fulfills the request with the booking of a named resource.</span></span> <span data-ttu-id="50525-111">אחרת, המשאב הכללי יישאר בצוות ומצב הבקשה ישתנה ל**נחוצה סקירה**, אם מנהל המשאבים הציע משאב בעל שם.</span><span class="sxs-lookup"><span data-stu-id="50525-111">Otherwise, the generic resource will remain on the team and the request status will change to **Needs Review**, if the resource manager has proposed a named resource.</span></span>
