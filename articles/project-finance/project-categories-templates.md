---
title: סנכרון קטגוריות של הוצאות בפרוייקט בין Finance and Operations ו- Project Service Automation
description: נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון קטגוריות של הוצאות בפרוייקט בין Microsoft Dynamics 365 Finance ו- Dynamics 365 Project Service Automation.
author: KimANelson
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: 7dd914dc-1913-45eb-8a67-e897b00089fa
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: 757fe1dbc804b986fc3334ebae7254a3f0491f59
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751834"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a><span data-ttu-id="f2e2b-103">סנכרון קטגוריות של הוצאות בפרוייקט בין Finance and Operations ו- Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="f2e2b-103">Synchronize project expense categories between Finance and Operations and Project Service Automation</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="f2e2b-104">נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון קטגוריות של הוצאות בפרוייקט בין Dynamics 365 Finance ו- Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-104">This topic describes the templates and underlying tasks that are used to synchronize project expense categories between Dynamics 365 Finance and Dynamics 365 Project Service Automation.</span></span>

> [!NOTE]
> - <span data-ttu-id="f2e2b-105">שילוב משימות פרוייקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונעילת פונקציונליות זמינים בגירסה 8.0.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="f2e2b-106">שילוב נתונים בפועל זמין בגירסה 8.0.1 ואילך.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-106">Actuals integration is available in version 8.0.1 or later.</span></span>
> - <span data-ttu-id="f2e2b-107">אם אתה משתמש ב- Enterprise Edition 7.3.0, לאחר התקנת KB 4132657 ו- KB 4132660, תוכל להשתמש בתבניות לשילוב משימות פרוייקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונתונים בפועל, וכן להגדיר תצורה של נעילת פונקציונליות.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-107">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="f2e2b-108">אם עליך לאפס את ההפצות החשבונאיות, מומלץ להתקין גם את KB 4131710.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-108">If you must reset the accounting distributions, we recommend that you also install KB 4131710.</span></span>

## <a name="data-flow-for-project-service-automation-and-finance"></a><span data-ttu-id="f2e2b-109">זרימת נתונים עבור Project Service Automation ו- Finance</span><span class="sxs-lookup"><span data-stu-id="f2e2b-109">Data flow for Project Service Automation and Finance</span></span>

<span data-ttu-id="f2e2b-110">פתרון השילוב Project Service Automation ו- Finance משתמש בתכונת שילוב הנתונים לסנכרון נתונים במופעים של Project Service Automation ו- Finance.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-110">The Project Service Automation and Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="f2e2b-111">תבניות השילוב שזמינות עם תכונת שילוב הנתונים מאפשרות זרימת נתונים על קטגוריות של עסקאות הוצאה בפרוייקט ובין Finance ו- Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-111">The integration templates that are available with the Data integration feature enable the flow of data about project expense transaction categories between Finance and Project Service Automation.</span></span>

<span data-ttu-id="f2e2b-112">אם הקטגוריות של הוצאות בפרוייקט נשלטות ב- Finance, זרימת השילוב תהיה ראשונה מ- Finance אל Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-112">If the project expense categories are mastered in Finance, the integration flow is first from Finance to Project Service Automation.</span></span> <span data-ttu-id="f2e2b-113">מזהי השילוב של קטגוריות הוצאות בפרוייקט מתעדכנים לאחר מכן באמצעות סנכרון מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-113">The integration IDs of the project expense categories are then updated through synchronization from Project Service Automation to Finance.</span></span>

<span data-ttu-id="f2e2b-114">אם הקטגוריות של הוצאות בפרוייקט נשלטות ב- Project Service Automation, זרימת השילוב תהיה ראשונה מ- Project Service Automation אל Finance.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-114">If the project expense categories are mastered in Project Service Automation, the integration flow is first from Project Service Automation to Finance.</span></span> <span data-ttu-id="f2e2b-115">יש להגדיר את קטגוריות הפרוייקט כבר ב- Finance לפני הסינכרון מ- Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-115">The project categories must already be configured in Finance before the synchronization from Project Service Automation.</span></span> <span data-ttu-id="f2e2b-116">לאחר מכן סנכרן מ- Finance בחזרה ל- Project Service Automation, ואז מ- Project Service Automation ל- Finance שוב.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-116">Then synchronize from Finance back to Project Service Automation, and then from Project Service Automation to Finance again.</span></span> <span data-ttu-id="f2e2b-117">באופן זה, אתה עוזר להבטיח שהקטגוריות יהיו מקושרות ושלא ייווצרו כפילויות.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-117">In this way, you help guarantee that the categories are linked, and that no duplicates are created.</span></span>

