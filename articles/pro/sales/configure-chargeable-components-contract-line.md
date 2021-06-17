---
title: ‏‫קביעת תצורה של רכיבים ניתנים לחיוב בסעיף חוזה מבוסס פרוייקט‬
description: נושא זה מספק מידע על אופן הוספת רכיבים הניתנים לחיוב לסעיפי חוזה ב-Project Operations.
author: rumant
ms.date: 10/08/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b29c912828aa4af2d2d9cb47869012087cb834b4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003722"
---
# <a name="configure-chargeable-components-of-a-project-based-contract-line"></a><span data-ttu-id="1bf5b-103">‏‫קביעת תצורה של רכיבים ניתנים לחיוב בסעיף חוזה מבוסס פרוייקט‬</span><span class="sxs-lookup"><span data-stu-id="1bf5b-103">Configure chargeable components of a project-based contract line</span></span>

<span data-ttu-id="1bf5b-104">_**חל על:** פריסה קלה - עסקה עם חשבונית פרופורמה, Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="1bf5b-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="1bf5b-105">בסעיף חוזה מבוסס פרויקט יש רכיבים *כלולים* ורכיבים *הניתנים לחיוב*.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-105">A project-based contract line has *included* components and *chargeable* components.</span></span>

<span data-ttu-id="1bf5b-106">רכיבים כלולים הם רכיבים הכפופים ל:</span><span class="sxs-lookup"><span data-stu-id="1bf5b-106">Included components are components that are subject to:</span></span>

  - <span data-ttu-id="1bf5b-107">שיטת חיוב ופיצולי לקוחות</span><span class="sxs-lookup"><span data-stu-id="1bf5b-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="1bf5b-108">מגבלות 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="1bf5b-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="1bf5b-109">הגדרות תדירות חשבוניות שהוגדרה בסעיף החוזה מבוסס הפרויקט</span><span class="sxs-lookup"><span data-stu-id="1bf5b-109">Invoice frequency settings defined on the project-based contract line</span></span>

<span data-ttu-id="1bf5b-110">ניתן לסמן תת קבוצה של הרכיבים הכלולים כניתנים לחיוב באמצעות השדה **סוג חיוב**.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="1bf5b-111">השדה **סוג חיוב** הוא קבוצת אפשרויות המאפשרת את הערכים הבאים בהקשר של סעיף חוזה:</span><span class="sxs-lookup"><span data-stu-id="1bf5b-111">The **Billing Type** field is an option-set that allows the following values in the context of a contract line:</span></span>

  - <span data-ttu-id="1bf5b-112">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-112">Chargeable</span></span>
  - <span data-ttu-id="1bf5b-113">לא ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-113">Non-chargeable</span></span>

<span data-ttu-id="1bf5b-114">ניתן להגדיר רכיבים הניתנים לחיוב במשימות, בתפקידים ובקטגוריות של עסקאות.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="1bf5b-115">יכולת חיוב מוגדרת במשימות עבור סעיף חוזה פרויקט וחל על כל סיווגי העסקאות הכלולות בסעיף.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-115">Chargeability is defined on tasks for a project contract line and applies to all transaction classes included on the line.</span></span> <span data-ttu-id="1bf5b-116">אם השדה **כלול משימות** בסעיף החוזה ריק או מוגדר **כפרויקט כולו**, הכרטיסיה **משימות ניתנות לחיוב** לא תהיה זמינה.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-116">If the **Include Tasks** field on a contract line is blank or set to **Entire project**, the **Chargeable tasks** tab will not be available.</span></span>

<span data-ttu-id="1bf5b-117">יכולת חיוב המוגדרת בתפקידים עבור סעיף חוזה פרויקט חלה רק על סיווג העסקאות **זמן**.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-117">Chargeability defined on roles for a project contract line only applies to the **Time** transaction class.</span></span> <span data-ttu-id="1bf5b-118">אם השדה **כלול משימות** בסעיף החוזה ריק או מוגדר **לא**, הכרטיסיה **תפקידים ניתנים לחיוב** לא תהיה זמינה.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-118">If the **Include Time** field on a contract line is set to **No**, the **Chargeable roles** tab will not be available.</span></span>

