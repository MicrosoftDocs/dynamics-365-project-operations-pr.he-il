---
title: נתונים בפועל
description: נושא זו מספק מידע אודות נתונים בפועל של פרוייקט.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 44c6e85f-5b21-4e24-999c-15a2f065d977
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8291e0eb8531e8e9690368675f333c44b6e92e48
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751868"
---
# <a name="actuals"></a><span data-ttu-id="e5b15-103">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="e5b15-103">Actuals</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="e5b15-104">נתונים בפועל הם כמות העבודה שהושלמה בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="e5b15-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="e5b15-105">ניתן לעקוב אחר נתונים בפועל בחזרה למסמכי המקור שלהם.</span><span class="sxs-lookup"><span data-stu-id="e5b15-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="e5b15-106">מסמכי מקור אלה כוללים ערכי זמן, הוצאות ויומן וכן חשבוניות.</span><span class="sxs-lookup"><span data-stu-id="e5b15-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![כיצד ניתן לשייך נתונים בפועל של פרוייקט למסמכי מקור](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="e5b15-108">שליחת ערך זמן</span><span class="sxs-lookup"><span data-stu-id="e5b15-108">Submitting a time entry</span></span>

<span data-ttu-id="e5b15-109">ב- PSA, כאשר ערך זמן נשלח עבור פרוייקט הממופה לסעיף חוזה של זמן וחומרים, נוצרות שתי שורות יומן.</span><span class="sxs-lookup"><span data-stu-id="e5b15-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="e5b15-110">שורה אחת היא עבור עלות, והשורה השנייה היא עבור מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="e5b15-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="e5b15-111">כאשר ערך זמן נשלח עבור פרוייקט הממופה לסעיף חוזה של מחיר קבוע, שורת יומן נוצרת רק עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="e5b15-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="e5b15-112">הלוגיקה להזנת מחירי ברירת מחדל טמונה בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="e5b15-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="e5b15-113">כל ערכי השדות מערך זמן מועתקים לשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="e5b15-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="e5b15-114">שדות אלה כוללים את תאריך העסקה, את סעיף החוזה שאליו ממופה הפרוייקט ואת תוצאת המטבע במחירון המתאים.</span><span class="sxs-lookup"><span data-stu-id="e5b15-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="e5b15-115">השדות המשפיעים על מחירי ברירת המחדל, כגון **תפקיד** ו**יחידה ארגונית**, גורמים להזנת מחיר מתאים כברירת מחדל בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="e5b15-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="e5b15-116">אם אתה מוסיף שדה מותאם אישית בערך הזמן, וברצונך שערך השדה יופץ לנתונים בפועל, עליך ליצור את השדה בישות 'נתונים בפועל' ולהשתמש במיפויי שדה כדי להעתיק את השדה מערך הזמן לנתון בפועל.</span><span class="sxs-lookup"><span data-stu-id="e5b15-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="e5b15-117">שליחת ערך הוצאה</span><span class="sxs-lookup"><span data-stu-id="e5b15-117">Submitting an expense entry</span></span>

<span data-ttu-id="e5b15-118">ב- PSA, כאשר ערך הוצאה נשלח עבור פרוייקט הממופה לסעיף חוזה של זמן וחומרים, נוצרות שתי שורות יומן.</span><span class="sxs-lookup"><span data-stu-id="e5b15-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="e5b15-119">שורה אחת היא עבור עלות, והשורה השנייה היא עבור מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="e5b15-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="e5b15-120">כאשר ערך הוצאה נשלח עבור פרוייקט הממופה לסעיף חוזה של מחיר קבוע, שורת יומן נוצרת רק עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="e5b15-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="e5b15-121">הלוגיקה להזנת מחירי ברירת מחדל עבור הוצאות מבוססת על קטגוריית ההוצאה שנבחרה בדף **ערך הוצאה**.</span><span class="sxs-lookup"><span data-stu-id="e5b15-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="e5b15-122">תאריך העסקה, סעיף החוזה שאליו ממופה הפרוייקט והמטבע משמשים כולם כדי לקבוע את המחירון המתאים.</span><span class="sxs-lookup"><span data-stu-id="e5b15-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="e5b15-123">עם זאת, עבור המחיר עצמו, הסכום שהמשתמש הזין מוגדר ישירות בשורות היומן של ההוצאות הקשורות עבור עלות ומכירות כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="e5b15-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="e5b15-124">בגירסה הנוכחית של PSA, ערך מבוסס-קטגוריה של מחירי ברירת מחדל ליחידה בערכי הוצאה אינו זמין.</span><span class="sxs-lookup"><span data-stu-id="e5b15-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-journals-to-record-costs"></a><span data-ttu-id="e5b15-125">שימוש ביומנים לתיעוד עלויות</span><span class="sxs-lookup"><span data-stu-id="e5b15-125">Using journals to record costs</span></span>

