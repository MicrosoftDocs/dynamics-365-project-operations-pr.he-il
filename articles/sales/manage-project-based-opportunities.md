---
title: ניהול הזדמנויות מבוססות פרויקט
description: נושא זה מספק מידע על אופן העבודה עם הזדמנויות שקשורות לפרויקטים.
author: rumant
manager: Annbe
ms.date: 10/21/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: c5a8bfea5540432a62d7075443cf237571bfa4de
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4118474"
---
# <a name="manage-project-based-opportunities"></a><span data-ttu-id="14a26-103">ניהול הזדמנויות מבוססות פרויקט</span><span class="sxs-lookup"><span data-stu-id="14a26-103">Manage project-based opportunities</span></span>

<span data-ttu-id="14a26-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="14a26-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="14a26-105">חברות מבוססות פרויקטים בדרך כלל מפעילות את המשלוח שלהן ברחבי מדינות ואזורים גיאוגרפיים רבים.</span><span class="sxs-lookup"><span data-stu-id="14a26-105">Project-based companies typically have their operations for delivery spread across multiple countries and geographies.</span></span> <span data-ttu-id="14a26-106">עלות ביצוע הפרויקט ומסירתו עשויה להשתנות בהתאם לאיזור הגיאוגרפי או למחלקה שמנהלת את המסירה.</span><span class="sxs-lookup"><span data-stu-id="14a26-106">The cost of the project execution and delivery can vary  based on which geography or division manages the delivery.</span></span> <span data-ttu-id="14a26-107">יכולה להיות לכך השפעה גם על שולי הרווח של העסקה.</span><span class="sxs-lookup"><span data-stu-id="14a26-107">In turn, this can impact the margins of the deal.</span></span> <span data-ttu-id="14a26-108">אספקת שירותים מבוססי פרויקטים כרוכה בדרך כלל בכמויות גדולות של זמן משאבי אנוש, בהוצאות ניכרות על נסיעות, בעלויות חומר והוצאות אחרות.</span><span class="sxs-lookup"><span data-stu-id="14a26-108">Delivery of project-based services typically involves large quantities of human resource time, considerable expenses for travel, material costs, and other expenses.</span></span>

<span data-ttu-id="14a26-109">הזדמנויות מבוססות-פרויקט ב-Dynamics 365 Project Operations תוכננו עם הרחבות ב- Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="14a26-109">Project-based opportunities in Dynamics 365 Project Operations are designed with extensions to Dynamics 365 Sales.</span></span> <span data-ttu-id="14a26-110">נושא זה מספק פרטים על התחומים השונים וההיגיון העסקי הכלולים בפונקציונליות הנוספת הנדרשת על ידי חברות מבוססות פרויקטים לניהול הזדמנויות מבוססות פרויקטים.</span><span class="sxs-lookup"><span data-stu-id="14a26-110">The topic provides details about the different fields and business logic included in the additional functionality that is required by project-based companies to manage project-based opportunities.</span></span>

## <a name="view-all-project-based-opportunities"></a><span data-ttu-id="14a26-111">ראה את כל ההזדמנויות המבוססות על פרויקטים</span><span class="sxs-lookup"><span data-stu-id="14a26-111">View all project-based opportunities</span></span>

<span data-ttu-id="14a26-112">ניתן לראות רשימה של כל ההזדמנויות המבוססות על פרויקטים בדף הרשימה **הזדמנות**.</span><span class="sxs-lookup"><span data-stu-id="14a26-112">A list of all the project-based opportunities can be seen from the **Opportunity** list page.</span></span> 

1. <span data-ttu-id="14a26-113">עבור אל **מכירות** > **הזדמנויות**.</span><span class="sxs-lookup"><span data-stu-id="14a26-113">Go to **Sales** > **Opportunities**.</span></span>
2. <span data-ttu-id="14a26-114">השתמש באפשרות **מחליף תצוגות** כדי לבחור תצוגות מסוננות אחרות של הזדמנויות.</span><span class="sxs-lookup"><span data-stu-id="14a26-114">Use the **View switcher** to select other filtered views of the opportunities.</span></span> <span data-ttu-id="14a26-115">אתה יכול ליצור תצוגות משלך עם קריטריונים מותאמים אישית לסינון כדי להגדיר תצוגות ואפשרויות ניווט אלה.</span><span class="sxs-lookup"><span data-stu-id="14a26-115">You can create your own views with custom filter criteria to configure these views and navigation options.</span></span>

<span data-ttu-id="14a26-116">ניתן ליצור או למחוק הזדמנויות לפרויקט מדף רשימה זו או מדף הפרטים.</span><span class="sxs-lookup"><span data-stu-id="14a26-116">Project Opportunities can be created or deleted from this list page or the detail page.</span></span>

