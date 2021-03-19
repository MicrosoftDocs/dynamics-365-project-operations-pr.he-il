---
title: הגדרת שדות מותאמים אישית כממדי תמחור
description: נושא זה מספק מידע אודות הגדרה של ממדי תמחור מותאמים אישית.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/20/2018
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 81f926e0aa209dd83f9b850c2342bd35a4f236c3
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5282469"
---
# <a name="setting-up-custom-fields-as-pricing-dimensions"></a><span data-ttu-id="c3239-103">הגדרת שדות מותאמים אישית כממדי תמחור</span><span class="sxs-lookup"><span data-stu-id="c3239-103">Setting up custom fields as pricing dimensions</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="c3239-104">לפני שתתחיל, נושא זה יוצא מנקודת הנחה שהשלמת את ההליכים בנושאים [יצירת שדות וישויות מותאמים אישית](create-custom-fields-entities.md) ו[הוספת שדות מותאמים אישית להגדרת מחיר וישויות של טרנזקציות](field-references.md).</span><span class="sxs-lookup"><span data-stu-id="c3239-104">Before you begin, this topic assumes that you have completed the procedures in the topics, [Create custom fields and entities](create-custom-fields-entities.md) and [Add custom fields to price setup and transactional entities](field-references.md).</span></span> <span data-ttu-id="c3239-105">אם לא השלמת הליכים אלה, חזור והשלם אותם ולאחר מכן חזור לנושא זה.</span><span class="sxs-lookup"><span data-stu-id="c3239-105">If you haven't completed those procedures, go back and complete them and then return to this topic.</span></span> 

<span data-ttu-id="c3239-106">נושא זה מספק מידע אודות הגדרה של ממדי תמחור מותאמים אישית.</span><span class="sxs-lookup"><span data-stu-id="c3239-106">This topic provides information about setting up custom pricing dimensions.</span></span> <span data-ttu-id="c3239-107">בממשק האינטרנט של Project Service, בדף **פרמטרים**, הכרטיסיה ‏‫**ממדי תמחור מבוססי-כמות** מציגה את הרשומות בישויות ממדי התמחור.</span><span class="sxs-lookup"><span data-stu-id="c3239-107">In the Project Service web interface, on the **Parameters** page, the **Amount-Based Pricing Dimensions** tab shows the records in the pricing dimension entities.</span></span> <span data-ttu-id="c3239-108">כברירת מחדל, ההתקנה של Project Service יוצרת 2 שורות ברשת בכרטיסיה זו:</span><span class="sxs-lookup"><span data-stu-id="c3239-108">By default, Project Service installation creates 2 rows in the grid on this tab:</span></span>

- <span data-ttu-id="c3239-109">**msdyn_resourcecategory** (תפקיד)</span><span class="sxs-lookup"><span data-stu-id="c3239-109">**msdyn_resourcecategory** (Role)</span></span>
- <span data-ttu-id="c3239-110">**msdyn_OrganizationalUnit** (יחידה ארגונית)</span><span class="sxs-lookup"><span data-stu-id="c3239-110">**msdyn_OrganizationalUnit** (Organizational Unit)</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c3239-111">אל תמחק שורות אלה.</span><span class="sxs-lookup"><span data-stu-id="c3239-111">Do not delete these rows.</span></span> <span data-ttu-id="c3239-112">עם זאת, אם אינך זקוק להן, ניתן להפוך אותן לבלתי ניתנות להחלה בהקשר מסוים על-ידי הגדרת כל האפשרויות הבאות: **חל על עלות‬**, **חל על מכירות** ו **חל על רכישה** ל **לא**.</span><span class="sxs-lookup"><span data-stu-id="c3239-112">However, if you do not need them, you can make them not applicable in a specific context by setting **Applicable to Cost**, **Applicable to Sales**, and **Applicable to Purchase** all to **No**.</span></span> <span data-ttu-id="c3239-113">הגדרת ערכי התכונות הללו ל **לא** משפיעה באופן זהה לזה שהשדה אינו ממד תמחור.</span><span class="sxs-lookup"><span data-stu-id="c3239-113">Setting these attribute values to **No** has the same effect of not having the field as a pricing dimension.</span></span>

