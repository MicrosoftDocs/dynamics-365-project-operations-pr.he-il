---
title: סנכרון משימות פרוייקטים ישירות מ- Project Service Automation ל- Finance and Operations
description: נושא זה מתאר את התבנית ואת המשימה הבסיסית המשמשות לסנכרון משימות פרוייקט ישירות מ- Microsoft Dynamics 365 Project Service Automation אל Dynamics 365 Finance.
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
ms.assetid: d7f32327-33c4-43ab-b799-786210e93277
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 66a255346727c7ee4fbbf2920d2ef437ded03308
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751870"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="e8a43-103">סנכרון משימות פרוייקטים ישירות מ- Project Service Automation ל- Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="e8a43-103">Synchronize project tasks directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="e8a43-104">נושא זה מתאר את התבנית ואת המשימה הבסיסית המשמשות לסנכרון משימות פרוייקט ישירות מ- Dynamics 365 Project Service Automation אל Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="e8a43-104">This topic describes the template and underlying task that are used to synchronize project tasks directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="e8a43-105">שילוב משימות פרוייקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונעילת פונקציונליות זמינים בגירסה 8.0.</span><span class="sxs-lookup"><span data-stu-id="e8a43-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="e8a43-106">אם אתה משתמש ב- Enterprise Edition 7.3.0, לאחר התקנת KB 4132657 ו- KB 4132660, תוכל להשתמש בתבניות לשילוב משימות פרוייקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונתונים בפועל, וכן להגדיר תצורה של נעילת פונקציונליות.</span><span class="sxs-lookup"><span data-stu-id="e8a43-106">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="e8a43-107">אם עליך לאפס את ההפצות החשבונאיות, מומלץ להתקין גם את KB 4131710.</span><span class="sxs-lookup"><span data-stu-id="e8a43-107">If you must reset the accounting distributions, we recommended that you also install KB 4131710.</span></span>
> - <span data-ttu-id="e8a43-108">שילוב נתונים בפועל זמין בגירסה 8.0.1 ואילך.</span><span class="sxs-lookup"><span data-stu-id="e8a43-108">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="e8a43-109">זרימת נתונים עבור Project Service Automation ל- Finance</span><span class="sxs-lookup"><span data-stu-id="e8a43-109">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="e8a43-110">פתרון השילוב Project Service Automation ל- Finance משתמש בתכונת שילוב הנתונים לסנכרון נתונים במופעים של Project Service Automation ו- Finance.</span><span class="sxs-lookup"><span data-stu-id="e8a43-110">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="e8a43-111">תבנית השילוב שזמינה עם תכונת שילוב הנתונים מאפשרת זרימת נתונים על משימות פרוייקט מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="e8a43-111">The integration template that is available with the Data integration feature enables the flow of data about project tasks from Project Service Automation to Finance.</span></span>

