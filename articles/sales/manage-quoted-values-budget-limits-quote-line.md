---
title: שורות הצעת מחיר המבוססות על פרוייקט
description: נושא זה מספק מידע על עבודה עם שורות הצעות מחיר המבוססות פרויקט לעבודת פרויקט.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 06a47c45dc3b3b174658e2fba14d3d2050aabf85
ms.sourcegitcommit: a0f80d024a5d3112a39781815bd31d0c05ddaf6f
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/30/2020
ms.locfileid: "3906187"
---
# <a name="project-based-quote-lines"></a><span data-ttu-id="d7bcc-103">שורות הצעת מחיר המבוססות על פרוייקט</span><span class="sxs-lookup"><span data-stu-id="d7bcc-103">Project-based quote lines</span></span>

<span data-ttu-id="d7bcc-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="d7bcc-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="d7bcc-105">שורות הצעת מחיר מבוססות פרויקט נועדו לעזור להעריך את עבודת הפרויקט עבור התקשרות.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="d7bcc-106">המבנה של שורת הצעות מחיר מבוסס פרויקט מורחב להערכות פרויקט באמצעות המושגים הבאים:</span><span class="sxs-lookup"><span data-stu-id="d7bcc-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="d7bcc-107">שיטת חיוב</span><span class="sxs-lookup"><span data-stu-id="d7bcc-107">Billing Method</span></span>
- <span data-ttu-id="d7bcc-108">מיפוי פרויקטים</span><span class="sxs-lookup"><span data-stu-id="d7bcc-108">Project Mapping</span></span>
- <span data-ttu-id="d7bcc-109">סווגי עסקה כלולים</span><span class="sxs-lookup"><span data-stu-id="d7bcc-109">Included Transaction classes</span></span>
- <span data-ttu-id="d7bcc-110">מגבלת 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="d7bcc-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="d7bcc-111">הגדרת יכולת חיוב</span><span class="sxs-lookup"><span data-stu-id="d7bcc-111">Chargeability setup</span></span>
- <span data-ttu-id="d7bcc-112">הערכה באמצעות פרטי קו הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="d7bcc-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="d7bcc-113">לקוחות של שורת הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="d7bcc-113">Quote line Customers</span></span>

