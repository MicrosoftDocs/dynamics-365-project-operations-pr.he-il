---
title: סנכרון הערכות פרוייקטים ישירות מ- Project Service Automation ל- Finance and Operations
description: נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון הערכת שעות בפרוייקט והערכת הוצאות בפרוייקט ישירות מ- Microsoft Dynamics 365 Project Service Automation אל Dynamics 365 Finance.
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
ms.assetid: d688ce9a-41e3-4ebe-952e-700f8351fbe9
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: a24a967d82c2e005e61234d34da8a583b61ff7b1
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751794"
---
# <a name="synchronize-project-estimates-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="6dda9-103">סנכרון הערכות פרוייקטים ישירות מ- Project Service Automation ל- Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="6dda9-103">Synchronize project estimates directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="6dda9-104">נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון הערכת שעות בפרוייקט והערכת הוצאות בפרוייקט ישירות מ- Dynamics 365 Project Service Automation אל Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="6dda9-104">This topic describes the templates and underlying tasks that are used to synchronize project hour estimates and project expense estimates directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="6dda9-105">שילוב משימות פרוייקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונעילת פונקציונליות זמינים בגירסה 8.0.</span><span class="sxs-lookup"><span data-stu-id="6dda9-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking is available in version 8.0.</span></span>
> - <span data-ttu-id="6dda9-106">שילוב נתונים בפועל זמין בגירסה 8.0.1 ואילך.</span><span class="sxs-lookup"><span data-stu-id="6dda9-106">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="6dda9-107">זרימת נתונים עבור Project Service Automation ל- Finance</span><span class="sxs-lookup"><span data-stu-id="6dda9-107">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="6dda9-108">פתרון השילוב Project Service Automation ל- Finance משתמש בתכונת שילוב הנתונים לסנכרון נתונים במופעים של Project Service Automation ו- Finance.</span><span class="sxs-lookup"><span data-stu-id="6dda9-108">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="6dda9-109">תבניות השילוב שזמינות עם תכונת שילוב הנתונים מאפשרות זרימת נתונים על הערכת שעות בפרוייקט והערכת הוצאות בפרוייקט מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="6dda9-109">The integration templates that are available with the Data integration feature enable the flow of data about project hour estimates and project expense estimates from Project Service Automation to Finance.</span></span>

