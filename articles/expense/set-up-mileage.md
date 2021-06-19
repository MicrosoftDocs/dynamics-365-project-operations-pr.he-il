---
title: הגדרת מרחק באמצעות רמות תעריפי מרחק
description: נושא זה מספק מידע על שיעורי הקילומטראז' ושכבות שיעורי הקילומטראז'.
author: suvaidya
ms.date: 05/20/2021
ms.topic: article
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: a44d32358a9e88824efc5452b2b5493ac8b97c7f
ms.sourcegitcommit: 18f99fbceccadd4b3e75875e1c5bcdd3e59ce206
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/20/2021
ms.locfileid: "6083672"
---
# <a name="set-up-mileage-using-mileage-rate-tiers"></a><span data-ttu-id="a92c2-103">הגדרת מרחק באמצעות רמות תעריפי מרחק</span><span class="sxs-lookup"><span data-stu-id="a92c2-103">Set up mileage using mileage rate tiers</span></span>

<span data-ttu-id="a92c2-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="a92c2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="a92c2-105">כאשר מדווחים על הוצאה וקטגוריית ההוצאות שנבחרה היא **קילומטרים‬**, הסכום עבור שורת ההוצאות מחושב על פי *תעריף לקילומטר*.</span><span class="sxs-lookup"><span data-stu-id="a92c2-105">When an expense is reported and the selected expense category is **Mileage**, the amount for that expense line is calculated according to the *rate per mileage* amount.</span></span> <span data-ttu-id="a92c2-106">סכום זה נקבע על ידי שימוש בשכבות קילומטראז' מוגדרות, ואם לא נקבעו שכבות קילומטראז', על ידי תעריף סטנדרטי לקילומטר.</span><span class="sxs-lookup"><span data-stu-id="a92c2-106">This amount is determined by using defined mileage tiers or, if no mileage rate tiers are set up, by following a standard rate of mileage.</span></span> 

<span data-ttu-id="a92c2-107">ניתן להגדיר את שכבות הקילומטראז' על ידי מעבר אל **ניהול הוצאות** > **הגדר** > **כללי** > **קטגוריות הוצאות** > **קילומטרים** > **הגדר קטגוריה**.</span><span class="sxs-lookup"><span data-stu-id="a92c2-107">Mileage rate tiers can be set up by going to **Expense Management** > **Setup** > **General** > **Expense categories** > **Mileage** > **Category setup**.</span></span>

<span data-ttu-id="a92c2-108">לאחר השדרוג ל- 10.0.18, אם הארגון שלך משתמש בקטגוריה של הוצאות קילומטראז', שקול להפעיל את תכונת הקילומטראז' לאחר בחינת שינויי העיצוב בהמשך.</span><span class="sxs-lookup"><span data-stu-id="a92c2-108">After you upgrade to 10.0.18, if your organization uses the mileage expense category, consider enabling the mileage feature after reviewing the design changes below.</span></span> 

<span data-ttu-id="a92c2-109">העיצוב החדש של שכבות קילומטראז' משפיע על האופן שבו השדה **כמות** מעובד.</span><span class="sxs-lookup"><span data-stu-id="a92c2-109">The new design of mileage rate tiers impacts how the value in the **Quantity** field is processed.</span></span> <span data-ttu-id="a92c2-110">לפני ההפצה של 10.0.18, הערך בשדה **כמות** נחשב לגבול התחתון.</span><span class="sxs-lookup"><span data-stu-id="a92c2-110">Prior to the release of 10.0.18, the value in the **Quantity** field was considered to be the lower limit.</span></span> <span data-ttu-id="a92c2-111">כאשר הסכום המצטבר חוצה את הערך הזה, נעשה שימוש בתעריף המקביל.</span><span class="sxs-lookup"><span data-stu-id="a92c2-111">When accumulation crossed that value, the corresponding rate was used.</span></span>  <span data-ttu-id="a92c2-112">החל מ- 10.0.18, הערך בשדה **כמות** נחשב לגבול העליון.</span><span class="sxs-lookup"><span data-stu-id="a92c2-112">As of 10.0.18, the value in the **Quantity** field is considered the upper limit.</span></span> <span data-ttu-id="a92c2-113">בתעריף המקביל משתמשים כאשר הצטברות הקילומטרים קטנה מהערך בשדה **כמות**.</span><span class="sxs-lookup"><span data-stu-id="a92c2-113">The corresponding rate is used when mileage accumulation is less than the value in the **Quantity** field.</span></span>  <span data-ttu-id="a92c2-114">המודל החדש של שכבות הקילומטראז' עוזר לשמור על עקביות בין שכבות קילומטראז' ושימושיות טובה יותר.</span><span class="sxs-lookup"><span data-stu-id="a92c2-114">The new model for mileage tiers helps with consistency across mileage tiers and better usability.</span></span>   