> [!NOTE]
> <span data-ttu-id="f2e2b-118">בדרך כלל, קטגוריות של הוצאות בפרוייקט נשלטות ב- Finance.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-118">Typically, the project expense categories are mastered in Finance.</span></span> <span data-ttu-id="f2e2b-119">עם זאת, אם הן לא נשלטות משם, או אם הקטגוריות של ההוצאות כבר נוצרו ב- Project Service Automation, עליך תחילה לסנכרן באמצעות תבנית קטגוריות של עסקאות הוצאות בפרוייקט (PSA ל- Fin and Ops).</span><span class="sxs-lookup"><span data-stu-id="f2e2b-119">However, if they aren't, or if expense categories have already been created in Project Service Automation, you must first synchronize by using the Project expense transaction categories (PSA to Fin and Ops) template.</span></span> <span data-ttu-id="f2e2b-120">לאחר מכן סנכרן באמצעות תבנית הקטגוריות של עסקאות הוצאות בפרוייקט (Fin and Ops ל- PSA).</span><span class="sxs-lookup"><span data-stu-id="f2e2b-120">Then synchronize by using the Project expense transaction categories (Fin and Ops to PSA) template.</span></span> <span data-ttu-id="f2e2b-121">לאחר מכן עליך להפעיל את הסנכרון מ- Project Service Automation ל- Finance פעם נוספת.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-121">You should then run the synchronization from Project Service Automation to Finance one more time.</span></span>
>
> <span data-ttu-id="f2e2b-122">אם אתה מסנכרן תחילה מ- Project Service Automation, יש לעמוד בדרישות הבאות ב- Finance לפני הפעלת הסנכרון:</span><span class="sxs-lookup"><span data-stu-id="f2e2b-122">If you synchronize first from Project Service Automation, the following requirements must be met in Finance before the synchronization is run:</span></span>
>
> - <span data-ttu-id="f2e2b-123">הקטגוריה המשותפת שתואמת לקטגוריית הפרויקט שמוגדרת ב- Project Service Automation חייבת להתקיים, והיא חייבת להיות מופעלת גם עבור **פרוייקט** וגם עבור **הוצאה**.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-123">The shared category that matches the project category that is set up in Project Service Automation must exist, and it must be enabled for both **Project** and **Expense**.</span></span>
> - <span data-ttu-id="f2e2b-124">עבור כל ישות משפטית ב- Finance שבה יש לשלב, קטגוריות הפרוייקט הבאות חייבות להתקיים:</span><span class="sxs-lookup"><span data-stu-id="f2e2b-124">For each Finance legal entity that must be integrated with, the following project categories must exist:</span></span>
>
>     - <span data-ttu-id="f2e2b-125">**קטגוריית פרוייקט** קיימת.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-125">**Project category** exists.</span></span> 
>     - <span data-ttu-id="f2e2b-126">האפשרות **השתמש בהוצאה** זמינה.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-126">**Use in Expense** is enabled.</span></span>
>     - <span data-ttu-id="f2e2b-127">האפשרות **פעיל ביומן** זמינה.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-127">**Active in journal** is enabled.</span></span>
>     - <span data-ttu-id="f2e2b-128">**סוג עסקה** נקבעה בתור **הוצאה**.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-128">**Transaction type** is set to **Expense**.</span></span>

<span data-ttu-id="f2e2b-129">האיור הבא מראה כיצד הנתונים מסונכרנים בין Project Service Automation ו- Finance.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-129">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="f2e2b-130">[![זרימת נתונים לשילוב Project Service Automation עם Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="f2e2b-130">[![Data flow for Project Service Automation integration with Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span></span>

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a><span data-ttu-id="f2e2b-131">סנכרון קטגוריית הוצאה בפרוייקט מ- Finance אל Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="f2e2b-131">Project expense category synchronization from Finance to Project Service Automation</span></span>

### <a name="template-and-task"></a><span data-ttu-id="f2e2b-132">תבנית ומשימה</span><span class="sxs-lookup"><span data-stu-id="f2e2b-132">Template and task</span></span>

<span data-ttu-id="f2e2b-133">כדי לגשת לתבנית, במרכז הניהול של Microsoft Power Apps, בחר **פרוייקטים** ולאחר מכן, בפינה העליונה, בחר **פרוייקט חדש** כדי לבחור תבניות ציבוריות.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-133">To access the template, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="f2e2b-134">התבנית והמשימה הבסיסית הבאות משמשות לסנכרון קטגוריות של הוצאות בפרוייקט מ- Finance אל Project Service Automation:</span><span class="sxs-lookup"><span data-stu-id="f2e2b-134">The following template and underlying task are used to synchronize project expense categories from Finance to Project Service Automation:</span></span>

