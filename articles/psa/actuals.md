---
title: מבט כולל על נתונים בפועל
description: נושא זו מספק מידע אודות נתונים בפועל של פרוייקט.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 08/03/2020
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
ms.openlocfilehash: cf9e36c99790b77f0ed6490f49b4ebeb043bcdf6
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4129769"
---
# <a name="actuals-overview"></a><span data-ttu-id="77034-103">מבט כולל על נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="77034-103">Actuals overview</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="77034-104">נתונים בפועל הם כמות העבודה שהושלמה בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="77034-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="77034-105">ניתן לעקוב אחר נתונים בפועל בחזרה למסמכי המקור שלהם.</span><span class="sxs-lookup"><span data-stu-id="77034-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="77034-106">מסמכי מקור אלה כוללים ערכי זמן, הוצאות ויומן וכן חשבוניות.</span><span class="sxs-lookup"><span data-stu-id="77034-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![כיצד ניתן לשייך נתונים בפועל של פרוייקט למסמכי מקור](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="77034-108">שליחת ערך זמן</span><span class="sxs-lookup"><span data-stu-id="77034-108">Submitting a time entry</span></span>

<span data-ttu-id="77034-109">ב- PSA, כאשר ערך זמן נשלח עבור פרוייקט הממופה לסעיף חוזה של זמן וחומרים, נוצרות שתי שורות יומן.</span><span class="sxs-lookup"><span data-stu-id="77034-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="77034-110">שורה אחת היא עבור עלות, והשורה השנייה היא עבור מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="77034-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="77034-111">כאשר ערך זמן נשלח עבור פרוייקט הממופה לסעיף חוזה של מחיר קבוע, שורת יומן נוצרת רק עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="77034-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="77034-112">הלוגיקה להזנת מחירי ברירת מחדל טמונה בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="77034-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="77034-113">כל ערכי השדות מערך זמן מועתקים לשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="77034-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="77034-114">שדות אלה כוללים את תאריך העסקה, את סעיף החוזה שאליו ממופה הפרוייקט ואת תוצאת המטבע במחירון המתאים.</span><span class="sxs-lookup"><span data-stu-id="77034-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="77034-115">השדות המשפיעים על מחירי ברירת המחדל, כגון **תפקיד** ו **יחידה ארגונית**, גורמים להזנת מחיר מתאים כברירת מחדל בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="77034-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="77034-116">אם אתה מוסיף שדה מותאם אישית בערך הזמן, וברצונך שערך השדה יופץ לנתונים בפועל, עליך ליצור את השדה בישות 'נתונים בפועל' ולהשתמש במיפויי שדה כדי להעתיק את השדה מערך הזמן לנתון בפועל.</span><span class="sxs-lookup"><span data-stu-id="77034-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="77034-117">שליחת ערך הוצאה</span><span class="sxs-lookup"><span data-stu-id="77034-117">Submitting an expense entry</span></span>

<span data-ttu-id="77034-118">ב- PSA, כאשר ערך הוצאה נשלח עבור פרוייקט הממופה לסעיף חוזה של זמן וחומרים, נוצרות שתי שורות יומן.</span><span class="sxs-lookup"><span data-stu-id="77034-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="77034-119">שורה אחת היא עבור עלות, והשורה השנייה היא עבור מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="77034-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="77034-120">כאשר ערך הוצאה נשלח עבור פרוייקט הממופה לסעיף חוזה של מחיר קבוע, שורת יומן נוצרת רק עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="77034-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="77034-121">הלוגיקה להזנת מחירי ברירת מחדל עבור הוצאות מבוססת על קטגוריית ההוצאה שנבחרה בדף **ערך הוצאה**.</span><span class="sxs-lookup"><span data-stu-id="77034-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="77034-122">תאריך העסקה, סעיף החוזה שאליו ממופה הפרוייקט והמטבע משמשים כולם כדי לקבוע את המחירון המתאים.</span><span class="sxs-lookup"><span data-stu-id="77034-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="77034-123">עם זאת, עבור המחיר עצמו, הסכום שהמשתמש הזין מוגדר ישירות בשורות היומן של ההוצאות הקשורות עבור עלות ומכירות כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="77034-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="77034-124">בגירסה הנוכחית של PSA, ערך מבוסס-קטגוריה של מחירי ברירת מחדל ליחידה בערכי הוצאה אינו זמין.</span><span class="sxs-lookup"><span data-stu-id="77034-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-entry-journals-to-record-costs"></a><span data-ttu-id="77034-125">שימוש בפקודות יומן לתיעוד עלויות</span><span class="sxs-lookup"><span data-stu-id="77034-125">Using Entry journals to record costs</span></span>

