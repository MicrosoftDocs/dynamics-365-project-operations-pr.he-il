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
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 78c7a9486d0338adfd7770447f21d17509e654f7
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996612"
---
# <a name="actuals"></a><span data-ttu-id="95adb-103">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="95adb-103">Actuals</span></span> 

<span data-ttu-id="95adb-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="95adb-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="95adb-105">‏‫נתונים בפועל‬ מייצגים את ההתקדמות הכספית והתקדמות לוח הזמנים שנבדקה ואושרה בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="95adb-105">Actuals represent the reviewed and approved financial and schedule progress on a project.</span></span> <span data-ttu-id="95adb-106">הם נוצרים כתוצאה מאישור זמן, הוצאות, ערכי שימוש בחומרים וערכים ביומן וחשבוניות.</span><span class="sxs-lookup"><span data-stu-id="95adb-106">They are created as a result of approval of time, expense, material usage entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="95adb-107">שורות יומן והגשת זמן</span><span class="sxs-lookup"><span data-stu-id="95adb-107">Journal lines and time submission</span></span>

<span data-ttu-id="95adb-108">לקבלת מידע נוסף אודות ערך זמן, ראה [מבט כולל על ערך זמן](../time/time-entry-overview.md).</span><span class="sxs-lookup"><span data-stu-id="95adb-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="95adb-109">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="95adb-109">Time and materials</span></span>

<span data-ttu-id="95adb-110">כאשר ערך זמן שמוגש מקושר לפרויקט הממופה לסעיף חוזה של זמן וחומרים, המערכת יוצרת שתי שורות יומן, אחת עובר עלות ואחת עבור מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="95adb-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="95adb-111">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="95adb-111">Fixed price</span></span>

<span data-ttu-id="95adb-112">כאשר ערך זמן שמוגש מקושר לפרוייקט הממופה לסעיף חוזה במחיר קבוע, המערכת יוצרת שורת יומן אחת עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="95adb-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="95adb-113">תמחור ברירת מחדל</span><span class="sxs-lookup"><span data-stu-id="95adb-113">Default pricing</span></span>

