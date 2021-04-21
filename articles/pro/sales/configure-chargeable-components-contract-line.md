---
title: ‏‫קביעת תצורה של רכיבים ניתנים לחיוב בסעיף חוזה מבוסס פרוייקט‬
description: נושא זה מספק מידע על אופן הוספת רכיבים הניתנים לחיוב לסעיפי חוזה ב-Project Operations.
author: rumant
manager: Annbe
ms.date: 10/08/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ddada2cb412ba7370fb0a750325a84772937d8d0
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858474"
---
# <a name="configure-chargeable-components-of-a-project-based-contract-line"></a><span data-ttu-id="d81b8-103">‏‫קביעת תצורה של רכיבים ניתנים לחיוב בסעיף חוזה מבוסס פרוייקט‬</span><span class="sxs-lookup"><span data-stu-id="d81b8-103">Configure chargeable components of a project-based contract line</span></span>

<span data-ttu-id="d81b8-104">_**חל על:** פריסה קלה - עסקה עם חשבונית פרופורמה, Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="d81b8-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="d81b8-105">בסעיף חוזה מבוסס פרויקט יש רכיבים *כלולים* ורכיבים *הניתנים לחיוב*.</span><span class="sxs-lookup"><span data-stu-id="d81b8-105">A project-based contract line has *included* components and *chargeable* components.</span></span>

<span data-ttu-id="d81b8-106">רכיבים כלולים הם רכיבים הכפופים ל:</span><span class="sxs-lookup"><span data-stu-id="d81b8-106">Included components are components that are subject to:</span></span>

  - <span data-ttu-id="d81b8-107">שיטת חיוב ופיצולי לקוחות</span><span class="sxs-lookup"><span data-stu-id="d81b8-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="d81b8-108">מגבלות 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="d81b8-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="d81b8-109">הגדרות תדירות חשבוניות שהוגדרה בסעיף החוזה מבוסס הפרויקט</span><span class="sxs-lookup"><span data-stu-id="d81b8-109">Invoice frequency settings defined on the project-based contract line</span></span>

<span data-ttu-id="d81b8-110">ניתן לסמן תת קבוצה של הרכיבים הכלולים כניתנים לחיוב באמצעות השדה **סוג חיוב**.</span><span class="sxs-lookup"><span data-stu-id="d81b8-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="d81b8-111">השדה **סוג חיוב** הוא קבוצת אפשרויות המאפשרת את הערכים הבאים בהקשר של סעיף חוזה:</span><span class="sxs-lookup"><span data-stu-id="d81b8-111">The **Billing Type** field is an option-set that allows the following values in the context of a contract line:</span></span>

  - <span data-ttu-id="d81b8-112">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-112">Chargeable</span></span>
  - <span data-ttu-id="d81b8-113">לא ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-113">Non-chargeable</span></span>

<span data-ttu-id="d81b8-114">ניתן להגדיר רכיבים הניתנים לחיוב במשימות, בתפקידים ובקטגוריות של עסקאות.</span><span class="sxs-lookup"><span data-stu-id="d81b8-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="d81b8-115">יכולת חיוב מוגדרת במשימות עבור סעיף חוזה פרויקט וחל על כל סיווגי העסקאות הכלולות בסעיף.</span><span class="sxs-lookup"><span data-stu-id="d81b8-115">Chargeability is defined on tasks for a project contract line and applies to all transaction classes included on the line.</span></span> <span data-ttu-id="d81b8-116">אם השדה **כלול משימות** בסעיף החוזה ריק או מוגדר **כפרויקט כולו**, הכרטיסיה **משימות ניתנות לחיוב** לא תהיה זמינה.</span><span class="sxs-lookup"><span data-stu-id="d81b8-116">If the **Include Tasks** field on a contract line is blank or set to **Entire project**, the **Chargeable tasks** tab will not be available.</span></span>

<span data-ttu-id="d81b8-117">יכולת חיוב המוגדרת בתפקידים עבור סעיף חוזה פרויקט חלה רק על סיווג העסקאות **זמן**.</span><span class="sxs-lookup"><span data-stu-id="d81b8-117">Chargeability defined on roles for a project contract line only applies to the **Time** transaction class.</span></span> <span data-ttu-id="d81b8-118">אם השדה **כלול משימות** בסעיף החוזה ריק או מוגדר **לא**, הכרטיסיה **תפקידים ניתנים לחיוב** לא תהיה זמינה.</span><span class="sxs-lookup"><span data-stu-id="d81b8-118">If the **Include Time** field on a contract line is set to **No**, the **Chargeable roles** tab will not be available.</span></span>

