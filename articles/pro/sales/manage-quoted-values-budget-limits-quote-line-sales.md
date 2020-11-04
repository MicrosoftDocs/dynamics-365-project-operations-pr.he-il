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
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077238"
---
# <a name="project-based-quote-lines-pro"></a><span data-ttu-id="2ae66-104">שורות הצעות מחיר מבוססות פרויקט (Pro)</span><span class="sxs-lookup"><span data-stu-id="2ae66-104">Project-based quote lines (Pro)</span></span>

<span data-ttu-id="2ae66-105">_**חל על** : פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="2ae66-105">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="2ae66-106">שורות הצעת מחיר מבוססות פרויקט נועדו לעזור להעריך את עבודת הפרויקט עבור התקשרות.</span><span class="sxs-lookup"><span data-stu-id="2ae66-106">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="2ae66-107">המבנה של שורת הצעות מחיר מבוסס פרויקט מורחב להערכות פרויקט באמצעות המושגים הבאים:</span><span class="sxs-lookup"><span data-stu-id="2ae66-107">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="2ae66-108">שיטת חיוב</span><span class="sxs-lookup"><span data-stu-id="2ae66-108">Billing Method</span></span>
- <span data-ttu-id="2ae66-109">מיפוי פרויקטים ומשימות</span><span class="sxs-lookup"><span data-stu-id="2ae66-109">Project and Task Mapping</span></span>
- <span data-ttu-id="2ae66-110">סווגי עסקה כלולים</span><span class="sxs-lookup"><span data-stu-id="2ae66-110">Included Transaction classes</span></span>
- <span data-ttu-id="2ae66-111">מגבלת 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="2ae66-111">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="2ae66-112">הגדרת יכולת חיוב</span><span class="sxs-lookup"><span data-stu-id="2ae66-112">Chargeability setup</span></span>
- <span data-ttu-id="2ae66-113">הערכה באמצעות פרטי קו הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="2ae66-113">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="2ae66-114">לקוחות של שורת הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="2ae66-114">Quote line Customers</span></span>

