---
title: יצירת שדות וישויות מותאמים אישית
description: נושא זה מסביר כיצד ליצור קבוצות אפשרויות וישויות בפתרון שלך בפלטפורמת Power Apps.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/26/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: fb160bfd-e037-4a21-a968-3ff2e6e16481
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 7ee30e3bb6b8034ef226e2e9181195685355011f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751871"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="823dc-103">יצירת שדות וישויות מותאמים אישית</span><span class="sxs-lookup"><span data-stu-id="823dc-103">Create custom fields and entities</span></span> 

<span data-ttu-id="823dc-104">בצע את השלבים הבאים בכל עת שברצונך ליצור קבוצת אפשרויות או ישות מותאמת אישית בפלטפורמת Power Apps.</span><span class="sxs-lookup"><span data-stu-id="823dc-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="823dc-105">יש להשלים את ההליכים בנושא זה באמצעות ממשק האינטרנט של Project Service Automation‏ (PSA).</span><span class="sxs-lookup"><span data-stu-id="823dc-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="823dc-106">מומלץ לבצע את כל השינויים בממד התמחור המותאם אישית בפתרון נפרד.</span><span class="sxs-lookup"><span data-stu-id="823dc-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="823dc-107">שיטת עבודה מומלצת וחשובה זו מספקת גמישות בעתיד כדי לעדכן או להסיר שינויים בהתאם לצורך, היא תסייע לך להשתמש מחדש בעבודתך ומאפשרת להפנות את השינויים הללו אל מופע אחר בקלות רבה יותר.</span><span class="sxs-lookup"><span data-stu-id="823dc-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="823dc-108">לאחר שביצעת את כל השינויים הדרושים, יצא פתרון זה כ**פתרון מנוהל** ויבא אותו אל מופעים אחרים כדי להשתמש שוב בהגדרת התמחור.</span><span class="sxs-lookup"><span data-stu-id="823dc-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>


## <a name="create-a-custom-solution-for-pricing-dimensions"></a><span data-ttu-id="823dc-109">יצירת פתרון מותאם אישית עבור ממדי תמחור</span><span class="sxs-lookup"><span data-stu-id="823dc-109">Create a custom solution for pricing dimensions</span></span>
1. <span data-ttu-id="823dc-110">ב- PSA, לחץ על **הגדרות** > **פתרונות** ולאחר מכן לחץ על **חדש** כדי ליצור פתרון חדש.</span><span class="sxs-lookup"><span data-stu-id="823dc-110">In PSA, click **Settings** > **Solutions**, and then click **New** to create a new solution.</span></span> 
2. <span data-ttu-id="823dc-111">תן שם לפתרון, **\<שם הארגון שלך> ממדי תמחור**, הזן את המידע הדרוש שנותר ולחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="823dc-111">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then click **Save**.</span></span>