<span data-ttu-id="d81b8-119">יכולת חיוב המוגדרת בקטגוריות של עסקאות עבור סעיף חוזה פרויקט חלה רק על סיווג העסקאות **הוצאה**.</span><span class="sxs-lookup"><span data-stu-id="d81b8-119">Chargeability defined on transaction categories for a project contract line only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="d81b8-120">אם השדה **לכלול הוצאות** מוגדר כ **לא**, הכרטיסיה **קטגוריות הניתנות לחיוב** לא תהיה זמינה.</span><span class="sxs-lookup"><span data-stu-id="d81b8-120">If the **Include Expenses** field is set to **No**, the **Chargeable Categories** tab will not be available.</span></span>

### <a name="update-a-project-task-as-chargeable-or-non-chargeable"></a><span data-ttu-id="d81b8-121">עדכן משימת פרויקט כניתנת לחיוב או כלא ניתנת לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-121">Update a project task as chargeable or non-chargeable</span></span>

<span data-ttu-id="d81b8-122">משימת פרויקט יכולה להיות ניתנת לחיוב או לא ניתנת לחיוב בסעיף חוזה ספציפי, דבר המאפשר את הגדרה הבאה:</span><span class="sxs-lookup"><span data-stu-id="d81b8-122">A project task can be chargeable or non-chargeable on a specific contract line, which makes the following setup possible:</span></span>

<span data-ttu-id="d81b8-123">אם סעיף חוזה מבוסס פרויקט כולל **זמן** ומשימה מסוימת, **T1** משוייכת אליו כניתנת לתשלום.</span><span class="sxs-lookup"><span data-stu-id="d81b8-123">If a project-based contract line includes **Time** and a certain task, **T1** is associated to it as chargeable.</span></span> <span data-ttu-id="d81b8-124">אם יש סעיף חוזה שני שכולל **הוצאה**, ניתן לשייך את המשימת T1 בסעיף החוזה כלא ניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="d81b8-124">If there is a second contract line that includes **Expense**, you can associate the T1 task on the contract line as non-chargeable.</span></span> <span data-ttu-id="d81b8-125">התוצאה היא שכל הזמן שנרשם במשימה ניתן לחיוב וכל ההוצאות אינן ניתנות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="d81b8-125">The result is that all of the time recorded on the task is chargeable and all expenses are non-chargeable.</span></span>

<span data-ttu-id="d81b8-126">ניתן להגדיר את סוג החיוב של משימה בכרטיסיה **משימות הניתנות לחיוב** של סעיף החוזה על ידי עדכון השדה **סוג החיוב** ברשת המשנה של משימות סעיף החוזה.</span><span class="sxs-lookup"><span data-stu-id="d81b8-126">A task's billing type can be configured on the **Chargeable Tasks** tab of the contract line by updating the **Billing Type** field on the contract line tasks subgrid.</span></span> <span data-ttu-id="d81b8-127">לחלופין, ניתן לעדכן את השדה **סוג חיוב** ברשת המשנה של הגדרת חיוב משימה של פרויקט המציג את סעיפי החוזה המשויכים למשימה.</span><span class="sxs-lookup"><span data-stu-id="d81b8-127">Alternatively, you can update the **Billing Type** field on the subgrid of the task Billing setup of a project that shows the contract lines associated to a task.</span></span>

### <a name="update-a-role-as-chargeable-or-non-chargeable"></a><span data-ttu-id="d81b8-128">עדכן תפקיד כניתן לחיוב או כלא ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-128">Update a role as chargeable or non-chargeable</span></span>

<span data-ttu-id="d81b8-129">תפקיד יכול להיות ניתן לחיוב או לא ניתן לחייב בסעיף חוזה ספציפי.</span><span class="sxs-lookup"><span data-stu-id="d81b8-129">A role can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="d81b8-130">ניתן להגדיר את סוג החיוב של תפקיד בכרטיסיה **תפקידים הניתנים לחיוב** של סעיף חוזה.</span><span class="sxs-lookup"><span data-stu-id="d81b8-130">A role's billing type can be configured on the **Chargeable Roles** tab of a contract line.</span></span> <span data-ttu-id="d81b8-131">לשם כך, עדכן את השדה **סוג חיוב** ברשת המשנה **תפקידים הניתנים לחיוב**.</span><span class="sxs-lookup"><span data-stu-id="d81b8-131">To do this, update the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-as-chargeable-or-non-chargeable"></a><span data-ttu-id="d81b8-132">עדכן קטגוריה של עסקאות כניתנת לחיוב או כלא ניתנת לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-132">Update a transaction category as chargeable or non-chargeable</span></span>

