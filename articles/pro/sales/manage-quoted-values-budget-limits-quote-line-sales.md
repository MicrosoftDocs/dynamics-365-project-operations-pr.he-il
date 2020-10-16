---
title: שורות הצעות מחיר מבוססות פרויקט (Pro)
description: נושא זה מספק מידע על עבודה עם שורות הצעות מחיר המבוססות פרויקט לעבודת פרויקט. (Pro)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a409d1e378afe97de7fb6c77cf3ad6703661bdff
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908189"
---
# <a name="project-based-quote-lines-pro"></a><span data-ttu-id="5df67-104">שורות הצעות מחיר מבוססות פרויקט (Pro)</span><span class="sxs-lookup"><span data-stu-id="5df67-104">Project-based quote lines (Pro)</span></span>

<span data-ttu-id="5df67-105">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="5df67-105">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5df67-106">שורות הצעת מחיר מבוססות פרויקט נועדו לעזור להעריך את עבודת הפרויקט עבור התקשרות.</span><span class="sxs-lookup"><span data-stu-id="5df67-106">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="5df67-107">המבנה של שורת הצעות מחיר מבוסס פרויקט מורחב להערכות פרויקט באמצעות המושגים הבאים:</span><span class="sxs-lookup"><span data-stu-id="5df67-107">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="5df67-108">שיטת חיוב</span><span class="sxs-lookup"><span data-stu-id="5df67-108">Billing Method</span></span>
- <span data-ttu-id="5df67-109">מיפוי פרוייקטים ומשימות</span><span class="sxs-lookup"><span data-stu-id="5df67-109">Project and Task Mapping</span></span>
- <span data-ttu-id="5df67-110">סווגי עסקה כלולים</span><span class="sxs-lookup"><span data-stu-id="5df67-110">Included Transaction classes</span></span>
- <span data-ttu-id="5df67-111">מגבלת 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="5df67-111">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="5df67-112">הגדרת יכולת חיוב</span><span class="sxs-lookup"><span data-stu-id="5df67-112">Chargeability setup</span></span>
- <span data-ttu-id="5df67-113">הערכה באמצעות פרטי קו הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="5df67-113">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="5df67-114">לקוחות של שורת הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="5df67-114">Quote line Customers</span></span>

