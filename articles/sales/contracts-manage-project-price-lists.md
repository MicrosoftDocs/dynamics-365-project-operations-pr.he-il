---
title: ניהול מחירוני פרוייקט בחוזי פרוייקט
description: נושא זה מספק מידע על ניהול מחירוני פרויקט בחוזי פרויקט.
author: rumant
manager: Annbe
ms.date: 10/27/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 2cfac6eda64d1d8e578115bba07942a7d786328f
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5278599"
---
# <a name="manage-project-price-lists-on-project-contracts"></a><span data-ttu-id="76e6d-103">ניהול מחירוני פרוייקט בחוזי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="76e6d-103">Manage project price lists on project contracts</span></span>

<span data-ttu-id="76e6d-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="76e6d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="76e6d-105">חוזי פרויקט ב- Dynamics 365 Project Operations נועדו לתמוך במחירוני מכירות מרובים עם תאריכי תוקף בחוזה.</span><span class="sxs-lookup"><span data-stu-id="76e6d-105">Project contracts in Dynamics 365 Project Operations are designed to support multiple date effective sales price lists on a contract.</span></span> <span data-ttu-id="76e6d-106">ב-Project Operations, יש ישות משויכת חדשה הנקראת **מחירוני פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="76e6d-106">In Project Operations, there is a new associated entity called **Project Price Lists**.</span></span> <span data-ttu-id="76e6d-107">לישות זו יש קשר גומלין של אחד לרבים לחוזה פרויקט.</span><span class="sxs-lookup"><span data-stu-id="76e6d-107">This entity has a one-to-many relationship to a project contract.</span></span>

<span data-ttu-id="76e6d-108">מחירוני הפרויקט משמשים לתמחור עסקאות זמן והוצאות בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="76e6d-108">Project price lists are used to price time and expense transactions on a project.</span></span> <span data-ttu-id="76e6d-109">כאשר בחוזה יש מחירון פרוייקט אחד או יותר, מחירונים אלה משמשים לתמחור הערכות זמן והוצאות ונתונים בפועל בפרויקטים המשויכים לחוזה דרך סעיף החוזה.</span><span class="sxs-lookup"><span data-stu-id="76e6d-109">When a contract has one or more project price lists, these price lists are used to price for time and expense estimates and actuals on projects that are associated to the contract through the contract line.</span></span>

<span data-ttu-id="76e6d-110">כאשר אין מחירוני פרויקט בחוזה הפרויקט, תוצג הודעת אזהרה שאין מחירוני פרויקטים ושההערכות שלך, עבודת הפרויקט בפועל וההוצאות לא יתומחרו.</span><span class="sxs-lookup"><span data-stu-id="76e6d-110">When there are no project price lists on a project contract, you will see a warning message that there are no project price lists and your estimates, actual project work, and expenses will not be priced.</span></span> <span data-ttu-id="76e6d-111">לא יהיה מחיר לערכי המכירות.</span><span class="sxs-lookup"><span data-stu-id="76e6d-111">There will be no price for sales values.</span></span>

## <a name="associate-or-unassociate-a-project-price-list-on-a-project-contract"></a><span data-ttu-id="76e6d-112">שיוך או ביטול שיוך של מחירון פרוייקט בחוזה הפרויקט</span><span class="sxs-lookup"><span data-stu-id="76e6d-112">Associate or unassociate a project price list on a project contract</span></span>

### <a name="create-or-associate-a-specific-price-list-for-estimating-project-based-work-and-expenses"></a><span data-ttu-id="76e6d-113">ליצור או לשייך מחירון ספציפי להערכת עבודה והוצאות מבוססות פרויקט</span><span class="sxs-lookup"><span data-stu-id="76e6d-113">Create or associate a specific price list for estimating project-based work and expenses</span></span>

1. <span data-ttu-id="76e6d-114">בחוזה הפרויקט בחר בכרטיסיה **מחירוני הפרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="76e6d-114">On the project contract, select the **Project Price Lists** tab.</span></span>
2. <span data-ttu-id="76e6d-115">ברשת המשנה בחר **+ הוסף מחירון פרוייקט חדש**.</span><span class="sxs-lookup"><span data-stu-id="76e6d-115">In the subgrid, select **+ Add New Project Price List**.</span></span>
3. <span data-ttu-id="76e6d-116">במחוון **יצירה מהירה**, בחר מחירון.</span><span class="sxs-lookup"><span data-stu-id="76e6d-116">On the **Quick Create** slider, select a price list.</span></span> 

  <span data-ttu-id="76e6d-117">הרשימה הנפתחת מציגה את כל המחירונים שההקשר שלהם מוגדר ל **מכירות**, כאשר המטבע במחירון תואם את המטבע בחוזה.</span><span class="sxs-lookup"><span data-stu-id="76e6d-117">The drop-down list shows all price lists that have the context set to **Sales**, where the currency on the price list matches the currency on the contract.</span></span>
  
