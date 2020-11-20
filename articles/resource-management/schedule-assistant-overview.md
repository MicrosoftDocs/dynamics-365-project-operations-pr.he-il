---
title: מבט כולל על מסייע לוחות זמנים
description: נושא זה מספק מידע על עבודה עם מסייע לוחות הזמנים להזמנת משאבים.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 92b12bd9272805a736286bf7e0ff926cb6361c05
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4125629"
---
# <a name="schedule-assistant-overview"></a><span data-ttu-id="c473c-103">מבט כולל על מסייע לוחות זמנים</span><span class="sxs-lookup"><span data-stu-id="c473c-103">Schedule assistant overview</span></span>

<span data-ttu-id="c473c-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="c473c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c473c-105">מסייע לוחות הזמנים משמש להזמנת משאבים על סמך דרישות שהוגדרו על-ידי מנהל הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="c473c-105">The Schedule assistant is used to book resources based on requirements defined by the Project manager.</span></span> <span data-ttu-id="c473c-106">מסייע לוחות הזמנים מסתמך על הפרמטרים המסופקים בדרישת המשאבים כדי למצוא את המשאב.</span><span class="sxs-lookup"><span data-stu-id="c473c-106">The schedule assistant relies on the parameters provided in the resource requirement to find the resource.</span></span> <span data-ttu-id="c473c-107">מסייע לוחות הזמנים ממליץ על משאבים התואמים לדרישות רלוונטיות, כמו חלונות זמן או כישורים נדרשים.</span><span class="sxs-lookup"><span data-stu-id="c473c-107">The Schedule assistant recommends resources that match relevant requirements, like time windows or skills needed.</span></span>

<span data-ttu-id="c473c-108">לאחר זיהוי משאבים מתאימים, מנהל המשאבים או מנהל הפרויקט יכולים להזמין את המשאב לעבודה.</span><span class="sxs-lookup"><span data-stu-id="c473c-108">After suitable resources are identified, the Resource or Project manager can book the resource to the work.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c473c-109">דרישות מוקדמות</span><span class="sxs-lookup"><span data-stu-id="c473c-109">Prerequisites</span></span>

<span data-ttu-id="c473c-110">מסייע לוחות הזמנים הוא חלק מהפתרון Universal Resource Scheduling.</span><span class="sxs-lookup"><span data-stu-id="c473c-110">The Schedule assistant is a part of the Universal Resource Scheduling solution.</span></span> <span data-ttu-id="c473c-111">פתרון זה נכלל ומותקן עם Dynamic 365 Project Operations‏, Dynamics 365 Field Service ו- Dynamics 365 Customer Service.</span><span class="sxs-lookup"><span data-stu-id="c473c-111">This solution is included and installed with Dynamics 365 Project Operations, Dynamics 365 Field Service, and Dynamics 365 Customer Service.</span></span>

## <a name="matching-requirements-and-resources"></a><span data-ttu-id="c473c-112">התאמת דרישות ומשאבים</span><span class="sxs-lookup"><span data-stu-id="c473c-112">Matching requirements and resources</span></span>

<span data-ttu-id="c473c-113">דרישת המשאבים שנוצרת מבוססת על פרטים כגון:</span><span class="sxs-lookup"><span data-stu-id="c473c-113">A generated resource requirement is based on details such as:</span></span>

-   <span data-ttu-id="c473c-114">מאפיינים</span><span class="sxs-lookup"><span data-stu-id="c473c-114">Characteristics</span></span>
-   <span data-ttu-id="c473c-115">תפקידים</span><span class="sxs-lookup"><span data-stu-id="c473c-115">Roles</span></span>
-   <span data-ttu-id="c473c-116">יחידות עסקיות</span><span class="sxs-lookup"><span data-stu-id="c473c-116">Business units</span></span>
-   <span data-ttu-id="c473c-117">העדפות משאב</span><span class="sxs-lookup"><span data-stu-id="c473c-117">Resource preferences</span></span>
-   <span data-ttu-id="c473c-118">קווי מתאר של מאמץ</span><span class="sxs-lookup"><span data-stu-id="c473c-118">Effort contours</span></span>
-   <span data-ttu-id="c473c-119">אזור זמן</span><span class="sxs-lookup"><span data-stu-id="c473c-119">Time zone</span></span>