<span data-ttu-id="c3239-114">כדי ששדה יהפוך לממד תמחור, עליו לעמוד בתנאים הבאים:</span><span class="sxs-lookup"><span data-stu-id="c3239-114">For a field to become a pricing dimension, it must be:</span></span>

- <span data-ttu-id="c3239-115">עליו להיווצר כשדה בישויות **מחיר תפקיד** ו **ייקור מחיר תפקיד**.</span><span class="sxs-lookup"><span data-stu-id="c3239-115">Created as a field in the **Role Price** and **Role Price markup** entities.</span></span> <span data-ttu-id="c3239-116">למידע נוסף שבעזרתו תגלה כיצד לעשות זאת, ראה [הוספת שדות מותאמים אישית להגדרת מחיר וישויות של טרנזקציות](field-references.md).</span><span class="sxs-lookup"><span data-stu-id="c3239-116">For more information on how to do this, see [Add custom fields to price setup and transactional entities](field-references.md).</span></span>
- <span data-ttu-id="c3239-117">עליו להיווצר כשורה בטבלה **ממד תמחור**.</span><span class="sxs-lookup"><span data-stu-id="c3239-117">Created as a row in the **Pricing Dimension** table.</span></span> <span data-ttu-id="c3239-118">לדוגמה, הוסף שורות ממד תמחור כמוצג בגרפיקה הבאה.</span><span class="sxs-lookup"><span data-stu-id="c3239-118">For example, add pricing dimension rows as shown in the following graphic.</span></span> 

![שורות ממדי תמחור מבוססי-כמות](media/Amt-based-PD.png)

<span data-ttu-id="c3239-120">שים לב כי שעות העבודה של המשאב (**msdyn_resourceworkhours**) נוספו כממד מבוסס-ייקור ונוספו לרשת בכרטיסיה **ממד תמחור מבוסס-ייקור**.</span><span class="sxs-lookup"><span data-stu-id="c3239-120">Notice that Resource Work hours (**msdyn_resourceworkhours**) has been added as a markup-based dimension and has been added to the grid on the **Markup Based Pricing Dimension** tab.</span></span>

![שורות ממדי תמחור מבוססי-ייקור](media/Markup-based-PD.png)

> [!IMPORTANT]
> <span data-ttu-id="c3239-122">כל שינוי בנתונים של ממד התמחור בטבלה זו, קיים או חדש, מועבר בירושה ללוגיקה העסקית של תמחור Project Service רק לאחר רענון המטמון.</span><span class="sxs-lookup"><span data-stu-id="c3239-122">Any change to pricing dimension data in this table, existing or new, is propagated to the Project Service pricing business logic only after the cache is refreshed.</span></span> <span data-ttu-id="c3239-123">זמן הרענון של המטמון עשוי להימשך עד 10 דקות.</span><span class="sxs-lookup"><span data-stu-id="c3239-123">The cache refresh time may take up to 10 minutes.</span></span> <span data-ttu-id="c3239-124">אפשר פרק זמן זה כדי לראות את השינויים בלוגיקת ברירת המחדל למחיר שעשויה לנבוע משינויים בנתוני ממד התמחור.</span><span class="sxs-lookup"><span data-stu-id="c3239-124">Allow that length of time to see the changes in price defaulting logic that must result from changes to the Pricing Dimension data.</span></span>


## <a name="attributes-of-the-pricing-dimensions-table"></a><span data-ttu-id="c3239-125">תכונות של הטבלה 'ממדי תמחור'</span><span class="sxs-lookup"><span data-stu-id="c3239-125">Attributes of the Pricing Dimensions table</span></span>
<span data-ttu-id="c3239-126">הסעיפים הבאים מספקים מידע אודות התכונות השונות בטבלה **ממדי תמחור**.</span><span class="sxs-lookup"><span data-stu-id="c3239-126">The following sections provide information about the different attributes in the **Pricing Dimensions** table.</span></span>

