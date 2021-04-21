---
title: נהל מחירוני פרויקטים בהצעות מחיר של פרויקטים
description: נושא זה מספק מידע על עבודה עם מחירונים של פרויקטים בהצעות מחיר.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 912d2fad33ac02c3ba980da7eeb88eef5c331230
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858609"
---
# <a name="manage-project-price-lists-on-project-quotes"></a><span data-ttu-id="8ca9c-103">ניהול מחירוני פרוייקטים בהצעות מחיר</span><span class="sxs-lookup"><span data-stu-id="8ca9c-103">Manage project price lists on project quotes</span></span> 

<span data-ttu-id="8ca9c-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="8ca9c-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8ca9c-105">מחירונים של פרויקטים נועדו לתמוך במחירוני מכירות מרובים התקפים בתאריכים מסוימים.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-105">Project quotes are designed to support multiple date effective sales price lists.</span></span> <span data-ttu-id="8ca9c-106">עם Dynamics 365 Project Operations, נוספה ישות משויכת חדשה הנקראת **מחירונים לפרויקט**.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-106">With Dynamics 365 Project Operations, a new associated entity called **Project price lists** is added.</span></span> <span data-ttu-id="8ca9c-107">לישות זו קשר אחד לרבים להצעת מחיר של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-107">This entity has a 1-to-many relationship to a project quote.</span></span>

<span data-ttu-id="8ca9c-108">מחירוני הפרויקט משמשים לתמחור עסקאות זמן, חומר והוצאות בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-108">Project price lists are used to price time, material, and expense transactions on a project.</span></span> <span data-ttu-id="8ca9c-109">כאשר להצעת מחיר יש מחירון פרוייקט אחד או יותר, מחירונים אלה משמשים לתמחור זמן, חומר, אומדני הוצאות ונתונים בפועל בפרויקטים המשויכים להצעת מחיר דרך שורת הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-109">When a quote has one or more project price lists, these price lists are used to price time, material, expense estimates, and actuals on projects that are associated to the quote through the quote line.</span></span>

<span data-ttu-id="8ca9c-110">כאשר אין מחירוני פרויקט בהצעת מחיר של פרויקט, תקבל הודעת אזהרה.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-110">When there are no project price lists on a project quote, you will receive a warning message.</span></span> <span data-ttu-id="8ca9c-111">ההודעה מציינת שמכיוון שאין מחירוני פרויקט, העבודה וההוצאות המשוערות והאקטואליות של הפרויקט יתומחרו.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-111">The message states that because there are no project price lists, your estimated and actual project work and expenses will not be priced.</span></span> <span data-ttu-id="8ca9c-112">במקום זאת, יהיה להם מחיר של אפס (0) לערכי מכירה.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-112">Instead, they will have zero (0) price for sales values.</span></span>

## <a name="associate-or-disassociate-a-project-price-list-on-a-project-quote"></a><span data-ttu-id="8ca9c-113">שיוך או ביטול השיוך של מחירון הפרויקט בהצעת מחיר של פרויקט</span><span class="sxs-lookup"><span data-stu-id="8ca9c-113">Associate or disassociate a project price list on a project quote</span></span>

<span data-ttu-id="8ca9c-114">כדי ליצור או לבחור מחירון ספציפי להערכת עבודה והוצאות מבוססות פרויקט, בצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-114">To create or select a specific price list for estimating project-based work and expenses, complete the following steps.</span></span>

1. <span data-ttu-id="8ca9c-115">בהצעת המחיר, בחר את הכרטיסיה **מחיר הפרויקט** וברשת המשנה, בחר **+ הוסף מחירון פרויקט חדש**.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-115">On the quote, select the **Project Price** tab and in the subgrid, select **+ Add New Project Price List**.</span></span>
2. <span data-ttu-id="8ca9c-116">בדף היצירה מהירה בחר מחירון.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-116">On the Quick Create page, select a price list.</span></span> <span data-ttu-id="8ca9c-117">הרשימה הנפתחת מציגה את כל המחירונים שבהם ההקשר מוגדר ל **מכירות** והמטבע תואם את המטבע שבהצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-117">The drop-down list shows all price lists that have the context set to **Sales** and the currency matches the currency on the quote.</span></span>
4. <span data-ttu-id="8ca9c-118">הזן תיאור עבור שיוך מחירון הפרויקט ובחר **שמור וסגור**.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-118">Enter a description for the project price list association and select **Save and Close**.</span></span>

