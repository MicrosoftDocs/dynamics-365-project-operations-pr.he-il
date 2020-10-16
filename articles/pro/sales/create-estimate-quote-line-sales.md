---
title: הערכת שורת הצעת מחיר מבוססת פרויקט
description: נושא זה מספק מידע על אופן יצירת הערכה בשורת הצעת מחיר מבוססת פרויקט.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 65aee7238781ac90f603e57c6d9b0b92cabd6644
ms.sourcegitcommit: f6509f7d50de4d4ebb92c1bf2cfcdf09f17458eb
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/06/2020
ms.locfileid: "3966791"
---
# <a name="estimating-a-project-based-quote-line"></a><span data-ttu-id="1cb80-103">הערכת שורת הצעת מחיר מבוססת פרויקט</span><span class="sxs-lookup"><span data-stu-id="1cb80-103">Estimating a project-based quote line</span></span>

<span data-ttu-id="1cb80-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="1cb80-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1cb80-105">בשורת הצעת מחיר מבוססת פרויקט יש פרטים המסייעים להערכת העלות וההכנסה הפוטנציאלית של העבודה הכרוכה באספקת קו הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="1cb80-105">A project-based quote line has details that help with estimating the cost and potential revenue of the work involved to deliver the quote line.</span></span>

<span data-ttu-id="1cb80-106">להערכת קו הצעת מחיר מבוסס-פרוייקט, בשורת הצעת המחיר בחר בכרטיסיה **פרטים בשורת הצעת מחיר**. ישנן שתי דרכים ליצור הערכה בשורת הצעת מחיר מבוססת פרויקט:</span><span class="sxs-lookup"><span data-stu-id="1cb80-106">To estimate a project-based quote line, on the project-based quote line, select the **Quote Line Detail** tab. There are two ways to create an estimate on a project-based quote line:</span></span>

- <span data-ttu-id="1cb80-107">צור את ההערכה באופן ידני, ישירות על שורת הצעת המחיר באמצעות פרטי שורת הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="1cb80-107">Manually create the estimate directly on the quote line using quote line details</span></span> 
- <span data-ttu-id="1cb80-108">צור פרויקט ותוכנית פרוייקט, ואז שייך את הפרויקט ואת המשימות בפרויקט לשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="1cb80-108">Create a project and a project plan, and then associate the project and tasks on the project to the quote line.</span></span> <span data-ttu-id="1cb80-109">התהליך לייבוא הערכות מתכנית הפרויקט לשורת הצעת המחיר על בסיס המידע שמסרת יהופך לזמין.</span><span class="sxs-lookup"><span data-stu-id="1cb80-109">The process to import the estimates on the project plan into the quote line based on the information you provided will be enabled.</span></span>

## <a name="create-estimates-directly-on-a-project-based-quote-line"></a><span data-ttu-id="1cb80-110">יצירת הערכות ישירות בשורת הצעת מחיר מבוססת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="1cb80-110">Create estimates directly on a project-based quote line</span></span>

<span data-ttu-id="1cb80-111">ליצירת הערכות בשורת הצעת מחיר מבוססת פרויקט, בחר בכרטיסיה **פרטים בשורת הצעת מחיר**. פריט השורה שאתה יוצר בכרטיסייה זו יסכם את הערך הצעת המחיר בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="1cb80-111">To create an estimate on a project-based quote line, select the **Quote Line Detail** tab. The line item that you create on this tab will summarize the quoted value for this quote line.</span></span> 

<span data-ttu-id="1cb80-112">ליצירת פרטי שורת הצעת מחיר בחר **+ פרט חדש בשורת הצעת מחיר** ברשת המשנה **פרטים בשורת הצעת המחיר**.</span><span class="sxs-lookup"><span data-stu-id="1cb80-112">To create quote line details, select **+ New quote line detail** on the **Quote Line Details** sub-grid.</span></span> <span data-ttu-id="1cb80-113">מחוון יצירה מהירה יפתח.</span><span class="sxs-lookup"><span data-stu-id="1cb80-113">A quick create slider will open.</span></span> <span data-ttu-id="1cb80-114">את השדות הבאים בטופס **שורת הצעת המחיר**:</span><span class="sxs-lookup"><span data-stu-id="1cb80-114">The following fields on the **Quote Line** form:</span></span>