<span data-ttu-id="2ae66-115">הטבלה הבאה מספקת מידע אודות השדות המופיעים בכרטיסיה **כללי** של שורת הצעת מחיר מבוססת פרויקט.</span><span class="sxs-lookup"><span data-stu-id="2ae66-115">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="2ae66-116">שדות אלה מסייעים בהכנת הבסיס לביצוע הערכה מפורטת ויסודיות לעבודת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="2ae66-116">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="2ae66-117">**שדה**</span><span class="sxs-lookup"><span data-stu-id="2ae66-117">**Field**</span></span> | <span data-ttu-id="2ae66-118">**רלוונטיות, מטרה והכוונה**</span><span class="sxs-lookup"><span data-stu-id="2ae66-118">**Relevance, purpose, and guidance**</span></span> | <span data-ttu-id="2ae66-119">**השפעה במורד הזרם**</span><span class="sxs-lookup"><span data-stu-id="2ae66-119">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="2ae66-120">שם</span><span class="sxs-lookup"><span data-stu-id="2ae66-120">Name</span></span> | <span data-ttu-id="2ae66-121">שם שורת הצעת המחיר אשר אמורה לעזור לך לזהות את המרכיב המובדל של הצעת המחיר שעבורה מתבצעת הערכה.</span><span class="sxs-lookup"><span data-stu-id="2ae66-121">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="2ae66-122">מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-122">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2ae66-123">שיטת חיוב</span><span class="sxs-lookup"><span data-stu-id="2ae66-123">Billing Method</span></span> | <span data-ttu-id="2ae66-124">כשנוצרת הצעת מחיר מהזדמנות, ערך זה מועתק מהשדה התואם שבשורת הזדמנות.</span><span class="sxs-lookup"><span data-stu-id="2ae66-124">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="2ae66-125">שדה זה כולל את שני המודלי החוזה העיקריים הנתמכים על ידי Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="2ae66-125">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="2ae66-126">- מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="2ae66-126">- Fixed price</span></span></br><span data-ttu-id="2ae66-127">- זמן וחומרים.</span><span class="sxs-lookup"><span data-stu-id="2ae66-127">- Time and material.</span></span>| <span data-ttu-id="2ae66-128">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-128">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2ae66-129">פרויקט</span><span class="sxs-lookup"><span data-stu-id="2ae66-129">Project</span></span> | <span data-ttu-id="2ae66-130">השתמש בשדה אופציונלי זה כדי לזהות את הפרויקט שישמש להגשת העבודה בהתקשרות זו.</span><span class="sxs-lookup"><span data-stu-id="2ae66-130">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="2ae66-131">כאשר פרויקט ממופה לשורת הצעת מחיר, זה עוזר בהגדרת משימות הניתנות לחיוב וגם בכנסת הערכה מבוססת פרויקט לשורת הצעת המחיר, כפרטים בשורת הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-131">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="2ae66-132">כאשר פרויקט אינו ממופה לשורת הצעת מחיר מבוססת פרויקט, יש ליצור את ההערכה באופן ידני על ידי יצירת כל פרט שבשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-132">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="2ae66-133">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-133">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="2ae66-134">משימות כלולות</span><span class="sxs-lookup"><span data-stu-id="2ae66-134">Included Tasks</span></span> | <span data-ttu-id="2ae66-135">הוא מציין אם שורת הצעת מחיר זו משמשת עבור כל משימות הפרויקט של הפרויקט שנבחר או עבור חלקן.</span><span class="sxs-lookup"><span data-stu-id="2ae66-135">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="2ae66-136">שדהזה כולל את הערכים אפשריים הבאים:</span><span class="sxs-lookup"><span data-stu-id="2ae66-136">This field has the following possible values:</span></span></br><span data-ttu-id="2ae66-137">- כל משימות הפרויקט</span><span class="sxs-lookup"><span data-stu-id="2ae66-137">- All project tasks</span></span></br><span data-ttu-id="2ae66-138">- משימות פרויקט נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="2ae66-138">- Selected project tasks only</span></span></br><span data-ttu-id="2ae66-139">ערך ריק בשדה זה שווה ערך לאפשרות **כל משימות הפרויקט**.</span><span class="sxs-lookup"><span data-stu-id="2ae66-139">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="2ae66-140">כשנבחרת האפשרות **משימות הפרויקט נבחרות בלבד** , אז בדף הפרויקט, הכרטיסיה **הגדרת חיוב משימות** מאפשרת לך לבחור משימות ספציפיות כדי לשייך אותן לשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="2ae66-140">When **Selected project tasks only** is selected then on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="2ae66-141">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-141">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2ae66-142">כלול זמן</span><span class="sxs-lookup"><span data-stu-id="2ae66-142">Include Time</span></span> | <span data-ttu-id="2ae66-143">דגל **כן**/**לא** מציין אם עסקאות זמן או עלויות עבודה בפרויקט שנבחר ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="2ae66-143">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="2ae66-144">הערך **לא** מציין שעסקאות זמן או עלויות עבודה לא ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="2ae66-144">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="2ae66-145">הערך **כן** מציין שעסקאות זמן או עלויות עבודה ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="2ae66-145">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="2ae66-146">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-146">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2ae66-147">כלול הוצאה</span><span class="sxs-lookup"><span data-stu-id="2ae66-147">Include Expense</span></span> | <span data-ttu-id="2ae66-148">דגל **כן**/**לא** מציין אם עלויות ההוצאות בפרויקט שנבחר ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="2ae66-148">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="2ae66-149">הערך **לא** מציין שעלויות ההוצאות לא ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="2ae66-149">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="2ae66-150">הערך **כן** מציין שעלויות ההוצאות ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="2ae66-150">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="2ae66-151">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-151">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2ae66-152">כלול תשלום</span><span class="sxs-lookup"><span data-stu-id="2ae66-152">Include Fee</span></span> | <span data-ttu-id="2ae66-153">דגל **כן**/**לא** מציין אם עמלות על הפרויקט שנבחר ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="2ae66-153">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="2ae66-154">הערך **לא** מציין שהעמלות לא ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="2ae66-154">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="2ae66-155">הערך **כן** מציין שהעמלות ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="2ae66-155">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="2ae66-156">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-156">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2ae66-157">הסכום של הצעת המחיר</span><span class="sxs-lookup"><span data-stu-id="2ae66-157">Quoted Amount</span></span> | <span data-ttu-id="2ae66-158">זהו סכום הצעת המחיר שינתן ללקוח עבור כל העבודה החזויה בשורת הצעת מחיר מבוססת פרויקט זו.</span><span class="sxs-lookup"><span data-stu-id="2ae66-158">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="2ae66-159">בהצעת מחיר שנוצרת מהזדמנות, ערך זה מועתק מהשדה **תקציב הלקוח** שבשורת הזדמנות.</span><span class="sxs-lookup"><span data-stu-id="2ae66-159">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="2ae66-160">כשבשורת צעת מחיר מבוססת הפרויקט יש פרטי שורה, שדה זה נעול לעריכה ומסוכם מהסכום שנמצא בפרטים בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-160">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="2ae66-161">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-161">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2ae66-162">מס משוער</span><span class="sxs-lookup"><span data-stu-id="2ae66-162">Estimated Tax</span></span> | <span data-ttu-id="2ae66-163">זהו שדה הניתן לעריכה שהמשתמש יכול להוסיף בו את סכום המס המשוער בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-163">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="2ae66-164">כשבשורת צעת מחיר מבוססת הפרויקט יש פרטי שורה, שדה זה נעול לעריכה ומסוכם מסכום המס שנמצא בפרטים בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-164">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="2ae66-165">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-165">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2ae66-166">סכום הצעת המחיר, אחרי מס</span><span class="sxs-lookup"><span data-stu-id="2ae66-166">Quoted Amount after Tax</span></span> | <span data-ttu-id="2ae66-167">שדה זה הוא סכום שורת הצעת המחיר לאחר מס והוא לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="2ae66-167">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="2ae66-168">הסכום בשדה זה מחושב כ *סכום הצעת המחיר + מס*.</span><span class="sxs-lookup"><span data-stu-id="2ae66-168">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="2ae66-169">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-169">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2ae66-170">מגבלת 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="2ae66-170">Not-to-exceed Limit</span></span> | <span data-ttu-id="2ae66-171">שדה זה ניתן לעריכה והוא זמין רק בשורות הצעות מחיר מבוססות פרויקט עם שיטת חיוב של **זמן וחומרים**.</span><span class="sxs-lookup"><span data-stu-id="2ae66-171">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="2ae66-172">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-172">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="2ae66-173">תקציב הלקוח</span><span class="sxs-lookup"><span data-stu-id="2ae66-173">Customer Budget</span></span> | <span data-ttu-id="2ae66-174">שדה זה ניתן לעריכה ומועתק מהשדה התואם בשורת ההזדמנות אם הצעת המחיר נוצרה מהזדמנות.</span><span class="sxs-lookup"><span data-stu-id="2ae66-174">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="2ae66-175">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-175">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="2ae66-176">כללי אימות עבור שדות בכרטיסיה 'כללי' של שורות הצעות מחיר מבוססות פרויקט</span><span class="sxs-lookup"><span data-stu-id="2ae66-176">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="2ae66-177">**כלל 1** : אם השדה **משימות כלולות** ריק, או אם הוא מוגדר ל **כל משימות הפרויקט** , פרויקט כלול בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-177">**Rule 1** : If the **Included Tasks** field is blank, or if it is set to **All project tasks** , a project is included in the quote line.</span></span>

