---
title: סנכרון נתונים בפועל של פרויקט ישירות מ- Project Service Automation ליומן שילוב הפרויקט עבור רישום ב- Finance and Operations
description: נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון נתונים בפועל של פרויקט ישירות מ- Microsoft Dynamics 365 Project Service Automation אל Finance and Operations.
author: Yowelle
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: cff62e739e88dc45e7c3d1ea044875f0600f2bc1
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077440"
---
# <a name="synchronize-project-actuals-directly-from-project-service-automation-to-the-project-integration-journal-for-posting-in-finance-and-operations"></a><span data-ttu-id="c0bab-103">סנכרון נתונים בפועל של פרויקט ישירות מ- Project Service Automation ליומן שילוב הפרויקט עבור רישום ב- Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="c0bab-103">Synchronize project actuals directly from Project Service Automation to the project integration journal for posting in Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="c0bab-104">נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון נתונים בפועל של פרויקט ישירות מ- Dynamics 365 Project Service Automation אל Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="c0bab-104">This topic describes the templates and underlying tasks that are used to synchronize project actuals directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

<span data-ttu-id="c0bab-105">התבנית מסנכרנת עסקאות מ- Project Service Automation לטבלת אחסון זמני ב- Finance.</span><span class="sxs-lookup"><span data-stu-id="c0bab-105">The template synchronizes transactions from Project Service Automation into a staging table in Finance.</span></span> <span data-ttu-id="c0bab-106">לאחר השלמת הסנכרון, **עליך** לייבא נתונים מטבלת האחסון הזמני אל יומן השילוב.</span><span class="sxs-lookup"><span data-stu-id="c0bab-106">After synchronization is completed, you **must** import the data from the staging table into the integration journal.</span></span>

> [!NOTE]
> - <span data-ttu-id="c0bab-107">שילוב נתונים בפועל של פרויקט יהיה זמין החל מגירסה 8.0.1 ואילך.</span><span class="sxs-lookup"><span data-stu-id="c0bab-107">Project actuals integration is available starting in version 8.0.1.</span></span>
> - <span data-ttu-id="c0bab-108">אם אתה משתמש ב- Enterprise Edition 7.3.0 לאחר התקנת KB 4132657 ו- KB 4132660, תוכל להשתמש בתבניות לשילוב משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונתונים בפועל, וכן להגדיר תצורה של נעילת פונקציונליות.</span><span class="sxs-lookup"><span data-stu-id="c0bab-108">If you're using Enterprise edition 7.3.0 after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="c0bab-109">אם עליך לאפס את ההפצות החשבונאיות, מומלץ להתקין גם את KB 4131710.</span><span class="sxs-lookup"><span data-stu-id="c0bab-109">If you must reset the accounting distributions, we recommend that you also install KB 4131710.</span></span>
> - <span data-ttu-id="c0bab-110">אם אתה משתמש בגירסה 7.3.0 ואתה מעביר עסקאות עמלה מ- Project Service Automation, עליך להתקין את KB 4345320 כדי לכלול את העמלות בחשבונית הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="c0bab-110">If you're using version 7.3.0, and you are bringing fee transactions over from Project Service Automation, you must install KB 4345320 in order to include those fees in the project invoice.</span></span>
> - <span data-ttu-id="c0bab-111">אם אתה מזין סכומי מס מכירות בעסקאות הוצאה או שעות ב- Project Service Automation, עליך להתקין את עדכון 7 של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="c0bab-111">If you're entering sales tax amounts on time or expense transactions in Project Service Automation, you must install Project Service Automation Update 7.</span></span> <span data-ttu-id="c0bab-112">אחרת, הנתונים בפועל של המס לא יקושרו לנתונים בפועל של ההוצאות או השעות המשויכות והם לא יסונכרנו אל Finance.</span><span class="sxs-lookup"><span data-stu-id="c0bab-112">Otherwise, the tax actuals won't be linked to the associated time or expense actuals, and they won't be synchronized to Finance.</span></span> <span data-ttu-id="c0bab-113">לקבלת מידע נוסף, פנה לתמיכה.</span><span class="sxs-lookup"><span data-stu-id="c0bab-113">For more information, contact Support.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="c0bab-114">זרימת נתונים עבור Project Service Automation ל- Finance</span><span class="sxs-lookup"><span data-stu-id="c0bab-114">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="c0bab-115">פתרון השילוב Project Service Automation ל- Finance משתמש בתכונת שילוב הנתונים לסנכרון נתונים במופעים של Project Service Automation ו- Finance.</span><span class="sxs-lookup"><span data-stu-id="c0bab-115">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="c0bab-116">תבניות השילוב שזמינות עם תכונת שילוב הנתונים מאפשרות זרימת נתונים על נתונים בפועל של פרויקט מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="c0bab-116">The integration templates that are available with the Data integration feature enable the flow of data about project actuals from Project Service Automation to Finance.</span></span>

