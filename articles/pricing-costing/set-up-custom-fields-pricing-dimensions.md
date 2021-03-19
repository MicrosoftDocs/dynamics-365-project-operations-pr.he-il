---
title: הגדרת שדות מותאמים אישית כממדי תמחור
description: נושא זה מספק מידע על אופן ההגדרה של ממדי תמחור באמצעות שדות מותאמים אישית.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
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
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 1468c3396a01c1bee1bc0f47eac1ee8b44eaa459
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274864"
---
# <a name="set-up-custom-fields-as-pricing-dimensions"></a><span data-ttu-id="1ed52-103">הגדרת שדות מותאמים אישית כממדי תמחור</span><span class="sxs-lookup"><span data-stu-id="1ed52-103">Set up custom fields as pricing dimensions</span></span>

<span data-ttu-id="1ed52-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="1ed52-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1ed52-105">לפני שתתחיל, נושא זה יוצא מנקודת הנחה שהשלמת את ההליכים בנושאים [יצירת שדות וישויות מותאמים אישית](create-custom-fields-entities-pricing-dimensions.md) ו[הוספת שדות מותאמים אישית להגדרת מחיר וישויות של טרנזקציות](add-custom-fields-price-setup-transactional-entities.md).</span><span class="sxs-lookup"><span data-stu-id="1ed52-105">Before you begin, this topic assumes that you have completed the procedures in the topics, [Create custom fields and entities](create-custom-fields-entities-pricing-dimensions.md) and [Add required custom fields to price setup and transactional entities](add-custom-fields-price-setup-transactional-entities.md).</span></span> <span data-ttu-id="1ed52-106">אם לא השלמת הליכים אלה, חזור והשלם אותם ולאחר מכן חזור לנושא זה.</span><span class="sxs-lookup"><span data-stu-id="1ed52-106">If you haven't completed those procedures, go back and complete them and then return to this topic.</span></span> 

<span data-ttu-id="1ed52-107">נושא זה מספק מידע אודות הגדרה של ממדי תמחור מותאמים אישית.</span><span class="sxs-lookup"><span data-stu-id="1ed52-107">This topic provides information about setting up custom pricing dimensions.</span></span> <span data-ttu-id="1ed52-108">בדף **פרמטרים**, הכרטיסיה ‏‫**ממדי תמחור מבוססי-כמות** מראה את הרשומות בישויות של ממדי התמחור.</span><span class="sxs-lookup"><span data-stu-id="1ed52-108">On the **Parameters** page, the **Amount-Based Pricing Dimensions** tab shows the records in the pricing dimension entities.</span></span> <span data-ttu-id="1ed52-109">כברירת מחדל, יש שתי שורות ברשת בכרטיסיה זו:</span><span class="sxs-lookup"><span data-stu-id="1ed52-109">By default, there are two rows in the grid on this tab:</span></span>

- <span data-ttu-id="1ed52-110">**msdyn_resourcecategory** (תפקיד)</span><span class="sxs-lookup"><span data-stu-id="1ed52-110">**msdyn_resourcecategory** (Role)</span></span>
- <span data-ttu-id="1ed52-111">**msdyn_OrganizationalUnit** (יחידה ארגונית)</span><span class="sxs-lookup"><span data-stu-id="1ed52-111">**msdyn_OrganizationalUnit** (Organizational Unit)</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1ed52-112">אל תמחק שורות אלה.</span><span class="sxs-lookup"><span data-stu-id="1ed52-112">Do not delete these rows.</span></span> <span data-ttu-id="1ed52-113">עם זאת, אם אינך זקוק להן, ניתן להפוך אותן לבלתי ניתנות להחלה בהקשר מסוים על-ידי הגדרת כל האפשרויות הבאות: **חל על עלות‬**, **חל על מכירות** ו **חל על רכישה** ל **לא**.</span><span class="sxs-lookup"><span data-stu-id="1ed52-113">However, if you do not need them, you can make them not applicable in a specific context by setting **Applicable to Cost**, **Applicable to Sales**, and **Applicable to Purchase** all to **No**.</span></span> <span data-ttu-id="1ed52-114">הגדרת ערכי התכונות הללו ל **לא** משפיעה באופן זהה לזה שהשדה אינו ממד תמחור.</span><span class="sxs-lookup"><span data-stu-id="1ed52-114">Setting these attribute values to **No** has the same effect of not having the field as a pricing dimension.</span></span>