<span data-ttu-id="2ae66-178">**כלל 2** : אם השדה **משימות כלולות** ריק, או אם הוא מוגדר ל **כל משימות הפרויקט** , פרויקט וסיווג עסקאות מסוים יכולים להיכלל רק בשורת הצעת מחיר מבוססת פרויקט אחת של הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-178">**Rule 2** : If the **Included Tasks** field is blank, or if it is set to **All project tasks** , a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="2ae66-179">**כלל 3** : אם השדה **משימות כלולות** מוגדר ל **משימות הפרויקט נבחרות בלבד** , פרויקט וסיווג עסקאות מסוים יכולים להיכלל בשורת הצעת מחיר מבוססת פרויקט מרובות של הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="2ae66-179">**Rule 3** : If the **Included Tasks** field is set to **Selected project tasks only** , a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="2ae66-180">**כלל 4** : אם להזדמנות יש הצעות מחיר מרובות, יכולות להיות שורות הצעות מחיר מהצעות מחיר שונות, שכולן מתייחסות לאותו פרויקט וכוללות את אותו סיווג עסקאות.</span><span class="sxs-lookup"><span data-stu-id="2ae66-180">**Rule 4** : If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="2ae66-181">**כלל 5** : אם הצעות המחיר אינן שייכות לאותה הזדמנות, הן אינן יכולות לכלול את אותו פרויקט וסיווג עסקאות.</span><span class="sxs-lookup"><span data-stu-id="2ae66-181">**Rule 5** : If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="2ae66-182">
                    <strong>הזדמנות</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2ae66-182">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="2ae66-183">
                    <strong>הצעת מחיר</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2ae66-183">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="2ae66-184">
                    <strong>שורת הצעת מחיר</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2ae66-184">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="2ae66-185">
                    <strong>פרויקט</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2ae66-185">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="90" valign="top">
                <p><span data-ttu-id="2ae66-186">
                    <strong>משימות כלולות</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2ae66-186">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="2ae66-187">
                    <strong>כלול זמן</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2ae66-187">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="2ae66-188">
                    <strong>כלול הוצאה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2ae66-188">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="2ae66-189">
                    <strong>הכללה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2ae66-189">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="2ae66-190">
                    <strong>תשלום</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2ae66-190">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="2ae66-191">
                    <strong>חוקי/לא חוקי</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2ae66-191">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="2ae66-192">
                    <strong>סיבה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="2ae66-192">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="2ae66-193">O1</span><span class="sxs-lookup"><span data-stu-id="2ae66-193">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2ae66-194">ר1</span><span class="sxs-lookup"><span data-stu-id="2ae66-194">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-195">QL1</span><span class="sxs-lookup"><span data-stu-id="2ae66-195">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-196">P1</span><span class="sxs-lookup"><span data-stu-id="2ae66-196">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="2ae66-197">ריק</span><span class="sxs-lookup"><span data-stu-id="2ae66-197">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-198">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-198">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-199">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-199">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-200">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-200">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2ae66-201">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="2ae66-201">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2ae66-202">הפרת כלל מס' 2.</span><span class="sxs-lookup"><span data-stu-id="2ae66-202">Violation of Rule #2.</span></span> <span data-ttu-id="2ae66-203">זמן, הוצאות ועמלות בפרויקט P1 כלולים בשורות הצעות מחיר QL1 ו-QL2.</span><span class="sxs-lookup"><span data-stu-id="2ae66-203">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="2ae66-204">O1</span><span class="sxs-lookup"><span data-stu-id="2ae66-204">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2ae66-205">ר1</span><span class="sxs-lookup"><span data-stu-id="2ae66-205">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-206">QL2</span><span class="sxs-lookup"><span data-stu-id="2ae66-206">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-207">P1</span><span class="sxs-lookup"><span data-stu-id="2ae66-207">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="2ae66-208">ריק</span><span class="sxs-lookup"><span data-stu-id="2ae66-208">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-209">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-209">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-210">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-210">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-211">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-211">Yes</span></span> </p>
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
<span data-ttu-id="2ae66-212">O1</span><span class="sxs-lookup"><span data-stu-id="2ae66-212">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2ae66-213">ר1</span><span class="sxs-lookup"><span data-stu-id="2ae66-213">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-214">QL1</span><span class="sxs-lookup"><span data-stu-id="2ae66-214">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-215">P1</span><span class="sxs-lookup"><span data-stu-id="2ae66-215">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="2ae66-216">ריק</span><span class="sxs-lookup"><span data-stu-id="2ae66-216">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-217">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-217">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-218">Yes</span><span class="sxs-lookup"><span data-stu-id="2ae66-218">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-219">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-219">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2ae66-220">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="2ae66-220">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2ae66-221">הפרת כלל מס' 2.</span><span class="sxs-lookup"><span data-stu-id="2ae66-221">Violation of Rule #2.</span></span> <span data-ttu-id="2ae66-222">זמן ועמלות בפרויקט P1 כלולים בשורות הצעות מחיר QL1 ו-QL2.</span><span class="sxs-lookup"><span data-stu-id="2ae66-222">Time and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="2ae66-223">O1</span><span class="sxs-lookup"><span data-stu-id="2ae66-223">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2ae66-224">ר1</span><span class="sxs-lookup"><span data-stu-id="2ae66-224">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-225">QL2</span><span class="sxs-lookup"><span data-stu-id="2ae66-225">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-226">P1</span><span class="sxs-lookup"><span data-stu-id="2ae66-226">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="2ae66-227">ריק</span><span class="sxs-lookup"><span data-stu-id="2ae66-227">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-228">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-228">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-229">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-229">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-230">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-230">Yes</span></span> </p>
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
<span data-ttu-id="2ae66-231">O1</span><span class="sxs-lookup"><span data-stu-id="2ae66-231">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2ae66-232">ר1</span><span class="sxs-lookup"><span data-stu-id="2ae66-232">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-233">QL1</span><span class="sxs-lookup"><span data-stu-id="2ae66-233">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-234">P1</span><span class="sxs-lookup"><span data-stu-id="2ae66-234">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="2ae66-235">ריק</span><span class="sxs-lookup"><span data-stu-id="2ae66-235">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-236">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-236">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-237">Yes</span><span class="sxs-lookup"><span data-stu-id="2ae66-237">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-238">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-238">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2ae66-239">חוקי</span><span class="sxs-lookup"><span data-stu-id="2ae66-239">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
<span data-ttu-id="2ae66-240">זמן ועמלות בפרויקט P1 כלולים ב-QL1.</span><span class="sxs-lookup"><span data-stu-id="2ae66-240">Time and Fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="2ae66-241">הוצאות בפרויקט P1 כלולות ב-QL2.</span><span class="sxs-lookup"><span data-stu-id="2ae66-241">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="2ae66-242">אין חפיפה במה שנכלל בכל שורת הצעת מחיר והוא תקף.</span><span class="sxs-lookup"><span data-stu-id="2ae66-242">There is no overlap in what is being included on each quote line and is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="2ae66-243">O1</span><span class="sxs-lookup"><span data-stu-id="2ae66-243">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2ae66-244">ר1</span><span class="sxs-lookup"><span data-stu-id="2ae66-244">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-245">QL2</span><span class="sxs-lookup"><span data-stu-id="2ae66-245">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-246">P1</span><span class="sxs-lookup"><span data-stu-id="2ae66-246">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="2ae66-247">ריק</span><span class="sxs-lookup"><span data-stu-id="2ae66-247">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-248">Yes</span><span class="sxs-lookup"><span data-stu-id="2ae66-248">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-249">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-250">Yes</span><span class="sxs-lookup"><span data-stu-id="2ae66-250">No</span></span> </p>
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
<span data-ttu-id="2ae66-251">O1</span><span class="sxs-lookup"><span data-stu-id="2ae66-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2ae66-252">ר1</span><span class="sxs-lookup"><span data-stu-id="2ae66-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-253">QL1</span><span class="sxs-lookup"><span data-stu-id="2ae66-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-254">P1</span><span class="sxs-lookup"><span data-stu-id="2ae66-254">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="2ae66-255">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="2ae66-255">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-256">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-256">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-257">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-257">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-258">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-258">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2ae66-259">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="2ae66-259">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2ae66-260">הפרת כלל מס' 2 שלעיל</span><span class="sxs-lookup"><span data-stu-id="2ae66-260">Violation of Rule #2 above</span></span> </p>
                <p>