<span data-ttu-id="d7bcc-114">הטבלה הבאה מספקת מידע אודות השדות המופיעים בכרטיסיה **כללי** של שורת הצעת מחיר מבוססת פרויקט.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="d7bcc-115">שדות אלה מסייעים בהכנת הבסיס לביצוע הערכה מפורטת ויסודיות לעבודת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="d7bcc-116">**שדה**</span><span class="sxs-lookup"><span data-stu-id="d7bcc-116">**Field**</span></span> | <span data-ttu-id="d7bcc-117">**רלוונטיות, מטרה והכוונה**</span><span class="sxs-lookup"><span data-stu-id="d7bcc-117">**Relevance, purpose, and guidance**</span></span> | <span data-ttu-id="d7bcc-118">**השפעה במורד הזרם**</span><span class="sxs-lookup"><span data-stu-id="d7bcc-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="d7bcc-119">שם</span><span class="sxs-lookup"><span data-stu-id="d7bcc-119">Name</span></span> | <span data-ttu-id="d7bcc-120">שם שורת הצעת המחיר אשר אמורה לעזור לך לזהות את המרכיב המובדל של הצעת המחיר שעבורה מתבצעת הערכה.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-120">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="d7bcc-121">מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d7bcc-122">שיטת חיוב</span><span class="sxs-lookup"><span data-stu-id="d7bcc-122">Billing Method</span></span> | <span data-ttu-id="d7bcc-123">כשנוצרת הצעת מחיר מהזדמנות, ערך זה מועתק מהשדה התואם שבשורת הזדמנות.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="d7bcc-124">שדה זה כולל את שני המודלי החוזה העיקריים הנתמכים על ידי Dynamics 365 Project Operations:</span><span class="sxs-lookup"><span data-stu-id="d7bcc-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="d7bcc-125">- מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="d7bcc-125">- Fixed price</span></span></br><span data-ttu-id="d7bcc-126">- זמן וחומרים.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-126">- Time and material.</span></span>| <span data-ttu-id="d7bcc-127">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-127">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d7bcc-128">פרויקט</span><span class="sxs-lookup"><span data-stu-id="d7bcc-128">Project</span></span> | <span data-ttu-id="d7bcc-129">השתמש בשדה אופציונלי זה כדי לזהות את הפרויקט שישמש להגשת העבודה בהתקשרות זו.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="d7bcc-130">כאשר פרויקט ממופה לשורת הצעת מחיר, זה עוזר בהגדרת משימות הניתנות לחיוב וגם בכנסת הערכה מבוססת פרויקט לשורת הצעת המחיר, כפרטים בשורת הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="d7bcc-131">כאשר פרויקט אינו ממופה לשורת הצעת מחיר מבוססת פרויקט, יש ליצור את ההערכה באופן ידני על ידי יצירת כל פרט שבשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="d7bcc-132">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-132">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d7bcc-133">כלול זמן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-133">Include Time</span></span> | <span data-ttu-id="d7bcc-134">דגל **כן**/**לא** מציין אם עסקאות זמן או עלויות עבודה בפרויקט שנבחר ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-134">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="d7bcc-135">הערך **לא** מציין שעסקאות זמן או עלויות עבודה לא ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-135">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="d7bcc-136">הערך **כן** מציין שעסקאות זמן או עלויות עבודה ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-136">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="d7bcc-137">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-137">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d7bcc-138">כלול הוצאה</span><span class="sxs-lookup"><span data-stu-id="d7bcc-138">Include Expense</span></span> | <span data-ttu-id="d7bcc-139">דגל **כן**/**לא** מציין אם עלויות ההוצאות בפרויקט שנבחר ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-139">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="d7bcc-140">הערך **לא** מציין שעלויות ההוצאות לא ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-140">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="d7bcc-141">הערך **כן** מציין שעלויות ההוצאות ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-141">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="d7bcc-142">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-142">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d7bcc-143">כלול תשלום</span><span class="sxs-lookup"><span data-stu-id="d7bcc-143">Include Fee</span></span> | <span data-ttu-id="d7bcc-144">דגל **כן**/**לא** מציין אם עמלות על הפרויקט שנבחר ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-144">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="d7bcc-145">הערך **לא** מציין שהעמלות לא ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-145">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="d7bcc-146">הערך **כן** מציין שהעמלות ייכללו בהערכה בשורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-146">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="d7bcc-147">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-147">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d7bcc-148">הסכום של הצעת המחיר</span><span class="sxs-lookup"><span data-stu-id="d7bcc-148">Quoted Amount</span></span> | <span data-ttu-id="d7bcc-149">זהו סכום הצעת המחיר שינתן ללקוח עבור כל העבודה החזויה בשורת הצעת מחיר מבוססת פרויקט זו.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-149">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="d7bcc-150">בהצעת מחיר שנוצרת מהזדמנות, ערך זה מועתק מהשדה **תקציב הלקוח** שבשורת הזדמנות.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-150">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="d7bcc-151">כשבשורת צעת מחיר מבוססת הפרויקט יש פרטי שורה, שדה זה נעול לעריכה ומסוכם מהסכום שנמצא בפרטים בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-151">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="d7bcc-152">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-152">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d7bcc-153">מס משוער</span><span class="sxs-lookup"><span data-stu-id="d7bcc-153">Estimated Tax</span></span> | <span data-ttu-id="d7bcc-154">זהו שדה הניתן לעריכה שהמשתמש יכול להוסיף בו את סכום המס המשוער בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-154">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="d7bcc-155">כשבשורת צעת מחיר מבוססת הפרויקט יש פרטי שורה, שדה זה נעול לעריכה ומסוכם מסכום המס שנמצא בפרטים בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-155">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="d7bcc-156">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-156">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d7bcc-157">סכום הצעת המחיר, אחרי מס</span><span class="sxs-lookup"><span data-stu-id="d7bcc-157">Quoted Amount after Tax</span></span> | <span data-ttu-id="d7bcc-158">שדה זה הוא סכום שורת הצעת המחיר לאחר מס והוא לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-158">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="d7bcc-159">הסכום בשדה זה מחושב כ*סכום הצעת המחיר + מס*.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-159">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="d7bcc-160">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-160">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d7bcc-161">מגבלת 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="d7bcc-161">Not-to-exceed Limit</span></span> | <span data-ttu-id="d7bcc-162">שדה זה ניתן לעריכה והוא זמין רק בשורות הצעות מחיר מבוססות פרויקט עם שיטת חיוב של **זמן וחומרים**.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-162">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="d7bcc-163">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-163">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d7bcc-164">תקציב הלקוח</span><span class="sxs-lookup"><span data-stu-id="d7bcc-164">Customer Budget</span></span> | <span data-ttu-id="d7bcc-165">שדה זה ניתן לעריכה ומועתק מהשדה התואם בשורת ההזדמנות אם הצעת המחיר נוצרה מהזדמנות.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-165">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="d7bcc-166">ערך שדה זה מועתק לסעיף חוזה הפרויקט שנוצר משורת הצעת מחיר זו בעת הזכייה הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-166">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |

## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="d7bcc-167">כללי אימות עבור שדות בכרטיסיה 'כללי' של שורות הצעות מחיר מבוססות פרויקט</span><span class="sxs-lookup"><span data-stu-id="d7bcc-167">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="d7bcc-168">**כלל 1**: ניתן לכלול סיווג עסקאות מסוים רק בשורת הצעת מחיר מבוססת פרויקט אחת של הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-168">**Rule 1**: A certain transaction class on the selected project can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="d7bcc-169">**כלל 2**: אם להזדמנות יש הצעות מחיר מרובות, יכולות להיות שורות הצעות מחיר מהצעות מחיר שונות, אשר מתייחסות כולן לאותו פרויקט וכוללות את אותו סיווג עסקאות.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-169">**Rule 2**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="d7bcc-170">**כלל 3**: אם הצעות המחיר אינן שייכות לאותה הזדמנות, הן אינן יכולות לכלול את אותו פרויקט וסיווג עסקאות.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-170">**Rule 3**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="1" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="d7bcc-171">
                    <strong>הזדמנות</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7bcc-171">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="d7bcc-172">
                    <strong>הצעת מחיר</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7bcc-172">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="d7bcc-173">
                    <strong>שורת הצעת מחיר</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7bcc-173">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="d7bcc-174">
                    <strong>פרויקט</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7bcc-174">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="d7bcc-175">
                    <strong>כלול זמן</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7bcc-175">
                    <strong>Include time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="d7bcc-176">
                    <strong>כלול הוצאה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7bcc-176">
                    <strong>Include expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="d7bcc-177">
                    <strong>הכללה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7bcc-177">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="d7bcc-178">
                    <strong>עמלה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7bcc-178">
                    <strong>fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="d7bcc-179">
                    <strong>חוקי/לא חוקי</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7bcc-179">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="d7bcc-180">
                    <strong>סיבה</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d7bcc-180">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d7bcc-181">O1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-181">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d7bcc-182">ר1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-182">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-183">QL1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-183">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-184">P1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-184">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-185">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-185">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-186">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-186">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-187">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-187">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d7bcc-188">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="d7bcc-188">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d7bcc-189">הפרת כלל מס' 1.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-189">Violation of Rule #1.</span></span> <span data-ttu-id="d7bcc-190">זמן, הוצאות ועמלות בפרויקט P1 כלולים בשתי שורות הצעות המחיר QL1 ו-QL2.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-190">Time, Expense, and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d7bcc-191">O1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-191">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d7bcc-192">ר1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-192">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-193">QL2</span><span class="sxs-lookup"><span data-stu-id="d7bcc-193">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-194">P1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-194">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-195">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-195">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-196">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-196">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-197">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-197">Yes</span></span> </p>
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
<span data-ttu-id="d7bcc-198">O1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-198">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d7bcc-199">ר1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-199">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-200">QL1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-200">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-201">P1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-201">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-202">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-202">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-203">Yes</span><span class="sxs-lookup"><span data-stu-id="d7bcc-203">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-204">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-204">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d7bcc-205">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="d7bcc-205">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d7bcc-206">הפרת כלל מס' 1.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-206">Violation of Rule #1.</span></span> <span data-ttu-id="d7bcc-207">זמן ועמלות בפרויקט P1 כלולים בשתי שורות הצעות המחיר QL1 ו-QL2.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-207">Time and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d7bcc-208">O1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-208">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d7bcc-209">ר1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-209">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-210">QL2</span><span class="sxs-lookup"><span data-stu-id="d7bcc-210">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-211">P1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-211">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-212">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-212">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-213">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-213">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-214">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-214">Yes</span></span> </p>
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
<span data-ttu-id="d7bcc-215">O1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-215">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d7bcc-216">ר1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-216">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-217">QL1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-217">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-218">P1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-218">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-219">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-219">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-220">Yes</span><span class="sxs-lookup"><span data-stu-id="d7bcc-220">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-221">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-221">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d7bcc-222">חוקי</span><span class="sxs-lookup"><span data-stu-id="d7bcc-222">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                 <p>
<span data-ttu-id="d7bcc-223">זמן ועמלות בפרויקט P1 כלולים ב-QL1.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-223">Time and fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="d7bcc-224">הוצאות בפרויקט P1 כלולות ב-QL2.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-224">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="d7bcc-225">אין חפיפה במה שנכלל בכל שורת הצעת מחיר כך ושהיא תקפה.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-225">There is no overlap in what is being included on each quote line so it is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d7bcc-226">O1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-226">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d7bcc-227">ר1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-227">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-228">QL2</span><span class="sxs-lookup"><span data-stu-id="d7bcc-228">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-229">P1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-229">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-230">Yes</span><span class="sxs-lookup"><span data-stu-id="d7bcc-230">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-231">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-231">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-232">Yes</span><span class="sxs-lookup"><span data-stu-id="d7bcc-232">No</span></span> </p>
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
<span data-ttu-id="d7bcc-233">O1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-233">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d7bcc-234">ר1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-234">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-235">QL1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-235">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-236">P1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-236">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-237">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-237">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-238">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-238">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-239">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-239">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d7bcc-240">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="d7bcc-240">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d7bcc-241">הפרת כלל מס' 1 שלעיל</span><span class="sxs-lookup"><span data-stu-id="d7bcc-241">Violation of Rule #1 above</span></span> </p>
                <p>
