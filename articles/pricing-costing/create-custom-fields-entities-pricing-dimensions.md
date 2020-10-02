---
title: יצירת שדות וישויות מותאמים אישית כממדי תמחור
description: נושא זה מספק מידע על אופן יצירת ישויות או קבוצות אפשרויות מותאמות אישית.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 2000f7e710267560fe2bd52b0e33024617d108ea
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898262"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a><span data-ttu-id="0a28f-103">יצירת שדות וישויות מותאמים אישית כממדי תמחור</span><span class="sxs-lookup"><span data-stu-id="0a28f-103">Create custom fields and entities as pricing dimensions</span></span>

<span data-ttu-id="0a28f-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="0a28f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="0a28f-105">בצע את השלבים הבאים בכל עת שברצונך ליצור קבוצת אפשרויות או ישות מותאמת אישית.</span><span class="sxs-lookup"><span data-stu-id="0a28f-105">Complete the following steps any time that you want to create a custom option set or entity.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0a28f-106">מומלץ לבצע את כל השינויים בממד התמחור המותאם אישית בפתרון נפרד.</span><span class="sxs-lookup"><span data-stu-id="0a28f-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="0a28f-107">שיטת עבודה מומלצת וחשובה זו מספקת גמישות בעתיד כדי לעדכן או להסיר שינויים בהתאם לצורך, היא תסייע לך להשתמש מחדש בעבודתך ומאפשרת להפנות את השינויים הללו אל מופע אחר בקלות רבה יותר.</span><span class="sxs-lookup"><span data-stu-id="0a28f-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="0a28f-108">לאחר שביצעת את כל השינויים הדרושים, יצא פתרון זה כ**פתרון מנוהל** ויבא אותו אל מופעים אחרים כדי להשתמש שוב בהגדרת התמחור.</span><span class="sxs-lookup"><span data-stu-id="0a28f-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>


## <a name="create-a-custom-solution-for-pricing-dimensions"></a><span data-ttu-id="0a28f-109">יצירת פתרון מותאם אישית עבור ממדי תמחור</span><span class="sxs-lookup"><span data-stu-id="0a28f-109">Create a custom solution for pricing dimensions</span></span>
1. <span data-ttu-id="0a28f-110">עבור אל **הגדרות** > **פתרונות** ולאחר מכן בחר **חדש** כדי ליצור פתרון חדש.</span><span class="sxs-lookup"><span data-stu-id="0a28f-110">Go to **Settings** > **Solutions**, and then select **New** to create a new solution.</span></span> 
2. <span data-ttu-id="0a28f-111">תן שם לפתרון, **\<your organization name> ממדי תמחור**, הזן את המידע הדרוש שנותר ובחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="0a28f-111">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then select **Save**.</span></span>
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="0a28f-112">יצור שדות וקבוצות אפשרויות מותאמים אישית בפתרון ממד התמחור</span><span class="sxs-lookup"><span data-stu-id="0a28f-112">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="0a28f-113">ממד תמחור יכול להיות קבוצת אפשרויות או ישות.</span><span class="sxs-lookup"><span data-stu-id="0a28f-113">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="0a28f-114">יש ליצור את שתיהן בפתרון התמחור.</span><span class="sxs-lookup"><span data-stu-id="0a28f-114">Both must be created in your pricing solution.</span></span> <span data-ttu-id="0a28f-115">השלבים בהליך זה מסבירים כיצד ליצור ממדים מבוססי-ישות וממדים מבוססי-קבוצת אפשרויות.</span><span class="sxs-lookup"><span data-stu-id="0a28f-115">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="0a28f-116">ממדים מבוססי-ישות</span><span class="sxs-lookup"><span data-stu-id="0a28f-116">Entity-based dimensions</span></span>

