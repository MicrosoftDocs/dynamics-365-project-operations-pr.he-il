---
title: יצירת חוזים מתקדמים לחיוב על סמך התקדמות
description: נושא זה מסביר כיצד ליצור חוזי פרויקט כדי שתוכל ליצור חשבוניות ללקוחות על סמך אחוז העבודה שהושלמה.
author: RadhikaRS
manager: AnnBe
ms.date: 03/26/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: b1de330df8cf85ed30c0ee4e4f2f2fe74d05dbff
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289505"
---
# <a name="create-advanced-contracts-for-billing-based-on-progress"></a><span data-ttu-id="af909-103">יצירת חוזים מתקדמים לחיוב על סמך התקדמות</span><span class="sxs-lookup"><span data-stu-id="af909-103">Create advanced contracts for billing based on progress</span></span>
[!include [banner](../includes/banner.md)]

<span data-ttu-id="af909-104">נושא זה מסביר כיצד ליצור חוזי פרויקט כדי שתוכל ליצור חשבוניות ללקוחות על סמך אחוז העבודה שהושלמה.</span><span class="sxs-lookup"><span data-stu-id="af909-104">This topic explains how to create project contracts so that you can create invoices for customers, based on a percentage of completed work.</span></span> <span data-ttu-id="af909-105">סכומי החשבונית מחושבים באופן אוטומטי עבור קטגוריות העבודה התקציביות שהגדרת לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="af909-105">Invoice amounts are automatically calculated for the budget categories of work that you set up for a project.</span></span> <span data-ttu-id="af909-106">תזמון החשבונית נקבע כאשר אתה מנהל משא ומתן על חוזה הפרויקט עם הלקוח.</span><span class="sxs-lookup"><span data-stu-id="af909-106">The invoice timing is set when you negotiate the project contract with the customer.</span></span>

<span data-ttu-id="af909-107">השתמש בתהליכים בנושא זה כדי להגדיר חוזה, פרויקט משויך וכללי חיוב המחשבים סכומי חשבונית עבור קטגוריות העבודה שאתה מגדיר לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="af909-107">Use the procedures in this topic to set up a contract, an associated project, and the billing rules that calculate invoice amounts for the budget categories of work that you set up for the project.</span></span>

<span data-ttu-id="af909-108">לאחר יצירת החוזה והפרויקט, תוכל להגדיר את פרטי הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="af909-108">After you've created the contract and the project, you can set up the details of the project.</span></span> <span data-ttu-id="af909-109">לדוגמה, תוכל להגדיר פעילויות ולהקצות עובדים לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="af909-109">For example, you can define activities and assign workers to the project.</span></span>

## <a name="example"></a><span data-ttu-id="af909-110">דוגמה</span><span class="sxs-lookup"><span data-stu-id="af909-110">Example</span></span>

<span data-ttu-id="af909-111">הארגון שלך הוא חברה לפיתוח תוכנה.</span><span class="sxs-lookup"><span data-stu-id="af909-111">Your organization is a software development firm.</span></span> <span data-ttu-id="af909-112">אתה מסכים לפתח חבילת תוכנות שכר ללקוח תמורת 20,000 דולר אמריקני (USD).</span><span class="sxs-lookup"><span data-stu-id="af909-112">You agree to develop a payroll accounting package for a customer for a total fee of 20,000 US dollars (USD).</span></span> <span data-ttu-id="af909-113">הארגון שלך מסכים להגיש ללקוח חשבונית בהתאם להשלמת אחוזים ספציפיים של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="af909-113">Your organization agrees to invoice the customer as you complete specific percentages of the project.</span></span> <span data-ttu-id="af909-114">אתה מגדיר את קטגוריות הפרויקט הבאות לעבודה, כדי שתוכל להשתמש בהן בתהליך החיוב:</span><span class="sxs-lookup"><span data-stu-id="af909-114">You set up the following project categories for the work, so that you can use them in the billing process:</span></span>

- <span data-ttu-id="af909-115">שירותי ייעוץ</span><span class="sxs-lookup"><span data-stu-id="af909-115">Consulting</span></span>
- <span data-ttu-id="af909-116">עיצוב</span><span class="sxs-lookup"><span data-stu-id="af909-116">Design</span></span>
- <span data-ttu-id="af909-117">התקנה</span><span class="sxs-lookup"><span data-stu-id="af909-117">Installation</span></span>

<span data-ttu-id="af909-118">אתה גם מגדיר כללי חיוב המחשבים אוטומטית את סכומי החשבונית עבור אחוז הפרויקט שהושלם בכל קטגוריה.</span><span class="sxs-lookup"><span data-stu-id="af909-118">You also set up billing rules that automatically calculate the invoice amounts for the percentage of project work that is completed in each category.</span></span>