<span data-ttu-id="1bf5b-119">יכולת חיוב המוגדרת בקטגוריות של עסקאות עבור סעיף חוזה פרויקט חלה רק על סיווג העסקאות **הוצאה**.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-119">Chargeability defined on transaction categories for a project contract line only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="1bf5b-120">אם השדה **לכלול הוצאות** מוגדר כ **לא**, הכרטיסיה **קטגוריות הניתנות לחיוב** לא תהיה זמינה.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-120">If the **Include Expenses** field is set to **No**, the **Chargeable Categories** tab will not be available.</span></span>

### <a name="update-a-project-task-as-chargeable-or-non-chargeable"></a><span data-ttu-id="1bf5b-121">עדכן משימת פרויקט כניתנת לחיוב או כלא ניתנת לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-121">Update a project task as chargeable or non-chargeable</span></span>

<span data-ttu-id="1bf5b-122">משימת פרויקט יכולה להיות ניתנת לחיוב או לא ניתנת לחיוב בסעיף חוזה ספציפי, דבר המאפשר את הגדרה הבאה:</span><span class="sxs-lookup"><span data-stu-id="1bf5b-122">A project task can be chargeable or non-chargeable on a specific contract line, which makes the following setup possible:</span></span>

<span data-ttu-id="1bf5b-123">אם סעיף חוזה מבוסס פרויקט כולל **זמן** ומשימה מסוימת, **T1** משוייכת אליו כניתנת לתשלום.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-123">If a project-based contract line includes **Time** and a certain task, **T1** is associated to it as chargeable.</span></span> <span data-ttu-id="1bf5b-124">אם יש סעיף חוזה שני שכולל **הוצאה**, ניתן לשייך את המשימת T1 בסעיף החוזה כלא ניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-124">If there is a second contract line that includes **Expense**, you can associate the T1 task on the contract line as non-chargeable.</span></span> <span data-ttu-id="1bf5b-125">התוצאה היא שכל הזמן שנרשם במשימה ניתן לחיוב וכל ההוצאות אינן ניתנות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-125">The result is that all of the time recorded on the task is chargeable and all expenses are non-chargeable.</span></span>

<span data-ttu-id="1bf5b-126">ניתן להגדיר את סוג החיוב של משימה בכרטיסיה **משימות הניתנות לחיוב** של סעיף החוזה על ידי עדכון השדה **סוג החיוב** ברשת המשנה של משימות סעיף החוזה.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-126">A task's billing type can be configured on the **Chargeable Tasks** tab of the contract line by updating the **Billing Type** field on the contract line tasks subgrid.</span></span> <span data-ttu-id="1bf5b-127">לחלופין, ניתן לעדכן את השדה **סוג חיוב** ברשת המשנה של הגדרת חיוב משימה של פרויקט המציג את סעיפי החוזה המשויכים למשימה.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-127">Alternatively, you can update the **Billing Type** field on the subgrid of the task Billing setup of a project that shows the contract lines associated to a task.</span></span>

### <a name="update-a-role-as-chargeable-or-non-chargeable"></a><span data-ttu-id="1bf5b-128">עדכן תפקיד כניתן לחיוב או כלא ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-128">Update a role as chargeable or non-chargeable</span></span>

<span data-ttu-id="1bf5b-129">תפקיד יכול להיות ניתן לחיוב או לא ניתן לחייב בסעיף חוזה ספציפי.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-129">A role can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="1bf5b-130">ניתן להגדיר את סוג החיוב של תפקיד בכרטיסיה **תפקידים הניתנים לחיוב** של סעיף חוזה.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-130">A role's billing type can be configured on the **Chargeable Roles** tab of a contract line.</span></span> <span data-ttu-id="1bf5b-131">לשם כך, עדכן את השדה **סוג חיוב** ברשת המשנה **תפקידים הניתנים לחיוב**.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-131">To do this, update the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-as-chargeable-or-non-chargeable"></a><span data-ttu-id="1bf5b-132">עדכן קטגוריה של עסקאות כניתנת לחיוב או כלא ניתנת לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-132">Update a transaction category as chargeable or non-chargeable</span></span>

<span data-ttu-id="1bf5b-133">קטגוריה של עסקאות יכולה להיות ניתנת לחיוב או לא ניתנת לחייב בסעיף חוזה ספציפי.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-133">A transaction category can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="1bf5b-134">ניתן להגדיר את סוג החיוב של עסקה בכרטיסיה **קטגוריות הניתנות לחיוב** של סעיף חוזה מבוסס פרויקט.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-134">A transaction's billing type can be configured on the **Chargeable Categories** tab of a project-based contract line.</span></span> <span data-ttu-id="1bf5b-135">לשם כך, עדכן את השדה **סוג חיוב** ברשת המשנה **קטגוריות הניתנות לחיוב**.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-135">To do this, update the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="1bf5b-136">פתרון של יכולת חיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-136">Resolve chargeability</span></span>

