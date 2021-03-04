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
ms.openlocfilehash: 63ad6544f0ec0a893aebd8d81f3ee895e51c294e
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5146124"
---
# <a name="actuals-overview"></a><span data-ttu-id="7c454-103">מבט כולל על נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="7c454-103">Actuals overview</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="7c454-104">נתונים בפועל הם כמות העבודה שהושלמה בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="7c454-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="7c454-105">ניתן לעקוב אחר נתונים בפועל בחזרה למסמכי המקור שלהם.</span><span class="sxs-lookup"><span data-stu-id="7c454-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="7c454-106">מסמכי מקור אלה כוללים ערכי זמן, הוצאות ויומן וכן חשבוניות.</span><span class="sxs-lookup"><span data-stu-id="7c454-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![כיצד ניתן לשייך נתונים בפועל של פרוייקט למסמכי מקור](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="7c454-108">שליחת ערך זמן</span><span class="sxs-lookup"><span data-stu-id="7c454-108">Submitting a time entry</span></span>

<span data-ttu-id="7c454-109">ב- PSA, כאשר ערך זמן נשלח עבור פרוייקט הממופה לסעיף חוזה של זמן וחומרים, נוצרות שתי שורות יומן.</span><span class="sxs-lookup"><span data-stu-id="7c454-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="7c454-110">שורה אחת היא עבור עלות, והשורה השנייה היא עבור מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="7c454-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="7c454-111">כאשר ערך זמן נשלח עבור פרוייקט הממופה לסעיף חוזה של מחיר קבוע, שורת יומן נוצרת רק עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="7c454-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="7c454-112">הלוגיקה להזנת מחירי ברירת מחדל טמונה בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="7c454-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="7c454-113">כל ערכי השדות מערך זמן מועתקים לשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="7c454-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="7c454-114">שדות אלה כוללים את תאריך העסקה, את סעיף החוזה שאליו ממופה הפרוייקט ואת תוצאת המטבע במחירון המתאים.</span><span class="sxs-lookup"><span data-stu-id="7c454-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="7c454-115">השדות המשפיעים על מחירי ברירת המחדל, כגון **תפקיד** ו **יחידה ארגונית**, גורמים להזנת מחיר מתאים כברירת מחדל בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="7c454-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="7c454-116">אם אתה מוסיף שדה מותאם אישית בערך הזמן, וברצונך שערך השדה יופץ לנתונים בפועל, עליך ליצור את השדה בישות 'נתונים בפועל' ולהשתמש במיפויי שדה כדי להעתיק את השדה מערך הזמן לנתון בפועל.</span><span class="sxs-lookup"><span data-stu-id="7c454-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="7c454-117">שליחת ערך הוצאה</span><span class="sxs-lookup"><span data-stu-id="7c454-117">Submitting an expense entry</span></span>

<span data-ttu-id="7c454-118">ב- PSA, כאשר ערך הוצאה נשלח עבור פרוייקט הממופה לסעיף חוזה של זמן וחומרים, נוצרות שתי שורות יומן.</span><span class="sxs-lookup"><span data-stu-id="7c454-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="7c454-119">שורה אחת היא עבור עלות, והשורה השנייה היא עבור מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="7c454-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="7c454-120">כאשר ערך הוצאה נשלח עבור פרוייקט הממופה לסעיף חוזה של מחיר קבוע, שורת יומן נוצרת רק עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="7c454-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="7c454-121">הלוגיקה להזנת מחירי ברירת מחדל עבור הוצאות מבוססת על קטגוריית ההוצאה שנבחרה בדף **ערך הוצאה**.</span><span class="sxs-lookup"><span data-stu-id="7c454-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="7c454-122">תאריך העסקה, סעיף החוזה שאליו ממופה הפרוייקט והמטבע משמשים כולם כדי לקבוע את המחירון המתאים.</span><span class="sxs-lookup"><span data-stu-id="7c454-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="7c454-123">עם זאת, עבור המחיר עצמו, הסכום שהמשתמש הזין מוגדר ישירות בשורות היומן של ההוצאות הקשורות עבור עלות ומכירות כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="7c454-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="7c454-124">בגירסה הנוכחית של PSA, ערך מבוסס-קטגוריה של מחירי ברירת מחדל ליחידה בערכי הוצאה אינו זמין.</span><span class="sxs-lookup"><span data-stu-id="7c454-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-entry-journals-to-record-costs"></a><span data-ttu-id="7c454-125">שימוש בפקודות יומן לתיעוד עלויות</span><span class="sxs-lookup"><span data-stu-id="7c454-125">Using Entry journals to record costs</span></span>