1. <span data-ttu-id="0a28f-117">עבור אל **הגדרות** > **פתרונות** ולחץ פעמיים על **\<your organization name> ממדי תמחור**.</span><span class="sxs-lookup"><span data-stu-id="0a28f-117">Go to **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="0a28f-118">בסייר הפתרונות, בחלונית הניווט הימנית, בחר **ישויות**.</span><span class="sxs-lookup"><span data-stu-id="0a28f-118">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="0a28f-119">בחר **חדש** כדי ליצור ישות חדשה בשם **כותרת סטנדרטית**.</span><span class="sxs-lookup"><span data-stu-id="0a28f-119">Select **New** to create a new entity called **Standard Title**.</span></span> 
4. <span data-ttu-id="0a28f-120">הזן את המידע הדרוש שנותר ולאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="0a28f-120">Enter the remaining required information, and then select **Save**.</span></span>


### <a name="option-set-based-dimensions"></a><span data-ttu-id="0a28f-121">ממדים מבוססי-קבוצת אפשרויות</span><span class="sxs-lookup"><span data-stu-id="0a28f-121">Option set-based dimensions</span></span> 
<span data-ttu-id="0a28f-122">באפשרותך ליצור שני ממדים מבוססי-קבוצת אפשרויות.</span><span class="sxs-lookup"><span data-stu-id="0a28f-122">You can create two option set-based dimensions.</span></span> <span data-ttu-id="0a28f-123">השתמש באפשרות **מיקום עבודה של משאב** כדי לעקוב אחר המחיר של עבודה במיקום **בית** ועבודה במיקום **באתר** והשתמש באפשרות **שעות עבודה של משאב** עם הערכים **רגיל** ו**שעות נוספות** כדי להחיל ייקור בעת השלמת העבודה.</span><span class="sxs-lookup"><span data-stu-id="0a28f-123">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="0a28f-124">עבור אל **הגדרות** > **פתרונות** ולחץ פעמיים על **\<your organization name> ממדי תמחור**.</span><span class="sxs-lookup"><span data-stu-id="0a28f-124">Go to **Settings** > **Solutions**, and double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="0a28f-125">בסייר הפתרונות, בחלונית הניווט הימנית, בחר **קבוצות אפשרויות**.</span><span class="sxs-lookup"><span data-stu-id="0a28f-125">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="0a28f-126">בחר **חדש** כדי ליצור קבוצת אפשרויות חדשה, הזן את המידע הדרוש שנותר ובחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="0a28f-126">Select **New** to create a new option set, enter the remaining required information, and then select **Save**.</span></span>

## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="0a28f-127">יצירת נתונים עבור ממדים מבוססי-ישות</span><span class="sxs-lookup"><span data-stu-id="0a28f-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="0a28f-128">באפשרותך ליצור נתונים עבור ממדים מבוססי-ישות באופן ידני, או באמצעות ייבוא או קריאות שירות של Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="0a28f-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="0a28f-129">השתמש בשלבים שבהליך זה כדי ליצור שני תארים רגילים, **מהנדס מערכות** ו**מהנדס מערכות בכיר** מהממד מבוסס הישות, **כותרת סטנדרטית**.</span><span class="sxs-lookup"><span data-stu-id="0a28f-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="0a28f-130">אם הנתונים שברצונך ליצור הם בכמות קטנה, בדומה לדוגמה הבאה, באפשרותך להשתמש בטופס רגיל.</span><span class="sxs-lookup"><span data-stu-id="0a28f-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="0a28f-131">בחר **חיפוש מתקדם**, בחר את הישות **כותרת סטנדרטית** ובחר **תוצאות**.</span><span class="sxs-lookup"><span data-stu-id="0a28f-131">Select **Advanced Find**, select the entity **Standard Title**, and then select **Results**.</span></span> <span data-ttu-id="0a28f-132">כל השורות בישות **כותרת סטנדרטית** יוצגו.</span><span class="sxs-lookup"><span data-stu-id="0a28f-132">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="0a28f-133">בחר **חדש**, ובשדה **שם** הזן "מהנדס מערכות" ובחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="0a28f-133">Select **New**, and in the **Name** field, enter "Systems Engineer" and then select **Save**.</span></span>
3. <span data-ttu-id="0a28f-134">סגור את הטופס.</span><span class="sxs-lookup"><span data-stu-id="0a28f-134">Close the form.</span></span> 
4. <span data-ttu-id="0a28f-135">חזור על שלבים 1-3 כדי ליצור כותרת סטנדרטית נוספת עבור "מהנדס מערכות בכיר".</span><span class="sxs-lookup"><span data-stu-id="0a28f-135">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="0a28f-136">הוסף את כל הישויות הנדרשות ואת הרכיבים הקשורים לפתרון ממד התמחור</span><span class="sxs-lookup"><span data-stu-id="0a28f-136">Add all required entities and related components to the Pricing Dimension Solution</span></span>
<span data-ttu-id="0a28f-137">יהיה עליך להוסיף את הישויות הבאות לפתרון התמחור שלך.</span><span class="sxs-lookup"><span data-stu-id="0a28f-137">You will need to add the following entities to your pricing solution.</span></span> <span data-ttu-id="0a28f-138">השתמש בשלבים שבהליך זה כדי לבצע שינויים חשובים בסכימה בפתרון התמחור כך שהישויות יהיו מודעות לממדי התמחור החדשים.</span><span class="sxs-lookup"><span data-stu-id="0a28f-138">Use the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="0a28f-139">בחר **הגדרות** > **פתרונות** ולחץ פעמיים על **\<your organization name> ממדי תמחור**.</span><span class="sxs-lookup"><span data-stu-id="0a28f-139">Select **Settings** > **Solutions**, and double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="0a28f-140">בסייר הפתרונות, בחלונית הניווט הימנית בחר **הוסף קיים**  > **ישויות**.</span><span class="sxs-lookup"><span data-stu-id="0a28f-140">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="0a28f-141">בתיבת הדו-שיח **רכיבי פתרון**, בחר את הישויות הבאות:</span><span class="sxs-lookup"><span data-stu-id="0a28f-141">In the **Solution Components** dialog box, select the following entities:</span></span>

  - <span data-ttu-id="0a28f-142">בפועל</span><span class="sxs-lookup"><span data-stu-id="0a28f-142">Actual</span></span>
  - <span data-ttu-id="0a28f-143">משאב הניתן להזמנה</span><span class="sxs-lookup"><span data-stu-id="0a28f-143">Bookable Resource</span></span>
  - <span data-ttu-id="0a28f-144">שורת הערכה</span><span class="sxs-lookup"><span data-stu-id="0a28f-144">Estimate Line</span></span>
  - <span data-ttu-id="0a28f-145">פרט בשורת חשבונית</span><span class="sxs-lookup"><span data-stu-id="0a28f-145">Invoice Line Detail</span></span>
  - <span data-ttu-id="0a28f-146">שורת יומן</span><span class="sxs-lookup"><span data-stu-id="0a28f-146">Journal Line</span></span>
  - <span data-ttu-id="0a28f-147">פרט סעיף חוזה של פרויקט</span><span class="sxs-lookup"><span data-stu-id="0a28f-147">Project Contract Line Detail</span></span>
  - <span data-ttu-id="0a28f-148">חבר צוות פרויקט</span><span class="sxs-lookup"><span data-stu-id="0a28f-148">Project Team Member</span></span>
  - <span data-ttu-id="0a28f-149">פרטים בשורת הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="0a28f-149">Quote Line Detail</span></span>
  - <span data-ttu-id="0a28f-150">ייקור מחיר תפקיד</span><span class="sxs-lookup"><span data-stu-id="0a28f-150">Role Price Markup</span></span>
  - <span data-ttu-id="0a28f-151">מחיר תפקיד</span><span class="sxs-lookup"><span data-stu-id="0a28f-151">Role Price</span></span> 
  - <span data-ttu-id="0a28f-152">ערך זמן</span><span class="sxs-lookup"><span data-stu-id="0a28f-152">Time Entry</span></span> 


> [!NOTE]
> <span data-ttu-id="0a28f-153">הקפד לכלול את כל הטפסים והתצוגות עבור כל אחת מהישויות שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="0a28f-153">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="0a28f-154">כאשר תתבקש לכלול ישויות תלויות עבור הישויות שנבחרו לעיל, בחר **לא**.</span><span class="sxs-lookup"><span data-stu-id="0a28f-154">When prompted to include any dependent entities for the entities selected above, select **No**.</span></span>

