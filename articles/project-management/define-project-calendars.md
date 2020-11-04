---
title: הגדרת לוחות שנה של פרויקטים
description: נושא זה מספק מידע על השימוש בלוח השנה של הפרויקט למעקב אחר לוח הזמנים של הפרויקט.
author: ruhercul
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 774399f2c02d8434c9c042c3a9f995792893bfce
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077482"
---
# <a name="define-project-calendars"></a><span data-ttu-id="b72c5-103">הגדרת לוחות שנה של פרויקטים</span><span class="sxs-lookup"><span data-stu-id="b72c5-103">Define project calendars</span></span>

<span data-ttu-id="b72c5-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="b72c5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b72c5-105">כדי ליצור לוח זמנים לפרויקט, עליך ליצור תבנית של לוח השנה של הפרויקט המגדירה את מספר שעות העבודה לכל יום ולכל מועדי סגירת העסק.</span><span class="sxs-lookup"><span data-stu-id="b72c5-105">To create a project schedule, you create a project calendar template that defines the number of working hours per day and any business closures.</span></span> <span data-ttu-id="b72c5-106">כדי ליצור תבנית לוח שנה של פרויקט, עליך לשייך תבנית עבודה עם השדה **תבנית לוח שנה** עבור הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="b72c5-106">To create a project calendar template, you associate a work template with the **Calendar template** field for the project.</span></span> <span data-ttu-id="b72c5-107">בצע את השלבים הבאים כדי ליצור תבנית עבודה.</span><span class="sxs-lookup"><span data-stu-id="b72c5-107">Follow these steps to create a work template.</span></span>

1. <span data-ttu-id="b72c5-108">בחלונית הניווט השמאלית, בחר **משאבים**.</span><span class="sxs-lookup"><span data-stu-id="b72c5-108">In the left navigation pane, select **Resources**.</span></span> 
2. <span data-ttu-id="b72c5-109">בדף הרשימה של **משאבים** , פתח רשומת משתמש ולאחר מכן בחר **הצג שעות עבודה**.</span><span class="sxs-lookup"><span data-stu-id="b72c5-109">On the **Resources** list page, open a user record, and then select **Show Work Hours**.</span></span>

  > [!NOTE]
  > <span data-ttu-id="b72c5-110">ודא שניתן להציג חלונות קופצים בדף הדפדפן.</span><span class="sxs-lookup"><span data-stu-id="b72c5-110">Make sure that you allow pop-ups on the browser page.</span></span> <span data-ttu-id="b72c5-111">פעולה זו מאפשרת לך לראות את שעות העבודה שנקבעו עבור המשאב.</span><span class="sxs-lookup"><span data-stu-id="b72c5-111">This lets you see the work hours set for the resource.</span></span>
  
3. <span data-ttu-id="b72c5-112">בכרטיסיה **תצוגה חודשית** , בחר **הגדר**.</span><span class="sxs-lookup"><span data-stu-id="b72c5-112">On the **Monthly View** tab, select **Set Up**.</span></span> <span data-ttu-id="b72c5-113">רשימה עם שלוש אפשרויות מופיעה:</span><span class="sxs-lookup"><span data-stu-id="b72c5-113">A list of three options appears:</span></span> 

  - <span data-ttu-id="b72c5-114">לוח זמנים שבועי חדש</span><span class="sxs-lookup"><span data-stu-id="b72c5-114">New Weekly Schedule</span></span>
  - <span data-ttu-id="b72c5-115">לוח זמני עבודה עבור יום אחד</span><span class="sxs-lookup"><span data-stu-id="b72c5-115">Work Schedule for One Day</span></span>
  - <span data-ttu-id="b72c5-116">שעות מנוחה</span><span class="sxs-lookup"><span data-stu-id="b72c5-116">Time Off</span></span>

4. <span data-ttu-id="b72c5-117">בחר **לוח זמנים שבועי חדש** ולאחר מכן קבע את האפשרויות עבור לוח הזמנים של המשאב הזה.</span><span class="sxs-lookup"><span data-stu-id="b72c5-117">Select **New Weekly Schedule** , and then set the options for this resource schedule.</span></span> <span data-ttu-id="b72c5-118">באפשרותך לקבוע לוח זמנים שבועי חוזר, פרמטרים של שעה יומית, סגירת עסק ועוד.</span><span class="sxs-lookup"><span data-stu-id="b72c5-118">You can set a recurring weekly schedule, daily hour parameters, business closures, and more.</span></span>
5. <span data-ttu-id="b72c5-119">הגדר את טווח התאריכים, בחר **שמור** ולאחר מכן בחר **סגור**.</span><span class="sxs-lookup"><span data-stu-id="b72c5-119">Set the date range, select **Save** , and then select **Close**.</span></span> 
6. <span data-ttu-id="b72c5-120">חזור אל דף הרשימה של **משאבים** ובחר את המשאב שעבורו תרצה להגדיר שעות עבודה.</span><span class="sxs-lookup"><span data-stu-id="b72c5-120">Go back to the **Resources** list page, and select the resource that you set the work hours for.</span></span> 
7. <span data-ttu-id="b72c5-121">בחר **הגדר לוח שנה כ:** כדי להגדיר את תבנית העבודה.</span><span class="sxs-lookup"><span data-stu-id="b72c5-121">Select **Set Calendar As** to set the work template.</span></span> 
8. <span data-ttu-id="b72c5-122">בתיבת הדו-שיח **תבנית עבודה** , הזן שם עבור תבנית העבודה ולאחר מכן בחר **החל**.</span><span class="sxs-lookup"><span data-stu-id="b72c5-122">In the **Work Template** dialog box, enter a name for the work template, and then select **Apply**.</span></span> 

<span data-ttu-id="b72c5-123">כעת תוכל לשייך את תבנית העבודה לתבנית לוח שנה של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="b72c5-123">You can now associate the work template with a project calendar template.</span></span>