<span data-ttu-id="8ca9c-119">נוצר שיוך למחירון פרויקט.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-119">A project price list association is created.</span></span>

<span data-ttu-id="8ca9c-120">ניתן לחזור על תהליך זה אם עליך לשייך יותר ממחירון פרויקט אחד להצעת המחיר של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-120">You can repeat this process if you need to associate more than one project price list to the project quote.</span></span> <span data-ttu-id="8ca9c-121">יש ליצור מחירוני פרויקטים מרובים רק אם יש לך תאריכים תוקף שונים בכל אחד ממחירוני הפרויקט המשויכים.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-121">Only create multiple project price lists if you have different effective dates on each of the associated project price lists.</span></span>

> [!NOTE]
> <span data-ttu-id="8ca9c-122">Project Operations אינו תומך בחפיפת תוקף תאריכים של מחירוני הפרויקטים.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-122">Project Operations does't support overlapping date effectivity of the project price lists.</span></span> <span data-ttu-id="8ca9c-123">אם קיימות מספר מחירוני פרויקט עבור עסקה עם תאריך נותן, כברירת מחדל המחיר של אותה עסקה יוגדר לאפס (0).</span><span class="sxs-lookup"><span data-stu-id="8ca9c-123">If there are multiple project prices lists for a transaction with given date, the price on that transaction will be defaulted to zero (0).</span></span>
<span data-ttu-id="8ca9c-124">כדי להסיר שיוך של מחירון פרויקט, בחר את מחירון הפרויקט ואז בחר **מחק את מחירון הפרויקט של הצעת מחיר**.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-124">To remove a project price list association, select the project price list and then select **Delete Quote Project Price List**.</span></span> <span data-ttu-id="8ca9c-125">המחירון יוסר ממחירוני הפרויקט של הצעת המחיר, אך המחירון עצמו אינו נמחק.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-125">The price list is removed from the project price lists of the quote, but the price list itself is not deleted.</span></span> <span data-ttu-id="8ca9c-126">רק השיוך להצעת המחיר נמחק.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-126">Only the association to the quote is deleted.</span></span>

## <a name="set-up-default-project-price-lists-on-a-quote"></a><span data-ttu-id="8ca9c-127">הגדר מחירוני פרויקט ברירת מחדל בהצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="8ca9c-127">Set up default project price lists on a quote</span></span>

<span data-ttu-id="8ca9c-128">ניתן להגדיר מחירוני פרויקטים כברירת מחדל בהצעת מחיר של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-128">Project price lists can be set up to default on a project quote.</span></span> <span data-ttu-id="8ca9c-129">הגדרה זו מבטיחה שכל הצעות המחיר בארגון שלך תמיד מתחילות במחירון סטנדרטי לאותה לתקופת המחיר.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-129">This setup ensures that all quotes in your organization always start with a standard price list for that price period.</span></span>

### <a name="set-up-organizational-default-for-project-price-lists"></a><span data-ttu-id="8ca9c-130">הגדר ברירת מחדל ארגוני עבור מחירוני פרויקט</span><span class="sxs-lookup"><span data-stu-id="8ca9c-130">Set up organizational default for project price lists</span></span>

1. <span data-ttu-id="8ca9c-131">עבור אל **הגדרות** > **כללי** > **פרמטרים**.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-131">Go to **Settings** > **General** > **Parameters**.</span></span>
2. <span data-ttu-id="8ca9c-132">בדף הרשימה **פרמטרים פעילים**, אתר את הרשומה ולחץ פעמיים כדי לפתוח אותה.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-132">On the **Active Parameters** list page, locate the record and double-click to open it.</span></span> 
3. <span data-ttu-id="8ca9c-133">בדף **פרמטרים** בחר את הכרטיסיה **מחירון**. תוכל לראות את רשימת המחירונים המוגדרים כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-133">On the **Parameters** page, select the **Price List** tab. You can see the list of default price lists is shown.</span></span> <span data-ttu-id="8ca9c-134">זוהי רשימת מחירי עלות סטנדרטיים ומחירוני מכירה.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-134">This is a list standard cost and sales price lists.</span></span> <span data-ttu-id="8ca9c-135">כאשר יש מחירון מכירות המשויך כאן לכל מטבע שבו אתה מוכר, הדבר יבטיח כי מחירון מכירה זה יוגדר כברירת מחדל בכל הצעת מחיר שתיצור עבור לקוחות המבצעים עסקאות במטבע זה.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-135">Having a sales price list associated here for every currency that you sell in, will ensure that this sales price list is defaulted on any quote that you create for customers that transact in this currency.</span></span>