<span data-ttu-id="7c454-126">ב- PSA, פקודות יומן מאפשרות לך לתעד עלות או הכנסות במחלקות החומר, התשלום, הזמן, ההוצאה או עסקת המס.</span><span class="sxs-lookup"><span data-stu-id="7c454-126">In PSA, Entry journals let you record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="7c454-127">יומן כולל כותרת, שורות ופעולת **אישור**.</span><span class="sxs-lookup"><span data-stu-id="7c454-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="7c454-128">להלן מספר תרחישים שבהם אתה כדאי להשתמש ביומן:</span><span class="sxs-lookup"><span data-stu-id="7c454-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="7c454-129">עליך לתעד עלויות בפועל של חומרים ומכירות בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="7c454-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="7c454-130">עליך להעביר נתונים בפועל של עסקה ממערכת אחרת ל- PSA.</span><span class="sxs-lookup"><span data-stu-id="7c454-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="7c454-131">עליך לתעד עלויות שהתרחשו במערכת אחרת, כגון עלויות רכישה או מסירה לקבלן משנה.</span><span class="sxs-lookup"><span data-stu-id="7c454-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7c454-132">השימוש בפקודת יומן ליצירת עובדות צריך להיעשות רק על ידי משתמש שמודע לחלוטין להשפעה החשבונאית שיש לעובדים על הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="7c454-132">Using Entry journals to create actuals should be done only by a user who is fully aware of the accounting impact the Actuals have on the project.</span></span> <span data-ttu-id="7c454-133">הסיבה לכך היא שהיישום אינו מאמת את סוג שורת היומן, או את התמחור הקשור שמוזן בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="7c454-133">This is because the application does not validate the journal line type, or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="7c454-134">בגלל ההשפעה של סוג יומן זה, יש לנקוט זהירות מספקת מבחינת מי שמקבל גישה ליצירת פקודות יומן.</span><span class="sxs-lookup"><span data-stu-id="7c454-134">Because of the impact of this journal type, exercise adequate caution in who is given access to create Entry journals.</span></span>     


## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="7c454-135">תיעוד נתונים בפועל בהתבסס על אירועי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-135">Recording actuals based on project events</span></span>

