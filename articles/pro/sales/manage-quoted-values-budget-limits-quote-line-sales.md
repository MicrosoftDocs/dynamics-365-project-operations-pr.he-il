---
title: מבט כולל על שורות הצעות מחיר מבוססות פרוייקט
description: נושא זה מספק מידע על עבודה עם שורות הצעות מחיר המבוססות פרויקט לעבודת פרויקט.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 32337b05f09ef7c5b84fdff9870744d6367e2693
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994857"
---
# <a name="project-based-quote-lines-overview"></a><span data-ttu-id="ab399-103">מבט כולל על שורות הצעות מחיר מבוססות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="ab399-103">Project-based quote lines overview</span></span> 

<span data-ttu-id="ab399-104">_**חל על:** פריסה קלה - עסקה עם חשבונית פרופורמה, Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="ab399-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="ab399-105">שורות הצעת מחיר מבוססות פרויקט נועדו לעזור להעריך את עבודת הפרויקט עבור התקשרות.</span><span class="sxs-lookup"><span data-stu-id="ab399-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="ab399-106">המבנה של שורת הצעות מחיר מבוסס פרויקט מורחב להערכות פרויקט באמצעות המושגים הבאים:</span><span class="sxs-lookup"><span data-stu-id="ab399-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="ab399-107">שיטת חיוב</span><span class="sxs-lookup"><span data-stu-id="ab399-107">Billing Method</span></span>
- <span data-ttu-id="ab399-108">מיפוי פרויקטים ומשימות</span><span class="sxs-lookup"><span data-stu-id="ab399-108">Project and Task Mapping</span></span>
- <span data-ttu-id="ab399-109">סווגי עסקה כלולים</span><span class="sxs-lookup"><span data-stu-id="ab399-109">Included Transaction classes</span></span>
- <span data-ttu-id="ab399-110">מגבלת 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="ab399-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="ab399-111">הגדרת יכולת חיוב</span><span class="sxs-lookup"><span data-stu-id="ab399-111">Chargeability setup</span></span>
- <span data-ttu-id="ab399-112">הערכה באמצעות פרטי קו הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="ab399-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="ab399-113">לקוחות של שורת הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="ab399-113">Quote line Customers</span></span>

