---
title: יצירת תבנית שעות עבודה
description: כיצד ליצור תבנית שעות עבודה ב- Project Service
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 54d7385a2bb161c7dd02d882090790debaef3bdb
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148779"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="1d50c-103">יצירת תבנית שעות עבודה (Project Service)</span><span class="sxs-lookup"><span data-stu-id="1d50c-103">Create a work hours template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="1d50c-104">לפני שתוכל ליצור לוחות זמנים של הפרוייקט, עליך להגדיר את לוח הזמנים של הפרוייקט המגדיר את מספר שעות העבודה כדי להתאים לכל יום בלוח הזמנים ולכל מועדי סגירת העסק.</span><span class="sxs-lookup"><span data-stu-id="1d50c-104">Before you can create project schedules, you need to set up a project calendar that defines the number of working hours to accommodate per day in the schedule and any business closures.</span></span> <span data-ttu-id="1d50c-105">ניתן לעשות זאת עם תבנית שעות עבודה, אשר מכילה פרטים על שעות העבודה בכל יום, ימי חופש וכל מועדי הסגירה האחרים של העסק.</span><span class="sxs-lookup"><span data-stu-id="1d50c-105">You do this with a work hours template, which contains details about work hours per day, days off, and any other business closures.</span></span>  
  
 <span data-ttu-id="1d50c-106">כשאתה יוצר פרוייקט, אתה משייך תבנית עבודה ללוח השנה של הפרוייקט כדי להחיל את לוח הזמנים של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="1d50c-106">When you’re creating a project, you associate a work template to the project calendar to apply the schedule for the project.</span></span>  
  
 <span data-ttu-id="1d50c-107">קיימות שתי דרכים שבהן באפשרותך ליצור תבנית שעות עבודה:</span><span class="sxs-lookup"><span data-stu-id="1d50c-107">There are two ways you can create a work hours template:</span></span>  
  
-   <span data-ttu-id="1d50c-108">צור תבנית שעות עבודה בהתבסס על לוח השנה של המשאב.</span><span class="sxs-lookup"><span data-stu-id="1d50c-108">Create a work hours template based on a resource’s calendar.</span></span>  
  
-   <span data-ttu-id="1d50c-109">צור תבנית שעות עבודה חדשה.</span><span class="sxs-lookup"><span data-stu-id="1d50c-109">Create a new work hours template.</span></span>  
  
#### <a name="to-create-a-work-hours-template-based-on-a-resources-calendar"></a><span data-ttu-id="1d50c-110">כדי ליצור תבנית שעות עבודה בהתבסס על לוח השנה של המשאב</span><span class="sxs-lookup"><span data-stu-id="1d50c-110">To create a work hours template based on a resource’s calendar</span></span>  
  
1.  <span data-ttu-id="1d50c-111">עבור אל **Project Service > משאבים**.</span><span class="sxs-lookup"><span data-stu-id="1d50c-111">Go to **Project Service > Resources**.</span></span>  
  
2.  <span data-ttu-id="1d50c-112">בחר את המשאב שעליו ברצונך לבסס את שעות העבודה שלך.</span><span class="sxs-lookup"><span data-stu-id="1d50c-112">Select the resource you want to base your work hours on.</span></span>  
  
3.  <span data-ttu-id="1d50c-113">לחץ על **שמירת לוח שנה בשם**, הזן שם עבור תבנית שעות העבודה ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="1d50c-113">Click **Save Calendar As**, enter a name for the work hours template, and then click **Save**.</span></span>  
  
4.  <span data-ttu-id="1d50c-114">לאחר שתסיים לערוך את האפשרויות, לחץ על **שמור וסגור**.</span><span class="sxs-lookup"><span data-stu-id="1d50c-114">When you’re done changing options, click **Save and Close**.</span></span>  
  
5.  <span data-ttu-id="1d50c-115">לחץ על הלחצן **שמור** בפינה הימנית התחתונה של המסך.</span><span class="sxs-lookup"><span data-stu-id="1d50c-115">Click the **Save** button at the bottom right corner of the screen.</span></span>  
  
#### <a name="to-create-a-new-work-hours-template"></a><span data-ttu-id="1d50c-116">כדי ליצור תבנית שעות עבודה חדשה</span><span class="sxs-lookup"><span data-stu-id="1d50c-116">To create a new work hours template</span></span>  
  
1.  <span data-ttu-id="1d50c-117">עבור אל **Project Service > תבניות שעות עבודה**.</span><span class="sxs-lookup"><span data-stu-id="1d50c-117">Go to **Project Service > Work Hours Templates**.</span></span>  
  
2.  <span data-ttu-id="1d50c-118">לחץ על **חדש**.</span><span class="sxs-lookup"><span data-stu-id="1d50c-118">Click **New**.</span></span>  
  
3.  <span data-ttu-id="1d50c-119">הזן שם עבור תבנית שעות העבודה.</span><span class="sxs-lookup"><span data-stu-id="1d50c-119">Enter a name for the work hours template.</span></span>  
  
4.  <span data-ttu-id="1d50c-120">בחר משאב שעליו יתבססו שעות העבודה ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="1d50c-120">Select a resource to base the work hours on, and then click **Save**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="1d50c-121">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="1d50c-121">See Also</span></span>  
 [<span data-ttu-id="1d50c-122">הגדרת משאבים</span><span class="sxs-lookup"><span data-stu-id="1d50c-122">Set up resources</span></span>](../psa/set-up-resources.md)
