---
title: הערך את מכירות הפרויקט ואת העלויות כאשר משאב שניתן להזמין ממלא מספר תפקידים בפרויקט
description: נושא זה מסביר כיצד להשתמש בממדי תמחור כדי לתמוך באומדני תמחור ובתמחור עבור משאב שממלא מספר תפקידים בפרויקט.
author: rumant
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 7ef9765b7db1c6650fb0599bf5fb4b4b6304be69
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013667"
---
# <a name="estimate-project-sales-and-costs-when-a-bookable-resource-fills-multiple-roles-on-a-project"></a><span data-ttu-id="26478-103">הערך את מכירות הפרויקט ואת העלויות כאשר משאב שניתן להזמין ממלא מספר תפקידים בפרויקט</span><span class="sxs-lookup"><span data-stu-id="26478-103">Estimate project sales and costs when a bookable resource fills multiple roles on a project</span></span> 

<span data-ttu-id="26478-104">_**חל על:** ‏ Project Operations לתרחישים מבוססי משאבים/ללא מלאי, פריסת לייט - מעסקה לחשבונית פרופורמה, Project Operations לתרחישים מלאי/מבוססי ייצור_</span><span class="sxs-lookup"><span data-stu-id="26478-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing, Project Operations for stocked/production-based scenarios_</span></span> 

<span data-ttu-id="26478-105">לחברות מבוססות פרויקטים לעיתים קרובות יש צורך במשאב אחד שימלא מספר תפקידים בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="26478-105">Project-based companies often have the need for one resource to fill multiple roles on a project.</span></span> <span data-ttu-id="26478-106">ניתן לתמחר כל תפקיד ולהגדיר לו עלות בצורה שונה.</span><span class="sxs-lookup"><span data-stu-id="26478-106">Each role can be priced and costed differently.</span></span> <span data-ttu-id="26478-107">המשמעות היא שהזמן אותו משאב בפרויקט יכול לקבל אומדן כספי שונה בהתאם לחשבון ולשיעורי העלות עבור כל תפקיד.</span><span class="sxs-lookup"><span data-stu-id="26478-107">This means that the same resource's time on a project could get a different financial estimate depending on the bill and cost rates for each role.</span></span> <span data-ttu-id="26478-108">באפשרותך להגדיר את הערכים ברשומת חברי הצוות עבור המשאב הנקוב עם עקיפות שונות על כל אחת מהמשימות שחבר הצוות מוקצה להן.</span><span class="sxs-lookup"><span data-stu-id="26478-108">You can set up the values on the team member record for the named resource with different overrides on each of the tasks that the team member is assigned to.</span></span>

<span data-ttu-id="26478-109">הדוגמה הבאה מדריכה אותך כיצד עקיפה פשוטה של ערך מאפשרת למשאב לקבל תפקידים מרובים בפרויקט עם שיעורי עלות וחיוב שונים.</span><span class="sxs-lookup"><span data-stu-id="26478-109">The following example walks you through how the simple override of a value allows a resource to have multiple roles on a project with different cost and bill rates.</span></span>

## <a name="create-tasks"></a><span data-ttu-id="26478-110">יצירת משימות</span><span class="sxs-lookup"><span data-stu-id="26478-110">Create tasks</span></span>
<span data-ttu-id="26478-111">כדי ליצור משימות, עליך להוסיף משימות ומשימות סיכום, ולאחר מכן עליך להקצות את המשימה לפני שתוסיף משך למשימות.</span><span class="sxs-lookup"><span data-stu-id="26478-111">To create tasks, you need to add tasks, as well as summary tasks, after which you need to assign the task before you add task duration.</span></span> 

### <a name="add-tasks-and-summary-tasks"></a><span data-ttu-id="26478-112">הוסף משימות ומשימות סיכום</span><span class="sxs-lookup"><span data-stu-id="26478-112">Add tasks and summary tasks</span></span>
<span data-ttu-id="26478-113">כדי להוסיף משימה יש לבצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="26478-113">To add a task, complete the following steps.</span></span>