<span data-ttu-id="af909-119">מנהל התקציב יוצר תקציב לקטגוריות הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="af909-119">The budget manager creates a budget for the project categories.</span></span> <span data-ttu-id="af909-120">כמות העבודה שהושלמה מחושבת באופן אוטומטי כאחוז מהעבודה בפועל בהשוואה לסכומים המתוקצבים.</span><span class="sxs-lookup"><span data-stu-id="af909-120">The amount of completed work is automatically calculated as a percentage of actual work in comparison to the budgeted amounts.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af909-121">דרישות מוקדמות</span><span class="sxs-lookup"><span data-stu-id="af909-121">Prerequisites</span></span>

<span data-ttu-id="af909-122">לפני יצירת פרויקט המשתמש בכללי חיוב, עליך להגדיר רצפי מספרים עבור כללי החיוב ויומן תשלומים המשמש לרישום החיובים על סמך ההתקדמות.</span><span class="sxs-lookup"><span data-stu-id="af909-122">Before you create a project that uses billing rules, you must set up the number sequences for billing rules and a fee journal that is used to post progress billings.</span></span>

1. <span data-ttu-id="af909-123">עבור אל **ניהול פרויקטים וחשבונאות** \> **הגדרה** \> **ניהול פרויקטים ופרמטרים חשבונאיים**.</span><span class="sxs-lookup"><span data-stu-id="af909-123">Go to **Project management and accounting** \> **Setup** \> **Project management and accounting parameters**.</span></span>
2. <span data-ttu-id="af909-124">בדף **ניהול פרויקטים ופרמטרים חשבונאיים**, בכרטיסיה **רצפי מספרים**, הגדר את רצף המספרים שבו אתה רוצה להשתמש בעת יצירת כללי החיוב.</span><span class="sxs-lookup"><span data-stu-id="af909-124">On the **Project management and accounting parameters** page, on the **Number sequences** tab, set up the number sequence that you want to use when billing rules are created.</span></span>
3. <span data-ttu-id="af909-125">עבור אל **ניהול פרויקטים וחשבונאות** \> **יומנים** \> **תשלום**.</span><span class="sxs-lookup"><span data-stu-id="af909-125">Go to **Project management and accounting** \> **Journals** \> **Fee**.</span></span>
4. <span data-ttu-id="af909-126">בדף **יומן תשלומים**, בחר באפשרות **חדש** והזן את שם היומן.</span><span class="sxs-lookup"><span data-stu-id="af909-126">On the **Fee journal** page, select **New**, and enter the journal name.</span></span>

## <a name="create-a-contract-for-progress-billings"></a><span data-ttu-id="af909-127">יצירת חוזה לחיובים על סמך התקדמות</span><span class="sxs-lookup"><span data-stu-id="af909-127">Create a contract for progress billings</span></span>

<span data-ttu-id="af909-128">השתמש בהליך זה כדי ליצור חוזה פרויקט לפרויקט במחיר קבוע.</span><span class="sxs-lookup"><span data-stu-id="af909-128">Use this procedure to create a project contract for a fixed-price project.</span></span> <span data-ttu-id="af909-129">אתה יוצר חשבונית פרויקט כאשר העבודה שהושלמה בפרויקט מגיעה לאחוזים שהוגדרו.</span><span class="sxs-lookup"><span data-stu-id="af909-129">You create a project invoice when the work that is completed on the project reaches a specified percentage.</span></span>

1. <span data-ttu-id="af909-130">עבור אל **ניהול פרויקטים וחשבונאות** \> **פרויקטים** \> **חוזי פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="af909-130">Go to **Project management and accounting** \> **Projects** \> **Project contracts**.</span></span>
2. <span data-ttu-id="af909-131">בדף **חוזי פרויקט**, בחר באפשרות **חדש**.</span><span class="sxs-lookup"><span data-stu-id="af909-131">On the **Project contracts** page, select **New**.</span></span>
3. <span data-ttu-id="af909-132">בתיבת הדו-שיח **חוזה פרויקט חדש**, הגדר את השדות הבאים:</span><span class="sxs-lookup"><span data-stu-id="af909-132">In the **New project contract** dialog box, set the following fields:</span></span>

    - <span data-ttu-id="af909-133">**שם**</span><span class="sxs-lookup"><span data-stu-id="af909-133">**Name**</span></span>
    - <span data-ttu-id="af909-134">**סוג מימון**</span><span class="sxs-lookup"><span data-stu-id="af909-134">**Funding type**</span></span>
    - <span data-ttu-id="af909-135">**מקור מימון**</span><span class="sxs-lookup"><span data-stu-id="af909-135">**Funding source**</span></span>
    - <span data-ttu-id="af909-136">**מטבע מכירות** - כברירת מחדל, נעשה שימוש במטבע זה בחשבוניות לקוח המשויכות לחוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="af909-136">**Sales currency** – By default, this currency is used for customer invoices that are associated with the project contract.</span></span> <span data-ttu-id="af909-137">עם זאת, תוכל לשנות את מטבע המכירות בחשבונית לקוח ספציפית.</span><span class="sxs-lookup"><span data-stu-id="af909-137">However, you can change the sales currency on a specific customer invoice.</span></span>

