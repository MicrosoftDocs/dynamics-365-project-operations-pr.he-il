---
title: מבט כולל על נתונים בפועל
description: נושא זו מספק מידע אודות נתונים בפועל של פרוייקט.
author: rumant
ms.custom:
- dyn365-projectservice
- intro-internal
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
ms.openlocfilehash: cbb3e5c7f74cdf37ae4d259687bf7a98102a8131
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368162"
---
# <a name="actuals-overview"></a><span data-ttu-id="ffbe8-103">מבט כולל על נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="ffbe8-103">Actuals overview</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="ffbe8-104">נתונים בפועל הם כמות העבודה שהושלמה בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="ffbe8-105">ניתן לעקוב אחר נתונים בפועל בחזרה למסמכי המקור שלהם.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="ffbe8-106">מסמכי מקור אלה כוללים ערכי זמן, הוצאות ויומן וכן חשבוניות.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![כיצד ניתן לשייך נתונים בפועל של פרוייקט למסמכי מקור](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="ffbe8-108">שליחת ערך זמן</span><span class="sxs-lookup"><span data-stu-id="ffbe8-108">Submitting a time entry</span></span>

<span data-ttu-id="ffbe8-109">ב- PSA, כאשר ערך זמן נשלח עבור פרוייקט הממופה לסעיף חוזה של זמן וחומרים, נוצרות שתי שורות יומן.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="ffbe8-110">שורה אחת היא עבור עלות, והשורה השנייה היא עבור מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="ffbe8-111">כאשר ערך זמן נשלח עבור פרוייקט הממופה לסעיף חוזה של מחיר קבוע, שורת יומן נוצרת רק עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="ffbe8-112">הלוגיקה להזנת מחירי ברירת מחדל טמונה בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="ffbe8-113">כל ערכי השדות מערך זמן מועתקים לשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="ffbe8-114">שדות אלה כוללים את תאריך העסקה, את סעיף החוזה שאליו ממופה הפרוייקט ואת תוצאת המטבע במחירון המתאים.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="ffbe8-115">השדות המשפיעים על מחירי ברירת המחדל, כגון **תפקיד** ו **יחידה ארגונית**, גורמים להזנת מחיר מתאים כברירת מחדל בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="ffbe8-116">אם אתה מוסיף שדה מותאם אישית בערך הזמן, וברצונך שערך השדה יופץ לנתונים בפועל, עליך ליצור את השדה בישות 'נתונים בפועל' ולהשתמש במיפויי שדה כדי להעתיק את השדה מערך הזמן לנתון בפועל.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="ffbe8-117">שליחת ערך הוצאה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-117">Submitting an expense entry</span></span>

<span data-ttu-id="ffbe8-118">ב- PSA, כאשר ערך הוצאה נשלח עבור פרוייקט הממופה לסעיף חוזה של זמן וחומרים, נוצרות שתי שורות יומן.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="ffbe8-119">שורה אחת היא עבור עלות, והשורה השנייה היא עבור מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="ffbe8-120">כאשר ערך הוצאה נשלח עבור פרוייקט הממופה לסעיף חוזה של מחיר קבוע, שורת יומן נוצרת רק עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="ffbe8-121">הלוגיקה להזנת מחירי ברירת מחדל עבור הוצאות מבוססת על קטגוריית ההוצאה שנבחרה בדף **ערך הוצאה**.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="ffbe8-122">תאריך העסקה, סעיף החוזה שאליו ממופה הפרוייקט והמטבע משמשים כולם כדי לקבוע את המחירון המתאים.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="ffbe8-123">עם זאת, עבור המחיר עצמו, הסכום שהמשתמש הזין מוגדר ישירות בשורות היומן של ההוצאות הקשורות עבור עלות ומכירות כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="ffbe8-124">בגירסה הנוכחית של PSA, ערך מבוסס-קטגוריה של מחירי ברירת מחדל ליחידה בערכי הוצאה אינו זמין.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-entry-journals-to-record-costs"></a><span data-ttu-id="ffbe8-125">שימוש בפקודות יומן לתיעוד עלויות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-125">Using Entry journals to record costs</span></span>

