---
title: סנכרון קטגוריות של הוצאות בפרויקט בין Finance and Operations ו- Project Service Automation
description: נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון קטגוריות של הוצאות בפרויקט בין Microsoft Dynamics 365 Finance ו- Dynamics 365 Project Service Automation.
author: Yowelle
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: 2816d363dbfe6ef2d98a584b214f72d9b30c49bb
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999852"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a><span data-ttu-id="a4915-103">סנכרון קטגוריות של הוצאות בפרויקט בין Finance and Operations ו- Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="a4915-103">Synchronize project expense categories between Finance and Operations and Project Service Automation</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="a4915-104">נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון קטגוריות של הוצאות בפרויקט בין Dynamics 365 Finance ו- Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="a4915-104">This topic describes the templates and underlying tasks that are used to synchronize project expense categories between Dynamics 365 Finance and Dynamics 365 Project Service Automation.</span></span>

> [!NOTE]
> - <span data-ttu-id="a4915-105">שילוב משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונעילת פונקציונליות זמינים בגירסה 8.0.</span><span class="sxs-lookup"><span data-stu-id="a4915-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="a4915-106">שילוב נתונים בפועל זמין בגירסה 8.0.1 ואילך.</span><span class="sxs-lookup"><span data-stu-id="a4915-106">Actuals integration is available in version 8.0.1 or later.</span></span>
> - <span data-ttu-id="a4915-107">אם אתה משתמש ב- Enterprise Edition 7.3.0, לאחר התקנת KB 4132657 ו- KB 4132660, תוכל להשתמש בתבניות לשילוב משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונתונים בפועל, וכן להגדיר תצורה של נעילת פונקציונליות.</span><span class="sxs-lookup"><span data-stu-id="a4915-107">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="a4915-108">אם עליך לאפס את ההפצות החשבונאיות, מומלץ להתקין גם את KB 4131710.</span><span class="sxs-lookup"><span data-stu-id="a4915-108">If you must reset the accounting distributions, we recommend that you also install KB 4131710.</span></span>

## <a name="data-flow-for-project-service-automation-and-finance"></a><span data-ttu-id="a4915-109">זרימת נתונים עבור Project Service Automation ו- Finance</span><span class="sxs-lookup"><span data-stu-id="a4915-109">Data flow for Project Service Automation and Finance</span></span>

<span data-ttu-id="a4915-110">פתרון השילוב Project Service Automation ו- Finance משתמש בתכונת שילוב הנתונים לסנכרון נתונים במופעים של Project Service Automation ו- Finance.</span><span class="sxs-lookup"><span data-stu-id="a4915-110">The Project Service Automation and Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="a4915-111">תבניות השילוב שזמינות עם תכונת שילוב הנתונים מאפשרות זרימת נתונים על קטגוריות של עסקאות הוצאה בפרויקט ובין Finance ו- Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="a4915-111">The integration templates that are available with the Data integration feature enable the flow of data about project expense transaction categories between Finance and Project Service Automation.</span></span>

<span data-ttu-id="a4915-112">אם הקטגוריות של הוצאות בפרויקט נשלטות ב- Finance, זרימת השילוב תהיה ראשונה מ- Finance אל Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="a4915-112">If the project expense categories are mastered in Finance, the integration flow is first from Finance to Project Service Automation.</span></span> <span data-ttu-id="a4915-113">מזהי השילוב של קטגוריות הוצאות בפרויקט מתעדכנים לאחר מכן באמצעות סנכרון מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="a4915-113">The integration IDs of the project expense categories are then updated through synchronization from Project Service Automation to Finance.</span></span>

