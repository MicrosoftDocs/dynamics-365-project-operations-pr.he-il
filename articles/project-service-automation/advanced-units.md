---
title: קבוצות יחידות ויחידות
description: נושא זה מספק מידע אודות קבוצות יחידות ויחידות.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: b5422be3-5bfc-4ee2-b19a-4eca68813ff2
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: fc2dde2d9471f8585c190a65f3ad9b32de75af86
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751909"
---
# <a name="unit-groups-and-units"></a><span data-ttu-id="07b62-103">קבוצות יחידות ויחידות</span><span class="sxs-lookup"><span data-stu-id="07b62-103">Unit groups and units</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="07b62-104">קבוצות יחידות ויחידות הן ישויות בסיסיות ב- Microsoft Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="07b62-104">Unit groups and units are basic entities in Microsoft Dynamics 365.</span></span> <span data-ttu-id="07b62-105">יחידה היא יחידת מידה יחידה, וניתן לקבץ יחידות מרובות לקבוצות יחידות.</span><span class="sxs-lookup"><span data-stu-id="07b62-105">A unit is a single unit of measure, and multiple units can be grouped into unit groups.</span></span> <span data-ttu-id="07b62-106">קבוצת יחידות מכונה לעתים לוח זמנים של יחידה בממשק המשתמש (UI) של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="07b62-106">A unit group is sometimes referred to as a unit schedule in the Dynamics 365 user interface (UI).</span></span> 

<span data-ttu-id="07b62-107">להלן מספר דוגמאות של יחידות וקבוצות יחידות:</span><span class="sxs-lookup"><span data-stu-id="07b62-107">Here are some examples of units and unit groups:</span></span>
 
- <span data-ttu-id="07b62-108">**קבוצת יחידות**: מרחק</span><span class="sxs-lookup"><span data-stu-id="07b62-108">**Unit group**: Distance</span></span> 
    - <span data-ttu-id="07b62-109">**יחידות**: מייל, קילומטר וכן הלאה.</span><span class="sxs-lookup"><span data-stu-id="07b62-109">**Units**: Mile, Kilometer, and so on.</span></span>
- <span data-ttu-id="07b62-110">**קבוצת יחידות**: זמן</span><span class="sxs-lookup"><span data-stu-id="07b62-110">**Unit group**: Time</span></span>
    - <span data-ttu-id="07b62-111">**יחידות**: שעה, יום, שבוע וכן הלאה.</span><span class="sxs-lookup"><span data-stu-id="07b62-111">**Units**: Hour, day, week, and so on.</span></span> 

<span data-ttu-id="07b62-112">כאשר אתה מגדיר יחידות מרובות בקבוצת יחידות, עליך גם להגדיר גורם המרה ביניהן על-ידי הקצאת היחידה הראשונה שאתה מגדיר כיחידת ברירת המחדל או היחידה הראשית עבור קבוצת היחידות.</span><span class="sxs-lookup"><span data-stu-id="07b62-112">When you set up multiple units in a unit group, you must also set up a conversion factor between them by designating the first unit that you set up as the default or primary unit for the unit group.</span></span> 

<span data-ttu-id="07b62-113">לדוגמה, בקבוצת יחידות **זמן**, אם אתה מגדיר את **שעה** כיחידה הראשונה, המערכת מקצה את **שעה** כיחידת ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="07b62-113">For example, in a **Time** unit group, if you set up **Hour** as the first unit, the system designates **Hour** as the default unit.</span></span> <span data-ttu-id="07b62-114">אם היחידה הבאה שאתה מגדיר היא **יום**, עליך להגדיר גורם המרה עבור **יום** ל**שעה**.</span><span class="sxs-lookup"><span data-stu-id="07b62-114">If the next unit that you set up is **Day**, you must set up a conversion factor for **Day** to **Hour**.</span></span> <span data-ttu-id="07b62-115">אם לאחר מכן אתה מוסיף את **שבוע** כיחידה שלישית, עליך להגדיר גורם המרה עבור **שבוע** במונחים של **יום** או **שעה**.</span><span class="sxs-lookup"><span data-stu-id="07b62-115">If you then add **Week** as a third unit, you must set up a conversion factor for **Week** in terms of **Day** or **Hour**.</span></span> 