<span data-ttu-id="5df67-115">הטבלה הבאה מספקת מידע אודות השדות המופיעים בכרטיסיה **כללי** של שורת הצעת מחיר מבוססת פרויקט.</span><span class="sxs-lookup"><span data-stu-id="5df67-115">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="5df67-116">שדות אלה מסייעים בהכנת הבסיס לביצוע הערכה מפורטת ויסודיות לעבודת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="5df67-116">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="5df67-117">**שדה**</span><span class="sxs-lookup"><span data-stu-id="5df67-117">**Field**</span></span> | <span data-ttu-id="5df67-118">**רלוונטיות, מטרה והכוונה**</span><span class="sxs-lookup"><span data-stu-id="5df67-118">**Relevance, purpose, and guidance**</span></span> | <span data-ttu-id="5df67-119">**השפעה במורד הזרם**</span><span class="sxs-lookup"><span data-stu-id="5df67-119">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="5df67-120">שם</span><span class="sxs-lookup"><span data-stu-id="5df67-120">Name</span></span> | <span data-ttu-id="5df67-121">שם שורת הצעת המחיר אשר אמורה לעזור לך לזהות את המרכיב המובדל של הצעת המחיר שעבורה מתבצעת הערכה.</span><span class="sxs-lookup"><span data-stu-id="5df67-121">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="5df67-122">מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-122">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="5df67-123">שיטת חיוב</span><span class="sxs-lookup"><span data-stu-id="5df67-123">Billing Method</span></span> | <span data-ttu-id="5df67-124">כשנוצרת הצעת מחיר מהזדמנות, ערך זה מועתק מהשדה התואם שבשורת הזדמנות.</span><span class="sxs-lookup"><span data-stu-id="5df67-124">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="5df67-125">שדה זה כולל את שני המודלי החוזה העיקריים הנתמכים על ידי Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="5df67-125">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="5df67-126">- מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="5df67-126">- Fixed price</span></span></br><span data-ttu-id="5df67-127">- זמן וחומרים.</span><span class="sxs-lookup"><span data-stu-id="5df67-127">- Time and material.</span></span>| <span data-ttu-id="5df67-128">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-128">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="5df67-129">פרויקט</span><span class="sxs-lookup"><span data-stu-id="5df67-129">Project</span></span> | <span data-ttu-id="5df67-130">השתמש בשדה אופציונלי זה כדי לזהות את הפרויקט שישמש להגשת העבודה בהתקשרות זו.</span><span class="sxs-lookup"><span data-stu-id="5df67-130">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="5df67-131">כאשר פרויקט ממופה לשורת הצעת מחיר, זה עוזר בהגדרת משימות הניתנות לחיוב וגם בכנסת הערכה מבוססת פרויקט לשורת הצעת המחיר, כפרטים בשורת הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-131">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="5df67-132">כאשר פרויקט אינו ממופה לשורת הצעת מחיר מבוססת פרויקט, יש ליצור את ההערכה באופן ידני על ידי יצירת כל פרט שבשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-132">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="5df67-133">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-133">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="5df67-134">משימות כלולות</span><span class="sxs-lookup"><span data-stu-id="5df67-134">Included Tasks</span></span> | <span data-ttu-id="5df67-135">הוא מציין אם שורת הצעת מחיר זו משמשת עבור כל משימות הפרויקט של הפרויקט שנבחר או עבור חלקן.</span><span class="sxs-lookup"><span data-stu-id="5df67-135">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="5df67-136">שדהזה כולל את הערכים אפשריים הבאים:</span><span class="sxs-lookup"><span data-stu-id="5df67-136">This field has the following possible values:</span></span></br><span data-ttu-id="5df67-137">- כל משימות הפרויקט</span><span class="sxs-lookup"><span data-stu-id="5df67-137">- All project tasks</span></span></br><span data-ttu-id="5df67-138">- משימות פרויקט נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="5df67-138">- Selected project tasks only</span></span></br><span data-ttu-id="5df67-139">ערך ריק בשדה זה שווה ערך לאפשרות **כל משימות הפרויקט**.</span><span class="sxs-lookup"><span data-stu-id="5df67-139">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="5df67-140">כשנבחרת האפשרות **משימות הפרויקט נבחרות בלבד**, אז בדף הפרויקט, הכרטיסיה **הגדרת חיוב משימות** מאפשרת לך לבחור משימות ספציפיות כדי לשייך אותן לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="5df67-140">When **Selected project tasks only** is selected then on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="5df67-141">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-141">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="5df67-142">כלול זמן</span><span class="sxs-lookup"><span data-stu-id="5df67-142">Include Time</span></span> | <span data-ttu-id="5df67-143">דגל **כן**/**לא** מציין אם עסקאות זמן או עלויות עבודה בפרויקט שנבחר ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="5df67-143">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="5df67-144">הערך **לא** מציין שעסקאות זמן או עלויות עבודה לא ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="5df67-144">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="5df67-145">הערך **כן** מציין שעסקאות זמן או עלויות עבודה ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="5df67-145">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="5df67-146">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-146">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="5df67-147">כלול הוצאה</span><span class="sxs-lookup"><span data-stu-id="5df67-147">Include Expense</span></span> | <span data-ttu-id="5df67-148">דגל **כן**/**לא** מציין אם עלויות ההוצאות בפרויקט שנבחר ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="5df67-148">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="5df67-149">הערך **לא** מציין שעלויות ההוצאות לא ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="5df67-149">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="5df67-150">הערך **כן** מציין שעלויות ההוצאות ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="5df67-150">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="5df67-151">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-151">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="5df67-152">כלול תשלום</span><span class="sxs-lookup"><span data-stu-id="5df67-152">Include Fee</span></span> | <span data-ttu-id="5df67-153">דגל **כן**/**לא** מציין אם עמלות על הפרויקט שנבחר ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="5df67-153">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="5df67-154">הערך **לא** מציין שהעמלות לא ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="5df67-154">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="5df67-155">הערך **כן** מציין שהעמלות ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="5df67-155">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="5df67-156">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-156">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="5df67-157">הסכום של הצעת המחיר</span><span class="sxs-lookup"><span data-stu-id="5df67-157">Quoted Amount</span></span> | <span data-ttu-id="5df67-158">זהו סכום הצעת המחיר שינתן ללקוח עבור כל העבודה החזויה בשורת הצעת מחיר מבוססת פרויקט זו.</span><span class="sxs-lookup"><span data-stu-id="5df67-158">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="5df67-159">בהצעת מחיר שנוצרת מהזדמנות, ערך זה מועתק מהשדה **תקציב הלקוח** שבשורת הזדמנות.</span><span class="sxs-lookup"><span data-stu-id="5df67-159">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="5df67-160">כשבשורת צעת מחיר מבוססת הפרויקט יש פרטי שורה, שדה זה נעול לעריכה ומסוכם מהסכום שנמצא בפרטים בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-160">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="5df67-161">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-161">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="5df67-162">מס משוער</span><span class="sxs-lookup"><span data-stu-id="5df67-162">Estimated Tax</span></span> | <span data-ttu-id="5df67-163">זהו שדה הניתן לעריכה שהמשתמש יכול להוסיף בו את סכום המס המשוער בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-163">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="5df67-164">כשבשורת צעת מחיר מבוססת הפרויקט יש פרטי שורה, שדה זה נעול לעריכה ומסוכם מסכום המס שנמצא בפרטים בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-164">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="5df67-165">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-165">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="5df67-166">סכום הצעת המחיר, אחרי מס</span><span class="sxs-lookup"><span data-stu-id="5df67-166">Quoted Amount after Tax</span></span> | <span data-ttu-id="5df67-167">שדה זה הוא סכום שורת הצעת המחיר לאחר מס והוא לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="5df67-167">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="5df67-168">הסכום בשדה זה מחושב כ*סכום הצעת המחיר + מס*.</span><span class="sxs-lookup"><span data-stu-id="5df67-168">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="5df67-169">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-169">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="5df67-170">מגבלת 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="5df67-170">Not-to-exceed Limit</span></span> | <span data-ttu-id="5df67-171">שדה זה ניתן לעריכה והוא זמין רק בשורות הצעות מחיר מבוססות פרויקט עם שיטת חיוב של **זמן וחומרים**.</span><span class="sxs-lookup"><span data-stu-id="5df67-171">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="5df67-172">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-172">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="5df67-173">תקציב הלקוח</span><span class="sxs-lookup"><span data-stu-id="5df67-173">Customer Budget</span></span> | <span data-ttu-id="5df67-174">שדה זה ניתן לעריכה ומועתק מהשדה התואם בשורת ההזדמנות אם הצעת המחיר נוצרה מהזדמנות.</span><span class="sxs-lookup"><span data-stu-id="5df67-174">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="5df67-175">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-175">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="5df67-176">כללי אימות עבור שדות בכרטיסיה 'כללי' של שורות הצעות מחיר מבוססות פרויקט</span><span class="sxs-lookup"><span data-stu-id="5df67-176">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="5df67-177">**כלל 1**: אם השדה **משימות כלולות** ריק, או אם הוא מוגדר ל**כל משימות הפרויקט**, פרויקט כלול בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-177">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="5df67-178">**כלל 2**: אם השדה **משימות כלולות** ריק, או אם הוא מוגדר ל**כל משימות הפרויקט**, פרויקט וסיווג עסקאות מסוים יכולים להיכלל רק בשורת הצעת מחיר מבוססת פרויקט אחת של הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-178">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="5df67-179">**כלל 3**: אם השדה **משימות כלולות** מוגדר ל**משימות הפרויקט נבחרות בלבד**, פרויקט וסיווג עסקאות מסוים יכולים להיכלל בשורת הצעת מחיר מבוססת פרויקט מרובות של הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="5df67-179">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="5df67-180">**כלל 4**: אם להזדמנות יש הצעות מחיר מרובות, יכולות להיות שורות הצעות מחיר מהצעות מחיר שונות, שכולן מתייחסות לאותו פרויקט וכוללות את אותו סיווג עסקאות.</span><span class="sxs-lookup"><span data-stu-id="5df67-180">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="5df67-181">**כלל 5**: אם הצעות המחיר אינן שייכות לאותה הזדמנות, הן אינן יכולות לכלול את אותו פרויקט וסיווג עסקאות.</span><span class="sxs-lookup"><span data-stu-id="5df67-181">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="5df67-182">
                    <strong>הזדמנות</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5df67-182">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="5df67-183">
                    <strong>הצעת מחיר</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5df67-183">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="5df67-184">
                    <strong>שורת הצעת מחיר</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5df67-184">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="5df67-185">
                    <strong>פרויקט</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5df67-185">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="90" valign="top">
                <p><span data-ttu-id="5df67-186">
                    <strong>משימות כלולות</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5df67-186">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="5df67-187">
                    <strong>כלול זמן</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5df67-187">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="5df67-188">
                    <strong>כלול הוצאה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5df67-188">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="5df67-189">
                    <strong>הכללה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5df67-189">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="5df67-190">
                    <strong>תשלום</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5df67-190">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="5df67-191">
                    <strong>חוקי/לא חוקי</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5df67-191">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="5df67-192">
                    <strong>סיבה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="5df67-192">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="5df67-193">O1</span><span class="sxs-lookup"><span data-stu-id="5df67-193">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="5df67-194">ר1</span><span class="sxs-lookup"><span data-stu-id="5df67-194">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-195">QL1</span><span class="sxs-lookup"><span data-stu-id="5df67-195">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-196">P1</span><span class="sxs-lookup"><span data-stu-id="5df67-196">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="5df67-197">ריק</span><span class="sxs-lookup"><span data-stu-id="5df67-197">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-198">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-198">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-199">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-199">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-200">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-200">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5df67-201">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="5df67-201">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5df67-202">הפרת כלל מס' 2.</span><span class="sxs-lookup"><span data-stu-id="5df67-202">Violation of Rule #2.</span></span> <span data-ttu-id="5df67-203">זמן, הוצאות ועמלות בפרויקט P1 כלולים בשורות הצעות מחיר QL1 ו-QL2.</span><span class="sxs-lookup"><span data-stu-id="5df67-203">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="5df67-204">O1</span><span class="sxs-lookup"><span data-stu-id="5df67-204">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="5df67-205">ר1</span><span class="sxs-lookup"><span data-stu-id="5df67-205">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-206">QL2</span><span class="sxs-lookup"><span data-stu-id="5df67-206">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-207">P1</span><span class="sxs-lookup"><span data-stu-id="5df67-207">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="5df67-208">ריק</span><span class="sxs-lookup"><span data-stu-id="5df67-208">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-209">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-209">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-210">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-210">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-211">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-211">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="5df67-212">O1</span><span class="sxs-lookup"><span data-stu-id="5df67-212">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="5df67-213">ר1</span><span class="sxs-lookup"><span data-stu-id="5df67-213">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-214">QL1</span><span class="sxs-lookup"><span data-stu-id="5df67-214">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-215">P1</span><span class="sxs-lookup"><span data-stu-id="5df67-215">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="5df67-216">ריק</span><span class="sxs-lookup"><span data-stu-id="5df67-216">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-217">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-217">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-218">Yes</span><span class="sxs-lookup"><span data-stu-id="5df67-218">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-219">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-219">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5df67-220">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="5df67-220">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5df67-221">הפרת כלל מס' 2.</span><span class="sxs-lookup"><span data-stu-id="5df67-221">Violation of Rule #2.</span></span> <span data-ttu-id="5df67-222">זמן ועמלות בפרויקט P1 כלולים בשורות הצעות מחיר QL1 ו-QL2.</span><span class="sxs-lookup"><span data-stu-id="5df67-222">Time and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="5df67-223">O1</span><span class="sxs-lookup"><span data-stu-id="5df67-223">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="5df67-224">ר1</span><span class="sxs-lookup"><span data-stu-id="5df67-224">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-225">QL2</span><span class="sxs-lookup"><span data-stu-id="5df67-225">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-226">P1</span><span class="sxs-lookup"><span data-stu-id="5df67-226">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="5df67-227">ריק</span><span class="sxs-lookup"><span data-stu-id="5df67-227">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-228">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-228">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-229">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-229">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-230">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-230">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="5df67-231">O1</span><span class="sxs-lookup"><span data-stu-id="5df67-231">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="5df67-232">ר1</span><span class="sxs-lookup"><span data-stu-id="5df67-232">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-233">QL1</span><span class="sxs-lookup"><span data-stu-id="5df67-233">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-234">P1</span><span class="sxs-lookup"><span data-stu-id="5df67-234">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="5df67-235">ריק</span><span class="sxs-lookup"><span data-stu-id="5df67-235">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-236">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-236">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-237">Yes</span><span class="sxs-lookup"><span data-stu-id="5df67-237">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-238">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-238">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5df67-239">חוקי</span><span class="sxs-lookup"><span data-stu-id="5df67-239">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
