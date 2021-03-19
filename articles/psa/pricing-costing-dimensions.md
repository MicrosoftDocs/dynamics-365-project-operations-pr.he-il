---
title: דף הבית לממדי תמחור ותמחיר
description: נושא זה מספק מבט כולל על ממדי תמחור.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
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
ms.openlocfilehash: 137fee27dd2302d47ae12faccde1682cff43db93
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5284134"
---
# <a name="pricing-and-costing-dimensions-home-page"></a><span data-ttu-id="16cfd-103">דף הבית לממדי תמחור ותמחיר</span><span class="sxs-lookup"><span data-stu-id="16cfd-103">Pricing and costing dimensions home page</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="16cfd-104">הממדים המשמשים לקביעת תמחור עבודה ועלות בארגונים מבוססי פרויקטים מושפעים מהתכונות הבאות:</span><span class="sxs-lookup"><span data-stu-id="16cfd-104">The dimensions used to set labor pricing and costing in project-based organizations are influenced by the following attributes:</span></span>

- <span data-ttu-id="16cfd-105">אנשים שעושים עבודה הדומה לניסיון, לתפקיד או למיקום הגיאוגרפי שלהם</span><span class="sxs-lookup"><span data-stu-id="16cfd-105">People doing work similar to their experience, role, or geography</span></span>
- <span data-ttu-id="16cfd-106">עבודה שתתבצע בדומה למורכבותה או לשעה ביום</span><span class="sxs-lookup"><span data-stu-id="16cfd-106">Work to be performed similar to its complexity or time of day</span></span>

<span data-ttu-id="16cfd-107">בהתחשב במה שמאפיין תכונות אלה של העבודה והאנשים הנדרשים לביצוע העבודה, ישנם שני סוגים של ערכי ממד תמחור שזמינים ב- Project Service Automation:</span><span class="sxs-lookup"><span data-stu-id="16cfd-107">Given the typical nature of these attrubutes of the work and the people required to perform the work, there are two types of pricing dimension values available in Project Service Automation:</span></span> 

- <span data-ttu-id="16cfd-108">**קבוצות של אפשרויות** - ממדים שהם ספירות קבועות עבור קבוצת ערכים.</span><span class="sxs-lookup"><span data-stu-id="16cfd-108">**Option sets** - Attributes that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="16cfd-109">**ערכים מבוססי ישויות** - תכונות שיכולות לכלול סט ערכים שונה אך סופי יכולות להשתנות לאורך זמן.</span><span class="sxs-lookup"><span data-stu-id="16cfd-109">**Entity-based values** - Attributes that can have a varied set of values that are finite but can change over time.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="16cfd-110">ממדי תמחור</span><span class="sxs-lookup"><span data-stu-id="16cfd-110">Pricing dimensions</span></span>

<span data-ttu-id="16cfd-111">PSA מסופק עם קבוצה של ממדי תמחור בברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="16cfd-111">PSA ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="16cfd-112">תוכל להציג אותם על-ידי מעבר אל **Project Service** > **פרמטרים**.</span><span class="sxs-lookup"><span data-stu-id="16cfd-112">You can view these by going to **Project Service** > **Parameters**.</span></span> <span data-ttu-id="16cfd-113">ברשומת הפרמטר, בכרטיסיה **‬‏‫ממדי תמחור מבוססי-כמות**, ודא שבתפקיד, **msdyn_resourcecategory** וביחידה הארגונית להקצאת משאבים, **msdyn_organizationalunit** השדה **‏‫חל על מכירות‬** והשדה **‏‫חל על עלות‬** מוגדרים בתור **כן**.</span><span class="sxs-lookup"><span data-stu-id="16cfd-113">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="16cfd-114">כך תוכל להגדיר את המחיר ואת העלות עבור כל שילוב של תפקיד ויחידה ארגונית.</span><span class="sxs-lookup"><span data-stu-id="16cfd-114">This will allow you to set up the price and cost for each role and organizational unit combination.</span></span>

