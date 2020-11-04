---
title: סנכרון הערכות פרויקטים ישירות מ- Project Service Automation ל- Finance and Operations
description: נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון הערכת שעות בפרויקט והערכת הוצאות בפרויקט ישירות מ- Microsoft Dynamics 365 Project Service Automation אל Dynamics 365 Finance.
author: Yowelle
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
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 336de474c859d30d1ec07ae34bf0c3d578faeef1
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077436"
---
# <a name="synchronize-project-estimates-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="88d62-103">סנכרון הערכות פרויקטים ישירות מ- Project Service Automation ל- Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="88d62-103">Synchronize project estimates directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="88d62-104">נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון הערכת שעות בפרויקט והערכת הוצאות בפרויקט ישירות מ- Dynamics 365 Project Service Automation אל Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="88d62-104">This topic describes the templates and underlying tasks that are used to synchronize project hour estimates and project expense estimates directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="88d62-105">שילוב משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונעילת פונקציונליות זמינים בגירסה 8.0.</span><span class="sxs-lookup"><span data-stu-id="88d62-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking is available in version 8.0.</span></span>
> - <span data-ttu-id="88d62-106">שילוב נתונים בפועל זמין בגירסה 8.0.1 ואילך.</span><span class="sxs-lookup"><span data-stu-id="88d62-106">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="88d62-107">זרימת נתונים עבור Project Service Automation ל- Finance</span><span class="sxs-lookup"><span data-stu-id="88d62-107">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="88d62-108">פתרון השילוב Project Service Automation ל- Finance משתמש בתכונת שילוב הנתונים לסנכרון נתונים במופעים של Project Service Automation ו- Finance.</span><span class="sxs-lookup"><span data-stu-id="88d62-108">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="88d62-109">תבניות השילוב שזמינות עם תכונת שילוב הנתונים מאפשרות זרימת נתונים על הערכת שעות בפרויקט והערכת הוצאות בפרויקט מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="88d62-109">The integration templates that are available with the Data integration feature enable the flow of data about project hour estimates and project expense estimates from Project Service Automation to Finance.</span></span>

