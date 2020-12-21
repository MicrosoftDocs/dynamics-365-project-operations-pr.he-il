---
title: יצירת שדות וישויות מותאמים אישית כממדי תמחור
description: נושא זה מספק מידע על אופן יצירת ישויות או קבוצות אפשרויות מותאמות אישית.
author: rumant
manager: AnnBe
ms.date: 11/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
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
ms.openlocfilehash: fc5917856b8f28d36dc55593a68eba7823a00b36
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642814"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a><span data-ttu-id="de54c-103">יצירת שדות וישויות מותאמים אישית כממדי תמחור</span><span class="sxs-lookup"><span data-stu-id="de54c-103">Create custom fields and entities as pricing dimensions</span></span>

<span data-ttu-id="de54c-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="de54c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="de54c-105">בצע את השלבים הבאים כאשר ברצונך ליצור קבוצת אפשרויות או ישות מותאמת אישית לשימוש בתור ממד תמחור.</span><span class="sxs-lookup"><span data-stu-id="de54c-105">Complete the following steps when you want to create a custom option set or entity for using it as a pricing dimension.</span></span> <span data-ttu-id="de54c-106">למידע נוסף, ראה [מבט כולל על ממדי תמחור](pricing-dimensions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="de54c-106">For more information, see [Pricing dimensions overview](pricing-dimensions-overview.md).</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="de54c-107">מומלץ לבצע את כל השינויים בממד התמחור המותאם אישית בפתרון נפרד.</span><span class="sxs-lookup"><span data-stu-id="de54c-107">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="de54c-108">שיטה מומלצת חשובה זו מספקת גמישות בעתיד לצורך עדכון או הסרת שינויים לפי הצורך.</span><span class="sxs-lookup"><span data-stu-id="de54c-108">This important best practice provides flexibility in the future to update or remove changes as needed.</span></span> <span data-ttu-id="de54c-109">היא גם תעזור לעשות שימוש חוזר בעבודה שכבר עשית, ותקל על העברת השינויים למופע אחר. אחרי שביצעת את כל השינויים הנדרשים, ייצא פתרון זה כ **פתרון מנוהל** וייבא אותו למופעים אחרים כדי לעשות שימוש חוזר בהגדרת התמחור.</span><span class="sxs-lookup"><span data-stu-id="de54c-109">This will also help with re-use of your work and make it easier to port these changes to another instance After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="de54c-110">יצור שדות וקבוצות אפשרויות מותאמים אישית בפתרון ממד התמחור</span><span class="sxs-lookup"><span data-stu-id="de54c-110">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="de54c-111">ממד תמחור יכול להיות קבוצת אפשרויות או ישות.</span><span class="sxs-lookup"><span data-stu-id="de54c-111">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="de54c-112">יש ליצור את שתיהן בפתרון התמחור.</span><span class="sxs-lookup"><span data-stu-id="de54c-112">Both must be created in your pricing solution.</span></span> <span data-ttu-id="de54c-113">השלבים בהליך זה מסבירים כיצד ליצור ממדים מבוססי-ישות וממדים מבוססי-קבוצת אפשרויות.</span><span class="sxs-lookup"><span data-stu-id="de54c-113">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="de54c-114">ממדים מבוססי-ישות</span><span class="sxs-lookup"><span data-stu-id="de54c-114">Entity-based dimensions</span></span>
<span data-ttu-id="de54c-115">כדי ליצור ממדים מבוססי-ישות, בצע את הצעדים הבאים:</span><span class="sxs-lookup"><span data-stu-id="de54c-115">To create entity-based dimensions, follow these steps:</span></span>

1. <span data-ttu-id="de54c-116">עבור אל **הגדרות** > **פתרונות** ולחץ פעמיים על **\<your organization name> ממדי תמחור**.</span><span class="sxs-lookup"><span data-stu-id="de54c-116">Go to **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="de54c-117">בסייר הפתרונות, בחלונית הניווט הימנית, בחר **ישויות**.</span><span class="sxs-lookup"><span data-stu-id="de54c-117">In Solution Explorer, in the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="de54c-118">בחר **חדש** כדי ליצור ישות חדשה בשם **כותרת סטנדרטית**.</span><span class="sxs-lookup"><span data-stu-id="de54c-118">Select **New** to create a new entity called **Standard Title**.</span></span> 
4. <span data-ttu-id="de54c-119">הזן את המידע הדרוש שנותר ולאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="de54c-119">Enter the remaining required information, and then select **Save**.</span></span>

> ![הגדרת ישות של כותרת סטנדרטית](media/Standard-Title-entity-definition.png)

### <a name="option-set-based-dimensions"></a><span data-ttu-id="de54c-121">ממדים מבוססי-קבוצת אפשרויות</span><span class="sxs-lookup"><span data-stu-id="de54c-121">Option set-based dimensions</span></span> 
<span data-ttu-id="de54c-122">באפשרותך ליצור שני ממדים מבוססי-קבוצת אפשרויות.</span><span class="sxs-lookup"><span data-stu-id="de54c-122">You can create two option set-based dimensions.</span></span> 

- <span data-ttu-id="de54c-123">השתמש ב **מיקום עבודת משאבים** כדי לעקוב אחר המחיר של מיקום העבודה **בית** או **באתר**.</span><span class="sxs-lookup"><span data-stu-id="de54c-123">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work.</span></span> 
- <span data-ttu-id="de54c-124">השתמש באפשרות **שעות עבודה של משאבים** עם הערכים **רגיל** ו **שעות נוספות** כדי להחיל ייקור כאשר העבודה מסתיימת.</span><span class="sxs-lookup"><span data-stu-id="de54c-124">Use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when the work is complete.</span></span>

<span data-ttu-id="de54c-125">האיור הבא מציג את הממד **מיקום עבודת משאבים**.</span><span class="sxs-lookup"><span data-stu-id="de54c-125">The following graphic provides a view of the **Resource Work Location** dimension.</span></span> 

> ![ממד תמחור מבוסס-קבוצת אפשרויות הנקרא 'מיקום עבודה של משאב'](media/Option-set-PD-called-Resource-Work-Location.png)

<span data-ttu-id="de54c-127">האיור הבא מציג את הממד **שעות עבודה של משאבים**.</span><span class="sxs-lookup"><span data-stu-id="de54c-127">The following graphic provides a view of the **Resource Work Hours** dimension.</span></span> 

> ![ממד תמחור מבוסס-קבוצת אפשרויות הנקרא 'שעות עבודה של משאב'](media/Option-set-PD-called-Resource-Work-Hours.png)

1. <span data-ttu-id="de54c-129">עבור אל **הגדרות** > **פתרונות** ולחץ פעמיים על **\<your organization name> ממדי תמחור**.</span><span class="sxs-lookup"><span data-stu-id="de54c-129">Go to **Settings** > **Solutions**, and double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="de54c-130">בסייר הפתרונות, בחלונית הניווט הימנית, בחר **קבוצות אפשרויות**.</span><span class="sxs-lookup"><span data-stu-id="de54c-130">In Solution Explorer, in the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="de54c-131">בחר **חדש** כדי ליצור קבוצת אפשרויות חדשה, הזן את המידע הדרוש שנותר ובחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="de54c-131">Select **New** to create a new option set, enter the remaining required information, and then select **Save**.</span></span>

## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="de54c-132">יצירת נתונים עבור ממדים מבוססי-ישות</span><span class="sxs-lookup"><span data-stu-id="de54c-132">Create data for entity-based dimensions</span></span>

<span data-ttu-id="de54c-133">באפשרותך ליצור נתונים עבור ממדים מבוססי-ישות באופן ידני, או באמצעות ייבוא או קריאות שירות של Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="de54c-133">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="de54c-134">השתמש בשלבים שבהליך זה כדי ליצור שני תארים רגילים, **מהנדס מערכות** ו **מהנדס מערכות בכיר** מהממד מבוסס הישות, **כותרת סטנדרטית**.</span><span class="sxs-lookup"><span data-stu-id="de54c-134">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="de54c-135">אם הנתונים שברצונך ליצור הם בכמות קטנה, בדומה לדוגמה הבאה, באפשרותך להשתמש בטופס רגיל.</span><span class="sxs-lookup"><span data-stu-id="de54c-135">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="de54c-136">בחר **חיפוש מתקדם**.</span><span class="sxs-lookup"><span data-stu-id="de54c-136">Select **Advanced Find**.</span></span>
2. <span data-ttu-id="de54c-137">בחר את הישות **כותרת סטנדרטית** ובחר **תוצאות**.</span><span class="sxs-lookup"><span data-stu-id="de54c-137">Select the entity **Standard Title**, and then select **Results**.</span></span> <span data-ttu-id="de54c-138">כל השורות בישות **כותרת סטנדרטית** יוצגו.</span><span class="sxs-lookup"><span data-stu-id="de54c-138">All of the rows in the **Standard Title** entity will be shown.</span></span>
3. <span data-ttu-id="de54c-139">בחר **חדש**, ובשדה **שם** הזן "מהנדס מערכות" ובחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="de54c-139">Select **New**, and in the **Name** field, enter "Systems Engineer" and then select **Save**.</span></span>
4. <span data-ttu-id="de54c-140">סגור את הדף.</span><span class="sxs-lookup"><span data-stu-id="de54c-140">Close the page.</span></span> 
5. <span data-ttu-id="de54c-141">חזור על שלבים 1-3 כדי ליצור כותרת סטנדרטית נוספת עבור "מהנדס מערכות בכיר".</span><span class="sxs-lookup"><span data-stu-id="de54c-141">Repeat steps 1-3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![נתונים לדוגמה עבור ישות 'כותרת סטנדרטית'](media/ST-data.png)