<span data-ttu-id="07b62-116">התמונה הבאה מציגה הגדרה לדוגמה עבור היחידה **יום** כאשר השדה **כמות** מציג את מספר השעות ביום, והיחידה **שבוע**, כאשר השדה **כמות** מציג את מספר הימים בשבוע.</span><span class="sxs-lookup"><span data-stu-id="07b62-116">The following image shows an example setup for the **Day** unit, where the **Quantity** field shows the number of hours that are in a day, and **Week**, where the **Quantity** field show the number of days that are in a week.</span></span>

> ![קבוצת יחידות: דף מידע](media/advanced-2.png)

## <a name="using-units-and-unit-groups"></a><span data-ttu-id="07b62-118">שימוש ביחידות ובקבוצות יחידות</span><span class="sxs-lookup"><span data-stu-id="07b62-118">Using units and unit groups</span></span>

<span data-ttu-id="07b62-119">Dynamics 365 Project Service Automation משתמש ביחידות ובקבוצות יחידות כדי לעבד הערכות וערכים עבור הוצאות וזמן.</span><span class="sxs-lookup"><span data-stu-id="07b62-119">Dynamics 365 Project Service Automation uses units and unit groups to process estimates and entries for both expenses and time.</span></span> 

<span data-ttu-id="07b62-120">עבור הוצאות, לכל קטגוריית הוצאה יש קבוצת יחידות ויחידה של ברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="07b62-120">For expenses, each expense category has a default unit group and unit.</span></span> <span data-ttu-id="07b62-121">ערכים אלה מוזנים כערכי ברירת מחדל בערכי מחירון עבור קטגוריות הוצאות.</span><span class="sxs-lookup"><span data-stu-id="07b62-121">These values are entered as default values on price list entries for expense categories.</span></span> 

<span data-ttu-id="07b62-122">לדוגמה, יש לך קטגוריית הוצאות שנקראת **מרחק**.</span><span class="sxs-lookup"><span data-stu-id="07b62-122">For example, you have an expense category that is named **Mileage**.</span></span> <span data-ttu-id="07b62-123">יש לה קבוצת יחידות שנקראת **מרחק** ויחידת ברירת מחדל שנקראת **מייל**.</span><span class="sxs-lookup"><span data-stu-id="07b62-123">It has a unit group that is named **Distance** and a default unit that is named **Mile**.</span></span> <span data-ttu-id="07b62-124">אם תגדיר את קבוצת היחידות **מרחק** כך שתכלול שתי יחידות (**מייל** ו**קילומטר**), תוכל להגדיר שני מחירים עבור הקטגוריה **מרחק** במחירון אחד: מחיר למייל ומחיר לקילומטר.</span><span class="sxs-lookup"><span data-stu-id="07b62-124">If you set up the **Distance** unit group so that it has two units (**Mile** and **Kilometer**), you can set two prices for the **Mileage** category on one price list: price per mile and price per kilometer.</span></span>