4. <span data-ttu-id="af909-138">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="af909-138">Select **OK**.</span></span> <span data-ttu-id="af909-139">המידע מועתק לכותרת של הדף **חוזי פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="af909-139">The information is copied to the header of the **Project contracts** page.</span></span>
5. <span data-ttu-id="af909-140">בדף **חוזי פרויקט**, מלא את שאר המידע הדרוש לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="af909-140">On the **Project contracts** page, fill in the rest of the required information for the project.</span></span>

## <a name="create-a-project-for-progress-billings"></a><span data-ttu-id="af909-141">יצירת פרויקט לחיובים על סמך התקדמות</span><span class="sxs-lookup"><span data-stu-id="af909-141">Create a project for progress billings</span></span>

<span data-ttu-id="af909-142">בצע את השלבים הבאים כדי ליצור פרויקט ופרויקטי משנה המשויכים לחוזה פרויקט.</span><span class="sxs-lookup"><span data-stu-id="af909-142">Follow these steps to create a project and any subprojects that are associated with a project contract.</span></span>

1. <span data-ttu-id="af909-143">עבור אל **ניהול פרויקטים וחשבונאות** \> **פרויקטים** \> **כל הפרויקטים**.</span><span class="sxs-lookup"><span data-stu-id="af909-143">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="af909-144">בדף **כל הפרויקטים**, בחר באפשרות **חדש**.</span><span class="sxs-lookup"><span data-stu-id="af909-144">On the **All projects** page, select **New**.</span></span>
3. <span data-ttu-id="af909-145">בתיבת הדו-שיח **פרויקט חדש**, בשדה **סוג פרויקט**, בחר באפשרות **זמן וחומר**.</span><span class="sxs-lookup"><span data-stu-id="af909-145">In the **New project** dialog box, in the **Project type** field, select **Time and material**.</span></span>
4. <span data-ttu-id="af909-146">בחר קבוצת פרויקטים.</span><span class="sxs-lookup"><span data-stu-id="af909-146">Select a project group.</span></span> <span data-ttu-id="af909-147">קבוצת פרויקטים מגדירה את פרטי הרישום של הפרויקטים המוקצים לקבוצה.</span><span class="sxs-lookup"><span data-stu-id="af909-147">A project group defines the posting information for the projects that are assigned to the group.</span></span>
5. <span data-ttu-id="af909-148">בחר **יצירת פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="af909-148">Select **Create project**.</span></span>
6. <span data-ttu-id="af909-149">לאחר יצירת הפרויקט, הגדר את השלב בפרויקט בתור **בתהליך**.</span><span class="sxs-lookup"><span data-stu-id="af909-149">After the project is created, set the project stage to **In process**.</span></span>

## <a name="create-a-budget-for-a-project"></a><span data-ttu-id="af909-150">יצירת תקציב עבור פרויקט</span><span class="sxs-lookup"><span data-stu-id="af909-150">Create a budget for a project</span></span>

<span data-ttu-id="af909-151">קטגוריות התקציב משמשות לחישוב אוטומטי של סכומי החשבונית עבור אחוז העבודה שהושלמה בכל קטגוריה.</span><span class="sxs-lookup"><span data-stu-id="af909-151">Budget categories are used to automatically calculate the invoice amounts for the percentage of work that is completed for each category.</span></span> <span data-ttu-id="af909-152">בצע את השלבים הבאים ליצירת קטגוריות תקציב עבור העלויות המשוערות.</span><span class="sxs-lookup"><span data-stu-id="af909-152">Follow these steps to create budget categories for the estimated costs.</span></span>