1. <span data-ttu-id="26478-114">עבור אל **פרויקטים** ופתח את הפרויקט שאליו ברצונך להוסיף משימות.</span><span class="sxs-lookup"><span data-stu-id="26478-114">Go to **Projects** and open the project to which you want to add tasks.</span></span>
2. <span data-ttu-id="26478-115">בחר **הוספת משימה חדשה**.</span><span class="sxs-lookup"><span data-stu-id="26478-115">Select **Add new task**.</span></span> <span data-ttu-id="26478-116">תן שם למשימה ולחץ על **Enter**.</span><span class="sxs-lookup"><span data-stu-id="26478-116">Name the task, and then press **Enter**.</span></span>
3. <span data-ttu-id="26478-117">תן שם נוסף למשימה ולחץ על **Enter**.</span><span class="sxs-lookup"><span data-stu-id="26478-117">Enter another task name and press **Enter**.</span></span> <span data-ttu-id="26478-118">חזור על פעולה זו עד שתהיה לך רשימה מלאה של משימות.</span><span class="sxs-lookup"><span data-stu-id="26478-118">Repeat this until you have a full list of tasks.</span></span>
3. <span data-ttu-id="26478-119">כדי להסיט משימות פנימה, תחת משימות **סיכום**, בחר את סמל שלוש הנקודות האנכיות לפי שם המשימה, ואז בחר **הפוך למשימת משנה**.</span><span class="sxs-lookup"><span data-stu-id="26478-119">To indent tasks under **Summary** tasks, select the three vertical dots by the task name, and then select **Make subtask**.</span></span> 

  > [!TIP]
  > <span data-ttu-id="26478-120">לבחירת יותר ממשימה אחת, בחר משימה, לחץ והחזק את מקש **Ctrl** ולאחר מכן בחר משימה אחרת.</span><span class="sxs-lookup"><span data-stu-id="26478-120">To select more than one task, select a task, press and hold **Ctrl**, and then select another task.</span></span>
  >
  > <span data-ttu-id="26478-121">אפשר גם לבחור **קדם משימת משנה** כדי להעביר משימות מתחת למשימות **סיכום**.</span><span class="sxs-lookup"><span data-stu-id="26478-121">You can also choose **Promote subtask** to move tasks out from under **Summary** tasks.</span></span>

### <a name="assign-tasks"></a><span data-ttu-id="26478-122">הקצאת משימות</span><span class="sxs-lookup"><span data-stu-id="26478-122">Assign tasks</span></span>

<span data-ttu-id="26478-123">כדי להקצות משימה יש לבצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="26478-123">Complete the following steps to assign tasks.</span></span>

1. <span data-ttu-id="26478-124">בעמודה **הוקצה ל** של משימה, בחר בסמל האדם.</span><span class="sxs-lookup"><span data-stu-id="26478-124">In the  **Assigned to**  column for a task, select the person icon.</span></span>
2. <span data-ttu-id="26478-125">בחר חבר צוות מהרשימה או הזן טקסט כדי לחפש שם.</span><span class="sxs-lookup"><span data-stu-id="26478-125">Choose a team member from the list or enter text to search for a name.</span></span>

### <a name="add-task-duration-and-columns"></a><span data-ttu-id="26478-126">הוסף משך משימה ועמודות</span><span class="sxs-lookup"><span data-stu-id="26478-126">Add task duration and columns</span></span>

<span data-ttu-id="26478-127">לעתים קרובות הכי קל להתחיל לבנות את הפרויקט שלך עם משך זמן.</span><span class="sxs-lookup"><span data-stu-id="26478-127">It's often easiest to begin constructing your project with duration.</span></span> <span data-ttu-id="26478-128">כדי להוסיף משך זמן יש לבצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="26478-128">Complete the following steps to add a task duration.</span></span>

1. <span data-ttu-id="26478-129">בעמודה **משך** של המשימה, הקלד את מספר הימים שלדעתך ייקח לבצע את המשימה.</span><span class="sxs-lookup"><span data-stu-id="26478-129">In the **Duration** column for a task, type the number of days you think it will take to accomplish the task.</span></span> <span data-ttu-id="26478-130">אם ברצונך להשתמש ביחידת זמן אחרת, הזן מספר בתוספת המילה **שעות**, **שבועות** או **חודשים**.</span><span class="sxs-lookup"><span data-stu-id="26478-130">If you want to use a different unit of time, enter a number plus the word **hours**, **weeks**, or **months**.</span></span>
2. <span data-ttu-id="26478-131">אם אתה רוצה שהמשימה שלך תופיע כאבן דרך בצורת יהלום בתצוגת **ציר הזמן**, בעמודה **משך** הזן **0 ימים**.</span><span class="sxs-lookup"><span data-stu-id="26478-131">If you want your task to appear as a diamond-shaped milestone in the **Timeline** view, in the **Duration** column, enter **0 days** .</span></span>
3. <span data-ttu-id="26478-132">לחץ על **Enter‎** כדי לעבור לשדה **משך** של המשימה הבאה והמשך להזין משכי זמן.</span><span class="sxs-lookup"><span data-stu-id="26478-132">Press **Enter**  to go to the next task's **Duration** field and continue entering durations.</span></span>

  > [!NOTE]
  > <span data-ttu-id="26478-133">אינך יכול להזין משך זמן למשימות סיכום.</span><span class="sxs-lookup"><span data-stu-id="26478-133">You can't enter a duration for summary tasks.</span></span>

