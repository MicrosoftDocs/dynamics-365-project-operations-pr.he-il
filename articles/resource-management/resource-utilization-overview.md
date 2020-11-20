---
title: מבט כולל על ניצול משאבים
description: נושא זו מספק מידע על ניצול המשאבים ב-Project Operations.
author: ruhercul
manager: Annbe
ms.date: 11/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 8b85464dbb68523b122116225a604f67e7236f3e
ms.sourcegitcommit: 14aa380759214713d9bf560f5a7f619b7f4bd5b8
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 11/05/2020
ms.locfileid: "4401377"
---
# <a name="resource-utilization-overview"></a><span data-ttu-id="41b4b-103">מבט כולל על ניצול משאבים</span><span class="sxs-lookup"><span data-stu-id="41b4b-103">Resource utilization overview</span></span>

<span data-ttu-id="41b4b-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="41b4b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="41b4b-105">המשאבים יכולים לכלול ניצול יעד לחיוב.</span><span class="sxs-lookup"><span data-stu-id="41b4b-105">Resources can have a target billable utilization.</span></span> <span data-ttu-id="41b4b-106">ניצול יעד זה מוגדר כתכונה בתפקיד ברירת מחדל של משאב או מוגדר ברשומה של המשאב הבודד הניתן להזמנה.</span><span class="sxs-lookup"><span data-stu-id="41b4b-106">This target utilization is defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="41b4b-107">חישובי ניצול מבוססים על השעות בפועל שדיווחו המשאבים באמצעות ערכי זמן שאושרו.</span><span class="sxs-lookup"><span data-stu-id="41b4b-107">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="41b4b-108">הנוסחאות הבאות משמשות לחישוב הניצול:</span><span class="sxs-lookup"><span data-stu-id="41b4b-108">The following formulas are used to calculate utilization:</span></span>

  - <span data-ttu-id="41b4b-109">ניצול לחיוב = שעות בפועל הניתנות לחיוב ÷ קיבולת משאב</span><span class="sxs-lookup"><span data-stu-id="41b4b-109">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
  - <span data-ttu-id="41b4b-110">ניצול שאינו לחיוב = זמן בפועל עם מזהה סוג חיוב = 'אינו לחיוב', 'משלים' או 'לא זמין' ÷ קיבולת משאב</span><span class="sxs-lookup"><span data-stu-id="41b4b-110">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
  - <span data-ttu-id="41b4b-111">פנימי = זמן בפועל ללא חוזה מכירות ÷ קיבולת משאב</span><span class="sxs-lookup"><span data-stu-id="41b4b-111">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
  - <span data-ttu-id="41b4b-112">קיבולת משאב = שעות עבודה של משאב – מחוץ למשרד – ימים שאינם ימי עבודה</span><span class="sxs-lookup"><span data-stu-id="41b4b-112">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="41b4b-113">ניתן למצוא את התצוגה **ניצול משאב** בחלונית **משאבים**.</span><span class="sxs-lookup"><span data-stu-id="41b4b-113">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

<span data-ttu-id="41b4b-114">כל תא ברשת מייצג את אחוז הניצול לחיוב של המשאב בתקופה, כגון יום, שבוע או חודש.</span><span class="sxs-lookup"><span data-stu-id="41b4b-114">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="41b4b-115">הנוסחאות הבאות משמשות לצביעת התאים:</span><span class="sxs-lookup"><span data-stu-id="41b4b-115">The following formulas are used to color the cells:</span></span>

  - <span data-ttu-id="41b4b-116">**ירוק**: ניצול הניתן לחיוב > = ניצול היעד של משאב</span><span class="sxs-lookup"><span data-stu-id="41b4b-116">**Green**: Billable utilization >= Resource target utilization</span></span>
  - <span data-ttu-id="41b4b-117">**צהוב**: יעד ניצול – 20 < = ניצול הניתן לחיוב < יעד ניצול</span><span class="sxs-lookup"><span data-stu-id="41b4b-117">**Yellow**: Target utilization – 20 <= Billable utilization < Target utilization</span></span>
  - <span data-ttu-id="41b4b-118">**אדום**: ניצול הניתן לחיוב < יעד ניצול – 20</span><span class="sxs-lookup"><span data-stu-id="41b4b-118">**Red**: Billable utilization < Target utilization – 20</span></span>

<span data-ttu-id="41b4b-119">מכיוון שהתצוגה **ניצול משאבים** מבוססת על לוח הזמנים, ניתן להשתמש ביכולות הסינון של לוח הזמנים כדי לסנן את התוצאות.</span><span class="sxs-lookup"><span data-stu-id="41b4b-119">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="41b4b-120">הרשת מחייבת הגדרה של ניצול יעד בתפקיד או במשאב הבודד.</span><span class="sxs-lookup"><span data-stu-id="41b4b-120">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="41b4b-121">לצורך ביצוע הגדרה זו, עבור אל **משאבים** > **תפקידי משאבים**.</span><span class="sxs-lookup"><span data-stu-id="41b4b-121">To do this setup, go to **Resources** > **Resource roles**.</span></span>

<span data-ttu-id="41b4b-122">בנוסף, יש להקצות תפקיד ברירת מחדל לכל משאב הניתן להזמנה.</span><span class="sxs-lookup"><span data-stu-id="41b4b-122">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="41b4b-123">עבור אל **משאבים** > **משאבים**.</span><span class="sxs-lookup"><span data-stu-id="41b4b-123">Go to **Resources** > **Resources**.</span></span> <span data-ttu-id="41b4b-124">בכרטיסיה **Project Service**, וודא שתפקיד משאב מוגדר ושהשדה **מהווה ברירת מחדל** מוגדר ל **כן**.</span><span class="sxs-lookup"><span data-stu-id="41b4b-124">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field is set to **Yes**.</span></span> <span data-ttu-id="41b4b-125">ניתן להוסיף תפקידים נוספים כאשר **מהווה ברירת מחדל** = **לא**.</span><span class="sxs-lookup"><span data-stu-id="41b4b-125">You can add additional roles where **Is Default** = **No**.</span></span> <span data-ttu-id="41b4b-126">התפקיד שבו **מהווה ברירת מחדל** = **כן** משמש להערכת ניצול המשאב כנגד היעד עבור אותו תפקיד.</span><span class="sxs-lookup"><span data-stu-id="41b4b-126">The role where the **Is Default** = **Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

<span data-ttu-id="41b4b-127">בכרטיסיה **Project Service**, ניתן גם להגדיר ניצול יעד בודד עבור המשאב.</span><span class="sxs-lookup"><span data-stu-id="41b4b-127">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="41b4b-128">כעת, חישוב הניצול משתמש בניצול היעד כדי להעריך את היעד של המשאב במקום את היעד של תפקיד ברירת המחדל של המשאב.</span><span class="sxs-lookup"><span data-stu-id="41b4b-128">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="41b4b-129">הניצול מוצג עבור משאב רק אם למשאב יש זמן מאושר הניתן לחיוב במהלך התקופה המופיעה ברשת.</span><span class="sxs-lookup"><span data-stu-id="41b4b-129">Utilization is only shown for a resource if that resource has approved, chargeable time during the period shown in the grid.</span></span>
