---
title: קבוצות יחידות ויחידות
description: נושא זה מספק מידע אודות קבוצות יחידות ויחידות.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 58ce821d11d729f6e2c33e5a50344458e395db4d
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130579"
---
# <a name="unit-groups-and-units"></a><span data-ttu-id="03cce-103">קבוצות יחידות ויחידות</span><span class="sxs-lookup"><span data-stu-id="03cce-103">Unit groups and units</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="03cce-104">קבוצות יחידות ויחידות הן ישויות בסיסיות ב- Microsoft Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="03cce-104">Unit groups and units are basic entities in Microsoft Dynamics 365.</span></span> <span data-ttu-id="03cce-105">יחידה היא יחידת מידה יחידה, וניתן לקבץ יחידות מרובות לקבוצות יחידות.</span><span class="sxs-lookup"><span data-stu-id="03cce-105">A unit is a single unit of measure, and multiple units can be grouped into unit groups.</span></span> <span data-ttu-id="03cce-106">קבוצת יחידות מכונה לעתים לוח זמנים של יחידה בממשק המשתמש (UI) של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="03cce-106">A unit group is sometimes referred to as a unit schedule in the Dynamics 365 user interface (UI).</span></span> 

<span data-ttu-id="03cce-107">להלן מספר דוגמאות של יחידות וקבוצות יחידות:</span><span class="sxs-lookup"><span data-stu-id="03cce-107">Here are some examples of units and unit groups:</span></span>
 
- <span data-ttu-id="03cce-108">**קבוצת יחידות**: מרחק</span><span class="sxs-lookup"><span data-stu-id="03cce-108">**Unit group**: Distance</span></span> 
    - <span data-ttu-id="03cce-109">**יחידות**: מייל, קילומטר וכן הלאה.</span><span class="sxs-lookup"><span data-stu-id="03cce-109">**Units**: Mile, Kilometer, and so on.</span></span>
- <span data-ttu-id="03cce-110">**קבוצת יחידות**: זמן</span><span class="sxs-lookup"><span data-stu-id="03cce-110">**Unit group**: Time</span></span>
    - <span data-ttu-id="03cce-111">**יחידות**: שעה, יום, שבוע וכן הלאה.</span><span class="sxs-lookup"><span data-stu-id="03cce-111">**Units**: Hour, day, week, and so on.</span></span> 

<span data-ttu-id="03cce-112">כאשר אתה מגדיר יחידות מרובות בקבוצת יחידות, עליך גם להגדיר גורם המרה ביניהן על-ידי הקצאת היחידה הראשונה שאתה מגדיר כיחידת ברירת המחדל או היחידה הראשית עבור קבוצת היחידות.</span><span class="sxs-lookup"><span data-stu-id="03cce-112">When you set up multiple units in a unit group, you must also set up a conversion factor between them by designating the first unit that you set up as the default or primary unit for the unit group.</span></span> 

<span data-ttu-id="03cce-113">לדוגמה, בקבוצת יחידות **זמן**, אם אתה מגדיר את **שעה** כיחידה הראשונה, המערכת מקצה את **שעה** כיחידת ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="03cce-113">For example, in a **Time** unit group, if you set up **Hour** as the first unit, the system designates **Hour** as the default unit.</span></span> <span data-ttu-id="03cce-114">אם היחידה הבאה שאתה מגדיר היא **יום**, עליך להגדיר גורם המרה עבור **יום** ל **שעה**.</span><span class="sxs-lookup"><span data-stu-id="03cce-114">If the next unit that you set up is **Day**, you must set up a conversion factor for **Day** to **Hour**.</span></span> <span data-ttu-id="03cce-115">אם לאחר מכן אתה מוסיף את **שבוע** כיחידה שלישית, עליך להגדיר גורם המרה עבור **שבוע** במונחים של **יום** או **שעה**.</span><span class="sxs-lookup"><span data-stu-id="03cce-115">If you then add **Week** as a third unit, you must set up a conversion factor for **Week** in terms of **Day** or **Hour**.</span></span> 

