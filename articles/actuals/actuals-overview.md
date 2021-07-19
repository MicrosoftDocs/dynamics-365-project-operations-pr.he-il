---
title: נתונים בפועל
description: נושא זה מספק מידע על אופן העבודה עם נתונים בפועל ב- Microsoft Dynamics 365 Project Operations.
author: rumant
ms.date: 04/01/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: intro-internal
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 9e046602a3005930c41ab8c50472d5b1a72303c6
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368612"
---
# <a name="actuals"></a><span data-ttu-id="31c22-103">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="31c22-103">Actuals</span></span> 

<span data-ttu-id="31c22-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="31c22-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="31c22-105">‏‫נתונים בפועל‬ מייצגים את ההתקדמות הכספית והתקדמות לוח הזמנים שנבדקה ואושרה בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="31c22-105">Actuals represent the reviewed and approved financial and schedule progress on a project.</span></span> <span data-ttu-id="31c22-106">הם נוצרים כתוצאה מאישור זמן, הוצאות, ערכי שימוש בחומרים וערכים ביומן וחשבוניות.</span><span class="sxs-lookup"><span data-stu-id="31c22-106">They are created as a result of approval of time, expense, material usage entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="31c22-107">שורות יומן והגשת זמן</span><span class="sxs-lookup"><span data-stu-id="31c22-107">Journal lines and time submission</span></span>

