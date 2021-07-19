---
title: מבט כולל על מצבי ניהול משאבים
description: נושא זה מספק מידע על ניהול משאבים ב- Dynamics 365 Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.custom: intro-internal
ms.openlocfilehash: 41265534661e51565bf31105ef69cec9b3b181c3
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 07/07/2021
ms.locfileid: "6367892"
---
# <a name="resource-management-modes-overview"></a><span data-ttu-id="e817f-103">מבט כולל על מצבי ניהול משאבים</span><span class="sxs-lookup"><span data-stu-id="e817f-103">Resource management modes overview</span></span>

<span data-ttu-id="e817f-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="e817f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="e817f-105">Dynamics 365 Project Operations תומך בשני מצבים על מנת שתוכל לבצע את זרימת ההזמנות הכוללת.</span><span class="sxs-lookup"><span data-stu-id="e817f-105">Dynamics 365 Project Operations supports two modes in order for you to execute the overall booking flow.</span></span> <span data-ttu-id="e817f-106">מצב הניהול מוגדר כפרמטר פרויקט וניתן לשנותו אם הצרכים העסקיים שלך משתנים.</span><span class="sxs-lookup"><span data-stu-id="e817f-106">The mode of management is defined as a project parameter and can be modified if your business needs change.</span></span>    

## <a name="central-mode"></a><span data-ttu-id="e817f-107">מצב מרכזי</span><span class="sxs-lookup"><span data-stu-id="e817f-107">Central mode</span></span>
<span data-ttu-id="e817f-108">לארגונים שמרכזים את הקצאת המשאבים לפרויקטים, המצב המרכזי מספק דרך להבטיח שמנהלי הפרויקטים יוכלו להגדיר דרישות משאבים ברמת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="e817f-108">For organizations who centralize the allocation for resources to projects, the Central mode provides a way to ensure Project managers can define resource requirements at the project level.</span></span> <span data-ttu-id="e817f-109">מילוי דרישות המשאבים מוקצה למנהל משאבים.</span><span class="sxs-lookup"><span data-stu-id="e817f-109">Fulfillment of the resource requirements is delegated to a Resource manager.</span></span> <span data-ttu-id="e817f-110">מנהלי פרויקטים יכולים לקבל או לדחות משאבים המוצעים על-ידי מנהל המשאבים.</span><span class="sxs-lookup"><span data-stu-id="e817f-110">Project managers can accept or reject resources that are proposed by the Resource manager.</span></span>

![מצב מרכזי](./media/resource-management-central.png)

<span data-ttu-id="e817f-112">כדי לנהל משאבים במצב המרכזי, ראה:</span><span class="sxs-lookup"><span data-stu-id="e817f-112">To manage resources with the Central mode, see:</span></span>

- [<span data-ttu-id="e817f-113">הקצאת משאבים כלליים הניתנים להזמנה למשימה ויצירת דרישות משאבים</span><span class="sxs-lookup"><span data-stu-id="e817f-113">Assign generic bookable resources to a task and generate resource requirements</span></span>](/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="e817f-114">הזמנת משאבים בעלי שם מדרישות משאב</span><span class="sxs-lookup"><span data-stu-id="e817f-114">Book named resources from resource requirements</span></span>](/dynamics365/project-service/book-named-resource)
- [<span data-ttu-id="e817f-115">שליחת בקשת משאב</span><span class="sxs-lookup"><span data-stu-id="e817f-115">Submit a resource request</span></span>](/dynamics365/project-service/submit-resource-request)
- [<span data-ttu-id="e817f-116">מימוש בקשה למשאב</span><span class="sxs-lookup"><span data-stu-id="e817f-116">Fulfill a resource request</span></span>](/dynamics365/project-service/resource-management-fulfill-requests)
- [<span data-ttu-id="e817f-117">קבלה או דחייה של משאב פרויקט מוצע מבקשת משאב</span><span class="sxs-lookup"><span data-stu-id="e817f-117">Accept or reject a proposed project resource from a resource request</span></span>](/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a><span data-ttu-id="e817f-118">מצב היברידי</span><span class="sxs-lookup"><span data-stu-id="e817f-118">Hybrid mode</span></span>
<span data-ttu-id="e817f-119">לארגונים שנדרשת להם גמישות בהקצאת משאבים, המצב ההיברידי מאפשר גם למנהלי פרויקטים וגם למנהלי משאבים להזמין משאבים.</span><span class="sxs-lookup"><span data-stu-id="e817f-119">For organizations who require flexibility in the allocation of resources, the hybrid mode enables both Project managers and Resource managers the ability to book resources.</span></span>

![מצב היברידי](./media/resource-management-hybrid.png)

<span data-ttu-id="e817f-121">בנוסף לתהליך המצב המרכזי הנתמך, עיין בנושאים הבאים לניהול כל זרימות ההזמנות הנתמכות הנוספות במצב היברידי:</span><span class="sxs-lookup"><span data-stu-id="e817f-121">In addition to the supported Central mode process, see the following topics to manage all other supported booking flows in the Hybrid mode:</span></span>

<span data-ttu-id="e817f-122">הזמן משאב ישירות לפרויקט:</span><span class="sxs-lookup"><span data-stu-id="e817f-122">Book a resource directly to a project:</span></span>
- [<span data-ttu-id="e817f-123">הזמנת משאבים בעלי שם הניתנים להזמנה לצוות פרויקט והקצאת משימות</span><span class="sxs-lookup"><span data-stu-id="e817f-123">Book named bookable resources to a project team and assign tasks</span></span>](/dynamics365/project-service/assign-named-bookable-resource)

<span data-ttu-id="e817f-124">הזמן משאב מדרישות משאב:</span><span class="sxs-lookup"><span data-stu-id="e817f-124">Book a resource from a resource requirement:</span></span>
- [<span data-ttu-id="e817f-125">הקצאת משאבים כלליים הניתנים להזמנה למשימה ויצירת דרישות משאבים</span><span class="sxs-lookup"><span data-stu-id="e817f-125">Assign generic bookable resources to a task and generate resource requirements</span></span>](/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="e817f-126">הזמנת משאבים בעלי שם מדרישות משאב</span><span class="sxs-lookup"><span data-stu-id="e817f-126">Book named resources from resource requirements</span></span>](/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]