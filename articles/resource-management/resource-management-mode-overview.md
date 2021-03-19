---
title: מבט כולל על מצבי ניהול משאבים
description: נושא זה מספק מידע על ניהול משאבים ב- Dynamics 365 Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 872f4f2878f474e16674932f23fe192c6a8de6eb
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279454"
---
# <a name="resource-management-modes-overview"></a><span data-ttu-id="263a2-103">מבט כולל על מצבי ניהול משאבים</span><span class="sxs-lookup"><span data-stu-id="263a2-103">Resource management modes overview</span></span>

<span data-ttu-id="263a2-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="263a2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="263a2-105">Dynamics 365 Project Operations תומך בשני מצבים על מנת שתוכל לבצע את זרימת ההזמנות הכוללת.</span><span class="sxs-lookup"><span data-stu-id="263a2-105">Dynamics 365 Project Operations supports two modes in order for you to execute the overall booking flow.</span></span> <span data-ttu-id="263a2-106">מצב הניהול מוגדר כפרמטר פרויקט וניתן לשנותו אם הצרכים העסקיים שלך משתנים.</span><span class="sxs-lookup"><span data-stu-id="263a2-106">The mode of management is defined as a project parameter and can be modified if your business needs change.</span></span>    

## <a name="central-mode"></a><span data-ttu-id="263a2-107">מצב מרכזי</span><span class="sxs-lookup"><span data-stu-id="263a2-107">Central mode</span></span>
<span data-ttu-id="263a2-108">לארגונים שמרכזים את הקצאת המשאבים לפרויקטים, המצב המרכזי מספק דרך להבטיח שמנהלי הפרויקטים יוכלו להגדיר דרישות משאבים ברמת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="263a2-108">For organizations who centralize the allocation for resources to projects, the Central mode provides a way to ensure Project managers can define resource requirements at the project level.</span></span> <span data-ttu-id="263a2-109">מילוי דרישות המשאבים מוקצה למנהל משאבים.</span><span class="sxs-lookup"><span data-stu-id="263a2-109">Fulfillment of the resource requirements is delegated to a Resource manager.</span></span> <span data-ttu-id="263a2-110">מנהלי פרויקטים יכולים לקבל או לדחות משאבים המוצעים על-ידי מנהל המשאבים.</span><span class="sxs-lookup"><span data-stu-id="263a2-110">Project managers can accept or reject resources that are proposed by the Resource manager.</span></span>

![מצב מרכזי](./media/resource-management-central.png)

<span data-ttu-id="263a2-112">כדי לנהל משאבים במצב המרכזי, ראה:</span><span class="sxs-lookup"><span data-stu-id="263a2-112">To manage resources with the Central mode, see:</span></span>

- [<span data-ttu-id="263a2-113">הקצאת משאבים כלליים הניתנים להזמנה למשימה ויצירת דרישות משאבים</span><span class="sxs-lookup"><span data-stu-id="263a2-113">Assign generic bookable resources to a task and generate resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="263a2-114">הזמנת משאבים בעלי שם מדרישות משאב</span><span class="sxs-lookup"><span data-stu-id="263a2-114">Book named resources from resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
- [<span data-ttu-id="263a2-115">שליחת בקשת משאב</span><span class="sxs-lookup"><span data-stu-id="263a2-115">Submit a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/submit-resource-request)
- [<span data-ttu-id="263a2-116">מימוש בקשה למשאב</span><span class="sxs-lookup"><span data-stu-id="263a2-116">Fulfill a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/resource-management-fulfill-requests)
- [<span data-ttu-id="263a2-117">קבלה או דחייה של משאב פרויקט מוצע מבקשת משאב</span><span class="sxs-lookup"><span data-stu-id="263a2-117">Accept or reject a proposed project resource from a resource request</span></span>](https://docs.microsoft.com/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a><span data-ttu-id="263a2-118">מצב היברידי</span><span class="sxs-lookup"><span data-stu-id="263a2-118">Hybrid mode</span></span>
<span data-ttu-id="263a2-119">לארגונים שנדרשת להם גמישות בהקצאת משאבים, המצב ההיברידי מאפשר גם למנהלי פרויקטים וגם למנהלי משאבים להזמין משאבים.</span><span class="sxs-lookup"><span data-stu-id="263a2-119">For organizations who require flexibility in the allocation of resources, the hybrid mode enables both Project managers and Resource managers the ability to book resources.</span></span>

![מצב היברידי](./media/resource-management-hybrid.png)

<span data-ttu-id="263a2-121">בנוסף לתהליך המצב המרכזי הנתמך, עיין בנושאים הבאים לניהול כל זרימות ההזמנות הנתמכות הנוספות במצב היברידי:</span><span class="sxs-lookup"><span data-stu-id="263a2-121">In addition to the supported Central mode process, see the following topics to manage all other supported booking flows in the Hybrid mode:</span></span>

<span data-ttu-id="263a2-122">הזמן משאב ישירות לפרויקט:</span><span class="sxs-lookup"><span data-stu-id="263a2-122">Book a resource directly to a project:</span></span>
- [<span data-ttu-id="263a2-123">הזמנת משאבים בעלי שם הניתנים להזמנה לצוות פרויקט והקצאת משימות</span><span class="sxs-lookup"><span data-stu-id="263a2-123">Book named bookable resources to a project team and assign tasks</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-named-bookable-resource)

<span data-ttu-id="263a2-124">הזמן משאב מדרישות משאב:</span><span class="sxs-lookup"><span data-stu-id="263a2-124">Book a resource from a resource requirement:</span></span>
- [<span data-ttu-id="263a2-125">הקצאת משאבים כלליים הניתנים להזמנה למשימה ויצירת דרישות משאבים</span><span class="sxs-lookup"><span data-stu-id="263a2-125">Assign generic bookable resources to a task and generate resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="263a2-126">הזמנת משאבים בעלי שם מדרישות משאב</span><span class="sxs-lookup"><span data-stu-id="263a2-126">Book named resources from resource requirements</span></span>](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]