> ![יצירת פתרון מותאם אישית עבור ממדי תמחור](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="823dc-113">יצור שדות וקבוצות אפשרויות מותאמים אישית בפתרון ממד התמחור</span><span class="sxs-lookup"><span data-stu-id="823dc-113">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="823dc-114">ממד תמחור יכול להיות קבוצת אפשרויות או ישות.</span><span class="sxs-lookup"><span data-stu-id="823dc-114">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="823dc-115">יש ליצור את שתיהן בפתרון התמחור.</span><span class="sxs-lookup"><span data-stu-id="823dc-115">Both must be created in your pricing solution.</span></span> <span data-ttu-id="823dc-116">השלבים בהליך זה מסבירים כיצד ליצור ממדים מבוססי-ישות וממדים מבוססי-קבוצת אפשרויות.</span><span class="sxs-lookup"><span data-stu-id="823dc-116">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="823dc-117">ממדים מבוססי-ישות</span><span class="sxs-lookup"><span data-stu-id="823dc-117">Entity-based dimensions</span></span>

1. <span data-ttu-id="823dc-118">ב- PSA, לחץ על **הגדרות** > **פתרונות**, ולאחר מכן לחץ לחיצה כפולה על **\<שם הארגון שלך> - ממדי תמחור**.</span><span class="sxs-lookup"><span data-stu-id="823dc-118">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="823dc-119">בסייר הפתרונות, בחלונית הניווט הימנית, בחר **ישויות**.</span><span class="sxs-lookup"><span data-stu-id="823dc-119">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="823dc-120">לחץ על **חדש** כדי ליצור ישות חדשה בשם **כותרת סטנדרטית**.</span><span class="sxs-lookup"><span data-stu-id="823dc-120">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="823dc-121">הזן את המידע הדרוש שנותר ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="823dc-121">Enter the remaining required information, and then click **Save**.</span></span>

> ![הגדרת ישות של כותרת סטנדרטית](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="823dc-123">ממדים מבוססי-קבוצת אפשרויות</span><span class="sxs-lookup"><span data-stu-id="823dc-123">Option set-based dimensions</span></span> 
<span data-ttu-id="823dc-124">באפשרותך ליצור שני ממדים מבוססי-קבוצת אפשרויות.</span><span class="sxs-lookup"><span data-stu-id="823dc-124">You can create two option set-based dimensions.</span></span> <span data-ttu-id="823dc-125">השתמש באפשרות **מיקום עבודה של משאב** כדי לעקוב אחר המחיר של עבודה במיקום **בית** ועבודה במיקום **באתר** והשתמש באפשרות **שעות עבודה של משאב** עם הערכים **רגיל** ו**שעות נוספות** כדי להחיל ייקור בעת השלמת העבודה.</span><span class="sxs-lookup"><span data-stu-id="823dc-125">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="823dc-126">ב- PSA, לחץ על **הגדרות** > **פתרונות**, ולאחר מכן לחץ לחיצה כפולה על **\<שם הארגון שלך> ממדי תמחור**.</span><span class="sxs-lookup"><span data-stu-id="823dc-126">In PSA, click **Settings** > **Solutions**, and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="823dc-127">בסייר הפתרונות, בחלונית הניווט הימנית, בחר **קבוצות אפשרויות**.</span><span class="sxs-lookup"><span data-stu-id="823dc-127">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="823dc-128">לחץ על **חדש** כדי ליצור קבוצת אפשרויות חדשה, הזן את המידע הדרוש שנותר ולחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="823dc-128">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="823dc-129">ממד תמחור מבוסס-קבוצת אפשרויות הנקרא 'מיקום עבודה של משאב'</span><span class="sxs-lookup"><span data-stu-id="823dc-129">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="823dc-130">ממד תמחור מבוסס-קבוצת אפשרויות הנקרא 'שעות עבודה של משאב'</span><span class="sxs-lookup"><span data-stu-id="823dc-130">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="823dc-131">יצירת נתונים עבור ממדים מבוססי-ישות</span><span class="sxs-lookup"><span data-stu-id="823dc-131">Create data for entity-based dimensions</span></span>

<span data-ttu-id="823dc-132">באפשרותך ליצור נתונים עבור ממדים מבוססי-ישות באופן ידני, או באמצעות ייבוא או קריאות שירות של Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="823dc-132">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="823dc-133">השתמש בשלבים שבהליך זה כדי ליצור שני תארים רגילים, **מהנדס מערכות** ו**מהנדס מערכות בכיר** מהממד מבוסס הישות, **כותרת סטנדרטית**.</span><span class="sxs-lookup"><span data-stu-id="823dc-133">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="823dc-134">אם הנתונים שברצונך ליצור הם בכמות קטנה, בדומה לדוגמה הבאה, באפשרותך להשתמש בטופס רגיל.</span><span class="sxs-lookup"><span data-stu-id="823dc-134">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="823dc-135">ב-PSA, לחץ על **חיפוש מתקדם**.</span><span class="sxs-lookup"><span data-stu-id="823dc-135">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="823dc-136">בחר את הישות **כותרת סטנדרטית** ולחץ על **תוצאות**.</span><span class="sxs-lookup"><span data-stu-id="823dc-136">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="823dc-137">כל השורות בישות **כותרת סטנדרטית** יוצגו.</span><span class="sxs-lookup"><span data-stu-id="823dc-137">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="823dc-138">לחץ על **חדש**.</span><span class="sxs-lookup"><span data-stu-id="823dc-138">Click **New**.</span></span> <span data-ttu-id="823dc-139">בשדה **שם**, הזן "מהנדס מערכות" ולחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="823dc-139">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="823dc-140">סגור את הטופס.</span><span class="sxs-lookup"><span data-stu-id="823dc-140">Close the form.</span></span> 
4. <span data-ttu-id="823dc-141">חזור על שלבים 1-3 כדי ליצור כותרת סטנדרטית נוספת עבור "מהנדס מערכות בכיר".</span><span class="sxs-lookup"><span data-stu-id="823dc-141">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="823dc-142">נתונים לדוגמה עבור ישות 'כותרת סטנדרטית'</span><span class="sxs-lookup"><span data-stu-id="823dc-142">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)

## <a name="add-all-required-psa-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="823dc-143">הוסף את כל ישויות PSA הנדרשות ואת הרכיבים הקשורים לפתרון ממד התמחור</span><span class="sxs-lookup"><span data-stu-id="823dc-143">Add all required PSA entities and related components to the Pricing Dimension Solution</span></span>
<span data-ttu-id="823dc-144">יהיה עליך להוסיף את הישויות הבאות של Project Service לפתרון התמחור שלך.</span><span class="sxs-lookup"><span data-stu-id="823dc-144">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="823dc-145">השתמש בשלבים שבהליך זה כדי לבצע שינויים חשובים בסכימה בפתרון התמחור כך שהישויות יהיו מודעות לממדי התמחור החדשים.</span><span class="sxs-lookup"><span data-stu-id="823dc-145">Use the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="823dc-146">ב- PSA, לחץ על **הגדרות** > **פתרונות**, ולאחר מכן לחץ לחיצה כפולה על **\<שם הארגון שלך> - ממדי תמחור**.</span><span class="sxs-lookup"><span data-stu-id="823dc-146">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="823dc-147">בסייר הפתרונות, בחלונית הניווט הימנית בחר **הוסף קיים**  > **ישויות**.</span><span class="sxs-lookup"><span data-stu-id="823dc-147">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="823dc-148">בתיבת הדו-שיח **רכיבי פתרון**, בחר את הישויות הבאות:</span><span class="sxs-lookup"><span data-stu-id="823dc-148">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="823dc-149">בפועל</span><span class="sxs-lookup"><span data-stu-id="823dc-149">Actual</span></span>
- <span data-ttu-id="823dc-150">משאב הניתן להזמנה</span><span class="sxs-lookup"><span data-stu-id="823dc-150">Bookable Resource</span></span>
- <span data-ttu-id="823dc-151">שורת הערכה</span><span class="sxs-lookup"><span data-stu-id="823dc-151">Estimate Line</span></span>
- <span data-ttu-id="823dc-152">פרט בשורת חשבונית</span><span class="sxs-lookup"><span data-stu-id="823dc-152">Invoice Line Detail</span></span>
- <span data-ttu-id="823dc-153">שורת יומן</span><span class="sxs-lookup"><span data-stu-id="823dc-153">Journal Line</span></span>
- <span data-ttu-id="823dc-154">פרט סעיף חוזה של פרוייקט</span><span class="sxs-lookup"><span data-stu-id="823dc-154">Project Contract Line Detail</span></span>
- <span data-ttu-id="823dc-155">חבר צוות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="823dc-155">Project Team Member</span></span>
- <span data-ttu-id="823dc-156">פרטים בשורת הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="823dc-156">Quote Line Detail</span></span>
- <span data-ttu-id="823dc-157">ייקור מחיר תפקיד</span><span class="sxs-lookup"><span data-stu-id="823dc-157">Role Price Markup</span></span>
- <span data-ttu-id="823dc-158">מחיר תפקיד</span><span class="sxs-lookup"><span data-stu-id="823dc-158">Role Price</span></span> 
- <span data-ttu-id="823dc-159">ערך זמן</span><span class="sxs-lookup"><span data-stu-id="823dc-159">Time Entry</span></span> 

> ![הוספת ישויות קיימות לפתרון ממדי התמחור](media/Existing-entities-to-PD-solution.png)

> ![בחירת רכיבי פתרון](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="823dc-162">הקפד לכלול את כל הטפסים והתצוגות עבור כל אחת מהישויות שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="823dc-162">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="823dc-163">כאשר תתבקש לכלול ישויות תלויות עבור הישויות שנבחרו לעיל, לחץ על **לא**.</span><span class="sxs-lookup"><span data-stu-id="823dc-163">When prompted to include any dependent entities for the entities selected above, click **No**.</span></span>

> ![אל תכלול את כל הרכיבים הקשורים](media/Do-not-include-required.png)