| <span data-ttu-id="07b62-125">קטגוריית הוצאות</span><span class="sxs-lookup"><span data-stu-id="07b62-125">Expense category</span></span>  | <span data-ttu-id="07b62-126">קבוצת יחידות</span><span class="sxs-lookup"><span data-stu-id="07b62-126">Unit group</span></span>  | <span data-ttu-id="07b62-127">יחידה</span><span class="sxs-lookup"><span data-stu-id="07b62-127">Unit</span></span>      | <span data-ttu-id="07b62-128">שיטת תמחור</span><span class="sxs-lookup"><span data-stu-id="07b62-128">Pricing method</span></span>  | <span data-ttu-id="07b62-129">מחיר ליחידה</span><span class="sxs-lookup"><span data-stu-id="07b62-129">Price per unit</span></span>  |
|-------------------|---------------|-----------|-------------------|-------------------|
| <span data-ttu-id="07b62-130">קילומטרים</span><span class="sxs-lookup"><span data-stu-id="07b62-130">Mileage</span></span>           | <span data-ttu-id="07b62-131">מרחק</span><span class="sxs-lookup"><span data-stu-id="07b62-131">Distance</span></span>      | <span data-ttu-id="07b62-132">מייל</span><span class="sxs-lookup"><span data-stu-id="07b62-132">Mile</span></span>      | <span data-ttu-id="07b62-133">מחיר ליחידה</span><span class="sxs-lookup"><span data-stu-id="07b62-133">Price per unit</span></span>    | <span data-ttu-id="07b62-134">10‎ USD</span><span class="sxs-lookup"><span data-stu-id="07b62-134">10 USD</span></span>            |
| <span data-ttu-id="07b62-135">קילומטרים</span><span class="sxs-lookup"><span data-stu-id="07b62-135">Mileage</span></span>           | <span data-ttu-id="07b62-136">מרחק</span><span class="sxs-lookup"><span data-stu-id="07b62-136">Distance</span></span>      | <span data-ttu-id="07b62-137">קילומטר</span><span class="sxs-lookup"><span data-stu-id="07b62-137">Kilometer</span></span> | <span data-ttu-id="07b62-138">מחיר ליחידה</span><span class="sxs-lookup"><span data-stu-id="07b62-138">Price per unit</span></span>    |  <span data-ttu-id="07b62-139">6‎ USD</span><span class="sxs-lookup"><span data-stu-id="07b62-139">6 USD</span></span>            |

<span data-ttu-id="07b62-140">בעת הזנת הוצאה בפרוייקט, המערכת קובעת את המחיר באמצעות שילוב הקטגוריה והיחידה בהוצאה.</span><span class="sxs-lookup"><span data-stu-id="07b62-140">When you enter an expense on a project, the system determines the price through the combination of the category and the unit on the expense.</span></span> 

| <span data-ttu-id="07b62-141">תיאור הוצאה</span><span class="sxs-lookup"><span data-stu-id="07b62-141">Expense description</span></span>        | <span data-ttu-id="07b62-142">קטגוריית הוצאות</span><span class="sxs-lookup"><span data-stu-id="07b62-142">Expense category</span></span>  | <span data-ttu-id="07b62-143">יחידה</span><span class="sxs-lookup"><span data-stu-id="07b62-143">Unit</span></span>  | <span data-ttu-id="07b62-144">כמות</span><span class="sxs-lookup"><span data-stu-id="07b62-144">Quantity</span></span>  | <span data-ttu-id="07b62-145">מחיר יחידה</span><span class="sxs-lookup"><span data-stu-id="07b62-145">Unit price</span></span>   |
|----------------------------|---------------------|-------|-----------|----------------|
| <span data-ttu-id="07b62-146">נסיעה למיקום לקוח</span><span class="sxs-lookup"><span data-stu-id="07b62-146">Drive to client location</span></span> | <span data-ttu-id="07b62-147">קילומטרים</span><span class="sxs-lookup"><span data-stu-id="07b62-147">Mileage</span></span>             | <span data-ttu-id="07b62-148">מייל</span><span class="sxs-lookup"><span data-stu-id="07b62-148">Mile</span></span>  | <span data-ttu-id="07b62-149">10</span><span class="sxs-lookup"><span data-stu-id="07b62-149">10</span></span>        | <span data-ttu-id="07b62-150">10‎ USD</span><span class="sxs-lookup"><span data-stu-id="07b62-150">10 USD</span></span>         |

<span data-ttu-id="07b62-151">עבור זמן, לכל כותרת מחירון יש שדה **יחידת זמן המהווה ברירת מחדל**.</span><span class="sxs-lookup"><span data-stu-id="07b62-151">For time, each price list header has a **Default Time Unit** field.</span></span> <span data-ttu-id="07b62-152">הערך מוגדר בעת יצירת כותרת המחירון.</span><span class="sxs-lookup"><span data-stu-id="07b62-152">The value is set when you create the price list header.</span></span> <span data-ttu-id="07b62-153">לאחר מכן, יחידה זו משמשת להגדרת כל המחירים מבוססי התפקיד במחירון זה.</span><span class="sxs-lookup"><span data-stu-id="07b62-153">This unit is then used to set all role-based prices on that price list.</span></span>