<span data-ttu-id="1ed52-115">כדי ששדה יהפוך לממד תמחור, עליו לעמוד בתנאים הבאים:</span><span class="sxs-lookup"><span data-stu-id="1ed52-115">For a field to become a pricing dimension, it must be:</span></span>

- <span data-ttu-id="1ed52-116">עליו להיווצר כשדה בישויות **מחיר תפקיד** ו **ייקור מחיר תפקיד**.</span><span class="sxs-lookup"><span data-stu-id="1ed52-116">Created as a field in the **Role Price** and **Role Price markup** entities.</span></span> <span data-ttu-id="1ed52-117">למידע נוסף שבעזרתו תגלה כיצד לעשות זאת, ראה [הוספת שדות מותאמים אישית להגדרת מחיר וישויות של טרנזקציות](add-custom-fields-price-setup-transactional-entities.md).</span><span class="sxs-lookup"><span data-stu-id="1ed52-117">For more information on how to do this, see [Add custom fields to price setup and transactional entities](add-custom-fields-price-setup-transactional-entities.md).</span></span>

- <span data-ttu-id="1ed52-118">עליו להיווצר כשורה בטבלה **ממד תמחור**.</span><span class="sxs-lookup"><span data-stu-id="1ed52-118">Created as a row in the **Pricing Dimension** table.</span></span> <span data-ttu-id="1ed52-119">לדוגמה, הוסף שורות ממד תמחור כמוצג בגרפיקה הבאה.</span><span class="sxs-lookup"><span data-stu-id="1ed52-119">For example, add pricing dimension rows as shown in the following graphic.</span></span> 

![שורות ממדי תמחור מבוססי-כמות](media/Amt-based-PD.png)

<span data-ttu-id="1ed52-121">שעות העבודה של המשאב (**msdyn_resourceworkhours**) נוספו כממד מבוסס-ייקור ונוספו לרשת בכרטיסיה **ממד תמחור מבוסס-ייקור**.</span><span class="sxs-lookup"><span data-stu-id="1ed52-121">Resource Work hours (**msdyn_resourceworkhours**) is added as a markup-based dimension and has been added to the grid on the **Markup Based Pricing Dimension** tab.</span></span>

![שורות ממדי תמחור מבוססי-ייקור](media/Markup-based-PD.png)


> [!IMPORTANT]
> <span data-ttu-id="1ed52-123">כל שינוי בנתונים של ממד התמחור בטבלה זו, קיים או חדש, מועבר בירושה ללוגיקה העסקית של תמחור רק לאחר רענון המטמון.</span><span class="sxs-lookup"><span data-stu-id="1ed52-123">Any change to pricing dimension data in this table, existing or new, is propagated to the pricing business logic only after the cache is refreshed.</span></span> <span data-ttu-id="1ed52-124">זמן הרענון של המטמון עשוי להימשך עד 10 דקות.</span><span class="sxs-lookup"><span data-stu-id="1ed52-124">The cache refresh time may take up to 10 minutes.</span></span> <span data-ttu-id="1ed52-125">אפשר פרק זמן זה כדי לראות את השינויים בלוגיקת ברירת המחדל למחיר שעשויה לנבוע משינויים בנתוני ממד התמחור.</span><span class="sxs-lookup"><span data-stu-id="1ed52-125">Allow that length of time to see the changes in price defaulting logic that must result from changes to the Pricing Dimension data.</span></span>


## <a name="attributes-of-the-pricing-dimensions-table"></a><span data-ttu-id="1ed52-126">תכונות של הטבלה 'ממדי תמחור'</span><span class="sxs-lookup"><span data-stu-id="1ed52-126">Attributes of the Pricing Dimensions table</span></span>
<span data-ttu-id="1ed52-127">הסעיפים הבאים מספקים מידע אודות התכונות השונות בטבלה **ממדי תמחור**.</span><span class="sxs-lookup"><span data-stu-id="1ed52-127">The following sections provide information about the different attributes in the **Pricing Dimensions** table.</span></span>

