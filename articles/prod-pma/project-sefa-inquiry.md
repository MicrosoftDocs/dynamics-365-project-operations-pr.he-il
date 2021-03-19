---
title: לוח זמנים להוצאות של חקירת הפרסים הפדרליים
description: נושא זה מספק מידע על לוח הזמנים להוצאות החקירה על פרסים פדרליים.
author: velofog
manager: Ann Beebe
ms.date: 04/2/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: PSNProjSEFAinquiry
audience: Application User
ms.devlang: ''
ms.reviewer: roschlom
ms.search.scope: Operations, Core
ms.tgt_pltfrm: ''
ms.custom: ''
ms.search.region: Global
ms.search.industry: public sector
ms.author: andchoi
ms.search.validFrom: 2020-4-01
ms.dyn365.ops.version: 10.0.11
ms.openlocfilehash: 70dff12c106723dda801668412cfd084c462db4b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288965"
---
# <a name="schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="1f103-103">לוח זמנים להוצאות של חקירת הפרסים הפדרליים</span><span class="sxs-lookup"><span data-stu-id="1f103-103">Schedule of Expenditures of Federal Awards inquiry</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="1f103-104">על פי משרד ניהול התקציב A-133, סוכנויות המקבלות כספים פדרליים כפופות לדרישות ביקורת, המכונות גם ביקורת יחידה.</span><span class="sxs-lookup"><span data-stu-id="1f103-104">According to Office of Management and Budget Circular A-133, agencies that receive federal funds are subject to audit requirements, which are also known as single audits.</span></span> <span data-ttu-id="1f103-105">תהליך הביקורת משמש לדיווח על הכנסות והוצאות של מענקים פדרליים על בסיס חוזר.</span><span class="sxs-lookup"><span data-stu-id="1f103-105">The audit process is used to report on the revenues and expenditures of federal grants on a recurring basis.</span></span> <span data-ttu-id="1f103-106">חלק מדוח ביקורת היחידה כולל את לוח הזמנים של ההוצאות של פרסים פדרליים (SEFA).</span><span class="sxs-lookup"><span data-stu-id="1f103-106">Part of the single audit report includes the Schedule of Expenditures of Federal Awards (SEFA).</span></span>

<span data-ttu-id="1f103-107">לוח הזמנים של ההוצאות על חקירת פרסים פדרליים כולל את קטלוג המסמך הפדרלי לסיוע מקומי (CFDA), מספר המענק, שנת המענק, שם הסוכנות הפדרלית המספקת את הכספים ושם ישות המעבר.</span><span class="sxs-lookup"><span data-stu-id="1f103-107">The Schedule of Expenditures of Federal Awards inquiry includes the Catalog of Federal Domestic Assistance (CFDA) title and number, the grant number, the year of the grant, the name of the federal agency that provides the funds, and the name of the pass-through entity.</span></span> <span data-ttu-id="1f103-108">החקירה היא לתקופה מסוימת.</span><span class="sxs-lookup"><span data-stu-id="1f103-108">The inquiry is for a specific period.</span></span> <span data-ttu-id="1f103-109">בדרך כלל, תקופה זו זהה לתקופת הדוח הכספי, שהיא שנת כספים.</span><span class="sxs-lookup"><span data-stu-id="1f103-109">Typically, that period is the same as the financial statement period, which is a fiscal year.</span></span>