<span data-ttu-id="26478-134">אתה יכול להוסיף עמודות לפרויקט כדי לספק פרטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="26478-134">You can add columns to your project to provide more details.</span></span> <span data-ttu-id="26478-135">לשם כך בחר **הוסף עמודה**.</span><span class="sxs-lookup"><span data-stu-id="26478-135">To do this, select **Add column**.</span></span> 

<span data-ttu-id="26478-136">לקבלת מידע נוסף, ראה [יצירת פרויקט](https://support.microsoft.com/en-us/office/create-a-project-a5b5e823-fb2e-45fd-be00-7d84422d9749).</span><span class="sxs-lookup"><span data-stu-id="26478-136">For more information, see [Create a project](https://support.microsoft.com/en-us/office/create-a-project-a5b5e823-fb2e-45fd-be00-7d84422d9749).</span></span>

## <a name="set-up-the-role-and-organization-unit-for-a-generic-project-team-member"></a><span data-ttu-id="26478-137">הגדר את התפקיד ואת היחידה בארגון עבור חבר צוות גנרי בפרויקט</span><span class="sxs-lookup"><span data-stu-id="26478-137">Set up the role and organization unit for a generic project team member</span></span>
<span data-ttu-id="26478-138">בצע את השלבים הבאים להגדרת תפקיד ויחידה ארגונית עבור חבר צוות כללי.</span><span class="sxs-lookup"><span data-stu-id="26478-138">Complete the following steps to set up a role and organizational unit for a generic team member.</span></span>

1. <span data-ttu-id="26478-139">בדף **משימות** בחר את השורה **משימה** עבור **משימה א'**.</span><span class="sxs-lookup"><span data-stu-id="26478-139">On the **Tasks** page, select the **Task** row for **Task A**.</span></span> 
2. <span data-ttu-id="26478-140">בשדה **הוקצה ל**, בחר **הוסף משאב כללי**.</span><span class="sxs-lookup"><span data-stu-id="26478-140">In **Assigned To**, select **Add generic resource**.</span></span> <span data-ttu-id="26478-141">זה פותח את הדף **יצירה מהירה של חבר צוות**.</span><span class="sxs-lookup"><span data-stu-id="26478-141">This opens the **Team Member Quick Create** page.</span></span>
3. <span data-ttu-id="26478-142">בדף **יצירה מהירה של חבר צוות**, ציין את התכונות של חבר הצוות הגנרי שיכול לבצע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="26478-142">On the **Team Member Quick Create** page, specify the attributes of the generic team member who can perform this task.</span></span>
4. <span data-ttu-id="26478-143">בחר את התפקיד והיחידה הארגונית המתאימה, ולאחר מכן בחר **שמור וסגור**.</span><span class="sxs-lookup"><span data-stu-id="26478-143">Select the appropriate role and organizational unit, and then select **Save and Close**.</span></span> <span data-ttu-id="26478-144">חבר צוות גנרי נוצר ומוקצה למשימה זו.</span><span class="sxs-lookup"><span data-stu-id="26478-144">A generic team member is created and assigned to this task.</span></span> 
5. <span data-ttu-id="26478-145">חזור על שלבים 1-4 עבור **משימה ב'**. עם זאת, ל **משימה ב'** צריך להיות תפקיד אחר ויחידה ארגונית שונה עבור חבר הצוות הגנרי לעומת **משימה א'**.</span><span class="sxs-lookup"><span data-stu-id="26478-145">Repeat steps 1-4 for **Task B**. However, **Task B** must have a different role and organizational unit assigned for the generic team member than **Task A**.</span></span> 

## <a name="set-up-the-role-and-organization-unit-for-a-project-task"></a><span data-ttu-id="26478-146">הגדר את התפקיד ואת היחידה בארגון עבור משימה בפרויקט</span><span class="sxs-lookup"><span data-stu-id="26478-146">Set up the role and organization unit for a project task</span></span>
<span data-ttu-id="26478-147">בצע את השלבים הבאים להגדרת תפקיד ויחידה ארגונית עבור משימה.</span><span class="sxs-lookup"><span data-stu-id="26478-147">Complete the following steps to set up a role and organizational unit for a task.</span></span>

1. <span data-ttu-id="26478-148">אחרי יצירת **משימה א**, בחר את המשימה ולאחר מכן בחר את הסמל **i** כדי לפתוח את החלונית **פרטי משימה**.</span><span class="sxs-lookup"><span data-stu-id="26478-148">After you create **Task A**, select the task, and then select the **i** icon to open the **Task Details** pane.</span></span> 
2. <span data-ttu-id="26478-149">בחלונית **פרטי משימה** גלול לתחתית ובחר **הצג פרטים** כדי לפתוח את הדף **פרטי משימה**.</span><span class="sxs-lookup"><span data-stu-id="26478-149">On the **Task Details** pane, scroll to the bottom and select **View Details** to open the **Task Details** page.</span></span>
3. <span data-ttu-id="26478-150">בדף **פרטי משימה**, בחלקים **תפקיד** ו **יחידה ארגונית**, הוסף את הערכים הנדרשים לביצוע משימה זו עבור המשאב.</span><span class="sxs-lookup"><span data-stu-id="26478-150">On the **Task Details** page, in **Role** and **Organizational Unit**, add the values that are required to perform this task for the resource.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="26478-151">אם השלמת תרחיש זה באמצעות נתוני ההדגמה של Project Operations, בחר **יועץ בכיר** לתפקיד, ו **Fabrikam US** כיחידה הארגונית.</span><span class="sxs-lookup"><span data-stu-id="26478-151">If you complete this scenario using the Project Operations demo data, select **Consulting Lead** for the role, and **Fabrikam US** as the organizational unit.</span></span>

4. <span data-ttu-id="26478-152">בחר את **משימה ב'**, ולאחר מכן בחר את המשימה.</span><span class="sxs-lookup"><span data-stu-id="26478-152">Select **Task B**, and then select the task.</span></span>
5. <span data-ttu-id="26478-153">בחר את הסמל **i** כדי לפתוח את החלונית **פרטי משימה**.</span><span class="sxs-lookup"><span data-stu-id="26478-153">Select the **i** icon to open **Task Details** pane.</span></span> 
6. <span data-ttu-id="26478-154">בחלונית **פרטי משימה** גלול לתחתית ובחר **הצג פרטים** כדי לפתוח את הדף **פרטי משימה**.</span><span class="sxs-lookup"><span data-stu-id="26478-154">On the **Task Details** pane, scroll to the bottom and select **View details** to open the **Task Details** page.</span></span>
7. <span data-ttu-id="26478-155">בדף **פרטי משימה**, בחלקים **תפקיד** ו **יחידה ארגונית**, הוסף את הערכים הנדרשים עבור המשאב שיבצע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="26478-155">On the **Task Details** page, in **Role** and **Organizational Unit**, add the values that are required of a resource that would perform this task.</span></span> <span data-ttu-id="26478-156">הערכים **תפקיד** ו **יחידה ארגונית** של **משימה ב'** צריכים להיות שונים מאלה של **משימה א'**.</span><span class="sxs-lookup"><span data-stu-id="26478-156">The values in **Role** and **Organizational Unit** for **Task B** must be different than those for **Task A**.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="26478-157">אם השלמת תרחיש זה באמצעות נתוני ההדגמה של Project Operations, בחר **טכנאי רשת** לתפקיד, ו **Fabrikam US** כיחידה הארגונית.</span><span class="sxs-lookup"><span data-stu-id="26478-157">If you complete this scenario using the Project Operations demo data, select **Network Technician** for the role, and **Fabrikam US** as the organizational unit.</span></span>

8. <span data-ttu-id="26478-158">שמור וסגור את הדף **פרטי משימה**.</span><span class="sxs-lookup"><span data-stu-id="26478-158">Save and close the **Task Details** page.</span></span> 

## <a name="team-member-and-estimates-behavior"></a><span data-ttu-id="26478-159">חבר צוות והתנהגות הערכה</span><span class="sxs-lookup"><span data-stu-id="26478-159">Team member and estimates behavior</span></span> 
<span data-ttu-id="26478-160">כדי להבין את ההתנהגות ברשת **חבר צוות** ואת ההערכות, השלם את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="26478-160">To understand the behavior on the **Team Member** grid and the estimates, complete the following steps.</span></span>

1. <span data-ttu-id="26478-161">ברשת **חבר צוות** בחר את שני חברי הצוות הגנריים ובחר **צור דרישות**.</span><span class="sxs-lookup"><span data-stu-id="26478-161">On the **Team Member** grid, select the two generic team members, and then select **Generate Requirements**.</span></span> <span data-ttu-id="26478-162">בעקבות זאת ייווצרו דרישות המשאבים.</span><span class="sxs-lookup"><span data-stu-id="26478-162">This will generate resource requirements.</span></span> 
2. <span data-ttu-id="26478-163">בחר בשורה של חבר הצוות עבור **הפנייה לייעוץ** ובחר **הזמנה**.</span><span class="sxs-lookup"><span data-stu-id="26478-163">Select the team member row for **Consulting Lead**, and then select **Book**.</span></span> <span data-ttu-id="26478-164">לוח הזמנים נפתח עם רשימת משאבים.</span><span class="sxs-lookup"><span data-stu-id="26478-164">The schedule board opens with a list of resources.</span></span> <span data-ttu-id="26478-165">בחר משאב ובחר **הזמן** כדי להזמין את המשאב לדרישה זו.</span><span class="sxs-lookup"><span data-stu-id="26478-165">Select a resource and then select **Book** to book the resource to that requirement.</span></span>
3. <span data-ttu-id="26478-166">בחר בשורה של חבר הצוות עבור **טכנאי רשת** ובחר **הזמנה**.</span><span class="sxs-lookup"><span data-stu-id="26478-166">Select the team member row for **Network Technician**, and then select **Book**.</span></span> <span data-ttu-id="26478-167">לוח הזמנים נפתח עם רשימת משאבים.</span><span class="sxs-lookup"><span data-stu-id="26478-167">The schedule board opens with a list of resources.</span></span> <span data-ttu-id="26478-168">בחר אותו משאב כמו קודם ובחר **הזמן** כדי להזמין את המשאב לדרישה זו.</span><span class="sxs-lookup"><span data-stu-id="26478-168">Select the same resource as above and then select **Book** to book the resource to that requirement.</span></span>

### <a name="team-member-grid"></a><span data-ttu-id="26478-169">רשת חברי הקבוצה</span><span class="sxs-lookup"><span data-stu-id="26478-169">Team Member grid</span></span> 

<span data-ttu-id="26478-170">ברשת **חבר צוות**, שתי הרשומות של חברי צוות כלליים נמחקות ומוחלפות במשאב אחד בלבד.</span><span class="sxs-lookup"><span data-stu-id="26478-170">On the **Team Member** grid, the two generic team member records are deleted and replaced with only one resource.</span></span> <span data-ttu-id="26478-171">יש קבוצה אחת של ערכים עבור אותו משאב, שהם קבוצת ערכים המוגדרת כברירת מחדל עבור **תפקיד** ו **יחידה ארגונית**.</span><span class="sxs-lookup"><span data-stu-id="26478-171">There is one set of values for that resource, which are a default set of values for **Role** and **Organizational Unit**.</span></span>

<span data-ttu-id="26478-172">כאשר אתה מרחיב את השורה עבור אותה רשומה של חברי צוות, תוכל לראות מטלות נפרדות ברשומת חברי הצוות לשתי המשימות.</span><span class="sxs-lookup"><span data-stu-id="26478-172">When you expand the row for that team member record, you can see distinct assignments on the team member record for both tasks.</span></span> <span data-ttu-id="26478-173">לכל שורת משימות יש ערכים ספציפיים למשימה עבור **תפקיד** ו **יחידה ארגונית**.</span><span class="sxs-lookup"><span data-stu-id="26478-173">Each assignment row has task-specific values for **Role** and **Organizational Unit**.</span></span> 

### <a name="estimates-grid"></a><span data-ttu-id="26478-174">רשת הערכות</span><span class="sxs-lookup"><span data-stu-id="26478-174">Estimates grid</span></span> 

<span data-ttu-id="26478-175">ברשת **אומדנים**, שתי המטלות עבור אותו משאב מתומחרות אחרת.</span><span class="sxs-lookup"><span data-stu-id="26478-175">On the **Estimates** grid, both assignments for the same resource are priced differently.</span></span> <span data-ttu-id="26478-176">ההקצאה של המשאב ב **משימה א'** מתומחרת לפי הערך בשדה **תפקיד** של **יועץ בכיר**.</span><span class="sxs-lookup"><span data-stu-id="26478-176">The assignment for the resource on **Task A** is priced using the **Role** attribute value of **Consulting Lead**.</span></span> <span data-ttu-id="26478-177">ההקצאה של אותו משאב ל **משימה ב'** מתומחרת לפי הערך בשדה **תפקיד** של **טכנאי רשת**.</span><span class="sxs-lookup"><span data-stu-id="26478-177">The assignment for the same resource on **Task B** is priced using the **Role** attribute value of **Network Technician**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]