<span data-ttu-id="95adb-114">הלוגיקה ליצירת מחירי ברירת מחדל נמצאת בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="95adb-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="95adb-115">ערכי השדות מערך הזמן מועתקים לשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="95adb-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="95adb-116">ערכים אלה כוללים את תאריך העסקה, את סעיף החוזה שאליו ממופה הפרוייקט ואת תוצאת המטבע במחירון המתאים.</span><span class="sxs-lookup"><span data-stu-id="95adb-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="95adb-117">שדות המשפיעים על תמחור ברירת המחדל, כגון **תפקיד** ו **‏‫יחידת הקצאת משאבים‬**, משמשים לקביעת המחיר המתאים בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="95adb-117">The fields that affect default pricing, such as **Role** and **Resourcing Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="95adb-118">ניתן להוסיף שדה מותאם אישית בערך הזמן.</span><span class="sxs-lookup"><span data-stu-id="95adb-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="95adb-119">אם ברצונך שערך השדה יופץ לנתונים בפועל, צור את השדה בטבלאות **נתונים בפועל** ו **שורת יומן**.</span><span class="sxs-lookup"><span data-stu-id="95adb-119">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="95adb-120">השתמש בקוד מותאם אישית כדי להפיץ את ערך השדה שנבחר מ'‏‫ערך זמן‬' ל'נתונים בפועל' דרך שורת היומן באמצעות מקורות העסקה.</span><span class="sxs-lookup"><span data-stu-id="95adb-120">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="95adb-121">למידע נוסף על מקורות העסקה וחיבורים, ראה [קישור נתונים בפועל לרשומות מקוריות](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="95adb-121">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="95adb-122">שורות יומן והגשת הוצאות בסיסיות</span><span class="sxs-lookup"><span data-stu-id="95adb-122">Journal lines and basic expense submission</span></span>

<span data-ttu-id="95adb-123">לקבלת מידע נוסף אודות ערכי הוצאה, ראה [מבט כולל על ערכי הוצאה](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="95adb-123">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="95adb-124">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="95adb-124">Time and materials</span></span>

<span data-ttu-id="95adb-125">כאשר ערך הוצאה בסיסית שמוגש מקושר לפרויקט הממופה לסעיף חוזה של זמן וחומרים, המערכת יוצרת שתי שורות יומן, אחת עבור עלות ואחת עבור מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="95adb-125">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="95adb-126">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="95adb-126">Fixed price</span></span>

<span data-ttu-id="95adb-127">כאשר ערך הוצאה בסיסית שנשלח מקושר לפרוייקט הממופה לסעיף חוזה של מחיר קבוע, המערכת יוצרת שורת יומן אחת עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="95adb-127">When a submitted basic expense entry is linked to a project that's mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="95adb-128">תמחור ברירת מחדל</span><span class="sxs-lookup"><span data-stu-id="95adb-128">Default pricing</span></span>

<span data-ttu-id="95adb-129">הלוגיקה להזנת מחירי ברירת מחדל להוצאות מבוססת על קטגוריית ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="95adb-129">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="95adb-130">תאריך העסקה, סעיף החוזה שאליו ממופה הפרוייקט והמטבע משמשים כולם כדי לקבוע את המחירון המתאים.</span><span class="sxs-lookup"><span data-stu-id="95adb-130">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="95adb-131">שדות המשפיעים על תמחור ברירת המחדל, כגון **‏‫קטגוריית עסקה‬** ו **‏‫יחידה‬**, משמשים לקביעת המחיר המתאים בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="95adb-131">The fields that affect default pricing, such as **Transaction Category** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="95adb-132">עם זאת, זה עובד רק כאשר שיטת התמחור במחירון היא **מחיר ליחידה**.</span><span class="sxs-lookup"><span data-stu-id="95adb-132">However, this only works when the pricing method in the price list is **Price per unit**.</span></span> <span data-ttu-id="95adb-133">אם שיטת התמחור היא **‏‫לפי עלות‬** או **ייקור מעל לעלות**, המחיר שהוזן בעת ערך ההוצאה משמש עבור עלות, והמחיר בשורת יומן המכירות מחושב לפי שיטת התמחור.</span><span class="sxs-lookup"><span data-stu-id="95adb-133">If pricing method is **At cost** or **Markup over cost**, the price entered when the expense entry is created is used for cost and the price on the sales journal line is calculated based on the pricing method.</span></span> 

<span data-ttu-id="95adb-134">באפשרותך להוסיף שדה מותאם אישית בערך ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="95adb-134">You can add a custom field on the expense entry.</span></span> <span data-ttu-id="95adb-135">אם ברצונך שערך השדה יופץ לנתונים בפועל, צור את השדה בטבלאות **נתונים בפועל** ו **שורת יומן**.</span><span class="sxs-lookup"><span data-stu-id="95adb-135">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="95adb-136">השתמש בקוד מותאם אישית כדי להפיץ את ערך השדה שנבחר מ'‏‫ערך זמן‬' ל'נתונים בפועל' דרך שורת היומן באמצעות מקורות העסקה.</span><span class="sxs-lookup"><span data-stu-id="95adb-136">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="95adb-137">למידע נוסף על מקורות העסקה וחיבורים, ראה [קישור נתונים בפועל לרשומות מקוריות](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="95adb-137">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-material-usage-log-submission"></a><span data-ttu-id="95adb-138">הגשת יומן של שורות יומן ושימוש בחומרים</span><span class="sxs-lookup"><span data-stu-id="95adb-138">Journal lines and material usage log submission</span></span>

<span data-ttu-id="95adb-139">לקבלת מידע נוסף אודות הזנת הוצאה, ראה [יומן שימוש בחומרים](../material/material-usage-log.md).</span><span class="sxs-lookup"><span data-stu-id="95adb-139">For more information about expense entry, see [Material Usage Log](../material/material-usage-log.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="95adb-140">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="95adb-140">Time and materials</span></span>

<span data-ttu-id="95adb-141">כאשר ערך ביומן השימוש בחומרים שנשלח מקושר לפרויקט הממופה לשורת חוזה של זמן וחומרים, המערכת יוצרת שתי שורות יומן, אחת עבור עלות ואחת עבור מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="95adb-141">When a submitted material usage log entry is linked to a project that is mapped to a time and materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="95adb-142">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="95adb-142">Fixed price</span></span>

<span data-ttu-id="95adb-143">כאשר ערך ביומן השימוש בחומרים שנשלח מקושר לפרוייקט הממופה לסעיף חוזה של מחיר קבוע, המערכת יוצרת שורת יומן אחת עבור עלות.</span><span class="sxs-lookup"><span data-stu-id="95adb-143">When a submitted material usage log entry is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="95adb-144">תמחור ברירת מחדל</span><span class="sxs-lookup"><span data-stu-id="95adb-144">Default pricing</span></span>

<span data-ttu-id="95adb-145">ההיגיון להזנת מחירי ברירת מחדל עבור חומר מבוסס על שילוב המוצר והיחידה.</span><span class="sxs-lookup"><span data-stu-id="95adb-145">The logic for entering default prices for material is based on the product and unit combination.</span></span> <span data-ttu-id="95adb-146">תאריך העסקה, סעיף החוזה שאליו ממופה הפרוייקט והמטבע משמשים כולם כדי לקבוע את המחירון המתאים.</span><span class="sxs-lookup"><span data-stu-id="95adb-146">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="95adb-147">שדות המשפיעים על תמחור ברירת המחדל, כגון **מזהה מוצר** ו **‏‫יחידה‬**, משמשים לקביעת המחיר המתאים בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="95adb-147">The fields that affect default pricing, such as **Product ID** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="95adb-148">עם זאת, זה עובד רק עבור מוצרי קטלוג.</span><span class="sxs-lookup"><span data-stu-id="95adb-148">However, this only works for catalog products.</span></span> <span data-ttu-id="95adb-149">עבור מוצרים שאינם מופיעים ברשימה, המחיר שהוזן בעת יצירת ערך ביומן השימוש בחומרים משמש עבור עלות ומחיר מכירה בשורות היומן.</span><span class="sxs-lookup"><span data-stu-id="95adb-149">For write-in products, the price entered when the material usage log entry is created is used for cost and sales price on the journal lines.</span></span> 

<span data-ttu-id="95adb-150">באפשרותך להוסיף שדה מותאם אישית בערך **‏‫יומן רישום של שימוש בחומרים‬**.</span><span class="sxs-lookup"><span data-stu-id="95adb-150">You can add a custom field on the **Material Usage Log** entry.</span></span> <span data-ttu-id="95adb-151">אם ברצונך שערך השדה יופץ לנתונים בפועל, צור את השדה בטבלאות **נתונים בפועל** ו **שורת יומן**.</span><span class="sxs-lookup"><span data-stu-id="95adb-151">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="95adb-152">השתמש בקוד מותאם אישית כדי להפיץ את ערך השדה שנבחר מ'‏‫ערך זמן‬' ל'נתונים בפועל' דרך שורת היומן באמצעות מקורות העסקה.</span><span class="sxs-lookup"><span data-stu-id="95adb-152">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="95adb-153">למידע נוסף על מקורות העסקה וחיבורים, ראה [קישור נתונים בפועל לרשומות מקוריות](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="95adb-153">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="95adb-154">שימוש ביומני ערכים לתיעוד עלויות</span><span class="sxs-lookup"><span data-stu-id="95adb-154">Use entry journals to record costs</span></span>

<span data-ttu-id="95adb-155">יומני ערכים מאפשרים לך לתעד עלות או הכנסה במחלקות החומר, התשלום, הזמן, ההוצאה או עסקאות מס.</span><span class="sxs-lookup"><span data-stu-id="95adb-155">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="95adb-156">ניתן להשתמש ביומנים למטרות הבאות:</span><span class="sxs-lookup"><span data-stu-id="95adb-156">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="95adb-157">נתונים בפועל נוספים על עסקאות ממערכת אחרת ל- Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="95adb-157">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="95adb-158">רישום עלויות שהתרחשו במערכת אחרת.</span><span class="sxs-lookup"><span data-stu-id="95adb-158">Record costs that occurred in another system.</span></span> <span data-ttu-id="95adb-159">עלויות אלה יכולות לכלול עלויות רכש או קבלנות משנה.</span><span class="sxs-lookup"><span data-stu-id="95adb-159">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="95adb-160">היישום אינו מאמת את סוג שורת היומן או את התמחור הקשור שמזינים בשורת היומן.</span><span class="sxs-lookup"><span data-stu-id="95adb-160">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="95adb-161">לכן, כדאי שרק משתמש שמודע לחלוטין להשפעה החשבונאית שיש נתונים בפועל על הפרויקט, ישתמש ביומני ערך ליצירת נתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="95adb-161">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="95adb-162">בגלל ההשפעה של סוג יומן זה, עליך לבחור בקפידה למי יש גישה ליצירת יומני ערך.</span><span class="sxs-lookup"><span data-stu-id="95adb-162">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>

## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="95adb-163">תיעוד נתונים בפועל בהתבסס על אירועי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-163">Record actuals based on project events</span></span>

<span data-ttu-id="95adb-164">Project Operations מתעד את העסקות הפיננסיות המתרחשות במהלך פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="95adb-164">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="95adb-165">עסקאות אלה מתועדות כנתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="95adb-165">These transactions are recorded as actuals.</span></span> <span data-ttu-id="95adb-166">הטבלאות הבאות מציגות את הסוגים השונים של נתונים בפועל שנוצרים, בהתאם לשאלה אם הפרוייקט הוא פרוייקט של זמן וחומרים פרוייקט במחיר קבוע, פרוייקט שנמצא בשלב קדם המכירות או פרוייקט פנימי.</span><span class="sxs-lookup"><span data-stu-id="95adb-166">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="95adb-167">המשאב משתייך לאותה יחידה ארגונית כשל יחידת החוזה של הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-167">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="95adb-168">אירוע</span><span class="sxs-lookup"><span data-stu-id="95adb-168">Event</span></span></th>
<th colspan="4"><span data-ttu-id="95adb-169">פרוייקט לחיוב או פרוייקט שנמכר</span><span class="sxs-lookup"><span data-stu-id="95adb-169">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="95adb-170">פרוייקט בשלב הקדם-מכירות</span><span class="sxs-lookup"><span data-stu-id="95adb-170">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="95adb-171">פרוייקט פנימי</span><span class="sxs-lookup"><span data-stu-id="95adb-171">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="95adb-172">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="95adb-172">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="95adb-173">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="95adb-173">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="95adb-174">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="95adb-174">Actuals</span></span></th>
<th><span data-ttu-id="95adb-175">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="95adb-175">Transaction currency</span></span></th>
<th><span data-ttu-id="95adb-176">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="95adb-176">Fixed price</span></span></th>
<th><span data-ttu-id="95adb-177">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="95adb-177">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="95adb-178">ערך זמן נוצר.</span><span class="sxs-lookup"><span data-stu-id="95adb-178">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="95adb-179">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="95adb-179">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-180">ערך זמן נשלח.</span><span class="sxs-lookup"><span data-stu-id="95adb-180">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="95adb-181">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="95adb-181">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="95adb-182">הזמן מאושר, ואין שינוי או עלייה בשעות לחיוב במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="95adb-182">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="95adb-183">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="95adb-183">Cost actual</span></span></td>
<td><span data-ttu-id="95adb-184">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="95adb-184">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="95adb-185">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="95adb-185">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="95adb-186">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="95adb-186">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="95adb-187">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="95adb-187">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="95adb-188">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="95adb-188">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-189">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="95adb-189">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="95adb-190">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="95adb-191">הזמן מאושר, וירידה בשעות לחיוב מתרחשת במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="95adb-191">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="95adb-192">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="95adb-192">Cost actual</span></span></td>
<td><span data-ttu-id="95adb-193">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="95adb-193">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="95adb-194">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="95adb-194">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="95adb-195">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="95adb-195">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="95adb-196">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="95adb-196">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="95adb-197">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="95adb-197">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-198">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="95adb-198">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="95adb-199">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-199">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-200">נתון בפועל של מכירות שלא חויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="95adb-200">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="95adb-201">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-201">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="95adb-202">חשבונית מאושרת, ואין שינוי או עלייה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="95adb-202">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="95adb-203">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="95adb-203">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="95adb-204">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-204">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="95adb-205">מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="95adb-205">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="95adb-206">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-206">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="95adb-207">לא ישים</span><span class="sxs-lookup"><span data-stu-id="95adb-207">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="95adb-208">לא ישים</span><span class="sxs-lookup"><span data-stu-id="95adb-208">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-209">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="95adb-209">Billed sales</span></span></td>
<td><span data-ttu-id="95adb-210">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-210">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="95adb-211">חשבונית מאושרת, ומתרחשת ירידה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="95adb-211">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="95adb-212">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="95adb-212">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="95adb-213">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-213">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="95adb-214">לא ישים</span><span class="sxs-lookup"><span data-stu-id="95adb-214">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="95adb-215">לא ישים</span><span class="sxs-lookup"><span data-stu-id="95adb-215">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="95adb-216">לא ישים</span><span class="sxs-lookup"><span data-stu-id="95adb-216">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="95adb-217">לא ישים</span><span class="sxs-lookup"><span data-stu-id="95adb-217">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-218">מכירות שחויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="95adb-218">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="95adb-219">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-219">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-220">מכירות שחויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="95adb-220">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="95adb-221">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-221">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="95adb-222">החשבונית מתוקנת כדי להגדיל את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="95adb-222">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="95adb-223">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="95adb-223">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="95adb-224">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-224">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="95adb-225">ביטול מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="95adb-225">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="95adb-226">שינוי במצב אבן דרך ממצב <strong>הוגשה חשבונית</strong> למצב <strong>מוכן להפקת חשבונית</strong></span><span class="sxs-lookup"><span data-stu-id="95adb-226">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="95adb-227">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-227">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="95adb-228">לא ישים</span><span class="sxs-lookup"><span data-stu-id="95adb-228">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="95adb-229">לא ישים</span><span class="sxs-lookup"><span data-stu-id="95adb-229">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-230">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="95adb-230">Billed sales</span></span></td>
<td><span data-ttu-id="95adb-231">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-231">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="95adb-232">החשבונית מתוקנת כדי להקטין את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="95adb-232">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="95adb-233">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="95adb-233">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="95adb-234">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-235">מכירות שחויבו עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="95adb-235">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="95adb-236">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-236">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-237">מכירות שלא חויבו - ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="95adb-237">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="95adb-238">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-238">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="95adb-239">המשאב משתייך ליחידה ארגונית השונה מיחידת החוזה של הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-239">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="95adb-240">אירוע</span><span class="sxs-lookup"><span data-stu-id="95adb-240">Event</span></span></th>
<th colspan="4"><span data-ttu-id="95adb-241">פרוייקט לחיוב או פרוייקט שנמכר</span><span class="sxs-lookup"><span data-stu-id="95adb-241">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="95adb-242">פרוייקט בשלב הקדם-מכירות</span><span class="sxs-lookup"><span data-stu-id="95adb-242">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="95adb-243">פרוייקט פנימי</span><span class="sxs-lookup"><span data-stu-id="95adb-243">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="95adb-244">זמן וחומרים</span><span class="sxs-lookup"><span data-stu-id="95adb-244">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="95adb-245">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="95adb-245">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="95adb-246">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="95adb-246">Actuals</span></span></th>
<th><span data-ttu-id="95adb-247">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="95adb-247">Transaction currency</span></span></th>
<th><span data-ttu-id="95adb-248">מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="95adb-248">Fixed price</span></span></th>
<th><span data-ttu-id="95adb-249">מטבע עסקה</span><span class="sxs-lookup"><span data-stu-id="95adb-249">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="95adb-250">ערך זמן נוצר.</span><span class="sxs-lookup"><span data-stu-id="95adb-250">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="95adb-251">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="95adb-251">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-252">ערך זמן נשלח.</span><span class="sxs-lookup"><span data-stu-id="95adb-252">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="95adb-253">אין פעילות בישות 'נתונים בפועל'</span><span class="sxs-lookup"><span data-stu-id="95adb-253">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="95adb-254">הזמן מאושר, ואין שינוי או עלייה בשעות לחיוב במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="95adb-254">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="95adb-255">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="95adb-255">Cost actual</span></span></td>
<td><span data-ttu-id="95adb-256">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="95adb-256">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="95adb-257">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="95adb-257">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="95adb-258">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="95adb-258">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="95adb-259">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="95adb-259">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="95adb-260">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="95adb-260">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-261">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב</span><span class="sxs-lookup"><span data-stu-id="95adb-261">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="95adb-262">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-262">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-263">עלות יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="95adb-263">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="95adb-264">מטבע של יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="95adb-264">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-265">מכירות בין-ארגוניות</span><span class="sxs-lookup"><span data-stu-id="95adb-265">Interorganizational sales</span></span></td>
<td><span data-ttu-id="95adb-266">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="95adb-266">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="95adb-267">הזמן מאושר, וירידה בשעות לחיוב מתרחשת במהלך האישור.</span><span class="sxs-lookup"><span data-stu-id="95adb-267">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="95adb-268">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="95adb-268">Cost actual</span></span></td>
<td><span data-ttu-id="95adb-269">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="95adb-269">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="95adb-270">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="95adb-270">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="95adb-271">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="95adb-271">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="95adb-272">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="95adb-272">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="95adb-273">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="95adb-273">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-274">עלות יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="95adb-274">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="95adb-275">מטבע של יחידת הקצאת משאבים</span><span class="sxs-lookup"><span data-stu-id="95adb-275">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-276">מכירות בין-ארגוניות</span><span class="sxs-lookup"><span data-stu-id="95adb-276">Interorganizational sales</span></span></td>
<td><span data-ttu-id="95adb-277">מטבע של יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="95adb-277">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-278">נתון בפועל של מכירות שלא חויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="95adb-278">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="95adb-279">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-279">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-280">נתון בפועל של מכירות שלא חויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="95adb-280">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="95adb-281">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-281">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="95adb-282">חשבונית מאושרת, ואין שינוי או עלייה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="95adb-282">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="95adb-283">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="95adb-283">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="95adb-284">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-284">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="95adb-285">מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="95adb-285">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="95adb-286">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-286">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="95adb-287">לא ישים</span><span class="sxs-lookup"><span data-stu-id="95adb-287">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="95adb-288">לא ישים</span><span class="sxs-lookup"><span data-stu-id="95adb-288">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-289">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="95adb-289">Billed sales</span></span></td>
<td><span data-ttu-id="95adb-290">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-290">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="95adb-291">חשבונית מאושרת, ומתרחשת ירידה בשעות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="95adb-291">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="95adb-292">ביטול עסקת מכירות שלא חויבה</span><span class="sxs-lookup"><span data-stu-id="95adb-292">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="95adb-293">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-293">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="95adb-294">לא ישים</span><span class="sxs-lookup"><span data-stu-id="95adb-294">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="95adb-295">לא ישים</span><span class="sxs-lookup"><span data-stu-id="95adb-295">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="95adb-296">לא ישים</span><span class="sxs-lookup"><span data-stu-id="95adb-296">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="95adb-297">לא ישים</span><span class="sxs-lookup"><span data-stu-id="95adb-297">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-298">מכירות שחויבו - ניתן לחיוב עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="95adb-298">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="95adb-299">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-299">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-300">מכירות שחויבו - לא ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="95adb-300">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="95adb-301">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-301">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="95adb-302">החשבונית מתוקנת כדי להגדיל את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="95adb-302">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="95adb-303">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="95adb-303">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="95adb-304">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-304">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="95adb-305">ביטול מכירות שחויבו עבור אבן דרך</span><span class="sxs-lookup"><span data-stu-id="95adb-305">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="95adb-306">שינוי במצב אבן דרך ממצב <strong>הוגשה חשבונית</strong> למצב <strong>מוכן להפקת חשבונית</strong></span><span class="sxs-lookup"><span data-stu-id="95adb-306">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="95adb-307">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-307">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="95adb-308">לא ישים</span><span class="sxs-lookup"><span data-stu-id="95adb-308">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="95adb-309">לא ישים</span><span class="sxs-lookup"><span data-stu-id="95adb-309">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-310">מכירות שחויבו</span><span class="sxs-lookup"><span data-stu-id="95adb-310">Billed sales</span></span></td>
<td><span data-ttu-id="95adb-311">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-311">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="95adb-312">החשבונית מתוקנת כדי להקטין את הכמות הניתנת לחיוב.</span><span class="sxs-lookup"><span data-stu-id="95adb-312">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="95adb-313">מכירות שחויבו - ביטול</span><span class="sxs-lookup"><span data-stu-id="95adb-313">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="95adb-314">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-314">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-315">מכירות שחויבו עבור הכמות החדשה</span><span class="sxs-lookup"><span data-stu-id="95adb-315">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="95adb-316">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-316">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="95adb-317">מכירות שלא חויבו - ניתן לחיוב עבור ההפרש</span><span class="sxs-lookup"><span data-stu-id="95adb-317">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="95adb-318">מטבע של חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="95adb-318">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
