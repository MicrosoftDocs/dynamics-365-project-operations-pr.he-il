---
title: הגדרת המרכיבים הניתנים לחיוב של שורת הצעת מחיר
description: נושא זה מספק מידע אודות הגדרת רכיבים הניתנים לחיוב ורכיבים שאינם ניתנים לחיוב בשורת הצעת מחיר מבוססת פרויקט.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 1a9e1851bd8c5a4070df2774c945d1f3eabaaa8a
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858294"
---
# <a name="configure-the-chargeable-components-of-a-quote-line"></a><span data-ttu-id="cc019-103">קביעת תצורה של הרכיבים הניתנים לחיוב של שורת הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="cc019-103">Configure the chargeable components of a quote line</span></span> 

<span data-ttu-id="cc019-104">_**חל על:** פריסה קלה - עסקה עם חשבונית פרופורמה, Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="cc019-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="cc019-105">בסעיף חוזה מבוסס פרויקט יש מושג של רכיבים *כלולים* ורכיבים *הניתנים לחיוב*.</span><span class="sxs-lookup"><span data-stu-id="cc019-105">A project-based quote line has the concept of *included* components and *chargeable* components.</span></span>

<span data-ttu-id="cc019-106">הרכיבים הכלולים כפופים ל:</span><span class="sxs-lookup"><span data-stu-id="cc019-106">Included components are subject to:</span></span>

  - <span data-ttu-id="cc019-107">שיטת חיוב ופיצולי לקוחות</span><span class="sxs-lookup"><span data-stu-id="cc019-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="cc019-108">מגבלות 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="cc019-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="cc019-109">הגדרות תדירות חשבוניות שהוגדרה בשורת הצעת המחיר מבוססת פרויקט</span><span class="sxs-lookup"><span data-stu-id="cc019-109">Invoice frequency settings defined on the project-based quote line</span></span>

<span data-ttu-id="cc019-110">ניתן לסמן תת קבוצה של הרכיבים הכלולים כניתנים לחיוב באמצעות השדה **סוג חיוב**.</span><span class="sxs-lookup"><span data-stu-id="cc019-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="cc019-111">השדה **סוג החיוב** הוא קבוצת אפשרויות המאפשרת את הערכים הבאים בהקשר של שורת הצעת מחיר:</span><span class="sxs-lookup"><span data-stu-id="cc019-111">The **Billing Type** field is an option-set that allows the following values in the context of a quote line:</span></span>

  - <span data-ttu-id="cc019-112">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-112">Chargeable</span></span>
  - <span data-ttu-id="cc019-113">לא ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-113">Non-chargeable</span></span>

<span data-ttu-id="cc019-114">ניתן להגדיר רכיבים הניתנים לחיוב במשימות, בתפקידים ובקטגוריות של עסקאות.</span><span class="sxs-lookup"><span data-stu-id="cc019-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="cc019-115">יכולת חיוב מוגדרת במשימות עבור שורת הצעת מחיר וחלה על כל סיווגי העסקאות הכלולות באותה שורה.</span><span class="sxs-lookup"><span data-stu-id="cc019-115">Chargeability is defined on the tasks for a quote line and applies to all transaction classes included on that line.</span></span> <span data-ttu-id="cc019-116">אם השדה **כלול משימות** מוגדר **כפרויקט כולו**, או נותר ריק, הכרטיסיה **משימות ניתנות לחיוב** לא תהיה זמינה.</span><span class="sxs-lookup"><span data-stu-id="cc019-116">If the **Include Tasks** field is set to **Entire project** or left blank, the **Chargeable Tasks** tab isn't available.</span></span>

<span data-ttu-id="cc019-117">יכולת חיוב המוגדרת בתפקידים עבור שורת הצעת מחיר וחלה רק על סיווג העסקאות **זמן**.</span><span class="sxs-lookup"><span data-stu-id="cc019-117">Chargeability is defined on roles for a quote line and only applies to the **Time** transaction class.</span></span> <span data-ttu-id="cc019-118">אם השדה **כלול משימות** מוגדר כ **לא** בשורת הצעת מחיר של פרויקט, הכרטיסיה **תפקידים ניתנים לחיוב** לא תהיה זמינה.</span><span class="sxs-lookup"><span data-stu-id="cc019-118">If the field, **Include Time** is set to **No** on a project quote line, the **Chargeable Roles** tab isn't available.</span></span>

