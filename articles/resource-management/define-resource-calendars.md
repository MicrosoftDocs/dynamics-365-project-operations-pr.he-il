---
title: הגדרת לוחות שנה של משאבים
description: נושא זה מספק מידע על אופן הגדרת לוח השנה של שעות העבודה עבור משאבים Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: a7b7c45ad2116519b0369bfd3d7cf6743704f4e1
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279814"
---
# <a name="define-resource-calendars"></a><span data-ttu-id="365c6-103">הגדרת לוחות שנה של משאבים</span><span class="sxs-lookup"><span data-stu-id="365c6-103">Define resource calendars</span></span>

<span data-ttu-id="365c6-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="365c6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="365c6-105">לכל משאב הניתן להזמנה שעובד על פרויקט חייב להיות לוח שנה של שעות עבודה כדי להגדיר את זמינותו.</span><span class="sxs-lookup"><span data-stu-id="365c6-105">Each bookable resource working on a project must have a calendar of working hours to define their availability.</span></span> <span data-ttu-id="365c6-106">ניתן להגדיר שעות עבודה של משאב בשתי דרכים:</span><span class="sxs-lookup"><span data-stu-id="365c6-106">Workings hours for a resource can be defined in two ways:</span></span> 

   - <span data-ttu-id="365c6-107">הגדרת כללי לוח שנה אינדבידואליים עבור משאב</span><span class="sxs-lookup"><span data-stu-id="365c6-107">Define individual calendar rules for a resource</span></span>
   - <span data-ttu-id="365c6-108">החלת תבנית לוח שנה קיימת עבור המשאב</span><span class="sxs-lookup"><span data-stu-id="365c6-108">Apply an existing calendar template for the resource</span></span>

## <a name="define-a-resources-working-hours"></a><span data-ttu-id="365c6-109">הגדרת שעות עבודה של משאב</span><span class="sxs-lookup"><span data-stu-id="365c6-109">Define a resource's working hours</span></span>

1. <span data-ttu-id="365c6-110">בתפריט **משאבים**, בחר **משאבים**.</span><span class="sxs-lookup"><span data-stu-id="365c6-110">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="365c6-111">מתצוגת הרשת בחר ב **משאב הניתן להזמנה** הרלוונטי.</span><span class="sxs-lookup"><span data-stu-id="365c6-111">From the grid view, select the applicable **Bookable Resource**.</span></span>
3. <span data-ttu-id="365c6-112">בדף **פרטי משאבים** בחר את הכרטיסיה **שעות עבודה**. כברירת מחדל, לוח השנה של המשאבים הניתנים להזמנה מוגדר לפי שעות העבודה של תבנית ברירת המחדל של שעות העבודה, המוגדרת עבור הארגון.</span><span class="sxs-lookup"><span data-stu-id="365c6-112">On the **Resource Details** page, select the **Working Hours** tab. By default, the bookable resources calendar defaults to the working hours of the default work hour template that is defined for the organization.</span></span>
4. <span data-ttu-id="365c6-113">לעדכון שעות העבודה, לחץ באמצעות לחצן העכבר הימני על תאריך ההתחלה של כלל לוח השנה אותו יש להגדיר.</span><span class="sxs-lookup"><span data-stu-id="365c6-113">To update the working hours, right-click on the start date of the proposed calendar rule to be defined.</span></span> <span data-ttu-id="365c6-114">השתמש בתפריט כללי לוח השנה כדי להגדיר כלל לוח שנה ליום מסוים, לשאר הסידרה או לכל לוח השנה.</span><span class="sxs-lookup"><span data-stu-id="365c6-114">Use the calendar rule menu to define a calendar rule for a specific day, the remainder of the series, or the entire calendar.</span></span>
5. <span data-ttu-id="365c6-115">לאחר שנבחרה האפשרות, ניתן להגדיר את:</span><span class="sxs-lookup"><span data-stu-id="365c6-115">After the option is selected, you can then define:</span></span>

    - <span data-ttu-id="365c6-116">היום בשבוע בו יחולו שעות העבודה.</span><span class="sxs-lookup"><span data-stu-id="365c6-116">The day of the week where the working hours will apply.</span></span>
    - <span data-ttu-id="365c6-117">שעות העבודה במהלך כל אחד מהימים.</span><span class="sxs-lookup"><span data-stu-id="365c6-117">The working times within each day.</span></span>
    - <span data-ttu-id="365c6-118">אזור זמן עבור כלל לוח השנה.</span><span class="sxs-lookup"><span data-stu-id="365c6-118">The time zone for the calendar rule.</span></span>
    - <span data-ttu-id="365c6-119">אם רלוונטי, ניתן גם לציין זמן שאינו זמן עבודה עבור הכלל.</span><span class="sxs-lookup"><span data-stu-id="365c6-119">If applicable, non-working time can also be specified for the rule.</span></span>

## <a name="applying-a-calendar-template-to-a-resource"></a><span data-ttu-id="365c6-120">החלת תבנית לוח שנה על משאב</span><span class="sxs-lookup"><span data-stu-id="365c6-120">Applying a calendar template to a resource</span></span>

1. <span data-ttu-id="365c6-121">בתפריט **משאבים**, בחר **משאבים**.</span><span class="sxs-lookup"><span data-stu-id="365c6-121">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="365c6-122">מתצוגת הרשת, בחר עד 25 **משאבים הניתנים להזמנה** לעדכון.</span><span class="sxs-lookup"><span data-stu-id="365c6-122">From the grid view, select up to 25 **Bookable Resources** to update.</span></span>
3. <span data-ttu-id="365c6-123">בחר **הגדר לוח שנה** ותיבת דו-שיח יבקש ממך רשימה של תבניות זמינות של שעות עבודה.</span><span class="sxs-lookup"><span data-stu-id="365c6-123">Select **Set Calendar** and a dialog will prompt you with a list of available work hour templates.</span></span>
4. <span data-ttu-id="365c6-124">בחר בתבנית הרצויה ולאחר מכן בחר **החל**.</span><span class="sxs-lookup"><span data-stu-id="365c6-124">Select the template you want to use, and then select **Apply**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]