<span data-ttu-id="d81b8-133">קטגוריה של עסקאות יכולה להיות ניתנת לחיוב או לא ניתנת לחייב בסעיף חוזה ספציפי.</span><span class="sxs-lookup"><span data-stu-id="d81b8-133">A transaction category can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="d81b8-134">ניתן להגדיר את סוג החיוב של עסקה בכרטיסיה **קטגוריות הניתנות לחיוב** של סעיף חוזה מבוסס פרויקט.</span><span class="sxs-lookup"><span data-stu-id="d81b8-134">A transaction's billing type can be configured on the **Chargeable Categories** tab of a project-based contract line.</span></span> <span data-ttu-id="d81b8-135">לשם כך, עדכן את השדה **סוג חיוב** ברשת המשנה **קטגוריות הניתנות לחיוב**.</span><span class="sxs-lookup"><span data-stu-id="d81b8-135">To do this, update the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="d81b8-136">פתרון של יכולת חיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-136">Resolve chargeability</span></span>

<span data-ttu-id="d81b8-137">הערכה או נתונים בפועל שנוצרו עבור זמן נחשבים כניתנים לחיוב רק אם:</span><span class="sxs-lookup"><span data-stu-id="d81b8-137">An estimate or actual created for time is only considered chargeable if:</span></span>

   - <span data-ttu-id="d81b8-138">**זמן** כלול בסעיף חוזה.</span><span class="sxs-lookup"><span data-stu-id="d81b8-138">**Time** is included on the contract line.</span></span>
   - <span data-ttu-id="d81b8-139">**תפקיד** מוגדר כניתן לחיוב בסעיף חוזה.</span><span class="sxs-lookup"><span data-stu-id="d81b8-139">**Role** is configured as chargeable on the contract line.</span></span>
   - <span data-ttu-id="d81b8-140">**משימות כלולות** מוגדרות בתור **משימות נבחרות** בסעיף חוזה.</span><span class="sxs-lookup"><span data-stu-id="d81b8-140">**Included Tasks** is set to **Selected tasks** on the contract line.</span></span>
 
 <span data-ttu-id="d81b8-141">אם שלושת הדברים הללו נכונים, המשימה מוגדרת כניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="d81b8-141">If these three things are true, the task is configured as chargeable.</span></span> 

<span data-ttu-id="d81b8-142">הערכה או נתונים בפועל שנוצרו עבור הוצאה נחשבים כניתנים לחיוב רק אם:</span><span class="sxs-lookup"><span data-stu-id="d81b8-142">An estimate or actual created for expense is only considered chargeable if:</span></span>

   - <span data-ttu-id="d81b8-143">**הוצאה** כלולה בסעיף חוזה</span><span class="sxs-lookup"><span data-stu-id="d81b8-143">**Expense** is included on the contract line</span></span>
   - <span data-ttu-id="d81b8-144">**קטגוריית עסקה** מוגדרת כניתנת לחיוב בסעיף חוזה</span><span class="sxs-lookup"><span data-stu-id="d81b8-144">**Transaction category** is configured as chargeable on the contract line</span></span>
   - <span data-ttu-id="d81b8-145">**משימות כלולות** מוגדרות בתור **משימות נבחרות** בסעיף חוזה</span><span class="sxs-lookup"><span data-stu-id="d81b8-145">**Included Tasks** is set to **Selected task** on the contract line</span></span>
  
 <span data-ttu-id="d81b8-146">אם שלושת הדברים הללו נכונים **המשימה** מוגדרת כניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="d81b8-146">If these three things are true, the **Task** is configured as chargeable.</span></span> 

<span data-ttu-id="d81b8-147">הערכה או נתונים בפועל שנוצרו עבור חומר נחשבים כניתנים לחיוב רק אם:</span><span class="sxs-lookup"><span data-stu-id="d81b8-147">An estimate or actual created for material is only considered chargeable if:</span></span>

   - <span data-ttu-id="d81b8-148">**חומרים** כלולים בסעיף חוזה</span><span class="sxs-lookup"><span data-stu-id="d81b8-148">**Materials** is included on the contract line</span></span>
   - <span data-ttu-id="d81b8-149">**משימות כלולות** מוגדרות בתור **משימות נבחרות** בסעיף חוזה</span><span class="sxs-lookup"><span data-stu-id="d81b8-149">**Included Tasks** is set to **Selected tasks** on the contract line</span></span>