<span data-ttu-id="77034-126">ב- PSA, פקודות יומן מאפשרות לך לתעד עלות או הכנסות במחלקות החומר, התשלום, הזמן, ההוצאה או עסקת המס.</span><span class="sxs-lookup"><span data-stu-id="77034-126">In PSA, Entry journals let you record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="77034-127">יומן כולל כותרת, שורות ופעולת **אישור**.</span><span class="sxs-lookup"><span data-stu-id="77034-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="77034-128">להלן מספר תרחישים שבהם אתה כדאי להשתמש ביומן:</span><span class="sxs-lookup"><span data-stu-id="77034-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="77034-129">עליך לתעד עלויות בפועל של חומרים ומכירות בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="77034-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="77034-130">עליך להעביר נתונים בפועל של עסקה ממערכת אחרת ל- PSA.</span><span class="sxs-lookup"><span data-stu-id="77034-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="77034-131">עליך לתעד עלויות שהתרחשו במערכת אחרת, כגון עלויות רכישה או מסירה לקבלן משנה.</span><span class="sxs-lookup"><span data-stu-id="77034-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="77034-132">השימוש בפקודת יומן ליצירת עובדות צריך להיעשות רק על ידי משתמש שמודע לחלוטין להשפעה החשבונאית שיש לעובדים על הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="77034-132">Using Entry journals to create actuals should be done only by a user who is fully aware of the accounting impact the Actuals have on the project.</span></span> <span data-ttu-id="77034-133">הסיבה לכך היא שהיישום אינו מאמת את סוג שורת היומן, או את התמחור הקשור שמוזן בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="77034-133">This is because the application does not validate the journal line type, or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="77034-134">בגלל ההשפעה של סוג יומן זה, יש לנקוט זהירות מספקת מבחינת מי שמקבל גישה ליצירת פקודות יומן.</span><span class="sxs-lookup"><span data-stu-id="77034-134">Because of the impact of this journal type, exercise adequate caution in who is given access to create Entry journals.</span></span>     


## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="77034-135">תיעוד נתונים בפועל בהתבסס על אירועי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-135">Recording actuals based on project events</span></span>