<span data-ttu-id="cc019-119">יכולת חיוב המוגדרת בקטגוריות של עסקאות עבור שורת הצעת מחיר וחלה רק על סיווג העסקאות **הוצאה**.</span><span class="sxs-lookup"><span data-stu-id="cc019-119">Chargeability is defined on transaction categories for a  quote line and only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="cc019-120">אם השדה **כלול הוצאות** מוגדר כ **לא** בשורת הצעת מחיר של פרויקט, הכרטיסיה **קטגוריות הניתנות לחיוב** לא תהיה זמינה.</span><span class="sxs-lookup"><span data-stu-id="cc019-120">If the field, **Include Expenses** is set to **No** on a project quote line, the **Chargeable Categories** tab isn't available.</span></span>

### <a name="update-a-project-task-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="cc019-121">עדכן משימת פרויקט כניתנת לחיוב או כלא ניתנת לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-121">Update a project task to be chargeable or non-chargeable</span></span>

<span data-ttu-id="cc019-122">משימת פרויקט יכולה להיות ניתנת לחיוב או לא ניתנת לחיוב בהקשר של שורת הצעת מחיר מבוססת פרויקט ספציפית, דבר המאפשר את הגדרה הבאה.</span><span class="sxs-lookup"><span data-stu-id="cc019-122">A project task can be chargeable or non-chargeable in the context of a specific project-based quote line, which makes the following setup possible.</span></span>

<span data-ttu-id="cc019-123">אם שורת הצעת מחיר מבוססת פרויקט כוללת **זמן** והמשימה **T1**, המשימה משויכת לשורת הצעת המחיר כניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="cc019-123">If a project-based quote line includes **Time** and the task **T1**, the task is associated to the quote line as chargeable.</span></span> <span data-ttu-id="cc019-124">אם יש שורת הצעת מחיר שניה שכוללת **הוצאות**, ניתן לשייך את המשימת **T1** בשורת הצעת המחיר כלא ניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="cc019-124">If there is a second quote line that includes **Expenses**, you can associate the **T1** task on the quote line as non-chargeable.</span></span> <span data-ttu-id="cc019-125">התוצאה היא שכל הזמן שנרשם במשימה ניתן לחיוב וכל ההוצאות הנרשמות במשימה אינן ניתנות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="cc019-125">The result is that all time recorded on the task is chargeable and all expenses recorded on the task are non-chargeable.</span></span>

<span data-ttu-id="cc019-126">ניתן להגדיר את סוג החיוב של משימה בכרטיסיה **משימות הניתנות לחיוב** של שורת הצעת מחיר מבוססת פרויקט על ידי עדכון השדה **סוג החיוב** ברשת המשנה של **משימות של שורת הצעת מחיר**.</span><span class="sxs-lookup"><span data-stu-id="cc019-126">A task's billing type can be configured on the **Chargeable Tasks** tab of a project-based quote line by updating the **Billing Type** field on the **Quote Line Tasks** subgrid.</span></span> <span data-ttu-id="cc019-127">לחלופין, ניתן לעדכן את סוג החיוב עבור משימת פרויקט בשדה **סוג החיוב** ברשת המשנה של הגדרת חיוב משימה של פרויקט, שמציג את שורות הצעות המחיר המשויכות למשימה.</span><span class="sxs-lookup"><span data-stu-id="cc019-127">Alternatively, you can update the billing type for a project task in the **Billing Type** field on the subgrid on the task billing setup of a project that shows the quote lines associated to a task.</span></span>

### <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="cc019-128">עדכן תפקיד כניתן לחיוב או כלא ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-128">Update a role to be chargeable or non-chargeable</span></span>

<span data-ttu-id="cc019-129">תפקיד יכול להיות ניתן לחיות או לא ניתן לחייב בהקשר של שורת הצעת מחיר מבוססת פרויקט ספציפית.</span><span class="sxs-lookup"><span data-stu-id="cc019-129">A role can be chargeable or non-chargeable in the context of a specific project-based quote line.</span></span>

<span data-ttu-id="cc019-130">ניתן להגדיר את סוג החיוב של תפיקד בכרטיסיה **תפקידים הניתנים לחיוב** של שורת הצעת מחיר על ידי עדכון השדה **סוג החיוב** ברשת המשנה של **תפקידים הניתנים לחיוב**.</span><span class="sxs-lookup"><span data-stu-id="cc019-130">A role's billing type can be configured on the **Chargeable Roles** tab of a quote line by updating the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="cc019-131">עדכן קטגוריית עסקאות כניתנת לחיוב או כלא ניתנת לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-131">Update a transaction category to be chargeable or non-chargeable</span></span>