<span data-ttu-id="2ae66-261">ר1 כולל זמן, הוצאות ועמלות על קבוצת משנה של משימות בפרויקט P1.</span><span class="sxs-lookup"><span data-stu-id="2ae66-261">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="2ae66-262">QL2 כולל זמן, הוצאות ועמלות עבור כל הפרויקט P1 וחופף למה שנכלל ר1.</span><span class="sxs-lookup"><span data-stu-id="2ae66-262">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="2ae66-263">O1</span><span class="sxs-lookup"><span data-stu-id="2ae66-263">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2ae66-264">ר1</span><span class="sxs-lookup"><span data-stu-id="2ae66-264">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-265">QL2</span><span class="sxs-lookup"><span data-stu-id="2ae66-265">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-266">P1</span><span class="sxs-lookup"><span data-stu-id="2ae66-266">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="2ae66-267">ריק</span><span class="sxs-lookup"><span data-stu-id="2ae66-267">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-268">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-268">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-269">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-269">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-270">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-270">Yes</span></span> </p>
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
<span data-ttu-id="2ae66-271">O1</span><span class="sxs-lookup"><span data-stu-id="2ae66-271">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2ae66-272">ר1</span><span class="sxs-lookup"><span data-stu-id="2ae66-272">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-273">QL1</span><span class="sxs-lookup"><span data-stu-id="2ae66-273">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-274">P1</span><span class="sxs-lookup"><span data-stu-id="2ae66-274">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="2ae66-275">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="2ae66-275">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-276">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-276">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-277">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-278">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-278">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2ae66-279">חוקי</span><span class="sxs-lookup"><span data-stu-id="2ae66-279">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2ae66-280">לפי כלל מס' 3 לעיל,</span><span class="sxs-lookup"><span data-stu-id="2ae66-280">Per Rule #3 above,</span></span> </p>
                <p>