<span data-ttu-id="d81b8-150">אם שני הדברים הללו נכונים **המשימה** מוגדרת כניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="d81b8-150">If these two things are true, the **Task** is configured as chargeable.</span></span> 

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="d81b8-151">
                    <strong>כולל זמן</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-151">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="d81b8-152">
                    <strong>כולל הוצאה</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-152">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="d81b8-153">
                    <strong>כולל חומרים</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-153">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="d81b8-154">
                    <strong>משימות כלולות</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-154">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d81b8-155">
                    <strong>תפקיד</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-155">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="d81b8-156">
                    <strong>קטגוריה</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-156">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d81b8-157">
                    <strong>משימה</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-157">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="d81b8-158">
                    <strong>השפעת יכולת החיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-158">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-159">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-159">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d81b8-160">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-160">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d81b8-161">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-161">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d81b8-162">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="d81b8-162">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-163">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-163">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-164">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-164">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-165">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="d81b8-165">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d81b8-166">חיוב לפי נתוני זמן בפועל: <strong>ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-166">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-167">סוג חיוב עבור נתוני הוצאה בפועל: <strong>ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-167">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-168">סוג חיוב עבור נתוני חומר בפועל: <strong>ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-168">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-169">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-169">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d81b8-170">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-170">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d81b8-171">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-171">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d81b8-172">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="d81b8-172">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-173">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-173">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-174">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-174">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-175">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-175">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d81b8-176">חיוב לפי נתוני זמן בפועל: <strong>ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-176">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-177">סוג חיוב עבור נתוני הוצאה בפועל: <strong>ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-177">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-178">סוג חיוב עבור נתוני חומר בפועל: <strong>ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-178">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-179">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-179">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d81b8-180">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-180">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d81b8-181">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-181">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d81b8-182">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="d81b8-182">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d81b8-183">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-183">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-184">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-184">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-185">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-185">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d81b8-186">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-186">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-187">סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-187">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="d81b8-188">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-188">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-189">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-189">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d81b8-190">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-190">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d81b8-191">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-191">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d81b8-192">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="d81b8-192">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-193">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-193">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-194">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-194">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d81b8-195">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-195">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d81b8-196">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-196">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-197">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-197">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-198">סוג חיוב עבור נתוני חומר בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-198">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-199">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-199">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d81b8-200">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-200">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d81b8-201">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-201">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d81b8-202">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="d81b8-202">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d81b8-203">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-203">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-204">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-204">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d81b8-205">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-205">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d81b8-206">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-206">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-207">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-207">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-208">סוג חיוב עבור נתוני חומר בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-208">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-209">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-209">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d81b8-210">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-210">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d81b8-211">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-211">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d81b8-212">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="d81b8-212">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d81b8-213">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-213">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="d81b8-214">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-214">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-215">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-215">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d81b8-216">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-216">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-217">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-217">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-218">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-218">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="d81b8-219">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-219">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d81b8-220">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-220">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d81b8-221">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-221">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d81b8-222">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="d81b8-222">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-223">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="d81b8-223">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="d81b8-224">
                    <strong>ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-224">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-225">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="d81b8-225">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d81b8-226">חיוב לפי נתוני זמן בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-226">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-227">סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-227">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="d81b8-228">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-228">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="d81b8-229">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-229">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d81b8-230">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-230">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d81b8-231">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-231">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d81b8-232">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="d81b8-232">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-233">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="d81b8-233">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="d81b8-234">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-234">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-235">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="d81b8-235">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d81b8-236">חיוב לפי נתוני זמן בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-236">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-237">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-237">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-238">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-238">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-239">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-239">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="d81b8-240">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-240">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d81b8-241">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-241">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d81b8-242">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="d81b8-242">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-243">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-243">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-244">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="d81b8-244">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-245">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="d81b8-245">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d81b8-246">חיוב לפי נתוני זמן בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-246">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="d81b8-247">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-247">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-248">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-248">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-249">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-249">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="d81b8-250">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-250">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="d81b8-251">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-251">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d81b8-252">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="d81b8-252">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d81b8-253">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-253">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-254">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="d81b8-254">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-255">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="d81b8-255">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d81b8-256">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-256">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-257">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-257">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-258">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-258">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-259">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-259">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d81b8-260">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-260">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="d81b8-261">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-261">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d81b8-262">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="d81b8-262">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-263">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-263">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-264">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-264">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-265">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="d81b8-265">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d81b8-266">חיוב לפי נתוני זמן בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-266">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="d81b8-267">סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="d81b8-267">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="d81b8-268">סוג חיוב עבור נתוני חומר בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-268">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="d81b8-269">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-269">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="d81b8-270">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d81b8-270">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="d81b8-271">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-271">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="d81b8-272">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="d81b8-272">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="d81b8-273">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-273">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="d81b8-274">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-274">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="d81b8-275">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="d81b8-275">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="d81b8-276">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-276">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-277">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-277">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="d81b8-278">סוג חיוב עבור נתוני חומר בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d81b8-278">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>





[!INCLUDE[footer-include](../../includes/footer-banner.md)]