<span data-ttu-id="07b62-154">שורות הערכה עבור השדה **זמן בהצעת מחיר** עשויות להיות מבוטאות בכל יחידת זמן.</span><span class="sxs-lookup"><span data-stu-id="07b62-154">Estimate lines for the **Time on Quote** field can be expressed in any unit of time.</span></span> <span data-ttu-id="07b62-155">עם זאת, שורות הערכה בפרוייקטים ובערכי זמן עבור פרוייקטים יכולות להשתמש רק ביחידת הזמן **שעה**.</span><span class="sxs-lookup"><span data-stu-id="07b62-155">However, estimate lines on projects and time entries for projects can use only the **Hour** unit of time.</span></span> <span data-ttu-id="07b62-156">אם היחידה בערך הזמן או בשורת ההערכה אינה תואמת ליחידה בשורת המחירון עבור תפקיד זה, המערכת ממירה את המחיר ליחידות המוגדרות בהערכת הפרוייקט או בעסקה בפועל של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="07b62-156">If the unit on the time entry or estimate line doesn't match the unit on the price list line for that role, the system converts the price to the units that are defined in the project estimate or the project actual transaction.</span></span>

<span data-ttu-id="07b62-157">הדוגמה הבאה מציגה כיצד PSA משתמש בקבוצת היחידות, ביחידות ובגורם ההמרה.</span><span class="sxs-lookup"><span data-stu-id="07b62-157">The following example shows how PSA uses the unit group, units, and conversion factors.</span></span>
- <span data-ttu-id="07b62-158">יחידות</span><span class="sxs-lookup"><span data-stu-id="07b62-158">Units</span></span>

   - <span data-ttu-id="07b62-159">**קבוצת יחידות**: זמן</span><span class="sxs-lookup"><span data-stu-id="07b62-159">**Unit group**: Time</span></span> 
   - <span data-ttu-id="07b62-160">**יחידות**: שעה</span><span class="sxs-lookup"><span data-stu-id="07b62-160">**Units**: Hour</span></span> 
    
    - <span data-ttu-id="07b62-161">**יום** - גורם המרה: 8 שעות</span><span class="sxs-lookup"><span data-stu-id="07b62-161">**Day** - Conversion factor: 8 hours</span></span>       
    - <span data-ttu-id="07b62-162">**שבוע** - גורם המרה: 40 שעות</span><span class="sxs-lookup"><span data-stu-id="07b62-162">**Week** - Conversion factor: 40 hours</span></span>  
        
- <span data-ttu-id="07b62-163">הגדרת מחירון בפרוייקט A:</span><span class="sxs-lookup"><span data-stu-id="07b62-163">Price list setup on Project A:</span></span>

    - <span data-ttu-id="07b62-164">**שם**: מחירי מכירות בבריטניה לשנת 2016</span><span class="sxs-lookup"><span data-stu-id="07b62-164">**Name**: UK sales prices 2016</span></span> 
    - <span data-ttu-id="07b62-165">**יחידת זמן המהווה ברירת מחדל**: יום</span><span class="sxs-lookup"><span data-stu-id="07b62-165">**Default time unit**: Day</span></span> 
    - <span data-ttu-id="07b62-166">**מטבע**:‏ GBP</span><span class="sxs-lookup"><span data-stu-id="07b62-166">**Currency**: GBP</span></span>

| <span data-ttu-id="07b62-167">תפקיד</span><span class="sxs-lookup"><span data-stu-id="07b62-167">Role</span></span>      | <span data-ttu-id="07b62-168">קבוצת יחידות</span><span class="sxs-lookup"><span data-stu-id="07b62-168">Unit group</span></span> | <span data-ttu-id="07b62-169">יחידה</span><span class="sxs-lookup"><span data-stu-id="07b62-169">Unit</span></span> | <span data-ttu-id="07b62-170">יחידה ארגונית</span><span class="sxs-lookup"><span data-stu-id="07b62-170">Organizational unit</span></span> | <span data-ttu-id="07b62-171">מחיר</span><span class="sxs-lookup"><span data-stu-id="07b62-171">Price</span></span>   |
|-----------|------------|------|---------------------|---------|
| <span data-ttu-id="07b62-172">מפתח</span><span class="sxs-lookup"><span data-stu-id="07b62-172">Developer</span></span> | <span data-ttu-id="07b62-173">Time</span><span class="sxs-lookup"><span data-stu-id="07b62-173">Time</span></span>       | <span data-ttu-id="07b62-174">Day</span><span class="sxs-lookup"><span data-stu-id="07b62-174">Day</span></span>  | <span data-ttu-id="07b62-175">Contoso UK</span><span class="sxs-lookup"><span data-stu-id="07b62-175">Contoso UK</span></span>          | <span data-ttu-id="07b62-176">80‎0 GBP</span><span class="sxs-lookup"><span data-stu-id="07b62-176">800 GBP</span></span> |