<span data-ttu-id="03cce-116">התמונה הבאה מציגה הגדרה לדוגמה עבור היחידה **יום** כאשר השדה **כמות** מציג את מספר השעות ביום, והיחידה **שבוע**, כאשר השדה **כמות** מציג את מספר הימים בשבוע.</span><span class="sxs-lookup"><span data-stu-id="03cce-116">The following image shows an example setup for the **Day** unit, where the **Quantity** field shows the number of hours that are in a day, and **Week**, where the **Quantity** field show the number of days that are in a week.</span></span>

> ![קבוצת יחידות: דף מידע](media/advanced-2.png)

## <a name="using-units-and-unit-groups"></a><span data-ttu-id="03cce-118">שימוש ביחידות ובקבוצות יחידות</span><span class="sxs-lookup"><span data-stu-id="03cce-118">Using units and unit groups</span></span>

<span data-ttu-id="03cce-119">Dynamics 365 Project Service Automation משתמש ביחידות ובקבוצות יחידות כדי לעבד הערכות וערכים עבור הוצאות וזמן.</span><span class="sxs-lookup"><span data-stu-id="03cce-119">Dynamics 365 Project Service Automation uses units and unit groups to process estimates and entries for both expenses and time.</span></span> 

<span data-ttu-id="03cce-120">עבור הוצאות, לכל קטגוריית הוצאה יש קבוצת יחידות ויחידה של ברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="03cce-120">For expenses, each expense category has a default unit group and unit.</span></span> <span data-ttu-id="03cce-121">ערכים אלה מוזנים כערכי ברירת מחדל בערכי מחירון עבור קטגוריות הוצאות.</span><span class="sxs-lookup"><span data-stu-id="03cce-121">These values are entered as default values on price list entries for expense categories.</span></span> 

<span data-ttu-id="03cce-122">לדוגמה, יש לך קטגוריית הוצאות שנקראת **מרחק**.</span><span class="sxs-lookup"><span data-stu-id="03cce-122">For example, you have an expense category that is named **Mileage**.</span></span> <span data-ttu-id="03cce-123">יש לה קבוצת יחידות שנקראת **מרחק** ויחידת ברירת מחדל שנקראת **מייל**.</span><span class="sxs-lookup"><span data-stu-id="03cce-123">It has a unit group that is named **Distance** and a default unit that is named **Mile**.</span></span> <span data-ttu-id="03cce-124">אם תגדיר את קבוצת היחידות **מרחק** כך שתכלול שתי יחידות (**מייל** ו **קילומטר**), תוכל להגדיר שני מחירים עבור הקטגוריה **מרחק** במחירון אחד: מחיר למייל ומחיר לקילומטר.</span><span class="sxs-lookup"><span data-stu-id="03cce-124">If you set up the **Distance** unit group so that it has two units (**Mile** and **Kilometer**), you can set two prices for the **Mileage** category on one price list: price per mile and price per kilometer.</span></span>

| <span data-ttu-id="03cce-125">קטגוריית הוצאות</span><span class="sxs-lookup"><span data-stu-id="03cce-125">Expense category</span></span>  | <span data-ttu-id="03cce-126">קבוצת יחידות</span><span class="sxs-lookup"><span data-stu-id="03cce-126">Unit group</span></span>  | <span data-ttu-id="03cce-127">יחידה</span><span class="sxs-lookup"><span data-stu-id="03cce-127">Unit</span></span>      | <span data-ttu-id="03cce-128">שיטת תמחור</span><span class="sxs-lookup"><span data-stu-id="03cce-128">Pricing method</span></span>  | <span data-ttu-id="03cce-129">מחיר ליחידה</span><span class="sxs-lookup"><span data-stu-id="03cce-129">Price per unit</span></span>  |
|-------------------|---------------|-----------|-------------------|-------------------|
| <span data-ttu-id="03cce-130">קילומטרים</span><span class="sxs-lookup"><span data-stu-id="03cce-130">Mileage</span></span>           | <span data-ttu-id="03cce-131">מרחק</span><span class="sxs-lookup"><span data-stu-id="03cce-131">Distance</span></span>      | <span data-ttu-id="03cce-132">מייל</span><span class="sxs-lookup"><span data-stu-id="03cce-132">Mile</span></span>      | <span data-ttu-id="03cce-133">מחיר ליחידה</span><span class="sxs-lookup"><span data-stu-id="03cce-133">Price per unit</span></span>    | <span data-ttu-id="03cce-134">10‎ USD</span><span class="sxs-lookup"><span data-stu-id="03cce-134">10 USD</span></span>            |
| <span data-ttu-id="03cce-135">קילומטרים</span><span class="sxs-lookup"><span data-stu-id="03cce-135">Mileage</span></span>           | <span data-ttu-id="03cce-136">מרחק</span><span class="sxs-lookup"><span data-stu-id="03cce-136">Distance</span></span>      | <span data-ttu-id="03cce-137">קילומטר</span><span class="sxs-lookup"><span data-stu-id="03cce-137">Kilometer</span></span> | <span data-ttu-id="03cce-138">מחיר ליחידה</span><span class="sxs-lookup"><span data-stu-id="03cce-138">Price per unit</span></span>    |  <span data-ttu-id="03cce-139">6‎ USD</span><span class="sxs-lookup"><span data-stu-id="03cce-139">6 USD</span></span>            |