| <span data-ttu-id="1cb80-115">**שדה**</span><span class="sxs-lookup"><span data-stu-id="1cb80-115">**Field**</span></span> | <span data-ttu-id="1cb80-116">**מיקום**</span><span class="sxs-lookup"><span data-stu-id="1cb80-116">**Location**</span></span> | <span data-ttu-id="1cb80-117">**רלוונטיות, מטרה והכוונה**</span><span class="sxs-lookup"><span data-stu-id="1cb80-117">**Relevance, purpose, and guidance**</span></span> | <span data-ttu-id="1cb80-118">**השפעה במורד הזרם**</span><span class="sxs-lookup"><span data-stu-id="1cb80-118">**Downstream impact**</span></span> |
| --- | --- | --- | --- |
| <span data-ttu-id="1cb80-119">תיאור</span><span class="sxs-lookup"><span data-stu-id="1cb80-119">Description</span></span> | <span data-ttu-id="1cb80-120">יצירה מהירה</span><span class="sxs-lookup"><span data-stu-id="1cb80-120">Quick create</span></span> | <span data-ttu-id="1cb80-121">תיאור של ההערכה הספיצפית.</span><span class="sxs-lookup"><span data-stu-id="1cb80-121">A description of the specific estimate.</span></span> | <span data-ttu-id="1cb80-122">ברירת מחדל של שדה זה היא פרט שורת הצעת המחיר שקשור לעלות, שנוצר באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="1cb80-122">This field defaults to the related quote line detail for cost that is automatically created.</span></span> |
| <span data-ttu-id="1cb80-123">מחלקת עסקאות</span><span class="sxs-lookup"><span data-stu-id="1cb80-123">Transaction Class</span></span> | <span data-ttu-id="1cb80-124">יצירה מהירה</span><span class="sxs-lookup"><span data-stu-id="1cb80-124">Quick create</span></span> | <span data-ttu-id="1cb80-125">רשימה נפתחת זו מספקת את סווגי העסקאות הכלולות בכטיסיה **כללי** של שורת הצעת מחיר מבוססות פרויקט.</span><span class="sxs-lookup"><span data-stu-id="1cb80-125">This drop-down list provides the transaction classes that are included on the **General** tab of project-based quote line.</span></span>  | <span data-ttu-id="1cb80-126">ברירת מחדל של שדה זה היא פרט שורת הצעת המחיר שקשור לעלות, שנוצר באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="1cb80-126">This field defaults to the related quote line detail for cost that is automatically created.</span></span> |
| <span data-ttu-id="1cb80-127">תפקיד</span><span class="sxs-lookup"><span data-stu-id="1cb80-127">Role</span></span> | <span data-ttu-id="1cb80-128">יצירה מהירה</span><span class="sxs-lookup"><span data-stu-id="1cb80-128">Quick create</span></span> | <span data-ttu-id="1cb80-129">האדם שיבצע עבודה זו או יישא בהוצאה זו.</span><span class="sxs-lookup"><span data-stu-id="1cb80-129">The person that will perform this work or incur this expense.</span></span> | <span data-ttu-id="1cb80-130">ברירת מחדל של שדה זה היא פרט שורת הצעת המחיר שקשור לעלות, שנוצר באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="1cb80-130">This field defaults to the related quote line detail for cost that is automatically created.</span></span> |
| <span data-ttu-id="1cb80-131">קטגוריה</span><span class="sxs-lookup"><span data-stu-id="1cb80-131">Category</span></span> | <span data-ttu-id="1cb80-132">יצירה מהירה</span><span class="sxs-lookup"><span data-stu-id="1cb80-132">Quick create</span></span> | <span data-ttu-id="1cb80-133">הקטגוריה של העבודה או של ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="1cb80-133">Category of the work or expense.</span></span> | <span data-ttu-id="1cb80-134">ברירת מחדל של שדה זה היא פרט שורת הצעת המחיר שקשור לעלות, שנוצר באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="1cb80-134">This field defaults to the related quote line detail for cost that is automatically created.</span></span> |
| <span data-ttu-id="1cb80-135">תאריך התחלה</span><span class="sxs-lookup"><span data-stu-id="1cb80-135">Start Date</span></span> | <span data-ttu-id="1cb80-136">יצירה מהירה</span><span class="sxs-lookup"><span data-stu-id="1cb80-136">Quick create</span></span> | <span data-ttu-id="1cb80-137">תאריך תחילת העבודה.</span><span class="sxs-lookup"><span data-stu-id="1cb80-137">Start date of the work.</span></span> | <span data-ttu-id="1cb80-138">ברירת מחדל של שדה זה היא פרט שורת הצעת המחיר שקשור לעלות, שנוצר באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="1cb80-138">This field defaults to the related quote line detail for cost that is automatically created.</span></span> |
| <span data-ttu-id="1cb80-139">תאריך סיום</span><span class="sxs-lookup"><span data-stu-id="1cb80-139">End Date</span></span> | <span data-ttu-id="1cb80-140">יצירה מהירה</span><span class="sxs-lookup"><span data-stu-id="1cb80-140">Quick create</span></span> | <span data-ttu-id="1cb80-141">תאריך סיום העבודה.</span><span class="sxs-lookup"><span data-stu-id="1cb80-141">End date of the work.</span></span> | <span data-ttu-id="1cb80-142">ברירת מחדל של שדה זה היא פרט שורת הצעת המחיר שקשור לעלות, שנוצר באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="1cb80-142">This field defaults to the related quote line detail for cost that is automatically created.</span></span> |
| <span data-ttu-id="1cb80-143">יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="1cb80-143">Resourcing Unit</span></span> | <span data-ttu-id="1cb80-144">יצירה מהירה</span><span class="sxs-lookup"><span data-stu-id="1cb80-144">Quick create</span></span> | <span data-ttu-id="1cb80-145">יחידת הקצאת המשאבים שתשא בעלות זו ותספק את המשאב שיעבוד עליה.</span><span class="sxs-lookup"><span data-stu-id="1cb80-145">Resourcing unit that will incur this cost and provide the resource to work on it.</span></span> | <span data-ttu-id="1cb80-146">ברירת מחדל של שדה זה היא פרט שורת הצעת המחיר שקשור לעלות, שנוצר באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="1cb80-146">This field defaults to the related quote line detail for cost that is automatically created.</span></span> <span data-ttu-id="1cb80-147">שדה זה משמש גם לאחזור מחירי עלות.</span><span class="sxs-lookup"><span data-stu-id="1cb80-147">This field is also used in cost price retrieval.</span></span> |
| <span data-ttu-id="1cb80-148">לוח זמני יחידה</span><span class="sxs-lookup"><span data-stu-id="1cb80-148">Unit schedule</span></span> | <span data-ttu-id="1cb80-149">יצירה מהירה</span><span class="sxs-lookup"><span data-stu-id="1cb80-149">Quick create</span></span> | <span data-ttu-id="1cb80-150">קבוצת יחידות של העבודה או ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="1cb80-150">Unit group of the work or expense.</span></span> <span data-ttu-id="1cb80-151">יחידות שייכות ללוח זמנים של יחידה או לקבוצת יחידות.</span><span class="sxs-lookup"><span data-stu-id="1cb80-151">Units belong to a unit schedule or a group of units.</span></span> <span data-ttu-id="1cb80-152">לדוגמה, מיילים וק"מ הם יחידות השייכות לקבוצת יחידות המתארת מרחק.</span><span class="sxs-lookup"><span data-stu-id="1cb80-152">For example, Miles and KMs are units that belong to a group of units that describes distance.</span></span> | <span data-ttu-id="1cb80-153">ברירת מחדל של שדה זה היא פרט שורת הצעת המחיר שקשור לעלות, שנוצר באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="1cb80-153">This field defaults to the related quote line detail for cost that is automatically created.</span></span> |
| <span data-ttu-id="1cb80-154">יחידה</span><span class="sxs-lookup"><span data-stu-id="1cb80-154">Unit</span></span> | <span data-ttu-id="1cb80-155">יצירה מהירה</span><span class="sxs-lookup"><span data-stu-id="1cb80-155">Quick create</span></span> | <span data-ttu-id="1cb80-156">יחידה של העבודה או ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="1cb80-156">Unit of the work or expense.</span></span> | <span data-ttu-id="1cb80-157">ברירת מחדל של שדה זה היא פרט שורת הצעת המחיר שקשור לעלות, שנוצר באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="1cb80-157">This field defaults to the related quote line detail for cost that is automatically created.</span></span> |
| <span data-ttu-id="1cb80-158">כמות</span><span class="sxs-lookup"><span data-stu-id="1cb80-158">Quantity</span></span> | <span data-ttu-id="1cb80-159">יצירה מהירה</span><span class="sxs-lookup"><span data-stu-id="1cb80-159">Quick create</span></span> | <span data-ttu-id="1cb80-160">כמות העבודה או ההוצאה</span><span class="sxs-lookup"><span data-stu-id="1cb80-160">Quantity of work or expense</span></span> | <span data-ttu-id="1cb80-161">ברירת מחדל של שדה זה היא פרט שורת הצעת המחיר שקשור לעלות, שנוצר באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="1cb80-161">This field defaults to the related quote line detail for cost that is automatically created.</span></span> |
| <span data-ttu-id="1cb80-162">מחיר יחידה</span><span class="sxs-lookup"><span data-stu-id="1cb80-162">Unit price</span></span> | <span data-ttu-id="1cb80-163">יצירה מהירה</span><span class="sxs-lookup"><span data-stu-id="1cb80-163">Quick create</span></span> | <span data-ttu-id="1cb80-164">תעריף החיוב של התפקיד שמבצע את העבודה או מחיר המכירה של קטגוריית ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="1cb80-164">Bill rate of the role that is performing the work or the Sales price of the expense category.</span></span> <span data-ttu-id="1cb80-165">ברירת המחדל של שדה זה היא זמן בהתבסס על שילוב התפקיד ויחידת המשאבים במחירון הפרויקט שתקף לתאריך ההתחלה.</span><span class="sxs-lookup"><span data-stu-id="1cb80-165">This field defaults for Time based on the role and resourcing unit combination on the project price list that is effective for the start date.</span></span> <span data-ttu-id="1cb80-166">עבור הוצאות, ברירת המחדל של שדה זה נקבעת מכיוונון המחיר עבור קטגוריית העסקאות במחירון הפרויקט שתקף לתאריך ההתחלה.</span><span class="sxs-lookup"><span data-stu-id="1cb80-166">For expenses, this field defaults from the price setup for the transaction category in the project price list that is effective for the start date.</span></span> <span data-ttu-id="1cb80-167">אם שיטת התמחור עבור קטגוריית העסקה אינה מחיר ליחידה, אין ברירת מחדל ושדה זה נותר ריק.</span><span class="sxs-lookup"><span data-stu-id="1cb80-167">If the pricing method for the transaction category is not price-per-unit, there is no default, and this field is left blank.</span></span> | <span data-ttu-id="1cb80-168">תעריף העלות של התפקיד שמבצע את העבודה או העלות ליחידה של קטגוריית ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="1cb80-168">Cost rate of the role that is performing the work or the cost-per-unit of the expense category.</span></span> <span data-ttu-id="1cb80-169">ברירת מחדל של שדה זה היא זמן, המתבסס על שילוב התפקיד ויחידת המשאבים במחיר יחידת החוזה של מחירון הצעת המחיר, שתקף לתאריך ההתחלה.</span><span class="sxs-lookup"><span data-stu-id="1cb80-169">This field defaults for Time based on the role and resourcing unit combination on the price of the Contracting unit of the Quote price list that is effective for the start date.</span></span> <span data-ttu-id="1cb80-170">עבור הוצאות, ברירת המחדל של שדה זה נקבעת מכיוונון המחיר עבור קטגוריית העסקאות במחירון העלות של יחידת החוזה שתקף לתאריך ההתחלה.</span><span class="sxs-lookup"><span data-stu-id="1cb80-170">For expenses, this field defaults from the price setup for the transaction category in the cost price list of Contracting unit that is effective for the start date.</span></span> <span data-ttu-id="1cb80-171">אם שיטת התמחור עבור קטגוריית העסקה אינה מחיר ליחידה, אין ברירת מחדל ושדה זה נותר ריק.</span><span class="sxs-lookup"><span data-stu-id="1cb80-171">If the pricing method for the transaction category is not price-per-unit, there is no default and this field is left blank.</span></span> |
| <span data-ttu-id="1cb80-172">מס משוער</span><span class="sxs-lookup"><span data-stu-id="1cb80-172">Estimated Tax</span></span> | <span data-ttu-id="1cb80-173">יצירה מהירה</span><span class="sxs-lookup"><span data-stu-id="1cb80-173">Quick create</span></span> | <span data-ttu-id="1cb80-174">ניתן להזין באופן ידני את המס המשוער עבור עבודה או הוצאה זו.</span><span class="sxs-lookup"><span data-stu-id="1cb80-174">You can manually enter the estimated tax for this work or expense.</span></span> | <span data-ttu-id="1cb80-175">לשדה זה אין השפעה במורד הזרם.</span><span class="sxs-lookup"><span data-stu-id="1cb80-175">There is no downstream impact of this field.</span></span> |
| <span data-ttu-id="1cb80-176">סכום</span><span class="sxs-lookup"><span data-stu-id="1cb80-176">Amount</span></span> | <span data-ttu-id="1cb80-177">יצירה מהירה</span><span class="sxs-lookup"><span data-stu-id="1cb80-177">Quick create</span></span> | <span data-ttu-id="1cb80-178">באפשרותך להזין מידע באופן ידני לשדה זה אם השדות **כמות** ו**מחיר** נותרים ריקים.</span><span class="sxs-lookup"><span data-stu-id="1cb80-178">You can manually input information into this field if the **Quantity** and **Price** fields are left blank.</span></span> <span data-ttu-id="1cb80-179">אם שדות אלה אינם ריקים, שדה זה הופך לשדה לקריאה בלבד ומחושב כ(כמות\* מחיר יחידה) + מס.</span><span class="sxs-lookup"><span data-stu-id="1cb80-179">If these fields are not blank, this field becomes read-only and is calculated as (Quantity \* Unit price) + Tax.</span></span> | <span data-ttu-id="1cb80-180">לשדה זה אין השפעה במורד הזרם.</span><span class="sxs-lookup"><span data-stu-id="1cb80-180">There is no downstream impact of this field.</span></span> |