<span data-ttu-id="a92c2-115">כל דוחות ההוצאות שאושרו יחושבו מחדש במהלך הפרסום בהתאם לתכנון החדש.</span><span class="sxs-lookup"><span data-stu-id="a92c2-115">All approved expense reports will be recalculated during posting according to the new design.</span></span>

## <a name="example"></a><span data-ttu-id="a92c2-116">דוגמה</span><span class="sxs-lookup"><span data-stu-id="a92c2-116">Example</span></span>
 
### <a name="before-version-10018"></a><span data-ttu-id="a92c2-117">לפני גירסה 10.0.18</span><span class="sxs-lookup"><span data-stu-id="a92c2-117">Before version 10.0.18</span></span>
<span data-ttu-id="a92c2-118">עם שתי שכבות של תעריפים, השדה **כמות** בכל שכבה מייצג את המגבלה התחתונה.</span><span class="sxs-lookup"><span data-stu-id="a92c2-118">With two mileage rate tiers, the **Quantity** field in each tier represents the lower mileage limit.</span></span> <span data-ttu-id="a92c2-119">נכון לעכשיו, לשכבה הראשונה יש ערך אפס (0) ותעריף של 0.45, ולשכבה השנייה יש ערך של 1000 ותעריף של 0.25.</span><span class="sxs-lookup"><span data-stu-id="a92c2-119">Currently, tier one has a value of zero (0) and a rate of 0.45, and tier two has a value of 1000 and a rate of 0.25.</span></span> <span data-ttu-id="a92c2-120">אם הקילומטרים שנצברו חוצים את הערך בשדה, נעשה שימוש בתעריף הקשור.</span><span class="sxs-lookup"><span data-stu-id="a92c2-120">If the accumulated miles or kilometers crosses the value in the field, the related rate is used.</span></span> <span data-ttu-id="a92c2-121">אם אין שורה עם כמות אפס, המערכת משתמשת בתעריף שמוגדר בניהול הוצאות.</span><span class="sxs-lookup"><span data-stu-id="a92c2-121">If there's no line with zero quantity, the system uses the rate of mileage that is defined in Expense management.</span></span> 
 
<span data-ttu-id="a92c2-122">אם עובד מגיש דוח הוצאות עם 1,500 קילומטר, שתי שורות הקילומטראז' בדוח ההוצאות שפורסם יהיו: 1000 (תעריף 0.45) + 500 (תעריף 0.25) = 575.00.</span><span class="sxs-lookup"><span data-stu-id="a92c2-122">If an employee submits an expense report with 1,500 miles, the two mileage lines on the posted expense report would be: 1000 (rate 0.45) +  500 (rate 0.25) = 575.00.</span></span>

### <a name="after-version-10018"></a><span data-ttu-id="a92c2-123">לאחר גירסה 10.0.18</span><span class="sxs-lookup"><span data-stu-id="a92c2-123">After version 10.0.18</span></span>
<span data-ttu-id="a92c2-124">ב- 10.0.18, השדה **כמות** בכל שכבה מייצג את הגבול העליון של השכבה.</span><span class="sxs-lookup"><span data-stu-id="a92c2-124">In 10.0.18, the **Quantity** field in each tier represents the upper limit of the tier.</span></span> <span data-ttu-id="a92c2-125">נכון לעכשיו, לשכבה הראשונה יש ערך 999 ותעריף של 0.45, ולשכבה השנייה יש ערך של 999,999,999.00 ותעריף של 0.25.</span><span class="sxs-lookup"><span data-stu-id="a92c2-125">Currently, tier one has a value of 999 and a rate of 0.45, and tier two has a value of 999,999,999.00 and a rate of 0.25.</span></span> <span data-ttu-id="a92c2-126">אם הקילומטרים שנצברו חוצים את הערך בשדה **כמות**, נעשה שימוש בתעריף הקשור.</span><span class="sxs-lookup"><span data-stu-id="a92c2-126">If the accumulated miles or kilometers crosses the value in the **Quantity** field, the related rate is used.</span></span> <span data-ttu-id="a92c2-127">אם יש חריגות מכל המגבלות העליונות, המערכת משתמשת בתעריף שמוגדר בניהול הוצאות.</span><span class="sxs-lookup"><span data-stu-id="a92c2-127">If all upper limits are exceeded, the system uses the rate of mileage that is defined in Expense management.</span></span> 
 
