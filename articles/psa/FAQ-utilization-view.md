---
title: הצגת ניצול שניתן לחיוב עבור משאבים
description: נושא זו מספק מידע על תצוגת ניצול המשאבים.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: b07af573bc8d312c45ee4aef50c95942401294fa
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5285934"
---
# <a name="view-chargeable-utilization-for-resources"></a><span data-ttu-id="ba6d5-103">הצגת ניצול שניתן לחיוב עבור משאבים</span><span class="sxs-lookup"><span data-stu-id="ba6d5-103">View chargeable utilization for resources</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]
 
<span data-ttu-id="ba6d5-104">**תצוגת הניצול** בדף **ניצול משאבים של Project Service** מציגה את הניצול שניתן לחיוב עבור כל משאב שניתן להזמין.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-104">The **Utilization View** on the **Project Service Resource Utilization** page shows the chargeable utilization for each bookable resource.</span></span> <span data-ttu-id="ba6d5-105">מכיוון שהתצוגה מבוססת על לוח הזמנים, תוכל למצוא בה פוקנציות רבות זהות.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-105">Because the view is based on the schedule board, you’ll find many of the same functions.</span></span>

> ![צילום מסך של תצוגת ניצול](media/FAQ-utilization-1.png)
 

<span data-ttu-id="ba6d5-107">חישוב ניצול שניתן לחיוב פועל באופן הבא:</span><span class="sxs-lookup"><span data-stu-id="ba6d5-107">The chargeable utilization calculation works as follows:</span></span>

   <span data-ttu-id="ba6d5-108">ניצול שניתן לחיוב = (שעות בפועל הניתנות לחיוב) / (קיבולת משאבים)</span><span class="sxs-lookup"><span data-stu-id="ba6d5-108">Chargeable utilization = (Chargeable actual hours) / (resource capacity)</span></span>

<span data-ttu-id="ba6d5-109">התאים מייצגים את הניצול הניתן לחיוב המחושב עבור התקופה שנבחרה (ימים, שבועות או חודשים).</span><span class="sxs-lookup"><span data-stu-id="ba6d5-109">The cells represent the calculated chargeable utilization for the selected period (days, weeks, or months).</span></span>

<span data-ttu-id="ba6d5-110">הצבעים בכל תא מציגים את הניצול שניתן לחיוב עבור משאב בהשוואה לניצול היעד שלהם שניתן לחיוב.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-110">The colors in each cell show the chargeable utilization for a resource as compared to their target chargeable utilization.</span></span> 

<span data-ttu-id="ba6d5-111">ניתן להגדיר את ניצול היעד בתפקיד ברירת המחדל של המשאב או במשאב הבודד עצמו.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-111">The target utilization can be set on the resource’s default role or on the individual resource itself.</span></span> <span data-ttu-id="ba6d5-112">החישוב מתייחס קודם אל המשאב הבודד עבור יעד ולאחר מכן לתפקיד ברירת המחדל של משאב.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-112">The calculation looks at the individual for the target first, and then to the resource’s default role.</span></span>

## <a name="set-target-on-a-resource"></a><span data-ttu-id="ba6d5-113">הגדרת יעד במשאב</span><span class="sxs-lookup"><span data-stu-id="ba6d5-113">Set target on a resource</span></span>

1. <span data-ttu-id="ba6d5-114">עבור אל **משאבים** \> **משאבים**.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-114">Go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="ba6d5-115">בחר משאב כדי לפתוח את הרשומה.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-115">Select a resource to open the record.</span></span> 
3. <span data-ttu-id="ba6d5-116">בכרטיסיה **Project Service**, תוכל להגדיר את ניצול היעד של המשאב.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-116">On the **Project Service** tab, you can set the resource’s target utilization.</span></span>

> ![צילום מסך של שימוש בכרטיסיה Project Service להגדרת יעד ניצול](media/FAQ-utilization-2.png)
 
## <a name="set-target-utilization-on-a-role"></a><span data-ttu-id="ba6d5-118">הגדרת ניצול יעד בתפקיד</span><span class="sxs-lookup"><span data-stu-id="ba6d5-118">Set target utilization on a role</span></span>