![צילום מסך של פרמטרי Project Service כאשר "חל על מכירות" מודגש](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> <span data-ttu-id="16cfd-116">אם השתמשת בשדות המוכנים לשימוש של תפקיד ויחידה ארגונית כממדי תמחור לפי גירסה 3 של PSA, לא יהיו שינויים נראים לעין.</span><span class="sxs-lookup"><span data-stu-id="16cfd-116">If you have been the using out-of-the box fields of role and organizational unit as pricing dimensions prior to version 3 of PSA, there will not be any observable change.</span></span> <span data-ttu-id="16cfd-117">באפשרותך להמשיך להשתמש ב- Project Service כרגיל.</span><span class="sxs-lookup"><span data-stu-id="16cfd-117">You can continue to use Project Service as usual.</span></span> 

<span data-ttu-id="16cfd-118">אם אתה צריך מחיר או עלות עבור המשאבים שלך באמצעות תכונות נוספות, תוכל ליצור שדות, ישויות וממדים מותאמים אישית.</span><span class="sxs-lookup"><span data-stu-id="16cfd-118">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="16cfd-119">לקבלת מידע נוסף, עיין בנושאים הבאים, אך שים לב שעליך להשלים את ההליכים בסדר המפורט להלן:</span><span class="sxs-lookup"><span data-stu-id="16cfd-119">For more information, see the following topics, however note that you must complete the procedures in the order listed below:</span></span>

- [<span data-ttu-id="16cfd-120">יצירת שדות וישויות מותאמים אישית</span><span class="sxs-lookup"><span data-stu-id="16cfd-120">Create custom fields and entities</span></span>](create-custom-fields-entities.md)
- [<span data-ttu-id="16cfd-121">הוספת שדות מותאמים אישית להגדרת מחיר וישויות של טרנזקציות</span><span class="sxs-lookup"><span data-stu-id="16cfd-121">Add custom fields to price setup and transactional entities</span></span>](field-references.md)
- [<span data-ttu-id="16cfd-122">הגדרת שדות מותאמים אישית כממדי תמחור </span><span class="sxs-lookup"><span data-stu-id="16cfd-122">Set up custom fields as pricing dimensions</span></span>](set-up-pricing-dimensions.md)
- [<span data-ttu-id="16cfd-123">עדכון תכונות של יישום Plug-in כדי לכלול ממדי תמחור חדשים</span><span class="sxs-lookup"><span data-stu-id="16cfd-123">Update plug-in attributes to include new pricing dimensions</span></span>](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a><span data-ttu-id="16cfd-124">תמחור זמן של משאב אנושי</span><span class="sxs-lookup"><span data-stu-id="16cfd-124">Pricing human resource time</span></span>
<span data-ttu-id="16cfd-125">כיצד ארגון מתמחר זמן של משאב אנושי הוא לרוב שיקול אסטרטגי חשוב שמשפיע ישירות על רווחיות הארגון.</span><span class="sxs-lookup"><span data-stu-id="16cfd-125">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="16cfd-126">עבוד עם הצוותים הפיננסיים וראשי אגפים כאשר הארגון שלך מוכן לזהות כיצד הוא מעוניין להגדיר את תעריפי עלויות וחיוב עבור הזמן של המשאב האנושי.</span><span class="sxs-lookup"><span data-stu-id="16cfd-126">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="16cfd-127">שיקולים אחרים לתמחור כוללים אם להשתמש מחדש בשדות או בישויות שאינם כרגע ממדי תמחור, אך מוחלים כממד תמחור עבור הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="16cfd-127">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="16cfd-128">שדות כמו **קטגוריית עסקה** (**msdyn_transactioncategory**) ו **משאב ניתן להזמנה** (**bookableresource**) הם דוגמאות לממדים מועמדים.</span><span class="sxs-lookup"><span data-stu-id="16cfd-128">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="16cfd-129">כדאי לשקול גם אם ממד התמחור שלך צריך להיות טבלה או קבוצת אפשרויות.</span><span class="sxs-lookup"><span data-stu-id="16cfd-129">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="16cfd-130">אם אתה צופה שינויים בערכים של ממד שיחרוג מ- 10 או 12 ואתה זקוק לתכונות נוספות בערכים אלה, תוכל ליצור ישות במקום קבוצת אפשרויות.</span><span class="sxs-lookup"><span data-stu-id="16cfd-130">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, create an entity rather than an option set.</span></span> <span data-ttu-id="16cfd-131">תחזוקה של קבוצת אפשרויות, כגון הוספה או הסרה של ערכים, מחייבת מנהל מערכת או מפתח בעוד שהוספת שורות חדשות לטבלה יכולה להתבצע על-ידי רוב המשתמשים העסקיים.</span><span class="sxs-lookup"><span data-stu-id="16cfd-131">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most business users.</span></span>

<span data-ttu-id="16cfd-132">הדוגמה הבאה מציגה את תעריפי החיוב שמוגדרים בהתאם לתפקיד וליחידה הארגונית להקצאת משאבים שאליה המשאב שייך.</span><span class="sxs-lookup"><span data-stu-id="16cfd-132">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="16cfd-133">תעריפי עלויות מבוססים בדרך כלל על טווח השכר של העובד ועל היחידה הארגונית שאליה הוא שייך.</span><span class="sxs-lookup"><span data-stu-id="16cfd-133">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="16cfd-134">בדוגמה זו, הטבלאות של תעריף החיוב ותעריף העלויות ייראו כך.</span><span class="sxs-lookup"><span data-stu-id="16cfd-134">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="16cfd-135">**תעריפי חיוב לדוגמה**</span><span class="sxs-lookup"><span data-stu-id="16cfd-135">**Sample bill rates**</span></span>

| <span data-ttu-id="16cfd-136">תפקיד</span><span class="sxs-lookup"><span data-stu-id="16cfd-136">Role</span></span>        | <span data-ttu-id="16cfd-137">יחידה ארגונית</span><span class="sxs-lookup"><span data-stu-id="16cfd-137">Org Unit</span></span>    |<span data-ttu-id="16cfd-138">יחידה</span><span class="sxs-lookup"><span data-stu-id="16cfd-138">Unit</span></span>      |<span data-ttu-id="16cfd-139">מחיר</span><span class="sxs-lookup"><span data-stu-id="16cfd-139">Price</span></span>      |<span data-ttu-id="16cfd-140">מטבע</span><span class="sxs-lookup"><span data-stu-id="16cfd-140">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="16cfd-141">מפתח</span><span class="sxs-lookup"><span data-stu-id="16cfd-141">Developer</span></span>   | <span data-ttu-id="16cfd-142">Contoso US</span><span class="sxs-lookup"><span data-stu-id="16cfd-142">Contoso US</span></span>  |<span data-ttu-id="16cfd-143">Hour</span><span class="sxs-lookup"><span data-stu-id="16cfd-143">Hour</span></span> | <span data-ttu-id="16cfd-144">200</span><span class="sxs-lookup"><span data-stu-id="16cfd-144">200</span></span>|<span data-ttu-id="16cfd-145">USD</span><span class="sxs-lookup"><span data-stu-id="16cfd-145">USD</span></span>     |
| <span data-ttu-id="16cfd-146">מפתח</span><span class="sxs-lookup"><span data-stu-id="16cfd-146">Developer</span></span>   | <span data-ttu-id="16cfd-147">Contoso India</span><span class="sxs-lookup"><span data-stu-id="16cfd-147">Contoso India</span></span> |<span data-ttu-id="16cfd-148">Hour</span><span class="sxs-lookup"><span data-stu-id="16cfd-148">Hour</span></span>|   <span data-ttu-id="16cfd-149">112</span><span class="sxs-lookup"><span data-stu-id="16cfd-149">112</span></span>|<span data-ttu-id="16cfd-150">USD</span><span class="sxs-lookup"><span data-stu-id="16cfd-150">USD</span></span>     |


<span data-ttu-id="16cfd-151">**תעריפי עלויות לדוגמה**</span><span class="sxs-lookup"><span data-stu-id="16cfd-151">**Sample cost rates**</span></span>

| <span data-ttu-id="16cfd-152">טווח שכר</span><span class="sxs-lookup"><span data-stu-id="16cfd-152">Salary Band</span></span>     | <span data-ttu-id="16cfd-153">יחידה ארגונית</span><span class="sxs-lookup"><span data-stu-id="16cfd-153">Org Unit</span></span>    |<span data-ttu-id="16cfd-154">יחידה</span><span class="sxs-lookup"><span data-stu-id="16cfd-154">Unit</span></span>      |<span data-ttu-id="16cfd-155">מחיר</span><span class="sxs-lookup"><span data-stu-id="16cfd-155">Price</span></span>      |<span data-ttu-id="16cfd-156">מטבע</span><span class="sxs-lookup"><span data-stu-id="16cfd-156">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="16cfd-157">טווח1_של החברה שלי</span><span class="sxs-lookup"><span data-stu-id="16cfd-157">My company_Band1</span></span> | <span data-ttu-id="16cfd-158">Contoso US</span><span class="sxs-lookup"><span data-stu-id="16cfd-158">Contoso US</span></span>  |<span data-ttu-id="16cfd-159">Hour</span><span class="sxs-lookup"><span data-stu-id="16cfd-159">Hour</span></span> | <span data-ttu-id="16cfd-160">145</span><span class="sxs-lookup"><span data-stu-id="16cfd-160">145</span></span>|<span data-ttu-id="16cfd-161">USD</span><span class="sxs-lookup"><span data-stu-id="16cfd-161">USD</span></span>     |
| <span data-ttu-id="16cfd-162">טווח2_של החברה שלי</span><span class="sxs-lookup"><span data-stu-id="16cfd-162">My company_Band2</span></span> | <span data-ttu-id="16cfd-163">Contoso India</span><span class="sxs-lookup"><span data-stu-id="16cfd-163">Contoso India</span></span> |<span data-ttu-id="16cfd-164">Hour</span><span class="sxs-lookup"><span data-stu-id="16cfd-164">Hour</span></span>|   <span data-ttu-id="16cfd-165">67</span><span class="sxs-lookup"><span data-stu-id="16cfd-165">67</span></span>|<span data-ttu-id="16cfd-166">USD</span><span class="sxs-lookup"><span data-stu-id="16cfd-166">USD</span></span>     |


[!INCLUDE[footer-include](../includes/footer-banner.md)]