<span data-ttu-id="31c22-108">לקבלת מידע נוסף אודות ערך זמן, ראה [מבט כולל על ערך זמן](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="31c22-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="31c22-109">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="31c22-109">Time and materials</span></span>

<span data-ttu-id="31c22-110">כאשר ערך זמן שמוגש מקושר לפרויקט הממופה לסעיף חוזה של זמן וחומרים, המערכת יוצרת שתי שורות יומן, אחת עובר עלות ואחת עבור מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="31c22-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="31c22-111">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="31c22-111">Fixed price</span></span>

<span data-ttu-id="31c22-112">כאשר ערך זמן שמוגש מקושר לפרוייקט הממופה לסעיף חוזה במחיר קבוע, המערכת יוצרת שורת יומן אחת עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="31c22-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="31c22-113">תמחור ברירת מחדל</span><span class="sxs-lookup"><span data-stu-id="31c22-113">Default pricing</span></span>

<span data-ttu-id="31c22-114">הלוגיקה ליצירת מחירי ברירת מחדל נמצאת בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="31c22-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="31c22-115">ערכי השדות מערך הזמן מועתקים לשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="31c22-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="31c22-116">ערכים אלה כוללים את תאריך העסקה, את סעיף החוזה שאליו ממופה הפרוייקט ואת תוצאת המטבע במחירון המתאים.</span><span class="sxs-lookup"><span data-stu-id="31c22-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="31c22-117">שדות המשפיעים על תמחור ברירת המחדל, כגון **תפקיד** ו **‏‫יחידת הקצאת משאבים‬**, משמשים לקביעת המחיר המתאים בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="31c22-117">The fields that affect default pricing, such as **Role** and **Resourcing Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="31c22-118">ניתן להוסיף שדה מותאם אישית בערך הזמן.</span><span class="sxs-lookup"><span data-stu-id="31c22-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="31c22-119">אם ברצונך שערך השדה יופץ לנתונים בפועל, צור את השדה בטבלאות **נתונים בפועל** ו **שורת יומן**.</span><span class="sxs-lookup"><span data-stu-id="31c22-119">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="31c22-120">השתמש בקוד מותאם אישית כדי להפיץ את ערך השדה שנבחר מ'‏‫ערך זמן‬' ל'נתונים בפועל' דרך שורת היומן באמצעות מקורות העסקה.</span><span class="sxs-lookup"><span data-stu-id="31c22-120">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="31c22-121">למידע נוסף על מקורות העסקה וחיבורים, ראה [קישור נתונים בפועל לרשומות מקוריות](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="31c22-121">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="31c22-122">שורות יומן והגשת הוצאות בסיסיות</span><span class="sxs-lookup"><span data-stu-id="31c22-122">Journal lines and basic expense submission</span></span>

<span data-ttu-id="31c22-123">לקבלת מידע נוסף אודות ערכי הוצאה, ראה [מבט כולל על ערכי הוצאה](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="31c22-123">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="31c22-124">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="31c22-124">Time and materials</span></span>

<span data-ttu-id="31c22-125">כאשר ערך הוצאה בסיסית שמוגש מקושר לפרויקט הממופה לסעיף חוזה של זמן וחומרים, המערכת יוצרת שתי שורות יומן, אחת עבור עלות ואחת עבור מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="31c22-125">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="31c22-126">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="31c22-126">Fixed price</span></span>

<span data-ttu-id="31c22-127">כאשר ערך הוצאה בסיסית שנשלח מקושר לפרוייקט הממופה לסעיף חוזה של מחיר קבוע, המערכת יוצרת שורת יומן אחת עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="31c22-127">When a submitted basic expense entry is linked to a project that's mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="31c22-128">תמחור ברירת מחדל</span><span class="sxs-lookup"><span data-stu-id="31c22-128">Default pricing</span></span>

<span data-ttu-id="31c22-129">הלוגיקה להזנת מחירי ברירת מחדל להוצאות מבוססת על קטגוריית ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="31c22-129">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="31c22-130">תאריך העסקה, סעיף החוזה שאליו ממופה הפרוייקט והמטבע משמשים כולם כדי לקבוע את המחירון המתאים.</span><span class="sxs-lookup"><span data-stu-id="31c22-130">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="31c22-131">שדות המשפיעים על תמחור ברירת המחדל, כגון **‏‫קטגוריית עסקה‬** ו **‏‫יחידה‬**, משמשים לקביעת המחיר המתאים בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="31c22-131">The fields that affect default pricing, such as **Transaction Category** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="31c22-132">עם זאת, זה עובד רק כאשר שיטת התמחור במחירון היא **מחיר ליחידה**.</span><span class="sxs-lookup"><span data-stu-id="31c22-132">However, this only works when the pricing method in the price list is **Price per unit**.</span></span> <span data-ttu-id="31c22-133">אם שיטת התמחור היא **‏‫לפי עלות‬** או **ייקור מעל לעלות**, המחיר שהוזן בעת ערך ההוצאה משמש עבור עלות, והמחיר בשורת יומן המכירות מחושב לפי שיטת התמחור.</span><span class="sxs-lookup"><span data-stu-id="31c22-133">If pricing method is **At cost** or **Markup over cost**, the price entered when the expense entry is created is used for cost and the price on the sales journal line is calculated based on the pricing method.</span></span> 

<span data-ttu-id="31c22-134">באפשרותך להוסיף שדה מותאם אישית בערך ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="31c22-134">You can add a custom field on the expense entry.</span></span> <span data-ttu-id="31c22-135">אם ברצונך שערך השדה יופץ לנתונים בפועל, צור את השדה בטבלאות **נתונים בפועל** ו **שורת יומן**.</span><span class="sxs-lookup"><span data-stu-id="31c22-135">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="31c22-136">השתמש בקוד מותאם אישית כדי להפיץ את ערך השדה שנבחר מ'‏‫ערך זמן‬' ל'נתונים בפועל' דרך שורת היומן באמצעות מקורות העסקה.</span><span class="sxs-lookup"><span data-stu-id="31c22-136">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="31c22-137">למידע נוסף על מקורות העסקה וחיבורים, ראה [קישור נתונים בפועל לרשומות מקוריות](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="31c22-137">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-material-usage-log-submission"></a><span data-ttu-id="31c22-138">הגשת יומן של שורות יומן ושימוש בחומרים</span><span class="sxs-lookup"><span data-stu-id="31c22-138">Journal lines and material usage log submission</span></span>

<span data-ttu-id="31c22-139">לקבלת מידע נוסף אודות הזנת הוצאה, ראה [יומן שימוש בחומרים](../material/material-usage-log.md).</span><span class="sxs-lookup"><span data-stu-id="31c22-139">For more information about expense entry, see [Material Usage Log](../material/material-usage-log.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="31c22-140">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="31c22-140">Time and materials</span></span>

<span data-ttu-id="31c22-141">כאשר ערך ביומן השימוש בחומרים שנשלח מקושר לפרויקט הממופה לשורת חוזה של זמן וחומרים, המערכת יוצרת שתי שורות יומן, אחת עבור עלות ואחת עבור מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="31c22-141">When a submitted material usage log entry is linked to a project that is mapped to a time and materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="31c22-142">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="31c22-142">Fixed price</span></span>

<span data-ttu-id="31c22-143">כאשר ערך ביומן השימוש בחומרים שנשלח מקושר לפרוייקט הממופה לסעיף חוזה של מחיר קבוע, המערכת יוצרת שורת יומן אחת עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="31c22-143">When a submitted material usage log entry is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="31c22-144">תמחור ברירת מחדל</span><span class="sxs-lookup"><span data-stu-id="31c22-144">Default pricing</span></span>

<span data-ttu-id="31c22-145">ההיגיון להזנת מחירי ברירת מחדל עבור חומר מבוסס על שילוב המוצר והיחידה.</span><span class="sxs-lookup"><span data-stu-id="31c22-145">The logic for entering default prices for material is based on the product and unit combination.</span></span> <span data-ttu-id="31c22-146">תאריך העסקה, סעיף החוזה שאליו ממופה הפרוייקט והמטבע משמשים כולם כדי לקבוע את המחירון המתאים.</span><span class="sxs-lookup"><span data-stu-id="31c22-146">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="31c22-147">שדות המשפיעים על תמחור ברירת המחדל, כגון **מזהה מוצר** ו **‏‫יחידה‬**, משמשים לקביעת המחיר המתאים בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="31c22-147">The fields that affect default pricing, such as **Product ID** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="31c22-148">עם זאת, זה עובד רק עבור מוצרי קטלוג.</span><span class="sxs-lookup"><span data-stu-id="31c22-148">However, this only works for catalog products.</span></span> <span data-ttu-id="31c22-149">עבור מוצרים שאינם מופיעים ברשימה, המחיר שהוזן בעת יצירת ערך ביומן השימוש בחומרים משמש עבור עלות ומחיר מכירה בשורות היומן.</span><span class="sxs-lookup"><span data-stu-id="31c22-149">For write-in products, the price entered when the material usage log entry is created is used for cost and sales price on the journal lines.</span></span> 

<span data-ttu-id="31c22-150">באפשרותך להוסיף שדה מותאם אישית בערך **‏‫יומן רישום של שימוש בחומרים‬**.</span><span class="sxs-lookup"><span data-stu-id="31c22-150">You can add a custom field on the **Material Usage Log** entry.</span></span> <span data-ttu-id="31c22-151">אם ברצונך שערך השדה יופץ לנתונים בפועל, צור את השדה בטבלאות **נתונים בפועל** ו **שורת יומן**.</span><span class="sxs-lookup"><span data-stu-id="31c22-151">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="31c22-152">השתמש בקוד מותאם אישית כדי להפיץ את ערך השדה שנבחר מ'‏‫ערך זמן‬' ל'נתונים בפועל' דרך שורת היומן באמצעות מקורות העסקה.</span><span class="sxs-lookup"><span data-stu-id="31c22-152">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="31c22-153">למידע נוסף על מקורות העסקה וחיבורים, ראה [קישור נתונים בפועל לרשומות מקוריות](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="31c22-153">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="31c22-154">שימוש ביומני ערכים לתיעוד עלויות</span><span class="sxs-lookup"><span data-stu-id="31c22-154">Use entry journals to record costs</span></span>

<span data-ttu-id="31c22-155">יומני ערכים מאפשרים לך לתעד עלות או הכנסה במחלקות החומר, התשלום, הזמן, ההוצאה או עסקאות מס.</span><span class="sxs-lookup"><span data-stu-id="31c22-155">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="31c22-156">ניתן להשתמש ביומנים למטרות הבאות:</span><span class="sxs-lookup"><span data-stu-id="31c22-156">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="31c22-157">נתונים בפועל נוספים על עסקאות ממערכת אחרת ל- Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="31c22-157">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="31c22-158">רישום עלויות שהתרחשו במערכת אחרת.</span><span class="sxs-lookup"><span data-stu-id="31c22-158">Record costs that occurred in another system.</span></span> <span data-ttu-id="31c22-159">עלויות אלה יכולות לכלול עלויות רכש או קבלנות משנה.</span><span class="sxs-lookup"><span data-stu-id="31c22-159">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="31c22-160">היישום אינו מאמת את סוג שורת היומן או את התמחור הקשור שמזינים בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="31c22-160">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="31c22-161">לכן, כדאי שרק משתמש שמודע לחלוטין להשפעה החשבונאית שיש נתונים בפועל על הפרויקט, ישתמש ביומני ערך ליצירת נתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="31c22-161">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="31c22-162">בגלל ההשפעה של סוג יומן זה, עליך לבחור בקפידה למי יש גישה ליצירת יומני ערך.</span><span class="sxs-lookup"><span data-stu-id="31c22-162">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>

## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="31c22-163">תיעוד נתונים בפועל בהתבסס על אירועי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-163">Record actuals based on project events</span></span>

<span data-ttu-id="31c22-164">Project Operations מתעד את העסקות הפיננסיות המתרחשות במהלך פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="31c22-164">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="31c22-165">עסקאות אלה מתועדות כנתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="31c22-165">These transactions are recorded as actuals.</span></span> <span data-ttu-id="31c22-166">הטבלאות הבאות מציגות את הסוגים השונים של נתונים בפועל שנוצרים, בהתאם לשאלה אם הפרוייקט הוא פרוייקט של זמן וחומרים פרוייקט במחיר קבוע, פרוייקט שנמצא בשלב קדם המכירות או פרוייקט פנימי.</span><span class="sxs-lookup"><span data-stu-id="31c22-166">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="31c22-167">המשאב משתייך לאותה יחידה ארגונית כשל יחידת החוזה של הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-167">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="31c22-168">אירוע</span><span class="sxs-lookup"><span data-stu-id="31c22-168">Event</span></span></th>
<th colspan="4"><span data-ttu-id="31c22-169">פרוייקט לחיוב או פרוייקט שנמכר</span><span class="sxs-lookup"><span data-stu-id="31c22-169">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="31c22-170">פרוייקט בשלב הקדם-מכירות</span><span class="sxs-lookup"><span data-stu-id="31c22-170">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="31c22-171">פרוייקט פנימי</span><span class="sxs-lookup"><span data-stu-id="31c22-171">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="31c22-172">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="31c22-172">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="31c22-173">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="31c22-173">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="31c22-174">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="31c22-174">Actuals</span></span></th>
<th><span data-ttu-id="31c22-175">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="31c22-175">Transaction currency</span></span></th>
<th><span data-ttu-id="31c22-176">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="31c22-176">Fixed price</span></span></th>
<th><span data-ttu-id="31c22-177">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="31c22-177">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="31c22-178">ערך זמן נוצר.</span><span class="sxs-lookup"><span data-stu-id="31c22-178">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="31c22-179">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="31c22-179">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-180">ערך זמן נשלח.</span><span class="sxs-lookup"><span data-stu-id="31c22-180">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="31c22-181">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="31c22-181">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="31c22-182">הזמן מאושר, ואין שינוי או עלייה בשעות לחיוב במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="31c22-182">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="31c22-183">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="31c22-183">Cost actual</span></span></td>
<td><span data-ttu-id="31c22-184">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="31c22-184">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="31c22-185">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="31c22-185">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="31c22-186">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="31c22-186">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="31c22-187">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="31c22-187">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="31c22-188">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="31c22-188">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-189">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="31c22-189">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="31c22-190">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="31c22-191">הזמן מאושר, וירידה בשעות לחיוב מתרחשת במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="31c22-191">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="31c22-192">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="31c22-192">Cost actual</span></span></td>
<td><span data-ttu-id="31c22-193">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="31c22-193">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="31c22-194">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="31c22-194">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="31c22-195">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="31c22-195">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="31c22-196">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="31c22-196">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="31c22-197">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="31c22-197">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-198">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="31c22-198">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="31c22-199">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-199">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-200">נתון בפועל של מכירות שלא חויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="31c22-200">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="31c22-201">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-201">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="31c22-202">חשבונית מאושרת, ואין שינוי או עלייה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="31c22-202">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="31c22-203">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="31c22-203">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="31c22-204">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-204">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="31c22-205">מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="31c22-205">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="31c22-206">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-206">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="31c22-207">לא ישים</span><span class="sxs-lookup"><span data-stu-id="31c22-207">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="31c22-208">לא ישים</span><span class="sxs-lookup"><span data-stu-id="31c22-208">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-209">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="31c22-209">Billed sales</span></span></td>
<td><span data-ttu-id="31c22-210">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-210">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="31c22-211">חשבונית מאושרת, ומתרחשת ירידה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="31c22-211">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="31c22-212">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="31c22-212">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="31c22-213">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-213">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="31c22-214">לא ישים</span><span class="sxs-lookup"><span data-stu-id="31c22-214">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="31c22-215">לא ישים</span><span class="sxs-lookup"><span data-stu-id="31c22-215">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="31c22-216">לא ישים</span><span class="sxs-lookup"><span data-stu-id="31c22-216">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="31c22-217">לא ישים</span><span class="sxs-lookup"><span data-stu-id="31c22-217">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-218">מכירות שחויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="31c22-218">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="31c22-219">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-219">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-220">מכירות שחויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="31c22-220">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="31c22-221">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-221">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="31c22-222">החשבונית מתוקנת כדי להגדיל את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="31c22-222">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="31c22-223">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="31c22-223">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="31c22-224">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-224">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="31c22-225">ביטול מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="31c22-225">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="31c22-226">שינוי במצב אבן דרך ממצב <strong>הוגשה חשבונית</strong> למצב <strong>מוכן להפקת חשבונית</strong></span><span class="sxs-lookup"><span data-stu-id="31c22-226">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="31c22-227">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-227">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="31c22-228">לא ישים</span><span class="sxs-lookup"><span data-stu-id="31c22-228">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="31c22-229">לא ישים</span><span class="sxs-lookup"><span data-stu-id="31c22-229">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-230">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="31c22-230">Billed sales</span></span></td>
<td><span data-ttu-id="31c22-231">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-231">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="31c22-232">החשבונית מתוקנת כדי להקטין את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="31c22-232">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="31c22-233">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="31c22-233">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="31c22-234">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-235">מכירות שחויבו עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="31c22-235">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="31c22-236">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-236">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-237">מכירות שלא חויבו - ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="31c22-237">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="31c22-238">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-238">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="31c22-239">המשאב משתייך ליחידה ארגונית השונה מיחידת החוזה של הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-239">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="31c22-240">אירוע</span><span class="sxs-lookup"><span data-stu-id="31c22-240">Event</span></span></th>
<th colspan="4"><span data-ttu-id="31c22-241">פרוייקט לחיוב או פרוייקט שנמכר</span><span class="sxs-lookup"><span data-stu-id="31c22-241">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="31c22-242">פרוייקט בשלב הקדם-מכירות</span><span class="sxs-lookup"><span data-stu-id="31c22-242">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="31c22-243">פרוייקט פנימי</span><span class="sxs-lookup"><span data-stu-id="31c22-243">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="31c22-244">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="31c22-244">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="31c22-245">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="31c22-245">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="31c22-246">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="31c22-246">Actuals</span></span></th>
<th><span data-ttu-id="31c22-247">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="31c22-247">Transaction currency</span></span></th>
<th><span data-ttu-id="31c22-248">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="31c22-248">Fixed price</span></span></th>
<th><span data-ttu-id="31c22-249">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="31c22-249">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="31c22-250">ערך זמן נוצר.</span><span class="sxs-lookup"><span data-stu-id="31c22-250">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="31c22-251">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="31c22-251">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-252">ערך זמן נשלח.</span><span class="sxs-lookup"><span data-stu-id="31c22-252">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="31c22-253">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="31c22-253">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="31c22-254">הזמן מאושר, ואין שינוי או עלייה בשעות לחיוב במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="31c22-254">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="31c22-255">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="31c22-255">Cost actual</span></span></td>
<td><span data-ttu-id="31c22-256">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="31c22-256">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="31c22-257">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="31c22-257">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="31c22-258">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="31c22-258">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="31c22-259">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="31c22-259">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="31c22-260">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="31c22-260">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-261">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="31c22-261">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="31c22-262">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-262">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-263">עלות יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="31c22-263">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="31c22-264">מטבע של יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="31c22-264">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-265">מכירות בין-ארגוניות</span><span class="sxs-lookup"><span data-stu-id="31c22-265">Interorganizational sales</span></span></td>
<td><span data-ttu-id="31c22-266">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="31c22-266">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="31c22-267">הזמן מאושר, וירידה בשעות לחיוב מתרחשת במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="31c22-267">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="31c22-268">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="31c22-268">Cost actual</span></span></td>
<td><span data-ttu-id="31c22-269">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="31c22-269">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="31c22-270">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="31c22-270">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="31c22-271">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="31c22-271">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="31c22-272">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="31c22-272">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="31c22-273">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="31c22-273">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-274">עלות יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="31c22-274">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="31c22-275">מטבע של יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="31c22-275">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-276">מכירות בין-ארגוניות</span><span class="sxs-lookup"><span data-stu-id="31c22-276">Interorganizational sales</span></span></td>
<td><span data-ttu-id="31c22-277">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="31c22-277">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-278">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="31c22-278">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="31c22-279">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-279">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-280">נתון בפועל של מכירות שלא חויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="31c22-280">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="31c22-281">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-281">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="31c22-282">חשבונית מאושרת, ואין שינוי או עלייה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="31c22-282">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="31c22-283">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="31c22-283">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="31c22-284">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-284">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="31c22-285">מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="31c22-285">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="31c22-286">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-286">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="31c22-287">לא ישים</span><span class="sxs-lookup"><span data-stu-id="31c22-287">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="31c22-288">לא ישים</span><span class="sxs-lookup"><span data-stu-id="31c22-288">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-289">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="31c22-289">Billed sales</span></span></td>
<td><span data-ttu-id="31c22-290">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-290">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="31c22-291">חשבונית מאושרת, ומתרחשת ירידה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="31c22-291">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="31c22-292">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="31c22-292">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="31c22-293">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-293">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="31c22-294">לא ישים</span><span class="sxs-lookup"><span data-stu-id="31c22-294">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="31c22-295">לא ישים</span><span class="sxs-lookup"><span data-stu-id="31c22-295">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="31c22-296">לא ישים</span><span class="sxs-lookup"><span data-stu-id="31c22-296">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="31c22-297">לא ישים</span><span class="sxs-lookup"><span data-stu-id="31c22-297">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-298">מכירות שחויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="31c22-298">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="31c22-299">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-299">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-300">מכירות שחויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="31c22-300">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="31c22-301">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-301">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="31c22-302">החשבונית מתוקנת כדי להגדיל את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="31c22-302">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="31c22-303">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="31c22-303">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="31c22-304">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-304">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="31c22-305">ביטול מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="31c22-305">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="31c22-306">שינוי במצב אבן דרך ממצב <strong>הוגשה חשבונית</strong> למצב <strong>מוכן להפקת חשבונית</strong></span><span class="sxs-lookup"><span data-stu-id="31c22-306">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="31c22-307">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-307">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="31c22-308">לא ישים</span><span class="sxs-lookup"><span data-stu-id="31c22-308">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="31c22-309">לא ישים</span><span class="sxs-lookup"><span data-stu-id="31c22-309">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-310">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="31c22-310">Billed sales</span></span></td>
<td><span data-ttu-id="31c22-311">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-311">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="31c22-312">החשבונית מתוקנת כדי להקטין את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="31c22-312">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="31c22-313">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="31c22-313">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="31c22-314">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-314">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-315">מכירות שחויבו עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="31c22-315">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="31c22-316">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-316">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="31c22-317">מכירות שלא חויבו - ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="31c22-317">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="31c22-318">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="31c22-318">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