<span data-ttu-id="e5b15-126">ב- PSA, יומנים מאפשרים לך לתעד עלות או הכנסות במחלקות החומר, התשלום, הזמן, ההוצאה או עסקת המס.</span><span class="sxs-lookup"><span data-stu-id="e5b15-126">In PSA, journals let you record cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="e5b15-127">יומן כולל כותרת, שורות ופעולת **אישור**.</span><span class="sxs-lookup"><span data-stu-id="e5b15-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="e5b15-128">להלן מספר תרחישים שבהם אתה כדאי להשתמש ביומן:</span><span class="sxs-lookup"><span data-stu-id="e5b15-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="e5b15-129">עליך לתעד עלויות בפועל של חומרים ומכירות בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="e5b15-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="e5b15-130">עליך להעביר נתונים בפועל של עסקה ממערכת אחרת ל- PSA.</span><span class="sxs-lookup"><span data-stu-id="e5b15-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="e5b15-131">עליך לתעד עלויות שהתרחשו במערכת אחרת, כגון עלויות רכישה או מסירה לקבלן משנה.</span><span class="sxs-lookup"><span data-stu-id="e5b15-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="e5b15-132">תיעוד נתונים בפועל בהתבסס על אירועי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-132">Recording actuals based on project events</span></span>