## <a name="update-prices-on-quote-line-details"></a><span data-ttu-id="1cb80-181">עדכן מחירים בפרטי שורת הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="1cb80-181">Update prices on quote line details</span></span>

<span data-ttu-id="1cb80-182">אם שינית מחירים במחירון הפרויקט המצורף להצעת המחיר, או במחירון העלות של היחידת החוזה, באפשרותך לבחור **חישוב מחדש** בדף **הצעת המחיר**, כדי לרענן את המחירים בפרטים הבודדים בשורת הצעת המחיר כדי לשקף שינוי זה.</span><span class="sxs-lookup"><span data-stu-id="1cb80-182">If you have changed prices on the project price list that is attached to the quote, or on cost price list of the contracting unit, you can select **Recalculate** on the **Quote** page, to refresh the prices on the individual quote line details to reflect this change.</span></span> <span data-ttu-id="1cb80-183">כשבוחרים ב**חישוב מחדש**, מופיעה אזהרה המודיעה לך כי המחירים בפרטי שורת הצעת המחיר עבור כל שורות הצעת המחיר בהצעת מחיר זו יאופסו.</span><span class="sxs-lookup"><span data-stu-id="1cb80-183">When you select **Recalculate**, a warning occurs that informs you that prices on quote line details for all quote lines on this quote will be reset.</span></span> <span data-ttu-id="1cb80-184">בחר **כן**, כדי לרענן מחירים הן עבור פרטי שורת המכירות והן עבור פרטי שורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="1cb80-184">Select **Yes**, to refresh prices for both sales and cost quote line details.</span></span>