### <a name="time-entry"></a><span data-ttu-id="07b62-177">ערך זמן</span><span class="sxs-lookup"><span data-stu-id="07b62-177">Time entry</span></span>

<span data-ttu-id="07b62-178">הטבלה הבאה מציגה את העסקה המתקבלת בצד המכירות שנוצרות על-ידי PSA עבור פרוייקט של שלוש שעות.</span><span class="sxs-lookup"><span data-stu-id="07b62-178">The following table shows the resulting sales-side transaction created by PSA for a three hour project.</span></span>


| <span data-ttu-id="07b62-179">פרוייקט</span><span class="sxs-lookup"><span data-stu-id="07b62-179">Project</span></span>   | <span data-ttu-id="07b62-180">משימה</span><span class="sxs-lookup"><span data-stu-id="07b62-180">Task</span></span>    | <span data-ttu-id="07b62-181">תפקיד</span><span class="sxs-lookup"><span data-stu-id="07b62-181">Role</span></span>      | <span data-ttu-id="07b62-182">כמות</span><span class="sxs-lookup"><span data-stu-id="07b62-182">Quantity</span></span> | <span data-ttu-id="07b62-183">יחידה</span><span class="sxs-lookup"><span data-stu-id="07b62-183">Unit</span></span>  | <span data-ttu-id="07b62-184">מחיר יחידה</span><span class="sxs-lookup"><span data-stu-id="07b62-184">Unit price</span></span> | <span data-ttu-id="07b62-185">סכום מכירות שלא חויבו</span><span class="sxs-lookup"><span data-stu-id="07b62-185">Unbilled sales amount</span></span> |
|-----------|---------|-----------|----------|-------|------------|-----------------------|
| <span data-ttu-id="07b62-186">פרוייקט A</span><span class="sxs-lookup"><span data-stu-id="07b62-186">Project A</span></span> | <span data-ttu-id="07b62-187">עיצוב</span><span class="sxs-lookup"><span data-stu-id="07b62-187">Design</span></span>  | <span data-ttu-id="07b62-188">מפתח</span><span class="sxs-lookup"><span data-stu-id="07b62-188">Developer</span></span> | <span data-ttu-id="07b62-189">3</span><span class="sxs-lookup"><span data-stu-id="07b62-189">3</span></span>        | <span data-ttu-id="07b62-190">Hour</span><span class="sxs-lookup"><span data-stu-id="07b62-190">Hour</span></span>  | <span data-ttu-id="07b62-191">10‎0 GBP</span><span class="sxs-lookup"><span data-stu-id="07b62-191">100 GBP</span></span>    | <span data-ttu-id="07b62-192">300‎ GBP</span><span class="sxs-lookup"><span data-stu-id="07b62-192">300 GBP</span></span>               |

## <a name="time-unit-faq"></a><span data-ttu-id="07b62-193">שאלות נפוצות אודות יחידת זמן</span><span class="sxs-lookup"><span data-stu-id="07b62-193">Time unit FAQ</span></span>

### <a name="does-psa-convert-to-different-units-in-the-case-of-expenses"></a><span data-ttu-id="07b62-194">האם PSA ממיר ליחידות שונות במקרה של הוצאות?</span><span class="sxs-lookup"><span data-stu-id="07b62-194">Does PSA convert to different units in the case of expenses?</span></span>
<span data-ttu-id="07b62-195">מספר</span><span class="sxs-lookup"><span data-stu-id="07b62-195">No.</span></span> <span data-ttu-id="07b62-196">המרת יחידה פועלת רק עבור זמן.</span><span class="sxs-lookup"><span data-stu-id="07b62-196">Unit conversion works only for time.</span></span> <span data-ttu-id="07b62-197">עבור הוצאות, אם למערכת אין אפשרות למצוא מחיר עבור השילוב של קטגוריית ההוצאות והיחידה, המחיר מוגדר כ- 0.00 כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="07b62-197">For expenses, if the system can't find a price for the combination of the expense category and unit, the price is set to 0.00 by default.</span></span>