<span data-ttu-id="1f103-110">החקירה כוללת מענקים שמועדי ההעברה שלהם נמצאים בטווח התאריכים שנבחר.</span><span class="sxs-lookup"><span data-stu-id="1f103-110">The inquiry includes grants that have projection dates in the selected date range.</span></span> <span data-ttu-id="1f103-111">העמודה **סוכנות מענקים** של החקירה מציגה את לקוח המענק או, עבור מענק מעבר, את הסוכנות המעניקה.</span><span class="sxs-lookup"><span data-stu-id="1f103-111">The **Grantor agency** column of the inquiry shows the grant customer or, for a pass-through grant, the grantor agency.</span></span> <span data-ttu-id="1f103-112">במקרה של מענק מעבר, העמודה **סוכנות מעבר** מציגה את לקוח המענק.</span><span class="sxs-lookup"><span data-stu-id="1f103-112">For a pass-through grant, the **Pass-through agency** column shows the grant customer.</span></span> <span data-ttu-id="1f103-113">אם המענק אינו מענק-מעבר, העמודה **סוכנות מעבר** ריקה.</span><span class="sxs-lookup"><span data-stu-id="1f103-113">If the grant isn't a pass-through grant, the **Pass-through agency** column is blank.</span></span>

## <a name="set-up-the-cfda-clusters"></a><span data-ttu-id="1f103-114">הגדרת אשכולות CFDA</span><span class="sxs-lookup"><span data-stu-id="1f103-114">Set up the CFDA clusters</span></span>

<span data-ttu-id="1f103-115">יש להגדיר את אשכולות ה- CFDA שיכולים להיות משויכים למספרי CFDA בתזמון ההוצאות של חקירת הפרסים הפדרליים.</span><span class="sxs-lookup"><span data-stu-id="1f103-115">You must set up the CFDA clusters that can be associated with CFDA numbers in the Schedule of Expenditures of Federal Awards inquiry.</span></span>

1. <span data-ttu-id="1f103-116">עבור אל **ניהול פרויקטים וחשבונאות\> הגדרה \> מענקים \> קטלוג אשכולות סיוע מקומי פדרלי**.</span><span class="sxs-lookup"><span data-stu-id="1f103-116">Go to **Project management and accounting \> Setup \> Grants \> Catalog of Federal Domestic Assistance clusters**.</span></span>
2. <span data-ttu-id="1f103-117">בחר **חדש** כדי ליצור אשכול CFDA.</span><span class="sxs-lookup"><span data-stu-id="1f103-117">Select **New** to create a CFDA cluster.</span></span>
3. <span data-ttu-id="1f103-118">הזן את שם האשכול.</span><span class="sxs-lookup"><span data-stu-id="1f103-118">Enter the cluster name.</span></span>
4. <span data-ttu-id="1f103-119">בחר **שמור** כדי לשמור את השינויים.</span><span class="sxs-lookup"><span data-stu-id="1f103-119">Select **Save** to save your changes.</span></span>

## <a name="set-up-cfda-numbers"></a><span data-ttu-id="1f103-120">הגדר מספרי CFDA</span><span class="sxs-lookup"><span data-stu-id="1f103-120">Set up CFDA numbers</span></span>

<span data-ttu-id="1f103-121">יש להגדיר את מספרי ה- CFDA שניתן להוסיף למענקים ולכלול בתזמון ההוצאות של חקירת הפרסים הפדרליים.</span><span class="sxs-lookup"><span data-stu-id="1f103-121">You must set up CFDA numbers that can be added to grants and included in the Schedule of Expenditures of Federal Awards inquiry.</span></span>