## <a name="business-process-flow-for-project-based-deals"></a><span data-ttu-id="14a26-117">זרימת תהליך עסקי לעסקאות מבוססות פרויקטים</span><span class="sxs-lookup"><span data-stu-id="14a26-117">Business process flow for project-based deals</span></span>

<span data-ttu-id="14a26-118">זרימת התהליכים העסקיים הבאים נתמכים עבור עסקאות מבוססות פרויקטים ב-Project Operations:</span><span class="sxs-lookup"><span data-stu-id="14a26-118">The following business process flows are supported for project-based deals in Project Operations:</span></span>

- <span data-ttu-id="14a26-119">תהליך עסקי של הפניה להזדמנות</span><span class="sxs-lookup"><span data-stu-id="14a26-119">Lead to Opportunity business process</span></span>
- <span data-ttu-id="14a26-120">תהליך מכירות של הזדמנות</span><span class="sxs-lookup"><span data-stu-id="14a26-120">Opportunity sales process</span></span>

### <a name="lead-to-opportunity-business-process"></a><span data-ttu-id="14a26-121">תהליך עסקי של הפניה להזדמנות</span><span class="sxs-lookup"><span data-stu-id="14a26-121">Lead to opportunity business process</span></span> 
<span data-ttu-id="14a26-122">התהליך העסקי הפניה להזדמנות תומך בשלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="14a26-122">The lead to opportunity business process supports the following stages:</span></span>

| <span data-ttu-id="14a26-123">שלב</span><span class="sxs-lookup"><span data-stu-id="14a26-123">Stage</span></span> | <span data-ttu-id="14a26-124">ישות ממופה</span><span class="sxs-lookup"><span data-stu-id="14a26-124">Mapped entity</span></span> | <span data-ttu-id="14a26-125">פונקציונליות</span><span class="sxs-lookup"><span data-stu-id="14a26-125">Functionality</span></span> |
| --- | --- | --- |
| <span data-ttu-id="14a26-126">אישור</span><span class="sxs-lookup"><span data-stu-id="14a26-126">Qualify</span></span> | <span data-ttu-id="14a26-127">הפניה</span><span class="sxs-lookup"><span data-stu-id="14a26-127">Lead</span></span> | <span data-ttu-id="14a26-128">אישור של הפניה ליצירת תיק לקוח, לאיש קשר והזדמנות.</span><span class="sxs-lookup"><span data-stu-id="14a26-128">Qualify the lead to create an account, contact, and an opportunity.</span></span> |
| <span data-ttu-id="14a26-129">פיתוח</span><span class="sxs-lookup"><span data-stu-id="14a26-129">Develop</span></span> | <span data-ttu-id="14a26-130">הזדמנות</span><span class="sxs-lookup"><span data-stu-id="14a26-130">Opportunity</span></span> | <span data-ttu-id="14a26-131">פתח את ההזדמנות להוספת מידע נוסף על העבודה המעורבת, בעלי עניין מרכזיים ותחרות.</span><span class="sxs-lookup"><span data-stu-id="14a26-131">Develop the opportunity to add more information on the work involved, key stakeholders, and competition.</span></span> |
| <span data-ttu-id="14a26-132">הצעה</span><span class="sxs-lookup"><span data-stu-id="14a26-132">Propose</span></span> | <span data-ttu-id="14a26-133">הזדמנות</span><span class="sxs-lookup"><span data-stu-id="14a26-133">Opportunity</span></span> | <span data-ttu-id="14a26-134">פתח את ההצעה וקבל אישור מצוות הסיקרה הפנימית.</span><span class="sxs-lookup"><span data-stu-id="14a26-134">Develop the proposal and get approval from the internal review team.</span></span> |
| <span data-ttu-id="14a26-135">סגורה</span><span class="sxs-lookup"><span data-stu-id="14a26-135">Close</span></span> | <span data-ttu-id="14a26-136">הזדמנות</span><span class="sxs-lookup"><span data-stu-id="14a26-136">Opportunity</span></span> | <span data-ttu-id="14a26-137">זכה בהזדמנות כדי לסגור את העסקה.</span><span class="sxs-lookup"><span data-stu-id="14a26-137">Win the opportunity to close the deal.</span></span> |

