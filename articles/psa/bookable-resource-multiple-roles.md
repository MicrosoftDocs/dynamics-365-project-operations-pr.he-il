---
title: הערך את מכירות הפרוייקט ואת העלויות כאשר משאב שניתן להזמין ממלא מספר תפקידים בפרוייקט
description: נושא זה כולל מידע על אופן השימוש בממדי תמחור כדי לתמוך בתמחור משאב שממלא מספר תפקידים בפרוייקט.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 67e24156e960b9b09cf92f7f0cd77f6c74a982b8
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5145044"
---
# <a name="estimate-project-sales-and-costs-when-a-bookable-resource-fills-multiple-roles-for-a-project"></a><span data-ttu-id="b94ae-103">הערך את מכירות הפרוייקט ואת העלויות כאשר משאב שניתן להזמין ממלא מספר תפקידים בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="b94ae-103">Estimate project sales and costs when a bookable resource fills multiple roles for a project</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="b94ae-104">לחברות מבוססות פרוייקטים לעיתים קרובות יש צורך במשאב אחד שיבצע מספר תפקידים בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b94ae-104">Project-based companies often have the need for one resource to perform multiple roles on a project.</span></span> <span data-ttu-id="b94ae-105">כל אחד מהתפקידים הללו יכול להיות מתומחר בצורה שונה, כלומר אותו זמן של המשאב בפרוייקט יכול לקבל אומדן כספי שונה בהתאם לחשבון ולשיעורי העלות של כל אחד מהתפקידים.</span><span class="sxs-lookup"><span data-stu-id="b94ae-105">Each of these roles could be priced and costed differently, which means the same resource's time on the project could get a different financial estimate depending on the bill and cost rates for each of the roles.</span></span> <span data-ttu-id="b94ae-106">Project Service Automation מאפשר להגדיר ערכים ברשומה של חבר צוות עבור המשאב שצוין ומאפשר עקיפות שונות בכל אחת מהמשימות שחבר הצוות מוקצה להן.</span><span class="sxs-lookup"><span data-stu-id="b94ae-106">Project Service Automation allows the setup of the values on the team member record for the named resource and allows for different overrides on each of the tasks that the team member is assigned to.</span></span>

<span data-ttu-id="b94ae-107">הדוגמה הבאה מסבירה כיצד עקיפה פשוטה של ערך זה מאפשרת למשאב לקבל תפקידים מרובים בפרויקט עם שיעורי עלות וחיוב שונים.</span><span class="sxs-lookup"><span data-stu-id="b94ae-107">The following example  explains how the simple override of this value allows a resource to have multiple roles on a project with different cost and bill rates.</span></span>

## <a name="create-tasks"></a><span data-ttu-id="b94ae-108">יצירת משימות</span><span class="sxs-lookup"><span data-stu-id="b94ae-108">Create tasks</span></span>
<span data-ttu-id="b94ae-109">צור שתי משימות פרויקט למשך 40 שעות כל אחת, משימה א' ומשימה ב'. הגדר שמשימה א' קודמת למשימה ב'.</span><span class="sxs-lookup"><span data-stu-id="b94ae-109">Create two project tasks for 40 hours each, Task A and Task B. Select Task A as a predecessor to Task B.</span></span>

## <a name="set-up-role-and-organization-unit-for-a-generic-project-team-member"></a><span data-ttu-id="b94ae-110">הגדר תפקיד ויחידה בארגון עבור חבר צוות כללי בפרויקט</span><span class="sxs-lookup"><span data-stu-id="b94ae-110">Set up Role and Organization Unit for a generic project team member</span></span>

1. <span data-ttu-id="b94ae-111">בדף **לוח זמנים** בחר את השורה **משימה** למשימה א'.</span><span class="sxs-lookup"><span data-stu-id="b94ae-111">On the **Schedule** page, select the **Task** row for Task A.</span></span> 
2. <span data-ttu-id="b94ae-112">בשדה **משאבים** בחר **צור** ברשימה הנפתחת.</span><span class="sxs-lookup"><span data-stu-id="b94ae-112">In the **Resources** field, select **Create** in the drop-down list.</span></span>
3. <span data-ttu-id="b94ae-113">בדף **יצירה מהירה של חבר צוות**, ציין את התכונות של חבר הצוות הגנרי שיכול לבצע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="b94ae-113">On the **Team Member Quick Create** page, specify the attributes of the generic team member who can perform this task.</span></span>
4. <span data-ttu-id="b94ae-114">בחר את התפקיד והיחידה הארגונית המתאימה, ולאחר מכן בחר **שמור וסגור**.</span><span class="sxs-lookup"><span data-stu-id="b94ae-114">Select the appropriate role and organizational unit, and then select **Save and Close**.</span></span> <span data-ttu-id="b94ae-115">חבר צוות גנרי נוצר ומוקצה למשימה זו.</span><span class="sxs-lookup"><span data-stu-id="b94ae-115">A generic team member is created and assigned to this task.</span></span> 