<span data-ttu-id="03cce-140">בעת הזנת הוצאה בפרוייקט, המערכת קובעת את המחיר באמצעות שילוב הקטגוריה והיחידה בהוצאה.</span><span class="sxs-lookup"><span data-stu-id="03cce-140">When you enter an expense on a project, the system determines the price through the combination of the category and the unit on the expense.</span></span> 

| <span data-ttu-id="03cce-141">תיאור הוצאה</span><span class="sxs-lookup"><span data-stu-id="03cce-141">Expense description</span></span>        | <span data-ttu-id="03cce-142">קטגוריית הוצאות</span><span class="sxs-lookup"><span data-stu-id="03cce-142">Expense category</span></span>  | <span data-ttu-id="03cce-143">יחידה</span><span class="sxs-lookup"><span data-stu-id="03cce-143">Unit</span></span>  | <span data-ttu-id="03cce-144">כמות</span><span class="sxs-lookup"><span data-stu-id="03cce-144">Quantity</span></span>  | <span data-ttu-id="03cce-145">מחיר יחידה</span><span class="sxs-lookup"><span data-stu-id="03cce-145">Unit price</span></span>   |
|----------------------------|---------------------|-------|-----------|----------------|
| <span data-ttu-id="03cce-146">נסיעה למיקום לקוח</span><span class="sxs-lookup"><span data-stu-id="03cce-146">Drive to client location</span></span> | <span data-ttu-id="03cce-147">קילומטרים</span><span class="sxs-lookup"><span data-stu-id="03cce-147">Mileage</span></span>             | <span data-ttu-id="03cce-148">מייל</span><span class="sxs-lookup"><span data-stu-id="03cce-148">Mile</span></span>  | <span data-ttu-id="03cce-149">10</span><span class="sxs-lookup"><span data-stu-id="03cce-149">10</span></span>        | <span data-ttu-id="03cce-150">10‎ USD</span><span class="sxs-lookup"><span data-stu-id="03cce-150">10 USD</span></span>         |

<span data-ttu-id="03cce-151">עבור זמן, לכל כותרת מחירון יש שדה **יחידת זמן המהווה ברירת מחדל**.</span><span class="sxs-lookup"><span data-stu-id="03cce-151">For time, each price list header has a **Default Time Unit** field.</span></span> <span data-ttu-id="03cce-152">הערך מוגדר בעת יצירת כותרת המחירון.</span><span class="sxs-lookup"><span data-stu-id="03cce-152">The value is set when you create the price list header.</span></span> <span data-ttu-id="03cce-153">לאחר מכן, יחידה זו משמשת להגדרת כל המחירים מבוססי התפקיד במחירון זה.</span><span class="sxs-lookup"><span data-stu-id="03cce-153">This unit is then used to set all role-based prices on that price list.</span></span>