1. <span data-ttu-id="1f103-122">עבור אל **ניהול פרויקטים וחשבונאות \> הגדרה \> מענקים \> קטלוג מספרים של סיוע מקומי פדרלי**.</span><span class="sxs-lookup"><span data-stu-id="1f103-122">Go to **Project management and accounting \> Setup \> Grants \> Catalog of Federal Domestic Assistance numbers**.</span></span>
2. <span data-ttu-id="1f103-123">בחר **חדש** כדי ליצור מספר CFDA.</span><span class="sxs-lookup"><span data-stu-id="1f103-123">Select **New** to create a CFDA number.</span></span>
3. <span data-ttu-id="1f103-124">בעמודה **מספר**, הזן את המספר ה- CFDA.</span><span class="sxs-lookup"><span data-stu-id="1f103-124">In the **Number** column, enter the CFDA number.</span></span>
4. <span data-ttu-id="1f103-125">לחץ על המקש **כרטיסיה**.</span><span class="sxs-lookup"><span data-stu-id="1f103-125">Press the **Tab** key.</span></span>
5. <span data-ttu-id="1f103-126">בעמודה **תיאור**, הזן את כותרת ה- CFDA.</span><span class="sxs-lookup"><span data-stu-id="1f103-126">In the **Description** column, enter the CFDA title.</span></span>
6. <span data-ttu-id="1f103-127">לחץ על המקש **כרטיסיה**.</span><span class="sxs-lookup"><span data-stu-id="1f103-127">Press the **Tab** key.</span></span>
7. <span data-ttu-id="1f103-128">אופציונלי: בשדה **אשכול התוכנית**, הוסף את אשכול ה- CFDA המתאים.</span><span class="sxs-lookup"><span data-stu-id="1f103-128">Optional: In the **Program cluster** field, add the appropriate CFDA cluster.</span></span>
8. <span data-ttu-id="1f103-129">בחר **שמור** כדי לשמור את השינויים.</span><span class="sxs-lookup"><span data-stu-id="1f103-129">Select **Save** to save your changes.</span></span>

## <a name="set-up-grants-to-report-for-the-schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="1f103-130">הגדר מענקים לדיווח עבור לוח הזמנים לחקירה של פרסי הוצאות פדרליים</span><span class="sxs-lookup"><span data-stu-id="1f103-130">Set up grants to report for the Schedule of Expenditures of Federal Awards inquiry</span></span>

1. <span data-ttu-id="1f103-131">עבור אל **ניהול פרויקטים וחשבונאות \> מענקים \> מענקים**, ובחר מענק קיים.</span><span class="sxs-lookup"><span data-stu-id="1f103-131">Go to **Project management and accounting \> Grants \> Grants**, and select an existing grant.</span></span>
2. <span data-ttu-id="1f103-132">בכרטיסיה המהירה **הגדרה** בשדה **קטלוג סיוע מקומי פדרלי**, הקצה את מספר ה- CFDA.</span><span class="sxs-lookup"><span data-stu-id="1f103-132">On the **Setup** FastTab, in the **Catalog of Federal Domestic Assistance** field, assign the CFDA number.</span></span> <span data-ttu-id="1f103-133">מספר ה- CFDA במענק קובע את אשכול ה- CFDA לדיווח.</span><span class="sxs-lookup"><span data-stu-id="1f103-133">The CFDA number on the grant determines the CFDA cluster for reporting.</span></span>
3. <span data-ttu-id="1f103-134">בכרטיסיה **פרטי התקשרות**, הזן את פרטי המעניק על ידי ביצוע השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="1f103-134">On **Contact information** FastTab, enter the grantor information by following these steps:</span></span>

    1. <span data-ttu-id="1f103-135">בשדה **לקוח המענק**, הזן את הלקוח שאחראי למענק.</span><span class="sxs-lookup"><span data-stu-id="1f103-135">In the **Grant customer** field, enter the customer who is responsible for the grant.</span></span> <span data-ttu-id="1f103-136">לקבלת מענק קיים, ייתכן שהמידע הזה כבר הוזן.</span><span class="sxs-lookup"><span data-stu-id="1f103-136">For an existing grant, this information might already be entered.</span></span>
    2. <span data-ttu-id="1f103-137">ציין אם לקוח המענק הוא המממן.</span><span class="sxs-lookup"><span data-stu-id="1f103-137">Indicate whether the grant customer is the funder.</span></span> <span data-ttu-id="1f103-138">אם לקוח המענק הוא המממן, השאר את התיבה **מעבר** ללא סימון.</span><span class="sxs-lookup"><span data-stu-id="1f103-138">If the grant customer is the funder, leave the **Pass-through** check box cleared.</span></span> <span data-ttu-id="1f103-139">אם לקוח אחר הוא המממן, ולקוח המענק אחראי על הוצאות הכסף ומעקב אחריו, סמן את התיבה **מעבר**.</span><span class="sxs-lookup"><span data-stu-id="1f103-139">If another customer is the funder, and the grant customer is responsible for spending and tracking the money, select the **Pass-through** check box.</span></span>