<span data-ttu-id="b94ae-116">חזור על שלבים אלה עבור משימה ב' וודא שהתפקיד והיחידה הארגונית בחבר הצוות הגנרי שנוצר עבור משימה ב' שונה ממשימה א'.</span><span class="sxs-lookup"><span data-stu-id="b94ae-116">Repeat these steps for Task B and make sure that the role and organizational unit on the generic team member created for Task B is different than Task A.</span></span> 

## <a name="set-up-role-and-organization-unit-for-a-project-task"></a><span data-ttu-id="b94ae-117">הגדר תפקיד ויחידה בארגון עבור משימה בפרויקט</span><span class="sxs-lookup"><span data-stu-id="b94ae-117">Set up role and organization unit for a project task</span></span>

1. <span data-ttu-id="b94ae-118">לאחר יצירת משימה א', בחר את המשימה ולאחר מכן בחר **ערוך את המשימה**.</span><span class="sxs-lookup"><span data-stu-id="b94ae-118">After you create Task A, select the task, and then select **Edit task**.</span></span>
2. <span data-ttu-id="b94ae-119">בדף **פרטי משימה**, מצא את השדות **תפקיד** ו **יחידה ארגונית** והוסף את הערכים הנדרשים של המשאב שיבצע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="b94ae-119">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="b94ae-120">אם אתה משלים תרחישים אלה באמצעות נתוני הדגמה של Project Service Automation, בחר **הפנייה לייעוץ** לתפקיד, ו **Fabrikam US** כיחידה הארגונית.</span><span class="sxs-lookup"><span data-stu-id="b94ae-120">If you are completing this scenarios using Project Service Automation demo data, select **Consulting Lead** for the role, and **Fabrikam US** as the organizational unit.</span></span>

3. <span data-ttu-id="b94ae-121">בחר את משימה ב' ובחר **ערוך משימה**.</span><span class="sxs-lookup"><span data-stu-id="b94ae-121">Select Task B and then select **Edit task**.</span></span>
4. <span data-ttu-id="b94ae-122">בדף **פרטי משימה**, מצא את השדות **תפקיד** ו **יחידה ארגונית** והוסף את הערכים הנדרשים של המשאב שיבצע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="b94ae-122">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> <span data-ttu-id="b94ae-123">ודא שהערכים בשדות **תפקיד** ו **יחידה ארגונית** של משימה B שונים מהערכים עבור משימה A.</span><span class="sxs-lookup"><span data-stu-id="b94ae-123">Make sure that the values in the **Role** and **Organizational Unit** fields are different for Task B from the values for Task A.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="b94ae-124">אם אתה משלים תרחישים אלה באמצעות נתוני הדגמה של Project Service Automation, בחר **טכנאי רשת** לתפקיד, ו **Fabrikam US** כיחידה הארגונית.</span><span class="sxs-lookup"><span data-stu-id="b94ae-124">If you are completing this scenarios using Project Service Automation demo data, select **Network Technician** for the role, and **Fabrikam US** as the organizational unit.</span></span>

5. <span data-ttu-id="b94ae-125">שמור וסגור את הדף **פרטי משימה**.</span><span class="sxs-lookup"><span data-stu-id="b94ae-125">Save and close the **Task Details** page.</span></span> 

## <a name="team-member-and-estimates-behavior"></a><span data-ttu-id="b94ae-126">חבר צוות והתנהגות הערכה</span><span class="sxs-lookup"><span data-stu-id="b94ae-126">Team member and estimates behavior</span></span> 