<span data-ttu-id="ffbe8-126">ב- PSA, פקודות יומן מאפשרות לך לתעד עלות או הכנסות במחלקות החומר, התשלום, הזמן, ההוצאה או עסקת המס.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-126">In PSA, Entry journals let you record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="ffbe8-127">יומן כולל כותרת, שורות ופעולת **אישור**.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="ffbe8-128">להלן מספר תרחישים שבהם אתה כדאי להשתמש ביומן:</span><span class="sxs-lookup"><span data-stu-id="ffbe8-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="ffbe8-129">עליך לתעד עלויות בפועל של חומרים ומכירות בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="ffbe8-130">עליך להעביר נתונים בפועל של עסקה ממערכת אחרת ל- PSA.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="ffbe8-131">עליך לתעד עלויות שהתרחשו במערכת אחרת, כגון עלויות רכישה או מסירה לקבלן משנה.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ffbe8-132">השימוש בפקודת יומן ליצירת עובדות צריך להיעשות רק על ידי משתמש שמודע לחלוטין להשפעה החשבונאית שיש לעובדים על הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-132">Using Entry journals to create actuals should be done only by a user who is fully aware of the accounting impact the Actuals have on the project.</span></span> <span data-ttu-id="ffbe8-133">הסיבה לכך היא שהיישום אינו מאמת את סוג שורת היומן, או את התמחור הקשור שמוזן בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-133">This is because the application does not validate the journal line type, or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="ffbe8-134">בגלל ההשפעה של סוג יומן זה, יש לנקוט זהירות מספקת מבחינת מי שמקבל גישה ליצירת פקודות יומן.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-134">Because of the impact of this journal type, exercise adequate caution in who is given access to create Entry journals.</span></span>     


## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="ffbe8-135">תיעוד נתונים בפועל בהתבסס על אירועי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-135">Recording actuals based on project events</span></span>