<span data-ttu-id="d7bcc-242">ר1 כולל זמן, הוצאות ועמלות עבור הפרויקט P1 בכללותו.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-242">Q1 includes Time, Expenses, and Fees for the whole project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="d7bcc-243">QL2 כולל זמן, הוצאות ועמלות עבור כל הפרויקט P1 וחופף למה שנכלל ר1.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-243">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d7bcc-244">O1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-244">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d7bcc-245">ר1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-245">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-246">QL2</span><span class="sxs-lookup"><span data-stu-id="d7bcc-246">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-247">P1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-247">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-248">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-248">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-249">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-250">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-250">Yes</span></span> </p>
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
<span data-ttu-id="d7bcc-251">O1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d7bcc-252">ר1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-253">QL1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-254">P1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-254">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-255">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-255">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-256">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-257">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-257">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="d7bcc-258">חוקי</span><span class="sxs-lookup"><span data-stu-id="d7bcc-258">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d7bcc-259">בהתבסס על כלל מס' 2, Q1 ו-Q2 הן שתי הצעות מחיר באותה הזדמנות, כך ששתיהן יכולות לשמש להערכת אותם רכיבי פרויקט.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-259">Based on Rule #2, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d7bcc-260">O1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-260">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d7bcc-261">ר2</span><span class="sxs-lookup"><span data-stu-id="d7bcc-261">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-262">‏‏QL1 ב-Q2</span><span class="sxs-lookup"><span data-stu-id="d7bcc-262">QL1 on Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-263">P1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-263">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-264">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-264">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-265">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-266">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-266">Yes</span></span> </p>
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
<span data-ttu-id="d7bcc-267">O1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-267">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d7bcc-268">ר1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-268">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-269">QL1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-269">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-270">P1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-270">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-271">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-271">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-272">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-272">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-273">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-273">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="d7bcc-274">חוקי</span><span class="sxs-lookup"><span data-stu-id="d7bcc-274">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d7bcc-275">בהתבסס על כלל מס' 3, Q1 ו-Q2 הן שתי הצעות מחיר עבור הזדמנויות שונות, כך שהן אינן יכולות לשמש להערכת אותם הרכיבים של אותו הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="d7bcc-275">Based on Rule #3, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d7bcc-276">O2</span><span class="sxs-lookup"><span data-stu-id="d7bcc-276">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d7bcc-277">ר1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-277">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-278">QL1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-278">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-279">P1</span><span class="sxs-lookup"><span data-stu-id="d7bcc-279">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-280">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-280">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d7bcc-281">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-281">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d7bcc-282">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="d7bcc-282">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="d7bcc-283">לא חוקי</span><span class="sxs-lookup"><span data-stu-id="d7bcc-283">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>