### <a name="why-does-psa-convert-time-units"></a><span data-ttu-id="07b62-198">מדוע PSA ממיר יחידות זמן?</span><span class="sxs-lookup"><span data-stu-id="07b62-198">Why does PSA convert time units?</span></span>
<span data-ttu-id="07b62-199">במדינות או באזורים מסוימים, קיימת דרישה משפטית שתעריפי החיוב יוגדרו בימים.</span><span class="sxs-lookup"><span data-stu-id="07b62-199">In some countries or regions, there is a legal requirement that bill rates be set up in days.</span></span> <span data-ttu-id="07b62-200">משא ומתן על מחירים והנחות במהלך מחזור הצעת המחיר מתבצע באמצעות תעריפי יום עבור כל תפקיד הניתן לחיוב.</span><span class="sxs-lookup"><span data-stu-id="07b62-200">Price negotiation and discounting during the quote cycle is done by using day rates for each billable role.</span></span> <span data-ttu-id="07b62-201">הזנת הערכה וזמן של לוח זמנים מתבצעת בשעות.</span><span class="sxs-lookup"><span data-stu-id="07b62-201">Schedule estimation and time entry are done in hours.</span></span> <span data-ttu-id="07b62-202">כדי לתמוך בהבדל זה ביחידות זמן, PSA ממיר יחידות זמן.</span><span class="sxs-lookup"><span data-stu-id="07b62-202">To support this difference in time units, PSA converts time units.</span></span>

### <a name="can-time-units-be-changed-on-project-estimates"></a><span data-ttu-id="07b62-203">האם ניתן לשנות יחידות זמן בהערכות של פרוייקט?</span><span class="sxs-lookup"><span data-stu-id="07b62-203">Can time units be changed on project estimates?</span></span>
<span data-ttu-id="07b62-204">מספר</span><span class="sxs-lookup"><span data-stu-id="07b62-204">No.</span></span> <span data-ttu-id="07b62-205">הערכת לוח זמנים מוגבלת כעת לשעות ולא ניתן לשנות אותה.</span><span class="sxs-lookup"><span data-stu-id="07b62-205">Schedule estimation is currently restricted to hours and can’t be changed.</span></span>

### <a name="can-units-and-unit-groups-be-edited-deleted-and-added"></a><span data-ttu-id="07b62-206">האם ניתן לערוך, למחוק ולהוסיף יחידות וקבוצות יחידות?</span><span class="sxs-lookup"><span data-stu-id="07b62-206">Can units and unit groups be edited, deleted, and added?</span></span>
<span data-ttu-id="07b62-207">כן.</span><span class="sxs-lookup"><span data-stu-id="07b62-207">Yes.</span></span> <span data-ttu-id="07b62-208">למעט קבוצת היחידות **זמן** והיחידה **שעה**, ניתן למחוק או לערוך את כל היחידות, ולהוסיף יחידות חדשות.</span><span class="sxs-lookup"><span data-stu-id="07b62-208">With exception of the **Time** unit group and the **Hour** unit, all units can be deleted or edited, and new units can be added.</span></span> <span data-ttu-id="07b62-209">ב- PSA, לא ניתן למחוק את קבוצת היחידות **זמן** ואת היחידה **שעה**.</span><span class="sxs-lookup"><span data-stu-id="07b62-209">In PSA, the **Time** unit group and the **Hour** unit can't be deleted.</span></span> <span data-ttu-id="07b62-210">עם זאת, ניתן לעדכן אותן בטקסט מתורגם עבור השדה **שם**.</span><span class="sxs-lookup"><span data-stu-id="07b62-210">However, they can be updated with a translated text for the **Name** field.</span></span>