- <span data-ttu-id="f2e2b-135">**שם התבנית בשילוב נתונים:** קטגוריות של עסקאות הוצאות בפרוייקט (Fin and Ops ל- PSA)</span><span class="sxs-lookup"><span data-stu-id="f2e2b-135">**Name of the template in Data integration:** Project expense transaction categories (Fin and Ops to PSA)</span></span>
- <span data-ttu-id="f2e2b-136">**שם המשימה בפרוייקט:** סנכרון קטגוריות ל- PSA</span><span class="sxs-lookup"><span data-stu-id="f2e2b-136">**Name of the task in the project:** Sync categories to PSA</span></span>

### <a name="entity-set"></a><span data-ttu-id="f2e2b-137">קבוצת ישויות</span><span class="sxs-lookup"><span data-stu-id="f2e2b-137">Entity set</span></span>

| <span data-ttu-id="f2e2b-138">כספים</span><span class="sxs-lookup"><span data-stu-id="f2e2b-138">Finance</span></span>                           | <span data-ttu-id="f2e2b-139">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="f2e2b-139">Project Service Automation</span></span> |
|-----------------------------------|----------------------------|
| <span data-ttu-id="f2e2b-140">ישות שילוב לקטגוריות</span><span class="sxs-lookup"><span data-stu-id="f2e2b-140">Integration entity for categories</span></span> | <span data-ttu-id="f2e2b-141">קטגוריות עסקה</span><span class="sxs-lookup"><span data-stu-id="f2e2b-141">Transaction categories</span></span>     |

### <a name="entity-flow"></a><span data-ttu-id="f2e2b-142">זרימת ישות</span><span class="sxs-lookup"><span data-stu-id="f2e2b-142">Entity flow</span></span>

<span data-ttu-id="f2e2b-143">קטגוריות של הוצאות בפרוייקט מנוהלות ב- Finance והן מסונכרנות ל- Project Service Automation כקטגוריות של עסקאות.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-143">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="f2e2b-144">Power Query</span><span class="sxs-lookup"><span data-stu-id="f2e2b-144">Power Query</span></span>

<span data-ttu-id="f2e2b-145">בעת סנכרון ל- Project Service Automation, עליך להשתמש ב- Microsoft Power Query for Excel כדי לקבוע את סוג החיוב בקטגוריית העסקה.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-145">When you're synchronizing to Project Service Automation, you must use Microsoft Power Query for Excel to set the billing type on the transaction category.</span></span> <span data-ttu-id="f2e2b-146">התבנית קטגוריות של עסקאות הוצאות בפרוייקט (Fin and Ops ל- PSA) מספק עמודה ומיפוי בברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-146">The Project expense transaction categories (Fin and Ops to PSA) template provides a default column and mapping.</span></span> <span data-ttu-id="f2e2b-147">אם אתה יוצר תבנית משלך, עליך להוסיף עמודה מותנית ב- Power Query.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-147">If you create your own template, you must add a conditional column in Power Query.</span></span> <span data-ttu-id="f2e2b-148">פעל בהתאם לשלבים אלה.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-148">Follow these steps.</span></span>

1. <span data-ttu-id="f2e2b-149">לחץ על החץ כדי לפתוח את המיפוי של משימת הקטגוריות של הוצאות בפרוייקט בתבנית קטגוריות עסקאות של הוצאות הפרוייקט (Fin and Ops ל- PSA).</span><span class="sxs-lookup"><span data-stu-id="f2e2b-149">Click the arrow to open the mapping of the project expense categories task in the Project expense transaction categories (Fin and Ops to PSA) template.</span></span>
2. <span data-ttu-id="f2e2b-150">לחץ על הקישור **שאילתות וסינון מתקדמים** כדי לפתוח את Power Query.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-150">Click the **Advance Query and Filtering** link to open Power Query.</span></span>
2. <span data-ttu-id="f2e2b-151">בחר **הוסף עמודה מותנית**.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-151">Select **Add Conditional Column**.</span></span>
3. <span data-ttu-id="f2e2b-152">הזן שם לעמודה החדשה, כגון **BillingType**.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-152">Enter a name for the new column, such as **BillingType**.</span></span>
4. <span data-ttu-id="f2e2b-153">הזן את התנאי הבא: **אם CATEGORYID לא שווה ל- Null אז 19235001, אחרת Null**.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-153">Enter the following condition: **if CATEGORYID not equal to null then 19235001, Otherwise null**.</span></span>
5. <span data-ttu-id="f2e2b-154">לחץ על **אישור** בעמודה.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-154">Click **OK** on the column.</span></span>
6. <span data-ttu-id="f2e2b-155">הקפד למפות את העמודה החדשה הזו בדף המיפוי.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-155">Be sure to map this new column on the mapping page.</span></span>