<span data-ttu-id="cc019-132">קטגוריה של עסקאות יכולה להיות ניתנת לחיוב או לא ניתנת לחייב בשורת הצעת מחיר ספציפית.</span><span class="sxs-lookup"><span data-stu-id="cc019-132">A transaction category can be chargeable or non-chargeable on a specific quote line.</span></span>

<span data-ttu-id="cc019-133">ניתן להגדיר את סוג החיוב של עסקה בכרטיסיה **קטגוריות הניתנות לחיוב** של שורת הצעת מחיר על ידי עדכון השדה **סוג החיוב** ברשת המשנה של **קטגוריות הניתנות לחיוב**.</span><span class="sxs-lookup"><span data-stu-id="cc019-133">A transaction's billing type can be configured on the **Chargeable Categories** tab of a quote line by updating the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="cc019-134">פתרון של יכולת חיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-134">Resolve chargeability</span></span>
<span data-ttu-id="cc019-135">הערכה או נתונים בפועל שנוצרו עבור זמן נחשבים כניתנים לחיוב רק אם:</span><span class="sxs-lookup"><span data-stu-id="cc019-135">An estimate or actual created for time will only be considered chargeable if:</span></span>

   - <span data-ttu-id="cc019-136">**זמן** כלול בסעיף הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="cc019-136">**Time** is included on the quote line.</span></span>
   - <span data-ttu-id="cc019-137">**תפקיד** מוגדר כניתן לחיוב בסעיף הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="cc019-137">**Role** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="cc019-138">**משימות כלולות** מוגדרות בתור **משימות נבחרות** בסעיף הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="cc019-138">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span> 

<span data-ttu-id="cc019-139">אם שלושת הדברים הללו נכונים **המשימה** גם מוגדרת כניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="cc019-139">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="cc019-140">הערכה או נתונים בפועל שנוצרו עבור הוצאה נחשבים כניתנים לחיוב רק אם:</span><span class="sxs-lookup"><span data-stu-id="cc019-140">An estimate or actual created for expense is only considered chargeable if:</span></span> 

   - <span data-ttu-id="cc019-141">**הוצאה** כלולה בסעיף הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="cc019-141">**Expense** is included on the quote line.</span></span>
   - <span data-ttu-id="cc019-142">**קטגוריית עסקה** מוגדרת כניתנת לחיוב בסעיף הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="cc019-142">**Transaction category** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="cc019-143">**משימות כלולות** מוגדרות בתור **משימות נבחרות** בסעיף הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="cc019-143">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="cc019-144">אם שלושת הדברים הללו נכונים **המשימה** גם מוגדרת כניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="cc019-144">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="cc019-145">הערכה או נתונים בפועל שנוצרו עבור חומר נחשבים כניתנים לחיוב רק אם:</span><span class="sxs-lookup"><span data-stu-id="cc019-145">An estimate or actual created for material will only be considered chargeable if:</span></span>

   - <span data-ttu-id="cc019-146">**חומרים** כלולים בסעיף הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="cc019-146">**Materials** is included on the quote line.</span></span>
   - <span data-ttu-id="cc019-147">**משימות כלולות** מוגדרות בתור **משימות נבחרות** בסעיף הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="cc019-147">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="cc019-148">אם שני הדברים הללו נכונים, **המשימה** גם צריכה להיות מוגדרת כניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="cc019-148">If these two things are true, the **Task** should also be configured as chargeable.</span></span> 