## <a name="access-quote-line-details-for-cost"></a><span data-ttu-id="1cb80-185">גישה לפרטי שורת הצעת מחיר לקבלת עלות</span><span class="sxs-lookup"><span data-stu-id="1cb80-185">Access quote line details for cost</span></span>

<span data-ttu-id="1cb80-186">על הכרטיסיה **פרטים בשורת הצעת מחיר**, בחר שורה ברשת כדי להפוך פעולות מסוימות בסרגל הכלים של רשת המשנה לזמינות.</span><span class="sxs-lookup"><span data-stu-id="1cb80-186">On the **Quote Line Details** tab, select a row in the grid to enable some actions on the toolbar of the sub-grid.</span></span> <span data-ttu-id="1cb80-187">הפעולה הראשונה בסרגל הכלים של רשת המשנה שהופכת לזמינה כאשר נבחר פרט בשורת הצעת מחיר היא **פתח פרטי עלות**.</span><span class="sxs-lookup"><span data-stu-id="1cb80-187">The first action on the sub-grid tool bar when a quote line detail is selected is **Open Cost Detail**.</span></span> <span data-ttu-id="1cb80-188">בחר **פתח פרטי עלות** כדי לראות את שיעור העלות והסכום הקשורים לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="1cb80-188">Select **Open Cost Detail** to see the related cost rate and amount for this quote line.</span></span>

