---
title: מבט כולל על סעיפי חוזה מבוססי פרוייקט
description: נושא זה מספק מידע על עבודה עם סעיפי חוזה מבוססי פרויקט.
author: rumant
manager: Annbe
ms.date: 10/28/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 824fdd54d7b513b49afd1a6d76d3387df81418e2
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858159"
---
# <a name="project-based-contract-lines-overview"></a><span data-ttu-id="5665f-103">מבט כולל על סעיפי חוזה מבוססי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="5665f-103">Project-based contract lines overview</span></span>

<span data-ttu-id="5665f-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="5665f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5665f-105">סעיפי חוזה מבוססי פרויקטים ב- Dynamics 365 Project Operations נועדו להחזיק את הסכמי ההערכה והחיוב עבור רכיבים ספציפיים בעבודת הפרויקט של ההתקשרות.</span><span class="sxs-lookup"><span data-stu-id="5665f-105">Project-based contract lines in Dynamics 365 Project Operations are designed to hold the estimate and billing agreements for specific components of project work on an engagement.</span></span> <span data-ttu-id="5665f-106">המבנה של סעיף חוזה מבוסס פרויקט מורחב להערכות פרויקט ותרחישי החיוב עם המושגים הבאים:</span><span class="sxs-lookup"><span data-stu-id="5665f-106">The structure of a project–based contract line is extended for project estimates and billing scenarios with the following concepts:</span></span>

- <span data-ttu-id="5665f-107">שיטת חיוב</span><span class="sxs-lookup"><span data-stu-id="5665f-107">Billing method</span></span>
- <span data-ttu-id="5665f-108">מיפוי פרוייקט ומשימות</span><span class="sxs-lookup"><span data-stu-id="5665f-108">Project and task mapping</span></span>
- <span data-ttu-id="5665f-109">סווגי עסקה כלולים</span><span class="sxs-lookup"><span data-stu-id="5665f-109">Included transaction classes</span></span>
- <span data-ttu-id="5665f-110">מגבלת 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="5665f-110">Not-to-exceed limit</span></span>
- <span data-ttu-id="5665f-111">הגדרת יכולת חיוב</span><span class="sxs-lookup"><span data-stu-id="5665f-111">Chargeability setup</span></span>
- <span data-ttu-id="5665f-112">הערכות המשתמשות בפרטי סעיף חוזה</span><span class="sxs-lookup"><span data-stu-id="5665f-112">Estimates using contract line details</span></span>
- <span data-ttu-id="5665f-113">לקוחות סעיף חוזה</span><span class="sxs-lookup"><span data-stu-id="5665f-113">Contract line customers</span></span>

<span data-ttu-id="5665f-114">הטבלה הבאה כוללת את השדות בכרטיסיה **כללי** של סעיפי חוזה מבוססי פרויקטים המסייעים בהגדרת הבסיס להערכה מפורטת ומבוססת והסדרי חיוב עבור עבודה מבוססת פרויקטים.</span><span class="sxs-lookup"><span data-stu-id="5665f-114">The following table includes the fields on the **General** tab of project–based contract lines that help set up the basis for a detailed, ground–up estimate and billing arrangements for project–based work.</span></span>