4. <span data-ttu-id="1f103-140">אם סימנת את התיבה **מעבר** בשלב הקודם, בשדה **סוכנות מענק** הזן את הלקוח שסיפק את המענק.</span><span class="sxs-lookup"><span data-stu-id="1f103-140">If you selected the **Pass-through** check box in the previous step, in the **Grantor agency** field, enter the customer who provided the grant.</span></span> <span data-ttu-id="1f103-141">הסוכנות המעניקה ולקוח המענק אינם יכולים להיות אותו לקוח.</span><span class="sxs-lookup"><span data-stu-id="1f103-141">The grantor agency and the grant customer can't be the same customer.</span></span>

<span data-ttu-id="1f103-142">הנה דוגמה למענק מעבר:</span><span class="sxs-lookup"><span data-stu-id="1f103-142">Here is an example of a pass-through grant:</span></span>

<span data-ttu-id="1f103-143">הממשלה הפדרלית מימנה פרויקט תשתית למדינה.</span><span class="sxs-lookup"><span data-stu-id="1f103-143">The federal government funded an infrastructure project for a state.</span></span> <span data-ttu-id="1f103-144">הממשלה הפדרלית נתנה את הכסף למדינה.</span><span class="sxs-lookup"><span data-stu-id="1f103-144">The federal government gave the money to the state to spend.</span></span> <span data-ttu-id="1f103-145">במקרה זה, הממשלה הפדרלית היא הסוכנות המעניקה, והמדינה היא לקוח המענק.</span><span class="sxs-lookup"><span data-stu-id="1f103-145">In this case, the federal government is the grantor agency, and the state is the grant customer.</span></span>

> [!NOTE] 
> <span data-ttu-id="1f103-146">כאשר אתה מפעיל לראשונה את התכונה, מספרי CFDA ראשוניים יוזנו באמצעות המספרים הקיימים במענקים.</span><span class="sxs-lookup"><span data-stu-id="1f103-146">When you first turn on the feature, initial CFDA numbers will be entered by using the existing numbers on grants.</span></span>

## <a name="exclude-grants-from-sefa-reporting-based-on-the-grant-type"></a><span data-ttu-id="1f103-147">אל תכלול מענקים מדיווח SEFA בהתבסס על סוג המענק</span><span class="sxs-lookup"><span data-stu-id="1f103-147">Exclude grants from SEFA reporting based on the grant type</span></span>

1. <span data-ttu-id="1f103-148">עבור אל **ניהול פרויקטים וחשבונאות \> הגדרה \> מענקים \> סוגי מענקים**.</span><span class="sxs-lookup"><span data-stu-id="1f103-148">Go to **Project management and accounting \> Setup \> Grants \> Grant types**.</span></span>
2. <span data-ttu-id="1f103-149">בכרטיסיה **פרטי ברירת מחדל** בחר את התיבה **לא לכלול בתזמון ההוצאות של פרסים פדרליים**.</span><span class="sxs-lookup"><span data-stu-id="1f103-149">On the **Default information** FastTab, select the **Exclude from Schedule of Expenditures of Federal Awards** check box.</span></span>
3. <span data-ttu-id="1f103-150">בחר **שמור** כדי לשמור את השינויים.</span><span class="sxs-lookup"><span data-stu-id="1f103-150">Select **Save** to save your changes.</span></span>