<span data-ttu-id="5df67-240">זמן ועמלות בפרויקט P1 כלולים ב-QL1.</span><span class="sxs-lookup"><span data-stu-id="5df67-240">Time and Fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="5df67-241">הוצאות בפרויקט P1 כלולות ב-QL2.</span><span class="sxs-lookup"><span data-stu-id="5df67-241">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="5df67-242">אין חפיפה במה שנכלל בכל שורת הצעת מחיר והוא תקף.</span><span class="sxs-lookup"><span data-stu-id="5df67-242">There is no overlap in what is being included on each quote line and is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="5df67-243">O1</span><span class="sxs-lookup"><span data-stu-id="5df67-243">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="5df67-244">ר1</span><span class="sxs-lookup"><span data-stu-id="5df67-244">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-245">QL2</span><span class="sxs-lookup"><span data-stu-id="5df67-245">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-246">P1</span><span class="sxs-lookup"><span data-stu-id="5df67-246">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="5df67-247">ריק</span><span class="sxs-lookup"><span data-stu-id="5df67-247">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-248">Yes</span><span class="sxs-lookup"><span data-stu-id="5df67-248">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-249">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-250">Yes</span><span class="sxs-lookup"><span data-stu-id="5df67-250">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="5df67-251">O1</span><span class="sxs-lookup"><span data-stu-id="5df67-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="5df67-252">ר1</span><span class="sxs-lookup"><span data-stu-id="5df67-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-253">QL1</span><span class="sxs-lookup"><span data-stu-id="5df67-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-254">P1</span><span class="sxs-lookup"><span data-stu-id="5df67-254">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="5df67-255">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="5df67-255">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-256">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-256">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-257">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-257">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-258">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-258">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5df67-259">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="5df67-259">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5df67-260">הפרת כלל מס' 2 שלעיל</span><span class="sxs-lookup"><span data-stu-id="5df67-260">Violation of Rule #2 above</span></span> </p>
                <p>