<span data-ttu-id="2ae66-281">ר1 כולל זמן, הוצאות ועמלות על קבוצת משנה של משימות בפרויקט P1.</span><span class="sxs-lookup"><span data-stu-id="2ae66-281">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="2ae66-282">QL2 כולל זמן, הוצאות ועמלות עבור קבוצת משנה של משימות בפרויקט P1.</span><span class="sxs-lookup"><span data-stu-id="2ae66-282">QL2 includes Time, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="2ae66-283">האימות הנוסף היחיד הוא סביב קבוצת המשנה של המשימות ב-QL1 אשר שונה מקבוצת המשנה של המשימות ב-QL2.</span><span class="sxs-lookup"><span data-stu-id="2ae66-283">The only additional validation is around the subset of tasks on QL1 which are different from the subset of tasks on QL2.</span></span> <span data-ttu-id="2ae66-284">דבר זה מבטיח שלא יהיו חפיפות.</span><span class="sxs-lookup"><span data-stu-id="2ae66-284">This ensures that there are no overlaps.</span></span> <span data-ttu-id="2ae66-285">פעולה זו מתבצעת על ידי המערכת כאשר משימות משויכות.</span><span class="sxs-lookup"><span data-stu-id="2ae66-285">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="2ae66-286">O1</span><span class="sxs-lookup"><span data-stu-id="2ae66-286">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2ae66-287">ר1</span><span class="sxs-lookup"><span data-stu-id="2ae66-287">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-288">QL2</span><span class="sxs-lookup"><span data-stu-id="2ae66-288">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-289">P1</span><span class="sxs-lookup"><span data-stu-id="2ae66-289">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="2ae66-290">משימות נבחרות בלבד</span><span class="sxs-lookup"><span data-stu-id="2ae66-290">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-291">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-291">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-292">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-292">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-293">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-293">Yes</span></span> </p>
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
<span data-ttu-id="2ae66-294">O1</span><span class="sxs-lookup"><span data-stu-id="2ae66-294">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2ae66-295">ר1</span><span class="sxs-lookup"><span data-stu-id="2ae66-295">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-296">QL1</span><span class="sxs-lookup"><span data-stu-id="2ae66-296">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-297">P1</span><span class="sxs-lookup"><span data-stu-id="2ae66-297">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="2ae66-298">כל משימות הפרויקט או ריק</span><span class="sxs-lookup"><span data-stu-id="2ae66-298">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-299">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-299">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-300">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-300">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-301">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-301">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="2ae66-302">חוקי</span><span class="sxs-lookup"><span data-stu-id="2ae66-302">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2ae66-303">בהתבסס על כלל מס' 5, Q1 ו-Q2 הן שתי הצעות מחיר באותה הזדמנות, כך ששתיהן יכולות לשמש להערכת אותם רכיבי פרויקט.</span><span class="sxs-lookup"><span data-stu-id="2ae66-303">Based on Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="2ae66-304">O1</span><span class="sxs-lookup"><span data-stu-id="2ae66-304">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2ae66-305">ר2</span><span class="sxs-lookup"><span data-stu-id="2ae66-305">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-306">QL1</span><span class="sxs-lookup"><span data-stu-id="2ae66-306">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-307">P1</span><span class="sxs-lookup"><span data-stu-id="2ae66-307">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="2ae66-308">כל משימות הפרויקט או ריק</span><span class="sxs-lookup"><span data-stu-id="2ae66-308">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-309">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-309">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-310">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-310">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-311">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-311">Yes</span></span> </p>
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
<span data-ttu-id="2ae66-312">O1</span><span class="sxs-lookup"><span data-stu-id="2ae66-312">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2ae66-313">ר1</span><span class="sxs-lookup"><span data-stu-id="2ae66-313">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-314">QL1</span><span class="sxs-lookup"><span data-stu-id="2ae66-314">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-315">P1</span><span class="sxs-lookup"><span data-stu-id="2ae66-315">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="2ae66-316">כל משימות הפרויקט או ריק</span><span class="sxs-lookup"><span data-stu-id="2ae66-316">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-317">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-317">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-318">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-318">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-319">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-319">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="2ae66-320">חוקי</span><span class="sxs-lookup"><span data-stu-id="2ae66-320">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="2ae66-321">בהתבסס על כלל מס' 4, Q1 ו-Q2 הן שתי הצעות מחיר עבור הזדמנויות שונות, כך שהן אינן יכולות לשמש להערכת אותם הרכיבים של אותו הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="2ae66-321">Based on Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="2ae66-322">O2</span><span class="sxs-lookup"><span data-stu-id="2ae66-322">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="2ae66-323">ר1</span><span class="sxs-lookup"><span data-stu-id="2ae66-323">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-324">QL1</span><span class="sxs-lookup"><span data-stu-id="2ae66-324">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-325">P1</span><span class="sxs-lookup"><span data-stu-id="2ae66-325">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="2ae66-326">כל משימות הפרויקט או ריק</span><span class="sxs-lookup"><span data-stu-id="2ae66-326">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-327">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-327">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="2ae66-328">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-328">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="2ae66-329">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="2ae66-329">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="2ae66-330">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="2ae66-330">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>

