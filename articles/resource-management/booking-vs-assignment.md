---
title: הזמנות לעומת הקצאות
description: נושא זה מספק מידע על ההבדלים שבין הזמנת משאבים והקצאות משאבים.
author: ruhercul
ms.date: 01/08/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 3c1a1003af0b23c4be44fefac0b3c4ea725f96b2
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012767"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="617b2-103">הזמנות לעומת הקצאות</span><span class="sxs-lookup"><span data-stu-id="617b2-103">Bookings vs assignments</span></span>

<span data-ttu-id="617b2-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="617b2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="617b2-105">הזמנות הן הקצאה בטוחה או טנטטיבית של משאבים לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="617b2-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="617b2-106">הזמנות בטוחות צורכות קיבולת של משאב.</span><span class="sxs-lookup"><span data-stu-id="617b2-106">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="617b2-107">הזמנות מייצגות מושגים ארגוניים עבור צוותים כדי שיוכלו להבין כיצד יועסקו משאבים בפרויקטים שונים.</span><span class="sxs-lookup"><span data-stu-id="617b2-107">Bookings represent organizational concepts for teams so that they can understand how resources will be engaged across various projects.</span></span> <span data-ttu-id="617b2-108">Dynamics 365 Project Operations רואה בהזמנות מושג ברמת הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="617b2-108">Dynamics 365 Project Operations considers bookings a project-level concept.</span></span> 

<span data-ttu-id="617b2-109">שלא כמו הזמנות, הקצאות הן הקצאה של משאבים למשימות פרויקט בלוח הזמנים של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="617b2-109">Unlike bookings, assignments are the commitment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="617b2-110">המשאבים יכולים להיות בעלי שם או כלליים.</span><span class="sxs-lookup"><span data-stu-id="617b2-110">The resources can be named or generic.</span></span>  <span data-ttu-id="617b2-111">כאשר דרישת משאבים נגזרת מהקצאת המשימות של הפרוייקט, Project Operations משתמש בקווי המתאר של הקצאת המשאבים כדי לבנות את קווי המתאר של פרטי דרישת המשאבים.</span><span class="sxs-lookup"><span data-stu-id="617b2-111">When a resource requirement is derived from the project task assignments, Project Operations uses the effort contours of the resources assignment to build the contours of the resource requirement details.</span></span> <span data-ttu-id="617b2-112">עם זאת, התייחסות להקצאות המשאבים אינה נשמרת.</span><span class="sxs-lookup"><span data-stu-id="617b2-112">However, a refence to the resource assignments isn't maintained.</span></span> <span data-ttu-id="617b2-113">עדכונים להזמנות שמקורם בדרישת המשאבים אינם מעדכנים את הקצאות המשאבים.</span><span class="sxs-lookup"><span data-stu-id="617b2-113">Updates to the bookings derived from the resource requirement don't update any resource assignments.</span></span>

<span data-ttu-id="617b2-114">בדרך כלל סך ההזמנות עבור משאב ישווה לסך המשימות של המשאב על פני משימה אחת או רבות.</span><span class="sxs-lookup"><span data-stu-id="617b2-114">Typically, the sum of the bookings for a resource will equal the sum of the resource's assignments across one or many tasks.</span></span> <span data-ttu-id="617b2-115">עם זאת, Project Operations אינו אוכף הסכם זה.</span><span class="sxs-lookup"><span data-stu-id="617b2-115">However, Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="617b2-116">התצוגה **התאמה** מציגה בפני מנהל פרויקט מקומות שבהם הזמנות וההקצאות של משאב אינן תואמות.</span><span class="sxs-lookup"><span data-stu-id="617b2-116">The **Reconciliation** view shows the Project manager places where a resource's bookings and assignments don't agree.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]