### <a name="opportunity-sales-process"></a><span data-ttu-id="14a26-138">תהליך מכירות של הזדמנות</span><span class="sxs-lookup"><span data-stu-id="14a26-138">Opportunity sales process</span></span>
<span data-ttu-id="14a26-139">תהליך המכירה של הזדמנות ב- Project Operations הוא הרחבה לזרם העסקי של תהליך המכירה של הזדמנות ביישום המכירות.</span><span class="sxs-lookup"><span data-stu-id="14a26-139">The Opportunity sales process in Project Operations is an extension to the Opportunity sales process business flow in the Sales application.</span></span> <span data-ttu-id="14a26-140">תהליך עסקי זה נכלל במוצר לתמיכה בשלבים הבאים בהזדמנות המבוססת על פרויקט.</span><span class="sxs-lookup"><span data-stu-id="14a26-140">This business process is designed out-of-the-box to support the following stages in a project-based opportunity.</span></span>

| <span data-ttu-id="14a26-141">שלב</span><span class="sxs-lookup"><span data-stu-id="14a26-141">Stage</span></span> | <span data-ttu-id="14a26-142">ישות ממופה</span><span class="sxs-lookup"><span data-stu-id="14a26-142">Mapped entity</span></span> | <span data-ttu-id="14a26-143">פונקציונליות</span><span class="sxs-lookup"><span data-stu-id="14a26-143">Functionality</span></span> |
| --- | --- | --- |
| <span data-ttu-id="14a26-144">אישור</span><span class="sxs-lookup"><span data-stu-id="14a26-144">Qualify</span></span> | <span data-ttu-id="14a26-145">הזדמנות</span><span class="sxs-lookup"><span data-stu-id="14a26-145">Opportunity</span></span> | <span data-ttu-id="14a26-146">אישור של הפניה ליצירת תיק לקוח, לאיש קשר והזדמנות.</span><span class="sxs-lookup"><span data-stu-id="14a26-146">Qualify the lead to create an account, contact, and an opportunity.</span></span> |
| <span data-ttu-id="14a26-147">הצעה</span><span class="sxs-lookup"><span data-stu-id="14a26-147">Propose</span></span> | <span data-ttu-id="14a26-148">הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="14a26-148">Quote</span></span> | <span data-ttu-id="14a26-149">פתח את ההצעה באמצעות הצעות מחיר בפרויקט וקבל אישור מצוות הסקירה הפנימית.</span><span class="sxs-lookup"><span data-stu-id="14a26-149">Develop the proposal using project quotes and get approval from the internal review team.</span></span> |
| <span data-ttu-id="14a26-150">חוזה</span><span class="sxs-lookup"><span data-stu-id="14a26-150">Contract</span></span> | <span data-ttu-id="14a26-151">חוזה פרויקט</span><span class="sxs-lookup"><span data-stu-id="14a26-151">Project Contract</span></span> | <span data-ttu-id="14a26-152">זכה בהצעת המחיר כדי ליצור את החוזה ולהתחיל בביצוע ומסירה בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="14a26-152">Win the quote to create the contract and begin execution and delivery on the project.</span></span> |
| <span data-ttu-id="14a26-153">סגורה</span><span class="sxs-lookup"><span data-stu-id="14a26-153">Close</span></span> | <span data-ttu-id="14a26-154">חוזה פרויקט</span><span class="sxs-lookup"><span data-stu-id="14a26-154">Project Contract</span></span> | <span data-ttu-id="14a26-155">סיים את העבודה בהצלחה וסגור את חוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="14a26-155">Finish the work successfully and close the project contract.</span></span> |

> [!NOTE]
> <span data-ttu-id="14a26-156">אם העסקה מבוססת הפרויקט התחילה עם הפניה, התהליך העסקי מהפניה להזדמנות מקבל עדיפות.</span><span class="sxs-lookup"><span data-stu-id="14a26-156">If your project-based deal started with a Lead, the Lead to Opportunity business process takes precedence.</span></span>
>
> <span data-ttu-id="14a26-157">אם העסקה מבוססת הפרויקט התחילה עם הזדמנות, התהליך העסקי מהזדמנות למכירה מקבל עדיפות.</span><span class="sxs-lookup"><span data-stu-id="14a26-157">If your project-based deal started with an Opportunity, the Opportunity sales process takes precedence.</span></span>

<span data-ttu-id="14a26-158">באפשרותך לערוך את זרימת התהליך העסקי של המוצר או ליצור זרימת תהליך עסקי משלך כדי לעקוב אחר תהליך המכירה לפי הצורך.</span><span class="sxs-lookup"><span data-stu-id="14a26-158">You can edit the product business process flow or create your own business process flows to track your sales process as needed.</span></span> <span data-ttu-id="14a26-159">למידע נוסף על זרימת התהליך העסקי, ראה [‏‫מבט כולל על זרימות תהליכים עסקיים‬](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/business-process-flows-overview).</span><span class="sxs-lookup"><span data-stu-id="14a26-159">For more information about the business process flow, see [Business process flows overview](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/business-process-flows-overview).</span></span>