<span data-ttu-id="a4915-114">אם הקטגוריות של הוצאות בפרויקט נשלטות ב- Project Service Automation, זרימת השילוב תהיה ראשונה מ- Project Service Automation אל Finance.</span><span class="sxs-lookup"><span data-stu-id="a4915-114">If the project expense categories are mastered in Project Service Automation, the integration flow is first from Project Service Automation to Finance.</span></span> <span data-ttu-id="a4915-115">יש להגדיר את קטגוריות הפרויקט כבר ב- Finance לפני הסינכרון מ- Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="a4915-115">The project categories must already be configured in Finance before the synchronization from Project Service Automation.</span></span> <span data-ttu-id="a4915-116">לאחר מכן סנכרן מ- Finance בחזרה ל- Project Service Automation, ואז מ- Project Service Automation ל- Finance שוב.</span><span class="sxs-lookup"><span data-stu-id="a4915-116">Then synchronize from Finance back to Project Service Automation, and then from Project Service Automation to Finance again.</span></span> <span data-ttu-id="a4915-117">באופן זה, אתה עוזר להבטיח שהקטגוריות יהיו מקושרות ושלא ייווצרו כפילויות.</span><span class="sxs-lookup"><span data-stu-id="a4915-117">In this way, you help guarantee that the categories are linked, and that no duplicates are created.</span></span>

> [!NOTE]
> <span data-ttu-id="a4915-118">בדרך כלל, קטגוריות של הוצאות בפרויקט נשלטות ב- Finance.</span><span class="sxs-lookup"><span data-stu-id="a4915-118">Typically, the project expense categories are mastered in Finance.</span></span> <span data-ttu-id="a4915-119">עם זאת, אם הן לא נשלטות משם, או אם הקטגוריות של ההוצאות כבר נוצרו ב- Project Service Automation, עליך תחילה לסנכרן באמצעות תבנית קטגוריות של עסקאות הוצאות בפרויקט (PSA ל- Fin and Ops).</span><span class="sxs-lookup"><span data-stu-id="a4915-119">However, if they aren't, or if expense categories have already been created in Project Service Automation, you must first synchronize by using the Project expense transaction categories (PSA to Fin and Ops) template.</span></span> <span data-ttu-id="a4915-120">לאחר מכן סנכרן באמצעות תבנית הקטגוריות של עסקאות הוצאות בפרויקט (Fin and Ops ל- PSA).</span><span class="sxs-lookup"><span data-stu-id="a4915-120">Then synchronize by using the Project expense transaction categories (Fin and Ops to PSA) template.</span></span> <span data-ttu-id="a4915-121">לאחר מכן עליך להפעיל את הסנכרון מ- Project Service Automation ל- Finance פעם נוספת.</span><span class="sxs-lookup"><span data-stu-id="a4915-121">You should then run the synchronization from Project Service Automation to Finance one more time.</span></span>
>
> <span data-ttu-id="a4915-122">אם אתה מסנכרן תחילה מ- Project Service Automation, יש לעמוד בדרישות הבאות ב- Finance לפני הפעלת הסנכרון:</span><span class="sxs-lookup"><span data-stu-id="a4915-122">If you synchronize first from Project Service Automation, the following requirements must be met in Finance before the synchronization is run:</span></span>
>
> - <span data-ttu-id="a4915-123">הקטגוריה המשותפת שתואמת לקטגוריית הפרויקט שמוגדרת ב- Project Service Automation חייבת להתקיים, והיא חייבת להיות מופעלת גם עבור **פרויקט** וגם עבור **הוצאה**.</span><span class="sxs-lookup"><span data-stu-id="a4915-123">The shared category that matches the project category that is set up in Project Service Automation must exist, and it must be enabled for both **Project** and **Expense**.</span></span>
> - <span data-ttu-id="a4915-124">עבור כל ישות משפטית ב- Finance שבה יש לשלב, קטגוריות הפרויקט הבאות חייבות להתקיים:</span><span class="sxs-lookup"><span data-stu-id="a4915-124">For each Finance legal entity that must be integrated with, the following project categories must exist:</span></span>
>
>     - <span data-ttu-id="a4915-125">**קטגוריית פרויקט** קיימת.</span><span class="sxs-lookup"><span data-stu-id="a4915-125">**Project category** exists.</span></span> 
>     - <span data-ttu-id="a4915-126">האפשרות **השתמש בהוצאה** זמינה.</span><span class="sxs-lookup"><span data-stu-id="a4915-126">**Use in Expense** is enabled.</span></span>
>     - <span data-ttu-id="a4915-127">האפשרות **פעיל ביומן** זמינה.</span><span class="sxs-lookup"><span data-stu-id="a4915-127">**Active in journal** is enabled.</span></span>
>     - <span data-ttu-id="a4915-128">**סוג עסקה** נקבעה בתור **הוצאה**.</span><span class="sxs-lookup"><span data-stu-id="a4915-128">**Transaction type** is set to **Expense**.</span></span>