<span data-ttu-id="5df67-261">ר1 כולל זמן, הוצאות ועמלות על קבוצת משנה של משימות בפרויקט P1.</span><span class="sxs-lookup"><span data-stu-id="5df67-261">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="5df67-262">QL2 כולל זמן, הוצאות ועמלות עבור כל הפרויקט P1 וחופף למה שנכלל ר1.</span><span class="sxs-lookup"><span data-stu-id="5df67-262">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="5df67-263">O1</span><span class="sxs-lookup"><span data-stu-id="5df67-263">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="5df67-264">ר1</span><span class="sxs-lookup"><span data-stu-id="5df67-264">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-265">QL2</span><span class="sxs-lookup"><span data-stu-id="5df67-265">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-266">P1</span><span class="sxs-lookup"><span data-stu-id="5df67-266">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="5df67-267">ריק</span><span class="sxs-lookup"><span data-stu-id="5df67-267">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-268">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-268">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-269">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-269">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-270">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-270">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="5df67-271">O1</span><span class="sxs-lookup"><span data-stu-id="5df67-271">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="5df67-272">ר1</span><span class="sxs-lookup"><span data-stu-id="5df67-272">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-273">QL1</span><span class="sxs-lookup"><span data-stu-id="5df67-273">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-274">P1</span><span class="sxs-lookup"><span data-stu-id="5df67-274">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="5df67-275">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="5df67-275">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-276">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-276">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-277">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-278">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-278">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5df67-279">חוקי</span><span class="sxs-lookup"><span data-stu-id="5df67-279">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5df67-280">לפי כלל מס' 3 לעיל,</span><span class="sxs-lookup"><span data-stu-id="5df67-280">Per Rule #3 above,</span></span> </p>
                <p>
