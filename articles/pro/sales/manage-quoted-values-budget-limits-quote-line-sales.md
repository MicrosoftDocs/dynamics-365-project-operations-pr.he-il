---
title: מבט כולל על שורות הצעות מחיר מבוססות פרוייקט
description: נושא זה מספק מידע על עבודה עם שורות הצעות מחיר המבוססות פרויקט לעבודת פרויקט.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: cfe98fc89130c93dd0a36af8583881fdcb4550c0
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858699"
---
# <a name="project-based-quote-lines-overview"></a><span data-ttu-id="dae21-103">מבט כולל על שורות הצעות מחיר מבוססות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="dae21-103">Project-based quote lines overview</span></span> 

<span data-ttu-id="dae21-104">_**חל על:** פריסה קלה - עסקה עם חשבונית פרופורמה, Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="dae21-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="dae21-105">שורות הצעת מחיר מבוססות פרויקט נועדו לעזור להעריך את עבודת הפרויקט עבור התקשרות.</span><span class="sxs-lookup"><span data-stu-id="dae21-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="dae21-106">המבנה של שורת הצעות מחיר מבוסס פרויקט מורחב להערכות פרויקט באמצעות המושגים הבאים:</span><span class="sxs-lookup"><span data-stu-id="dae21-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="dae21-107">שיטת חיוב</span><span class="sxs-lookup"><span data-stu-id="dae21-107">Billing Method</span></span>
- <span data-ttu-id="dae21-108">מיפוי פרויקטים ומשימות</span><span class="sxs-lookup"><span data-stu-id="dae21-108">Project and Task Mapping</span></span>
- <span data-ttu-id="dae21-109">סווגי עסקה כלולים</span><span class="sxs-lookup"><span data-stu-id="dae21-109">Included Transaction classes</span></span>
- <span data-ttu-id="dae21-110">מגבלת 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="dae21-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="dae21-111">הגדרת יכולת חיוב</span><span class="sxs-lookup"><span data-stu-id="dae21-111">Chargeability setup</span></span>
- <span data-ttu-id="dae21-112">הערכה באמצעות פרטי קו הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="dae21-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="dae21-113">לקוחות של שורת הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="dae21-113">Quote line Customers</span></span>