<span data-ttu-id="e8a43-112">האיור הבא מראה כיצד הנתונים מסונכרנים בין Project Service Automation ו- Finance.</span><span class="sxs-lookup"><span data-stu-id="e8a43-112">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="e8a43-113">[![זרימת נתונים לשילוב Project Service Automation עם Finance](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span><span class="sxs-lookup"><span data-stu-id="e8a43-113">[![Data flow for Project Service Automation integration with Finance](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span></span>

## <a name="template-and-task"></a><span data-ttu-id="e8a43-114">תבנית ומשימה</span><span class="sxs-lookup"><span data-stu-id="e8a43-114">Template and task</span></span>

<span data-ttu-id="e8a43-115">כדי לגשת לתבנית, במרכז הניהול של Microsoft Power Apps, בחר **פרוייקטים** ולאחר מכן, בפינה העליונה, בחר **פרוייקט חדש** כדי לבחור תבניות ציבוריות.</span><span class="sxs-lookup"><span data-stu-id="e8a43-115">To access the template, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="e8a43-116">התבנית והמשימה הבסיסית הבאות משמשות לסנכרון משימות פרוייקט מ- Project Service Automation אל Finance:</span><span class="sxs-lookup"><span data-stu-id="e8a43-116">The following template and underlying task are used to synchronize project tasks from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="e8a43-117">**שם התבנית בשילוב נתונים:** משימות פרוייקט (PSA ל- Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="e8a43-117">**Name of the template in Data integration:** Project tasks (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="e8a43-118">**שם המשימה בפרוייקט:** משימות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e8a43-118">**Name of the task in the project:** Project tasks</span></span>

<span data-ttu-id="e8a43-119">עליך לסנכרן חוזי פרוייקטים ופרוייקטים לפני שתוכל לסנכרן משימות פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="e8a43-119">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="entity-set"></a><span data-ttu-id="e8a43-120">קבוצת ישויות</span><span class="sxs-lookup"><span data-stu-id="e8a43-120">Entity set</span></span>

| <span data-ttu-id="e8a43-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="e8a43-121">Project Service Automation</span></span> | <span data-ttu-id="e8a43-122">כספים</span><span class="sxs-lookup"><span data-stu-id="e8a43-122">Finance</span></span>                             |
|----------------------------|-------------------------------------|
| <span data-ttu-id="e8a43-123">משימות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e8a43-123">Project Tasks</span></span>              | <span data-ttu-id="e8a43-124">ישות שילוב למשימת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="e8a43-124">Integration entity for project task</span></span> |

## <a name="entity-flow"></a><span data-ttu-id="e8a43-125">זרימת ישות</span><span class="sxs-lookup"><span data-stu-id="e8a43-125">Entity flow</span></span>

<span data-ttu-id="e8a43-126">משימות פרוייקטים מנוהלות ב- Project Service Automation והם מסונכרנים ל- Finance כפעילויות פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="e8a43-126">Project tasks are managed in Project Service Automation, and they are synchronized to Finance as project activities.</span></span>

## <a name="prerequisites-and-mapping-setup"></a><span data-ttu-id="e8a43-127">דרישות מוקדמות והגדרת מיפוי</span><span class="sxs-lookup"><span data-stu-id="e8a43-127">Prerequisites and mapping setup</span></span>

<span data-ttu-id="e8a43-128">עליך לסנכרן חוזי פרוייקטים ופרוייקטים לפני שתוכל לסנכרן משימות פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="e8a43-128">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="power-query"></a><span data-ttu-id="e8a43-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="e8a43-129">Power Query</span></span>

<span data-ttu-id="e8a43-130">עליך להשתמש ב- Microsoft Power Query for Excel כדי לסנן נתונים אם מתקיים התנאי הזה:</span><span class="sxs-lookup"><span data-stu-id="e8a43-130">You must use Microsoft Power Query for Excel to filter data if this condition is met:</span></span>

- <span data-ttu-id="e8a43-131">יש לך רשומות ספציפיות למשאבים במשימת הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="e8a43-131">You have resource-specific records in a project task.</span></span>

<span data-ttu-id="e8a43-132">אם עליך להשתמש ב- Power Query, פעל לפי ההנחיה זו:</span><span class="sxs-lookup"><span data-stu-id="e8a43-132">If you must use Power Query, follow this guideline:</span></span>

- <span data-ttu-id="e8a43-133">תבנית משימות הפרוייקט (PSA ל- Fin and Ops) כוללת מסנן ברירת מחדל המסנן רשומות ספציפיות למשאבים ממשימת פרוייקט על ידי הגדרת המסנן ל- **IsLineTask** בתור **False**.</span><span class="sxs-lookup"><span data-stu-id="e8a43-133">The Project tasks (PSA to Fin and Ops) template has a default filter that excludes resource-specific records from a project task by setting the filter on **IsLineTask** to **False**.</span></span> <span data-ttu-id="e8a43-134">אם אתה יוצר תבנית משלך, עליך להוסיף מסנן זה.</span><span class="sxs-lookup"><span data-stu-id="e8a43-134">If you create your own template, you must add this filter.</span></span>

## <a name="template-mapping-in-data-integration"></a><span data-ttu-id="e8a43-135">מיפוי תבנית בשילוב נתונים</span><span class="sxs-lookup"><span data-stu-id="e8a43-135">Template mapping in Data integration</span></span>

<span data-ttu-id="e8a43-136">האיור הבא מציג דוגמה למיפויי משימת התבנית בשילוב נתונים.</span><span class="sxs-lookup"><span data-stu-id="e8a43-136">The following illustration shows an example of the template task mappings in Data integration.</span></span> <span data-ttu-id="e8a43-137">המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="e8a43-137">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="e8a43-138">[![מיפוי תבנית](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span><span class="sxs-lookup"><span data-stu-id="e8a43-138">[![Template mapping](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span></span>