<span data-ttu-id="c0bab-117">האיור הבא מראה כיצד הנתונים מסונכרנים בין Project Service Automation ו- Finance.</span><span class="sxs-lookup"><span data-stu-id="c0bab-117">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="c0bab-118">[![זרימת נתונים לשילוב Project Service Automation עם Finance and Operations](./media/ProjectActualsFlow.jpg)](./media/ProjectActualsFlow.jpg)</span><span class="sxs-lookup"><span data-stu-id="c0bab-118">[![Data flow for Project Service Automation integration with Finance and Operations](./media/ProjectActualsFlow.jpg)](./media/ProjectActualsFlow.jpg)</span></span>

## <a name="project-actuals-from-project-service-automation"></a><span data-ttu-id="c0bab-119">נתונים בפועל של פרויקט מ- Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="c0bab-119">Project actuals from Project Service Automation</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="c0bab-120">תבנית ומשימות</span><span class="sxs-lookup"><span data-stu-id="c0bab-120">Template and tasks</span></span>

<span data-ttu-id="c0bab-121">כדי לגשת לתבניות הזמינות, במרכז הניהול של Microsoft Power Apps, בחר **פרויקטים** ולאחר מכן, בפינה העליונה, בחר **פרויקט חדש** כדי לבחור תבניות ציבוריות.</span><span class="sxs-lookup"><span data-stu-id="c0bab-121">To access the available templates, in the Microsoft Power Apps admin center, select **Projects** , and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="c0bab-122">התבנית והמשימות הבסיסיות הבאות משמשות לסנכרון נתונים בפועל של פרויקט מ- Project Service Automation אל Finance:</span><span class="sxs-lookup"><span data-stu-id="c0bab-122">The following template and underlying tasks are used to synchronize project actuals from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="c0bab-123">**שם התבנית בשילוב נתונים:** נתונים בפועל של פרויקט (PSA ל- Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="c0bab-123">**Name of the template in Data integration:** Project actuals (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="c0bab-124">**שם המשימות בפרויקט:**</span><span class="sxs-lookup"><span data-stu-id="c0bab-124">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="c0bab-125">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="c0bab-125">Actuals</span></span>
    - <span data-ttu-id="c0bab-126">TransactionConnections</span><span class="sxs-lookup"><span data-stu-id="c0bab-126">TransactionConnections</span></span>

### <a name="entity-set"></a><span data-ttu-id="c0bab-127">קבוצת ישויות</span><span class="sxs-lookup"><span data-stu-id="c0bab-127">Entity set</span></span>

| <span data-ttu-id="c0bab-128">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="c0bab-128">Project Service Automation</span></span> | <span data-ttu-id="c0bab-129">כספים</span><span class="sxs-lookup"><span data-stu-id="c0bab-129">Finance</span></span>                                   |
|----------------------------|----------------------------------------------------------|
| <span data-ttu-id="c0bab-130">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="c0bab-130">Actuals</span></span>                    | <span data-ttu-id="c0bab-131">ישות שילוב לנתונים בפועל של פרויקט</span><span class="sxs-lookup"><span data-stu-id="c0bab-131">Integration entity for project actuals</span></span>                   |
| <span data-ttu-id="c0bab-132">חיבורי עסקה</span><span class="sxs-lookup"><span data-stu-id="c0bab-132">Transaction Connections</span></span>    | <span data-ttu-id="c0bab-133">ישות שילוב ליחסי גומלין של עסקה בפרויקט</span><span class="sxs-lookup"><span data-stu-id="c0bab-133">Integration entity for project transaction relationships</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="c0bab-134">זרימת ישות</span><span class="sxs-lookup"><span data-stu-id="c0bab-134">Entity flow</span></span>

<span data-ttu-id="c0bab-135">נתונים בפועל של פרויקט מנוהלים ב- Project Service Automation והם מסונכרנים ליומן שילוב הפרויקט ב- Finance.</span><span class="sxs-lookup"><span data-stu-id="c0bab-135">Project actuals are managed in Project Service Automation, and they are synchronized to the project integration journal in Finance.</span></span> <span data-ttu-id="c0bab-136">החשבונאות תוחל על סמך הממדים הכספיים בברירת המחדל והגדרת הרישום.</span><span class="sxs-lookup"><span data-stu-id="c0bab-136">The accounting will be applied based on default financial dimensions and the posting setup.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="c0bab-137">דרישות מוקדמות</span><span class="sxs-lookup"><span data-stu-id="c0bab-137">Prerequisites</span></span>

<span data-ttu-id="c0bab-138">לפני שיתרחש סנכרון של נתונים בפועל, עליך להגדיר את התצורה של פרמטרי השילוב של Project Service Automation ולסנכרן פרויקטים, משימות פרויקט וקטגוריות עסקאות של הוצאות בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="c0bab-138">Before synchronization of actuals can occur, you must configure the Project Service Automation integration parameters and synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="c0bab-139">Power Query</span><span class="sxs-lookup"><span data-stu-id="c0bab-139">Power Query</span></span>

<span data-ttu-id="c0bab-140">בתבנית נתונים בפועל של פרויקט, עליך להשתמש ב- Microsoft Power Query for Excel כדי להשלים את המשימות הבאות:</span><span class="sxs-lookup"><span data-stu-id="c0bab-140">In the project actuals template, you must use Microsoft Power Query for Excel to complete these tasks:</span></span>

- <span data-ttu-id="c0bab-141">שנה את סוג העסקה ב- Project Service Automation לסוג העסקה הנכון ב- Finance.</span><span class="sxs-lookup"><span data-stu-id="c0bab-141">Transform the transaction type in Project Service Automation to the correct transaction type in Finance.</span></span> <span data-ttu-id="c0bab-142">שינוי זה כבר הוגדר בתבנית נתונים בפועל של פרויקט (PSA ל- Fin and Ops).</span><span class="sxs-lookup"><span data-stu-id="c0bab-142">This transformation is already defined in the Project actuals (PSA to Fin and Ops) template.</span></span>
- <span data-ttu-id="c0bab-143">שנה את סוג החיוב ב- Project Service Automation לסוג החיוב הנכון ב- Finance.</span><span class="sxs-lookup"><span data-stu-id="c0bab-143">Transform the billing type in Project Service Automation to the correct billing type in Finance.</span></span> <span data-ttu-id="c0bab-144">שינוי זה כבר הוגדר בתבנית נתונים בפועל של פרויקט (PSA ל- Fin and Ops).</span><span class="sxs-lookup"><span data-stu-id="c0bab-144">This transformation is already defined in the Project actuals (PSA to Fin and Ops) template.</span></span> <span data-ttu-id="c0bab-145">לאחר מכן, סוג החיוב ימופה אל מאפיין השורה, בהתאם לתצורה בדף **פרמטרי שילוב של Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="c0bab-145">The billing type is then mapped to the line property, based on the configuration on the **Project Service Automation integration parameters** page.</span></span>
- <span data-ttu-id="c0bab-146">יש לסנכרן סינון ליחידות ארגוניות ספציפיות של משאב באמצעות תבנית זו.</span><span class="sxs-lookup"><span data-stu-id="c0bab-146">Filter to specific resource organizational units that must be synchronized with this template.</span></span>
- <span data-ttu-id="c0bab-147">אם נתונים בפועל של שעות בין-חברתיות או הוצאות בין-חברתיות יסונכרנו ל- Finance, עליך לשנות את היחידה הארגונית של החוזה לישות המשפטית הנכונה ב- Finance.</span><span class="sxs-lookup"><span data-stu-id="c0bab-147">If intercompany time or intercompany expense actuals will be synchronized to Finance, you must transform the contract organizational unit to the correct legal entity in Finance.</span></span> <span data-ttu-id="c0bab-148">בתבנית נתונים בפועל של פרויקט (PSA ל- Fin and Ops), עמודה מותנית מוגדרת בהתאם לנתוני ההדגמה.</span><span class="sxs-lookup"><span data-stu-id="c0bab-148">In the Project actuals (PSA to Fin and Ops) template, a conditional column is defined based on demo data.</span></span> <span data-ttu-id="c0bab-149">עליך לעדכן את העמודה המותנית שהוכנסה לאחרונה לישויות המשפטיות הנכונות.</span><span class="sxs-lookup"><span data-stu-id="c0bab-149">You must update the last inserted conditional column to the correct legal entities.</span></span> <span data-ttu-id="c0bab-150">אחרת, עלולה להתרחש שגיאת שילוב או ייבוא של עסקאות בפועל שגויות אל Finance.</span><span class="sxs-lookup"><span data-stu-id="c0bab-150">Otherwise, either an integration error might occur, or incorrect actual transactions might be imported into Finance.</span></span>
- <span data-ttu-id="c0bab-151">אם לא יסונכרנו הנתונים בפועל של שעות בין-חברתיות והוצאות בין-חברתיות ל- Finance, עליך למחוק את העמודה המותנית האחרונה שהוכנסה מהתבנית.</span><span class="sxs-lookup"><span data-stu-id="c0bab-151">If intercompany time or intercompany expense actuals won't be synchronized to Finance, you must delete the last inserted conditional column from your template.</span></span> <span data-ttu-id="c0bab-152">אחרת, עלולה להתרחש שגיאת שילוב או ייבוא של עסקאות בפועל שגויות אל Finance.</span><span class="sxs-lookup"><span data-stu-id="c0bab-152">Otherwise, either an integration error might occur, or incorrect actual transactions might be imported into Finance.</span></span>

#### <a name="contract-organizational-unit"></a><span data-ttu-id="c0bab-153">יחידה ארגונית של חוזה</span><span class="sxs-lookup"><span data-stu-id="c0bab-153">Contract organizational unit</span></span>
<span data-ttu-id="c0bab-154">כדי לעדכן את העמודה המותנית שהוכנסה בתבנית, לחץ על החץ **מפה** כדי לפתוח את המיפוי.</span><span class="sxs-lookup"><span data-stu-id="c0bab-154">To update the inserted conditional column in the template, click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="c0bab-155">בחר בקישור **שאילתות וסינון מתקדמים** כדי לפתוח את Power Query.</span><span class="sxs-lookup"><span data-stu-id="c0bab-155">Select the **Advanced Query and Filtering** link to open Power Query.</span></span>

- <span data-ttu-id="c0bab-156">אם אתה משתמש בתבנית ברירת מחדל לנתונים בפועל של פרויקט (PSA ל- Fin and Ops), ב- Power Query, בחר באפשרות האחרונה **תנאי שהוכנס** במקטע **שלבים שהוחלו**.</span><span class="sxs-lookup"><span data-stu-id="c0bab-156">If you're using the default Project actuals (PSA to Fin and Ops) template, in Power Query, select the last **Inserted Condition** from the **Applied Steps** section.</span></span> <span data-ttu-id="c0bab-157">בערך **פונקציה** , החלף את **USSI** בשם של הישות המשפטית שתהיה בשימוש בשילוב.</span><span class="sxs-lookup"><span data-stu-id="c0bab-157">In the **Function** entry, replace **USSI** with the name of the legal entity that should be used with the integration.</span></span> <span data-ttu-id="c0bab-158">הוסף תנאים נוספים לערך **פונקציה** כנדרש ועדכן את התנאי **else** מ- **USMF** לישות המשפטית הנכונה.</span><span class="sxs-lookup"><span data-stu-id="c0bab-158">Add additional conditions to the **Function** entry as you require, and update the **else** condition from **USMF** to the correct legal entity.</span></span>
- <span data-ttu-id="c0bab-159">אם אתה יוצר תבנית חדשה, עליך להוסיף את העמודה כדי לתמוך בשעות והוצאות בין-חברתיות.</span><span class="sxs-lookup"><span data-stu-id="c0bab-159">If you're creating a new template, you must add the column to support intercompany time and expenses.</span></span> <span data-ttu-id="c0bab-160">בחר **הוסף עמודה מותנית** והזן שם לעמודה, כגון **LegalEntity**.</span><span class="sxs-lookup"><span data-stu-id="c0bab-160">Select **Add Conditional Column** , and enter a name for the column, such as **LegalEntity**.</span></span> <span data-ttu-id="c0bab-161">הזן תנאי עבור העמודה, שבו, אם **msdyn\_contractorganizationalunitid.msdyn\_name** הוא \<organizational unit\>, אז \<enter the legal entity\>; אחרת Null.</span><span class="sxs-lookup"><span data-stu-id="c0bab-161">Enter a condition for the column, where, if **msdyn\_contractorganizationalunitid.msdyn\_name** is \<organizational unit\>, then \<enter the legal entity\>; else null.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="c0bab-162">מיפוי תבנית בשילוב נתונים</span><span class="sxs-lookup"><span data-stu-id="c0bab-162">Template mapping in Data integration</span></span>

<span data-ttu-id="c0bab-163">האיורים הבאים מציגים דוגמה למיפוי משימת התבנית בשילוב נתונים.</span><span class="sxs-lookup"><span data-stu-id="c0bab-163">The following illustrations show an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="c0bab-164">המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="c0bab-164">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="c0bab-165">[![מיפוי תבניות - ‏‫נתונים בפועל](./media/ActualsMapping.jpg)](./media/ActualsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="c0bab-165">[![Template mapping - Actuals](./media/ActualsMapping.jpg)](./media/ActualsMapping.jpg)</span></span>

<span data-ttu-id="c0bab-166">[![מיפוי תבניות - חיבורי עסקאות](./media/TransactionConnections.jpg)](./media/TransactionConnections.jpg)</span><span class="sxs-lookup"><span data-stu-id="c0bab-166">[![Template mapping - Transaction connections](./media/TransactionConnections.jpg)](./media/TransactionConnections.jpg)</span></span>

## <a name="import-from-staging-table-after-integration-from-project-service-automation"></a><span data-ttu-id="c0bab-167">ייבוא מטבלת אחסון זמני לאחר שילוב מ- Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="c0bab-167">Import from staging table after integration from Project Service Automation</span></span>

<span data-ttu-id="c0bab-168">יש להפעיל את התהליך התקופתי לייבוא מטבלת אחסון זמני לאחר סנכרון של נתונים בפועל מ- Project Service Automation אל Finance.</span><span class="sxs-lookup"><span data-stu-id="c0bab-168">The Import from staging table periodic process must be run after the synchronization of actuals from Project Service Automation to Finance.</span></span> <span data-ttu-id="c0bab-169">תהליך זה ייבא את עסקאות הפרויקט מטבלת האחסון הזמני אל יומן שילוב Project Service Automation, שבו החשבונאות חלה וניתן לרשום את העסקאות שיובאו.</span><span class="sxs-lookup"><span data-stu-id="c0bab-169">This process will import the project transactions from the staging table into the Project Service Automation integration journal, where the accounting is applied and the imported transactions can be posted.</span></span> <span data-ttu-id="c0bab-170">מומלץ להפעיל תהליך זה במצב אצווה; באפשרותך להגדיר אותו כך שיפעל כאצווה חוזרת.</span><span class="sxs-lookup"><span data-stu-id="c0bab-170">We recommend that you run this process in batch mode; it can optionally be set up to run as a recurring batch.</span></span>

## <a name="update-actuals-from-finance"></a><span data-ttu-id="c0bab-171">עדכון נתונים בפועל מ- Finance</span><span class="sxs-lookup"><span data-stu-id="c0bab-171">Update actuals from Finance</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="c0bab-172">תבנית ומשימות</span><span class="sxs-lookup"><span data-stu-id="c0bab-172">Template and tasks</span></span>

<span data-ttu-id="c0bab-173">התבנית והמשימות הבסיסיות הבאות משמשות לסנכרון מספר השובר ומסי המכירות עבור עסקאות פרויקט שנרשמו מ- Finance ל- Project Service Automation:</span><span class="sxs-lookup"><span data-stu-id="c0bab-173">The following template and underlying tasks are used to synchronize the voucher number and sales taxes for posted project transactions from Finance to Project Service Automation:</span></span>

- <span data-ttu-id="c0bab-174">**שם התבנית בשילוב נתונים:** עדכון נתונים בפועל של פרויקט (Fin Ops ל- PSA)</span><span class="sxs-lookup"><span data-stu-id="c0bab-174">**Name of the template in Data integration:** Project actuals update (Fin Ops to PSA)</span></span>
- <span data-ttu-id="c0bab-175">**שם המשימות בפרויקט:**</span><span class="sxs-lookup"><span data-stu-id="c0bab-175">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="c0bab-176">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="c0bab-176">Actuals</span></span> 
    - <span data-ttu-id="c0bab-177">TransactionConnections</span><span class="sxs-lookup"><span data-stu-id="c0bab-177">TransactionConnections</span></span>

### <a name="entity-set"></a><span data-ttu-id="c0bab-178">קבוצת ישויות</span><span class="sxs-lookup"><span data-stu-id="c0bab-178">Entity set</span></span>

| <span data-ttu-id="c0bab-179">כספים</span><span class="sxs-lookup"><span data-stu-id="c0bab-179">Finance</span></span>                                                  | <span data-ttu-id="c0bab-180">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="c0bab-180">Project Service Automation</span></span> |
|----------------------------------------------------------|----------------------------|
| <span data-ttu-id="c0bab-181">ישות שילוב לנתונים בפועל של פרויקט</span><span class="sxs-lookup"><span data-stu-id="c0bab-181">Integration entity for project actuals</span></span>                   | <span data-ttu-id="c0bab-182">נתונים בפועל</span><span class="sxs-lookup"><span data-stu-id="c0bab-182">Actuals</span></span>                    |
| <span data-ttu-id="c0bab-183">ישות שילוב ליחסי גומלין של עסקה בפרויקט</span><span class="sxs-lookup"><span data-stu-id="c0bab-183">Integration entity for project transaction relationships</span></span> | <span data-ttu-id="c0bab-184">חיבורי עסקה</span><span class="sxs-lookup"><span data-stu-id="c0bab-184">Transaction Connections</span></span>    |

### <a name="entity-flow"></a><span data-ttu-id="c0bab-185">זרימת ישות</span><span class="sxs-lookup"><span data-stu-id="c0bab-185">Entity flow</span></span>

<span data-ttu-id="c0bab-186">נתונים בפועל של פרויקט מנוהלים ב- Project Service Automation והם מסונכרנים ליומן שילוב הפרויקט ב- Finance.</span><span class="sxs-lookup"><span data-stu-id="c0bab-186">Project actuals are managed in Project Service Automation, and they are synchronized to the project integration journal in Finance.</span></span> <span data-ttu-id="c0bab-187">לאחר רישום נתונים בפועל ב- Finance, הם מעודכנים ב- Project Service Automation עם מספר השובר מ- Finance.</span><span class="sxs-lookup"><span data-stu-id="c0bab-187">After actuals are posted in Finance, they are updated in Project Service Automation with the voucher number from Finance.</span></span> <span data-ttu-id="c0bab-188">אם מסי המכירות התווספו ב- Finance, נוצרים נתונים בפועל חדשים למסים ב- Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="c0bab-188">If sales taxes were added in Finance, new tax actuals are created in Project Service Automation.</span></span>

### <a name="power-query"></a><span data-ttu-id="c0bab-189">Power Query</span><span class="sxs-lookup"><span data-stu-id="c0bab-189">Power Query</span></span>

<span data-ttu-id="c0bab-190">בתבנית עדכון נתונים בפועל של פרויקט, עליך להשתמש ב- Power Query כדי להשלים את המשימות הבאות:</span><span class="sxs-lookup"><span data-stu-id="c0bab-190">In the project actuals update template, you must use Power Query to complete these tasks:</span></span>

- <span data-ttu-id="c0bab-191">שנה את סוג העסקה ב- Finance לסוג העסקה הנכון ב- Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="c0bab-191">Transform the transaction type in Finance to the correct transaction type in Project Service Automation.</span></span> <span data-ttu-id="c0bab-192">שינוי זה כבר הוגדר בתבנית עדכון נתונים בפועל של פרויקט (Fin Ops ל- PSA).</span><span class="sxs-lookup"><span data-stu-id="c0bab-192">This transformation is already defined in the Project actuals update (Fin Ops to PSA) template.</span></span>
- <span data-ttu-id="c0bab-193">שנה את סוג החיוב ב- Finance לסוג החיוב הנכון ב- Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="c0bab-193">Transform the billing type in Finance to the correct billing type in Project Service Automation.</span></span> <span data-ttu-id="c0bab-194">שינוי זה כבר הוגדר בתבנית עדכון נתונים בפועל של פרויקט (Fin Ops ל- PSA).</span><span class="sxs-lookup"><span data-stu-id="c0bab-194">This transformation is already defined in the Project actuals update (Fin Ops to PSA) template.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="c0bab-195">מיפוי תבנית בשילוב נתונים</span><span class="sxs-lookup"><span data-stu-id="c0bab-195">Template mapping in Data integration</span></span>

<span data-ttu-id="c0bab-196">האיורים הבאים מציגים דוגמאות למיפויי משימות התבנית בשילוב נתונים.</span><span class="sxs-lookup"><span data-stu-id="c0bab-196">The following illustrations show examples of the template task mappings in Data integration.</span></span> <span data-ttu-id="c0bab-197">המיפוי מציג את פרטי השדה שיסונכרנו מ- Finance ל- Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="c0bab-197">The mapping shows the field information that will be synchronized from Finance to Project Service Automation.</span></span>

<span data-ttu-id="c0bab-198">[![מיפוי תבניות - ‏‫עדכון נתונים בפועל](./media/ActualsUpdateMapping.jpg)](./media/ActualsUpdateMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="c0bab-198">[![Template mapping - Actuals update](./media/ActualsUpdateMapping.jpg)](./media/ActualsUpdateMapping.jpg)</span></span>

<span data-ttu-id="c0bab-199">[![מיפוי תבניות - ‏‫עדכון עסקאות](./media/TransactionConnectionsUpdate.jpg)](./media/TransactionConnectionsUpdate.jpg)</span><span class="sxs-lookup"><span data-stu-id="c0bab-199">[![Template mapping - Transaction update](./media/TransactionConnectionsUpdate.jpg)](./media/TransactionConnectionsUpdate.jpg)</span></span>
