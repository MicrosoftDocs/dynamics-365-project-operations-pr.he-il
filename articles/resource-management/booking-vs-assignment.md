---
title: הזמנות לעומת הקצאות
description: נושא זה מספק מידע על ההבדלים שבין הזמנת משאבים והקצאות משאבים.
author: ruhercul
manager: Annbe
ms.date: 01/08/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 3aaf8dcbae0a5762879c2b1223eba3bdc33af1a7
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279904"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="e2b2c-103">הזמנות לעומת הקצאות</span><span class="sxs-lookup"><span data-stu-id="e2b2c-103">Bookings vs assignments</span></span>

<span data-ttu-id="e2b2c-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="e2b2c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e2b2c-105">הזמנות הן הקצאה בטוחה או טנטטיבית של משאבים לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="e2b2c-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="e2b2c-106">הזמנות בטוחות צורכות קיבולת של משאב.</span><span class="sxs-lookup"><span data-stu-id="e2b2c-106">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="e2b2c-107">הזמנות מייצגות מושגים ארגוניים עבור צוותים כדי שיוכלו להבין כיצד יועסקו משאבים בפרויקטים שונים.</span><span class="sxs-lookup"><span data-stu-id="e2b2c-107">Bookings represent organizational concepts for teams so that they can understand how resources will be engaged across various projects.</span></span> <span data-ttu-id="e2b2c-108">Dynamics 365 Project Operations רואה בהזמנות מושג ברמת הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="e2b2c-108">Dynamics 365 Project Operations considers bookings a project-level concept.</span></span> 

<span data-ttu-id="e2b2c-109">שלא כמו הזמנות, הקצאות הן הקצאה של משאבים למשימות פרויקט בלוח הזמנים של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="e2b2c-109">Unlike bookings, assignments are the commitment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="e2b2c-110">המשאבים יכולים להיות בעלי שם או כלליים.</span><span class="sxs-lookup"><span data-stu-id="e2b2c-110">The resources can be named or generic.</span></span>  <span data-ttu-id="e2b2c-111">כאשר דרישת משאבים נגזרת מהקצאת המשימות של הפרוייקט, Project Operations משתמש בקווי המתאר של הקצאת המשאבים כדי לבנות את קווי המתאר של פרטי דרישת המשאבים.</span><span class="sxs-lookup"><span data-stu-id="e2b2c-111">When a resource requirement is derived from the project task assignments, Project Operations uses the effort contours of the resources assignment to build the contours of the resource requirement details.</span></span> <span data-ttu-id="e2b2c-112">עם זאת, התייחסות להקצאות המשאבים אינה נשמרת.</span><span class="sxs-lookup"><span data-stu-id="e2b2c-112">However, a refence to the resource assignments isn't maintained.</span></span> <span data-ttu-id="e2b2c-113">עדכונים להזמנות שמקורם בדרישת המשאבים אינם מעדכנים את הקצאות המשאבים.</span><span class="sxs-lookup"><span data-stu-id="e2b2c-113">Updates to the bookings derived from the resource requirement don't update any resource assignments.</span></span>

<span data-ttu-id="e2b2c-114">בדרך כלל סך ההזמנות עבור משאב ישווה לסך המשימות של המשאב על פני משימה אחת או רבות.</span><span class="sxs-lookup"><span data-stu-id="e2b2c-114">Typically, the sum of the bookings for a resource will equal the sum of the resource's assignments across one or many tasks.</span></span> <span data-ttu-id="e2b2c-115">עם זאת, Project Operations אינו אוכף הסכם זה.</span><span class="sxs-lookup"><span data-stu-id="e2b2c-115">However, Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="e2b2c-116">התצוגה **התאמה** מציגה בפני מנהל פרויקט מקומות שבהם הזמנות וההקצאות של משאב אינן תואמות.</span><span class="sxs-lookup"><span data-stu-id="e2b2c-116">The **Reconciliation** view shows the Project manager places where a resource's bookings and assignments don't agree.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]