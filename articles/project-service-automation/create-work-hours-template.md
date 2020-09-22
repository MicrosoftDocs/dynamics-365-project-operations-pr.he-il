---
title: יצירת תבנית שעות עבודה
description: כיצד ליצור תבנית שעות עבודה ב- Project Service
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 1a519487-25f1-4e9d-b739-1c1becf1d649
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5e7ef4af5f22419cccd8f29ea2a0a0a21a75875a
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751833"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="40dec-103">יצירת תבנית שעות עבודה (Project Service)</span><span class="sxs-lookup"><span data-stu-id="40dec-103">Create a work hours template (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="40dec-104">לפני שתוכל ליצור לוחות זמנים של הפרוייקט, עליך להגדיר את לוח הזמנים של הפרוייקט המגדיר את מספר שעות העבודה כדי להתאים לכל יום בלוח הזמנים ולכל מועדי סגירת העסק.</span><span class="sxs-lookup"><span data-stu-id="40dec-104">Before you can create project schedules, you need to set up a project calendar that defines the number of working hours to accommodate per day in the schedule and any business closures.</span></span> <span data-ttu-id="40dec-105">ניתן לעשות זאת עם תבנית שעות עבודה, אשר מכילה פרטים על שעות העבודה בכל יום, ימי חופש וכל מועדי הסגירה האחרים של העסק.</span><span class="sxs-lookup"><span data-stu-id="40dec-105">You do this with a work hours template, which contains details about work hours per day, days off, and any other business closures.</span></span>  
  
 <span data-ttu-id="40dec-106">כשאתה יוצר פרוייקט, אתה משייך תבנית עבודה ללוח השנה של הפרוייקט כדי להחיל את לוח הזמנים של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="40dec-106">When you’re creating a project, you associate a work template to the project calendar to apply the schedule for the project.</span></span>  
  
 <span data-ttu-id="40dec-107">קיימות שתי דרכים שבהן באפשרותך ליצור תבנית שעות עבודה:</span><span class="sxs-lookup"><span data-stu-id="40dec-107">There are two ways you can create a work hours template:</span></span>  
  
-   <span data-ttu-id="40dec-108">צור תבנית שעות עבודה בהתבסס על לוח השנה של המשאב.</span><span class="sxs-lookup"><span data-stu-id="40dec-108">Create a work hours template based on a resource’s calendar.</span></span>  
  
-   <span data-ttu-id="40dec-109">צור תבנית שעות עבודה חדשה.</span><span class="sxs-lookup"><span data-stu-id="40dec-109">Create a new work hours template.</span></span>  
  
#### <a name="to-create-a-work-hours-template-based-on-a-resources-calendar"></a><span data-ttu-id="40dec-110">כדי ליצור תבנית שעות עבודה בהתבסס על לוח השנה של המשאב</span><span class="sxs-lookup"><span data-stu-id="40dec-110">To create a work hours template based on a resource’s calendar</span></span>  
  
1.  <span data-ttu-id="40dec-111">עבור אל **Project Service > משאבים**.</span><span class="sxs-lookup"><span data-stu-id="40dec-111">Go to **Project Service > Resources**.</span></span>  
  
2.  <span data-ttu-id="40dec-112">בחר את המשאב שעליו ברצונך לבסס את שעות העבודה שלך.</span><span class="sxs-lookup"><span data-stu-id="40dec-112">Select the resource you want to base your work hours on.</span></span>  
  
3.  <span data-ttu-id="40dec-113">לחץ על **שמירת לוח שנה בשם**, הזן שם עבור תבנית שעות העבודה ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="40dec-113">Click **Save Calendar As**, enter a name for the work hours template, and then click **Save**.</span></span>  
  
4.  <span data-ttu-id="40dec-114">לאחר שתסיים לערוך את האפשרויות, לחץ על **שמור וסגור**.</span><span class="sxs-lookup"><span data-stu-id="40dec-114">When you’re done changing options, click **Save and Close**.</span></span>  
  
5.  <span data-ttu-id="40dec-115">לחץ על הלחצן **שמור** בפינה הימנית התחתונה של המסך.</span><span class="sxs-lookup"><span data-stu-id="40dec-115">Click the **Save** button at the bottom right corner of the screen.</span></span>  
  
#### <a name="to-create-a-new-work-hours-template"></a><span data-ttu-id="40dec-116">כדי ליצור תבנית שעות עבודה חדשה</span><span class="sxs-lookup"><span data-stu-id="40dec-116">To create a new work hours template</span></span>  
  
1.  <span data-ttu-id="40dec-117">עבור אל **Project Service > תבניות שעות עבודה**.</span><span class="sxs-lookup"><span data-stu-id="40dec-117">Go to **Project Service > Work Hours Templates**.</span></span>  
  
2.  <span data-ttu-id="40dec-118">לחץ על **חדש**.</span><span class="sxs-lookup"><span data-stu-id="40dec-118">Click **New**.</span></span>  
  
3.  <span data-ttu-id="40dec-119">הזן שם עבור תבנית שעות העבודה.</span><span class="sxs-lookup"><span data-stu-id="40dec-119">Enter a name for the work hours template.</span></span>  
  
4.  <span data-ttu-id="40dec-120">בחר משאב שעליו יתבססו שעות העבודה ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="40dec-120">Select a resource to base the work hours on, and then click **Save**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="40dec-121">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="40dec-121">See Also</span></span>  
 [<span data-ttu-id="40dec-122">הגדרת משאבים</span><span class="sxs-lookup"><span data-stu-id="40dec-122">Set up resources</span></span>](../project-service/set-up-resources.md)