## <a name="run-the-schedule-of-expenditures-of-federal-awards-inquiry"></a><span data-ttu-id="1f103-151">הפעל את לוח זמנים להוצאות של חקירת הפרסים הפדרליים</span><span class="sxs-lookup"><span data-stu-id="1f103-151">Run the Schedule of Expenditures of Federal Awards inquiry</span></span>

1. <span data-ttu-id="1f103-152">עבור אל **ניהול פרויקטים וחשבונאות \> חקירות ודוחות \> חקירת מענקים \> לוח זמנים להוצאות של פרסים פדרליים**.</span><span class="sxs-lookup"><span data-stu-id="1f103-152">Go to **Project management and accounting \> Inquiries and reports \> Grant inquiry \> Schedule of Expenditures of Federal Awards**.</span></span>
2. <span data-ttu-id="1f103-153">במקטע **פרמטרים**, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="1f103-153">In the **Parameters** section, follow these steps:</span></span>

    1. <span data-ttu-id="1f103-154">בשדה **טווח תאריכים** בחר את הקוד עבור טווח התאריכים.</span><span class="sxs-lookup"><span data-stu-id="1f103-154">In the **Date interval** field, select the code for the date interval.</span></span> <span data-ttu-id="1f103-155">לחלופין, בשדות **מתאריך** ו- **עד תאריך**, הגדר את טווח התאריכים.</span><span class="sxs-lookup"><span data-stu-id="1f103-155">Alternatively, in the **From date** and **To date** fields, define the date interval.</span></span>
    2. <span data-ttu-id="1f103-156">אופציונלי: כדי לכלול רק עסקאות שחויבו כהכנסות בחקירה, הגדר את האפשרות **כלול רק הכנסות שחויבו** שתהיה **כן**.</span><span class="sxs-lookup"><span data-stu-id="1f103-156">Optional: To include only billed transactions as revenue in the inquiry, set the **Include only billed revenues** option to **Yes**.</span></span>

## <a name="columns"></a><span data-ttu-id="1f103-157">עמודות</span><span class="sxs-lookup"><span data-stu-id="1f103-157">Columns</span></span>

<span data-ttu-id="1f103-158">לוח הזמנים להוצאות של חקירת הפרסים הפדרליים כולל את העמודות הבאות:</span><span class="sxs-lookup"><span data-stu-id="1f103-158">The Schedule of Expenditures of Federal Awards inquiry includes the following columns:</span></span>

- <span data-ttu-id="1f103-159">שם הקטלוג של אשכול פדרלי לסיוע מקומי</span><span class="sxs-lookup"><span data-stu-id="1f103-159">Catalog of Federal Domestic Assistance cluster name</span></span>
- <span data-ttu-id="1f103-160">סוכנות מענק</span><span class="sxs-lookup"><span data-stu-id="1f103-160">Grantor agency</span></span>
- <span data-ttu-id="1f103-161">סוכנות מעבר</span><span class="sxs-lookup"><span data-stu-id="1f103-161">Pass-through agency</span></span>
- <span data-ttu-id="1f103-162">שם מענק</span><span class="sxs-lookup"><span data-stu-id="1f103-162">Grant name</span></span>
- <span data-ttu-id="1f103-163">מזהה מענק</span><span class="sxs-lookup"><span data-stu-id="1f103-163">Grant ID</span></span>
- <span data-ttu-id="1f103-164">מזהה יישום מענק</span><span class="sxs-lookup"><span data-stu-id="1f103-164">Grant application ID</span></span>
- <span data-ttu-id="1f103-165">קטלוג של אשכולות פדרליים לסיוע מקומי</span><span class="sxs-lookup"><span data-stu-id="1f103-165">Catalog of Federal Domestic Assistance</span></span>
- <span data-ttu-id="1f103-166">קבלות</span><span class="sxs-lookup"><span data-stu-id="1f103-166">Receipts</span></span>
- <span data-ttu-id="1f103-167">הוצאות</span><span class="sxs-lookup"><span data-stu-id="1f103-167">Expenditures</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]