### <a name="pricing-dimension-name"></a><span data-ttu-id="c3239-127">שם ממד התמחור</span><span class="sxs-lookup"><span data-stu-id="c3239-127">Pricing Dimension Name</span></span>
<span data-ttu-id="c3239-128">ערך זה צריך להיות זהה לגמרי לשם הסכימה של השדה שנוסף לטבלה **מחיר תפקיד** עבור ממדי תמחור מותאמים אישית.</span><span class="sxs-lookup"><span data-stu-id="c3239-128">This value should be the exact same as the schema name of the field that is added to the **Role Price** table for custom pricing dimensions.</span></span> <span data-ttu-id="c3239-129">לקבלת מידע נוסף אודות הוספת שדות לטבלה **מחיר תפקיד**, ראה [‬‏‫הוספת שדות מותאמים אישית להגדרת מחיר וישויות של טרנזקציות](field-references.md).</span><span class="sxs-lookup"><span data-stu-id="c3239-129">For more information about adding fields to the **Role Price** table, see [Add custom fields to price setup and transactional entities](field-references.md).</span></span>

### <a name="type-of-dimension"></a><span data-ttu-id="c3239-130">סוג ממד</span><span class="sxs-lookup"><span data-stu-id="c3239-130">Type of dimension</span></span>
<span data-ttu-id="c3239-131">קיימים שני סוגים של ממדי תמחור:</span><span class="sxs-lookup"><span data-stu-id="c3239-131">There are two types of pricing dimensions:</span></span>
  
  - <span data-ttu-id="c3239-132">**ממדים מבוססי-כמות**: ערכי הממד מהקשר הקלט מותאמים לערכי הממד בשורה **מחיר תפקיד** והמחיר/העלות מוגדרים כברירת מחדל ישירות מהטבלה **מחיר תפקיד**.</span><span class="sxs-lookup"><span data-stu-id="c3239-132">**Amount-based dimensions**: The dimension values from the input context are matched to the dimension values on **Role Price** line and the price/cost is defaulted directly from the **Role Price** table.</span></span>
  - <span data-ttu-id="c3239-133">**ממדים מבוססי-ייקור**: אלה הם ממדים שבהם Project Service יאמץ את תהליך שלושת השלבים הבא כדי לקבל את המחיר/העלות</span><span class="sxs-lookup"><span data-stu-id="c3239-133">**Markup-based dimensions**: These are dimensions where Project Service will adopt the following 3-step process to get the price/cost</span></span>
 
    1. <span data-ttu-id="c3239-134">Project Service מתאים את ערכי הממד שאינו מבוסס-ייקור מהקשר הקלט לשורה 'מחיר תפקיד' כדי לקבל את תעריף הבסיס.</span><span class="sxs-lookup"><span data-stu-id="c3239-134">Project Service matches the non-markup-based dimension values from the input context to the Role Price line to get the base rate.</span></span>
    2. <span data-ttu-id="c3239-135">Project Service מתאים את כל ערכי הממד מהקשר הקלט לשורה **ייקור מחיר תפקיד** כדי לקבל אחוז ייקור.</span><span class="sxs-lookup"><span data-stu-id="c3239-135">Project Service matches all of the dimension values from the input context to the **Role Price Markup** line to get a markup percentage.</span></span>
    3. <span data-ttu-id="c3239-136">Project Service מחיל את אחוז הייקור מהשלב השני על תעריף הבסיס שהושג מן הטבלה **מחיר תפקיד** בשלב הראשון כדי להגיע למחיר/עלות סופיים.</span><span class="sxs-lookup"><span data-stu-id="c3239-136">Project Service applies the markup percentage from the second step to the base rate obtained from the **Role Price** table in the first step to arrive at final price/cost.</span></span>
   
   <span data-ttu-id="c3239-137">הטבלה הבאה מתארת את החישוב של ייקורי מחירים.</span><span class="sxs-lookup"><span data-stu-id="c3239-137">The following table illustrates the calculation of price markups.</span></span>
  