<span data-ttu-id="03cce-154">שורות הערכה עבור השדה **זמן בהצעת מחיר** עשויות להיות מבוטאות בכל יחידת זמן.</span><span class="sxs-lookup"><span data-stu-id="03cce-154">Estimate lines for the **Time on Quote** field can be expressed in any unit of time.</span></span> <span data-ttu-id="03cce-155">עם זאת, שורות הערכה בפרוייקטים ובערכי זמן עבור פרוייקטים יכולות להשתמש רק ביחידת הזמן **שעה**.</span><span class="sxs-lookup"><span data-stu-id="03cce-155">However, estimate lines on projects and time entries for projects can use only the **Hour** unit of time.</span></span> <span data-ttu-id="03cce-156">אם היחידה בערך הזמן או בשורת ההערכה אינה תואמת ליחידה בשורת המחירון עבור תפקיד זה, המערכת ממירה את המחיר ליחידות המוגדרות בהערכת הפרוייקט או בעסקה בפועל של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="03cce-156">If the unit on the time entry or estimate line doesn't match the unit on the price list line for that role, the system converts the price to the units that are defined in the project estimate or the project actual transaction.</span></span>

<span data-ttu-id="03cce-157">הדוגמה הבאה מציגה כיצד PSA משתמש בקבוצת היחידות, ביחידות ובגורם ההמרה.</span><span class="sxs-lookup"><span data-stu-id="03cce-157">The following example shows how PSA uses the unit group, units, and conversion factors.</span></span>
- <span data-ttu-id="03cce-158">יחידות</span><span class="sxs-lookup"><span data-stu-id="03cce-158">Units</span></span>

   - <span data-ttu-id="03cce-159">**קבוצת יחידות**: זמן</span><span class="sxs-lookup"><span data-stu-id="03cce-159">**Unit group**: Time</span></span> 
   - <span data-ttu-id="03cce-160">**יחידות**: שעה</span><span class="sxs-lookup"><span data-stu-id="03cce-160">**Units**: Hour</span></span> 
    
    - <span data-ttu-id="03cce-161">**יום** - גורם המרה: 8 שעות</span><span class="sxs-lookup"><span data-stu-id="03cce-161">**Day** - Conversion factor: 8 hours</span></span>       
    - <span data-ttu-id="03cce-162">**שבוע** - גורם המרה: 40 שעות</span><span class="sxs-lookup"><span data-stu-id="03cce-162">**Week** - Conversion factor: 40 hours</span></span>  
        
- <span data-ttu-id="03cce-163">הגדרת מחירון בפרוייקט A:</span><span class="sxs-lookup"><span data-stu-id="03cce-163">Price list setup on Project A:</span></span>

    - <span data-ttu-id="03cce-164">**שם**: מחירי מכירות בבריטניה לשנת 2016</span><span class="sxs-lookup"><span data-stu-id="03cce-164">**Name**: UK sales prices 2016</span></span> 
    - <span data-ttu-id="03cce-165">**יחידת זמן המהווה ברירת מחדל**: יום</span><span class="sxs-lookup"><span data-stu-id="03cce-165">**Default time unit**: Day</span></span> 
    - <span data-ttu-id="03cce-166">**מטבע**:‏ GBP</span><span class="sxs-lookup"><span data-stu-id="03cce-166">**Currency**: GBP</span></span>

| <span data-ttu-id="03cce-167">תפקיד</span><span class="sxs-lookup"><span data-stu-id="03cce-167">Role</span></span>      | <span data-ttu-id="03cce-168">קבוצת יחידות</span><span class="sxs-lookup"><span data-stu-id="03cce-168">Unit group</span></span> | <span data-ttu-id="03cce-169">יחידה</span><span class="sxs-lookup"><span data-stu-id="03cce-169">Unit</span></span> | <span data-ttu-id="03cce-170">יחידה ארגונית</span><span class="sxs-lookup"><span data-stu-id="03cce-170">Organizational unit</span></span> | <span data-ttu-id="03cce-171">מחיר</span><span class="sxs-lookup"><span data-stu-id="03cce-171">Price</span></span>   |
|-----------|------------|------|---------------------|---------|
| <span data-ttu-id="03cce-172">מפתח</span><span class="sxs-lookup"><span data-stu-id="03cce-172">Developer</span></span> | <span data-ttu-id="03cce-173">Time</span><span class="sxs-lookup"><span data-stu-id="03cce-173">Time</span></span>       | <span data-ttu-id="03cce-174">Day</span><span class="sxs-lookup"><span data-stu-id="03cce-174">Day</span></span>  | <span data-ttu-id="03cce-175">Contoso UK</span><span class="sxs-lookup"><span data-stu-id="03cce-175">Contoso UK</span></span>          | <span data-ttu-id="03cce-176">80‎0 GBP</span><span class="sxs-lookup"><span data-stu-id="03cce-176">800 GBP</span></span> |