| <span data-ttu-id="5665f-115">שדה</span><span class="sxs-lookup"><span data-stu-id="5665f-115">Field</span></span> | <span data-ttu-id="5665f-116">תיאור</span><span class="sxs-lookup"><span data-stu-id="5665f-116">Description</span></span> | <span data-ttu-id="5665f-117">השפעה במורד הזרם</span><span class="sxs-lookup"><span data-stu-id="5665f-117">Downstream impact</span></span> |
| --- | --- | --- |
| <span data-ttu-id="5665f-118">**שם**</span><span class="sxs-lookup"><span data-stu-id="5665f-118">**Name**</span></span> | <span data-ttu-id="5665f-119">שם סעיף החוזה.</span><span class="sxs-lookup"><span data-stu-id="5665f-119">Name of the contract line.</span></span> <span data-ttu-id="5665f-120">שם זה מזהה את המרכיב הנפרד של החוזה שמוערך.</span><span class="sxs-lookup"><span data-stu-id="5665f-120">This identifies the discrete component of the contract that is being estimated.</span></span> <span data-ttu-id="5665f-121">עבור חוזה פרויקט שנוצר מהצעת מחיר, ערך זה מועתק מערך מקביל בשורת הצעת המחיר מבוססת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="5665f-121">For a project contract created from a quote, this value is copied from a corresponding value of the project-based quote line.</span></span> | <span data-ttu-id="5665f-122">השם שהועתק לשורת חשבונית הפרויקט שנוצרת מסעיף חוזה זה בעת יצירת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="5665f-122">The name copied over to the project invoice line that is created from this contract line when the invoice is created.</span></span> |
| <span data-ttu-id="5665f-123">**שיטת חיוב**</span><span class="sxs-lookup"><span data-stu-id="5665f-123">**Billing Method**</span></span> | <span data-ttu-id="5665f-124">בחוזה פרויקט שנוצר מהצעת מחיר, ערך זה מועתק מהשדה המקביל בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5665f-124">On a project contract created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="5665f-125">זהו קבוצת אפשרויות המייצג את שני המודלי החוזה העיקריים הנתמכים על ידי Project Operations:</span><span class="sxs-lookup"><span data-stu-id="5665f-125">This is an option set that represents the two main contracting models supported by Project Operations:</span></span></br><span data-ttu-id="5665f-126">- **מחיר קבוע**</span><span class="sxs-lookup"><span data-stu-id="5665f-126">- **Fixed Price**</span></span></br><span data-ttu-id="5665f-127">- **זמן וחומרים**</span><span class="sxs-lookup"><span data-stu-id="5665f-127">- **Time and Material**</span></span> | <span data-ttu-id="5665f-128">העסקה בפועל תעובד בהתבסס על שיטת החיוב של סעיף החוזה המוזכר.</span><span class="sxs-lookup"><span data-stu-id="5665f-128">Based on the billing method of the referenced contract line, the actual transaction will be processed.</span></span> <span data-ttu-id="5665f-129">אם לסעיף החוזה אליו מתייחס הנתון בפועל יש שיטת חיוב של זמן וחומרים, נוצרים רשומות של נתונים בפועל של עלויות ומכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="5665f-129">If the contract line referenced by the actual has a time and material billing method, cost and unbilled sales actual records are created.</span></span> <span data-ttu-id="5665f-130">אם לסעיף החוזה אליו מתייחס הנתון בפועל יש שיטת חיוב במחיר קבוע, נוצר רק נתון בפועל של עלות.</span><span class="sxs-lookup"><span data-stu-id="5665f-130">If the contract line referenced by the actual has a fixed price billing method, only a cost actual is created.</span></span> |
| <span data-ttu-id="5665f-131">**פרויקט**</span><span class="sxs-lookup"><span data-stu-id="5665f-131">**Project**</span></span> | <span data-ttu-id="5665f-132">השתמש בשדה זה כדי לזהות את הפרויקט שישמש מסירת העבודה בהתקשרות זו.</span><span class="sxs-lookup"><span data-stu-id="5665f-132">Use this field to identify the project that will be used to deliver the work on this engagement.</span></span> | <span data-ttu-id="5665f-133">ערך זה ישמש יחד עם **משימות כלולות** ו **סיווגי עסקאות כלולים** כדי לפענח את ההפניה לסעיף החוזה ברשומת שורת הערכה או נתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="5665f-133">This value will be used in conjunction with **Included Tasks** and **Included Transaction Classes** to resolve the contract line reference on an actual or estimate line record.</span></span> |
| <span data-ttu-id="5665f-134">**משימות כלולות**</span><span class="sxs-lookup"><span data-stu-id="5665f-134">**Included Tasks**</span></span> | <span data-ttu-id="5665f-135">מציין אם סעיף חוזה זה כולל את כל משימות הפרויקט עבור הפרויקט שנבחר או רק קבוצת משנה של המשימות.</span><span class="sxs-lookup"><span data-stu-id="5665f-135">Indicates if this contract line includes all project tasks for the selected project or only a subset of the tasks.</span></span> <span data-ttu-id="5665f-136">זוהי קבוצת אפשרויות בעלת הערכים האפשריים הבאים:</span><span class="sxs-lookup"><span data-stu-id="5665f-136">This is an option set that has the following possible values:</span></span></br><span data-ttu-id="5665f-137">- **כל משימות הפרויקט**</span><span class="sxs-lookup"><span data-stu-id="5665f-137">- **All Project Tasks**</span></span></br><span data-ttu-id="5665f-138">- **משימות פרויקט נבחרות בלבד**.</span><span class="sxs-lookup"><span data-stu-id="5665f-138">- **Selected Project Tasks Only**.</span></span> <span data-ttu-id="5665f-139">ערך ריק בשדה זה שווה לבחירה של **כל משימות הפרויקט**.</span><span class="sxs-lookup"><span data-stu-id="5665f-139">A blank value in this field is equal to selecting **All Project Tasks**.</span></span> | <span data-ttu-id="5665f-140">אם האפשרות **משימות נבחרות בלבד** נבחרת, ניתן לבחור משימות ספציפיות ולשייך אותן לסעיף חוזה זה בכרטיסיה **הגדרת חיוב משימות**  בדף **פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="5665f-140">If **Selected Tasks Only** is selected, you can select specific tasks and associate them to this contract line on the **Task Billing Setup** tab on the **Project** page.</span></span> <span data-ttu-id="5665f-141">ערך זה ישמש יחד עם הסיווגים **פרוייקט** ו **משימה כלולה** כדי לפתור את הפניה ברשומת שורה של נתון בפועל או הערכה.</span><span class="sxs-lookup"><span data-stu-id="5665f-141">The value will be used in conjunction with **Project** and **Included Transaction** classes to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="5665f-142">**כלול זמן**</span><span class="sxs-lookup"><span data-stu-id="5665f-142">**Include Time**</span></span> | <span data-ttu-id="5665f-143">הערך **כן**/**לא** מציין אם עסקאות זמן או עלויות עבודה בפרויקט שנבחר ייכללו בסעיף חוזה זה.</span><span class="sxs-lookup"><span data-stu-id="5665f-143">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="5665f-144">הערך **לא** מציין שעסקאות זמן או עלויות עבודה לא ייכללו בסעיף החוזה הזה.</span><span class="sxs-lookup"><span data-stu-id="5665f-144">A **No** value indicates that the time transactions or labor cost will not be included on this contract line.</span></span> <span data-ttu-id="5665f-145">הערך **כן** מציין שהם יכללו.</span><span class="sxs-lookup"><span data-stu-id="5665f-145">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="5665f-146">ערך זה משמש בשילוב עם הפרויקט כדי לפענח את הפניה לסעיף החוזה ברשומת שורת הערכה או נתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="5665f-146">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="5665f-147">**כלול הוצאה**</span><span class="sxs-lookup"><span data-stu-id="5665f-147">**Include Expense**</span></span> | <span data-ttu-id="5665f-148">הערך **כן**/**לא** מציין אם עלויות הוצאה בפרויקט שנבחר ייכללו בסעיף חוזה זה.</span><span class="sxs-lookup"><span data-stu-id="5665f-148">A **Yes**/**No** value indicates if expense costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="5665f-149">הערך **לא** מציין שעלות ההוצאה לא תיכלל בסעיף החוזה הזה.</span><span class="sxs-lookup"><span data-stu-id="5665f-149">A **No** value indicates that the expense cost will not be included on this contract line.</span></span> <span data-ttu-id="5665f-150">הערך **כן** מציין שהיא תיכלל.</span><span class="sxs-lookup"><span data-stu-id="5665f-150">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="5665f-151">ערך זה משמש בשילוב עם הפרויקט כדי לפענח את הפניה לסעיף החוזה ברשומת שורת הערכה או נתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="5665f-151">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="5665f-152">**כלול חומרים**</span><span class="sxs-lookup"><span data-stu-id="5665f-152">**Include Materials**</span></span> | <span data-ttu-id="5665f-153">הערך **כן**/**לא** מציין אם עלויות חומר בפרויקט שנבחר ייכללו בסעיף חוזה זה.</span><span class="sxs-lookup"><span data-stu-id="5665f-153">A **Yes**/**No** value indicates if material costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="5665f-154">הערך **לא** מציין שעלויות חומר לא ייכללו בסעיף חוזה זה.</span><span class="sxs-lookup"><span data-stu-id="5665f-154">A **No** value indicates that the material costs will not be included on this contract line.</span></span> <span data-ttu-id="5665f-155">הערך **כן** מציין שהיא תיכלל.</span><span class="sxs-lookup"><span data-stu-id="5665f-155">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="5665f-156">ערך זה משמש בשילוב עם הפרויקט כדי לפענח את הפניה לסעיף החוזה ברשומת שורת הערכה או נתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="5665f-156">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="5665f-157">**כלול תשלום**</span><span class="sxs-lookup"><span data-stu-id="5665f-157">**Include Fee**</span></span> | <span data-ttu-id="5665f-158">הערך **כן**/**לא** מציין אם עמלות בפרויקט שנבחר ייכללו בסעיף חוזה זה.</span><span class="sxs-lookup"><span data-stu-id="5665f-158">A **Yes**/**No** value indicates if fees on the selected project will be included on this contract line.</span></span> <span data-ttu-id="5665f-159">הערך **לא** מציין שעמלות לא יכללו בסעיף החוזה הזה.</span><span class="sxs-lookup"><span data-stu-id="5665f-159">A **No** value indicates that the fees will not be included on this contract line.</span></span> <span data-ttu-id="5665f-160">הערך **כן** מציין שהם יכללו.</span><span class="sxs-lookup"><span data-stu-id="5665f-160">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="5665f-161">ערך זה משמש בשילוב עם הפרויקט כדי לפענח את הפניה לסעיף החוזה ברשומת שורת הערכה או נתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="5665f-161">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="5665f-162">**הסכום שעליו סוכם בחוזה**</span><span class="sxs-lookup"><span data-stu-id="5665f-162">**Contracted Amount**</span></span> | <span data-ttu-id="5665f-163">בסעיף חוזה במחיר קבוע, סכום זה הוא הערך המוסכם שיחויב ללקוח עבור כל רכיבי העבודה הקשורים לסעיף חוזה זה.</span><span class="sxs-lookup"><span data-stu-id="5665f-163">On a fixed price contract line, this amount is the agreed-on value that will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="5665f-164">בסעיף חוזה במחיר קבוע, סכום זה הוא ערך מעורך של מה שיחויב ללקוח עבור כל רכיבי העבודה הקשורים לסעיף חוזה זה.</span><span class="sxs-lookup"><span data-stu-id="5665f-164">On a time and material contract line, this amount is an estimated value of what will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="5665f-165">בחוזה פרויקט שנוצר מהצעת מחיר, ערך זה מועתק מהשדה המקביל בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5665f-165">On a project contract that is created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="5665f-166">כאשר בסעיף חוזה מבוסס פרויקט יש פרטי סעיף, שדה זה נעול לעריכה ומסוכם מהסכום המופיע בפרטי סעיף החוזה.</span><span class="sxs-lookup"><span data-stu-id="5665f-166">When a project–based contract line has line details, this field is locked for editing and is summarized from the amount on the contract line details.</span></span> | <span data-ttu-id="5665f-167">כאשר בסעיף החוזה יש פרטי סעיף, ניתן לשנות ערך זה על ידי שינוי הסכומים בפרטי הסעיף.</span><span class="sxs-lookup"><span data-stu-id="5665f-167">When the contract line has line details, this value can be modified by changing the amounts on the line details.</span></span> <span data-ttu-id="5665f-168">בסעיף חוזה במחיר קבוע, ערך זה משמש להפקת הסכום לפני מס בגין אבני דרך תקופתיות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="5665f-168">On a fixed price contract line, this value is used to generate the amount before tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="5665f-169">**מס משוער**</span><span class="sxs-lookup"><span data-stu-id="5665f-169">**Estimated Tax**</span></span> | <span data-ttu-id="5665f-170">המשתמש יכול לערוך שדה זה כדי להזין את סכום המס המשוער בסעיף החוזה.</span><span class="sxs-lookup"><span data-stu-id="5665f-170">The user can edit this field to input the estimated tax amount on the contract line.</span></span> <span data-ttu-id="5665f-171">כאשר בסעיף חוזה מבוסס פרויקט יש פרטי סעיף, שדה זה נעול לעריכה ומסוכם מסכום המס המופיע בפרטי סעיף החוזה.</span><span class="sxs-lookup"><span data-stu-id="5665f-171">When a project–based contract line has line details, this field is locked for editing and is summarized from the tax amount on the contract line details.</span></span> | <span data-ttu-id="5665f-172">כאשר בסעיף החוזה יש פרטי סעיף, ניתן לשנות ערך זה על ידי שינוי סכומי המס בפרטי הסעיף.</span><span class="sxs-lookup"><span data-stu-id="5665f-172">When the contract line has line details, this value can be modified by changing the tax amounts on the line details.</span></span> <span data-ttu-id="5665f-173">בסעיף חוזה במחיר קבוע, ערך זה משמש להפקת המס בגין אבני דרך תקופתיות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="5665f-173">On a fixed price contract line, this value is used to generate the tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="5665f-174">**הסכום שעליו סוכם בחוזה, אחרי מס**</span><span class="sxs-lookup"><span data-stu-id="5665f-174">**Contracted Amount after Tax**</span></span> | <span data-ttu-id="5665f-175">הסכום סעיף החוזה, אחרי מס.</span><span class="sxs-lookup"><span data-stu-id="5665f-175">The contract line amount after tax.</span></span> <span data-ttu-id="5665f-176">שדה זה הוא לקריאה בלבד ומחושב כ **הסכום שעלו סוכם בחוזה + מס**.</span><span class="sxs-lookup"><span data-stu-id="5665f-176">This field is read only and is calculated as **Contracted Amount + Tax**.</span></span> | <span data-ttu-id="5665f-177">בסעיף חוזה במחיר קבוע, ערך זה משמש להפקת אבני דרך תקופתיות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="5665f-177">On a fixed price contract line, this value is used to generate periodic billing milestones.</span></span> |
| <span data-ttu-id="5665f-178">**מגבלת 'אין לחרוג'**</span><span class="sxs-lookup"><span data-stu-id="5665f-178">**Not-to-Exceed Limit**</span></span> | <span data-ttu-id="5665f-179">המשתמש יכול לערוך שדה זה והוא זמין רק סעיפי חוזה מבוססי פרויקט שבהם מגדרת שיטת החיוב כזמן וחומרים.</span><span class="sxs-lookup"><span data-stu-id="5665f-179">The user can edit this field and it is only available on project-based contract lines that have the billing method set as time and material.</span></span> | <span data-ttu-id="5665f-180">המשתמש יכול לערוך שדה זה.</span><span class="sxs-lookup"><span data-stu-id="5665f-180">The user can edit this field.</span></span> <span data-ttu-id="5665f-181">כאשר נתון בפעול של זמן וחומרים מפנה לסעיף חוזה זה עבור זמן וחומרים, הסכום בנתון פועל מוערך מול מגבלת אין לחרוג בסעיף החוזה.</span><span class="sxs-lookup"><span data-stu-id="5665f-181">When an actual for time and material references this contract line for time and material, the amount on the actual is evaluated against the not-to-exceed limit on the contract line.</span></span> <span data-ttu-id="5665f-182">הערכה זו מסתיימת לאחר שהסכומים שכבר הוצאו ושמחויבים הובאו בחשבון.</span><span class="sxs-lookup"><span data-stu-id="5665f-182">This evaluation is completed after  the already spent and committed amounts are accounted for.</span></span> |
| <span data-ttu-id="5665f-183">**תקציב הלקוח**</span><span class="sxs-lookup"><span data-stu-id="5665f-183">**Customer Budget**</span></span> | <span data-ttu-id="5665f-184">שדה זה ניתן לעריכה ומועתק מהשדה המקביל בשורת הצעת המחיר עם החוזה נוצר מהצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="5665f-184">This field is editable and is copied from the corresponding field on the quote line if the contract was created from a quote.</span></span> | <span data-ttu-id="5665f-185">שדה זה משמש למידע בלבד ואין לו שום משמעות במורד הזרם.</span><span class="sxs-lookup"><span data-stu-id="5665f-185">This field is only used for information and does not have any downstream significance.</span></span> |

## <a name="validation-rules-for-the-options-on-the-general-tab-of-project-based-contract-lines"></a><span data-ttu-id="5665f-186">כללי אימות עבור האפשרויות בכרטיסיה 'כללי' של סעיפי חוזה מבוססי פרויקט</span><span class="sxs-lookup"><span data-stu-id="5665f-186">Validation rules for the options on the General tab of project-based contract lines</span></span>

<span data-ttu-id="5665f-187">כלל 1: אם השדה **משימות כלולות** ריק או מוגדר כ **כל משימות הפרויקט**, כל המשימות של הפרויקט כלולות בסעיף החוזה.</span><span class="sxs-lookup"><span data-stu-id="5665f-187">Rule 1: If the **Included Tasks** field is blank or set to **All Project Tasks**, all tasks of the project are included on the contract line.</span></span>

<span data-ttu-id="5665f-188">כלל 2: כאשר השדה **משימות כלולות** ריק או מוגדר במפורש כ **כל משימות הפרויקט**, פרויקט וסיווג עסקאות מסוים יכולים להיכלל בסעיף חוזה מבוסס פרויקט אחד בלבד של חוזה.</span><span class="sxs-lookup"><span data-stu-id="5665f-188">Rule 2: When the **Included Tasks** field is blank or explicitly set to **All Project Tasks**, a project and a certain transaction class can only be included on one project-based contract line of a contract.</span></span>

<span data-ttu-id="5665f-189">כלל 3: כאשר השדה **משימות כלולות** מוגדר כ **משימות הפרויקט נבחרות בלבד**, פרויקט וסיווג עסקאות מסוים יכולים להיכלל בסעיפי חוזה מבוססי פרויקט מרובים של חוזה.</span><span class="sxs-lookup"><span data-stu-id="5665f-189">Rule 3: When the **Included Tasks** field is set to **Selected Project Tasks Only**, a project and a certain transaction class can be included on multiple project-based contract lines of a contract.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="43" valign="top">
                <p><span data-ttu-id="5665f-190">
                    <strong>חוזה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5665f-190">
                    <strong>Contract</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="5665f-191">
                    <strong>סעיף חוזה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5665f-191">
                    <strong>Contract line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="5665f-192">
                    <strong>פרויקט</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5665f-192">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="67" valign="top">
                <p><span data-ttu-id="5665f-193">
                    <strong>משימות כלולות</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5665f-193">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="5665f-194">
                    <strong>כלול זמן</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5665f-194">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="5665f-195">
                    <strong>כלול הוצאה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5665f-195">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="5665f-196">
                    <strong>כלול חומרים</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5665f-196">
                    <strong>Include Materials</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="5665f-197">
                    <strong>כולל</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5665f-197">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="5665f-198">
                    <strong>תשלום</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5665f-198">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="53" valign="top">
                <p><span data-ttu-id="5665f-199">
                    <strong>חוקי/לא חוקי</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5665f-199">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="250" valign="top">
                <p><span data-ttu-id="5665f-200">
                    <strong>סיבה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5665f-200">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="5665f-201">C1</span><span class="sxs-lookup"><span data-stu-id="5665f-201">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="5665f-202">CL1</span><span class="sxs-lookup"><span data-stu-id="5665f-202">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-203">P1</span><span class="sxs-lookup"><span data-stu-id="5665f-203">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="5665f-204">ריק</span><span class="sxs-lookup"><span data-stu-id="5665f-204">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-205">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-205">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-206">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-206">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-207">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-207">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-208">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-208">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5665f-209">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="5665f-209">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5665f-210">הפרת כלל מס' 2.</span><span class="sxs-lookup"><span data-stu-id="5665f-210">Violation of Rule #2.</span></span> <span data-ttu-id="5665f-211">זמן, הוצאות, חומרים ועמלות בפרויקט P1 כלולים בסעיפי החוזה CL1 ו- CL2.</span><span class="sxs-lookup"><span data-stu-id="5665f-211">Time, Expense, Materials, and Fees on P1 project are included on both Contract lines CL1 and CL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="5665f-212">C1</span><span class="sxs-lookup"><span data-stu-id="5665f-212">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="5665f-213">CL2</span><span class="sxs-lookup"><span data-stu-id="5665f-213">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-214">P1</span><span class="sxs-lookup"><span data-stu-id="5665f-214">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="5665f-215">ריק</span><span class="sxs-lookup"><span data-stu-id="5665f-215">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-216">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-216">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-217">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-217">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-218">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-218">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-219">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-219">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="5665f-220">C1</span><span class="sxs-lookup"><span data-stu-id="5665f-220">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="5665f-221">CL1</span><span class="sxs-lookup"><span data-stu-id="5665f-221">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-222">P1</span><span class="sxs-lookup"><span data-stu-id="5665f-222">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="5665f-223">ריק</span><span class="sxs-lookup"><span data-stu-id="5665f-223">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-224">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-224">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-225">Yes</span><span class="sxs-lookup"><span data-stu-id="5665f-225">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-226">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-226">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-227">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-227">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5665f-228">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="5665f-228">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5665f-229">הפרת כלל מס' 2.</span><span class="sxs-lookup"><span data-stu-id="5665f-229">Violation of Rule #2.</span></span> <span data-ttu-id="5665f-230">זמן, חומרים ועמלות בפרויקט P1 כלולים בסעיפי החוזה CL1 ו- CL2.</span><span class="sxs-lookup"><span data-stu-id="5665f-230">Time, Materials, and Fees on P1 project are included on both Contract lines CL1 and CL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="5665f-231">C1</span><span class="sxs-lookup"><span data-stu-id="5665f-231">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="5665f-232">CL2</span><span class="sxs-lookup"><span data-stu-id="5665f-232">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-233">P1</span><span class="sxs-lookup"><span data-stu-id="5665f-233">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="5665f-234">ריק</span><span class="sxs-lookup"><span data-stu-id="5665f-234">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-235">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-235">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-236">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-236">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-237">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-237">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-238">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-238">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="5665f-239">C1</span><span class="sxs-lookup"><span data-stu-id="5665f-239">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="5665f-240">CL1</span><span class="sxs-lookup"><span data-stu-id="5665f-240">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-241">P1</span><span class="sxs-lookup"><span data-stu-id="5665f-241">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="5665f-242">ריק</span><span class="sxs-lookup"><span data-stu-id="5665f-242">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-243">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-243">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-244">Yes</span><span class="sxs-lookup"><span data-stu-id="5665f-244">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-245">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-245">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-246">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-246">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5665f-247">חוקי</span><span class="sxs-lookup"><span data-stu-id="5665f-247">Valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5665f-248">זמן, חומרים ועמלות בפרויקט P1 כלולים ב- CL1.</span><span class="sxs-lookup"><span data-stu-id="5665f-248">Time, Materials, and Fees on P1 project are included on CL1.</span></span>
                </p>
                <ul>
                    <li>
<span data-ttu-id="5665f-249">הוצאות בפרויקט P1 כלולות ב-CL2.</span><span class="sxs-lookup"><span data-stu-id="5665f-249">Expense on P1 project is included on CL2.</span></span>
                    </li>
                </ul>
                <p>
<span data-ttu-id="5665f-250">אין חפיפה במה שנכלל בכל סעיף חוזה, ולכן תקף.</span><span class="sxs-lookup"><span data-stu-id="5665f-250">No overlap in what is being included on each Contract line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="5665f-251">C1</span><span class="sxs-lookup"><span data-stu-id="5665f-251">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="5665f-252">CL2</span><span class="sxs-lookup"><span data-stu-id="5665f-252">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-253">P1</span><span class="sxs-lookup"><span data-stu-id="5665f-253">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="5665f-254">ריק</span><span class="sxs-lookup"><span data-stu-id="5665f-254">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-255">Yes</span><span class="sxs-lookup"><span data-stu-id="5665f-255">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-256">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-257">Yes</span><span class="sxs-lookup"><span data-stu-id="5665f-257">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-258">Yes</span><span class="sxs-lookup"><span data-stu-id="5665f-258">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="5665f-259">C1</span><span class="sxs-lookup"><span data-stu-id="5665f-259">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="5665f-260">CL1</span><span class="sxs-lookup"><span data-stu-id="5665f-260">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-261">P1</span><span class="sxs-lookup"><span data-stu-id="5665f-261">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="5665f-262">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="5665f-262">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-263">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-263">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-264">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-264">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-265">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-266">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-266">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5665f-267">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="5665f-267">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5665f-268">הפרת כלל מס' 2</span><span class="sxs-lookup"><span data-stu-id="5665f-268">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="5665f-269">C1 כולל זמן, חומרים, הוצאות ועמלות לקבוצת משנה של משימות בפרויקט P1.</span><span class="sxs-lookup"><span data-stu-id="5665f-269">C1 includes Time, Materials, Expenses and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="5665f-270">CL2 כולל זמן, חומרים, הוצאות ועמלות עבור כל הפרויקט P1 ולכן חופף למה שנכלל ב- C1.</span><span class="sxs-lookup"><span data-stu-id="5665f-270">CL2 includes Time, Materials, Expenses and Fees for the whole project P1 and therefore overlaps with what is included on C1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="5665f-271">C1</span><span class="sxs-lookup"><span data-stu-id="5665f-271">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="5665f-272">CL2</span><span class="sxs-lookup"><span data-stu-id="5665f-272">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-273">P1</span><span class="sxs-lookup"><span data-stu-id="5665f-273">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="5665f-274">ריק</span><span class="sxs-lookup"><span data-stu-id="5665f-274">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-275">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-275">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-276">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-276">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-277">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-278">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-278">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="5665f-279">C1</span><span class="sxs-lookup"><span data-stu-id="5665f-279">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="5665f-280">CL1</span><span class="sxs-lookup"><span data-stu-id="5665f-280">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-281">P1</span><span class="sxs-lookup"><span data-stu-id="5665f-281">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="5665f-282">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="5665f-282">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-283">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-283">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-284">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-284">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-285">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-285">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-286">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-286">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5665f-287">חוקי</span><span class="sxs-lookup"><span data-stu-id="5665f-287">Valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5665f-288">לפי כלל מס '3</span><span class="sxs-lookup"><span data-stu-id="5665f-288">Per Rule #3</span></span> </p>
                <p>
<span data-ttu-id="5665f-289">C1 כולל זמן, חומרים, הוצאות ועמלות לקבוצת משנה של משימות בפרויקט P1.</span><span class="sxs-lookup"><span data-stu-id="5665f-289">C1 includes Time, Expenses, Materials, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="5665f-290">CL2 כולל זמן, חומרים, הוצאות ועמלות לקבוצת משנה של משימות בפרויקט P1.</span><span class="sxs-lookup"><span data-stu-id="5665f-290">CL2 includes Time, Expenses, Materials, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="5665f-291">האימות הנוסף היחיד הוא שקבוצת המשנה של המשימות ב- CL1 שונה מקבוצת משנה של המשימות ב- CL2 כדי להבטיח שאין שם חפיפה.</span><span class="sxs-lookup"><span data-stu-id="5665f-291">The only additional validation is around the subset of tasks on CL1 is different from the subset of tasks on CL2 to ensure that there are no overlaps there.</span></span> <span data-ttu-id="5665f-292">פעולה זו מתבצעת על ידי המערכת כאשר משימות משויכות.</span><span class="sxs-lookup"><span data-stu-id="5665f-292">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="5665f-293">C1</span><span class="sxs-lookup"><span data-stu-id="5665f-293">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="5665f-294">CL2</span><span class="sxs-lookup"><span data-stu-id="5665f-294">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-295">P1</span><span class="sxs-lookup"><span data-stu-id="5665f-295">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="5665f-296">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="5665f-296">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-297">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-297">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5665f-298">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-298">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-299">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-299">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5665f-300">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5665f-300">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