<span data-ttu-id="5df67-281">ר1 כולל זמן, הוצאות ועמלות על קבוצת משנה של משימות בפרויקט P1.</span><span class="sxs-lookup"><span data-stu-id="5df67-281">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="5df67-282">QL2 כולל זמן, הוצאות ועמלות עבור קבוצת משנה של משימות בפרויקט P1.</span><span class="sxs-lookup"><span data-stu-id="5df67-282">QL2 includes Time, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="5df67-283">האימות הנוסף היחיד הוא סביב קבוצת המשנה של המשימות ב-QL1 אשר שונה מקבוצת המשנה של המשימות ב-QL2.</span><span class="sxs-lookup"><span data-stu-id="5df67-283">The only additional validation is around the subset of tasks on QL1 which are different from the subset of tasks on QL2.</span></span> <span data-ttu-id="5df67-284">דבר זה מבטיח שלא יהיו חפיפות.</span><span class="sxs-lookup"><span data-stu-id="5df67-284">This ensures that there are no overlaps.</span></span> <span data-ttu-id="5df67-285">פעולה זו מתבצעת על ידי המערכת כאשר משימות משויכות.</span><span class="sxs-lookup"><span data-stu-id="5df67-285">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="5df67-286">O1</span><span class="sxs-lookup"><span data-stu-id="5df67-286">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="5df67-287">ר1</span><span class="sxs-lookup"><span data-stu-id="5df67-287">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-288">QL2</span><span class="sxs-lookup"><span data-stu-id="5df67-288">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-289">P1</span><span class="sxs-lookup"><span data-stu-id="5df67-289">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="5df67-290">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="5df67-290">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-291">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-291">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-292">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-292">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-293">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-293">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="5df67-294">O1</span><span class="sxs-lookup"><span data-stu-id="5df67-294">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="5df67-295">ר1</span><span class="sxs-lookup"><span data-stu-id="5df67-295">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-296">QL1</span><span class="sxs-lookup"><span data-stu-id="5df67-296">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-297">P1</span><span class="sxs-lookup"><span data-stu-id="5df67-297">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="5df67-298">כל משימות הפרוייקט או ריק</span><span class="sxs-lookup"><span data-stu-id="5df67-298">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-299">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-299">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-300">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-300">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-301">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-301">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="5df67-302">חוקי</span><span class="sxs-lookup"><span data-stu-id="5df67-302">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5df67-303">בהתבסס על כלל מס' 5, Q1 ו-Q2 הן שתי הצעות מחיר באותה הזדמנות, כך ששתיהן יכולות לשמש להערכת אותם רכיבי פרויקט.</span><span class="sxs-lookup"><span data-stu-id="5df67-303">Based on Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="5df67-304">O1</span><span class="sxs-lookup"><span data-stu-id="5df67-304">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="5df67-305">ר2</span><span class="sxs-lookup"><span data-stu-id="5df67-305">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-306">QL1</span><span class="sxs-lookup"><span data-stu-id="5df67-306">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-307">P1</span><span class="sxs-lookup"><span data-stu-id="5df67-307">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="5df67-308">כל משימות הפרוייקט או ריק</span><span class="sxs-lookup"><span data-stu-id="5df67-308">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-309">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-309">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-310">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-310">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-311">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-311">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="5df67-312">O1</span><span class="sxs-lookup"><span data-stu-id="5df67-312">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="5df67-313">ר1</span><span class="sxs-lookup"><span data-stu-id="5df67-313">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-314">QL1</span><span class="sxs-lookup"><span data-stu-id="5df67-314">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-315">P1</span><span class="sxs-lookup"><span data-stu-id="5df67-315">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="5df67-316">כל משימות הפרוייקט או ריק</span><span class="sxs-lookup"><span data-stu-id="5df67-316">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-317">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-317">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-318">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-318">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-319">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-319">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="5df67-320">חוקי</span><span class="sxs-lookup"><span data-stu-id="5df67-320">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="5df67-321">בהתבסס על כלל מס' 4, Q1 ו-Q2 הן שתי הצעות מחיר עבור הזדמנויות שונות, כך שהן אינן יכולות לשמש להערכת אותם הרכיבים של אותו הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="5df67-321">Based on Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="5df67-322">O2</span><span class="sxs-lookup"><span data-stu-id="5df67-322">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="5df67-323">ר1</span><span class="sxs-lookup"><span data-stu-id="5df67-323">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-324">QL1</span><span class="sxs-lookup"><span data-stu-id="5df67-324">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-325">P1</span><span class="sxs-lookup"><span data-stu-id="5df67-325">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="5df67-326">כל משימות הפרוייקט או ריק</span><span class="sxs-lookup"><span data-stu-id="5df67-326">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-327">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-327">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="5df67-328">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-328">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="5df67-329">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="5df67-329">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="5df67-330">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="5df67-330">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>