### <a name="time-entry"></a><span data-ttu-id="03cce-177">ערך זמן</span><span class="sxs-lookup"><span data-stu-id="03cce-177">Time entry</span></span>

<span data-ttu-id="03cce-178">הטבלה הבאה מציגה את העסקה המתקבלת בצד המכירות שנוצרות על-ידי PSA עבור פרוייקט של שלוש שעות.</span><span class="sxs-lookup"><span data-stu-id="03cce-178">The following table shows the resulting sales-side transaction created by PSA for a three hour project.</span></span>


| <span data-ttu-id="03cce-179">פרוייקט</span><span class="sxs-lookup"><span data-stu-id="03cce-179">Project</span></span>   | <span data-ttu-id="03cce-180">משימה</span><span class="sxs-lookup"><span data-stu-id="03cce-180">Task</span></span>    | <span data-ttu-id="03cce-181">תפקיד</span><span class="sxs-lookup"><span data-stu-id="03cce-181">Role</span></span>      | <span data-ttu-id="03cce-182">כמות</span><span class="sxs-lookup"><span data-stu-id="03cce-182">Quantity</span></span> | <span data-ttu-id="03cce-183">יחידה</span><span class="sxs-lookup"><span data-stu-id="03cce-183">Unit</span></span>  | <span data-ttu-id="03cce-184">מחיר יחידה</span><span class="sxs-lookup"><span data-stu-id="03cce-184">Unit price</span></span> | <span data-ttu-id="03cce-185">סכום מכירות שלא חויבו</span><span class="sxs-lookup"><span data-stu-id="03cce-185">Unbilled sales amount</span></span> |
|-----------|---------|-----------|----------|-------|------------|-----------------------|
| <span data-ttu-id="03cce-186">פרוייקט A</span><span class="sxs-lookup"><span data-stu-id="03cce-186">Project A</span></span> | <span data-ttu-id="03cce-187">עיצוב</span><span class="sxs-lookup"><span data-stu-id="03cce-187">Design</span></span>  | <span data-ttu-id="03cce-188">מפתח</span><span class="sxs-lookup"><span data-stu-id="03cce-188">Developer</span></span> | <span data-ttu-id="03cce-189">3</span><span class="sxs-lookup"><span data-stu-id="03cce-189">3</span></span>        | <span data-ttu-id="03cce-190">Hour</span><span class="sxs-lookup"><span data-stu-id="03cce-190">Hour</span></span>  | <span data-ttu-id="03cce-191">10‎0 GBP</span><span class="sxs-lookup"><span data-stu-id="03cce-191">100 GBP</span></span>    | <span data-ttu-id="03cce-192">300‎ GBP</span><span class="sxs-lookup"><span data-stu-id="03cce-192">300 GBP</span></span>               |

## <a name="time-unit-faq"></a><span data-ttu-id="03cce-193">שאלות נפוצות אודות יחידת זמן</span><span class="sxs-lookup"><span data-stu-id="03cce-193">Time unit FAQ</span></span>

### <a name="does-psa-convert-to-different-units-in-the-case-of-expenses"></a><span data-ttu-id="03cce-194">האם PSA ממיר ליחידות שונות במקרה של הוצאות?</span><span class="sxs-lookup"><span data-stu-id="03cce-194">Does PSA convert to different units in the case of expenses?</span></span>
<span data-ttu-id="03cce-195">מספר</span><span class="sxs-lookup"><span data-stu-id="03cce-195">No.</span></span> <span data-ttu-id="03cce-196">המרת יחידה פועלת רק עבור זמן.</span><span class="sxs-lookup"><span data-stu-id="03cce-196">Unit conversion works only for time.</span></span> <span data-ttu-id="03cce-197">עבור הוצאות, אם למערכת אין אפשרות למצוא מחיר עבור השילוב של קטגוריית ההוצאות והיחידה, המחיר מוגדר כ- 0.00 כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="03cce-197">For expenses, if the system can't find a price for the combination of the expense category and unit, the price is set to 0.00 by default.</span></span>

