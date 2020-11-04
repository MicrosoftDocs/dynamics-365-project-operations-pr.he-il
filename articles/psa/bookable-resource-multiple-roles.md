---
title: הערך את מכירות הפרויקטים והעלויות כאשר משאב שניתן להזמין ממלא תפקידים מרובים בפרויקט
description: נושא זה מספק מידע על האופן שבו ניתן להשתמש בממדי תמחור לתמיכה בתמחור ובמחיר עבור משאב שממלא תפקידים מרובים בפרויקט.
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
ms.openlocfilehash: 8ddc827a4170c5576c0a4350b51e6a119094ac50
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077360"
---
# <a name="estimate-project-sales-and-costs-when-a-bookable-resource-fills-mulitple-roles-on-a-project"></a><span data-ttu-id="bbb9a-103">הערך את מכירות הפרויקטים והעלויות כאשר משאב שניתן להזמין ממלא תפקידים מרובים בפרויקט</span><span class="sxs-lookup"><span data-stu-id="bbb9a-103">Estimate project sales and costs when a bookable resource fills mulitple roles on a project</span></span> 

<span data-ttu-id="bbb9a-104">לחברות מבוססות פרויקטים לעיתים קרובות יש צורך במשאב אחד לביצוע תפקידים מרובים בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-104">Project-based companies often have the need for one resource to perform mulitple roles on a project.</span></span> <span data-ttu-id="bbb9a-105">כל אחד מהתפקידים הללו יכול להיות מתומחר בצורה שונה, מה שאומר שאותו זמן של המשאב בפרויקט יכול לקבל אומדן כספי שונה בהתאם לחשבון ולשיעורי העלות של כל אחד מהתפקידים.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-105">Each of these roles could be priced and costed differently which means the same resource's time on the project could get a different financial estimate depending on the bill and cost rates for each of the roles.</span></span> <span data-ttu-id="bbb9a-106">Project Service Automation מאפשר להגדיר ערכים ברשומה של חבר צוות עבור המשאב שצוין ומאפשר עקיפות שונות בכל אחת מהמשימות שחבר הצוות מוקצה להן.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-106">Project Service Automation allows the setup of the values on the team member record for the named resource and allows for different overrides on each of the tasks that the team member is assigned to.</span></span>

<span data-ttu-id="bbb9a-107">הדוגמה הבאה מסבירה כיצד עקיפה פשוטה של ערך זה מאפשרת למשאב לקבל תפקידים מרובים בפרויקט עם שיעורי עלות וחיוב שונים.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-107">The following example  explains how the simple override of this value allows a resource to have multiple roles on a project with different cost and bill rates.</span></span>

## <a name="create-tasks"></a><span data-ttu-id="bbb9a-108">יצירת משימות</span><span class="sxs-lookup"><span data-stu-id="bbb9a-108">Create tasks</span></span>
<span data-ttu-id="bbb9a-109">צור שתי משימות פרויקט למשך 40 שעות כל אחת, משימה א' ומשימה ב'. הגדר שמשימה א' קודמת למשימה ב'.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-109">Create two project tasks for 40 hours each, Task A and Task B. Select Task A as a predecessor to Task B.</span></span>

## <a name="set-up-role-and-organization-unit-for-a-generic-project-team-member"></a><span data-ttu-id="bbb9a-110">הגדר תפקיד ויחידה בארגון עבור חבר צוות כללי בפרויקט</span><span class="sxs-lookup"><span data-stu-id="bbb9a-110">Set up Role and Organization Unit for a generic project team member</span></span>