<span data-ttu-id="ab399-114">הטבלה הבאה מספקת מידע אודות השדות המופיעים בכרטיסיה **כללי** של שורת הצעת מחיר מבוססת פרויקט.</span><span class="sxs-lookup"><span data-stu-id="ab399-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="ab399-115">שדות אלה מסייעים בהכנת הבסיס לביצוע הערכה מפורטת ויסודיות לעבודת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ab399-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="ab399-116">**שדה**</span><span class="sxs-lookup"><span data-stu-id="ab399-116">**Field**</span></span> | <span data-ttu-id="ab399-117">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="ab399-117">**Description**</span></span> | <span data-ttu-id="ab399-118">**השפעה במורד הזרם**</span><span class="sxs-lookup"><span data-stu-id="ab399-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="ab399-119">שם</span><span class="sxs-lookup"><span data-stu-id="ab399-119">Name</span></span> | <span data-ttu-id="ab399-120">שם שורת הצעת המחיר המסייע לך לזהות את המרכיב הנפרד של הצעת המחיר המוערכת.</span><span class="sxs-lookup"><span data-stu-id="ab399-120">The name of quote line that helps you to identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="ab399-121">מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="ab399-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="ab399-122">שיטת חיוב</span><span class="sxs-lookup"><span data-stu-id="ab399-122">Billing Method</span></span> | <span data-ttu-id="ab399-123">כשנוצרת הצעת מחיר מהזדמנות, ערך זה מועתק מהשדה התואם שבשורת הזדמנות.</span><span class="sxs-lookup"><span data-stu-id="ab399-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="ab399-124">תחום זה כולל את שני המודלים העיקריים לחוזים, שנתמכים על ידי Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="ab399-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="ab399-125">- מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="ab399-125">- Fixed price</span></span></br><span data-ttu-id="ab399-126">- זמן וחומרים.</span><span class="sxs-lookup"><span data-stu-id="ab399-126">- Time and material.</span></span>| <span data-ttu-id="ab399-127">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="ab399-127">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="ab399-128">פרויקט</span><span class="sxs-lookup"><span data-stu-id="ab399-128">Project</span></span> | <span data-ttu-id="ab399-129">השתמש בשדה אופציונלי זה כדי לזהות את הפרויקט שישמש להגשת העבודה בהתקשרות זו.</span><span class="sxs-lookup"><span data-stu-id="ab399-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="ab399-130">כאשר פרויקט ממופה לשורת הצעת מחיר, זה עוזר בהגדרת משימות הניתנות לחיוב וגם בכנסת הערכה מבוססת פרויקט לשורת הצעת המחיר, כפרטים בשורת הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="ab399-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="ab399-131">כאשר פרויקט אינו ממופה לשורת הצעת מחיר מבוססת פרויקט, יש ליצור את ההערכה באופן ידני על ידי יצירת כל פרט שבשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="ab399-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="ab399-132">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="ab399-132">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="ab399-133">משימות כלולות</span><span class="sxs-lookup"><span data-stu-id="ab399-133">Included Tasks</span></span> | <span data-ttu-id="ab399-134">הוא מציין אם שורת הצעת מחיר זו משמשת עבור כל משימות הפרויקט של הפרויקט שנבחר או עבור חלקן.</span><span class="sxs-lookup"><span data-stu-id="ab399-134">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="ab399-135">שדהזה כולל את הערכים אפשריים הבאים:</span><span class="sxs-lookup"><span data-stu-id="ab399-135">This field has the following possible values:</span></span></br><span data-ttu-id="ab399-136">- כל משימות הפרויקט</span><span class="sxs-lookup"><span data-stu-id="ab399-136">- All project tasks</span></span></br><span data-ttu-id="ab399-137">- משימות פרויקט נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="ab399-137">- Selected project tasks only</span></span></br><span data-ttu-id="ab399-138">ערך ריק בשדה זה שווה ערך לאפשרות **כל משימות הפרויקט**.</span><span class="sxs-lookup"><span data-stu-id="ab399-138">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="ab399-139">בעת בחירה באפשרות **משימות פרויקט נבחרות בלבד** בדף הפרויקט, הכרטיסיה **הגדרת חיוב משימה** מאפשרת לך לבחור משימות ספציפיות כדי לשייך אותן לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="ab399-139">When **Selected project tasks only** is selected on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="ab399-140">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="ab399-140">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="ab399-141">כלול זמן</span><span class="sxs-lookup"><span data-stu-id="ab399-141">Include Time</span></span> | <span data-ttu-id="ab399-142">הערך **כן**/**לא** מציין אם עסקאות זמן או עלויות עבודה בפרויקט שנבחר ייכללו בהערכה לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="ab399-142">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="ab399-143">הערך **לא** מציין שעסקאות זמן או עלויות עבודה לא ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="ab399-143">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="ab399-144">הערך **כן** מציין שעסקאות זמן או עלויות עבודה ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="ab399-144">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="ab399-145">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="ab399-145">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="ab399-146">כלול הוצאה</span><span class="sxs-lookup"><span data-stu-id="ab399-146">Include Expense</span></span> | <span data-ttu-id="ab399-147">הערך **כן**/**לא** מציין אם עלויות הוצאה בפרויקט שנבחר ייכללו בהערכה לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="ab399-147">A **Yes**/**No** value indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="ab399-148">הערך **לא** מציין שעלויות ההוצאות לא ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="ab399-148">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="ab399-149">הערך **כן** מציין שעלויות ההוצאות ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="ab399-149">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="ab399-150">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="ab399-150">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="ab399-151">כלול חומר</span><span class="sxs-lookup"><span data-stu-id="ab399-151">Include Material</span></span> | <span data-ttu-id="ab399-152">הערך **כן**/**לא** מציין אם עלויות חומר בפרויקט שנבחר ייכללו בהערכה לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="ab399-152">A **Yes**/**No** value indicates if material costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="ab399-153">הערך **לא** מציין שעלויות חומר לא ייכללו בהערכה לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="ab399-153">A **No** value indicates that the material costs will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="ab399-154">הערך **כן** מציין שעלויות חומר ייכללו בהערכה לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="ab399-154">A **Yes** value indicates that the material costs will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="ab399-155">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="ab399-155">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="ab399-156">כלול תשלום</span><span class="sxs-lookup"><span data-stu-id="ab399-156">Include Fee</span></span> | <span data-ttu-id="ab399-157">הערך **כן**/**לא** מציין אם עמלות בפרויקט שנבחר ייכללו בהערכה לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="ab399-157">A **Yes**/**No** value indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="ab399-158">הערך **לא** מציין שהעמלות לא ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="ab399-158">A **No** value indicates that the fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="ab399-159">הערך **כן** מציין שהעמלות ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="ab399-159">A **Yes** value indicates that the fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="ab399-160">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="ab399-160">This value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="ab399-161">הסכום של הצעת המחיר</span><span class="sxs-lookup"><span data-stu-id="ab399-161">Quoted Amount</span></span> | <span data-ttu-id="ab399-162">זהו הסכום שיוצע כהצעת מחיר ללקוח עבור כל העבודה החזויה בשורת הצעת מחיר זו המבוססת על פרויקט.</span><span class="sxs-lookup"><span data-stu-id="ab399-162">This is the amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="ab399-163">בהצעת מחיר שנוצרת מהזדמנות, ערך זה מועתק מהשדה **תקציב הלקוח** שבשורת הזדמנות.</span><span class="sxs-lookup"><span data-stu-id="ab399-163">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="ab399-164">כשבשורת צעת מחיר מבוססת הפרויקט יש פרטי שורה, שדה זה נעול לעריכה ומסוכם מהסכום שנמצא בפרטים בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="ab399-164">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="ab399-165">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="ab399-165">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="ab399-166">מס משוער</span><span class="sxs-lookup"><span data-stu-id="ab399-166">Estimated Tax</span></span> | <span data-ttu-id="ab399-167">זהו שדה הניתן לעריכה שהמשתמש יכול להוסיף בו את סכום המס המשוער בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="ab399-167">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="ab399-168">כשבשורת צעת מחיר מבוססת הפרויקט יש פרטי שורה, שדה זה נעול לעריכה ומסוכם מסכום המס שנמצא בפרטים בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="ab399-168">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="ab399-169">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="ab399-169">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="ab399-170">סכום הצעת המחיר, אחרי מס</span><span class="sxs-lookup"><span data-stu-id="ab399-170">Quoted Amount after Tax</span></span> | <span data-ttu-id="ab399-171">שדה זה הוא סכום שורת הצעת המחיר לאחר מס והוא לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="ab399-171">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="ab399-172">הסכום בשדה זה מחושב כ *סכום הצעת המחיר + מס*.</span><span class="sxs-lookup"><span data-stu-id="ab399-172">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="ab399-173">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="ab399-173">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="ab399-174">מגבלת 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="ab399-174">Not-to-exceed Limit</span></span> | <span data-ttu-id="ab399-175">שדה זה ניתן לעריכה והוא זמין רק בשורות הצעות מחיר מבוססות פרויקט עם שיטת חיוב של **זמן וחומרים**.</span><span class="sxs-lookup"><span data-stu-id="ab399-175">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="ab399-176">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="ab399-176">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="ab399-177">תקציב הלקוח</span><span class="sxs-lookup"><span data-stu-id="ab399-177">Customer Budget</span></span> | <span data-ttu-id="ab399-178">שדה זה ניתן לעריכה ומועתק מהשדה התואם בשורת ההזדמנות אם הצעת המחיר נוצרה מהזדמנות.</span><span class="sxs-lookup"><span data-stu-id="ab399-178">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="ab399-179">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="ab399-179">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="ab399-180">כללי אימות עבור שדות בכרטיסיה 'כללי' של שורות הצעות מחיר מבוססות פרויקט</span><span class="sxs-lookup"><span data-stu-id="ab399-180">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="ab399-181">**כלל 1**: אם השדה **משימות כלולות** ריק, או אם הוא מוגדר ל **כל משימות הפרויקט**, פרויקט כלול בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="ab399-181">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="ab399-182">**כלל 2**: אם השדה **משימות כלולות** ריק, או אם הוא מוגדר ל **כל משימות הפרויקט**, פרויקט וסיווג עסקאות מסוים יכולים להיכלל רק בשורת הצעת מחיר מבוססת פרויקט אחת של הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="ab399-182">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="ab399-183">**כלל 3**: אם השדה **משימות כלולות** מוגדר ל **משימות הפרויקט נבחרות בלבד**, פרויקט וסיווג עסקאות מסוים יכולים להיכלל בשורת הצעת מחיר מבוססת פרויקט מרובות של הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="ab399-183">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="ab399-184">**כלל 4**: אם להזדמנות יש הצעות מחיר מרובות, יכולות להיות שורות הצעות מחיר מהצעות מחיר שונות, שכולן מתייחסות לאותו פרויקט וכוללות את אותו סיווג עסקאות.</span><span class="sxs-lookup"><span data-stu-id="ab399-184">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="ab399-185">**כלל 5**: אם הצעות המחיר אינן שייכות לאותה הזדמנות, הן אינן יכולות לכלול את אותו פרויקט וסיווג עסקאות.</span><span class="sxs-lookup"><span data-stu-id="ab399-185">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="59" valign="top">
                <p><span data-ttu-id="ab399-186">
                    <strong>הזדמנות</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ab399-186">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="39" valign="top">
                <p><span data-ttu-id="ab399-187">
                    <strong>הצעת מחיר</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ab399-187">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="40" valign="top">
                <p><span data-ttu-id="ab399-188">
                    <strong>שורת הצעת מחיר</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ab399-188">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="ab399-189">
                    <strong>פרויקט</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ab399-189">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="77" valign="top">
                <p><span data-ttu-id="ab399-190">
                    <strong>משימות כלולות</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ab399-190">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="45" valign="top">
                <p><span data-ttu-id="ab399-191">
                    <strong>כלול זמן</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ab399-191">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="46" valign="top">
                <p><span data-ttu-id="ab399-192">
                    <strong>כלול הוצאה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ab399-192">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="43" valign="top">
                <p><span data-ttu-id="ab399-193">
                    <strong>כלול חומר</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ab399-193">
                    <strong>Include Material</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="ab399-194">
                    <strong>כולל</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ab399-194">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="ab399-195">
                    <strong>תשלום</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ab399-195">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="49" valign="top">
                <p><span data-ttu-id="ab399-196">
                    <strong>חוקי/לא חוקי</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ab399-196">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="200" valign="top">
                <p><span data-ttu-id="ab399-197">
                    <strong>סיבה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="ab399-197">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="ab399-198">O1</span><span class="sxs-lookup"><span data-stu-id="ab399-198">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="ab399-199">ר1</span><span class="sxs-lookup"><span data-stu-id="ab399-199">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="ab399-200">QL1</span><span class="sxs-lookup"><span data-stu-id="ab399-200">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-201">P1</span><span class="sxs-lookup"><span data-stu-id="ab399-201">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="ab399-202">ריק</span><span class="sxs-lookup"><span data-stu-id="ab399-202">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="ab399-203">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-203">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="ab399-204">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-204">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="ab399-205">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-205">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-206">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-206">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ab399-207">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="ab399-207">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ab399-208">הפרת כלל מס' 2.</span><span class="sxs-lookup"><span data-stu-id="ab399-208">Violation of Rule #2.</span></span> <span data-ttu-id="ab399-209">זמן, הוצאות ועמלות בפרויקט P1 כלולים בשורות הצעות מחיר QL1 ו-QL2</span><span class="sxs-lookup"><span data-stu-id="ab399-209">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="ab399-210">O1</span><span class="sxs-lookup"><span data-stu-id="ab399-210">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="ab399-211">ר1</span><span class="sxs-lookup"><span data-stu-id="ab399-211">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="ab399-212">QL2</span><span class="sxs-lookup"><span data-stu-id="ab399-212">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-213">P1</span><span class="sxs-lookup"><span data-stu-id="ab399-213">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="ab399-214">ריק</span><span class="sxs-lookup"><span data-stu-id="ab399-214">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="ab399-215">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-215">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="ab399-216">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-216">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="ab399-217">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-217">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-218">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-218">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="ab399-219">O1</span><span class="sxs-lookup"><span data-stu-id="ab399-219">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="ab399-220">ר1</span><span class="sxs-lookup"><span data-stu-id="ab399-220">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="ab399-221">QL1</span><span class="sxs-lookup"><span data-stu-id="ab399-221">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-222">P1</span><span class="sxs-lookup"><span data-stu-id="ab399-222">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="ab399-223">ריק</span><span class="sxs-lookup"><span data-stu-id="ab399-223">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="ab399-224">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-224">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="ab399-225">Yes</span><span class="sxs-lookup"><span data-stu-id="ab399-225">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="ab399-226">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-226">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-227">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-227">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ab399-228">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="ab399-228">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ab399-229">הפרת כלל מס' 2.</span><span class="sxs-lookup"><span data-stu-id="ab399-229">Violation of Rule #2.</span></span> <span data-ttu-id="ab399-230">זמן, חומר ועמלות בפרויקט P1 כלולים בשורות הצעות מחיר QL1 ו-QL2</span><span class="sxs-lookup"><span data-stu-id="ab399-230">Time, Material, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="ab399-231">O1</span><span class="sxs-lookup"><span data-stu-id="ab399-231">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="ab399-232">ר1</span><span class="sxs-lookup"><span data-stu-id="ab399-232">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="ab399-233">QL2</span><span class="sxs-lookup"><span data-stu-id="ab399-233">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-234">P1</span><span class="sxs-lookup"><span data-stu-id="ab399-234">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="ab399-235">ריק</span><span class="sxs-lookup"><span data-stu-id="ab399-235">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="ab399-236">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-236">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="ab399-237">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-237">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="ab399-238">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-238">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-239">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-239">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="ab399-240">O1</span><span class="sxs-lookup"><span data-stu-id="ab399-240">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="ab399-241">ר1</span><span class="sxs-lookup"><span data-stu-id="ab399-241">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="ab399-242">QL1</span><span class="sxs-lookup"><span data-stu-id="ab399-242">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-243">P1</span><span class="sxs-lookup"><span data-stu-id="ab399-243">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="ab399-244">ריק</span><span class="sxs-lookup"><span data-stu-id="ab399-244">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="ab399-245">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-245">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="ab399-246">Yes</span><span class="sxs-lookup"><span data-stu-id="ab399-246">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="ab399-247">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-247">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-248">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-248">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ab399-249">חוקי</span><span class="sxs-lookup"><span data-stu-id="ab399-249">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ab399-250">זמן, חומר ועמלות בפרויקט P1 כלולים ב- QL1</span><span class="sxs-lookup"><span data-stu-id="ab399-250">Time, Material, and Fees on P1 project are included on QL1</span></span> <br>
<span data-ttu-id="ab399-251">הוצאות בפרויקט P1 כלולות ב-QL2</span><span class="sxs-lookup"><span data-stu-id="ab399-251">Expense on P1 project is included on QL2</span></span> <br>
<span data-ttu-id="ab399-252">אין חפיפה במה שנכלל בכל שורת הצעת מחיר, ולכן תקף.</span><span class="sxs-lookup"><span data-stu-id="ab399-252">No overlap in what is being included on each quote line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="ab399-253">O1</span><span class="sxs-lookup"><span data-stu-id="ab399-253">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="ab399-254">ר1</span><span class="sxs-lookup"><span data-stu-id="ab399-254">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="ab399-255">QL2</span><span class="sxs-lookup"><span data-stu-id="ab399-255">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-256">P1</span><span class="sxs-lookup"><span data-stu-id="ab399-256">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="ab399-257">ריק</span><span class="sxs-lookup"><span data-stu-id="ab399-257">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="ab399-258">Yes</span><span class="sxs-lookup"><span data-stu-id="ab399-258">No</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="ab399-259">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-259">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="ab399-260">Yes</span><span class="sxs-lookup"><span data-stu-id="ab399-260">No</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-261">Yes</span><span class="sxs-lookup"><span data-stu-id="ab399-261">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="ab399-262">O1</span><span class="sxs-lookup"><span data-stu-id="ab399-262">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="ab399-263">ר1</span><span class="sxs-lookup"><span data-stu-id="ab399-263">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="ab399-264">QL1</span><span class="sxs-lookup"><span data-stu-id="ab399-264">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-265">P1</span><span class="sxs-lookup"><span data-stu-id="ab399-265">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="ab399-266">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="ab399-266">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="ab399-267">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-267">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="ab399-268">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-268">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="ab399-269">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-269">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-270">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-270">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ab399-271">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="ab399-271">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ab399-272">הפרת כלל מס' 2</span><span class="sxs-lookup"><span data-stu-id="ab399-272">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="ab399-273">Q1 כולל זמן, חומר, הוצאות ועמלות לקבוצת משנה של משימות בפרויקט P1</span><span class="sxs-lookup"><span data-stu-id="ab399-273">Q1 includes Time, Material, Expenses and Fees on a subset of tasks on project P1</span></span> </p>
                <p>
<span data-ttu-id="ab399-274">QL2 כולל זמן, הוצאות ועמלות עבור כל הפרויקט P1 ולכן חופף את מה שנכלל ב-Q1.</span><span class="sxs-lookup"><span data-stu-id="ab399-274">QL2 includes Time, Expenses, and Fees for the whole project P1 and therefore overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="ab399-275">O1</span><span class="sxs-lookup"><span data-stu-id="ab399-275">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="ab399-276">ר1</span><span class="sxs-lookup"><span data-stu-id="ab399-276">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="ab399-277">QL2</span><span class="sxs-lookup"><span data-stu-id="ab399-277">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-278">P1</span><span class="sxs-lookup"><span data-stu-id="ab399-278">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="ab399-279">ריק</span><span class="sxs-lookup"><span data-stu-id="ab399-279">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="ab399-280">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-280">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="ab399-281">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-281">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="ab399-282">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-282">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-283">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-283">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="ab399-284">O1</span><span class="sxs-lookup"><span data-stu-id="ab399-284">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="ab399-285">ר1</span><span class="sxs-lookup"><span data-stu-id="ab399-285">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="ab399-286">QL1</span><span class="sxs-lookup"><span data-stu-id="ab399-286">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-287">P1</span><span class="sxs-lookup"><span data-stu-id="ab399-287">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="ab399-288">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="ab399-288">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="ab399-289">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-289">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="ab399-290">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-290">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="ab399-291">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-291">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-292">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-292">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ab399-293">חוקי</span><span class="sxs-lookup"><span data-stu-id="ab399-293">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ab399-294">לפי כלל מס '3,</span><span class="sxs-lookup"><span data-stu-id="ab399-294">Per Rule #3,</span></span> </p>
                <p>
<span data-ttu-id="ab399-295">Q1 כולל זמן, חומר, הוצאות ועמלות לקבוצת משנה של משימות בפרויקט P1.</span><span class="sxs-lookup"><span data-stu-id="ab399-295">Q1 includes Time, Material, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="ab399-296">QL2 כולל זמן, חומרים, הוצאות ועמלות לקבוצת משנה של משימות בפרויקט P1.</span><span class="sxs-lookup"><span data-stu-id="ab399-296">QL2 includes Time, Material, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="ab399-297">האימות הנוסף היחיד הוא שקבוצת המשנה של המשימות ב- QL1 שונה מקבוצת משנה של המשימות ב- QL2 כדי להבטיח שאין חפיפה.</span><span class="sxs-lookup"><span data-stu-id="ab399-297">The only additional validation is around the subset of tasks on QL1 which is different from the subset of tasks on QL2 to ensure that there is no overlap.</span></span> <span data-ttu-id="ab399-298">פעולה זו מתבצעת על ידי המערכת כאשר משימות משויכות.</span><span class="sxs-lookup"><span data-stu-id="ab399-298">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="ab399-299">O1</span><span class="sxs-lookup"><span data-stu-id="ab399-299">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="ab399-300">ר1</span><span class="sxs-lookup"><span data-stu-id="ab399-300">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="ab399-301">QL2</span><span class="sxs-lookup"><span data-stu-id="ab399-301">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-302">P1</span><span class="sxs-lookup"><span data-stu-id="ab399-302">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="ab399-303">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="ab399-303">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="ab399-304">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-304">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="ab399-305">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-305">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="ab399-306">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-306">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-307">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-307">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="ab399-308">O1</span><span class="sxs-lookup"><span data-stu-id="ab399-308">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="ab399-309">ר1</span><span class="sxs-lookup"><span data-stu-id="ab399-309">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="ab399-310">QL1</span><span class="sxs-lookup"><span data-stu-id="ab399-310">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-311">P1</span><span class="sxs-lookup"><span data-stu-id="ab399-311">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="ab399-312">כל משימות הפרויקט או ריק</span><span class="sxs-lookup"><span data-stu-id="ab399-312">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="ab399-313">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-313">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="ab399-314">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-314">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="ab399-315">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-315">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-316">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-316">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ab399-317">חוקי</span><span class="sxs-lookup"><span data-stu-id="ab399-317">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ab399-318">לפי כלל מס '5, Q1 ו- Q2 הן שתי הצעות מחיר לאותה הזדמנות, כך שניתן להשתמש בשתיהן להערכת אותם מרכיבי הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ab399-318">Per Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="ab399-319">O1</span><span class="sxs-lookup"><span data-stu-id="ab399-319">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="ab399-320">ר2</span><span class="sxs-lookup"><span data-stu-id="ab399-320">Q2</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="ab399-321">QL1</span><span class="sxs-lookup"><span data-stu-id="ab399-321">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-322">P1</span><span class="sxs-lookup"><span data-stu-id="ab399-322">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="ab399-323">כל משימות הפרויקט או ריק</span><span class="sxs-lookup"><span data-stu-id="ab399-323">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="ab399-324">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-324">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="ab399-325">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-325">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="ab399-326">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-326">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-327">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-327">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="ab399-328">O1</span><span class="sxs-lookup"><span data-stu-id="ab399-328">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="ab399-329">ר1</span><span class="sxs-lookup"><span data-stu-id="ab399-329">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="ab399-330">QL1</span><span class="sxs-lookup"><span data-stu-id="ab399-330">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-331">P1</span><span class="sxs-lookup"><span data-stu-id="ab399-331">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="ab399-332">כל משימות הפרויקט או ריק</span><span class="sxs-lookup"><span data-stu-id="ab399-332">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="ab399-333">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-333">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="ab399-334">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-334">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="ab399-335">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-335">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-336">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-336">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ab399-337">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="ab399-337">Not Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="ab399-338">לפי כלל מס '4, Q1 ו- Q2 הן שתי הצעות מחיר להזדמנויות שונות, כך שלא ניתן להשתמש בשתיהן להערכת אותם מרכיבים של אותו הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ab399-338">Per Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="ab399-339">O2</span><span class="sxs-lookup"><span data-stu-id="ab399-339">O2</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="ab399-340">ר1</span><span class="sxs-lookup"><span data-stu-id="ab399-340">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="ab399-341">QL1</span><span class="sxs-lookup"><span data-stu-id="ab399-341">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-342">P1</span><span class="sxs-lookup"><span data-stu-id="ab399-342">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="ab399-343">כל משימות הפרויקט או ריק</span><span class="sxs-lookup"><span data-stu-id="ab399-343">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="ab399-344">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-344">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="ab399-345">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-345">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="ab399-346">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-346">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="ab399-347">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="ab399-347">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