<span data-ttu-id="c473c-120">מסייע לוחות הזמנים משתמש בפרטים אלה לסינון משאבים.</span><span class="sxs-lookup"><span data-stu-id="c473c-120">The Schedule assistant uses these details to filter resources.</span></span>

## <a name="launch-the-schedule-assistant"></a><span data-ttu-id="c473c-121">הפעל את מסייע לוחות הזמנים</span><span class="sxs-lookup"><span data-stu-id="c473c-121">Launch the Schedule assistant</span></span>

<span data-ttu-id="c473c-122">ישנן שתי דרכים בהן ניתן להפעיל את מסייע לוחות הזמנים.</span><span class="sxs-lookup"><span data-stu-id="c473c-122">There are two ways in which the schedule assistant is launched.</span></span> <span data-ttu-id="c473c-123">אם אתה משתמש במצב היברידי, ברשת חברי הצוות אתה יכול לבחור כל חבר צוות עם דרישת משאבים שלא מומשה, ואז בחר **הזמן**.</span><span class="sxs-lookup"><span data-stu-id="c473c-123">If you're using the hybrid mode, in the team member grid you can select any team member with an unfulfilled resource requirement, and then select **Book**.</span></span> <span data-ttu-id="c473c-124">אם אתה משתמש במצב המרכזי, מנהל המשאבים ימצא ויבחר את המשאב.</span><span class="sxs-lookup"><span data-stu-id="c473c-124">If you're using the central mode, the Resource manager finds and selects the resource.</span></span>

## <a name="schedule-assistant-filters"></a><span data-ttu-id="c473c-125">מסננים במסייע לוח הזמנים</span><span class="sxs-lookup"><span data-stu-id="c473c-125">Schedule assistant filters</span></span>

<span data-ttu-id="c473c-126">לאחר הפעלת מסייע לוחות הזמנים, הפרטים מדרישת המשאבים יוצגו כערכים מסוננים בחלונית השמאלית.</span><span class="sxs-lookup"><span data-stu-id="c473c-126">After the Schedule assistant runs, the details from the resource requirement are displayed as filtered values in the left pane.</span></span> <span data-ttu-id="c473c-127">מנהל המשאבים או מנהל הפרויקט יכולים לכוונן תוצאות על-ידי התאמת פילטרים כדי לענות על צורכי התזמון.</span><span class="sxs-lookup"><span data-stu-id="c473c-127">The Resource manager or the Project manager can fine-tune results by adjusting filters to meet the scheduling needs.</span></span>

<span data-ttu-id="c473c-128">חלונית הסינון מציגה אפשרויות הקשורות לעבודה, כולל:</span><span class="sxs-lookup"><span data-stu-id="c473c-128">The filter pane shows work-related options, including:</span></span>

-   <span data-ttu-id="c473c-129">תאריכי ההתחלה והסיום של העבודה</span><span class="sxs-lookup"><span data-stu-id="c473c-129">Work start and end</span></span>
-   <span data-ttu-id="c473c-130">מאפיינים</span><span class="sxs-lookup"><span data-stu-id="c473c-130">Characteristics</span></span>
-   <span data-ttu-id="c473c-131">תפקידים</span><span class="sxs-lookup"><span data-stu-id="c473c-131">Roles</span></span>
-   <span data-ttu-id="c473c-132">יחידות ארגוניות</span><span class="sxs-lookup"><span data-stu-id="c473c-132">Organizational units</span></span>
-   <span data-ttu-id="c473c-133">החברה של הקצאת המשאבים</span><span class="sxs-lookup"><span data-stu-id="c473c-133">Resourcing company</span></span>
-   <span data-ttu-id="c473c-134">סוגי משאבים‬</span><span class="sxs-lookup"><span data-stu-id="c473c-134">Resource types</span></span>
-   <span data-ttu-id="c473c-135">משאבים מועדפים</span><span class="sxs-lookup"><span data-stu-id="c473c-135">Preferred resources</span></span>