<span data-ttu-id="88d62-110">האיור הבא מראה כיצד הנתונים מסונכרנים בין Project Service Automation ו- Finance.</span><span class="sxs-lookup"><span data-stu-id="88d62-110">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="88d62-111">[![זרימת נתונים לשילוב Project Service Automation עם Finance](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="88d62-111">[![Data flow for Project Service Automation integration with Finance](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span></span>

## <a name="project-hour-estimates"></a><span data-ttu-id="88d62-112">הערכת שעות בפרויקט</span><span class="sxs-lookup"><span data-stu-id="88d62-112">Project hour estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="88d62-113">תבנית ומשימות</span><span class="sxs-lookup"><span data-stu-id="88d62-113">Template and tasks</span></span>

<span data-ttu-id="88d62-114">כדי לגשת לתבניות הזמינות, במרכז הניהול של Microsoft Power Apps, בחר **פרויקטים** ולאחר מכן, בפינה העליונה, בחר **פרויקט חדש** כדי לבחור תבניות ציבוריות.</span><span class="sxs-lookup"><span data-stu-id="88d62-114">To access the available templates, in the Microsoft Power Apps admin center, select **Projects** , and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="88d62-115">התבנית והמשימות הבסיסיות הבאות משמשות לסנכרון הערכת שעות בפרויקט מ- Project Service Automation אל Finance:</span><span class="sxs-lookup"><span data-stu-id="88d62-115">The following template and underlying tasks are used to synchronize project hour estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="88d62-116">**שם התבנית בשילוב נתונים:** הערכת שעות בפרויקט (PSA ל- Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="88d62-116">**Name of the template in Data integration:** Project hour estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="88d62-117">**שם המשימות בפרויקט:**</span><span class="sxs-lookup"><span data-stu-id="88d62-117">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="88d62-118">יחסי גומלין של עסקה</span><span class="sxs-lookup"><span data-stu-id="88d62-118">Transaction relationships</span></span>
    - <span data-ttu-id="88d62-119">הערכות הוצאות</span><span class="sxs-lookup"><span data-stu-id="88d62-119">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="88d62-120">קבוצת ישויות</span><span class="sxs-lookup"><span data-stu-id="88d62-120">Entity set</span></span>

| <span data-ttu-id="88d62-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="88d62-121">Project Service Automation</span></span> | <span data-ttu-id="88d62-122">כספים</span><span class="sxs-lookup"><span data-stu-id="88d62-122">Finance</span></span>                                       |
|----------------------------|-----------------------------------------------|
| <span data-ttu-id="88d62-123">משימות פרויקט</span><span class="sxs-lookup"><span data-stu-id="88d62-123">Project tasks</span></span>              | <span data-ttu-id="88d62-124">ישות שילוב להערכת שעות בפרויקט</span><span class="sxs-lookup"><span data-stu-id="88d62-124">Integration entity for project hour estimates</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="88d62-125">זרימת ישות</span><span class="sxs-lookup"><span data-stu-id="88d62-125">Entity flow</span></span>

<span data-ttu-id="88d62-126">הערכות של שעות בפרויקט מנוהלים ב- Project Service Automation והן מסונכרנות ל- Finance כתחזיות לשעות בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="88d62-126">Project hour estimates are managed in Project Service Automation, and they are synchronized to Finance as project hour forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="88d62-127">דרישות מוקדמות</span><span class="sxs-lookup"><span data-stu-id="88d62-127">Prerequisites</span></span>

<span data-ttu-id="88d62-128">לפני שתוכל לסנכרן הערכת שעות בפרויקט, עליך לסנכרן פרויקטים, משימות פרויקט וקטגוריות של עסקאות הוצאות בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="88d62-128">Before synchronization of project hour estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="88d62-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="88d62-129">Power Query</span></span>

<span data-ttu-id="88d62-130">בתבנית הערכת שעות בפרויקט, עליך להשתמש ב- Microsoft Power Query for Excel כדי להשלים את המשימות הבאות:</span><span class="sxs-lookup"><span data-stu-id="88d62-130">In the project hour estimates template, you must use Microsoft Power Query for Excel to complete these tasks:</span></span>

- <span data-ttu-id="88d62-131">הגדר את מזהה מודל תחזית ברירת המחדל שישמש כאשר השילוב יוצר תחזיות חדשות לשעות.</span><span class="sxs-lookup"><span data-stu-id="88d62-131">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="88d62-132">סנן רשומות שספציפיות למשאבים במשימה אשר יכשלו בשילוב בתוך תחזיות השעות.</span><span class="sxs-lookup"><span data-stu-id="88d62-132">Filter out any resource-specific records in the task that will fail the integration into hour forecasts.</span></span>
- <span data-ttu-id="88d62-133">סנן כל שורה ריקה בקטגוריית עסקה.</span><span class="sxs-lookup"><span data-stu-id="88d62-133">Filter out any empty transaction category rows.</span></span> <span data-ttu-id="88d62-134">אי השלמת המשימה עשויה להוביל לתחזית שעות שגויה.</span><span class="sxs-lookup"><span data-stu-id="88d62-134">Failure to complete this task might result in incorrect hour forecasts.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="88d62-135">הגדר את מזהה מודל התחזית בברירת מחדל</span><span class="sxs-lookup"><span data-stu-id="88d62-135">Set the default forecast model ID</span></span>

<span data-ttu-id="88d62-136">כדי לעדכן את מזהה מודל התחזית בברירת מחדל בתבנית, לחץ על החץ **מפה** כדי לפתוח את המיפוי.</span><span class="sxs-lookup"><span data-stu-id="88d62-136">To update the default forecast model ID in the template, click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="88d62-137">לאחר מכן, בחר בקישור **שאילתות וסינון מתקדמים**.</span><span class="sxs-lookup"><span data-stu-id="88d62-137">Then select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="88d62-138">אם אתה משתמש בתבנית ברירת מחדל להערכת השעות בפרויקט (PSA ל- Fin and Ops), בחר באפשרות **תנאי שהוכנס** ברשימה **שלבים שהוחלו**.</span><span class="sxs-lookup"><span data-stu-id="88d62-138">If you're using the default Project hour estimates (PSA to Fin and Ops) template, select the **Inserted Condition** in the list of **Applied Steps**.</span></span> <span data-ttu-id="88d62-139">בערך **פונקציה** , החלף את **O\_forecast** בשם של מזהה מודל התחזית שבו יש להשתמש בשילוב.</span><span class="sxs-lookup"><span data-stu-id="88d62-139">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="88d62-140">לתבנית ברירת המחדל יש מזהה מודל תחזית מנתוני ההדגמה.</span><span class="sxs-lookup"><span data-stu-id="88d62-140">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="88d62-141">אם אתה יוצר תבנית חדשה, עליך להוסיף עמודה זו.</span><span class="sxs-lookup"><span data-stu-id="88d62-141">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="88d62-142">ב- Power Query, בחר **הוסף עמודה מותנית** והזן שם לעמודה החדשה, כגון **ModelID**.</span><span class="sxs-lookup"><span data-stu-id="88d62-142">In Power Query, select **Add Conditional Column** , and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="88d62-143">הזן את התנאי עבור העמודה, שבה, אם משימה בפרויקט אינה Null, \<enter the forecast model ID\>; אחרת Null.</span><span class="sxs-lookup"><span data-stu-id="88d62-143">Enter the condition for the column, where, if Project task is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="filter-out-resource-specific-records"></a><span data-ttu-id="88d62-144">סנן רשומות שספציפיות למשאבים</span><span class="sxs-lookup"><span data-stu-id="88d62-144">Filter out resource-specific records</span></span>

<span data-ttu-id="88d62-145">לתבנית הערכת שעות בפרויקט (PSA ל- Fin and Ops) יש מסנן ברירת מחדל שמסיר כל רשומה שספציפית למשאבים.</span><span class="sxs-lookup"><span data-stu-id="88d62-145">The Project hour estimates (PSA to Fin and Ops) template has a default filter that removes any resource-specific records.</span></span> <span data-ttu-id="88d62-146">אם אתה יוצר תבנית משלך, עליך להוסיף מסנן זה.</span><span class="sxs-lookup"><span data-stu-id="88d62-146">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="88d62-147">בחר בקישור **שאילתות וסינון מתקדמים** כדי לסנן את העמודה **msdyn\_islinetask** כך שרק הרשומות שהן **False** יהיו כלולות.</span><span class="sxs-lookup"><span data-stu-id="88d62-147">Select the **Advanced Query and Filtering** link to filter on the **msdyn\_islinetask** column so that only **False** records are included.</span></span>

#### <a name="filter-out-empty-transaction-category-rows"></a><span data-ttu-id="88d62-148">סנן כל שורה ריקה בקטגוריית עסקה</span><span class="sxs-lookup"><span data-stu-id="88d62-148">Filter out empty transaction category rows</span></span>

<span data-ttu-id="88d62-149">עליך להוסיף מסנן כדי להסיר שורות שיש בהן קטגוריות של עסקאות ריקות.</span><span class="sxs-lookup"><span data-stu-id="88d62-149">You must add a filter to remove any rows that have empty transaction categories.</span></span> <span data-ttu-id="88d62-150">משימה זו נדרשת, בין אם אתה משתמש בתבנית ברירת המחדל או יוצר תבנית משלך.</span><span class="sxs-lookup"><span data-stu-id="88d62-150">This task is required, regardless of whether you're using the default template or creating your own template.</span></span> <span data-ttu-id="88d62-151">מסנן זה מסיר שורות סיכום מ- Project Service Automation העלולות לגרום לתחזיות השעות ב- Finance להיות שגויות.</span><span class="sxs-lookup"><span data-stu-id="88d62-151">This filter removes any summary rows from Project Service Automation that might cause the hour forecasts in Finance to be incorrect.</span></span> <span data-ttu-id="88d62-152">בחר בקישור **שאילתות וסינון מתקדמים** כדי לסנן רשומות שהן Null בעמודה **msdyn\_transactioncategory\_value**.</span><span class="sxs-lookup"><span data-stu-id="88d62-152">Select **Advanced Query and Filtering** link to filter out null records in the **msdyn\_transactioncategory\_value** column.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="88d62-153">מיפוי תבנית בשילוב נתונים</span><span class="sxs-lookup"><span data-stu-id="88d62-153">Template mapping in Data integration</span></span>

<span data-ttu-id="88d62-154">האיור הבא מציג דוגמה למיפוי משימת התבנית בשילוב נתונים.</span><span class="sxs-lookup"><span data-stu-id="88d62-154">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="88d62-155">המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="88d62-155">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="88d62-156">[![מיפוי משימת תבנית בשילוב נתונים](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="88d62-156">[![Template task mapping in data integration](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span></span>

## <a name="project-expense-estimates"></a><span data-ttu-id="88d62-157">הערכות הוצאה בפרויקט</span><span class="sxs-lookup"><span data-stu-id="88d62-157">Project expense estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="88d62-158">תבנית ומשימות</span><span class="sxs-lookup"><span data-stu-id="88d62-158">Template and tasks</span></span>

<span data-ttu-id="88d62-159">התבנית והמשימות הבסיסיות הבאות משמשות לסנכרון הערכת הוצאות בפרויקט מ- Project Service Automation אל Finance:</span><span class="sxs-lookup"><span data-stu-id="88d62-159">The following template and underlying tasks are used to synchronize project expense estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="88d62-160">**שם התבנית בשילוב נתונים:** הערכת הוצאות בפרויקט (PSA ל- Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="88d62-160">**Name of the template in Data integration:** Project expense estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="88d62-161">**שם המשימות בפרויקט:**</span><span class="sxs-lookup"><span data-stu-id="88d62-161">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="88d62-162">יחסי גומלין של עסקה</span><span class="sxs-lookup"><span data-stu-id="88d62-162">Transaction relationships</span></span> 
    - <span data-ttu-id="88d62-163">הערכות הוצאות</span><span class="sxs-lookup"><span data-stu-id="88d62-163">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="88d62-164">קבוצת ישויות</span><span class="sxs-lookup"><span data-stu-id="88d62-164">Entity set</span></span>

| <span data-ttu-id="88d62-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="88d62-165">Project Service Automation</span></span> | <span data-ttu-id="88d62-166">כספים</span><span class="sxs-lookup"><span data-stu-id="88d62-166">Finance</span></span>                                                  |
|----------------------------|----------------------------------------------------------|
| <span data-ttu-id="88d62-167">חיבורי עסקה</span><span class="sxs-lookup"><span data-stu-id="88d62-167">Transaction Connections</span></span>    | <span data-ttu-id="88d62-168">ישות שילוב ליחסי גומלין של עסקה בפרויקט</span><span class="sxs-lookup"><span data-stu-id="88d62-168">Integration entity for project transaction relationships</span></span> |
| <span data-ttu-id="88d62-169">שורות של הערכות</span><span class="sxs-lookup"><span data-stu-id="88d62-169">Estimate Lines</span></span>             | <span data-ttu-id="88d62-170">ישות שילוב להערכת הוצאות בפרויקט</span><span class="sxs-lookup"><span data-stu-id="88d62-170">Integration entity for project expense estimates</span></span>         |

### <a name="entity-flow"></a><span data-ttu-id="88d62-171">זרימת ישות</span><span class="sxs-lookup"><span data-stu-id="88d62-171">Entity flow</span></span>

<span data-ttu-id="88d62-172">הערכות של הוצאות בפרויקט מנוהלות ב- Project Service Automation והן מסונכרנות ל- Finance כתחזיות להוצאות בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="88d62-172">Project expense estimates are managed in Project Service Automation, and they are synchronized to Finance as project expense forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="88d62-173">דרישות מוקדמות</span><span class="sxs-lookup"><span data-stu-id="88d62-173">Prerequisites</span></span>

<span data-ttu-id="88d62-174">לפני שתוכל לסנכרן הערכת הוצאות בפרויקט, עליך לסנכרן פרויקטים, משימות פרויקט וקטגוריות של עסקאות הוצאות בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="88d62-174">Before synchronization of project expense estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="88d62-175">Power Query</span><span class="sxs-lookup"><span data-stu-id="88d62-175">Power Query</span></span>

<span data-ttu-id="88d62-176">בתבנית הערכת הוצאות בפרויקט, עליך להשתמש ב- Power Query כדי להשלים את המשימות הבאות:</span><span class="sxs-lookup"><span data-stu-id="88d62-176">In the project expense estimates template, you must use Power Query to complete the following tasks:</span></span>

- <span data-ttu-id="88d62-177">סנן כדי לכלול רק רשומות של שורת הערכת הוצאות.</span><span class="sxs-lookup"><span data-stu-id="88d62-177">Filter to include only expense estimate line records.</span></span>
- <span data-ttu-id="88d62-178">הגדר את מזהה מודל תחזית ברירת המחדל שישמש כאשר השילוב יוצר תחזיות חדשות לשעות.</span><span class="sxs-lookup"><span data-stu-id="88d62-178">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="88d62-179">שנה את סוגי החיובים.</span><span class="sxs-lookup"><span data-stu-id="88d62-179">Transform the billing types.</span></span>
- <span data-ttu-id="88d62-180">שנה את סוגי העסקאות.</span><span class="sxs-lookup"><span data-stu-id="88d62-180">Transform the transaction types.</span></span>

#### <a name="filter-to-include-only-expense-estimate-lines"></a><span data-ttu-id="88d62-181">סנן כדי לכלול רק שורות של הערכת הוצאות</span><span class="sxs-lookup"><span data-stu-id="88d62-181">Filter to include only expense estimate lines</span></span>

<span data-ttu-id="88d62-182">לתבנית הערכת הוצאות בפרויקט (PSA ל- Fin and Ops) יש מסנן ברירת מחדל הכולל רק שורות הוצאות בשילוב.</span><span class="sxs-lookup"><span data-stu-id="88d62-182">The Project expense estimates (PSA to Fin and Ops) template has a default filter that includes only expense lines in the integration.</span></span> <span data-ttu-id="88d62-183">אם אתה יוצר תבנית משלך, עליך להוסיף מסנן זה.</span><span class="sxs-lookup"><span data-stu-id="88d62-183">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="88d62-184">בחר במשימה **‏‫יחסי גומלין של עסקה‬** ולאחר מכן לחץ על החץ **מפה** כדי לפתח את המיפוי.</span><span class="sxs-lookup"><span data-stu-id="88d62-184">Select the **Transaction relationships** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="88d62-185">בחר בקישור **שאילתות וסינון מתקדמים**.</span><span class="sxs-lookup"><span data-stu-id="88d62-185">Select the **Advanced Query and Filtering** link.</span></span> <span data-ttu-id="88d62-186">סנן את העמודה **msdyn\_transactiontype1** כך שתכלול רק את **msdyn\_estimateline**.</span><span class="sxs-lookup"><span data-stu-id="88d62-186">Filter the **msdyn\_transactiontype1** column so that it includes only **msdyn\_estimateline**.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="88d62-187">הגדר את מזהה מודל התחזית בברירת מחדל</span><span class="sxs-lookup"><span data-stu-id="88d62-187">Set the default forecast model ID</span></span>

<span data-ttu-id="88d62-188">כדי לעדכן את מזהה מודל התחזית בברירת מחדל בתבנית, בחר במשימה **הערכת הוצאות** ולאחר מכן לחץ על החץ **מפה** כדי לפתוח את המיפוי.</span><span class="sxs-lookup"><span data-stu-id="88d62-188">To update the default forecast model ID in the template, select the **Expense estimates** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="88d62-189">בחר בקישור **שאילתות וסינון מתקדמים**.</span><span class="sxs-lookup"><span data-stu-id="88d62-189">Select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="88d62-190">אם אתה משתמש בתבנית ברירת מחדל להערכת הוצאות בפרויקט (PSA ל- Fin and Ops), ב- Power Query, בחר באפשרות הראשונה **תנאי שהוכנס** במקטע **שלבים שהוחלו**.</span><span class="sxs-lookup"><span data-stu-id="88d62-190">If you're using the default Project expense estimates (PSA to Fin and Ops) template, in Power Query, select the first **Inserted Condition** from the **Applied Steps** section.</span></span> <span data-ttu-id="88d62-191">בערך **פונקציה** , החלף את **O\_forecast** בשם של מזהה מודל התחזית שבו יש להשתמש בשילוב.</span><span class="sxs-lookup"><span data-stu-id="88d62-191">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="88d62-192">לתבנית ברירת המחדל יש מזהה מודל תחזית מנתוני ההדגמה.</span><span class="sxs-lookup"><span data-stu-id="88d62-192">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="88d62-193">אם אתה יוצר תבנית חדשה, עליך להוסיף עמודה זו.</span><span class="sxs-lookup"><span data-stu-id="88d62-193">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="88d62-194">ב- Power Query, בחר **הוסף עמודה מותנית** והזן שם לעמודה החדשה, כגון **ModelID**.</span><span class="sxs-lookup"><span data-stu-id="88d62-194">In Power Query, select **Add Conditional Column** , and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="88d62-195">הזן את התנאי עבור העמודה, שבה, אם מזהה שורת הערכה אינו Null, \<enter the forecast model ID\>; אחרת Null.</span><span class="sxs-lookup"><span data-stu-id="88d62-195">Enter the condition for the column, where, if Estimate line ID is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="transform-the-billing-types"></a><span data-ttu-id="88d62-196">שנה את סוגי החיובים</span><span class="sxs-lookup"><span data-stu-id="88d62-196">Transform the billing types</span></span>

<span data-ttu-id="88d62-197">תבנית הערכת הוצאות בפרויקט (PSA ל- Fin and Ops) כוללת עמודה מותנית המשמשת לשינוי סוגי החיובים המתקבלים מ- Project Service Automation במהלך השילוב.</span><span class="sxs-lookup"><span data-stu-id="88d62-197">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the billing types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="88d62-198">אם אתה יוצר תבנית משלך, עליך להוסיף עמודה מותנית זו.</span><span class="sxs-lookup"><span data-stu-id="88d62-198">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="88d62-199">בחר בקישור **שאילתות וסינון מתקדמים** ולאחר מכן בחר **הוסף עמודה מותנית**.</span><span class="sxs-lookup"><span data-stu-id="88d62-199">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="88d62-200">הזן שם לעמודה החדשה, כגון **BillingType**.</span><span class="sxs-lookup"><span data-stu-id="88d62-200">Enter a name for the new column, such as **BillingType**.</span></span> <span data-ttu-id="88d62-201">לאחר מכן הזן את התנאי הבא:</span><span class="sxs-lookup"><span data-stu-id="88d62-201">Then enter the following condition:</span></span>

<span data-ttu-id="88d62-202">אם ‎ **msdyn\_billingtype** = 192350000, אז **NonChargeable**</span><span class="sxs-lookup"><span data-stu-id="88d62-202">If **msdyn\_billingtype** = 192350000, then **NonChargeable**</span></span>  
<span data-ttu-id="88d62-203">אחרת, אם ‎ **msdyn\_billingtype** = 192350001, אז **Chargeable**</span><span class="sxs-lookup"><span data-stu-id="88d62-203">else if **msdyn\_billingtype** = 192350001, then **Chargeable**</span></span>  
<span data-ttu-id="88d62-204">אחרת, אם ‎ **msdyn\_billingtype** = 192350002, אז **Complimentary**</span><span class="sxs-lookup"><span data-stu-id="88d62-204">else if **msdyn\_billingtype** = 192350002, then **Complimentary**</span></span>  
<span data-ttu-id="88d62-205">אחרת **NotAvailable**</span><span class="sxs-lookup"><span data-stu-id="88d62-205">else **NotAvailable**</span></span>

#### <a name="transform-the-transaction-types"></a><span data-ttu-id="88d62-206">שנה את סוגי העסקאות</span><span class="sxs-lookup"><span data-stu-id="88d62-206">Transform the transaction types</span></span>

<span data-ttu-id="88d62-207">תבנית הערכת הוצאות בפרויקט (PSA ל- Fin and Ops) כוללת עמודה מותנית המשמשת לשינוי סוגי העסקאות המתקבלים מ- Project Service Automation במהלך השילוב.</span><span class="sxs-lookup"><span data-stu-id="88d62-207">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the transaction types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="88d62-208">אם אתה יוצר תבנית משלך, עליך להוסיף עמודה מותנית זו.</span><span class="sxs-lookup"><span data-stu-id="88d62-208">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="88d62-209">בחר בקישור **שאילתות וסינון מתקדמים** ולאחר מכן בחר **הוסף עמודה מותנית**.</span><span class="sxs-lookup"><span data-stu-id="88d62-209">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="88d62-210">הזן שם לעמודה החדשה, כגון **TransactionType**.</span><span class="sxs-lookup"><span data-stu-id="88d62-210">Enter a name for the new column, such as **TransactionType**.</span></span> <span data-ttu-id="88d62-211">לאחר מכן הזן את התנאי הבא:</span><span class="sxs-lookup"><span data-stu-id="88d62-211">Then enter the following condition:</span></span>

<span data-ttu-id="88d62-212">אם ‎ **msdyn\_transactiontypecode** = 192350000, אחרת **Cost**</span><span class="sxs-lookup"><span data-stu-id="88d62-212">If **msdyn\_transactiontypecode** = 192350000, then **Cost**</span></span>  
<span data-ttu-id="88d62-213">אחרת, אם ‎ **msdyn\_transactiontypecode** = 192350005, אחרת **Sales**</span><span class="sxs-lookup"><span data-stu-id="88d62-213">else if **msdyn\_transactiontypecode** = 192350005, then **Sales**</span></span>  
<span data-ttu-id="88d62-214">אחרת **null**</span><span class="sxs-lookup"><span data-stu-id="88d62-214">else **null**</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="88d62-215">מיפוי תבנית בשילוב נתונים</span><span class="sxs-lookup"><span data-stu-id="88d62-215">Template mapping in Data integration</span></span>

<span data-ttu-id="88d62-216">האיורים הבאים מציגים דוגמאות למיפויי משימות התבנית בשילוב נתונים.</span><span class="sxs-lookup"><span data-stu-id="88d62-216">The following illustrations show examples of the template task mappings in Data integration.</span></span> <span data-ttu-id="88d62-217">המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="88d62-217">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="88d62-218">[![מיפוי תבניות של עסקאות אומדן הוצאות](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="88d62-218">[![Template mapping of expense estimate transactions](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span></span>

<span data-ttu-id="88d62-219">[![מיפוי תבניות של אומדן הוצאות](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="88d62-219">[![Template mapping of expense estimates](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span></span>
