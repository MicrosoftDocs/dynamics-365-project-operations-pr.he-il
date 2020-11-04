---
title: נתונים בפועל
description: נושא זה מספק מידע על אופן העבודה עם נתונים בפועל ב-Project Operations ‏365 Microsoft Dynamics.
author: rumant
manager: AnnBe
ms.date: 09/16/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 93a945ffbe9c6dd998456b506b95e717ab8fbab7
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077298"
---
# <a name="actuals"></a><span data-ttu-id="2e8e2-103">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="2e8e2-103">Actuals</span></span> 

<span data-ttu-id="2e8e2-104">_**חל על** : Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="2e8e2-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="2e8e2-105">נתונים בפועל הם כמות העבודה שהושלמה בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-105">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="2e8e2-106">הם נוצרים כתוצאה ערכי זמן והוצאות, ופקודות יומן וחשבוניות.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-106">They are created as a result of time and expense entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="2e8e2-107">שורות יומן והגשת זמן</span><span class="sxs-lookup"><span data-stu-id="2e8e2-107">Journal lines and time submission</span></span>

<span data-ttu-id="2e8e2-108">לקבלת מידע נוסף אודות ערך זמן, ראה [מבט כולל על ערך זמן](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="2e8e2-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="2e8e2-109">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-109">Time and materials</span></span>

<span data-ttu-id="2e8e2-110">כאשר ערך זמן שמוגש מקושר לפרויקט הממופה לסעיף חוזה של זמן וחומרים, המערכת יוצרת שתי שורות יומן, אחת עובר עלות ואחת עבור מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="2e8e2-111">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="2e8e2-111">Fixed price</span></span>

<span data-ttu-id="2e8e2-112">כאשר ערך זמן שמוגש מקושר לפרוייקט הממופה לסעיף חוזה במחיר קבוע, המערכת יוצרת שורת יומן אחת עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="2e8e2-113">תמחור ברירת מחדל</span><span class="sxs-lookup"><span data-stu-id="2e8e2-113">Default pricing</span></span>

<span data-ttu-id="2e8e2-114">הלוגיקה ליצירת מחירי ברירת מחדל נמצאת בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="2e8e2-115">ערכי השדות מערך הזמן מועתקים לשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="2e8e2-116">ערכים אלה כוללים את תאריך העסקה, את סעיף החוזה שאליו ממופה הפרוייקט ואת תוצאת המטבע במחירון המתאים.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="2e8e2-117">השדות המשפיעים על תמחור ברירת המחדל, כגון **תפקיד** ו **יחידה ארגונית** , משמשים לקביעת מחיר מתאים בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-117">The fields that affect default pricing, such as **Role** and **Org Unit** , are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="2e8e2-118">ניתן להוסיף שדה מותאם אישית בערך הזמן.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="2e8e2-119">אם ברצונך שערך השדה יופץ לנתונים בפועל, עליך ליצור את השדה בישות 'נתונים בפועל' ולהשתמש במיפויי שדה כדי להעתיק את השדה מערך הזמן לנתון בפועל.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-119">If you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="2e8e2-120">שורות יומן והגשת הוצאות בסיסיות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-120">Journal lines and basic expense submission</span></span>

<span data-ttu-id="2e8e2-121">לקבלת מידע נוסף אודות ערכי הוצאה, ראה [מבט כולל על ערכי הוצאה](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="2e8e2-121">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="2e8e2-122">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-122">Time and materials</span></span>

<span data-ttu-id="2e8e2-123">כאשר ערך הוצאה בסיסית שמוגש מקושר לפרויקט הממופה לסעיף חוזה של זמן וחומרים, המערכת יוצרת שתי שורות יומן, אחת עבור עלות ואחת עבור מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-123">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="2e8e2-124">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="2e8e2-124">Fixed price</span></span>

<span data-ttu-id="2e8e2-125">כאשר ערך הוצאה בסיסית שמוגש מקושר לפרוייקט הממופה לסעיף חוזה במחיר קבוע, המערכת יוצרת שורת יומן אחת עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-125">When a basic expense entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="2e8e2-126">תמחור ברירת מחדל</span><span class="sxs-lookup"><span data-stu-id="2e8e2-126">Default pricing</span></span>

<span data-ttu-id="2e8e2-127">הלוגיקה להזנת מחירי ברירת מחדל להוצאות מבוססת על קטגוריית ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-127">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="2e8e2-128">תאריך העסקה, סעיף החוזה שאליו ממופה הפרוייקט והמטבע משמשים כולם כדי לקבוע את המחירון המתאים.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-128">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="2e8e2-129">עם זאת, כברירת מחדל, הסכום שמוזן עבור המחיר עצמו, מוגדר ישירות לשורות היומן של ההוצאות הקשורות עבור עלות ומכירות.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-129">However, by default, the amount that is entered for the price itself is set directly on the related expense journal lines for cost and sales.</span></span>

<span data-ttu-id="2e8e2-130">ערך מבוסס-קטגוריה של מחירי ברירת מחדל ליחידה אינו זמין בערכי הוצאה.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-130">Category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="2e8e2-131">שימוש ביומני ערכים לתיעוד עלויות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-131">Use entry journals to record costs</span></span>

<span data-ttu-id="2e8e2-132">יומני ערכים מאפשרים לך לתעד עלות או הכנסה במחלקות החומר, התשלום, הזמן, ההוצאה או עסקאות מס.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-132">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="2e8e2-133">ניתן להשתמש ביומנים למטרות הבאות:</span><span class="sxs-lookup"><span data-stu-id="2e8e2-133">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="2e8e2-134">תיעוד עלויות בפועל של חומרים ומכירות בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-134">Record the actual cost of materials and sales on a project.</span></span>
- <span data-ttu-id="2e8e2-135">העברת נתונים בפועל של עסקאות ממערכת אחרת ל-‎‏Project Operations ‏365 Microsoft Dynamics‎.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-135">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="2e8e2-136">רישום עלויות שהתרחשו במערכת אחרת.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-136">Record costs that occurred in another system.</span></span> <span data-ttu-id="2e8e2-137">עלויות אלה יכולות לכלול עלויות רכש או קבלנות משנה.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-137">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2e8e2-138">היישום אינו מאמת את סוג שורת היומן או את התמחור הקשור שמזינים בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-138">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="2e8e2-139">לכן, כדאי שרק משתמש שמודע לחלוטין להשפעה החשבונאית שיש נתונים בפועל על הפרויקט, ישתמש ביומני ערך ליצירת נתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-139">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="2e8e2-140">בגלל ההשפעה של סוג יומן זה, עליך לבחור בקפידה למי יש גישה ליצירת יומני ערך.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-140">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>
## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="2e8e2-141">תיעוד נתונים בפועל בהתבסס על אירועי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-141">Record actuals based on project events</span></span>

<span data-ttu-id="2e8e2-142">Project Operations מתעד את העסקות הפיננסיות המתרחשות במהלך פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-142">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="2e8e2-143">עסקאות אלה מתועדות כנתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-143">These transactions are recorded as actuals.</span></span> <span data-ttu-id="2e8e2-144">הטבלאות הבאות מציגות את הסוגים השונים של נתונים בפועל שנוצרים, בהתאם לשאלה אם הפרוייקט הוא פרוייקט של זמן וחומרים פרוייקט במחיר קבוע, פרוייקט שנמצא בשלב קדם המכירות או פרוייקט פנימי.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-144">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="2e8e2-145">המשאב משתייך לאותה יחידה ארגונית כשל יחידת החוזה של הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-145">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="2e8e2-146">אירוע</span><span class="sxs-lookup"><span data-stu-id="2e8e2-146">Event</span></span></th>
<th colspan="4"><span data-ttu-id="2e8e2-147">פרוייקט לחיוב או פרוייקט שנמכר</span><span class="sxs-lookup"><span data-stu-id="2e8e2-147">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="2e8e2-148">פרוייקט בשלב הקדם-מכירות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-148">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="2e8e2-149">פרוייקט פנימי</span><span class="sxs-lookup"><span data-stu-id="2e8e2-149">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="2e8e2-150">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-150">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="2e8e2-151">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="2e8e2-151">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="2e8e2-152">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="2e8e2-152">Actuals</span></span></th>
<th><span data-ttu-id="2e8e2-153">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-153">Transaction currency</span></span></th>
<th><span data-ttu-id="2e8e2-154">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="2e8e2-154">Fixed price</span></span></th>
<th><span data-ttu-id="2e8e2-155">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-155">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="2e8e2-156">ערך זמן נוצר.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-156">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="2e8e2-157">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="2e8e2-157">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-158">ערך זמן נשלח.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-158">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="2e8e2-159">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="2e8e2-159">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="2e8e2-160">הזמן מאושר, ואין שינוי או עלייה בשעות לחיוב במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-160">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="2e8e2-161">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-161">Cost actual</span></span></td>
<td><span data-ttu-id="2e8e2-162">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-162">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="2e8e2-163">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-163">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="2e8e2-164">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-164">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="2e8e2-165">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-165">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="2e8e2-166">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-167">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="2e8e2-167">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="2e8e2-168">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-168">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="2e8e2-169">הזמן מאושר, וירידה בשעות לחיוב מתרחשת במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-169">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="2e8e2-170">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-170">Cost actual</span></span></td>
<td><span data-ttu-id="2e8e2-171">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-171">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="2e8e2-172">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-172">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="2e8e2-173">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-173">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="2e8e2-174">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-174">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="2e8e2-175">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-175">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-176">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-176">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="2e8e2-177">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-177">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-178">נתון בפועל של מכירות שלא חויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="2e8e2-178">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="2e8e2-179">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="2e8e2-180">חשבונית מאושרת, ואין שינוי או עלייה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-180">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="2e8e2-181">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="2e8e2-182">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-182">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="2e8e2-183">מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="2e8e2-183">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="2e8e2-184">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-184">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="2e8e2-185">לא ישים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-185">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="2e8e2-186">לא ישים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-187">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="2e8e2-187">Billed sales</span></span></td>
<td><span data-ttu-id="2e8e2-188">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-188">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="2e8e2-189">חשבונית מאושרת, ומתרחשת ירידה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-189">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="2e8e2-190">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-190">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="2e8e2-191">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-191">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="2e8e2-192">לא ישים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-192">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="2e8e2-193">לא ישים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-193">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="2e8e2-194">לא ישים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-194">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="2e8e2-195">לא ישים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-195">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-196">מכירות שחויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-196">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="2e8e2-197">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-197">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-198">מכירות שחויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="2e8e2-198">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="2e8e2-199">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-199">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="2e8e2-200">החשבונית מתוקנת כדי להגדיל את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-200">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="2e8e2-201">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="2e8e2-201">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="2e8e2-202">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-202">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="2e8e2-203">ביטול מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="2e8e2-203">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="2e8e2-204">שינוי במצב אבן דרך ממצב <strong>הוגשה חשבונית</strong> למצב <strong>מוכן להפקת חשבונית</strong></span><span class="sxs-lookup"><span data-stu-id="2e8e2-204">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="2e8e2-205">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-205">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="2e8e2-206">לא ישים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-206">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="2e8e2-207">לא ישים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-207">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-208">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="2e8e2-208">Billed sales</span></span></td>
<td><span data-ttu-id="2e8e2-209">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-209">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="2e8e2-210">החשבונית מתוקנת כדי להקטין את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-210">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="2e8e2-211">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="2e8e2-211">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="2e8e2-212">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-212">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-213">מכירות שחויבו עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-213">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="2e8e2-214">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-214">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-215">מכירות שלא חויבו - ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="2e8e2-215">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="2e8e2-216">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-216">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="2e8e2-217">המשאב משתייך ליחידה ארגונית השונה מיחידת החוזה של הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-217">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="2e8e2-218">אירוע</span><span class="sxs-lookup"><span data-stu-id="2e8e2-218">Event</span></span></th>
<th colspan="4"><span data-ttu-id="2e8e2-219">פרוייקט לחיוב או פרוייקט שנמכר</span><span class="sxs-lookup"><span data-stu-id="2e8e2-219">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="2e8e2-220">פרוייקט בשלב הקדם-מכירות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-220">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="2e8e2-221">פרוייקט פנימי</span><span class="sxs-lookup"><span data-stu-id="2e8e2-221">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="2e8e2-222">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-222">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="2e8e2-223">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="2e8e2-223">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="2e8e2-224">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="2e8e2-224">Actuals</span></span></th>
<th><span data-ttu-id="2e8e2-225">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-225">Transaction currency</span></span></th>
<th><span data-ttu-id="2e8e2-226">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="2e8e2-226">Fixed price</span></span></th>
<th><span data-ttu-id="2e8e2-227">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-227">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="2e8e2-228">ערך זמן נוצר.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-228">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="2e8e2-229">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="2e8e2-229">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-230">ערך זמן נשלח.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-230">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="2e8e2-231">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="2e8e2-231">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="2e8e2-232">הזמן מאושר, ואין שינוי או עלייה בשעות לחיוב במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-232">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="2e8e2-233">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-233">Cost actual</span></span></td>
<td><span data-ttu-id="2e8e2-234">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-234">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="2e8e2-235">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-235">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="2e8e2-236">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-236">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="2e8e2-237">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-237">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="2e8e2-238">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-238">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-239">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="2e8e2-239">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="2e8e2-240">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-240">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-241">עלות יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-241">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="2e8e2-242">מטבע של יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-242">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-243">מכירות בין-ארגוניות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-243">Interorganizational sales</span></span></td>
<td><span data-ttu-id="2e8e2-244">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-244">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="2e8e2-245">הזמן מאושר, וירידה בשעות לחיוב מתרחשת במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-245">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="2e8e2-246">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-246">Cost actual</span></span></td>
<td><span data-ttu-id="2e8e2-247">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-247">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="2e8e2-248">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-248">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="2e8e2-249">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-249">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="2e8e2-250">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-250">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="2e8e2-251">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-251">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-252">עלות יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-252">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="2e8e2-253">מטבע של יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-253">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-254">מכירות בין-ארגוניות</span><span class="sxs-lookup"><span data-stu-id="2e8e2-254">Interorganizational sales</span></span></td>
<td><span data-ttu-id="2e8e2-255">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-255">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-256">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-256">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="2e8e2-257">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-257">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-258">נתון בפועל של מכירות שלא חויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="2e8e2-258">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="2e8e2-259">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="2e8e2-260">חשבונית מאושרת, ואין שינוי או עלייה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-260">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="2e8e2-261">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="2e8e2-262">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-262">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="2e8e2-263">מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="2e8e2-263">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="2e8e2-264">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-264">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="2e8e2-265">לא ישים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-265">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="2e8e2-266">לא ישים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-267">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="2e8e2-267">Billed sales</span></span></td>
<td><span data-ttu-id="2e8e2-268">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-268">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="2e8e2-269">חשבונית מאושרת, ומתרחשת ירידה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-269">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="2e8e2-270">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-270">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="2e8e2-271">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-271">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="2e8e2-272">לא ישים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-272">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="2e8e2-273">לא ישים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-273">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="2e8e2-274">לא ישים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-274">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="2e8e2-275">לא ישים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-275">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-276">מכירות שחויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-276">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="2e8e2-277">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-277">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-278">מכירות שחויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="2e8e2-278">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="2e8e2-279">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-279">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="2e8e2-280">החשבונית מתוקנת כדי להגדיל את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-280">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="2e8e2-281">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="2e8e2-281">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="2e8e2-282">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-282">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="2e8e2-283">ביטול מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="2e8e2-283">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="2e8e2-284">שינוי במצב אבן דרך ממצב <strong>הוגשה חשבונית</strong> למצב <strong>מוכן להפקת חשבונית</strong></span><span class="sxs-lookup"><span data-stu-id="2e8e2-284">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="2e8e2-285">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-285">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="2e8e2-286">לא ישים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-286">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="2e8e2-287">לא ישים</span><span class="sxs-lookup"><span data-stu-id="2e8e2-287">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-288">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="2e8e2-288">Billed sales</span></span></td>
<td><span data-ttu-id="2e8e2-289">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-289">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="2e8e2-290">החשבונית מתוקנת כדי להקטין את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="2e8e2-290">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="2e8e2-291">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="2e8e2-291">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="2e8e2-292">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-292">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-293">מכירות שחויבו עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="2e8e2-293">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="2e8e2-294">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-294">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="2e8e2-295">מכירות שלא חויבו - ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="2e8e2-295">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="2e8e2-296">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e8e2-296">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
