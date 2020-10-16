---
title: הגדרת לוחות שנה של משאבים
description: נושא זה מספק מידע על אופן הגדרת לוח השנה של שעות העבודה עבור משאבים Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: ab39d7e5dc2d8c01ed49ca0f1a4d1691aaf15637
ms.sourcegitcommit: 396e0fea2f1598a5313cb0128eca4fe0bb5aade9
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961872"
---
# <a name="define-resource-calendars"></a><span data-ttu-id="690d3-103">הגדרת לוחות שנה של משאבים</span><span class="sxs-lookup"><span data-stu-id="690d3-103">Define resource calendars</span></span>

<span data-ttu-id="690d3-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="690d3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="690d3-105">לכל משאב הניתן להזמנה שעובד על פרויקט חייב להיות לוח שנה של שעות עבודה כדי להגדיר את זמינותו.</span><span class="sxs-lookup"><span data-stu-id="690d3-105">Each bookable resource working on a project must have a calendar of working hours to define their availability.</span></span> <span data-ttu-id="690d3-106">ניתן להגדיר שעות עבודה של משאב בשתי דרכים:</span><span class="sxs-lookup"><span data-stu-id="690d3-106">Workings hours for a resource can be defined in two ways:</span></span> 

   - <span data-ttu-id="690d3-107">הגדרת כללי לוח שנה אינדבידואליים עבור משאב</span><span class="sxs-lookup"><span data-stu-id="690d3-107">Define individual calendar rules for a resource</span></span>
   - <span data-ttu-id="690d3-108">החלת תבנית לוח שנה קיימת עבור המשאב</span><span class="sxs-lookup"><span data-stu-id="690d3-108">Apply an existing calendar template for the resource</span></span>

## <a name="define-a-resources-working-hours"></a><span data-ttu-id="690d3-109">הגדרת שעות עבודה של משאב</span><span class="sxs-lookup"><span data-stu-id="690d3-109">Define a resource's working hours</span></span>

1. <span data-ttu-id="690d3-110">בתפריט **משאבים**, בחר **משאבים**.</span><span class="sxs-lookup"><span data-stu-id="690d3-110">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="690d3-111">מתצוגת הרשת בחר ב**משאב הניתן להזמנה** הרלוונטי.</span><span class="sxs-lookup"><span data-stu-id="690d3-111">From the grid view, select the applicable **Bookable Resource**.</span></span>
3. <span data-ttu-id="690d3-112">בדף **פרטי משאבים** בחר את הכרטיסיה **שעות עבודה**. כברירת מחדל, לוח השנה של המשאבים הניתנים להזמנה מוגדר לפי שעות העבודה של תבנית ברירת המחדל של שעות העבודה, המוגדרת עבור הארגון.</span><span class="sxs-lookup"><span data-stu-id="690d3-112">On the **Resource Details** page, select the **Working Hours** tab. By default, the bookable resources calendar defaults to the working hours of the default work hour template that is defined for the organization.</span></span>
4. <span data-ttu-id="690d3-113">לעדכון שעות העבודה, לחץ באמצעות לחצן העכבר הימני על תאריך ההתחלה של כלל לוח השנה אותו יש להגדיר.</span><span class="sxs-lookup"><span data-stu-id="690d3-113">To update the working hours, right-click on the start date of the proposed calendar rule to be defined.</span></span> <span data-ttu-id="690d3-114">השתמש בתפריט כללי לוח השנה כדי להגדיר כלל לוח שנה ליום מסוים, לשאר הסידרה או לכל לוח השנה.</span><span class="sxs-lookup"><span data-stu-id="690d3-114">Use the calendar rule menu to define a calendar rule for a specific day, the remainder of the series, or the entire calendar.</span></span>
5. <span data-ttu-id="690d3-115">לאחר שנבחרה האפשרות, ניתן להגדיר את:</span><span class="sxs-lookup"><span data-stu-id="690d3-115">After the option is selected, you can then define:</span></span>

    - <span data-ttu-id="690d3-116">היום בשבוע בו יחולו שעות העבודה.</span><span class="sxs-lookup"><span data-stu-id="690d3-116">The day of the week where the working hours will apply.</span></span>
    - <span data-ttu-id="690d3-117">שעות העבודה במהלך כל אחד מהימים.</span><span class="sxs-lookup"><span data-stu-id="690d3-117">The working times within each day.</span></span>
    - <span data-ttu-id="690d3-118">אזור זמן עבור כלל לוח השנה.</span><span class="sxs-lookup"><span data-stu-id="690d3-118">The time zone for the calendar rule.</span></span>
    - <span data-ttu-id="690d3-119">אם רלוונטי, ניתן גם לציין זמן שאינו זמן עבודה עבור הכלל.</span><span class="sxs-lookup"><span data-stu-id="690d3-119">If applicable, non-working time can also be specified for the rule.</span></span>

## <a name="applying-a-calendar-template-to-a-resource"></a><span data-ttu-id="690d3-120">החלת תבנית לוח שנה על משאב</span><span class="sxs-lookup"><span data-stu-id="690d3-120">Applying a calendar template to a resource</span></span>

1. <span data-ttu-id="690d3-121">בתפריט **משאבים**, בחר **משאבים**.</span><span class="sxs-lookup"><span data-stu-id="690d3-121">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="690d3-122">מתצוגת הרשת, בחר עד 25 **משאבים הניתנים להזמנה** לעדכון.</span><span class="sxs-lookup"><span data-stu-id="690d3-122">From the grid view, select up to 25 **Bookable Resources** to update.</span></span>
3. <span data-ttu-id="690d3-123">בחר **הגדר לוח שנה** ותיבת דו-שיח יבקש ממך רשימה של תבניות זמינות של שעות עבודה.</span><span class="sxs-lookup"><span data-stu-id="690d3-123">Select **Set Calendar** and a dialog will prompt you with a list of available work hour templates.</span></span>
4. <span data-ttu-id="690d3-124">בחר בתבנית הרצויה ולאחר מכן בחר **החל**.</span><span class="sxs-lookup"><span data-stu-id="690d3-124">Select the template you want to use, and then select **Apply**.</span></span>