<span data-ttu-id="77034-136">PSA מתעד את העסקות הפיננסיות המתרחשות במהלך פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="77034-136">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="77034-137">עסקאות אלה מתועדות כ **נתונים בפועל**.</span><span class="sxs-lookup"><span data-stu-id="77034-137">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="77034-138">הטבלאות הבאות מציגות את הסוגים השונים של נתונים בפועל שנוצרים, בהתאם לשאלה אם הפרוייקט הוא פרוייקט של זמן וחומרים פרוייקט במחיר קבוע, פרוייקט שנמצא בשלב קדם המכירות או פרוייקט פנימי.</span><span class="sxs-lookup"><span data-stu-id="77034-138">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="77034-139">**המשאב משתייך לאותה יחידה ארגונית כשל יחידת החוזה של הפרוייקט**</span><span class="sxs-lookup"><span data-stu-id="77034-139">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="77034-140">אירוע</span><span class="sxs-lookup"><span data-stu-id="77034-140">Event</span></span></th>
<th colspan="4"><span data-ttu-id="77034-141">פרוייקט לחיוב או פרוייקט שנמכר</span><span class="sxs-lookup"><span data-stu-id="77034-141">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="77034-142">פרוייקט בשלב הקדם-מכירות</span><span class="sxs-lookup"><span data-stu-id="77034-142">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="77034-143">פרוייקט פנימי</span><span class="sxs-lookup"><span data-stu-id="77034-143">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="77034-144">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="77034-144">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="77034-145">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="77034-145">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="77034-146">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="77034-146">Actuals</span></span></th>
<th><span data-ttu-id="77034-147">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="77034-147">Transaction currency</span></span></th>
<th><span data-ttu-id="77034-148">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="77034-148">Fixed price</span></span></th>
<th><span data-ttu-id="77034-149">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="77034-149">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="77034-150">ערך זמן נוצר.</span><span class="sxs-lookup"><span data-stu-id="77034-150">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="77034-151">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="77034-151">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-152">ערך זמן נשלח.</span><span class="sxs-lookup"><span data-stu-id="77034-152">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="77034-153">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="77034-153">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="77034-154">הזמן מאושר, ואין שינוי או עלייה בשעות לחיוב במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="77034-154">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="77034-155">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="77034-155">Cost actual</span></span></td>
<td><span data-ttu-id="77034-156">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="77034-156">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="77034-157">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="77034-157">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="77034-158">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="77034-158">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="77034-159">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="77034-159">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="77034-160">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="77034-160">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-161">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="77034-161">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="77034-162">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-162">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="77034-163">הזמן מאושר, וירידה בשעות לחיוב מתרחשת במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="77034-163">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="77034-164">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="77034-164">Cost actual</span></span></td>
<td><span data-ttu-id="77034-165">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="77034-165">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="77034-166">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="77034-166">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="77034-167">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="77034-167">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="77034-168">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="77034-168">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="77034-169">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="77034-169">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-170">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="77034-170">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="77034-171">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-171">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-172">נתון בפועל של מכירות שלא חויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="77034-172">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="77034-173">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-173">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="77034-174">חשבונית מאושרת, ואין שינוי או עלייה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="77034-174">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="77034-175">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="77034-175">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="77034-176">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-176">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="77034-177">מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="77034-177">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="77034-178">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-178">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="77034-179">לא ישים</span><span class="sxs-lookup"><span data-stu-id="77034-179">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="77034-180">לא ישים</span><span class="sxs-lookup"><span data-stu-id="77034-180">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-181">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="77034-181">Billed sales</span></span></td>
<td><span data-ttu-id="77034-182">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-182">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="77034-183">חשבונית מאושרת, ומתרחשת ירידה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="77034-183">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="77034-184">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="77034-184">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="77034-185">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-185">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="77034-186">לא ישים</span><span class="sxs-lookup"><span data-stu-id="77034-186">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="77034-187">לא ישים</span><span class="sxs-lookup"><span data-stu-id="77034-187">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="77034-188">לא ישים</span><span class="sxs-lookup"><span data-stu-id="77034-188">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="77034-189">לא ישים</span><span class="sxs-lookup"><span data-stu-id="77034-189">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-190">מכירות שחויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="77034-190">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="77034-191">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-191">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-192">מכירות שחויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="77034-192">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="77034-193">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-193">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="77034-194">החשבונית מתוקנת כדי להגדיל את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="77034-194">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="77034-195">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="77034-195">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="77034-196">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-196">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="77034-197">ביטול מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="77034-197">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="77034-198">שינוי במצב אבן דרך ממצב <strong>הוגשה חשבונית</strong> למצב <strong>מוכן להפקת חשבונית</strong></span><span class="sxs-lookup"><span data-stu-id="77034-198">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="77034-199">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-199">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="77034-200">לא ישים</span><span class="sxs-lookup"><span data-stu-id="77034-200">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="77034-201">לא ישים</span><span class="sxs-lookup"><span data-stu-id="77034-201">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-202">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="77034-202">Billed sales</span></span></td>
<td><span data-ttu-id="77034-203">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-203">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="77034-204">החשבונית מתוקנת כדי להקטין את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="77034-204">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="77034-205">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="77034-205">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="77034-206">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-206">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-207">מכירות שחויבו עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="77034-207">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="77034-208">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-208">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-209">מכירות שלא חויבו - ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="77034-209">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="77034-210">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-210">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="77034-211">**המשאב משתייך ליחידה ארגונית השונה מיחידת החוזה של הפרוייקט**</span><span class="sxs-lookup"><span data-stu-id="77034-211">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="77034-212">אירוע</span><span class="sxs-lookup"><span data-stu-id="77034-212">Event</span></span></th>
<th colspan="4"><span data-ttu-id="77034-213">פרוייקט לחיוב או פרוייקט שנמכר</span><span class="sxs-lookup"><span data-stu-id="77034-213">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="77034-214">פרוייקט בשלב הקדם-מכירות</span><span class="sxs-lookup"><span data-stu-id="77034-214">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="77034-215">פרוייקט פנימי</span><span class="sxs-lookup"><span data-stu-id="77034-215">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="77034-216">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="77034-216">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="77034-217">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="77034-217">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="77034-218">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="77034-218">Actuals</span></span></th>
<th><span data-ttu-id="77034-219">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="77034-219">Transaction currency</span></span></th>
<th><span data-ttu-id="77034-220">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="77034-220">Fixed price</span></span></th>
<th><span data-ttu-id="77034-221">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="77034-221">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="77034-222">ערך זמן נוצר.</span><span class="sxs-lookup"><span data-stu-id="77034-222">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="77034-223">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="77034-223">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-224">ערך זמן נשלח.</span><span class="sxs-lookup"><span data-stu-id="77034-224">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="77034-225">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="77034-225">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="77034-226">הזמן מאושר, ואין שינוי או עלייה בשעות לחיוב במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="77034-226">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="77034-227">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="77034-227">Cost actual</span></span></td>
<td><span data-ttu-id="77034-228">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="77034-228">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="77034-229">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="77034-229">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="77034-230">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="77034-230">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="77034-231">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="77034-231">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="77034-232">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="77034-232">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-233">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="77034-233">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="77034-234">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-235">עלות יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="77034-235">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="77034-236">מטבע של יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="77034-236">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-237">מכירות בין-ארגוניות</span><span class="sxs-lookup"><span data-stu-id="77034-237">Interorganizational sales</span></span></td>
<td><span data-ttu-id="77034-238">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="77034-238">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="77034-239">הזמן מאושר, וירידה בשעות לחיוב מתרחשת במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="77034-239">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="77034-240">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="77034-240">Cost actual</span></span></td>
<td><span data-ttu-id="77034-241">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="77034-241">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="77034-242">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="77034-242">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="77034-243">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="77034-243">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="77034-244">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="77034-244">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="77034-245">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="77034-245">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-246">עלות יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="77034-246">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="77034-247">מטבע של יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="77034-247">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-248">מכירות בין-ארגוניות</span><span class="sxs-lookup"><span data-stu-id="77034-248">Interorganizational sales</span></span></td>
<td><span data-ttu-id="77034-249">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="77034-249">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-250">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="77034-250">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="77034-251">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-251">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-252">נתון בפועל של מכירות שלא חויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="77034-252">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="77034-253">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-253">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="77034-254">חשבונית מאושרת, ואין שינוי או עלייה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="77034-254">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="77034-255">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="77034-255">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="77034-256">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-256">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="77034-257">מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="77034-257">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="77034-258">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-258">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="77034-259">לא ישים</span><span class="sxs-lookup"><span data-stu-id="77034-259">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="77034-260">לא ישים</span><span class="sxs-lookup"><span data-stu-id="77034-260">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-261">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="77034-261">Billed sales</span></span></td>
<td><span data-ttu-id="77034-262">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-262">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="77034-263">חשבונית מאושרת, ומתרחשת ירידה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="77034-263">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="77034-264">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="77034-264">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="77034-265">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-265">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="77034-266">לא ישים</span><span class="sxs-lookup"><span data-stu-id="77034-266">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="77034-267">לא ישים</span><span class="sxs-lookup"><span data-stu-id="77034-267">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="77034-268">לא ישים</span><span class="sxs-lookup"><span data-stu-id="77034-268">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="77034-269">לא ישים</span><span class="sxs-lookup"><span data-stu-id="77034-269">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-270">מכירות שחויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="77034-270">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="77034-271">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-271">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-272">מכירות שחויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="77034-272">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="77034-273">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-273">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="77034-274">החשבונית מתוקנת כדי להגדיל את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="77034-274">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="77034-275">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="77034-275">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="77034-276">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-276">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="77034-277">ביטול מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="77034-277">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="77034-278">שינוי במצב אבן דרך ממצב <strong>הוגשה חשבונית</strong> למצב <strong>מוכן להפקת חשבונית</strong></span><span class="sxs-lookup"><span data-stu-id="77034-278">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="77034-279">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-279">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="77034-280">לא ישים</span><span class="sxs-lookup"><span data-stu-id="77034-280">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="77034-281">לא ישים</span><span class="sxs-lookup"><span data-stu-id="77034-281">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-282">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="77034-282">Billed sales</span></span></td>
<td><span data-ttu-id="77034-283">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-283">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="77034-284">החשבונית מתוקנת כדי להקטין את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="77034-284">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="77034-285">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="77034-285">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="77034-286">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-286">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-287">מכירות שחויבו עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="77034-287">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="77034-288">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-288">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="77034-289">מכירות שלא חויבו - ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="77034-289">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="77034-290">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77034-290">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