### <a name="set-up-customer-specific-project-price-lists"></a><span data-ttu-id="8ca9c-136">הגדר מחירוני פרויקט ספציפיים ללקוח</span><span class="sxs-lookup"><span data-stu-id="8ca9c-136">Set up customer-specific project price lists</span></span>

<span data-ttu-id="8ca9c-137">ניתן להגדיר מחירוני פרויקט ספציפיים ללקוח גם כאשר סיכמתם במשא ומתן על הסכם תמחור ראשי עם הלקוחות שלכם.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-137">Customer-specific project price lists can also be set up when you have negotiated a master pricing agreement with your customers.</span></span>

<span data-ttu-id="8ca9c-138">כדי להגדיר מחירון פרויקט ספציפי ללקוח, בצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-138">To set up a customer-specific project price list, complete the following steps.</span></span>

1. <span data-ttu-id="8ca9c-139">באזור **מכירות** , בחר **לקוחות**.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-139">In the **Sales** area, select **Customers**.</span></span>
2. <span data-ttu-id="8ca9c-140">ברשימת תיקי הלקוח הפעילים שלך, בחר ופתח את הרשומה של הלקוח שעבורו יש לך מחירון מיוחד.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-140">In the list of your active accounts, select and open the customer record that you have special price list for.</span></span>
3. <span data-ttu-id="8ca9c-141">על הכרטיסיסה **מחירוני לפרויקט**, ניתן ליצור שיוך מחירון חדש כדי לקבל את מחירון הפרויקט הספציפי של לקוח זה.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-141">On the **Project Price Lists** tab, you can create a new price list association to have the project price list that is specific to this customer.</span></span>

## <a name="create-custom-pricing-on-a-project-quote"></a><span data-ttu-id="8ca9c-142">יצירת תמחור מותאם אישית בהצעת מחיר של פרויקט</span><span class="sxs-lookup"><span data-stu-id="8ca9c-142">Create custom pricing on a project quote</span></span>

<span data-ttu-id="8ca9c-143">לאחר הגדרת מחירוני פרויקט ברירת מחדל שהם ספציפיים לארגונים וללקוחות, הצעות המחיר להפרויקט ייווצרו אוטומטית עם שיוכים אלו של מחירוני פרויקט.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-143">After you have organizational and customer-specific default project price lists, your project quotes will automatically be created with these project price list associations.</span></span> <span data-ttu-id="8ca9c-144">עם זאת, במקרים מסוימים, ייתכן שיהיה עליך ליצור תמחור מותאם אישית להצעת מחיר ספציפית של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-144">However, in certain cases, you may need to create custom pricing for a specific project quote.</span></span> 

1. <span data-ttu-id="8ca9c-145">ב **הצעת מחיר של פרויקט**, בכרטיסיה **מחירון הפרויקט**, ודא ברשת המשנה שלא נבחרה רשומת מחירון ספציפית.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-145">On the **Project Quote**, on the **Project Price List** tab, verify in the subgrid that no specific price list record is selected.</span></span>
2. <span data-ttu-id="8ca9c-146">בחר **צור תמחור מותאם אישית**.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-146">Select **Create Custom Pricing**.</span></span> <span data-ttu-id="8ca9c-147">פעולה זו תיצור עותקים של כל המחירונים הסטנדרטיים המשויכים כרגע להצעת המחיר ותשייך עותקים אלה אל הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-147">This will make copies of all the standard price lists currently associated to the quote and associate these copies to the quote.</span></span> <span data-ttu-id="8ca9c-148">השיוכים הקיימות למחירונים הסטנדרטיים יוסרו.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-148">The existing associations to standard price lists will be removed.</span></span> <span data-ttu-id="8ca9c-149">לאחר מכן, איש המכירות יכול להתחיל לערוך את המחירים בהעתקים אלה.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-149">The salesperson can then begin making edits to prices on these copies.</span></span> <span data-ttu-id="8ca9c-150">מחירים אלה ששונו, יחולו רק על הצעת המחיר זו לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8ca9c-150">These changed prices will be applicable to this project quote only.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