1. <span data-ttu-id="af909-153">עבור אל **ניהול פרויקטים וחשבונאות** \> **פרויקטים** \> **כל הפרויקטים**.</span><span class="sxs-lookup"><span data-stu-id="af909-153">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="af909-154">בדף **כל הפרויקטים**, בחר ופתח את הפרויקט הרצוי.</span><span class="sxs-lookup"><span data-stu-id="af909-154">On the **All projects** page, select and open the project that you want.</span></span>
3. <span data-ttu-id="af909-155">בדף **פרויקטים**, בחלונית הפעולות, בכרטיסיה **תכנון**, בקבוצה **תקציב**, בחר באפשרות **תקציב פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="af909-155">On the **Projects** page, on the Action Pane, on the **Plan** tab, in the **Budget** group, select **Project budget**.</span></span>
4. <span data-ttu-id="af909-156">בדף **תקציב פרויקט**, הזן עלות משוערת עבור כל קטגוריה בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="af909-156">On the **Project budget** page, enter an estimated cost for each category in the project.</span></span>

## <a name="create-billing-rules-for-progress-billings"></a><span data-ttu-id="af909-157">יצירת כללי חיוב לחיובים על סמך התקדמות</span><span class="sxs-lookup"><span data-stu-id="af909-157">Create billing rules for progress billings</span></span>

1. <span data-ttu-id="af909-158">עבור אל **ניהול פרויקטים וחשבונאות** \> **פרויקטים** \> **חוזי פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="af909-158">Go to **Project management and accounting** \> **Projects** \> **Project contracts**.</span></span>
2. <span data-ttu-id="af909-159">בדף **חוזי פרויקט**, בחר ופתח חוזה פרויקט.</span><span class="sxs-lookup"><span data-stu-id="af909-159">On the **Project contracts** page, select and open a project contract.</span></span>
3. <span data-ttu-id="af909-160">בדף חוזה הפרויקט, ב- FastTab **כללי חיוב**, בחר באפשרות **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="af909-160">On the project contract page, on the **Billing rules** FastTab, select **Add**.</span></span>
4. <span data-ttu-id="af909-161">בדף **כלל חיוב**, בשדה **סוג שורה**, בחר באפשרות **התקדמות**.</span><span class="sxs-lookup"><span data-stu-id="af909-161">On the **Billing rule** page, in the **Line type** field, select **Progress**.</span></span>
5. <span data-ttu-id="af909-162">ב- FastTab **פרטי שורת כלל חיוב**, בשדה **ערך חוזה**, הזן את הערך הכולל של החוזה.</span><span class="sxs-lookup"><span data-stu-id="af909-162">On the **Billing rule line details** FastTab, in the **Contract value** field, enter the total value of the contract.</span></span>
6. <span data-ttu-id="af909-163">בשדה **קטגוריה**, בחר את הקטגוריה שאליה תרשום את עסקת התשלום.</span><span class="sxs-lookup"><span data-stu-id="af909-163">In the **Category** field, select the category to post the fee transaction to.</span></span>
7. <span data-ttu-id="af909-164">בשדה **פרויקט**, בחר את הפרויקט המשתמש בכלל חיוב זה.</span><span class="sxs-lookup"><span data-stu-id="af909-164">In the **Project** field, select the project that uses this billing rule.</span></span>
8. <span data-ttu-id="af909-165">אופציונלי: הקצאת כלל החיוב לפרויקטים נוספים.</span><span class="sxs-lookup"><span data-stu-id="af909-165">Optional: Assign the billing rule to additional projects.</span></span> <span data-ttu-id="af909-166">ב- FastTab **פרויקט**, בקטע **פרויקטים זמינים**, בחר פרויקט ולאחר מכן לחץ על לחצן החץ ימינה כדי להוסיף את הפרויקט למקטע **פרויקטים שנבחרו**.</span><span class="sxs-lookup"><span data-stu-id="af909-166">On the **Project** FastTab, in the **Available projects** section, select a project, and then select the right arrow button to add the project to the **Selected projects** section.</span></span>
9. <span data-ttu-id="af909-167">אופציונלי: חישוב הסכום באחוזים שהלקוח מעכב את התשלום שלו בחשבונית.</span><span class="sxs-lookup"><span data-stu-id="af909-167">Optional: Calculate the percentage amount that the customer withholds from payments on an invoice.</span></span> <span data-ttu-id="af909-168">ב- FastTab **תנאי שמירת תשלום**, בחר את מקור המימון ואז, בשדה **אחוז שמירה**, הזן את אחוז השמירה.</span><span class="sxs-lookup"><span data-stu-id="af909-168">On the **Payment retention terms** FastTab, select the funding source, and then, in the **Retention percentage** field, enter the retention percentage.</span></span>
10. <span data-ttu-id="af909-169">חזור על שלבים אלה כדי ליצור כללי חיוב נוספים עבור חוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="af909-169">Repeat these steps to create additional billing rules for the project contract.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]