<span data-ttu-id="1bf5b-137">הערכה או נתונים בפועל שנוצרו עבור זמן נחשבים כניתנים לחיוב רק אם:</span><span class="sxs-lookup"><span data-stu-id="1bf5b-137">An estimate or actual created for time is only considered chargeable if:</span></span>

   - <span data-ttu-id="1bf5b-138">**זמן** כלול בסעיף חוזה.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-138">**Time** is included on the contract line.</span></span>
   - <span data-ttu-id="1bf5b-139">**תפקיד** מוגדר כניתן לחיוב בסעיף חוזה.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-139">**Role** is configured as chargeable on the contract line.</span></span>
   - <span data-ttu-id="1bf5b-140">**משימות כלולות** מוגדרות בתור **משימות נבחרות** בסעיף חוזה.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-140">**Included Tasks** is set to **Selected tasks** on the contract line.</span></span>
 
 <span data-ttu-id="1bf5b-141">אם שלושת הדברים הללו נכונים, המשימה מוגדרת כניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-141">If these three things are true, the task is configured as chargeable.</span></span> 

<span data-ttu-id="1bf5b-142">הערכה או נתונים בפועל שנוצרו עבור הוצאה נחשבים כניתנים לחיוב רק אם:</span><span class="sxs-lookup"><span data-stu-id="1bf5b-142">An estimate or actual created for expense is only considered chargeable if:</span></span>

   - <span data-ttu-id="1bf5b-143">**הוצאה** כלולה בסעיף חוזה</span><span class="sxs-lookup"><span data-stu-id="1bf5b-143">**Expense** is included on the contract line</span></span>
   - <span data-ttu-id="1bf5b-144">**קטגוריית עסקה** מוגדרת כניתנת לחיוב בסעיף חוזה</span><span class="sxs-lookup"><span data-stu-id="1bf5b-144">**Transaction category** is configured as chargeable on the contract line</span></span>
   - <span data-ttu-id="1bf5b-145">**משימות כלולות** מוגדרות בתור **משימות נבחרות** בסעיף חוזה</span><span class="sxs-lookup"><span data-stu-id="1bf5b-145">**Included Tasks** is set to **Selected task** on the contract line</span></span>
  
 <span data-ttu-id="1bf5b-146">אם שלושת הדברים הללו נכונים **המשימה** מוגדרת כניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-146">If these three things are true, the **Task** is configured as chargeable.</span></span> 

<span data-ttu-id="1bf5b-147">הערכה או נתונים בפועל שנוצרו עבור חומר נחשבים כניתנים לחיוב רק אם:</span><span class="sxs-lookup"><span data-stu-id="1bf5b-147">An estimate or actual created for material is only considered chargeable if:</span></span>

   - <span data-ttu-id="1bf5b-148">**חומרים** כלולים בסעיף חוזה</span><span class="sxs-lookup"><span data-stu-id="1bf5b-148">**Materials** is included on the contract line</span></span>
   - <span data-ttu-id="1bf5b-149">**משימות כלולות** מוגדרות בתור **משימות נבחרות** בסעיף חוזה</span><span class="sxs-lookup"><span data-stu-id="1bf5b-149">**Included Tasks** is set to **Selected tasks** on the contract line</span></span>