<span data-ttu-id="ffbe8-136">PSA מתעד את העסקות הפיננסיות המתרחשות במהלך פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-136">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="ffbe8-137">עסקאות אלה מתועדות כ **נתונים בפועל**.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-137">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="ffbe8-138">הטבלאות הבאות מציגות את הסוגים השונים של נתונים בפועל שנוצרים, בהתאם לשאלה אם הפרוייקט הוא פרוייקט של זמן וחומרים פרוייקט במחיר קבוע, פרוייקט שנמצא בשלב קדם המכירות או פרוייקט פנימי.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-138">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="ffbe8-139">**המשאב משתייך לאותה יחידה ארגונית כשל יחידת החוזה של הפרוייקט**</span><span class="sxs-lookup"><span data-stu-id="ffbe8-139">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="ffbe8-140">אירוע</span><span class="sxs-lookup"><span data-stu-id="ffbe8-140">Event</span></span></th>
<th colspan="4"><span data-ttu-id="ffbe8-141">פרוייקט לחיוב או פרוייקט שנמכר</span><span class="sxs-lookup"><span data-stu-id="ffbe8-141">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="ffbe8-142">פרוייקט בשלב הקדם-מכירות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-142">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="ffbe8-143">פרוייקט פנימי</span><span class="sxs-lookup"><span data-stu-id="ffbe8-143">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="ffbe8-144">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-144">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="ffbe8-145">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="ffbe8-145">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="ffbe8-146">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="ffbe8-146">Actuals</span></span></th>
<th><span data-ttu-id="ffbe8-147">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-147">Transaction currency</span></span></th>
<th><span data-ttu-id="ffbe8-148">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="ffbe8-148">Fixed price</span></span></th>
<th><span data-ttu-id="ffbe8-149">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-149">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="ffbe8-150">ערך זמן נוצר.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-150">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="ffbe8-151">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="ffbe8-151">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-152">ערך זמן נשלח.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-152">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="ffbe8-153">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="ffbe8-153">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ffbe8-154">הזמן מאושר, ואין שינוי או עלייה בשעות לחיוב במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-154">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="ffbe8-155">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-155">Cost actual</span></span></td>
<td><span data-ttu-id="ffbe8-156">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-156">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ffbe8-157">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-157">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="ffbe8-158">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-158">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="ffbe8-159">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-159">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="ffbe8-160">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-160">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-161">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="ffbe8-161">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="ffbe8-162">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-162">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ffbe8-163">הזמן מאושר, וירידה בשעות לחיוב מתרחשת במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-163">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="ffbe8-164">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-164">Cost actual</span></span></td>
<td><span data-ttu-id="ffbe8-165">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-165">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="ffbe8-166">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-166">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="ffbe8-167">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-167">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="ffbe8-168">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-168">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="ffbe8-169">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-169">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-170">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-170">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="ffbe8-171">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-171">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-172">נתון בפועל של מכירות שלא חויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="ffbe8-172">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="ffbe8-173">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-173">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ffbe8-174">חשבונית מאושרת, ואין שינוי או עלייה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-174">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="ffbe8-175">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-175">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="ffbe8-176">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-176">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ffbe8-177">מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="ffbe8-177">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="ffbe8-178">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-178">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ffbe8-179">לא ישים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-179">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="ffbe8-180">לא ישים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-180">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-181">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="ffbe8-181">Billed sales</span></span></td>
<td><span data-ttu-id="ffbe8-182">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-182">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ffbe8-183">חשבונית מאושרת, ומתרחשת ירידה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-183">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="ffbe8-184">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-184">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="ffbe8-185">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-185">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="ffbe8-186">לא ישים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-186">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ffbe8-187">לא ישים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-187">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ffbe8-188">לא ישים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-188">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ffbe8-189">לא ישים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-189">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-190">מכירות שחויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-190">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="ffbe8-191">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-191">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-192">מכירות שחויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="ffbe8-192">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="ffbe8-193">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-193">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ffbe8-194">החשבונית מתוקנת כדי להגדיל את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-194">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="ffbe8-195">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="ffbe8-195">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="ffbe8-196">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-196">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="ffbe8-197">ביטול מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="ffbe8-197">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="ffbe8-198">שינוי במצב אבן דרך ממצב <strong>הוגשה חשבונית</strong> למצב <strong>מוכן להפקת חשבונית</strong></span><span class="sxs-lookup"><span data-stu-id="ffbe8-198">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="ffbe8-199">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-199">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="ffbe8-200">לא ישים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-200">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="ffbe8-201">לא ישים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-201">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-202">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="ffbe8-202">Billed sales</span></span></td>
<td><span data-ttu-id="ffbe8-203">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-203">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ffbe8-204">החשבונית מתוקנת כדי להקטין את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-204">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="ffbe8-205">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="ffbe8-205">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="ffbe8-206">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-206">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-207">מכירות שחויבו עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-207">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="ffbe8-208">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-208">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-209">מכירות שלא חויבו - ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="ffbe8-209">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="ffbe8-210">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-210">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="ffbe8-211">**המשאב משתייך ליחידה ארגונית השונה מיחידת החוזה של הפרוייקט**</span><span class="sxs-lookup"><span data-stu-id="ffbe8-211">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="ffbe8-212">אירוע</span><span class="sxs-lookup"><span data-stu-id="ffbe8-212">Event</span></span></th>
<th colspan="4"><span data-ttu-id="ffbe8-213">פרוייקט לחיוב או פרוייקט שנמכר</span><span class="sxs-lookup"><span data-stu-id="ffbe8-213">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="ffbe8-214">פרוייקט בשלב הקדם-מכירות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-214">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="ffbe8-215">פרוייקט פנימי</span><span class="sxs-lookup"><span data-stu-id="ffbe8-215">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="ffbe8-216">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-216">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="ffbe8-217">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="ffbe8-217">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="ffbe8-218">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="ffbe8-218">Actuals</span></span></th>
<th><span data-ttu-id="ffbe8-219">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-219">Transaction currency</span></span></th>
<th><span data-ttu-id="ffbe8-220">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="ffbe8-220">Fixed price</span></span></th>
<th><span data-ttu-id="ffbe8-221">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-221">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="ffbe8-222">ערך זמן נוצר.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-222">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="ffbe8-223">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="ffbe8-223">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-224">ערך זמן נשלח.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-224">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="ffbe8-225">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="ffbe8-225">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="ffbe8-226">הזמן מאושר, ואין שינוי או עלייה בשעות לחיוב במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-226">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="ffbe8-227">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-227">Cost actual</span></span></td>
<td><span data-ttu-id="ffbe8-228">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-228">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="ffbe8-229">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-229">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="ffbe8-230">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-230">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="ffbe8-231">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-231">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="ffbe8-232">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-232">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-233">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="ffbe8-233">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="ffbe8-234">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-235">עלות יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-235">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="ffbe8-236">מטבע של יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-236">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-237">מכירות בין-ארגוניות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-237">Interorganizational sales</span></span></td>
<td><span data-ttu-id="ffbe8-238">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-238">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="ffbe8-239">הזמן מאושר, וירידה בשעות לחיוב מתרחשת במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-239">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="ffbe8-240">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-240">Cost actual</span></span></td>
<td><span data-ttu-id="ffbe8-241">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-241">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="ffbe8-242">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-242">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="ffbe8-243">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-243">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="ffbe8-244">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-244">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="ffbe8-245">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-245">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-246">עלות יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-246">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="ffbe8-247">מטבע של יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-247">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-248">מכירות בין-ארגוניות</span><span class="sxs-lookup"><span data-stu-id="ffbe8-248">Interorganizational sales</span></span></td>
<td><span data-ttu-id="ffbe8-249">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-249">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-250">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-250">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="ffbe8-251">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-251">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-252">נתון בפועל של מכירות שלא חויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="ffbe8-252">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="ffbe8-253">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-253">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ffbe8-254">חשבונית מאושרת, ואין שינוי או עלייה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-254">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="ffbe8-255">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-255">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="ffbe8-256">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-256">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ffbe8-257">מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="ffbe8-257">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="ffbe8-258">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-258">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="ffbe8-259">לא ישים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-259">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="ffbe8-260">לא ישים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-260">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-261">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="ffbe8-261">Billed sales</span></span></td>
<td><span data-ttu-id="ffbe8-262">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-262">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ffbe8-263">חשבונית מאושרת, ומתרחשת ירידה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-263">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="ffbe8-264">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-264">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="ffbe8-265">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-265">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="ffbe8-266">לא ישים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-266">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ffbe8-267">לא ישים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-267">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ffbe8-268">לא ישים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-268">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="ffbe8-269">לא ישים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-269">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-270">מכירות שחויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-270">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="ffbe8-271">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-271">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-272">מכירות שחויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="ffbe8-272">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="ffbe8-273">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-273">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="ffbe8-274">החשבונית מתוקנת כדי להגדיל את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-274">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="ffbe8-275">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="ffbe8-275">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="ffbe8-276">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-276">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="ffbe8-277">ביטול מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="ffbe8-277">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="ffbe8-278">שינוי במצב אבן דרך ממצב <strong>הוגשה חשבונית</strong> למצב <strong>מוכן להפקת חשבונית</strong></span><span class="sxs-lookup"><span data-stu-id="ffbe8-278">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="ffbe8-279">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-279">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="ffbe8-280">לא ישים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-280">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="ffbe8-281">לא ישים</span><span class="sxs-lookup"><span data-stu-id="ffbe8-281">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-282">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="ffbe8-282">Billed sales</span></span></td>
<td><span data-ttu-id="ffbe8-283">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-283">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="ffbe8-284">החשבונית מתוקנת כדי להקטין את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="ffbe8-284">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="ffbe8-285">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="ffbe8-285">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="ffbe8-286">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-286">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-287">מכירות שחויבו עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="ffbe8-287">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="ffbe8-288">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-288">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="ffbe8-289">מכירות שלא חויבו - ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="ffbe8-289">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="ffbe8-290">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ffbe8-290">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]