<span data-ttu-id="6dda9-110">האיור הבא מראה כיצד הנתונים מסונכרנים בין Project Service Automation ו- Finance.</span><span class="sxs-lookup"><span data-stu-id="6dda9-110">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="6dda9-111">[![זרימת נתונים לשילוב Project Service Automation עם Finance](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="6dda9-111">[![Data flow for Project Service Automation integration with Finance](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span></span>

## <a name="project-hour-estimates"></a><span data-ttu-id="6dda9-112">הערכת שעות בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="6dda9-112">Project hour estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="6dda9-113">תבנית ומשימות</span><span class="sxs-lookup"><span data-stu-id="6dda9-113">Template and tasks</span></span>

<span data-ttu-id="6dda9-114">כדי לגשת לתבניות הזמינות, במרכז הניהול של Microsoft Power Apps, בחר **פרוייקטים** ולאחר מכן, בפינה העליונה, בחר **פרוייקט חדש** כדי לבחור תבניות ציבוריות.</span><span class="sxs-lookup"><span data-stu-id="6dda9-114">To access the available templates, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="6dda9-115">התבנית והמשימות הבסיסיות הבאות משמשות לסנכרון הערכת שעות בפרוייקט מ- Project Service Automation אל Finance:</span><span class="sxs-lookup"><span data-stu-id="6dda9-115">The following template and underlying tasks are used to synchronize project hour estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="6dda9-116">**שם התבנית בשילוב נתונים:** הערכת שעות בפרוייקט (PSA ל- Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="6dda9-116">**Name of the template in Data integration:** Project hour estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="6dda9-117">**שם המשימות בפרוייקט:**</span><span class="sxs-lookup"><span data-stu-id="6dda9-117">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="6dda9-118">יחסי גומלין של עסקה</span><span class="sxs-lookup"><span data-stu-id="6dda9-118">Transaction relationships</span></span>
    - <span data-ttu-id="6dda9-119">הערכות הוצאות</span><span class="sxs-lookup"><span data-stu-id="6dda9-119">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="6dda9-120">קבוצת ישויות</span><span class="sxs-lookup"><span data-stu-id="6dda9-120">Entity set</span></span>

| <span data-ttu-id="6dda9-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="6dda9-121">Project Service Automation</span></span> | <span data-ttu-id="6dda9-122">כספים</span><span class="sxs-lookup"><span data-stu-id="6dda9-122">Finance</span></span>                                       |
|----------------------------|-----------------------------------------------|
| <span data-ttu-id="6dda9-123">משימות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="6dda9-123">Project tasks</span></span>              | <span data-ttu-id="6dda9-124">ישות שילוב להערכת שעות בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="6dda9-124">Integration entity for project hour estimates</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="6dda9-125">זרימת ישות</span><span class="sxs-lookup"><span data-stu-id="6dda9-125">Entity flow</span></span>

<span data-ttu-id="6dda9-126">הערכות של שעות בפרוייקט מנוהלים ב- Project Service Automation והן מסונכרנות ל- Finance כתחזיות לשעות בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="6dda9-126">Project hour estimates are managed in Project Service Automation, and they are synchronized to Finance as project hour forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="6dda9-127">דרישות מוקדמות</span><span class="sxs-lookup"><span data-stu-id="6dda9-127">Prerequisites</span></span>

<span data-ttu-id="6dda9-128">לפני שתוכל לסנכרן הערכת שעות בפרויקט, עליך לסנכרן פרוייקטים, משימות פרוייקט וקטגוריות של עסקאות הוצאות בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="6dda9-128">Before synchronization of project hour estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="6dda9-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="6dda9-129">Power Query</span></span>

<span data-ttu-id="6dda9-130">בתבנית הערכת שעות בפרוייקט, עליך להשתמש ב- Microsoft Power Query for Excel כדי להשלים את המשימות הבאות:</span><span class="sxs-lookup"><span data-stu-id="6dda9-130">In the project hour estimates template, you must use Microsoft Power Query for Excel to complete these tasks:</span></span>

- <span data-ttu-id="6dda9-131">הגדר את מזהה מודל תחזית ברירת המחדל שישמש כאשר השילוב יוצר תחזיות חדשות לשעות.</span><span class="sxs-lookup"><span data-stu-id="6dda9-131">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="6dda9-132">סנן רשומות שספציפיות למשאבים במשימה אשר יכשלו בשילוב בתוך תחזיות השעות.</span><span class="sxs-lookup"><span data-stu-id="6dda9-132">Filter out any resource-specific records in the task that will fail the integration into hour forecasts.</span></span>
- <span data-ttu-id="6dda9-133">סנן כל שורה ריקה בקטגוריית עסקה.</span><span class="sxs-lookup"><span data-stu-id="6dda9-133">Filter out any empty transaction category rows.</span></span> <span data-ttu-id="6dda9-134">אי השלמת המשימה עשויה להוביל לתחזית שעות שגויה.</span><span class="sxs-lookup"><span data-stu-id="6dda9-134">Failure to complete this task might result in incorrect hour forecasts.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="6dda9-135">הגדר את מזהה מודל התחזית בברירת מחדל</span><span class="sxs-lookup"><span data-stu-id="6dda9-135">Set the default forecast model ID</span></span>

<span data-ttu-id="6dda9-136">כדי לעדכן את מזהה מודל התחזית בברירת מחדל בתבנית, לחץ על החץ **מפה** כדי לפתוח את המיפוי.</span><span class="sxs-lookup"><span data-stu-id="6dda9-136">To update the default forecast model ID in the template, click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="6dda9-137">לאחר מכן, בחר בקישור **שאילתות וסינון מתקדמים**.</span><span class="sxs-lookup"><span data-stu-id="6dda9-137">Then select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="6dda9-138">אם אתה משתמש בתבנית ברירת מחדל להערכת השעות בפרוייקט (PSA ל- Fin and Ops), בחר באפשרות **תנאי שהוכנס** ברשימה **שלבים שהוחלו**.</span><span class="sxs-lookup"><span data-stu-id="6dda9-138">If you're using the default Project hour estimates (PSA to Fin and Ops) template, select the **Inserted Condition** in the list of **Applied Steps**.</span></span> <span data-ttu-id="6dda9-139">בערך **פונקציה**, החלף את **O\_forecast** בשם של מזהה מודל התחזית שבו יש להשתמש בשילוב.</span><span class="sxs-lookup"><span data-stu-id="6dda9-139">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="6dda9-140">לתבנית ברירת המחדל יש מזהה מודל תחזית מנתוני ההדגמה.</span><span class="sxs-lookup"><span data-stu-id="6dda9-140">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="6dda9-141">אם אתה יוצר תבנית חדשה, עליך להוסיף עמודה זו.</span><span class="sxs-lookup"><span data-stu-id="6dda9-141">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="6dda9-142">ב- Power Query, בחר **הוסף עמודה מותנית** והזן שם לעמודה החדשה, כגון **ModelID**.</span><span class="sxs-lookup"><span data-stu-id="6dda9-142">In Power Query, select **Add Conditional Column**, and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="6dda9-143">הזן את התנאי עבור העמודה, שבה, אם משימה הפרוייקט אינה Null, אז \<הזן את מזהה מודל התחזית\>; אחרת Null.</span><span class="sxs-lookup"><span data-stu-id="6dda9-143">Enter the condition for the column, where, if Project task is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="filter-out-resource-specific-records"></a><span data-ttu-id="6dda9-144">סנן רשומות שספציפיות למשאבים</span><span class="sxs-lookup"><span data-stu-id="6dda9-144">Filter out resource-specific records</span></span>

<span data-ttu-id="6dda9-145">לתבנית הערכת שעות בפרוייקט (PSA ל- Fin and Ops) יש מסנן ברירת מחדל שמסיר כל רשומה שספציפית למשאבים.</span><span class="sxs-lookup"><span data-stu-id="6dda9-145">The Project hour estimates (PSA to Fin and Ops) template has a default filter that removes any resource-specific records.</span></span> <span data-ttu-id="6dda9-146">אם אתה יוצר תבנית משלך, עליך להוסיף מסנן זה.</span><span class="sxs-lookup"><span data-stu-id="6dda9-146">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="6dda9-147">בחר בקישור **שאילתות וסינון מתקדמים** כדי לסנן את העמודה **msdyn\_islinetask** כך שרק הרשומות שהן **False** יהיו כלולות.</span><span class="sxs-lookup"><span data-stu-id="6dda9-147">Select the **Advanced Query and Filtering** link to filter on the **msdyn\_islinetask** column so that only **False** records are included.</span></span>

#### <a name="filter-out-empty-transaction-category-rows"></a><span data-ttu-id="6dda9-148">סנן כל שורה ריקה בקטגוריית עסקה</span><span class="sxs-lookup"><span data-stu-id="6dda9-148">Filter out empty transaction category rows</span></span>

<span data-ttu-id="6dda9-149">עליך להוסיף מסנן כדי להסיר שורות שיש בהן קטגוריות של עסקאות ריקות.</span><span class="sxs-lookup"><span data-stu-id="6dda9-149">You must add a filter to remove any rows that have empty transaction categories.</span></span> <span data-ttu-id="6dda9-150">משימה זו נדרשת, בין אם אתה משתמש בתבנית ברירת המחדל או יוצר תבנית משלך.</span><span class="sxs-lookup"><span data-stu-id="6dda9-150">This task is required, regardless of whether you're using the default template or creating your own template.</span></span> <span data-ttu-id="6dda9-151">מסנן זה מסיר שורות סיכום מ- Project Service Automation העלולות לגרום לתחזיות השעות ב- Finance להיות שגויות.</span><span class="sxs-lookup"><span data-stu-id="6dda9-151">This filter removes any summary rows from Project Service Automation that might cause the hour forecasts in Finance to be incorrect.</span></span> <span data-ttu-id="6dda9-152">בחר בקישור **שאילתות וסינון מתקדמים** כדי לסנן רשומות שהן Null בעמודה **msdyn\_transactioncategory\_value**.</span><span class="sxs-lookup"><span data-stu-id="6dda9-152">Select **Advanced Query and Filtering** link to filter out null records in the **msdyn\_transactioncategory\_value** column.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="6dda9-153">מיפוי תבנית בשילוב נתונים</span><span class="sxs-lookup"><span data-stu-id="6dda9-153">Template mapping in Data integration</span></span>

<span data-ttu-id="6dda9-154">האיור הבא מציג דוגמה למיפוי משימת התבנית בשילוב נתונים.</span><span class="sxs-lookup"><span data-stu-id="6dda9-154">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="6dda9-155">המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="6dda9-155">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="6dda9-156">[![מיפוי תבנית](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="6dda9-156">[![Template mapping](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span></span>

## <a name="project-expense-estimates"></a><span data-ttu-id="6dda9-157">הערכות הוצאה בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="6dda9-157">Project expense estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="6dda9-158">תבנית ומשימות</span><span class="sxs-lookup"><span data-stu-id="6dda9-158">Template and tasks</span></span>

<span data-ttu-id="6dda9-159">התבנית והמשימות הבסיסיות הבאות משמשות לסנכרון הערכת הוצאות בפרוייקט מ- Project Service Automation אל Finance:</span><span class="sxs-lookup"><span data-stu-id="6dda9-159">The following template and underlying tasks are used to synchronize project expense estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="6dda9-160">**שם התבנית בשילוב נתונים:** הערכת הוצאות בפרוייקט (PSA ל- Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="6dda9-160">**Name of the template in Data integration:** Project expense estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="6dda9-161">**שם המשימות בפרוייקט:**</span><span class="sxs-lookup"><span data-stu-id="6dda9-161">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="6dda9-162">יחסי גומלין של עסקה</span><span class="sxs-lookup"><span data-stu-id="6dda9-162">Transaction relationships</span></span> 
    - <span data-ttu-id="6dda9-163">הערכות הוצאות</span><span class="sxs-lookup"><span data-stu-id="6dda9-163">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="6dda9-164">קבוצת ישויות</span><span class="sxs-lookup"><span data-stu-id="6dda9-164">Entity set</span></span>

| <span data-ttu-id="6dda9-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="6dda9-165">Project Service Automation</span></span> | <span data-ttu-id="6dda9-166">כספים</span><span class="sxs-lookup"><span data-stu-id="6dda9-166">Finance</span></span>                                                  |
|----------------------------|----------------------------------------------------------|
| <span data-ttu-id="6dda9-167">חיבורי עסקה</span><span class="sxs-lookup"><span data-stu-id="6dda9-167">Transaction Connections</span></span>    | <span data-ttu-id="6dda9-168">ישות שילוב ליחסי גומלין של עסקה בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="6dda9-168">Integration entity for project transaction relationships</span></span> |
| <span data-ttu-id="6dda9-169">שורות של הערכות</span><span class="sxs-lookup"><span data-stu-id="6dda9-169">Estimate Lines</span></span>             | <span data-ttu-id="6dda9-170">ישות שילוב להערכת הוצאות בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="6dda9-170">Integration entity for project expense estimates</span></span>         |

### <a name="entity-flow"></a><span data-ttu-id="6dda9-171">זרימת ישות</span><span class="sxs-lookup"><span data-stu-id="6dda9-171">Entity flow</span></span>

<span data-ttu-id="6dda9-172">הערכות של הוצאות בפרוייקט מנוהלות ב- Project Service Automation והן מסונכרנות ל- Finance כתחזיות להוצאות בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="6dda9-172">Project expense estimates are managed in Project Service Automation, and they are synchronized to Finance as project expense forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="6dda9-173">דרישות מוקדמות</span><span class="sxs-lookup"><span data-stu-id="6dda9-173">Prerequisites</span></span>

<span data-ttu-id="6dda9-174">לפני שתוכל לסנכרן הערכת הוצאות בפרויקט, עליך לסנכרן פרוייקטים, משימות פרוייקט וקטגוריות של עסקאות הוצאות בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="6dda9-174">Before synchronization of project expense estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="6dda9-175">Power Query</span><span class="sxs-lookup"><span data-stu-id="6dda9-175">Power Query</span></span>

<span data-ttu-id="6dda9-176">בתבנית הערכת הוצאות בפרוייקט, עליך להשתמש ב- Power Query כדי להשלים את המשימות הבאות:</span><span class="sxs-lookup"><span data-stu-id="6dda9-176">In the project expense estimates template, you must use Power Query to complete the following tasks:</span></span>

- <span data-ttu-id="6dda9-177">סנן כדי לכלול רק רשומות של שורת הערכת הוצאות.</span><span class="sxs-lookup"><span data-stu-id="6dda9-177">Filter to include only expense estimate line records.</span></span>
- <span data-ttu-id="6dda9-178">הגדר את מזהה מודל תחזית ברירת המחדל שישמש כאשר השילוב יוצר תחזיות חדשות לשעות.</span><span class="sxs-lookup"><span data-stu-id="6dda9-178">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="6dda9-179">שנה את סוגי החיובים.</span><span class="sxs-lookup"><span data-stu-id="6dda9-179">Transform the billing types.</span></span>
- <span data-ttu-id="6dda9-180">שנה את סוגי העסקאות.</span><span class="sxs-lookup"><span data-stu-id="6dda9-180">Transform the transaction types.</span></span>

#### <a name="filter-to-include-only-expense-estimate-lines"></a><span data-ttu-id="6dda9-181">סנן כדי לכלול רק שורות של הערכת הוצאות</span><span class="sxs-lookup"><span data-stu-id="6dda9-181">Filter to include only expense estimate lines</span></span>

<span data-ttu-id="6dda9-182">לתבנית הערכת הוצאות בפרוייקט (PSA ל- Fin and Ops) יש מסנן ברירת מחדל הכולל רק שורות הוצאות בשילוב.</span><span class="sxs-lookup"><span data-stu-id="6dda9-182">The Project expense estimates (PSA to Fin and Ops) template has a default filter that includes only expense lines in the integration.</span></span> <span data-ttu-id="6dda9-183">אם אתה יוצר תבנית משלך, עליך להוסיף מסנן זה.</span><span class="sxs-lookup"><span data-stu-id="6dda9-183">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="6dda9-184">בחר במשימה **‏‫יחסי גומלין של עסקה‬** ולאחר מכן לחץ על החץ **מפה** כדי לפתח את המיפוי.</span><span class="sxs-lookup"><span data-stu-id="6dda9-184">Select the **Transaction relationships** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="6dda9-185">בחר בקישור **שאילתות וסינון מתקדמים**.</span><span class="sxs-lookup"><span data-stu-id="6dda9-185">Select the **Advanced Query and Filtering** link.</span></span> <span data-ttu-id="6dda9-186">סנן את העמודה **msdyn\_transactiontype1** כך שתכלול רק את **msdyn\_estimateline**.</span><span class="sxs-lookup"><span data-stu-id="6dda9-186">Filter the **msdyn\_transactiontype1** column so that it includes only **msdyn\_estimateline**.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="6dda9-187">הגדר את מזהה מודל התחזית בברירת מחדל</span><span class="sxs-lookup"><span data-stu-id="6dda9-187">Set the default forecast model ID</span></span>

<span data-ttu-id="6dda9-188">כדי לעדכן את מזהה מודל התחזית בברירת מחדל בתבנית, בחר במשימה **הערכת הוצאות** ולאחר מכן לחץ על החץ **מפה** כדי לפתוח את המיפוי.</span><span class="sxs-lookup"><span data-stu-id="6dda9-188">To update the default forecast model ID in the template, select the **Expense estimates** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="6dda9-189">בחר בקישור **שאילתות וסינון מתקדמים**.</span><span class="sxs-lookup"><span data-stu-id="6dda9-189">Select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="6dda9-190">אם אתה משתמש בתבנית ברירת מחדל להערכת הוצאות בפרוייקט (PSA ל- Fin and Ops), ב- Power Query, בחר באפשרות הראשונה **תנאי שהוכנס** במקטע **שלבים שהוחלו**.</span><span class="sxs-lookup"><span data-stu-id="6dda9-190">If you're using the default Project expense estimates (PSA to Fin and Ops) template, in Power Query, select the first **Inserted Condition** from the **Applied Steps** section.</span></span> <span data-ttu-id="6dda9-191">בערך **פונקציה**, החלף את **O\_forecast** בשם של מזהה מודל התחזית שבו יש להשתמש בשילוב.</span><span class="sxs-lookup"><span data-stu-id="6dda9-191">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="6dda9-192">לתבנית ברירת המחדל יש מזהה מודל תחזית מנתוני ההדגמה.</span><span class="sxs-lookup"><span data-stu-id="6dda9-192">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="6dda9-193">אם אתה יוצר תבנית חדשה, עליך להוסיף עמודה זו.</span><span class="sxs-lookup"><span data-stu-id="6dda9-193">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="6dda9-194">ב- Power Query, בחר **הוסף עמודה מותנית** והזן שם לעמודה החדשה, כגון **ModelID**.</span><span class="sxs-lookup"><span data-stu-id="6dda9-194">In Power Query, select **Add Conditional Column**, and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="6dda9-195">הזן את התנאי עבור העמודה, שבה, אם מזהה שורת ההערכה אינו Null, אז \<הזן את מזהה מודל התחזית\>; אחרת Null.</span><span class="sxs-lookup"><span data-stu-id="6dda9-195">Enter the condition for the column, where, if Estimate line ID is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="transform-the-billing-types"></a><span data-ttu-id="6dda9-196">שנה את סוגי החיובים</span><span class="sxs-lookup"><span data-stu-id="6dda9-196">Transform the billing types</span></span>

<span data-ttu-id="6dda9-197">תבנית הערכת הוצאות בפרוייקט (PSA ל- Fin and Ops) כוללת עמודה מותנית המשמשת לשינוי סוגי החיובים המתקבלים מ- Project Service Automation במהלך השילוב.</span><span class="sxs-lookup"><span data-stu-id="6dda9-197">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the billing types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="6dda9-198">אם אתה יוצר תבנית משלך, עליך להוסיף עמודה מותנית זו.</span><span class="sxs-lookup"><span data-stu-id="6dda9-198">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="6dda9-199">בחר בקישור **שאילתות וסינון מתקדמים** ולאחר מכן בחר **הוסף עמודה מותנית**.</span><span class="sxs-lookup"><span data-stu-id="6dda9-199">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="6dda9-200">הזן שם לעמודה החדשה, כגון **BillingType**.</span><span class="sxs-lookup"><span data-stu-id="6dda9-200">Enter a name for the new column, such as **BillingType**.</span></span> <span data-ttu-id="6dda9-201">לאחר מכן הזן את התנאי הבא:</span><span class="sxs-lookup"><span data-stu-id="6dda9-201">Then enter the following condition:</span></span>

<span data-ttu-id="6dda9-202">אם ‎**msdyn\_billingtype** = 192350000, אז **NonChargeable**</span><span class="sxs-lookup"><span data-stu-id="6dda9-202">If **msdyn\_billingtype** = 192350000, then **NonChargeable**</span></span>  
<span data-ttu-id="6dda9-203">אחרת, אם ‎**msdyn\_billingtype** = 192350001, אז **Chargeable**</span><span class="sxs-lookup"><span data-stu-id="6dda9-203">else if **msdyn\_billingtype** = 192350001, then **Chargeable**</span></span>  
<span data-ttu-id="6dda9-204">אחרת, אם ‎**msdyn\_billingtype** = 192350002, אז **Complimentary**</span><span class="sxs-lookup"><span data-stu-id="6dda9-204">else if **msdyn\_billingtype** = 192350002, then **Complimentary**</span></span>  
<span data-ttu-id="6dda9-205">אחרת **NotAvailable**</span><span class="sxs-lookup"><span data-stu-id="6dda9-205">else **NotAvailable**</span></span>

#### <a name="transform-the-transaction-types"></a><span data-ttu-id="6dda9-206">שנה את סוגי העסקאות</span><span class="sxs-lookup"><span data-stu-id="6dda9-206">Transform the transaction types</span></span>

<span data-ttu-id="6dda9-207">תבנית הערכת הוצאות בפרוייקט (PSA ל- Fin and Ops) כוללת עמודה מותנית המשמשת לשינוי סוגי העסקאות המתקבלים מ- Project Service Automation במהלך השילוב.</span><span class="sxs-lookup"><span data-stu-id="6dda9-207">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the transaction types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="6dda9-208">אם אתה יוצר תבנית משלך, עליך להוסיף עמודה מותנית זו.</span><span class="sxs-lookup"><span data-stu-id="6dda9-208">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="6dda9-209">בחר בקישור **שאילתות וסינון מתקדמים** ולאחר מכן בחר **הוסף עמודה מותנית**.</span><span class="sxs-lookup"><span data-stu-id="6dda9-209">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="6dda9-210">הזן שם לעמודה החדשה, כגון **TransactionType**.</span><span class="sxs-lookup"><span data-stu-id="6dda9-210">Enter a name for the new column, such as **TransactionType**.</span></span> <span data-ttu-id="6dda9-211">לאחר מכן הזן את התנאי הבא:</span><span class="sxs-lookup"><span data-stu-id="6dda9-211">Then enter the following condition:</span></span>

<span data-ttu-id="6dda9-212">אם ‎**msdyn\_transactiontypecode** = 192350000, אחרת **Cost**</span><span class="sxs-lookup"><span data-stu-id="6dda9-212">If **msdyn\_transactiontypecode** = 192350000, then **Cost**</span></span>  
<span data-ttu-id="6dda9-213">אחרת, אם ‎**msdyn\_transactiontypecode** = 192350005, אחרת **Sales**</span><span class="sxs-lookup"><span data-stu-id="6dda9-213">else if **msdyn\_transactiontypecode** = 192350005, then **Sales**</span></span>  
<span data-ttu-id="6dda9-214">אחרת **null**</span><span class="sxs-lookup"><span data-stu-id="6dda9-214">else **null**</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="6dda9-215">מיפוי תבנית בשילוב נתונים</span><span class="sxs-lookup"><span data-stu-id="6dda9-215">Template mapping in Data integration</span></span>

<span data-ttu-id="6dda9-216">האיורים הבאים מציגים דוגמאות למיפויי משימות התבנית בשילוב נתונים.</span><span class="sxs-lookup"><span data-stu-id="6dda9-216">The following illustrations show examples of the template task mappings in Data integration.</span></span> <span data-ttu-id="6dda9-217">המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="6dda9-217">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="6dda9-218">[![מיפוי תבנית](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="6dda9-218">[![Template mapping](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span></span>

<span data-ttu-id="6dda9-219">[![מיפוי תבנית](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="6dda9-219">[![Template mapping](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span></span>
