---
title: קביעת תצורה של הגדרות פרמטרים נוספים
description: כיצד לקבוע תצורה של הגדרות פרמטרים נוספים ב- Project Service
author: JohnPBurrows
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
ms.openlocfilehash: 73264845808e12950a48eea2b79e54c393d9c024
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5151569"
---
# <a name="configure-additional-parameter-settings-project-service"></a><span data-ttu-id="53904-103">קביעת תצורה של הגדרות פרמטרים נוספים (Project Service)</span><span class="sxs-lookup"><span data-stu-id="53904-103">Configure additional parameter settings (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="53904-104">לאחר שקבעת את הפריטים בנושאים הקודמים, עליך להגדיר פרמטרים נוספים של הפרוייקט לשימוש עבור הפרוייקטים שלך.</span><span class="sxs-lookup"><span data-stu-id="53904-104">Once you’ve configured the items in previous topics, you need to set additional project parameters to use for your projects.</span></span> <span data-ttu-id="53904-105">כאשר התקנת לראשונה את [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], יצרת הגדרת פרמטרים כדי ליצור תחילה את כל הרשומות הדרושות עבור [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="53904-105">When you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you created a parameters setting to first create all the records required for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to work.</span></span> <span data-ttu-id="53904-106">כעת הגיע הזמן לחזור ולהגדיר שדות נוספים עבור הגדרת אלה.</span><span class="sxs-lookup"><span data-stu-id="53904-106">Now it’s time to go back and configure additional fields for these settings.</span></span>  
  
 <span data-ttu-id="53904-107">עליך לקבוע את ההגדרות הבאות:</span><span class="sxs-lookup"><span data-stu-id="53904-107">You’ll need to have configured the following settings:</span></span>  
  
-   <span data-ttu-id="53904-108">יחידה ארגונית</span><span class="sxs-lookup"><span data-stu-id="53904-108">Organizational unit</span></span>  
  
-   <span data-ttu-id="53904-109">תדירות הגשת חשבונית</span><span class="sxs-lookup"><span data-stu-id="53904-109">Invoice frequency</span></span>  
  
-   <span data-ttu-id="53904-110">תבנית שעות עבודה</span><span class="sxs-lookup"><span data-stu-id="53904-110">Work hours template</span></span>  
  
-   <span data-ttu-id="53904-111">מחירון</span><span class="sxs-lookup"><span data-stu-id="53904-111">Price list</span></span>  
 
<span data-ttu-id="53904-112">בשלב זה, גם תציין איזה סוג של הקצאת משאבים רצוי לך:</span><span class="sxs-lookup"><span data-stu-id="53904-112">In this step, you’ll also indicate what type of resource allocation you want:</span></span>  
  
- <span data-ttu-id="53904-113">**מרכזי**.</span><span class="sxs-lookup"><span data-stu-id="53904-113">**Central**.</span></span> <span data-ttu-id="53904-114">רק מנהלי משאבים יוכלו להקצות משאבים לפרוייקטים.</span><span class="sxs-lookup"><span data-stu-id="53904-114">Only resource managers can allocate resources to projects.</span></span>  
  
- <span data-ttu-id="53904-115">**היברידי**.</span><span class="sxs-lookup"><span data-stu-id="53904-115">**Hybrid**.</span></span> <span data-ttu-id="53904-116">מנהלי משאבים, מנהלי פרוייקטים ומנהלי תיקי לקוחות יוכלו להקצות משאבים לפרוייקטים.</span><span class="sxs-lookup"><span data-stu-id="53904-116">Resource managers, project managers, and account managers can allocate resources to projects.</span></span>  
  
 
<span data-ttu-id="53904-117">כדי לקבוע פרמטרים לפרוייקט:</span><span class="sxs-lookup"><span data-stu-id="53904-117">To set project parameters:</span></span>  
  
1. <span data-ttu-id="53904-118">עבור אל **Project Service > פרמטרים**.</span><span class="sxs-lookup"><span data-stu-id="53904-118">Go to **Project Service > Parameters**.</span></span>  
  
2. <span data-ttu-id="53904-119">לחץ על הגדרת הפרמטרים שברצונך לקבוע (זו שיצרת כאשר התקנת לראשונה את [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]), או לחץ על **חדש** כדי ליצור הגדרה חדשה.</span><span class="sxs-lookup"><span data-stu-id="53904-119">Click the parameters setting you want to configure (the one you created when you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]), or click **New** to create a new one.</span></span>  
  
3. <span data-ttu-id="53904-120">באזור **כללי**, הגדר את האפשרויות עבור הפרמטרים של הפרוייקט שלך.</span><span class="sxs-lookup"><span data-stu-id="53904-120">In the **General** area, set all the options for your project parameters.</span></span>  
  
4. <span data-ttu-id="53904-121">באזור **מחירון**, לחץ על **+** כדי להוסיף מחירון, בחר מחירון ברשימה הנפתחת **מחירון של פרמטר בפרוייקט**, ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="53904-121">In the **Price List** area, click **+** to add a price list, select a price list in the **Project Parameter Price List** drop-down list, and then click **Save**.</span></span>  
  
5. <span data-ttu-id="53904-122">לחץ על הלחצן **שמור** בפינה השמאלית התחתונה של המסך.</span><span class="sxs-lookup"><span data-stu-id="53904-122">Click the **Save** button in the bottom right corner of the screen.</span></span>  

> [!NOTE]
> <span data-ttu-id="53904-123">יש לשמור על רשומת הפרמטרים של הפרויקט כדי ש- Project Service יתפקד בצורה תקינה.</span><span class="sxs-lookup"><span data-stu-id="53904-123">The project parameter record must be maintained for Project Service to function correcly.</span></span> <span data-ttu-id="53904-124">אין למחוק רשומה זו.</span><span class="sxs-lookup"><span data-stu-id="53904-124">This record should not be deleted.</span></span>

### <a name="see-also"></a><span data-ttu-id="53904-125">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="53904-125">See Also</span></span>  
 [<span data-ttu-id="53904-126">הגדרת משאבים</span><span class="sxs-lookup"><span data-stu-id="53904-126">Set up resources</span></span>](../psa/set-up-resources.md)
