---
title: יצירת שדות וישויות מותאמים אישית
description: נושא זה מסביר כיצד ליצור קבוצות אפשרויות וישויות בפתרון שלך בפלטפורמת Power Apps.
author: Rumant
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
ms.openlocfilehash: 442ff9cf2206bec307cea7ff30b9266502d8f77b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077377"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="6a3f3-103">יצירת שדות וישויות מותאמים אישית</span><span class="sxs-lookup"><span data-stu-id="6a3f3-103">Create custom fields and entities</span></span> 

<span data-ttu-id="6a3f3-104">בצע את השלבים הבאים בכל עת שברצונך ליצור קבוצת אפשרויות או ישות מותאמת אישית בפלטפורמת Power Apps.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="6a3f3-105">יש להשלים את ההליכים בנושא זה באמצעות ממשק האינטרנט של Project Service Automation‏ (PSA).</span><span class="sxs-lookup"><span data-stu-id="6a3f3-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="6a3f3-106">מומלץ לבצע את כל השינויים בממד התמחור המותאם אישית בפתרון נפרד.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="6a3f3-107">שיטת עבודה מומלצת וחשובה זו מספקת גמישות בעתיד כדי לעדכן או להסיר שינויים בהתאם לצורך, היא תסייע לך להשתמש מחדש בעבודתך ומאפשרת להפנות את השינויים הללו אל מופע אחר בקלות רבה יותר.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="6a3f3-108">לאחר שביצעת את כל השינויים הדרושים, יצא פתרון זה כ **פתרון מנוהל** ויבא אותו אל מופעים אחרים כדי להשתמש שוב בהגדרת התמחור.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="6a3f3-109">יצור שדות וקבוצות אפשרויות מותאמים אישית בפתרון ממד התמחור</span><span class="sxs-lookup"><span data-stu-id="6a3f3-109">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="6a3f3-110">ממד תמחור יכול להיות קבוצת אפשרויות או ישות.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-110">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="6a3f3-111">יש ליצור את שתיהן בפתרון התמחור.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-111">Both must be created in your pricing solution.</span></span> <span data-ttu-id="6a3f3-112">השלבים בהליך זה מסבירים כיצד ליצור ממדים מבוססי-ישות וממדים מבוססי-קבוצת אפשרויות.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-112">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="6a3f3-113">ממדים מבוססי-ישות</span><span class="sxs-lookup"><span data-stu-id="6a3f3-113">Entity-based dimensions</span></span>

1. <span data-ttu-id="6a3f3-114">ב-PSA, בחר **הגדרות** > **פתרונות** ולחץ פעמיים על **\<your organization name> ממדי תמחור**.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-114">In PSA, click **Settings** > **Solutions** , and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="6a3f3-115">בסייר הפתרונות, בחלונית הניווט הימנית, בחר **ישויות**.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-115">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="6a3f3-116">לחץ על **חדש** כדי ליצור ישות חדשה בשם **כותרת סטנדרטית**.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-116">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="6a3f3-117">הזן את המידע הדרוש שנותר ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-117">Enter the remaining required information, and then click **Save**.</span></span>

> ![הגדרת ישות של כותרת סטנדרטית](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="6a3f3-119">ממדים מבוססי-קבוצת אפשרויות</span><span class="sxs-lookup"><span data-stu-id="6a3f3-119">Option set-based dimensions</span></span> 
<span data-ttu-id="6a3f3-120">באפשרותך ליצור שני ממדים מבוססי-קבוצת אפשרויות.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-120">You can create two option set-based dimensions.</span></span> <span data-ttu-id="6a3f3-121">השתמש באפשרות **מיקום עבודה של משאב** כדי לעקוב אחר המחיר של עבודה במיקום **בית** ועבודה במיקום **באתר** והשתמש באפשרות **שעות עבודה של משאב** עם הערכים **רגיל** ו **שעות נוספות** כדי להחיל ייקור בעת השלמת העבודה.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-121">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="6a3f3-122">ב-PSA, בחר **הגדרות** > **פתרונות** ולחץ פעמיים על **\<your organization name> ממדי תמחור**.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-122">In PSA, click **Settings** > **Solutions** , and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="6a3f3-123">בסייר הפתרונות, בחלונית הניווט הימנית, בחר **קבוצות אפשרויות**.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-123">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="6a3f3-124">לחץ על **חדש** כדי ליצור קבוצת אפשרויות חדשה, הזן את המידע הדרוש שנותר ולחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-124">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="6a3f3-125">ממד תמחור מבוסס-קבוצת אפשרויות הנקרא 'מיקום עבודה של משאב'</span><span class="sxs-lookup"><span data-stu-id="6a3f3-125">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="6a3f3-126">ממד תמחור מבוסס-קבוצת אפשרויות הנקרא 'שעות עבודה של משאב'</span><span class="sxs-lookup"><span data-stu-id="6a3f3-126">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="6a3f3-127">יצירת נתונים עבור ממדים מבוססי-ישות</span><span class="sxs-lookup"><span data-stu-id="6a3f3-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="6a3f3-128">באפשרותך ליצור נתונים עבור ממדים מבוססי-ישות באופן ידני, או באמצעות ייבוא או קריאות שירות של Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="6a3f3-129">השתמש בשלבים שבהליך זה כדי ליצור שני תארים רגילים, **מהנדס מערכות** ו **מהנדס מערכות בכיר** מהממד מבוסס הישות, **כותרת סטנדרטית**.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="6a3f3-130">אם הנתונים שברצונך ליצור הם בכמות קטנה, בדומה לדוגמה הבאה, באפשרותך להשתמש בטופס רגיל.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="6a3f3-131">ב-PSA, לחץ על **חיפוש מתקדם**.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-131">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="6a3f3-132">בחר את הישות **כותרת סטנדרטית** ולחץ על **תוצאות**.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-132">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="6a3f3-133">כל השורות בישות **כותרת סטנדרטית** יוצגו.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-133">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="6a3f3-134">לחץ על **חדש**.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-134">Click **New**.</span></span> <span data-ttu-id="6a3f3-135">בשדה **שם** , הזן "מהנדס מערכות" ולחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-135">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="6a3f3-136">סגור את הטופס.</span><span class="sxs-lookup"><span data-stu-id="6a3f3-136">Close the form.</span></span> 
4. <span data-ttu-id="6a3f3-137">חזור על שלבים 1-3 כדי ליצור כותרת סטנדרטית נוספת עבור "מהנדס מערכות בכיר".</span><span class="sxs-lookup"><span data-stu-id="6a3f3-137">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="6a3f3-138">נתונים לדוגמה עבור ישות 'כותרת סטנדרטית'</span><span class="sxs-lookup"><span data-stu-id="6a3f3-138">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)