<span data-ttu-id="7c454-136">PSA מתעד את העסקות הפיננסיות המתרחשות במהלך פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="7c454-136">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="7c454-137">עסקאות אלה מתועדות כ **נתונים בפועל**.</span><span class="sxs-lookup"><span data-stu-id="7c454-137">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="7c454-138">הטבלאות הבאות מציגות את הסוגים השונים של נתונים בפועל שנוצרים, בהתאם לשאלה אם הפרוייקט הוא פרוייקט של זמן וחומרים פרוייקט במחיר קבוע, פרוייקט שנמצא בשלב קדם המכירות או פרוייקט פנימי.</span><span class="sxs-lookup"><span data-stu-id="7c454-138">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="7c454-139">**המשאב משתייך לאותה יחידה ארגונית כשל יחידת החוזה של הפרוייקט**</span><span class="sxs-lookup"><span data-stu-id="7c454-139">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="7c454-140">אירוע</span><span class="sxs-lookup"><span data-stu-id="7c454-140">Event</span></span></th>
<th colspan="4"><span data-ttu-id="7c454-141">פרוייקט לחיוב או פרוייקט שנמכר</span><span class="sxs-lookup"><span data-stu-id="7c454-141">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="7c454-142">פרוייקט בשלב הקדם-מכירות</span><span class="sxs-lookup"><span data-stu-id="7c454-142">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="7c454-143">פרוייקט פנימי</span><span class="sxs-lookup"><span data-stu-id="7c454-143">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="7c454-144">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="7c454-144">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="7c454-145">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="7c454-145">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="7c454-146">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="7c454-146">Actuals</span></span></th>
<th><span data-ttu-id="7c454-147">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="7c454-147">Transaction currency</span></span></th>
<th><span data-ttu-id="7c454-148">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="7c454-148">Fixed price</span></span></th>
<th><span data-ttu-id="7c454-149">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="7c454-149">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="7c454-150">ערך זמן נוצר.</span><span class="sxs-lookup"><span data-stu-id="7c454-150">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="7c454-151">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="7c454-151">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-152">ערך זמן נשלח.</span><span class="sxs-lookup"><span data-stu-id="7c454-152">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="7c454-153">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="7c454-153">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7c454-154">הזמן מאושר, ואין שינוי או עלייה בשעות לחיוב במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="7c454-154">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="7c454-155">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="7c454-155">Cost actual</span></span></td>
<td><span data-ttu-id="7c454-156">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="7c454-156">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7c454-157">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="7c454-157">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="7c454-158">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="7c454-158">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="7c454-159">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="7c454-159">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="7c454-160">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="7c454-160">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-161">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="7c454-161">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="7c454-162">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-162">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7c454-163">הזמן מאושר, וירידה בשעות לחיוב מתרחשת במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="7c454-163">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="7c454-164">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="7c454-164">Cost actual</span></span></td>
<td><span data-ttu-id="7c454-165">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="7c454-165">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="7c454-166">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="7c454-166">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="7c454-167">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="7c454-167">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="7c454-168">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="7c454-168">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="7c454-169">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="7c454-169">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-170">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="7c454-170">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="7c454-171">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-171">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-172">נתון בפועל של מכירות שלא חויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="7c454-172">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="7c454-173">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-173">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7c454-174">חשבונית מאושרת, ואין שינוי או עלייה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="7c454-174">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="7c454-175">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="7c454-175">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="7c454-176">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-176">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7c454-177">מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="7c454-177">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="7c454-178">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-178">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7c454-179">לא ישים</span><span class="sxs-lookup"><span data-stu-id="7c454-179">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="7c454-180">לא ישים</span><span class="sxs-lookup"><span data-stu-id="7c454-180">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-181">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="7c454-181">Billed sales</span></span></td>
<td><span data-ttu-id="7c454-182">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-182">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7c454-183">חשבונית מאושרת, ומתרחשת ירידה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="7c454-183">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="7c454-184">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="7c454-184">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="7c454-185">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-185">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="7c454-186">לא ישים</span><span class="sxs-lookup"><span data-stu-id="7c454-186">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7c454-187">לא ישים</span><span class="sxs-lookup"><span data-stu-id="7c454-187">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7c454-188">לא ישים</span><span class="sxs-lookup"><span data-stu-id="7c454-188">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7c454-189">לא ישים</span><span class="sxs-lookup"><span data-stu-id="7c454-189">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-190">מכירות שחויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="7c454-190">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="7c454-191">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-191">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-192">מכירות שחויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="7c454-192">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="7c454-193">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-193">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7c454-194">החשבונית מתוקנת כדי להגדיל את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="7c454-194">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="7c454-195">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="7c454-195">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="7c454-196">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-196">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="7c454-197">ביטול מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="7c454-197">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="7c454-198">שינוי במצב אבן דרך ממצב <strong>הוגשה חשבונית</strong> למצב <strong>מוכן להפקת חשבונית</strong></span><span class="sxs-lookup"><span data-stu-id="7c454-198">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="7c454-199">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-199">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="7c454-200">לא ישים</span><span class="sxs-lookup"><span data-stu-id="7c454-200">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="7c454-201">לא ישים</span><span class="sxs-lookup"><span data-stu-id="7c454-201">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-202">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="7c454-202">Billed sales</span></span></td>
<td><span data-ttu-id="7c454-203">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-203">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7c454-204">החשבונית מתוקנת כדי להקטין את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="7c454-204">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="7c454-205">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="7c454-205">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="7c454-206">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-206">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-207">מכירות שחויבו עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="7c454-207">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="7c454-208">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-208">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-209">מכירות שלא חויבו - ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="7c454-209">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="7c454-210">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-210">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="7c454-211">**המשאב משתייך ליחידה ארגונית השונה מיחידת החוזה של הפרוייקט**</span><span class="sxs-lookup"><span data-stu-id="7c454-211">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="7c454-212">אירוע</span><span class="sxs-lookup"><span data-stu-id="7c454-212">Event</span></span></th>
<th colspan="4"><span data-ttu-id="7c454-213">פרוייקט לחיוב או פרוייקט שנמכר</span><span class="sxs-lookup"><span data-stu-id="7c454-213">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="7c454-214">פרוייקט בשלב הקדם-מכירות</span><span class="sxs-lookup"><span data-stu-id="7c454-214">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="7c454-215">פרוייקט פנימי</span><span class="sxs-lookup"><span data-stu-id="7c454-215">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="7c454-216">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="7c454-216">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="7c454-217">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="7c454-217">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="7c454-218">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="7c454-218">Actuals</span></span></th>
<th><span data-ttu-id="7c454-219">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="7c454-219">Transaction currency</span></span></th>
<th><span data-ttu-id="7c454-220">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="7c454-220">Fixed price</span></span></th>
<th><span data-ttu-id="7c454-221">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="7c454-221">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="7c454-222">ערך זמן נוצר.</span><span class="sxs-lookup"><span data-stu-id="7c454-222">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="7c454-223">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="7c454-223">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-224">ערך זמן נשלח.</span><span class="sxs-lookup"><span data-stu-id="7c454-224">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="7c454-225">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="7c454-225">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="7c454-226">הזמן מאושר, ואין שינוי או עלייה בשעות לחיוב במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="7c454-226">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="7c454-227">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="7c454-227">Cost actual</span></span></td>
<td><span data-ttu-id="7c454-228">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="7c454-228">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="7c454-229">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="7c454-229">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="7c454-230">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="7c454-230">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="7c454-231">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="7c454-231">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="7c454-232">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="7c454-232">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-233">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="7c454-233">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="7c454-234">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-235">עלות יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="7c454-235">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="7c454-236">מטבע של יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="7c454-236">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-237">מכירות בין-ארגוניות</span><span class="sxs-lookup"><span data-stu-id="7c454-237">Interorganizational sales</span></span></td>
<td><span data-ttu-id="7c454-238">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="7c454-238">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="7c454-239">הזמן מאושר, וירידה בשעות לחיוב מתרחשת במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="7c454-239">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="7c454-240">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="7c454-240">Cost actual</span></span></td>
<td><span data-ttu-id="7c454-241">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="7c454-241">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="7c454-242">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="7c454-242">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="7c454-243">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="7c454-243">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="7c454-244">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="7c454-244">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="7c454-245">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="7c454-245">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-246">עלות יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="7c454-246">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="7c454-247">מטבע של יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="7c454-247">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-248">מכירות בין-ארגוניות</span><span class="sxs-lookup"><span data-stu-id="7c454-248">Interorganizational sales</span></span></td>
<td><span data-ttu-id="7c454-249">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="7c454-249">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-250">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="7c454-250">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="7c454-251">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-251">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-252">נתון בפועל של מכירות שלא חויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="7c454-252">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="7c454-253">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-253">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7c454-254">חשבונית מאושרת, ואין שינוי או עלייה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="7c454-254">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="7c454-255">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="7c454-255">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="7c454-256">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-256">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7c454-257">מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="7c454-257">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="7c454-258">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-258">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7c454-259">לא ישים</span><span class="sxs-lookup"><span data-stu-id="7c454-259">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="7c454-260">לא ישים</span><span class="sxs-lookup"><span data-stu-id="7c454-260">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-261">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="7c454-261">Billed sales</span></span></td>
<td><span data-ttu-id="7c454-262">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-262">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7c454-263">חשבונית מאושרת, ומתרחשת ירידה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="7c454-263">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="7c454-264">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="7c454-264">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="7c454-265">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-265">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="7c454-266">לא ישים</span><span class="sxs-lookup"><span data-stu-id="7c454-266">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7c454-267">לא ישים</span><span class="sxs-lookup"><span data-stu-id="7c454-267">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7c454-268">לא ישים</span><span class="sxs-lookup"><span data-stu-id="7c454-268">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7c454-269">לא ישים</span><span class="sxs-lookup"><span data-stu-id="7c454-269">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-270">מכירות שחויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="7c454-270">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="7c454-271">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-271">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-272">מכירות שחויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="7c454-272">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="7c454-273">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-273">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7c454-274">החשבונית מתוקנת כדי להגדיל את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="7c454-274">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="7c454-275">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="7c454-275">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="7c454-276">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-276">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="7c454-277">ביטול מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="7c454-277">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="7c454-278">שינוי במצב אבן דרך ממצב <strong>הוגשה חשבונית</strong> למצב <strong>מוכן להפקת חשבונית</strong></span><span class="sxs-lookup"><span data-stu-id="7c454-278">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="7c454-279">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-279">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="7c454-280">לא ישים</span><span class="sxs-lookup"><span data-stu-id="7c454-280">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="7c454-281">לא ישים</span><span class="sxs-lookup"><span data-stu-id="7c454-281">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-282">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="7c454-282">Billed sales</span></span></td>
<td><span data-ttu-id="7c454-283">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-283">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7c454-284">החשבונית מתוקנת כדי להקטין את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="7c454-284">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="7c454-285">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="7c454-285">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="7c454-286">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-286">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-287">מכירות שחויבו עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="7c454-287">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="7c454-288">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-288">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7c454-289">מכירות שלא חויבו - ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="7c454-289">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="7c454-290">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="7c454-290">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