<span data-ttu-id="dae21-114">הטבלה הבאה מספקת מידע אודות השדות המופיעים בכרטיסיה **כללי** של שורת הצעת מחיר מבוססת פרויקט.</span><span class="sxs-lookup"><span data-stu-id="dae21-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="dae21-115">שדות אלה מסייעים בהכנת הבסיס לביצוע הערכה מפורטת ויסודיות לעבודת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="dae21-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="dae21-116">**שדה**</span><span class="sxs-lookup"><span data-stu-id="dae21-116">**Field**</span></span> | <span data-ttu-id="dae21-117">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="dae21-117">**Description**</span></span> | <span data-ttu-id="dae21-118">**השפעה במורד הזרם**</span><span class="sxs-lookup"><span data-stu-id="dae21-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="dae21-119">שם</span><span class="sxs-lookup"><span data-stu-id="dae21-119">Name</span></span> | <span data-ttu-id="dae21-120">שם שורת הצעת המחיר המסייע לך לזהות את המרכיב הנפרד של הצעת המחיר המוערכת.</span><span class="sxs-lookup"><span data-stu-id="dae21-120">The name of quote line that helps you to identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="dae21-121">מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="dae21-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dae21-122">שיטת חיוב</span><span class="sxs-lookup"><span data-stu-id="dae21-122">Billing Method</span></span> | <span data-ttu-id="dae21-123">כשנוצרת הצעת מחיר מהזדמנות, ערך זה מועתק מהשדה התואם שבשורת הזדמנות.</span><span class="sxs-lookup"><span data-stu-id="dae21-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="dae21-124">תחום זה כולל את שני המודלים העיקריים לחוזים, שנתמכים על ידי Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="dae21-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="dae21-125">- מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="dae21-125">- Fixed price</span></span></br><span data-ttu-id="dae21-126">- זמן וחומרים.</span><span class="sxs-lookup"><span data-stu-id="dae21-126">- Time and material.</span></span>| <span data-ttu-id="dae21-127">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="dae21-127">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dae21-128">פרויקט</span><span class="sxs-lookup"><span data-stu-id="dae21-128">Project</span></span> | <span data-ttu-id="dae21-129">השתמש בשדה אופציונלי זה כדי לזהות את הפרויקט שישמש להגשת העבודה בהתקשרות זו.</span><span class="sxs-lookup"><span data-stu-id="dae21-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="dae21-130">כאשר פרויקט ממופה לשורת הצעת מחיר, זה עוזר בהגדרת משימות הניתנות לחיוב וגם בכנסת הערכה מבוססת פרויקט לשורת הצעת המחיר, כפרטים בשורת הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="dae21-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="dae21-131">כאשר פרויקט אינו ממופה לשורת הצעת מחיר מבוססת פרויקט, יש ליצור את ההערכה באופן ידני על ידי יצירת כל פרט שבשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="dae21-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="dae21-132">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="dae21-132">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="dae21-133">משימות כלולות</span><span class="sxs-lookup"><span data-stu-id="dae21-133">Included Tasks</span></span> | <span data-ttu-id="dae21-134">הוא מציין אם שורת הצעת מחיר זו משמשת עבור כל משימות הפרויקט של הפרויקט שנבחר או עבור חלקן.</span><span class="sxs-lookup"><span data-stu-id="dae21-134">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="dae21-135">שדהזה כולל את הערכים אפשריים הבאים:</span><span class="sxs-lookup"><span data-stu-id="dae21-135">This field has the following possible values:</span></span></br><span data-ttu-id="dae21-136">- כל משימות הפרויקט</span><span class="sxs-lookup"><span data-stu-id="dae21-136">- All project tasks</span></span></br><span data-ttu-id="dae21-137">- משימות פרויקט נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="dae21-137">- Selected project tasks only</span></span></br><span data-ttu-id="dae21-138">ערך ריק בשדה זה שווה ערך לאפשרות **כל משימות הפרויקט**.</span><span class="sxs-lookup"><span data-stu-id="dae21-138">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="dae21-139">בעת בחירה באפשרות **משימות פרויקט נבחרות בלבד** בדף הפרויקט, הכרטיסיה **הגדרת חיוב משימה** מאפשרת לך לבחור משימות ספציפיות כדי לשייך אותן לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="dae21-139">When **Selected project tasks only** is selected on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="dae21-140">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="dae21-140">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dae21-141">כלול זמן</span><span class="sxs-lookup"><span data-stu-id="dae21-141">Include Time</span></span> | <span data-ttu-id="dae21-142">הערך **כן**/**לא** מציין אם עסקאות זמן או עלויות עבודה בפרויקט שנבחר ייכללו בהערכה לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="dae21-142">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="dae21-143">הערך **לא** מציין שעסקאות זמן או עלויות עבודה לא ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="dae21-143">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="dae21-144">הערך **כן** מציין שעסקאות זמן או עלויות עבודה ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="dae21-144">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="dae21-145">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="dae21-145">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dae21-146">כלול הוצאה</span><span class="sxs-lookup"><span data-stu-id="dae21-146">Include Expense</span></span> | <span data-ttu-id="dae21-147">הערך **כן**/**לא** מציין אם עלויות הוצאה בפרויקט שנבחר ייכללו בהערכה לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="dae21-147">A **Yes**/**No** value indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="dae21-148">הערך **לא** מציין שעלויות ההוצאות לא ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="dae21-148">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="dae21-149">הערך **כן** מציין שעלויות ההוצאות ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="dae21-149">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="dae21-150">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="dae21-150">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dae21-151">כלול חומר</span><span class="sxs-lookup"><span data-stu-id="dae21-151">Include Material</span></span> | <span data-ttu-id="dae21-152">הערך **כן**/**לא** מציין אם עלויות חומר בפרויקט שנבחר ייכללו בהערכה לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="dae21-152">A **Yes**/**No** value indicates if material costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="dae21-153">הערך **לא** מציין שעלויות חומר לא ייכללו בהערכה לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="dae21-153">A **No** value indicates that the material costs will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="dae21-154">הערך **כן** מציין שעלויות חומר ייכללו בהערכה לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="dae21-154">A **Yes** value indicates that the material costs will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="dae21-155">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="dae21-155">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dae21-156">כלול תשלום</span><span class="sxs-lookup"><span data-stu-id="dae21-156">Include Fee</span></span> | <span data-ttu-id="dae21-157">הערך **כן**/**לא** מציין אם עמלות בפרויקט שנבחר ייכללו בהערכה לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="dae21-157">A **Yes**/**No** value indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="dae21-158">הערך **לא** מציין שהעמלות לא ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="dae21-158">A **No** value indicates that the fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="dae21-159">הערך **כן** מציין שהעמלות ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="dae21-159">A **Yes** value indicates that the fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="dae21-160">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="dae21-160">This value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dae21-161">הסכום של הצעת המחיר</span><span class="sxs-lookup"><span data-stu-id="dae21-161">Quoted Amount</span></span> | <span data-ttu-id="dae21-162">זהו הסכום שיוצע כהצעת מחיר ללקוח עבור כל העבודה החזויה בשורת הצעת מחיר זו המבוססת על פרויקט.</span><span class="sxs-lookup"><span data-stu-id="dae21-162">This is the amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="dae21-163">בהצעת מחיר שנוצרת מהזדמנות, ערך זה מועתק מהשדה **תקציב הלקוח** שבשורת הזדמנות.</span><span class="sxs-lookup"><span data-stu-id="dae21-163">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="dae21-164">כשבשורת צעת מחיר מבוססת הפרויקט יש פרטי שורה, שדה זה נעול לעריכה ומסוכם מהסכום שנמצא בפרטים בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="dae21-164">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="dae21-165">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="dae21-165">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dae21-166">מס משוער</span><span class="sxs-lookup"><span data-stu-id="dae21-166">Estimated Tax</span></span> | <span data-ttu-id="dae21-167">זהו שדה הניתן לעריכה שהמשתמש יכול להוסיף בו את סכום המס המשוער בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="dae21-167">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="dae21-168">כשבשורת צעת מחיר מבוססת הפרויקט יש פרטי שורה, שדה זה נעול לעריכה ומסוכם מסכום המס שנמצא בפרטים בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="dae21-168">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="dae21-169">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="dae21-169">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dae21-170">סכום הצעת המחיר, אחרי מס</span><span class="sxs-lookup"><span data-stu-id="dae21-170">Quoted Amount after Tax</span></span> | <span data-ttu-id="dae21-171">שדה זה הוא סכום שורת הצעת המחיר לאחר מס והוא לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="dae21-171">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="dae21-172">הסכום בשדה זה מחושב כ *סכום הצעת המחיר + מס*.</span><span class="sxs-lookup"><span data-stu-id="dae21-172">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="dae21-173">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="dae21-173">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dae21-174">מגבלת 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="dae21-174">Not-to-exceed Limit</span></span> | <span data-ttu-id="dae21-175">שדה זה ניתן לעריכה והוא זמין רק בשורות הצעות מחיר מבוססות פרויקט עם שיטת חיוב של **זמן וחומרים**.</span><span class="sxs-lookup"><span data-stu-id="dae21-175">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="dae21-176">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="dae21-176">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dae21-177">תקציב הלקוח</span><span class="sxs-lookup"><span data-stu-id="dae21-177">Customer Budget</span></span> | <span data-ttu-id="dae21-178">שדה זה ניתן לעריכה ומועתק מהשדה התואם בשורת ההזדמנות אם הצעת המחיר נוצרה מהזדמנות.</span><span class="sxs-lookup"><span data-stu-id="dae21-178">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="dae21-179">ערך זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו כאשר הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="dae21-179">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="dae21-180">כללי אימות עבור שדות בכרטיסיה 'כללי' של שורות הצעות מחיר מבוססות פרויקט</span><span class="sxs-lookup"><span data-stu-id="dae21-180">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="dae21-181">**כלל 1**: אם השדה **משימות כלולות** ריק, או אם הוא מוגדר ל **כל משימות הפרויקט**, פרויקט כלול בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="dae21-181">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="dae21-182">**כלל 2**: אם השדה **משימות כלולות** ריק, או אם הוא מוגדר ל **כל משימות הפרויקט**, פרויקט וסיווג עסקאות מסוים יכולים להיכלל רק בשורת הצעת מחיר מבוססת פרויקט אחת של הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="dae21-182">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="dae21-183">**כלל 3**: אם השדה **משימות כלולות** מוגדר ל **משימות הפרויקט נבחרות בלבד**, פרויקט וסיווג עסקאות מסוים יכולים להיכלל בשורת הצעת מחיר מבוססת פרויקט מרובות של הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="dae21-183">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="dae21-184">**כלל 4**: אם להזדמנות יש הצעות מחיר מרובות, יכולות להיות שורות הצעות מחיר מהצעות מחיר שונות, שכולן מתייחסות לאותו פרויקט וכוללות את אותו סיווג עסקאות.</span><span class="sxs-lookup"><span data-stu-id="dae21-184">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="dae21-185">**כלל 5**: אם הצעות המחיר אינן שייכות לאותה הזדמנות, הן אינן יכולות לכלול את אותו פרויקט וסיווג עסקאות.</span><span class="sxs-lookup"><span data-stu-id="dae21-185">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="59" valign="top">
                <p><span data-ttu-id="dae21-186">
                    <strong>הזדמנות</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dae21-186">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="39" valign="top">
                <p><span data-ttu-id="dae21-187">
                    <strong>הצעת מחיר</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dae21-187">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="40" valign="top">
                <p><span data-ttu-id="dae21-188">
                    <strong>שורת הצעת מחיר</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dae21-188">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="dae21-189">
                    <strong>פרויקט</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dae21-189">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="77" valign="top">
                <p><span data-ttu-id="dae21-190">
                    <strong>משימות כלולות</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dae21-190">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="45" valign="top">
                <p><span data-ttu-id="dae21-191">
                    <strong>כלול זמן</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dae21-191">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="46" valign="top">
                <p><span data-ttu-id="dae21-192">
                    <strong>כלול הוצאה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dae21-192">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="43" valign="top">
                <p><span data-ttu-id="dae21-193">
                    <strong>כלול חומר</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dae21-193">
                    <strong>Include Material</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="dae21-194">
                    <strong>כולל</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dae21-194">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="dae21-195">
                    <strong>תשלום</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dae21-195">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="49" valign="top">
                <p><span data-ttu-id="dae21-196">
                    <strong>חוקי/לא חוקי</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dae21-196">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="200" valign="top">
                <p><span data-ttu-id="dae21-197">
                    <strong>סיבה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dae21-197">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="dae21-198">O1</span><span class="sxs-lookup"><span data-stu-id="dae21-198">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="dae21-199">ר1</span><span class="sxs-lookup"><span data-stu-id="dae21-199">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="dae21-200">QL1</span><span class="sxs-lookup"><span data-stu-id="dae21-200">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-201">P1</span><span class="sxs-lookup"><span data-stu-id="dae21-201">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="dae21-202">ריק</span><span class="sxs-lookup"><span data-stu-id="dae21-202">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="dae21-203">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-203">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="dae21-204">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-204">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="dae21-205">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-205">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-206">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-206">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dae21-207">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="dae21-207">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dae21-208">הפרת כלל מס' 2.</span><span class="sxs-lookup"><span data-stu-id="dae21-208">Violation of Rule #2.</span></span> <span data-ttu-id="dae21-209">זמן, הוצאות ועמלות בפרויקט P1 כלולים בשורות הצעות מחיר QL1 ו-QL2</span><span class="sxs-lookup"><span data-stu-id="dae21-209">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="dae21-210">O1</span><span class="sxs-lookup"><span data-stu-id="dae21-210">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="dae21-211">ר1</span><span class="sxs-lookup"><span data-stu-id="dae21-211">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="dae21-212">QL2</span><span class="sxs-lookup"><span data-stu-id="dae21-212">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-213">P1</span><span class="sxs-lookup"><span data-stu-id="dae21-213">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="dae21-214">ריק</span><span class="sxs-lookup"><span data-stu-id="dae21-214">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="dae21-215">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-215">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="dae21-216">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-216">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="dae21-217">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-217">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-218">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-218">Yes</span></span> </p>
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
<span data-ttu-id="dae21-219">O1</span><span class="sxs-lookup"><span data-stu-id="dae21-219">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="dae21-220">ר1</span><span class="sxs-lookup"><span data-stu-id="dae21-220">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="dae21-221">QL1</span><span class="sxs-lookup"><span data-stu-id="dae21-221">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-222">P1</span><span class="sxs-lookup"><span data-stu-id="dae21-222">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="dae21-223">ריק</span><span class="sxs-lookup"><span data-stu-id="dae21-223">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="dae21-224">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-224">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="dae21-225">Yes</span><span class="sxs-lookup"><span data-stu-id="dae21-225">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="dae21-226">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-226">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-227">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-227">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dae21-228">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="dae21-228">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dae21-229">הפרת כלל מס' 2.</span><span class="sxs-lookup"><span data-stu-id="dae21-229">Violation of Rule #2.</span></span> <span data-ttu-id="dae21-230">זמן, חומר ועמלות בפרויקט P1 כלולים בשורות הצעות מחיר QL1 ו-QL2</span><span class="sxs-lookup"><span data-stu-id="dae21-230">Time, Material, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="dae21-231">O1</span><span class="sxs-lookup"><span data-stu-id="dae21-231">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="dae21-232">ר1</span><span class="sxs-lookup"><span data-stu-id="dae21-232">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="dae21-233">QL2</span><span class="sxs-lookup"><span data-stu-id="dae21-233">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-234">P1</span><span class="sxs-lookup"><span data-stu-id="dae21-234">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="dae21-235">ריק</span><span class="sxs-lookup"><span data-stu-id="dae21-235">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="dae21-236">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-236">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="dae21-237">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-237">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="dae21-238">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-238">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-239">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-239">Yes</span></span> </p>
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
<span data-ttu-id="dae21-240">O1</span><span class="sxs-lookup"><span data-stu-id="dae21-240">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="dae21-241">ר1</span><span class="sxs-lookup"><span data-stu-id="dae21-241">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="dae21-242">QL1</span><span class="sxs-lookup"><span data-stu-id="dae21-242">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-243">P1</span><span class="sxs-lookup"><span data-stu-id="dae21-243">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="dae21-244">ריק</span><span class="sxs-lookup"><span data-stu-id="dae21-244">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="dae21-245">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-245">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="dae21-246">Yes</span><span class="sxs-lookup"><span data-stu-id="dae21-246">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="dae21-247">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-247">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-248">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-248">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dae21-249">חוקי</span><span class="sxs-lookup"><span data-stu-id="dae21-249">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dae21-250">זמן, חומר ועמלות בפרויקט P1 כלולים ב- QL1</span><span class="sxs-lookup"><span data-stu-id="dae21-250">Time, Material, and Fees on P1 project are included on QL1</span></span> <br>
<span data-ttu-id="dae21-251">הוצאות בפרויקט P1 כלולות ב-QL2</span><span class="sxs-lookup"><span data-stu-id="dae21-251">Expense on P1 project is included on QL2</span></span> <br>
<span data-ttu-id="dae21-252">אין חפיפה במה שנכלל בכל שורת הצעת מחיר, ולכן תקף.</span><span class="sxs-lookup"><span data-stu-id="dae21-252">No overlap in what is being included on each quote line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="dae21-253">O1</span><span class="sxs-lookup"><span data-stu-id="dae21-253">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="dae21-254">ר1</span><span class="sxs-lookup"><span data-stu-id="dae21-254">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="dae21-255">QL2</span><span class="sxs-lookup"><span data-stu-id="dae21-255">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-256">P1</span><span class="sxs-lookup"><span data-stu-id="dae21-256">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="dae21-257">ריק</span><span class="sxs-lookup"><span data-stu-id="dae21-257">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="dae21-258">Yes</span><span class="sxs-lookup"><span data-stu-id="dae21-258">No</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="dae21-259">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-259">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="dae21-260">Yes</span><span class="sxs-lookup"><span data-stu-id="dae21-260">No</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-261">Yes</span><span class="sxs-lookup"><span data-stu-id="dae21-261">No</span></span> </p>
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
<span data-ttu-id="dae21-262">O1</span><span class="sxs-lookup"><span data-stu-id="dae21-262">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="dae21-263">ר1</span><span class="sxs-lookup"><span data-stu-id="dae21-263">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="dae21-264">QL1</span><span class="sxs-lookup"><span data-stu-id="dae21-264">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-265">P1</span><span class="sxs-lookup"><span data-stu-id="dae21-265">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="dae21-266">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="dae21-266">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="dae21-267">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-267">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="dae21-268">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-268">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="dae21-269">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-269">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-270">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-270">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dae21-271">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="dae21-271">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dae21-272">הפרת כלל מס' 2</span><span class="sxs-lookup"><span data-stu-id="dae21-272">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="dae21-273">Q1 כולל זמן, חומר, הוצאות ועמלות לקבוצת משנה של משימות בפרויקט P1</span><span class="sxs-lookup"><span data-stu-id="dae21-273">Q1 includes Time, Material, Expenses and Fees on a subset of tasks on project P1</span></span> </p>
                <p>
<span data-ttu-id="dae21-274">QL2 כולל זמן, הוצאות ועמלות עבור כל הפרויקט P1 ולכן חופף את מה שנכלל ב-Q1.</span><span class="sxs-lookup"><span data-stu-id="dae21-274">QL2 includes Time, Expenses, and Fees for the whole project P1 and therefore overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="dae21-275">O1</span><span class="sxs-lookup"><span data-stu-id="dae21-275">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="dae21-276">ר1</span><span class="sxs-lookup"><span data-stu-id="dae21-276">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="dae21-277">QL2</span><span class="sxs-lookup"><span data-stu-id="dae21-277">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-278">P1</span><span class="sxs-lookup"><span data-stu-id="dae21-278">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="dae21-279">ריק</span><span class="sxs-lookup"><span data-stu-id="dae21-279">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="dae21-280">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-280">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="dae21-281">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-281">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="dae21-282">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-282">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-283">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-283">Yes</span></span> </p>
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
<span data-ttu-id="dae21-284">O1</span><span class="sxs-lookup"><span data-stu-id="dae21-284">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="dae21-285">ר1</span><span class="sxs-lookup"><span data-stu-id="dae21-285">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="dae21-286">QL1</span><span class="sxs-lookup"><span data-stu-id="dae21-286">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-287">P1</span><span class="sxs-lookup"><span data-stu-id="dae21-287">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="dae21-288">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="dae21-288">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="dae21-289">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-289">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="dae21-290">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-290">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="dae21-291">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-291">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-292">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-292">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dae21-293">חוקי</span><span class="sxs-lookup"><span data-stu-id="dae21-293">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dae21-294">לפי כלל מס '3,</span><span class="sxs-lookup"><span data-stu-id="dae21-294">Per Rule #3,</span></span> </p>
                <p>
<span data-ttu-id="dae21-295">Q1 כולל זמן, חומר, הוצאות ועמלות לקבוצת משנה של משימות בפרויקט P1.</span><span class="sxs-lookup"><span data-stu-id="dae21-295">Q1 includes Time, Material, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="dae21-296">QL2 כולל זמן, חומרים, הוצאות ועמלות לקבוצת משנה של משימות בפרויקט P1.</span><span class="sxs-lookup"><span data-stu-id="dae21-296">QL2 includes Time, Material, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="dae21-297">האימות הנוסף היחיד הוא שקבוצת המשנה של המשימות ב- QL1 שונה מקבוצת משנה של המשימות ב- QL2 כדי להבטיח שאין חפיפה.</span><span class="sxs-lookup"><span data-stu-id="dae21-297">The only additional validation is around the subset of tasks on QL1 which is different from the subset of tasks on QL2 to ensure that there is no overlap.</span></span> <span data-ttu-id="dae21-298">פעולה זו מתבצעת על ידי המערכת כאשר משימות משויכות.</span><span class="sxs-lookup"><span data-stu-id="dae21-298">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="dae21-299">O1</span><span class="sxs-lookup"><span data-stu-id="dae21-299">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="dae21-300">ר1</span><span class="sxs-lookup"><span data-stu-id="dae21-300">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="dae21-301">QL2</span><span class="sxs-lookup"><span data-stu-id="dae21-301">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-302">P1</span><span class="sxs-lookup"><span data-stu-id="dae21-302">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="dae21-303">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="dae21-303">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="dae21-304">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-304">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="dae21-305">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-305">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="dae21-306">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-306">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-307">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-307">Yes</span></span> </p>
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
<span data-ttu-id="dae21-308">O1</span><span class="sxs-lookup"><span data-stu-id="dae21-308">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="dae21-309">ר1</span><span class="sxs-lookup"><span data-stu-id="dae21-309">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="dae21-310">QL1</span><span class="sxs-lookup"><span data-stu-id="dae21-310">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-311">P1</span><span class="sxs-lookup"><span data-stu-id="dae21-311">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="dae21-312">כל משימות הפרויקט או ריק</span><span class="sxs-lookup"><span data-stu-id="dae21-312">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="dae21-313">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-313">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="dae21-314">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-314">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="dae21-315">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-315">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-316">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-316">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dae21-317">חוקי</span><span class="sxs-lookup"><span data-stu-id="dae21-317">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dae21-318">לפי כלל מס '5, Q1 ו- Q2 הן שתי הצעות מחיר לאותה הזדמנות, כך שניתן להשתמש בשתיהן להערכת אותם מרכיבי הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="dae21-318">Per Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="dae21-319">O1</span><span class="sxs-lookup"><span data-stu-id="dae21-319">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="dae21-320">ר2</span><span class="sxs-lookup"><span data-stu-id="dae21-320">Q2</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="dae21-321">QL1</span><span class="sxs-lookup"><span data-stu-id="dae21-321">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-322">P1</span><span class="sxs-lookup"><span data-stu-id="dae21-322">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="dae21-323">כל משימות הפרויקט או ריק</span><span class="sxs-lookup"><span data-stu-id="dae21-323">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="dae21-324">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-324">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="dae21-325">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-325">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="dae21-326">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-326">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-327">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-327">Yes</span></span> </p>
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
<span data-ttu-id="dae21-328">O1</span><span class="sxs-lookup"><span data-stu-id="dae21-328">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="dae21-329">ר1</span><span class="sxs-lookup"><span data-stu-id="dae21-329">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="dae21-330">QL1</span><span class="sxs-lookup"><span data-stu-id="dae21-330">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-331">P1</span><span class="sxs-lookup"><span data-stu-id="dae21-331">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="dae21-332">כל משימות הפרויקט או ריק</span><span class="sxs-lookup"><span data-stu-id="dae21-332">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="dae21-333">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-333">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="dae21-334">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-334">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="dae21-335">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-335">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-336">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-336">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dae21-337">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="dae21-337">Not Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dae21-338">לפי כלל מס '4, Q1 ו- Q2 הן שתי הצעות מחיר להזדמנויות שונות, כך שלא ניתן להשתמש בשתיהן להערכת אותם מרכיבים של אותו הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="dae21-338">Per Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="dae21-339">O2</span><span class="sxs-lookup"><span data-stu-id="dae21-339">O2</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="dae21-340">ר1</span><span class="sxs-lookup"><span data-stu-id="dae21-340">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="dae21-341">QL1</span><span class="sxs-lookup"><span data-stu-id="dae21-341">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-342">P1</span><span class="sxs-lookup"><span data-stu-id="dae21-342">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="dae21-343">כל משימות הפרויקט או ריק</span><span class="sxs-lookup"><span data-stu-id="dae21-343">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="dae21-344">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-344">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="dae21-345">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-345">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="dae21-346">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-346">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dae21-347">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="dae21-347">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