1. <span data-ttu-id="ba6d5-119">עבור אל **משאבים** \> **תפקידי משאבים**.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-119">Go to **Resources** \> **Resource Roles**.</span></span> 
2. <span data-ttu-id="ba6d5-120">בחר תפקיד ופתח את הרשומה.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-120">Select a role and open the record.</span></span> 
3. <span data-ttu-id="ba6d5-121">הגדר את ניצול היעד עבור התפקיד.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-121">Set the target utilization for the role.</span></span>

> ![צילום מסך של שימוש ב'תפקידי משאבים' להגדרת יעד הניצול](media/FAQ-utilization-3.png)
 
## <a name="calculate-chargeable-utilization-for-a-resource"></a><span data-ttu-id="ba6d5-123">חישוב ניצול שניתן לחיוב עבור משאב</span><span class="sxs-lookup"><span data-stu-id="ba6d5-123">Calculate chargeable utilization for a resource</span></span>

<span data-ttu-id="ba6d5-124">לחישוב ניצול לחיוב עבור משאב, עליך להשלים כמה דרישות מקדימות.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-124">To calculate chargeable utilization for a resource, you will need to complete some pre-requisites.</span></span> 

### <a name="set-default-role-for-individual-resource"></a><span data-ttu-id="ba6d5-125">הגדרת תפקיד בברירת מחדל עבור משאב בודד</span><span class="sxs-lookup"><span data-stu-id="ba6d5-125">Set default role for individual resource</span></span>

<span data-ttu-id="ba6d5-126">תחילה, יש להגדיר את ניצול היעד עבור משאב בודד או עבור תפקידי משאב.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-126">First, the target utilization must be set on either the individual resource or on resource roles.</span></span> <span data-ttu-id="ba6d5-127">אם אתה משתמש בתפקידי משאבים עבור יעדים, לכל משאב בודד חייב להיות תפקיד ברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-127">If you are using resource roles for targets, each individual resource must have a default role.</span></span> 

1. <span data-ttu-id="ba6d5-128">כדי להגדיר זאת, עבור אל **משאבים** \> **משאבים**.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-128">To set this, go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="ba6d5-129">בחר משאב, פתח את הרשומה ולאחר מכן בחר את הכרטיסיה **Project Service**.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-129">Select a resource, open the record, and then select the **Project Service** tab.</span></span> 
3. <span data-ttu-id="ba6d5-130">ברשת **תפקיד משאב**, ודא שיש תפקיד אחד עבור המשאב ושהאפשרות **‏‫מהווה ברירת מחדל‬** מוגדרת בתור **כן**.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-130">In the **Resource Role** grid, make sure there’s one role for the resource and **Is Default** is set to **Yes**.</span></span>
 
### <a name="change-billing-type-for-resource-role"></a><span data-ttu-id="ba6d5-131">שינוי סוג החיוב עבור תפקיד משאב</span><span class="sxs-lookup"><span data-stu-id="ba6d5-131">Change billing type for resource role</span></span>

<span data-ttu-id="ba6d5-132">יש להגדיר את תפקידי המשאב כדי שסוג החיוב יהיה **‏‫ניתן לחיוב‬**.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-132">The resource roles must be set to have a billing type of **Chargeable**.</span></span> 

1. <span data-ttu-id="ba6d5-133">עבור אל **משאבים** \> **תפקידי משאבים**.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-133">Go to **Resources** \> **Resource Roles**.</span></span> 
2. <span data-ttu-id="ba6d5-134">פתח את הרשומה שברצונך לעדכן ולאחר מכן הגדר את ברירת המחדל של סוג החיוב ל **‏‫ניתן לחיוב‬**.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-134">Open the record you want to update, and then set the billing type default to **Chargeable**.</span></span>

### <a name="set-working-hours-for-resource-role"></a><span data-ttu-id="ba6d5-135">הגדרת שעות עבודה עבור תפקיד משאב</span><span class="sxs-lookup"><span data-stu-id="ba6d5-135">Set working hours for resource role</span></span>
 