<span data-ttu-id="1bf5b-150">אם שני הדברים הללו נכונים **המשימה** מוגדרת כניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="1bf5b-150">If these two things are true, the **Task** is configured as chargeable.</span></span> 

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="1bf5b-151">
                    <strong>כולל זמן</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-151">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="1bf5b-152">
                    <strong>כולל הוצאה</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-152">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="1bf5b-153">
                    <strong>כולל חומרים</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-153">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="1bf5b-154">
                    <strong>משימות כלולות</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-154">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bf5b-155">
                    <strong>תפקיד</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-155">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="1bf5b-156">
                    <strong>קטגוריה</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-156">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bf5b-157">
                    <strong>משימה</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-157">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="1bf5b-158">
                    <strong>השפעת יכולת החיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-158">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-159">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-159">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bf5b-160">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-160">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bf5b-161">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-161">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bf5b-162">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="1bf5b-162">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-163">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-163">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-164">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-164">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-165">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="1bf5b-165">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bf5b-166">חיוב לפי נתוני זמן בפועל: <strong>ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-166">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-167">סוג חיוב עבור נתוני הוצאה בפועל: <strong>ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-167">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-168">סוג חיוב עבור נתוני חומר בפועל: <strong>ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-168">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-169">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-169">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bf5b-170">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-170">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bf5b-171">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-171">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bf5b-172">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="1bf5b-172">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-173">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-173">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-174">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-174">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-175">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-175">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bf5b-176">חיוב לפי נתוני זמן בפועל: <strong>ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-176">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-177">סוג חיוב עבור נתוני הוצאה בפועל: <strong>ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-177">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-178">סוג חיוב עבור נתוני חומר בפועל: <strong>ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-178">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-179">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-179">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bf5b-180">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-180">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bf5b-181">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-181">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bf5b-182">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="1bf5b-182">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bf5b-183">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-183">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-184">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-184">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-185">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-185">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bf5b-186">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-186">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-187">סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-187">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="1bf5b-188">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-188">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-189">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-189">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bf5b-190">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-190">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bf5b-191">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-191">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bf5b-192">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="1bf5b-192">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-193">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-193">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-194">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-194">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bf5b-195">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-195">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bf5b-196">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-196">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-197">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-197">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-198">סוג חיוב עבור נתוני חומר בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-198">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-199">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-199">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bf5b-200">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-200">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bf5b-201">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-201">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bf5b-202">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="1bf5b-202">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bf5b-203">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-203">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-204">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-204">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bf5b-205">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-205">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bf5b-206">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-206">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-207">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-207">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-208">סוג חיוב עבור נתוני חומר בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-208">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-209">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-209">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bf5b-210">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-210">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bf5b-211">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-211">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bf5b-212">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="1bf5b-212">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bf5b-213">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-213">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="1bf5b-214">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-214">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-215">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-215">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bf5b-216">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-216">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-217">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-217">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-218">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-218">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="1bf5b-219">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-219">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bf5b-220">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-220">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bf5b-221">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-221">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bf5b-222">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="1bf5b-222">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-223">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="1bf5b-223">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="1bf5b-224">
                    <strong>ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-224">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-225">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="1bf5b-225">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bf5b-226">חיוב לפי נתוני זמן בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-226">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-227">סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-227">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="1bf5b-228">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-228">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="1bf5b-229">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-229">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bf5b-230">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-230">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bf5b-231">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-231">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bf5b-232">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="1bf5b-232">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-233">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="1bf5b-233">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="1bf5b-234">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-234">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-235">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="1bf5b-235">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bf5b-236">חיוב לפי נתוני זמן בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-236">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-237">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-237">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-238">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-238">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-239">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-239">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="1bf5b-240">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-240">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bf5b-241">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-241">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bf5b-242">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="1bf5b-242">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-243">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-243">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-244">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="1bf5b-244">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-245">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="1bf5b-245">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bf5b-246">חיוב לפי נתוני זמן בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-246">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="1bf5b-247">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-247">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-248">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-248">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-249">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-249">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="1bf5b-250">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-250">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="1bf5b-251">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-251">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bf5b-252">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="1bf5b-252">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bf5b-253">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-253">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-254">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="1bf5b-254">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-255">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="1bf5b-255">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bf5b-256">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-256">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-257">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-257">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-258">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-258">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-259">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-259">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bf5b-260">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-260">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="1bf5b-261">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-261">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bf5b-262">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="1bf5b-262">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-263">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-263">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-264">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-264">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-265">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="1bf5b-265">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bf5b-266">חיוב לפי נתוני זמן בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-266">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="1bf5b-267">סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="1bf5b-267">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="1bf5b-268">סוג חיוב עבור נתוני חומר בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-268">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="1bf5b-269">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-269">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="1bf5b-270">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="1bf5b-270">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="1bf5b-271">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-271">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="1bf5b-272">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="1bf5b-272">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="1bf5b-273">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-273">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="1bf5b-274">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-274">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="1bf5b-275">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="1bf5b-275">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="1bf5b-276">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-276">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-277">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-277">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="1bf5b-278">סוג חיוב עבור נתוני חומר בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="1bf5b-278">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>





[!INCLUDE[footer-include](../../includes/footer-banner.md)]
