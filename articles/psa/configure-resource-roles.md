---
title: הגדרת תפקידי משאב
description: כיצד להגדיר תפקידי משאב ב- Project Service
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
ms.openlocfilehash: deaff0977ebb50382a28494fba2a1c34ed5cc9b4
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5144909"
---
# <a name="configure-resource-roles-project-service"></a><span data-ttu-id="9c8bd-103">הגדרת תפקידי משאב (Project Service)</span><span class="sxs-lookup"><span data-stu-id="9c8bd-103">Configure resource roles (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="9c8bd-104">תפקידים משחקים תפקיד חשוב בתכנון הפרוייקט, בעת קביעת דרישות המשאבים או עלויות של פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-104">Roles play an important part in project planning, when determining resource requirements or costs of a project.</span></span> <span data-ttu-id="9c8bd-105">עבור כל תפקיד שדורשים הפרוייקטים שלך, עליך ליצור תפקיד משאב ולשייך כישורים ומיומנויות לתפקיד זה.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-105">For each role your projects require, you need to create a resource role and associate skills and proficiencies to that role.</span></span> <span data-ttu-id="9c8bd-106">לדוגמה, ייתכן שתרצה ליצור תפקידים עבור מפתח, מנהל פרוייקט או בוחן משחק.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-106">For example, you might want to create roles for developer, project manager, or game tester.</span></span> <span data-ttu-id="9c8bd-107">גם תגדיר רמות כישורים ומיומנויות הדרושים עבור התפקיד.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-107">You’ll also set the skills and proficiency levels required for the role.</span></span>  
  
 <span data-ttu-id="9c8bd-108">קבע תצורה של תפקידי משאבים כדי להבטיח הערכת פרוייקט יעילה עבור הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-108">Configure resource roles to ensure effective project estimation for your organization.</span></span>  <span data-ttu-id="9c8bd-109">כמו כן, ודא שהגדרת במדויק את סוג החיוב.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-109">Also make sure you accurately set the billing type.</span></span> <span data-ttu-id="9c8bd-110">פריט שהוגדר עם סוג חיוב שאינו ניתן לחיוב לא יופיע בשורות חוזה או הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-110">An item set with a non-chargeable billing type doesn’t show up on contract or quote lines.</span></span>  
  
 <span data-ttu-id="9c8bd-111">לאחר שהגדרת תפקידי משאבים, באפשרותך להגדיר מחירי עלות ומכירה עם מחירון.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-111">Once you’ve set up resource roles, you can set up cost and sales prices with a price list.</span></span>  
  
 <span data-ttu-id="9c8bd-112">עבור כל תפקיד שברצונך להוסיף, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="9c8bd-112">For each role you want to add, do the following:</span></span>  
  
1.  <span data-ttu-id="9c8bd-113">עבור אל **Project Service > תפקידי משאב**.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-113">Go to **Project Service > Resource Roles**.</span></span>  
  
2.  <span data-ttu-id="9c8bd-114">לחץ על **חדש**.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-114">Click **New**.</span></span>  
  
3.  <span data-ttu-id="9c8bd-115">באזור **כללי** הזן שם עבור התפקיד בשדה **שם**, ולאחר מכן מלא שדות אחרים לפי הצורך.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-115">In the **General** area, enter a name for the role in **Name**, and then fill in the other fields as necessary.</span></span>  
  
4.  <span data-ttu-id="9c8bd-116">לחץ על **שמור** כדי ליצור את הרשומה כך שתוכל להמשיך לערוך אותה.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-116">Click **Save** to create the record so you can continue editing it.</span></span>  
  
5.  <span data-ttu-id="9c8bd-117">באזור **כישורים**, לחץ על **+** כדי להוסיף כישור.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-117">In the **Skills** area, click **+** to add a skill.</span></span>  
  
6.  <span data-ttu-id="9c8bd-118">באזור **דרישת כשירות לתפקיד** , לחץ על השדה **כישור** לחץ על הלחצן **חיפוש** ולאחר מכן בחר כישור.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-118">In the **Role competency requirement** pane, click in the **Skill** field, click the **Search** button, and then select a skill.</span></span>  
  
7.  <span data-ttu-id="9c8bd-119">בחר מומחיות עבור כישור זה, ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-119">Select a proficiency for that skill, and then click **Save**.</span></span>  
  
8.  <span data-ttu-id="9c8bd-120">המשך להוסיף כישורים לפי הצורך.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-120">Continue adding skills as necessary.</span></span> <span data-ttu-id="9c8bd-121">אחרי שתסיים, לחץ על **שמור** בפינה הימנית התחתונה של המסך.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-121">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
9. <span data-ttu-id="9c8bd-122">כדי להפוך תפקיד משאב זה לזמין לשימוש עבור פרוייקטים, לחץ על **הפעלה**.</span><span class="sxs-lookup"><span data-stu-id="9c8bd-122">To make this resource role available for projects to use, click **Activate**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="9c8bd-123">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="9c8bd-123">See Also</span></span>  
 [<span data-ttu-id="9c8bd-124">הגדרת משאבים</span><span class="sxs-lookup"><span data-stu-id="9c8bd-124">Set up resources</span></span>](../psa/set-up-resources.md)