<span data-ttu-id="ba6d5-136">המשאב חייב להכיל שעות עבודה לחישוב הקיבולת.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-136">The resource must have working hours for the capacity calculation.</span></span> 

1. <span data-ttu-id="ba6d5-137">עבור אל **משאבים** \> **משאבים**.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-137">Go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="ba6d5-138">בחר משאב כדי לפתוח את הרשומה ולאחר מכן בחר **הצג שעות עבודה**.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-138">Select a resource to open the record, and then select **Show Work Hours**.</span></span> 
3. <span data-ttu-id="ba6d5-139">אתה יכול לבצע עדכון בצובר של רשימת המשאבים על-ידי החלת **תבנית שעות עבודה** מהתצוגה **רשימת משאבים**.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-139">You can bulk-update the list of resources by applying a **Work Hour Template** from the **Resource List** view.</span></span>

## <a name="troubleshooting-chargeable-actual-hours"></a><span data-ttu-id="ba6d5-140">פתרון בעיות של שעות בפועל לחיוב</span><span class="sxs-lookup"><span data-stu-id="ba6d5-140">Troubleshooting chargeable actual hours</span></span>

<span data-ttu-id="ba6d5-141">מקור השעות בפועל לחיוב הוא מהישות  **נתונים בפועל**.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-141">The chargeable actual hours are sourced from the **Actuals** entity.</span></span> <span data-ttu-id="ba6d5-142">נתונים בפועל עם חיוב מסוג **ניתן לחיוב** כלולים בחישוב ומסיבה זו עליך הנתונים בפועל בפרוייקטים שלך חייבים להיות ניתנים לחיוב.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-142">Actuals with a billing type of **Chargeable** are included in the calculation and, for this reason, you must have projects where the actuals that are chargeable.</span></span>

<span data-ttu-id="ba6d5-143">אם אינך רואה ניצול לחיוב, להלן מספר דברים שניתן לבדוק:</span><span class="sxs-lookup"><span data-stu-id="ba6d5-143">If you are not seeing chargeable utilization, here are some things you can check:</span></span>

- <span data-ttu-id="ba6d5-144">המשאב מכיל שעות עבודה המוגדרות עבור קיבולת.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-144">The resource has working hours defined for capacity.</span></span>
- <span data-ttu-id="ba6d5-145">המשאב כולל יעד ניצול המוגדר בנפרד או בעל תפקיד ברירת מחדל שהוקצה לו.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-145">The resource has either an individually defined utilization target or has a default role assigned to it.</span></span> <span data-ttu-id="ba6d5-146">התפקיד כולל יעד ניצול שהוגדר עבורו.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-146">The role has a utilization target defined for it.</span></span>
- <span data-ttu-id="ba6d5-147">לנתונים בפועל יש חיוב מסוג **ניתן לחיוב** עבור התקופה שבה אתה מצפה לחישוב ניצול.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-147">Actuals have a billing type of **Chargeable** for the period you are expecting a utilization calculation for.</span></span> <span data-ttu-id="ba6d5-148">בדוק את הנקודות הבאות אם אתה רואה נתונים בפועל עם סוגי חיוב שאינם 'ניתן לחיוב':</span><span class="sxs-lookup"><span data-stu-id="ba6d5-148">Check the following if you are seeing actuals with billing types other than chargeable:</span></span>

  - <span data-ttu-id="ba6d5-149">לתפקיד המשמש בשעות פועל יש ברירת מחדל לסוג חיוב השונה מהסוג 'לחיוב'.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-149">The role used on the actual has a default billing type of something other than chargeable.</span></span>
  - <span data-ttu-id="ba6d5-150">התפקיד בסעיף חוזה הפרוייקט שמגבה את הפרוייקט הוגדר בתור 'אינו ניתן לחיוב'.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-150">The role on the project contract line backing the project has been set to non-chargeable.</span></span>
  - <span data-ttu-id="ba6d5-151">לפרוייקט לא משויך סעיף חוזה.</span><span class="sxs-lookup"><span data-stu-id="ba6d5-151">The project does not have an associated contract line.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]