<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="cc019-149">
                    <strong>כולל זמן</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-149">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="cc019-150">
                    <strong>כולל הוצאה</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-150">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="cc019-151">
                    <strong>כולל חומרים</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-151">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="cc019-152">
                    <strong>משימות כלולות</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-152">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="cc019-153">
                    <strong>תפקיד</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-153">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="cc019-154">
                    <strong>קטגוריה</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-154">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="cc019-155">
                    <strong>משימה</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-155">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="cc019-156">
                    <strong>השפעת יכולת החיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-156">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-157">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-157">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="cc019-158">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-158">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="cc019-159">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-159">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="cc019-160">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="cc019-160">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-161">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-161">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-162">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-162">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-163">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="cc019-163">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="cc019-164">חיוב לפי נתוני זמן בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-164">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="cc019-165">סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-165">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="cc019-166">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-166">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-167">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-167">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="cc019-168">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-168">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="cc019-169">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-169">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="cc019-170">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="cc019-170">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-171">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-171">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-172">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-172">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-173">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-173">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="cc019-174">חיוב לפי נתוני זמן בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-174">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="cc019-175">סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-175">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="cc019-176">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-176">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-177">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-177">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="cc019-178">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-178">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="cc019-179">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-179">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="cc019-180">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="cc019-180">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="cc019-181">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-181">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-182">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-182">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-183">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-183">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="cc019-184">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-184">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="cc019-185">סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-185">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="cc019-186">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-186">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-187">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-187">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="cc019-188">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-188">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="cc019-189">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-189">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="cc019-190">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="cc019-190">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-191">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-191">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-192">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-192">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="cc019-193">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-193">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="cc019-194">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-194">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="cc019-195">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-195">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="cc019-196">סוג חיוב עבור נתוני חומר בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-196">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-197">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-197">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="cc019-198">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-198">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="cc019-199">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-199">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="cc019-200">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="cc019-200">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="cc019-201">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-201">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-202">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-202">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="cc019-203">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-203">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="cc019-204">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-204">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="cc019-205">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-205">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="cc019-206">סוג חיוב עבור נתוני חומר בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-206">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-207">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-207">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="cc019-208">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-208">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="cc019-209">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-209">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="cc019-210">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="cc019-210">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="cc019-211">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-211">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="cc019-212">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-212">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-213">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-213">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="cc019-214">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-214">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="cc019-215">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-215">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="cc019-216">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-216">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="cc019-217">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-217">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="cc019-218">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-218">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="cc019-219">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-219">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="cc019-220">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="cc019-220">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-221">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="cc019-221">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="cc019-222">
                    <strong>ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-222">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-223">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="cc019-223">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="cc019-224">חיוב לפי נתוני זמן בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-224">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="cc019-225">סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-225">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="cc019-226">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-226">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="cc019-227">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-227">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="cc019-228">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-228">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="cc019-229">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-229">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="cc019-230">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="cc019-230">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-231">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="cc019-231">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="cc019-232">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-232">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-233">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="cc019-233">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="cc019-234">חיוב לפי נתוני זמן בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-234">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="cc019-235">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-235">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="cc019-236">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-236">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-237">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-237">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="cc019-238">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-238">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="cc019-239">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-239">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="cc019-240">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="cc019-240">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-241">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-241">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-242">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="cc019-242">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-243">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="cc019-243">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="cc019-244">חיוב לפי נתוני זמן בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-244">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="cc019-245">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-245">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="cc019-246">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-246">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-247">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-247">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="cc019-248">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-248">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="cc019-249">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-249">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="cc019-250">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="cc019-250">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="cc019-251">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-251">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-252">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="cc019-252">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-253">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="cc019-253">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="cc019-254">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-254">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="cc019-255">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-255">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="cc019-256">סוג חיוב עבור נתוני חומר בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-256">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-257">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-257">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="cc019-258">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-258">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="cc019-259">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-259">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="cc019-260">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="cc019-260">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-261">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-261">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-262">ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-262">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-263">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="cc019-263">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="cc019-264">חיוב לפי נתוני זמן בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-264">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="cc019-265">סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="cc019-265">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="cc019-266">סוג חיוב עבור נתוני חומר בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-266">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="cc019-267">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-267">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="cc019-268">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="cc019-268">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="cc019-269">
                    <strong>Yes</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-269">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="cc019-270">הפרוייקט כולו</span><span class="sxs-lookup"><span data-stu-id="cc019-270">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="cc019-271">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-271">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="cc019-272">
                    <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-272">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="cc019-273">לא ניתן להגדיר</span><span class="sxs-lookup"><span data-stu-id="cc019-273">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="cc019-274">חיוב לפי נתוני זמן בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-274">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="cc019-275">סוג חיוב עבור נתוני הוצאה בפועל: <strong>לא ניתן לחיוב</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-275">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="cc019-276">סוג חיוב עבור נתוני חומר בפועל: <strong>לא זמין</strong>
                </span><span class="sxs-lookup"><span data-stu-id="cc019-276">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]