> [!NOTE]
> <span data-ttu-id="1cb80-189">שינוי של ערכי יחידת הקצאת המשאבים, הכמות, התאריכים, התפקיד או הקטגוריה בפרטים שבשורת הצעת המחיר לעלות ישנה את הערכים המתאימים בפרטים בשורת הצעת המחיר למכירות.</span><span class="sxs-lookup"><span data-stu-id="1cb80-189">Changing the resourcing unit, quantity, dates, role, or category values on the quote line detail for cost will change the corresponding values on the quote line details for sales.</span></span>
## <a name="currency-on-quote-line-details-for-cost-and-sales"></a><span data-ttu-id="1cb80-190">המטבע בפרטים שבשורת הצעת מחיר עבור עלות ומכירות</span><span class="sxs-lookup"><span data-stu-id="1cb80-190">Currency on quote line details for cost and sales</span></span>

<span data-ttu-id="1cb80-191">המטבע בפרטים שבשורת הצעת מחיר עבור מכירות נקבע כברירות מחדל ממחירון הפרויקט שתקף לתאריך ההתחלה של הפרט בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="1cb80-191">Currency on the quote line detail for sales defaults from the project price list that is effective for the start date of the quote line detail.</span></span>

<span data-ttu-id="1cb80-192">המטבע שבפרטים בשורת הצעת מחיר עבור עלות נקבע כברירות מחדל ממחירון יחידת החוזה של הצעת המחיר, שתקף לתאריך ההתחלה של הפרט בשורת הצעת המחיר עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="1cb80-192">Currency on the quote line detail for cost defaults from the price list of the contracting unit of the quote that is effective for the start date of the quote line detail for cost.</span></span>