4. <span data-ttu-id="76e6d-118">הזן תיאור עבור שיוך מחירון הפרויקט, בחר **שמור** ואז סגור את המחוון **יצירה מהירה**.</span><span class="sxs-lookup"><span data-stu-id="76e6d-118">Enter a description for the project price list association, select **Save**, and then close the **Quick Create** slider.</span></span>

   <span data-ttu-id="76e6d-119">נוצר שיוך למחירון פרויקט.</span><span class="sxs-lookup"><span data-stu-id="76e6d-119">A project price list association is created.</span></span>
   
5. <span data-ttu-id="76e6d-120">חזור על שלבים 1-4 כדי לשייך יותר ממחירון פרוייקט אחד לחוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="76e6d-120">Repeat steps 1-4 to associate more than one project price list to the project contract.</span></span> <span data-ttu-id="76e6d-121">צור מחירוני פרוייקט מרובים רק אם לכל אחד ממחירוני הפרויקט המשויכים תאריכי תוקף שונים.</span><span class="sxs-lookup"><span data-stu-id="76e6d-121">Only create multiple project price lists if you have different date effectivity on each of the associated project price list.</span></span>

> [!NOTE]
> <span data-ttu-id="76e6d-122">Project Operations אינו תומך בחפיפה של תאריכי תוקף של מחירוני הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="76e6d-122">Project Operations doesn't support overlapping the date effectivity of the project price lists.</span></span> <span data-ttu-id="76e6d-123">אם קיימים מחירוני פרוייקט מרובים עובר עסקה עם תאריך נתון, המחיר של אותה עסקה יוגדר כברירת מחדל לאפס.</span><span class="sxs-lookup"><span data-stu-id="76e6d-123">If there are multiple project prices lists for a transaction with a given date, the price on that transaction will be defaulted to zero.</span></span>

### <a name="remove-a-project-price-list-association"></a><span data-ttu-id="76e6d-124">הסרת שיוך של מחירון פרוייקט</span><span class="sxs-lookup"><span data-stu-id="76e6d-124">Remove a project price list association</span></span>

- <span data-ttu-id="76e6d-125">בחר את מחירון הפרויקט ואז בחר **מחק את מחירון פרויקט החוזה** ברשת המשנה.</span><span class="sxs-lookup"><span data-stu-id="76e6d-125">Select the project price list, and then select **Delete Contract Project Price List** on the subgrid.</span></span> 

  <span data-ttu-id="76e6d-126">המחירון מוסר ממחירוני הפרויקט בחוזה.</span><span class="sxs-lookup"><span data-stu-id="76e6d-126">The price list is removed from the project price lists on the contract.</span></span> <span data-ttu-id="76e6d-127">המחירון עצמו לא יימחק.</span><span class="sxs-lookup"><span data-stu-id="76e6d-127">The price list itself will not be deleted.</span></span> <span data-ttu-id="76e6d-128">רק השיוך לחוזה יימחק.</span><span class="sxs-lookup"><span data-stu-id="76e6d-128">Only the association to the contract will be deleted.</span></span>

## <a name="set-up-automatic-defaulting-of-project-price-lists-on-a-contract"></a><span data-ttu-id="76e6d-129">הגדר ברירת מחדל אוטומטית של מחירוני הפרויקט בחוזה</span><span class="sxs-lookup"><span data-stu-id="76e6d-129">Set up automatic defaulting of project price lists on a contract</span></span>

<span data-ttu-id="76e6d-130">ניתן להגדיר מחירון פרויקט כמחירון ברירת המחדל בחוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="76e6d-130">A project price list can be set up as the default list on a project contract.</span></span> <span data-ttu-id="76e6d-131">הגדרה זו יכולה לעזור להבטיח כי כל החוזים בארגון שלך יתחילו תמיד עם מחירון סטנדרטי לאותה תקופת מחירים.</span><span class="sxs-lookup"><span data-stu-id="76e6d-131">This setup can help ensure that all contracts in your organization always start with a standard price list for that price period.</span></span>

### <a name="set-up-the-organizational-default-for-project-price-lists"></a><span data-ttu-id="76e6d-132">הגדרת ברירת המחדל הארגונית למחירוני פרוייקט</span><span class="sxs-lookup"><span data-stu-id="76e6d-132">Set up the organizational default for project price lists</span></span>