### <a name="pricing-dimension-name"></a><span data-ttu-id="1ed52-128">שם ממד התמחור</span><span class="sxs-lookup"><span data-stu-id="1ed52-128">Pricing Dimension Name</span></span>
<span data-ttu-id="1ed52-129">ערך זה צריך להיות זהה לגמרי לשם הסכימה של השדה שנוסף לטבלה **מחיר תפקיד** עבור ממדי תמחור מותאמים אישית.</span><span class="sxs-lookup"><span data-stu-id="1ed52-129">This value should be the exact same as the schema name of the field that is added to the **Role Price** table for custom pricing dimensions.</span></span> <span data-ttu-id="1ed52-130">לקבלת מידע נוסף אודות הוספת שדות לטבלה **מחיר תפקיד**, ראה [‬‏‫הוספת שדות מותאמים אישית להגדרת מחיר וישויות של טרנזקציות](add-custom-fields-price-setup-transactional-entities.md).</span><span class="sxs-lookup"><span data-stu-id="1ed52-130">For more information about adding fields to the **Role Price** table, see [Add custom fields to price setup and transactional entities](add-custom-fields-price-setup-transactional-entities.md).</span></span>

### <a name="type-of-dimension"></a><span data-ttu-id="1ed52-131">סוג ממד</span><span class="sxs-lookup"><span data-stu-id="1ed52-131">Type of dimension</span></span>
<span data-ttu-id="1ed52-132">קיימים שני סוגים של ממדי תמחור:</span><span class="sxs-lookup"><span data-stu-id="1ed52-132">There are two types of pricing dimensions:</span></span>
  
  - <span data-ttu-id="1ed52-133">**ממדים מבוססי-כמות**: ערכי הממד מהקשר הקלט מותאמים לערכי הממד בשורה **מחיר תפקיד** והמחיר/העלות מוגדרים כברירת מחדל ישירות מהטבלה **מחיר תפקיד**.</span><span class="sxs-lookup"><span data-stu-id="1ed52-133">**Amount-based dimensions**: The dimension values from the input context are matched to the dimension values on **Role Price** line and the price/cost is defaulted directly from the **Role Price** table.</span></span>
  - <span data-ttu-id="1ed52-134">**ממדים מבוססי-ייקור**: אלה הם ממדים שבהם נעשה שימוש בתהליך בן שלושה שלבים כדי לקבל את המחיר/העלות:</span><span class="sxs-lookup"><span data-stu-id="1ed52-134">**Markup-based dimensions**: These are dimensions where the following three-step process to get the price/cost is used:</span></span>
 
    1. <span data-ttu-id="1ed52-135">ערכי הממד שאינו מבוסס-ייקור מהקשר הקלט מותאמים לשורה 'מחיר תפקיד' כדי לקבל את תעריף הבסיס.</span><span class="sxs-lookup"><span data-stu-id="1ed52-135">The non-markup-based dimension values from the input context are matched to the Role Price line to get the base rate.</span></span>
    2. <span data-ttu-id="1ed52-136">מבוצעת התאמה של ערכי הממד מהקשר הקלט לשורה **ייקור מחיר תפקיד** כדי לקבל אחוז ייקור.</span><span class="sxs-lookup"><span data-stu-id="1ed52-136">The dimension values from the input context are matched to the **Role Price Markup** line to get a markup percentage.</span></span>
    3. <span data-ttu-id="1ed52-137">אחוז הייקור מהשלב השני מוחל על תעריף הבסיס שהושג מן הטבלה **מחיר תפקיד** בשלב הראשון כדי להגיע למחיר/עלות סופיים.</span><span class="sxs-lookup"><span data-stu-id="1ed52-137">The markup percentage from the second step is applied to the base rate obtained from the **Role Price** table in the first step to arrive at final price/cost.</span></span>
   
   <span data-ttu-id="1ed52-138">הטבלה הבאה מתארת את החישוב של ייקורי מחירים.</span><span class="sxs-lookup"><span data-stu-id="1ed52-138">The following table illustrates the calculation of price markups.</span></span>
  