### <a name="why-does-psa-convert-time-units"></a><span data-ttu-id="03cce-198">מדוע PSA ממיר יחידות זמן?</span><span class="sxs-lookup"><span data-stu-id="03cce-198">Why does PSA convert time units?</span></span>
<span data-ttu-id="03cce-199">במדינות או באזורים מסוימים, קיימת דרישה משפטית שתעריפי החיוב יוגדרו בימים.</span><span class="sxs-lookup"><span data-stu-id="03cce-199">In some countries or regions, there is a legal requirement that bill rates be set up in days.</span></span> <span data-ttu-id="03cce-200">משא ומתן על מחירים והנחות במהלך מחזור הצעת המחיר מתבצע באמצעות תעריפי יום עבור כל תפקיד הניתן לחיוב.</span><span class="sxs-lookup"><span data-stu-id="03cce-200">Price negotiation and discounting during the quote cycle is done by using day rates for each billable role.</span></span> <span data-ttu-id="03cce-201">הזנת הערכה וזמן של לוח זמנים מתבצעת בשעות.</span><span class="sxs-lookup"><span data-stu-id="03cce-201">Schedule estimation and time entry are done in hours.</span></span> <span data-ttu-id="03cce-202">כדי לתמוך בהבדל זה ביחידות זמן, PSA ממיר יחידות זמן.</span><span class="sxs-lookup"><span data-stu-id="03cce-202">To support this difference in time units, PSA converts time units.</span></span>

### <a name="can-time-units-be-changed-on-project-estimates"></a><span data-ttu-id="03cce-203">האם ניתן לשנות יחידות זמן בהערכות של פרוייקט?</span><span class="sxs-lookup"><span data-stu-id="03cce-203">Can time units be changed on project estimates?</span></span>
<span data-ttu-id="03cce-204">מספר</span><span class="sxs-lookup"><span data-stu-id="03cce-204">No.</span></span> <span data-ttu-id="03cce-205">הערכת לוח זמנים מוגבלת כעת לשעות ולא ניתן לשנות אותה.</span><span class="sxs-lookup"><span data-stu-id="03cce-205">Schedule estimation is currently restricted to hours and can’t be changed.</span></span>

### <a name="can-units-and-unit-groups-be-edited-deleted-and-added"></a><span data-ttu-id="03cce-206">האם ניתן לערוך, למחוק ולהוסיף יחידות וקבוצות יחידות?</span><span class="sxs-lookup"><span data-stu-id="03cce-206">Can units and unit groups be edited, deleted, and added?</span></span>
<span data-ttu-id="03cce-207">כן.</span><span class="sxs-lookup"><span data-stu-id="03cce-207">Yes.</span></span> <span data-ttu-id="03cce-208">למעט קבוצת היחידות **זמן** והיחידה **שעה**, ניתן למחוק או לערוך את כל היחידות, ולהוסיף יחידות חדשות.</span><span class="sxs-lookup"><span data-stu-id="03cce-208">With exception of the **Time** unit group and the **Hour** unit, all units can be deleted or edited, and new units can be added.</span></span> <span data-ttu-id="03cce-209">ב- PSA, לא ניתן למחוק את קבוצת היחידות **זמן** ואת היחידה **שעה**.</span><span class="sxs-lookup"><span data-stu-id="03cce-209">In PSA, the **Time** unit group and the **Hour** unit can't be deleted.</span></span> <span data-ttu-id="03cce-210">עם זאת, ניתן לעדכן אותן בטקסט מתורגם עבור השדה **שם**.</span><span class="sxs-lookup"><span data-stu-id="03cce-210">However, they can be updated with a translated text for the **Name** field.</span></span>