<span data-ttu-id="e5b15-133">PSA מתעד את העסקות הפיננסיות המתרחשות במהלך פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="e5b15-133">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="e5b15-134">עסקאות אלה מתועדות כ**נתונים בפועל**.</span><span class="sxs-lookup"><span data-stu-id="e5b15-134">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="e5b15-135">הטבלאות הבאות מציגות את הסוגים השונים של נתונים בפועל שנוצרים, בהתאם לשאלה אם הפרוייקט הוא פרוייקט של זמן וחומרים פרוייקט במחיר קבוע, פרוייקט שנמצא בשלב קדם המכירות או פרוייקט פנימי.</span><span class="sxs-lookup"><span data-stu-id="e5b15-135">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="e5b15-136">**המשאב משתייך לאותה יחידה ארגונית כשל יחידת החוזה של הפרוייקט**</span><span class="sxs-lookup"><span data-stu-id="e5b15-136">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="e5b15-137">אירוע</span><span class="sxs-lookup"><span data-stu-id="e5b15-137">Event</span></span></th>
<th colspan="4"><span data-ttu-id="e5b15-138">פרוייקט לחיוב או פרוייקט שנמכר</span><span class="sxs-lookup"><span data-stu-id="e5b15-138">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="e5b15-139">פרוייקט בשלב הקדם-מכירות</span><span class="sxs-lookup"><span data-stu-id="e5b15-139">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="e5b15-140">פרוייקט פנימי</span><span class="sxs-lookup"><span data-stu-id="e5b15-140">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="e5b15-141">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="e5b15-141">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="e5b15-142">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="e5b15-142">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="e5b15-143">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="e5b15-143">Actuals</span></span></th>
<th><span data-ttu-id="e5b15-144">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="e5b15-144">Transaction currency</span></span></th>
<th><span data-ttu-id="e5b15-145">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="e5b15-145">Fixed price</span></span></th>
<th><span data-ttu-id="e5b15-146">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="e5b15-146">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="e5b15-147">ערך זמן נוצר.</span><span class="sxs-lookup"><span data-stu-id="e5b15-147">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="e5b15-148">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="e5b15-148">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-149">ערך זמן נשלח.</span><span class="sxs-lookup"><span data-stu-id="e5b15-149">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="e5b15-150">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="e5b15-150">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="e5b15-151">הזמן מאושר, ואין שינוי או עלייה בשעות לחיוב במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="e5b15-151">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="e5b15-152">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="e5b15-152">Cost actual</span></span></td>
<td><span data-ttu-id="e5b15-153">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="e5b15-153">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="e5b15-154">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="e5b15-154">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="e5b15-155">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="e5b15-155">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="e5b15-156">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="e5b15-156">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="e5b15-157">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="e5b15-157">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-158">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="e5b15-158">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="e5b15-159">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-159">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="e5b15-160">הזמן מאושר, וירידה בשעות לחיוב מתרחשת במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="e5b15-160">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="e5b15-161">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="e5b15-161">Cost actual</span></span></td>
<td><span data-ttu-id="e5b15-162">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="e5b15-162">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="e5b15-163">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="e5b15-163">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="e5b15-164">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="e5b15-164">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="e5b15-165">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="e5b15-165">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="e5b15-166">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="e5b15-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-167">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="e5b15-167">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="e5b15-168">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-168">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-169">נתון בפועל של מכירות שלא חויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="e5b15-169">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="e5b15-170">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-170">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="e5b15-171">חשבונית מאושרת, ואין שינוי או עלייה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="e5b15-171">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="e5b15-172">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="e5b15-172">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="e5b15-173">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-173">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="e5b15-174">מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="e5b15-174">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="e5b15-175">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-175">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="e5b15-176">לא ישים</span><span class="sxs-lookup"><span data-stu-id="e5b15-176">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="e5b15-177">לא ישים</span><span class="sxs-lookup"><span data-stu-id="e5b15-177">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-178">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="e5b15-178">Billed sales</span></span></td>
<td><span data-ttu-id="e5b15-179">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="e5b15-180">חשבונית מאושרת, ומתרחשת ירידה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="e5b15-180">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="e5b15-181">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="e5b15-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="e5b15-182">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-182">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="e5b15-183">לא ישים</span><span class="sxs-lookup"><span data-stu-id="e5b15-183">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e5b15-184">לא ישים</span><span class="sxs-lookup"><span data-stu-id="e5b15-184">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e5b15-185">לא ישים</span><span class="sxs-lookup"><span data-stu-id="e5b15-185">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e5b15-186">לא ישים</span><span class="sxs-lookup"><span data-stu-id="e5b15-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-187">מכירות שחויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="e5b15-187">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="e5b15-188">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-188">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-189">מכירות שחויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="e5b15-189">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="e5b15-190">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="e5b15-191">החשבונית מתוקנת כדי להגדיל את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="e5b15-191">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="e5b15-192">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="e5b15-192">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="e5b15-193">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-193">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="e5b15-194">ביטול מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="e5b15-194">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="e5b15-195">שינוי במצב אבן דרך ממצב <strong>הוגשה חשבונית</strong> למצב <strong>מוכן להפקת חשבונית</strong></span><span class="sxs-lookup"><span data-stu-id="e5b15-195">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="e5b15-196">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-196">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="e5b15-197">לא ישים</span><span class="sxs-lookup"><span data-stu-id="e5b15-197">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="e5b15-198">לא ישים</span><span class="sxs-lookup"><span data-stu-id="e5b15-198">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-199">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="e5b15-199">Billed sales</span></span></td>
<td><span data-ttu-id="e5b15-200">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-200">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="e5b15-201">החשבונית מתוקנת כדי להקטין את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="e5b15-201">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="e5b15-202">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="e5b15-202">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="e5b15-203">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-203">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-204">מכירות שחויבו עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="e5b15-204">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="e5b15-205">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-205">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-206">מכירות שלא חויבו - ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="e5b15-206">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="e5b15-207">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-207">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="e5b15-208">**המשאב משתייך ליחידה ארגונית השונה מיחידת החוזה של הפרוייקט**</span><span class="sxs-lookup"><span data-stu-id="e5b15-208">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="e5b15-209">אירוע</span><span class="sxs-lookup"><span data-stu-id="e5b15-209">Event</span></span></th>
<th colspan="4"><span data-ttu-id="e5b15-210">פרוייקט לחיוב או פרוייקט שנמכר</span><span class="sxs-lookup"><span data-stu-id="e5b15-210">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="e5b15-211">פרוייקט בשלב הקדם-מכירות</span><span class="sxs-lookup"><span data-stu-id="e5b15-211">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="e5b15-212">פרוייקט פנימי</span><span class="sxs-lookup"><span data-stu-id="e5b15-212">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="e5b15-213">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="e5b15-213">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="e5b15-214">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="e5b15-214">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="e5b15-215">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="e5b15-215">Actuals</span></span></th>
<th><span data-ttu-id="e5b15-216">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="e5b15-216">Transaction currency</span></span></th>
<th><span data-ttu-id="e5b15-217">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="e5b15-217">Fixed price</span></span></th>
<th><span data-ttu-id="e5b15-218">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="e5b15-218">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="e5b15-219">ערך זמן נוצר.</span><span class="sxs-lookup"><span data-stu-id="e5b15-219">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="e5b15-220">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="e5b15-220">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-221">ערך זמן נשלח.</span><span class="sxs-lookup"><span data-stu-id="e5b15-221">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="e5b15-222">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="e5b15-222">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="e5b15-223">הזמן מאושר, ואין שינוי או עלייה בשעות לחיוב במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="e5b15-223">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="e5b15-224">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="e5b15-224">Cost actual</span></span></td>
<td><span data-ttu-id="e5b15-225">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="e5b15-225">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="e5b15-226">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="e5b15-226">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="e5b15-227">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="e5b15-227">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="e5b15-228">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="e5b15-228">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="e5b15-229">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="e5b15-229">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-230">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="e5b15-230">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="e5b15-231">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-231">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-232">עלות יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="e5b15-232">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="e5b15-233">מטבע של יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="e5b15-233">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-234">מכירות בין-ארגוניות</span><span class="sxs-lookup"><span data-stu-id="e5b15-234">Interorganizational sales</span></span></td>
<td><span data-ttu-id="e5b15-235">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="e5b15-235">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="e5b15-236">הזמן מאושר, וירידה בשעות לחיוב מתרחשת במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="e5b15-236">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="e5b15-237">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="e5b15-237">Cost actual</span></span></td>
<td><span data-ttu-id="e5b15-238">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="e5b15-238">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="e5b15-239">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="e5b15-239">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="e5b15-240">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="e5b15-240">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="e5b15-241">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="e5b15-241">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="e5b15-242">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="e5b15-242">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-243">עלות יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="e5b15-243">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="e5b15-244">מטבע של יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="e5b15-244">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-245">מכירות בין-ארגוניות</span><span class="sxs-lookup"><span data-stu-id="e5b15-245">Interorganizational sales</span></span></td>
<td><span data-ttu-id="e5b15-246">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="e5b15-246">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-247">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="e5b15-247">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="e5b15-248">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-248">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-249">נתון בפועל של מכירות שלא חויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="e5b15-249">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="e5b15-250">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-250">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="e5b15-251">חשבונית מאושרת, ואין שינוי או עלייה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="e5b15-251">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="e5b15-252">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="e5b15-252">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="e5b15-253">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-253">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="e5b15-254">מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="e5b15-254">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="e5b15-255">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-255">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="e5b15-256">לא ישים</span><span class="sxs-lookup"><span data-stu-id="e5b15-256">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="e5b15-257">לא ישים</span><span class="sxs-lookup"><span data-stu-id="e5b15-257">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-258">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="e5b15-258">Billed sales</span></span></td>
<td><span data-ttu-id="e5b15-259">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="e5b15-260">חשבונית מאושרת, ומתרחשת ירידה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="e5b15-260">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="e5b15-261">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="e5b15-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="e5b15-262">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-262">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="e5b15-263">לא ישים</span><span class="sxs-lookup"><span data-stu-id="e5b15-263">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e5b15-264">לא ישים</span><span class="sxs-lookup"><span data-stu-id="e5b15-264">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e5b15-265">לא ישים</span><span class="sxs-lookup"><span data-stu-id="e5b15-265">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="e5b15-266">לא ישים</span><span class="sxs-lookup"><span data-stu-id="e5b15-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-267">מכירות שחויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="e5b15-267">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="e5b15-268">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-268">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-269">מכירות שחויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="e5b15-269">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="e5b15-270">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-270">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="e5b15-271">החשבונית מתוקנת כדי להגדיל את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="e5b15-271">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="e5b15-272">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="e5b15-272">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="e5b15-273">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-273">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="e5b15-274">ביטול מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="e5b15-274">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="e5b15-275">שינוי במצב אבן דרך ממצב <strong>הוגשה חשבונית</strong> למצב <strong>מוכן להפקת חשבונית</strong></span><span class="sxs-lookup"><span data-stu-id="e5b15-275">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="e5b15-276">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-276">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="e5b15-277">לא ישים</span><span class="sxs-lookup"><span data-stu-id="e5b15-277">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="e5b15-278">לא ישים</span><span class="sxs-lookup"><span data-stu-id="e5b15-278">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-279">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="e5b15-279">Billed sales</span></span></td>
<td><span data-ttu-id="e5b15-280">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-280">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="e5b15-281">החשבונית מתוקנת כדי להקטין את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="e5b15-281">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="e5b15-282">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="e5b15-282">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="e5b15-283">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-283">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-284">מכירות שחויבו עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="e5b15-284">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="e5b15-285">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-285">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="e5b15-286">מכירות שלא חויבו - ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="e5b15-286">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="e5b15-287">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e5b15-287">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