<span data-ttu-id="a4915-129">האיור הבא מראה כיצד הנתונים מסונכרנים בין Project Service Automation ו- Finance.</span><span class="sxs-lookup"><span data-stu-id="a4915-129">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="a4915-130">[![זרימת נתונים לשילוב Project Service Automation עם Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="a4915-130">[![Data flow for Project Service Automation integration with Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span></span>

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a><span data-ttu-id="a4915-131">סנכרון קטגוריית הוצאה בפרויקט מ- Finance אל Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="a4915-131">Project expense category synchronization from Finance to Project Service Automation</span></span>

### <a name="template-and-task"></a><span data-ttu-id="a4915-132">תבנית ומשימה</span><span class="sxs-lookup"><span data-stu-id="a4915-132">Template and task</span></span>

<span data-ttu-id="a4915-133">כדי לגשת לתבנית, במרכז הניהול של Microsoft Power Apps, בחר **פרויקטים** ולאחר מכן, בפינה העליונה, בחר **פרויקט חדש** כדי לבחור תבניות ציבוריות.</span><span class="sxs-lookup"><span data-stu-id="a4915-133">To access the template, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="a4915-134">התבנית והמשימה הבסיסית הבאות משמשות לסנכרון קטגוריות של הוצאות בפרויקט מ- Finance אל Project Service Automation:</span><span class="sxs-lookup"><span data-stu-id="a4915-134">The following template and underlying task are used to synchronize project expense categories from Finance to Project Service Automation:</span></span>

- <span data-ttu-id="a4915-135">**שם התבנית בשילוב נתונים:** קטגוריות של עסקאות הוצאות בפרויקט (Fin and Ops ל- PSA)</span><span class="sxs-lookup"><span data-stu-id="a4915-135">**Name of the template in Data integration:** Project expense transaction categories (Fin and Ops to PSA)</span></span>
- <span data-ttu-id="a4915-136">**שם המשימה בפרויקט:** סנכרון קטגוריות ל- PSA</span><span class="sxs-lookup"><span data-stu-id="a4915-136">**Name of the task in the project:** Sync categories to PSA</span></span>

### <a name="entity-set"></a><span data-ttu-id="a4915-137">קבוצת ישויות</span><span class="sxs-lookup"><span data-stu-id="a4915-137">Entity set</span></span>

| <span data-ttu-id="a4915-138">כספים</span><span class="sxs-lookup"><span data-stu-id="a4915-138">Finance</span></span>                           | <span data-ttu-id="a4915-139">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="a4915-139">Project Service Automation</span></span> |
|-----------------------------------|----------------------------|
| <span data-ttu-id="a4915-140">ישות שילוב לקטגוריות</span><span class="sxs-lookup"><span data-stu-id="a4915-140">Integration entity for categories</span></span> | <span data-ttu-id="a4915-141">קטגוריות עסקה</span><span class="sxs-lookup"><span data-stu-id="a4915-141">Transaction categories</span></span>     |

### <a name="entity-flow"></a><span data-ttu-id="a4915-142">זרימת ישות</span><span class="sxs-lookup"><span data-stu-id="a4915-142">Entity flow</span></span>

<span data-ttu-id="a4915-143">קטגוריות של הוצאות בפרויקט מנוהלות ב- Finance והן מסונכרנות ל- Project Service Automation כקטגוריות של עסקאות.</span><span class="sxs-lookup"><span data-stu-id="a4915-143">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="a4915-144">Power Query</span><span class="sxs-lookup"><span data-stu-id="a4915-144">Power Query</span></span>

<span data-ttu-id="a4915-145">בעת סנכרון ל- Project Service Automation, עליך להשתמש ב- Microsoft Power Query for Excel כדי לקבוע את סוג החיוב בקטגוריית העסקה.</span><span class="sxs-lookup"><span data-stu-id="a4915-145">When you're synchronizing to Project Service Automation, you must use Microsoft Power Query for Excel to set the billing type on the transaction category.</span></span> <span data-ttu-id="a4915-146">התבנית קטגוריות של עסקאות הוצאות בפרויקט (Fin and Ops ל- PSA) מספק עמודה ומיפוי בברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="a4915-146">The Project expense transaction categories (Fin and Ops to PSA) template provides a default column and mapping.</span></span> <span data-ttu-id="a4915-147">אם אתה יוצר תבנית משלך, עליך להוסיף עמודה מותנית ב- Power Query.</span><span class="sxs-lookup"><span data-stu-id="a4915-147">If you create your own template, you must add a conditional column in Power Query.</span></span> <span data-ttu-id="a4915-148">פעל בהתאם לשלבים אלה.</span><span class="sxs-lookup"><span data-stu-id="a4915-148">Follow these steps.</span></span>

1. <span data-ttu-id="a4915-149">לחץ על החץ כדי לפתוח את המיפוי של משימת הקטגוריות של הוצאות בפרויקט בתבנית קטגוריות עסקאות של הוצאות הפרויקט (Fin and Ops ל- PSA).</span><span class="sxs-lookup"><span data-stu-id="a4915-149">Click the arrow to open the mapping of the project expense categories task in the Project expense transaction categories (Fin and Ops to PSA) template.</span></span>
2. <span data-ttu-id="a4915-150">לחץ על הקישור **שאילתות וסינון מתקדמים** כדי לפתוח את Power Query.</span><span class="sxs-lookup"><span data-stu-id="a4915-150">Click the **Advance Query and Filtering** link to open Power Query.</span></span>
2. <span data-ttu-id="a4915-151">בחר **הוסף עמודה מותנית**.</span><span class="sxs-lookup"><span data-stu-id="a4915-151">Select **Add Conditional Column**.</span></span>
3. <span data-ttu-id="a4915-152">הזן שם לעמודה החדשה, כגון **BillingType**.</span><span class="sxs-lookup"><span data-stu-id="a4915-152">Enter a name for the new column, such as **BillingType**.</span></span>
4. <span data-ttu-id="a4915-153">הזן את התנאי הבא: **אם CATEGORYID לא שווה ל- Null אז 19235001, אחרת Null**.</span><span class="sxs-lookup"><span data-stu-id="a4915-153">Enter the following condition: **if CATEGORYID not equal to null then 19235001, Otherwise null**.</span></span>
5. <span data-ttu-id="a4915-154">לחץ על **אישור** בעמודה.</span><span class="sxs-lookup"><span data-stu-id="a4915-154">Click **OK** on the column.</span></span>
6. <span data-ttu-id="a4915-155">הקפד למפות את העמודה החדשה הזו בדף המיפוי.</span><span class="sxs-lookup"><span data-stu-id="a4915-155">Be sure to map this new column on the mapping page.</span></span>

<span data-ttu-id="a4915-156">האיור הבא מציג דוגמה למיפוי משימת התבנית בשילוב נתונים.</span><span class="sxs-lookup"><span data-stu-id="a4915-156">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="a4915-157">המיפוי מציג את פרטי השדה שיסונכרנו מ- Finance ל- Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="a4915-157">The mapping shows the field information that will be synchronized from Finance to Project Service Automation.</span></span>

<span data-ttu-id="a4915-158">[![קטגוריית הוצאה בפרויקט למיפוי תבנית של Project Service Automation](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="a4915-158">[![Project expense category to Project Service Automation template mapping](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span></span>

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a><span data-ttu-id="a4915-159">סנכרון קטגוריית הוצאה בפרויקט מ- Project Service Automation אל Finance</span><span class="sxs-lookup"><span data-stu-id="a4915-159">Project expense category synchronization from Project Service Automation to Finance</span></span>

### <a name="template-and-task"></a><span data-ttu-id="a4915-160">תבנית ומשימה</span><span class="sxs-lookup"><span data-stu-id="a4915-160">Template and task</span></span>

<span data-ttu-id="a4915-161">התבנית והמשימה הבסיסית הבאות משמשות לסנכרון קטגוריות של הוצאות בפרויקט מ- Project Service Automation אל Finance:</span><span class="sxs-lookup"><span data-stu-id="a4915-161">The following template and underlying task are used to synchronize project expense categories from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="a4915-162">**שם התבנית בשילוב נתונים:** קטגוריות של עסקאות הוצאות בפרויקט (PSA ל- Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="a4915-162">**Name of the template in Data integration:** Project expense transaction categories (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="a4915-163">**שם המשימה בפרויקט:** סנכרון קטגוריות ל- Fin and Ops</span><span class="sxs-lookup"><span data-stu-id="a4915-163">**Name of the task in the project:** Sync categories to Fin Ops</span></span>

### <a name="entity-set"></a><span data-ttu-id="a4915-164">קבוצת ישויות</span><span class="sxs-lookup"><span data-stu-id="a4915-164">Entity set</span></span>

| <span data-ttu-id="a4915-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="a4915-165">Project Service Automation</span></span> | <span data-ttu-id="a4915-166">כספים</span><span class="sxs-lookup"><span data-stu-id="a4915-166">Finance</span></span>                           |
|----------------------------|-----------------------------------|
| <span data-ttu-id="a4915-167">קטגוריות עסקה</span><span class="sxs-lookup"><span data-stu-id="a4915-167">Transaction categories</span></span>     | <span data-ttu-id="a4915-168">ישות שילוב לקטגוריות</span><span class="sxs-lookup"><span data-stu-id="a4915-168">Integration entity for categories</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="a4915-169">זרימת ישות</span><span class="sxs-lookup"><span data-stu-id="a4915-169">Entity flow</span></span>

<span data-ttu-id="a4915-170">קטגוריות של הוצאות בפרויקט מנוהלות ב- Finance והן מסונכרנות ל- Project Service Automation כקטגוריות של עסקאות.</span><span class="sxs-lookup"><span data-stu-id="a4915-170">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span> <span data-ttu-id="a4915-171">הסנכרון בחזרה אל Finance מעדכן את קטגוריית הפרויקט ב- Finance עם מזהה השילוב מ- Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="a4915-171">The synchronization back to Finance updates the project category in Finance with the integration ID from Project Service Automation.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="a4915-172">מיפוי תבנית בשילוב נתונים</span><span class="sxs-lookup"><span data-stu-id="a4915-172">Template mapping in Data integration</span></span>

<span data-ttu-id="a4915-173">האיור הבא מציג דוגמה למיפוי משימת התבנית בשילוב נתונים.</span><span class="sxs-lookup"><span data-stu-id="a4915-173">The following illustration shows an example of the template task mapping in Data integration.</span></span>

> [!NOTE]
> <span data-ttu-id="a4915-174">המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="a4915-174">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="a4915-175">[![Project Service Automation למיפוי תבנית Finance](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="a4915-175">[![Project Service Automation to Finance template mapping](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]