| <span data-ttu-id="1ed52-139">תפקיד</span><span class="sxs-lookup"><span data-stu-id="1ed52-139">Role</span></span>        | <span data-ttu-id="1ed52-140">יחידה ארגונית</span><span class="sxs-lookup"><span data-stu-id="1ed52-140">Org Unit</span></span>    |<span data-ttu-id="1ed52-141">מיקום עבודה</span><span class="sxs-lookup"><span data-stu-id="1ed52-141">Work Location</span></span>      |<span data-ttu-id="1ed52-142">כותרת סטנדרטית</span><span class="sxs-lookup"><span data-stu-id="1ed52-142">Standard Title</span></span>      |<span data-ttu-id="1ed52-143">שעות עבודה של משאב</span><span class="sxs-lookup"><span data-stu-id="1ed52-143">Resource Work Hours</span></span>      |  <span data-ttu-id="1ed52-144">ייקור</span><span class="sxs-lookup"><span data-stu-id="1ed52-144">Mark Up</span></span>|
| ------------|-------------|-------------------|--------------------|-------------------------|--------:|
|             | <span data-ttu-id="1ed52-145">Contoso India</span><span class="sxs-lookup"><span data-stu-id="1ed52-145">Contoso India</span></span>|<span data-ttu-id="1ed52-146">באתר</span><span class="sxs-lookup"><span data-stu-id="1ed52-146">Onsite</span></span>            |                    |<span data-ttu-id="1ed52-147">שעות נוספות</span><span class="sxs-lookup"><span data-stu-id="1ed52-147">Overtime</span></span>                 |<span data-ttu-id="1ed52-148">15</span><span class="sxs-lookup"><span data-stu-id="1ed52-148">15</span></span>     |
|             | <span data-ttu-id="1ed52-149">Contoso India</span><span class="sxs-lookup"><span data-stu-id="1ed52-149">Contoso India</span></span>|<span data-ttu-id="1ed52-150">מקומי</span><span class="sxs-lookup"><span data-stu-id="1ed52-150">Local</span></span>             |                    |<span data-ttu-id="1ed52-151">שעות נוספות</span><span class="sxs-lookup"><span data-stu-id="1ed52-151">Overtime</span></span>                 |<span data-ttu-id="1ed52-152">10</span><span class="sxs-lookup"><span data-stu-id="1ed52-152">10</span></span>     |
|             | <span data-ttu-id="1ed52-153">Contoso US</span><span class="sxs-lookup"><span data-stu-id="1ed52-153">Contoso US</span></span>   |<span data-ttu-id="1ed52-154">מקומי</span><span class="sxs-lookup"><span data-stu-id="1ed52-154">Local</span></span>             |                    |<span data-ttu-id="1ed52-155">שעות נוספות</span><span class="sxs-lookup"><span data-stu-id="1ed52-155">Overtime</span></span>                 |<span data-ttu-id="1ed52-156">20</span><span class="sxs-lookup"><span data-stu-id="1ed52-156">20</span></span>     |


<span data-ttu-id="1ed52-157">אם משאב מ- Contoso India, שתעריף הבסיס שלו הוא ‎,100 USD עובד באתר ומבצע רישום של 8 שעות עבודה רגילות ו- 2 שעות נוספות בערך הזמן, מנגנון התמחור ישתמש בתעריף הבסיס של 100 עבור 8 השעות כדי לרשום ‎800 USD.</span><span class="sxs-lookup"><span data-stu-id="1ed52-157">If a resource from Contoso India whose base rate is 100 USD is working onsite, and they log 8 hours of Regular time and 2 hours of overtime on the time entry, the pricing engine will use the base rate of 100 for the 8 hours to record 800 USD.</span></span> <span data-ttu-id="1ed52-158">לגבי 2 השעות הנוספות יחול ייקור של 15% על תעריף הבסיס של 100 כדי לקבל מחיר יחידה של ‎115 USD ותירשם עלות כוללת של ‎230 USD.</span><span class="sxs-lookup"><span data-stu-id="1ed52-158">For the 2 hours overtime, a markup of 15% will be applied to the base rate of 100 to get a unit price of 115 USD and will record a total cost of 230 USD.</span></span>

### <a name="applicable-to-cost"></a><span data-ttu-id="1ed52-159">חל על עלות</span><span class="sxs-lookup"><span data-stu-id="1ed52-159">Applicable to Cost</span></span> 
<span data-ttu-id="1ed52-160">אם ערך זה מוגדר ל **כן**, פירוש הדבר שיש להשתמש בערך הממד מהקשר הקלט כדי להתאים ל **מחיר תפקיד** ול **ייקור מחיר תפקיד** בעת אחזור תעריפי העלות והייקור.</span><span class="sxs-lookup"><span data-stu-id="1ed52-160">If this is set to **Yes**, it indicates that the dimension value from the input context should be used to match to the **Role Price** and **Role Price Markup** when retrieving the cost and markup rates.</span></span>