<span data-ttu-id="1cb80-193">חישובי רווחיות ממירים את הסכום שבפרטים בשורת הצעת מחיר עבור עלות ומכירות למטבע הבסיס של הסביבה, כדי לדווח על שולי הרווח המשוערים הכוללים על הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="1cb80-193">Profitability calculations convert the amount on quote line details for cost and sales into the base currency of the environment to report the overall estimated margin on the quote.</span></span>

<span data-ttu-id="1cb80-194">דבר זה עלול לגרום לשגיאות בעיגול מטבעות ולשינויים בשוליים בגלל היעדר שערי חליפין של תאריכי תוקף.</span><span class="sxs-lookup"><span data-stu-id="1cb80-194">This could result in currency rounding errors and changing margins because of the lack of date effective exchange rates.</span></span> <span data-ttu-id="1cb80-195">השתמש בחישובים אלה בהצעות מחיר לפרויקטים רק כאומדנים ולא כדיווח סטטוטורי או אחר הדורש דיוק גבוה יותר של עיגול ומודעות לתוקף התאריכים עובר שערי החליפין.</span><span class="sxs-lookup"><span data-stu-id="1cb80-195">Use these calculations on Project quotes only as approximations and not actual statutory or other reporting that requires higher precision of rounding and awareness of date effectivity for exchange rates.</span></span>