1. <span data-ttu-id="bbb9a-111">בדף **לוח זמנים** בחר את השורה **משימה** למשימה א'.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-111">On the **Schedule** page, select the **Task** row for Task A.</span></span> 
2. <span data-ttu-id="bbb9a-112">בשדה **משאבים** בחר **צור** ברשימה הנפתחת.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-112">In the **Resources** field, select **Create** in the drop-down list.</span></span>
3. <span data-ttu-id="bbb9a-113">בדף **יצירה מהירה של חבר צוות** , ציין את התכונות של חבר הצוות הגנרי שיכול לבצע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-113">On the **Team Member Quick Create** page, specify the attributes of the generic team member who can perform this task.</span></span>
4. <span data-ttu-id="bbb9a-114">בחר את התפקיד והיחידה הארגונית המתאימה, ולאחר מכן בחר **שמור וסגור**.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-114">Select the appropriate role and organizational unit, and then select **Save and Close**.</span></span> <span data-ttu-id="bbb9a-115">חבר צוות גנרי נוצר ומוקצה למשימה זו.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-115">A generic team member is created and assigned to this task.</span></span> 

<span data-ttu-id="bbb9a-116">חזור על שלבים אלה עבור משימה ב' וודא שהתפקיד והיחידה הארגונית בחבר הצוות הגנרי שנוצר עבור משימה ב' שונה ממשימה א'.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-116">Repeat these steps for Task B and make sure that the role and organizational unit on the generic team member created for Task B is different than Task A.</span></span> 

## <a name="set-up-role-and-organization-unit-for-a-project-task"></a><span data-ttu-id="bbb9a-117">הגדר תפקיד ויחידה בארגון עבור משימה בפרויקט</span><span class="sxs-lookup"><span data-stu-id="bbb9a-117">Set up role and organization unit for a project task</span></span>

1. <span data-ttu-id="bbb9a-118">לאחר יצירת משימה א', בחר את המשימה ולאחר מכן בחר **ערוך את המשימה**.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-118">After you create Task A, select the task, and then select **Edit task**.</span></span>
2. <span data-ttu-id="bbb9a-119">בדף **פרטי משימה** , מצא את השדות **תפקיד** ו **יחידה ארגונית** והוסף את הערכים הנדרשים של המשאב שיבצע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-119">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="bbb9a-120">אם אתה משלים תרחישים אלה באמצעות נתוני הדגמה של Project Service Automation, בחר **הפנייה לייעוץ** לתפקיד, ו **Fabrikam US** כיחידה הארגונית.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-120">If you are completing this scenarios using Project Service Automation demo data, select **Consulting Lead** for the role, and **Fabrikam US** as the organizational unit.</span></span>

3. <span data-ttu-id="bbb9a-121">בחר את משימה ב' ובחר **ערוך משימה**.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-121">Select Task B and then select **Edit task**.</span></span>
4. <span data-ttu-id="bbb9a-122">בדף **פרטי משימה** , מצא את השדות **תפקיד** ו **יחידה ארגונית** והוסף את הערכים הנדרשים של המשאב שיבצע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-122">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> <span data-ttu-id="bbb9a-123">ודא שהערכים בשדות **תפקיד** ו **יחידה ארגונית** שונים עבור משימה ב' מאלה של משימה א'.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-123">Make sure that the values in the **Role** and **Organizational Unit** fields are different for Task B from those for Task A.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="bbb9a-124">אם אתה משלים תרחישים אלה באמצעות נתוני הדגמה של Project Service Automation, בחר **טכנאי רשת** לתפקיד, ו **Fabrikam US** כיחידה הארגונית.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-124">If you are completing this scenarios using Project Service Automation demo data, select **Network Technician** for the role, and **Fabrikam US** as the organizational unit.</span></span>

5. <span data-ttu-id="bbb9a-125">שמור וסגור את הדף **פרטי משימה**.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-125">Save and close the **Task Details** page.</span></span> 

## <a name="team-member-and-estimates-behaviour"></a><span data-ttu-id="bbb9a-126">חבר צוות ומעריך התנהגות</span><span class="sxs-lookup"><span data-stu-id="bbb9a-126">Team member and estimates behaviour</span></span> 