<span data-ttu-id="a92c2-128">כדי לחשב נכון את אותו תרחיש, יש לשנות את הגדרת השכבה.</span><span class="sxs-lookup"><span data-stu-id="a92c2-128">To correctly calculate the same scenario, the tier set up must be changed.</span></span> <span data-ttu-id="a92c2-129">לשדה **כמות** יש ערך 999.00 בשכבה הראשונה וערך 999,999,999.00 בשכבה השנייה.</span><span class="sxs-lookup"><span data-stu-id="a92c2-129">The **Quantity** field in tier one has a value of 999.00 and a value of 999,999,999.00 in tier two.</span></span> <span data-ttu-id="a92c2-130">אם עובד חורג מהכמות הכוללת של קילומטרים או קילומטרים בשכבה 1, המערכת משתמשת בתעריף הקילומטראז' המוגדר בניהול הוצאות.</span><span class="sxs-lookup"><span data-stu-id="a92c2-130">If an employee exceeds the total quantity of miles or kilometers in tier one, the system uses the rate of mileage that is defined in Expense management.</span></span> 
  
<span data-ttu-id="a92c2-131">אם עובד מגיש דוח הוצאות עם 1,500 קילומטר, שתי שורות הקילומטראז' בדוח ההוצאות שפורסם יהיו: 1000 (תעריף 0.45) + 500 (תעריף 0.25) = 575</span><span class="sxs-lookup"><span data-stu-id="a92c2-131">If an employee submits an expense report with 1,500 miles, the two mileage lines on the posted expense report would be: 1000 (rate 0.45) +  500 (rate 0.25) = 575</span></span>

## <a name="enable-the-mileage-amount-calculation-for-multiple-mileage-tiers-with-same-rate-feature"></a><span data-ttu-id="a92c2-132">הפעל את חישוב כמות הקילומטראז' למספר שכבות קילומטראז' עם תכונת תעריף זהה</span><span class="sxs-lookup"><span data-stu-id="a92c2-132">Enable the Mileage amount calculation for multiple mileage tiers with same rate feature</span></span>

<span data-ttu-id="a92c2-133">התכונה **חישוב כמות הקילומטראז' למספר שכבות קילומטראז' עם תעריף זהה** משפרת את חישוב התעריף.</span><span class="sxs-lookup"><span data-stu-id="a92c2-133">The **Mileage amount calculation for multiple mileage tiers with same rate** feature improves mileage rate calculation.</span></span> <span data-ttu-id="a92c2-134">בצע את השלבים הבאים כדי להפעיל תכונה זו.</span><span class="sxs-lookup"><span data-stu-id="a92c2-134">Complete the following steps to enable this feature.</span></span>

1. <span data-ttu-id="a92c2-135">עבור אל **סביבות עבודה** > **ניהול תכונות**.</span><span class="sxs-lookup"><span data-stu-id="a92c2-135">Go to **Workspaces** > **Feature Management**.</span></span> 
2. <span data-ttu-id="a92c2-136">ברשימה, אתר ובחר את **חישוב כמות קילומטראז' למספר שכבות קילומטראז' בתעריף זהה** ולאחר מכן בחר **הפוך לזמין עכשיו**.</span><span class="sxs-lookup"><span data-stu-id="a92c2-136">In the list, locate and select **Mileage amount calculation for multiple mileage tiers with same rate**, and then select **Enable now**.</span></span>

<span data-ttu-id="a92c2-137">לאחר הפעלת התכונה, אפס את שכבות הקילומטראז' כך שהן ישקפו נכון את הערך בשדה **כמות**.</span><span class="sxs-lookup"><span data-stu-id="a92c2-137">After you enable the feature, reset the mileage tiers to correctly reflect the value of the **Quantity** field.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]