<span data-ttu-id="f2e2b-156">האיור הבא מציג דוגמה למיפוי משימת התבנית בשילוב נתונים.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-156">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="f2e2b-157">המיפוי מציג את פרטי השדה שיסונכרנו מ- Finance ל- Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-157">The mapping shows the field information that will be synchronized from Finance to Project Service Automation.</span></span>

<span data-ttu-id="f2e2b-158">[![מיפוי תבנית](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="f2e2b-158">[![Template mapping](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span></span>

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a><span data-ttu-id="f2e2b-159">סנכרון קטגוריית הוצאה בפרוייקט מ- Project Service Automation אל Finance</span><span class="sxs-lookup"><span data-stu-id="f2e2b-159">Project expense category synchronization from Project Service Automation to Finance</span></span>

### <a name="template-and-task"></a><span data-ttu-id="f2e2b-160">תבנית ומשימה</span><span class="sxs-lookup"><span data-stu-id="f2e2b-160">Template and task</span></span>

<span data-ttu-id="f2e2b-161">התבנית והמשימה הבסיסית הבאות משמשות לסנכרון קטגוריות של הוצאות בפרוייקט מ- Project Service Automation אל Finance:</span><span class="sxs-lookup"><span data-stu-id="f2e2b-161">The following template and underlying task are used to synchronize project expense categories from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="f2e2b-162">**שם התבנית בשילוב נתונים:** קטגוריות של עסקאות הוצאות בפרוייקט (PSA ל- Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="f2e2b-162">**Name of the template in Data integration:** Project expense transaction categories (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="f2e2b-163">**שם המשימה בפרוייקט:** סנכרון קטגוריות ל- Fin and Ops</span><span class="sxs-lookup"><span data-stu-id="f2e2b-163">**Name of the task in the project:** Sync categories to Fin Ops</span></span>

### <a name="entity-set"></a><span data-ttu-id="f2e2b-164">קבוצת ישויות</span><span class="sxs-lookup"><span data-stu-id="f2e2b-164">Entity set</span></span>

| <span data-ttu-id="f2e2b-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="f2e2b-165">Project Service Automation</span></span> | <span data-ttu-id="f2e2b-166">כספים</span><span class="sxs-lookup"><span data-stu-id="f2e2b-166">Finance</span></span>                           |
|----------------------------|-----------------------------------|
| <span data-ttu-id="f2e2b-167">קטגוריות עסקה</span><span class="sxs-lookup"><span data-stu-id="f2e2b-167">Transaction categories</span></span>     | <span data-ttu-id="f2e2b-168">ישות שילוב לקטגוריות</span><span class="sxs-lookup"><span data-stu-id="f2e2b-168">Integration entity for categories</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="f2e2b-169">זרימת ישות</span><span class="sxs-lookup"><span data-stu-id="f2e2b-169">Entity flow</span></span>

<span data-ttu-id="f2e2b-170">קטגוריות של הוצאות בפרוייקט מנוהלות ב- Finance והן מסונכרנות ל- Project Service Automation כקטגוריות של עסקאות.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-170">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span> <span data-ttu-id="f2e2b-171">הסנכרון בחזרה אל Finance מעדכן את קטגוריית הפרוייקט ב- Finance עם מזהה השילוב מ- Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-171">The synchronization back to Finance updates the project category in Finance with the integration ID from Project Service Automation.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="f2e2b-172">מיפוי תבנית בשילוב נתונים</span><span class="sxs-lookup"><span data-stu-id="f2e2b-172">Template mapping in Data integration</span></span>

<span data-ttu-id="f2e2b-173">האיור הבא מציג דוגמה למיפוי משימת התבנית בשילוב נתונים.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-173">The following illustration shows an example of the template task mapping in Data integration.</span></span>

> [!NOTE]
> <span data-ttu-id="f2e2b-174">המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="f2e2b-174">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="f2e2b-175">[![מיפוי תבנית](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="f2e2b-175">[![Template mapping](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span></span>