| <span data-ttu-id="c3239-138">תפקיד</span><span class="sxs-lookup"><span data-stu-id="c3239-138">Role</span></span>        | <span data-ttu-id="c3239-139">יחידה ארגונית</span><span class="sxs-lookup"><span data-stu-id="c3239-139">Org Unit</span></span>    |<span data-ttu-id="c3239-140">מיקום עבודה</span><span class="sxs-lookup"><span data-stu-id="c3239-140">Work Location</span></span>      |<span data-ttu-id="c3239-141">כותרת סטנדרטית</span><span class="sxs-lookup"><span data-stu-id="c3239-141">Standard Title</span></span>      |<span data-ttu-id="c3239-142">שעות עבודה של משאב</span><span class="sxs-lookup"><span data-stu-id="c3239-142">Resource Work Hours</span></span>      |  <span data-ttu-id="c3239-143">ייקור</span><span class="sxs-lookup"><span data-stu-id="c3239-143">Mark Up</span></span>|
| ------------|-------------|-------------------|--------------------|-------------------------|--------:|
|             | <span data-ttu-id="c3239-144">Contoso India</span><span class="sxs-lookup"><span data-stu-id="c3239-144">Contoso India</span></span>|<span data-ttu-id="c3239-145">באתר</span><span class="sxs-lookup"><span data-stu-id="c3239-145">Onsite</span></span>            |                    |<span data-ttu-id="c3239-146">שעות נוספות</span><span class="sxs-lookup"><span data-stu-id="c3239-146">Overtime</span></span>                 |<span data-ttu-id="c3239-147">15</span><span class="sxs-lookup"><span data-stu-id="c3239-147">15</span></span>     |
|             | <span data-ttu-id="c3239-148">Contoso India</span><span class="sxs-lookup"><span data-stu-id="c3239-148">Contoso India</span></span>|<span data-ttu-id="c3239-149">מקומי</span><span class="sxs-lookup"><span data-stu-id="c3239-149">Local</span></span>             |                    |<span data-ttu-id="c3239-150">שעות נוספות</span><span class="sxs-lookup"><span data-stu-id="c3239-150">Overtime</span></span>                 |<span data-ttu-id="c3239-151">10</span><span class="sxs-lookup"><span data-stu-id="c3239-151">10</span></span>     |
|             | <span data-ttu-id="c3239-152">Contoso US</span><span class="sxs-lookup"><span data-stu-id="c3239-152">Contoso US</span></span>   |<span data-ttu-id="c3239-153">מקומי</span><span class="sxs-lookup"><span data-stu-id="c3239-153">Local</span></span>             |                    |<span data-ttu-id="c3239-154">שעות נוספות</span><span class="sxs-lookup"><span data-stu-id="c3239-154">Overtime</span></span>                 |<span data-ttu-id="c3239-155">20</span><span class="sxs-lookup"><span data-stu-id="c3239-155">20</span></span>     |


<span data-ttu-id="c3239-156">אם משאב מ- Contoso India, שתעריף הבסיס שלו הוא ‎,100 USD עובד באתר ומבצע רישום של 8 שעות עבודה רגילות ו- 2 שעות נוספות בערך הזמן, מנגנון התמחור של Project Service ישתמש בתעריף הבסיס של 100 עבור 8 השעות כדי לרשום ‎800 USD.</span><span class="sxs-lookup"><span data-stu-id="c3239-156">If a resource from Contoso India whose base rate is 100 USD is working onsite, and they log 8 hours of Regular time and 2 hours of overtime on the time entry, the Project Service pricing engine will use the base rate of 100 for the 8 hours to record 800 USD.</span></span> <span data-ttu-id="c3239-157">לגבי 2 השעות הנוספות יחול ייקור של 15% על תעריף הבסיס של 100 כדי לקבל מחיר יחידה של ‎115 USD ותירשם עלות כוללת של ‎230 USD.</span><span class="sxs-lookup"><span data-stu-id="c3239-157">For the 2 hours overtime, a markup of 15% will be applied to the base rate of 100 to get a unit price of 115 USD and will record a total cost of 230 USD.</span></span>

### <a name="applicable-to-cost"></a><span data-ttu-id="c3239-158">חל על עלות</span><span class="sxs-lookup"><span data-stu-id="c3239-158">Applicable to Cost</span></span> 
<span data-ttu-id="c3239-159">אם ערך זה מוגדר ל **כן**, פירוש הדבר שיש להשתמש בערך הממד מהקשר הקלט כדי להתאים ל **מחיר תפקיד** ול **ייקור מחיר תפקיד** בעת אחזור תעריפי העלות והייקור.</span><span class="sxs-lookup"><span data-stu-id="c3239-159">If this is set to **Yes**, it indicates that the dimension value from the input context should be used to match to the **Role Price** and **Role Price Markup** when retrieving the cost and markup rates.</span></span>