1. <span data-ttu-id="76e6d-133">עבור אל **הגדרות** > **כללי** ואז בחר **פרמטרים**.</span><span class="sxs-lookup"><span data-stu-id="76e6d-133">Go to **Settings** > **General**, and then select **Parameters**.</span></span>
2. <span data-ttu-id="76e6d-134">בדף הרשימה **פרמטרים פעילים**, בחר ולחץ פעמיים על הרשומה כדי לפתוח אותה.</span><span class="sxs-lookup"><span data-stu-id="76e6d-134">In the **Active Parameters** list page, select and double-click the record to open it.</span></span> <span data-ttu-id="76e6d-135">בזמן הלחיצה כפולה, ודא שאינך לוחץ על ערך שדה שהוא היפר-קישור.</span><span class="sxs-lookup"><span data-stu-id="76e6d-135">While double–clicking, make sure that you are not clicking on a field value that is hyperlink.</span></span> 
3. <span data-ttu-id="76e6d-136">בדף **פרמטרים פעילים** בחר את הכרטיסיה **מחירונים**. רשת משנה מציגה רשימה של מחירוני ברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="76e6d-136">On the **Active Parameters** page, select the **Price List** tab. A subgrid shows a list of default price lists.</span></span> <span data-ttu-id="76e6d-137">זוהי רשימה של מחירוני עלות ומכירה סטנדרטיים.</span><span class="sxs-lookup"><span data-stu-id="76e6d-137">This is a list of standard cost and sales price lists.</span></span> <span data-ttu-id="76e6d-138">קיומו של מחירון **מכירות** המשויך לכל מטבע שבו אתה מוכר, מבטיח שמחירון המכירה תשמש כברירת המחדל בכל חוזה שאתה יוצר עבור לקוחות המבצעים עסקאות במטבע זה.</span><span class="sxs-lookup"><span data-stu-id="76e6d-138">Having a **Sales** price list associated here for every currency that you sell in ensures that the sales price list is the default on any contract that you create for customers that transact in this currency.</span></span>

### <a name="set-up-a-customer-specific-project-price-list"></a><span data-ttu-id="76e6d-139">הגדר מחירון פרוייקט ספציפי ללקוח</span><span class="sxs-lookup"><span data-stu-id="76e6d-139">Set up a customer-specific project price list</span></span>

<span data-ttu-id="76e6d-140">ניתן גם להגדיר מחירוני פרויקט ספציפיים ללקוח במקרים שבהם הסכמת עם לקוחותיך על הסכם תמחור ראשי.</span><span class="sxs-lookup"><span data-stu-id="76e6d-140">You can also set up customer–specific project price lists when you have negotiated a master pricing agreement with your customers.</span></span>

1. <span data-ttu-id="76e6d-141">עבור אל **מכירות** > **לקוחות**.</span><span class="sxs-lookup"><span data-stu-id="76e6d-141">Go to **Sales** > **Customers**.</span></span>
2. <span data-ttu-id="76e6d-142">מרשימת תיקי הלקוח הפעילים, בחר את הלקוח אשר עבורו יש מחירון מיוחד.</span><span class="sxs-lookup"><span data-stu-id="76e6d-142">From the list of active accounts, select the customer for whom have special price list.</span></span>
3. <span data-ttu-id="76e6d-143">בחר את רשומת הלקוח כדי לפתוח אותה ואז בחר את הכרטיסיה **מחירוני פרוייקט**. רשת משנה מציגה רשימה של מחירוני פרויקט שהם ספציפיים ללקוח זה.</span><span class="sxs-lookup"><span data-stu-id="76e6d-143">Select the customer record to open it and then select the **Project Price Lists** tab. A subgrid shows a list of project price lists specific to this customer.</span></span> 
4. <span data-ttu-id="76e6d-144">צור כאן שיוך מחירון חדש כדי ליצור מחירון פרויקט ספציפי ללקוח זה.</span><span class="sxs-lookup"><span data-stu-id="76e6d-144">Create a new price list association here to have project price list specific to this customer.</span></span>

## <a name="custom-pricing-on-a-project-contract"></a><span data-ttu-id="76e6d-145">תמחור מותאם אישית בחוזה פרויקט</span><span class="sxs-lookup"><span data-stu-id="76e6d-145">Custom pricing on a project contract</span></span>

<span data-ttu-id="76e6d-146">לאחר שיש לך מחירוני פרויקט ארגוניים המוגדרים כברירת מחדל כספציפיים ללקוח, חוזי הפרויקט שלך ייווצרו עם שיוך אוטומטי של מחירוני פרוייקט האלה.</span><span class="sxs-lookup"><span data-stu-id="76e6d-146">After you have organizational and customer-specific default project price lists, your project contracts will be created with these project price list associations automatically.</span></span> <span data-ttu-id="76e6d-147">עם זאת, מחירוני הפרויקט בחוזה פרויקט מועתקים תמיד בצריוף תאריך ושם החוזה.</span><span class="sxs-lookup"><span data-stu-id="76e6d-147">However, project price lists on a project contract are always copied with the date and contract name appended to them.</span></span> <span data-ttu-id="76e6d-148">מנהלי החשבונות והפרויקטים יכולים להתחיל לערוך את המחירים בעותקים אלה.</span><span class="sxs-lookup"><span data-stu-id="76e6d-148">The account and project managers can then begin making edits to prices on these copies.</span></span> <span data-ttu-id="76e6d-149">מחירים אלה ששונו יחולו על חוזה פרויקט זה בלבד.</span><span class="sxs-lookup"><span data-stu-id="76e6d-149">These changed prices will be applicable to this project contract only.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]