### <a name="applicable-to-sales"></a><span data-ttu-id="1ed52-161">חל על מכירות</span><span class="sxs-lookup"><span data-stu-id="1ed52-161">Applicable to Sales</span></span>
<span data-ttu-id="1ed52-162">אם ערך זה מוגדר ל **כן**, פירוש הדבר שיש להשתמש בערך הממד מהקשר הקלט כדי להתאים ל **מחיר תפקיד** ול **ייקור מחיר תפקיד** בעת אחזור תעריפי החיוב והייקור.</span><span class="sxs-lookup"><span data-stu-id="1ed52-162">If this is set to **Yes**, it indicates that the dimension value from the input context should be used to match to the **Role Price** and **Role Price Markup** when retrieving the bill and markup rates.</span></span>

### <a name="applicable-to-purchase"></a><span data-ttu-id="1ed52-163">חל על רכישה</span><span class="sxs-lookup"><span data-stu-id="1ed52-163">Applicable to Purchase</span></span>
<span data-ttu-id="1ed52-164">אם ערך זה מוגדר ל **כן**, פירוש הדבר שיש להשתמש בערך הממד מהקשר הקלט כדי להתאים ל **מחיר תפקיד** ול **ייקור מחיר תפקיד** בעת אחזור מחיר הרכישה.</span><span class="sxs-lookup"><span data-stu-id="1ed52-164">If this is set to **Yes**, it indicates that the dimension value from the input context should be used to match to the **Role Price** and **Role Price Markup** when retrieving the purchase price.</span></span> <span data-ttu-id="1ed52-165">תרחישי קבלנות-משנה אינם נתמכים, ולכן לא נעשה שימוש בשדה זה.</span><span class="sxs-lookup"><span data-stu-id="1ed52-165">Subcontracting scenarios are not supported, so this field is not used.</span></span> 

### <a name="priority"></a><span data-ttu-id="1ed52-166">עדיפות</span><span class="sxs-lookup"><span data-stu-id="1ed52-166">Priority</span></span>
<span data-ttu-id="1ed52-167">הגדרת עדיפות הממד עוזרת לתמחור להפיק מחיר גם כשהוא לא יכול למצוא התאמה מדויקת בין ערכי ממד הקלט לערכים מן הטבלאות **מחיר תפקיד** או **ייקור מחיר תפקיד**.</span><span class="sxs-lookup"><span data-stu-id="1ed52-167">Setting the dimension priority helps pricing produce a price even when it can't find an exact match between the input dimension values and the values from the **Role Price** or **Role Price Markup** tables.</span></span> <span data-ttu-id="1ed52-168">בתרחיש זה נעשה שימוש בערכי Null עבור ערכי ממד לא תואמים על-ידי שקלול הממדים לפי סדרי העדיפויות שלהם.</span><span class="sxs-lookup"><span data-stu-id="1ed52-168">In this scenario, null values are used for unmatched dimension values by weighing the dimensions in order of their priority.</span></span>

- <span data-ttu-id="1ed52-169">**עדיפות עלות**: הערך עדיפות עלות של ממד יציין את המשקל של ממד זה בעת התאמתו להגדרת מחירי העלות.</span><span class="sxs-lookup"><span data-stu-id="1ed52-169">**Cost Priority**: The value of a dimension's cost priority will indicate the weight of that dimension when matching against the setup of cost prices.</span></span> <span data-ttu-id="1ed52-170">הערך של **עדיפות עלות** חייב להיות ייחודי בין ממדים שהערך שלהם **חל על עלות**.</span><span class="sxs-lookup"><span data-stu-id="1ed52-170">The value of **Cost Priority** must be unique across dimensions that are **Applicable to Cost**.</span></span>
- <span data-ttu-id="1ed52-171">**עדיפות מכירות**: הערך עדיפות מכירות של ממד יציין את המשקל של ממד זה בעת התאמתו להגדרת מחירי המכירות או תעריפי החיוב.</span><span class="sxs-lookup"><span data-stu-id="1ed52-171">**Sales Priority**: The value of dimension's sales priority will indicate the weight of that dimension when matching against the setup of sales prices or bill rates.</span></span> <span data-ttu-id="1ed52-172">הערך של **עדיפות מכירות** חייב להיות ייחודי בין ממדים שהערך שלהם **חל על מכירות**.</span><span class="sxs-lookup"><span data-stu-id="1ed52-172">The value of **Sales Priority** must be unique across dimensions that are **Applicable to Sales**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]