1. <span data-ttu-id="b94ae-127">בדף **פרטי משימה**, ב **חבר צוות**, בחר את שני חברי הצוות הגנריים ובחר **צור דרישות**.</span><span class="sxs-lookup"><span data-stu-id="b94ae-127">On the **Task Details** page, on the **Team Member**, select the two generic team Members and then select **Generate Requirements**.</span></span> 
2. <span data-ttu-id="b94ae-128">בחר בשורה של חבר הצוות עבור **הפנייה לייעוץ** ובחר **הזמנה**.</span><span class="sxs-lookup"><span data-stu-id="b94ae-128">Select the team member row for **Consulting Lead** and then select **Book**.</span></span> <span data-ttu-id="b94ae-129">לוח הזמנים נפתח ונעשית הזמנת משאב לדרישה זו.</span><span class="sxs-lookup"><span data-stu-id="b94ae-129">The schedule board opens and books a resource to that requirement.</span></span>
3. <span data-ttu-id="b94ae-130">בחר בשורה של חבר הצוות עבור **טכנאי רשת** ובחר **הזמנה**.</span><span class="sxs-lookup"><span data-stu-id="b94ae-130">Select the team member row for **Network Technician** and the select **Book**.</span></span> <span data-ttu-id="b94ae-131">לוח הזמנים נפתח ונעשית הזמנה של אותו משאב לדרישה זו.</span><span class="sxs-lookup"><span data-stu-id="b94ae-131">The schedule board opens and books the same resource on that requirement.</span></span>

### <a name="team-member-grid"></a><span data-ttu-id="b94ae-132">רשת חברי הקבוצה</span><span class="sxs-lookup"><span data-stu-id="b94ae-132">Team Member grid</span></span> 
<span data-ttu-id="b94ae-133">ברשת **חבר צוות**, שים לב ששתי הרשומות של חברי הצוות הכלליים נמחקות והוחלפו במשאב אחד.</span><span class="sxs-lookup"><span data-stu-id="b94ae-133">On the **Team Member** grid, notice that the two generic team member records are deleted and have been replaced one resource.</span></span> <span data-ttu-id="b94ae-134">יש קבוצה אחת של ערכים עבור אותו משאב המציגה ערכת ברירת מחדל של ערכים עבור **תפקיד** ו **יחידה ארגונית**.</span><span class="sxs-lookup"><span data-stu-id="b94ae-134">There is one set of values for that resource that shows a default set of values for **Role** and **Organizational Unit**.</span></span>
<span data-ttu-id="b94ae-135">כאשר אתה מרחיב את השורה של אותה רשומת חבר צוות, אתה יכול לראות משימות נפרדות ברשומת חבר הצוות עבור שתי המשימות האלה.</span><span class="sxs-lookup"><span data-stu-id="b94ae-135">When you expand the row of that Team Member record, you can see distinct assignments on the team member record for both of those tasks.</span></span> <span data-ttu-id="b94ae-136">לכל שורת משימות יש ערכים ספציפיים למשימה עבור **תפקיד** ו **יחידה ארגונית**.</span><span class="sxs-lookup"><span data-stu-id="b94ae-136">Each assignment row has task-specific values for **Role** and **Organizational Unit**.</span></span> 

### <a name="estimates-grid"></a><span data-ttu-id="b94ae-137">רשת הערכות</span><span class="sxs-lookup"><span data-stu-id="b94ae-137">Estimates grid</span></span> 
<span data-ttu-id="b94ae-138">כשאתה עובר אל רשת **אומדנים**, תוכל להבחין ששתי המשימות עבור אותו משאב מתומחרות אחרת.</span><span class="sxs-lookup"><span data-stu-id="b94ae-138">When you navigate to the **Estimates** grid, you will notice that both assignments for the same resource are priced differently.</span></span>
<span data-ttu-id="b94ae-139">הקצאת המשאב למשימה א' מתומחרת לפי הערך בשדה **תפקיד** של **הפנייה לייעוץ**.</span><span class="sxs-lookup"><span data-stu-id="b94ae-139">The assignment for the resource on Task A is priced using the **Role** attribute value of **Consulting Lead**.</span></span> <span data-ttu-id="b94ae-140">ההקצאה של אותו משאב למשימה ב' מתומחרת לפי הערך בשדה **תפקיד** של **טכנאי רשת**.</span><span class="sxs-lookup"><span data-stu-id="b94ae-140">The assignment for the same resource on Task B is priced using the **Role** attribute value of **Network Technician**.</span></span>

