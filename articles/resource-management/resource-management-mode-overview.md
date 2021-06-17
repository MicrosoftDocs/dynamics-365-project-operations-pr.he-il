---
title: מבט כולל על מצבי ניהול משאבים
description: נושא זה מספק מידע על ניהול משאבים ב- Dynamics 365 Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 94db65a2ddbdc6a7226c70907bcce4c45b4a3923
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000887"
---
# <a name="resource-management-modes-overview"></a><span data-ttu-id="d26a0-103">מבט כולל על מצבי ניהול משאבים</span><span class="sxs-lookup"><span data-stu-id="d26a0-103">Resource management modes overview</span></span>

<span data-ttu-id="d26a0-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="d26a0-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="d26a0-105">Dynamics 365 Project Operations תומך בשני מצבים על מנת שתוכל לבצע את זרימת ההזמנות הכוללת.</span><span class="sxs-lookup"><span data-stu-id="d26a0-105">Dynamics 365 Project Operations supports two modes in order for you to execute the overall booking flow.</span></span> <span data-ttu-id="d26a0-106">מצב הניהול מוגדר כפרמטר פרויקט וניתן לשנותו אם הצרכים העסקיים שלך משתנים.</span><span class="sxs-lookup"><span data-stu-id="d26a0-106">The mode of management is defined as a project parameter and can be modified if your business needs change.</span></span>    

## <a name="central-mode"></a><span data-ttu-id="d26a0-107">מצב מרכזי</span><span class="sxs-lookup"><span data-stu-id="d26a0-107">Central mode</span></span>
<span data-ttu-id="d26a0-108">לארגונים שמרכזים את הקצאת המשאבים לפרויקטים, המצב המרכזי מספק דרך להבטיח שמנהלי הפרויקטים יוכלו להגדיר דרישות משאבים ברמת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="d26a0-108">For organizations who centralize the allocation for resources to projects, the Central mode provides a way to ensure Project managers can define resource requirements at the project level.</span></span> <span data-ttu-id="d26a0-109">מילוי דרישות המשאבים מוקצה למנהל משאבים.</span><span class="sxs-lookup"><span data-stu-id="d26a0-109">Fulfillment of the resource requirements is delegated to a Resource manager.</span></span> <span data-ttu-id="d26a0-110">מנהלי פרויקטים יכולים לקבל או לדחות משאבים המוצעים על-ידי מנהל המשאבים.</span><span class="sxs-lookup"><span data-stu-id="d26a0-110">Project managers can accept or reject resources that are proposed by the Resource manager.</span></span>

![מצב מרכזי](./media/resource-management-central.png)

<span data-ttu-id="d26a0-112">כדי לנהל משאבים במצב המרכזי, ראה:</span><span class="sxs-lookup"><span data-stu-id="d26a0-112">To manage resources with the Central mode, see:</span></span>

- [<span data-ttu-id="d26a0-113">הקצאת משאבים כלליים הניתנים להזמנה למשימה ויצירת דרישות משאבים</span><span class="sxs-lookup"><span data-stu-id="d26a0-113">Assign generic bookable resources to a task and generate resource requirements</span></span>](/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="d26a0-114">הזמנת משאבים בעלי שם מדרישות משאב</span><span class="sxs-lookup"><span data-stu-id="d26a0-114">Book named resources from resource requirements</span></span>](/dynamics365/project-service/book-named-resource)
- [<span data-ttu-id="d26a0-115">שליחת בקשת משאב</span><span class="sxs-lookup"><span data-stu-id="d26a0-115">Submit a resource request</span></span>](/dynamics365/project-service/submit-resource-request)
- [<span data-ttu-id="d26a0-116">מימוש בקשה למשאב</span><span class="sxs-lookup"><span data-stu-id="d26a0-116">Fulfill a resource request</span></span>](/dynamics365/project-service/resource-management-fulfill-requests)
- [<span data-ttu-id="d26a0-117">קבלה או דחייה של משאב פרויקט מוצע מבקשת משאב</span><span class="sxs-lookup"><span data-stu-id="d26a0-117">Accept or reject a proposed project resource from a resource request</span></span>](/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a><span data-ttu-id="d26a0-118">מצב היברידי</span><span class="sxs-lookup"><span data-stu-id="d26a0-118">Hybrid mode</span></span>
<span data-ttu-id="d26a0-119">לארגונים שנדרשת להם גמישות בהקצאת משאבים, המצב ההיברידי מאפשר גם למנהלי פרויקטים וגם למנהלי משאבים להזמין משאבים.</span><span class="sxs-lookup"><span data-stu-id="d26a0-119">For organizations who require flexibility in the allocation of resources, the hybrid mode enables both Project managers and Resource managers the ability to book resources.</span></span>

![מצב היברידי](./media/resource-management-hybrid.png)

<span data-ttu-id="d26a0-121">בנוסף לתהליך המצב המרכזי הנתמך, עיין בנושאים הבאים לניהול כל זרימות ההזמנות הנתמכות הנוספות במצב היברידי:</span><span class="sxs-lookup"><span data-stu-id="d26a0-121">In addition to the supported Central mode process, see the following topics to manage all other supported booking flows in the Hybrid mode:</span></span>

<span data-ttu-id="d26a0-122">הזמן משאב ישירות לפרויקט:</span><span class="sxs-lookup"><span data-stu-id="d26a0-122">Book a resource directly to a project:</span></span>
- [<span data-ttu-id="d26a0-123">הזמנת משאבים בעלי שם הניתנים להזמנה לצוות פרויקט והקצאת משימות</span><span class="sxs-lookup"><span data-stu-id="d26a0-123">Book named bookable resources to a project team and assign tasks</span></span>](/dynamics365/project-service/assign-named-bookable-resource)

<span data-ttu-id="d26a0-124">הזמן משאב מדרישות משאב:</span><span class="sxs-lookup"><span data-stu-id="d26a0-124">Book a resource from a resource requirement:</span></span>
- [<span data-ttu-id="d26a0-125">הקצאת משאבים כלליים הניתנים להזמנה למשימה ויצירת דרישות משאבים</span><span class="sxs-lookup"><span data-stu-id="d26a0-125">Assign generic bookable resources to a task and generate resource requirements</span></span>](/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="d26a0-126">הזמנת משאבים בעלי שם מדרישות משאב</span><span class="sxs-lookup"><span data-stu-id="d26a0-126">Book named resources from resource requirements</span></span>](/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]