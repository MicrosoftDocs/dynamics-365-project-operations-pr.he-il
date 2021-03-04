---
title: יצירת פרוייקט
description: כיצד ליצור פרוייקט ב- Project Service
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/13/2020
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
ms.openlocfilehash: 93958f8e7654ebc4cb038ba7ca0c5e4e02f39937
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148869"
---
# <a name="create-a-project-project-service"></a><span data-ttu-id="38cbc-103">יצירת פרוייקט (Project Service)</span><span class="sxs-lookup"><span data-stu-id="38cbc-103">Create a project (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="38cbc-104">צור פרוייקט באמצעות היכולות של [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ב- [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] כשתרצה ליצור הזדמנות, הצעת מחיר או חוזה עבור שירותים מבוססי-פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="38cbc-104">Create a project using the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] when you want to create an opportunity, quote, or contract for project-based services.</span></span> <span data-ttu-id="38cbc-105">היכולות של [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] מסייעות לך לנהל את הפרוייקט מהזדמנות עד להשלמה.</span><span class="sxs-lookup"><span data-stu-id="38cbc-105">The [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities help you manage your project from opportunity through completion.</span></span> <span data-ttu-id="38cbc-106">בעת יצירת פרוייקט, תיצור גם מבנה התפלגות עבודה שמשפיע על הצעות מחיר, הערכות עלות וניהול משאבים שלך.</span><span class="sxs-lookup"><span data-stu-id="38cbc-106">When you create a project, you’ll also create a work breakdown structure, which affects your quotes, cost estimates, and resource management.</span></span>  
  
1.  <span data-ttu-id="38cbc-107">עבור אל **Project Service > פרוייקטים**.</span><span class="sxs-lookup"><span data-stu-id="38cbc-107">Go to **Project Service > Projects**.</span></span>  
  
2.  <span data-ttu-id="38cbc-108">לחץ על **פרוייקט חדש**.</span><span class="sxs-lookup"><span data-stu-id="38cbc-108">Click **New Project**.</span></span>  
  
3.  <span data-ttu-id="38cbc-109">באזור **סיכום**, הזן שם עבור הפרוייקט שלך, ולאחר מכן מלא כמה שיותר פרטים.</span><span class="sxs-lookup"><span data-stu-id="38cbc-109">In the **Summary** area, enter a name for your project, and then fill in as many of the details as you can.</span></span> <span data-ttu-id="38cbc-110">פריטים המסומנים בכוכבית (\*) אדומה הם חובה.</span><span class="sxs-lookup"><span data-stu-id="38cbc-110">Items marked with a red asterisk (\*) are required.</span></span>  
  
4.  <span data-ttu-id="38cbc-111">לחץ על **שמור** כדי ליצור את הפרוייקט כך שתוכל להמשיך לערוך אותו.</span><span class="sxs-lookup"><span data-stu-id="38cbc-111">Click **Save** to create your project so you can continue editing it.</span></span>  
  
<span data-ttu-id="38cbc-112">בשלב הבא, תיצור מבנה התפלגות עבודה עבור הפרוייקט שלך להגדיר את המשימות, את התזמון ואת תפקידי המשאבים הדרושים עבור הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="38cbc-112">Next, you’ll create a work breakdown structure for your project to define the tasks, timing, and resource roles needed for the project.</span></span>  

> [!NOTE]
> <span data-ttu-id="38cbc-113">בעת קביעת תזמון, Project Service Automation מתחשב באזור הזמן של התבנית **שעת עבודה** שחלה.</span><span class="sxs-lookup"><span data-stu-id="38cbc-113">When scheduling, Project Service Automation respects the time zone of the applied **Work Hour** template.</span></span> <span data-ttu-id="38cbc-114">עם זאת, בעת הצגת משימות התזמון, תאריכי ההתחלה והסיום של המשימה יופיעו באזור הזמן של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="38cbc-114">However, when viewing the schedule tasks, the start and end dates of a task will be displayed in the user's time zone.</span></span> <span data-ttu-id="38cbc-115">זה חל על תצוגות אחרות המופיעות בשלבים בזמן בטופס **פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="38cbc-115">This applies to other time-phased views in the **Project** form.</span></span> <span data-ttu-id="38cbc-116">אם אזור הזמן של המשתמש אינו תואם את אזור הזמן של תבנית שעות העבודה שהוחלה על הפרויקט, תופיע אזהרה המסבירה את ההבדל.</span><span class="sxs-lookup"><span data-stu-id="38cbc-116">If the user's time zone does not match the time zone of the work hour template applied to the project, a warning which explains the difference will occur.</span></span> 
  
### <a name="see-also"></a><span data-ttu-id="38cbc-117">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="38cbc-117">See Also</span></span>  
 [<span data-ttu-id="38cbc-118">מדריך למנהל פרוייקט</span><span class="sxs-lookup"><span data-stu-id="38cbc-118">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
