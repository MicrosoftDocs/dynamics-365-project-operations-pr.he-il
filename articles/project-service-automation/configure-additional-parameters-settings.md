---
title: קביעת תצורה של הגדרות פרמטרים נוספים
description: כיצד לקבוע תצורה של הגדרות פרמטרים נוספים ב- Project Service
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: de2fe830-4313-4711-b03b-76d56bf56cb6
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: f3e110163088f8e3b78da9f273113d74775bf24c
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751899"
---
# <a name="configure-additional-parameter-settings-project-service"></a><span data-ttu-id="baf55-103">קביעת תצורה של הגדרות פרמטרים נוספים (Project Service)</span><span class="sxs-lookup"><span data-stu-id="baf55-103">Configure additional parameter settings (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="baf55-104">לאחר שקבעת את הפריטים בנושאים הקודמים, עליך להגדיר פרמטרים נוספים של הפרוייקט לשימוש עבור הפרוייקטים שלך.</span><span class="sxs-lookup"><span data-stu-id="baf55-104">Once you’ve configured the items in previous topics, you need to set additional project parameters to use for your projects.</span></span> <span data-ttu-id="baf55-105">כאשר התקנת לראשונה את [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], יצרת הגדרת פרמטרים כדי ליצור תחילה את כל הרשומות הדרושות עבור [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="baf55-105">When you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you created a parameters setting to first create all the records required for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to work.</span></span> <span data-ttu-id="baf55-106">כעת הגיע הזמן לחזור ולהגדיר שדות נוספים עבור הגדרת אלה.</span><span class="sxs-lookup"><span data-stu-id="baf55-106">Now it’s time to go back and configure additional fields for these settings.</span></span>  
  
 <span data-ttu-id="baf55-107">עליך לקבוע את ההגדרות הבאות:</span><span class="sxs-lookup"><span data-stu-id="baf55-107">You’ll need to have configured the following settings:</span></span>  
  
-   <span data-ttu-id="baf55-108">יחידה ארגונית</span><span class="sxs-lookup"><span data-stu-id="baf55-108">Organizational unit</span></span>  
  
-   <span data-ttu-id="baf55-109">תדירות הגשת חשבונית</span><span class="sxs-lookup"><span data-stu-id="baf55-109">Invoice frequency</span></span>  
  
-   <span data-ttu-id="baf55-110">תבנית שעות עבודה</span><span class="sxs-lookup"><span data-stu-id="baf55-110">Work hours template</span></span>  
  
-   <span data-ttu-id="baf55-111">מחירון</span><span class="sxs-lookup"><span data-stu-id="baf55-111">Price list</span></span>  
 
<span data-ttu-id="baf55-112">בשלב זה, גם תציין איזה סוג של הקצאת משאבים רצוי לך:</span><span class="sxs-lookup"><span data-stu-id="baf55-112">In this step, you’ll also indicate what type of resource allocation you want:</span></span>  
  
- <span data-ttu-id="baf55-113">**מרכזי**.</span><span class="sxs-lookup"><span data-stu-id="baf55-113">**Central**.</span></span> <span data-ttu-id="baf55-114">רק מנהלי משאבים יוכלו להקצות משאבים לפרוייקטים.</span><span class="sxs-lookup"><span data-stu-id="baf55-114">Only resource managers can allocate resources to projects.</span></span>  
  
- <span data-ttu-id="baf55-115">**היברידי**.</span><span class="sxs-lookup"><span data-stu-id="baf55-115">**Hybrid**.</span></span> <span data-ttu-id="baf55-116">מנהלי משאבים, מנהלי פרוייקטים ומנהלי תיקי לקוחות יוכלו להקצות משאבים לפרוייקטים.</span><span class="sxs-lookup"><span data-stu-id="baf55-116">Resource managers, project managers, and account managers can allocate resources to projects.</span></span>  
  
 
<span data-ttu-id="baf55-117">כדי לקבוע פרמטרים לפרוייקט:</span><span class="sxs-lookup"><span data-stu-id="baf55-117">To set project parameters:</span></span>  
  
1. <span data-ttu-id="baf55-118">עבור אל **Project Service > פרמטרים**.</span><span class="sxs-lookup"><span data-stu-id="baf55-118">Go to **Project Service > Parameters**.</span></span>  
  
2. <span data-ttu-id="baf55-119">לחץ על הגדרת הפרמטרים שברצונך לקבוע (זו שיצרת כאשר התקנת לראשונה את [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]), או לחץ על **חדש** כדי ליצור הגדרה חדשה.</span><span class="sxs-lookup"><span data-stu-id="baf55-119">Click the parameters setting you want to configure (the one you created when you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]), or click **New** to create a new one.</span></span>  
  
3. <span data-ttu-id="baf55-120">באזור **כללי**, הגדר את האפשרויות עבור הפרמטרים של הפרוייקט שלך.</span><span class="sxs-lookup"><span data-stu-id="baf55-120">In the **General** area, set all the options for your project parameters.</span></span>  
  
4. <span data-ttu-id="baf55-121">באזור **מחירון**, לחץ על **+** כדי להוסיף מחירון, בחר מחירון ברשימה הנפתחת **מחירון של פרמטר בפרוייקט**, ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="baf55-121">In the **Price List** area, click **+** to add a price list, select a price list in the **Project Parameter Price List** drop-down list, and then click **Save**.</span></span>  
  
5. <span data-ttu-id="baf55-122">לחץ על הלחצן **שמור** בפינה השמאלית התחתונה של המסך.</span><span class="sxs-lookup"><span data-stu-id="baf55-122">Click the **Save** button in the bottom right corner of the screen.</span></span>  

> [!NOTE]
> <span data-ttu-id="baf55-123">יש לשמור על רשומת הפרמטרים של הפרויקט כדי ש- Project Service יתפקד בצורה תקינה.</span><span class="sxs-lookup"><span data-stu-id="baf55-123">The project parameter record must be maintained for Project Service to function correcly.</span></span> <span data-ttu-id="baf55-124">אין למחוק רשומה זו.</span><span class="sxs-lookup"><span data-stu-id="baf55-124">This record should not be deleted.</span></span>

### <a name="see-also"></a><span data-ttu-id="baf55-125">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="baf55-125">See Also</span></span>  
 [<span data-ttu-id="baf55-126">הגדרת משאבים</span><span class="sxs-lookup"><span data-stu-id="baf55-126">Set up resources</span></span>](../project-service/set-up-resources.md)