1. <span data-ttu-id="bbb9a-127">בדף **פרטי משימה** , ב **חבר צוות** , בחר את שני חברי הצוות הגנריים ובחר **צור דרישות**.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-127">On the **Task Details** page, on the **Team Member** , select the two generic team Members and then select **Generate Requirements**.</span></span> <span data-ttu-id="bbb9a-128">בעקבות זאת ייווצרו דרישות המשאבים.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-128">This will generate resource requirements.</span></span> 
2. <span data-ttu-id="bbb9a-129">בחר בשורה של חבר הצוות עבור **הפנייה לייעוץ** ובחר **הזמנה**.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-129">Select the team member row for **Consulting Lead** and then select **Book**.</span></span> <span data-ttu-id="bbb9a-130">לוח הזמנים נפתח ונעשית הזמנת משאב לדרישה זו.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-130">The schedule board opens and books a resource to that requirement.</span></span>
3. <span data-ttu-id="bbb9a-131">בחר בשורה של חבר הצוות עבור **טכנאי רשת** ובחר **הזמנה**.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-131">Select the team member row for **Network Technician** and the select **Book**.</span></span> <span data-ttu-id="bbb9a-132">לוח הזמנים נפתח ונעשית הזמנה של אותו משאב לדרישה זו.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-132">The schedule board opens and books the same resource on that requirement.</span></span>

### <a name="team-member-grid"></a><span data-ttu-id="bbb9a-133">רשת חברי הקבוצה</span><span class="sxs-lookup"><span data-stu-id="bbb9a-133">Team Member grid</span></span> 
<span data-ttu-id="bbb9a-134">ברשת **חבר צוות** , שים לב ששתי הרשומות של חברי הצוות הכלליים נמחקות והוחלפו במשאב אחד.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-134">On the **Team Member** grid, notice that the two generic team member records are deleted and have been replaced one resource.</span></span> <span data-ttu-id="bbb9a-135">יש קבוצה אחת של ערכים עבור אותו משאב המציגה ערכת ברירת מחדל של ערכים עבור **תפקיד** ו **יחידה ארגונית**.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-135">There is one set of values for that resource that shows a default set of values for **Role** and **Organizational Unit**.</span></span>
<span data-ttu-id="bbb9a-136">כאשר אתה מרחיב את השורה של אותה רשומת חבר צוות, אתה יכול לראות משימות נפרדות ברשומת חבר הצוות עבור שתי המשימות האלה.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-136">When you expand the row of that Team Member record, you can see distinct assignments on the team member record for both of those tasks.</span></span> <span data-ttu-id="bbb9a-137">לכל שורת משימות יש ערכים ספציפיים למשימה עבור **תפקיד** ו **יחידה ארגונית**.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-137">Each assignment row has task specific values for **Role** and **Organizational Unit**.</span></span> 

### <a name="estimates-grid"></a><span data-ttu-id="bbb9a-138">רשת הערכות</span><span class="sxs-lookup"><span data-stu-id="bbb9a-138">Estimates grid</span></span> 
<span data-ttu-id="bbb9a-139">כשאתה עובר אל רשת **אומדנים** , תוכל להבחין ששתי המשימות עבור אותו משאב מתומחרות אחרת.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-139">When you navigate to the **Estimates** grid, you will notice that both assignments for the same resource are priced differently.</span></span>
<span data-ttu-id="bbb9a-140">הקצאת המשאב למשימה א' מתומחרת לפי הערך בשדה **תפקיד** של **הפנייה לייעוץ**.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-140">The assignment for the resource on Task A is priced using the **Role** attribute value of **Consulting Lead**.</span></span> <span data-ttu-id="bbb9a-141">ההקצאה של אותו משאב למשימה ב' מתומחרת לפי הערך בשדה **תפקיד** של **טכנאי רשת**.</span><span class="sxs-lookup"><span data-stu-id="bbb9a-141">The assignment for the same resource on Task B is priced using the **Role** attribute value of **Network Technician**.</span></span>