### <a name="applicable-to-sales"></a><span data-ttu-id="c3239-160">חל על מכירות</span><span class="sxs-lookup"><span data-stu-id="c3239-160">Applicable to Sales</span></span>
<span data-ttu-id="c3239-161">אם ערך זה מוגדר ל **כן**, פירוש הדבר שיש להשתמש בערך הממד מהקשר הקלט כדי להתאים ל **מחיר תפקיד** ול **ייקור מחיר תפקיד** בעת אחזור תעריפי החיוב והייקור.</span><span class="sxs-lookup"><span data-stu-id="c3239-161">If this is set to **Yes**, it indicates that the dimension value from the input context should be used to match to the **Role Price** and **Role Price Markup** when retrieving the bill and markup rates.</span></span>

### <a name="applicable-to-purchase"></a><span data-ttu-id="c3239-162">חל על רכישה</span><span class="sxs-lookup"><span data-stu-id="c3239-162">Applicable to Purchase</span></span>
<span data-ttu-id="c3239-163">אם ערך זה מוגדר ל **כן**, פירוש הדבר שיש להשתמש בערך הממד מהקשר הקלט כדי להתאים ל **מחיר תפקיד** ול **ייקור מחיר תפקיד** בעת אחזור מחיר הרכישה.</span><span class="sxs-lookup"><span data-stu-id="c3239-163">If this is set to **Yes**, it indicates that the dimension value from the input context should be used to match to the **Role Price** and **Role Price Markup** when retrieving the purchase price.</span></span> <span data-ttu-id="c3239-164">בשלב זה, Project Service אינו תומך בתרחישים של קבלנות משנה, כך שלא נעשה שימוש בשדה זה.</span><span class="sxs-lookup"><span data-stu-id="c3239-164">Currently Project Service does not support subcontracting scenarios, so this field is not used.</span></span> 

### <a name="priority"></a><span data-ttu-id="c3239-165">עדיפות</span><span class="sxs-lookup"><span data-stu-id="c3239-165">Priority</span></span>
<span data-ttu-id="c3239-166">הגדרת עדיפות הממד עוזרת לתמחור של Project Service להפיק מחיר גם כשהוא לא יכול למצוא התאמה מדויקת בין ערכי ממד הקלט לערכים מן הטבלאות **מחיר תפקיד** או **ייקור מחיר תפקיד**.</span><span class="sxs-lookup"><span data-stu-id="c3239-166">Setting the dimension priority helps Project Service pricing produce a price even when it can't find an exact match between the input dimension values and the values from the **Role Price** or **Role Price Markup** tables.</span></span> <span data-ttu-id="c3239-167">בתרחיש זה, Project Service ישתמש בערכי Null עבור ערכי ממד לא תואמים על-ידי שקלול הממדים לפי סדרי העדיפויות שלהם.</span><span class="sxs-lookup"><span data-stu-id="c3239-167">In this scenario, Project Service will use null values for unmatched dimension values by weighing the dimensions in order of their priority.</span></span>

- <span data-ttu-id="c3239-168">**עדיפות עלות**: הערך עדיפות עלות של ממד יציין את המשקל של ממד זה בעת התאמתו להגדרת מחירי העלות.</span><span class="sxs-lookup"><span data-stu-id="c3239-168">**Cost Priority**: The value of a dimension's cost priority will indicate the weight of that dimension when matching against the setup of cost prices.</span></span> <span data-ttu-id="c3239-169">הערך של **עדיפות עלות** חייב להיות ייחודי בין ממדים שהערך שלהם **חל על עלות**.</span><span class="sxs-lookup"><span data-stu-id="c3239-169">The value of **Cost Priority** must be unique across dimensions that are **Applicable to Cost**.</span></span>
- <span data-ttu-id="c3239-170">**עדיפות מכירות**: הערך עדיפות מכירות של ממד יציין את המשקל של ממד זה בעת התאמתו להגדרת מחירי המכירות או תעריפי החיוב.</span><span class="sxs-lookup"><span data-stu-id="c3239-170">**Sales Priority**: The value of dimension's sales priority will indicate the weight of that dimension when matching against the setup of sales prices or bill rates.</span></span> <span data-ttu-id="c3239-171">הערך של **עדיפות מכירות** חייב להיות ייחודי בין ממדים שהערך שלהם **חל על מכירות**.</span><span class="sxs-lookup"><span data-stu-id="c3239-171">The value of **Sales Priority** must be unique across dimensions that are **Applicable to Sales**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]