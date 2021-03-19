---
title: סנכרון משימות פרויקטים ישירות מ- Project Service Automation ל- Finance and Operations
description: נושא זה מתאר את התבנית ואת המשימה הבסיסית המשמשות לסנכרון משימות פרויקט ישירות מ- Microsoft Dynamics 365 Project Service Automation אל Dynamics 365 Finance.
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
ms.openlocfilehash: 7cc9ee9de576549c132e14c333a1000c22a55236
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288920"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="fddab-103">סנכרון משימות פרויקטים ישירות מ- Project Service Automation ל- Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="fddab-103">Synchronize project tasks directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="fddab-104">נושא זה מתאר את התבנית ואת המשימה הבסיסית המשמשות לסנכרון משימות פרויקט ישירות מ- Dynamics 365 Project Service Automation אל Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="fddab-104">This topic describes the template and underlying task that are used to synchronize project tasks directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="fddab-105">שילוב משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונעילת פונקציונליות זמינים בגירסה 8.0.</span><span class="sxs-lookup"><span data-stu-id="fddab-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="fddab-106">אם אתה משתמש ב- Enterprise Edition 7.3.0, לאחר התקנת KB 4132657 ו- KB 4132660, תוכל להשתמש בתבניות לשילוב משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונתונים בפועל, וכן להגדיר תצורה של נעילת פונקציונליות.</span><span class="sxs-lookup"><span data-stu-id="fddab-106">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="fddab-107">אם עליך לאפס את ההפצות החשבונאיות, מומלץ להתקין גם את KB 4131710.</span><span class="sxs-lookup"><span data-stu-id="fddab-107">If you must reset the accounting distributions, we recommended that you also install KB 4131710.</span></span>
> - <span data-ttu-id="fddab-108">שילוב נתונים בפועל זמין בגירסה 8.0.1 ואילך.</span><span class="sxs-lookup"><span data-stu-id="fddab-108">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="fddab-109">זרימת נתונים עבור Project Service Automation ל- Finance</span><span class="sxs-lookup"><span data-stu-id="fddab-109">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="fddab-110">פתרון השילוב Project Service Automation ל- Finance משתמש בתכונת שילוב הנתונים לסנכרון נתונים במופעים של Project Service Automation ו- Finance.</span><span class="sxs-lookup"><span data-stu-id="fddab-110">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="fddab-111">תבנית השילוב שזמינה עם תכונת שילוב הנתונים מאפשרת זרימת נתונים על משימות פרויקט מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="fddab-111">The integration template that is available with the Data integration feature enables the flow of data about project tasks from Project Service Automation to Finance.</span></span>

<span data-ttu-id="fddab-112">האיור הבא מראה כיצד הנתונים מסונכרנים בין Project Service Automation ו- Finance.</span><span class="sxs-lookup"><span data-stu-id="fddab-112">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="fddab-113">[![זרימת נתונים לשילוב Project Service Automation עם Finance](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span><span class="sxs-lookup"><span data-stu-id="fddab-113">[![Data flow for Project Service Automation integration with Finance](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span></span>

## <a name="template-and-task"></a><span data-ttu-id="fddab-114">תבנית ומשימה</span><span class="sxs-lookup"><span data-stu-id="fddab-114">Template and task</span></span>

<span data-ttu-id="fddab-115">כדי לגשת לתבנית, במרכז הניהול של Microsoft Power Apps, בחר **פרויקטים** ולאחר מכן, בפינה העליונה, בחר **פרויקט חדש** כדי לבחור תבניות ציבוריות.</span><span class="sxs-lookup"><span data-stu-id="fddab-115">To access the template, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="fddab-116">התבנית והמשימה הבסיסית הבאות משמשות לסנכרון משימות פרויקט מ- Project Service Automation אל Finance:</span><span class="sxs-lookup"><span data-stu-id="fddab-116">The following template and underlying task are used to synchronize project tasks from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="fddab-117">**שם התבנית בשילוב נתונים:** משימות פרויקט (PSA ל- Fin and Ops)</span><span class="sxs-lookup"><span data-stu-id="fddab-117">**Name of the template in Data integration:** Project tasks (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="fddab-118">**שם המשימה בפרויקט:** משימות פרויקט</span><span class="sxs-lookup"><span data-stu-id="fddab-118">**Name of the task in the project:** Project tasks</span></span>

<span data-ttu-id="fddab-119">עליך לסנכרן חוזי פרויקטים ופרויקטים לפני שתוכל לסנכרן משימות פרויקט.</span><span class="sxs-lookup"><span data-stu-id="fddab-119">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="entity-set"></a><span data-ttu-id="fddab-120">קבוצת ישויות</span><span class="sxs-lookup"><span data-stu-id="fddab-120">Entity set</span></span>

| <span data-ttu-id="fddab-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="fddab-121">Project Service Automation</span></span> | <span data-ttu-id="fddab-122">כספים</span><span class="sxs-lookup"><span data-stu-id="fddab-122">Finance</span></span>                             |
|----------------------------|-------------------------------------|
| <span data-ttu-id="fddab-123">משימות פרויקט</span><span class="sxs-lookup"><span data-stu-id="fddab-123">Project Tasks</span></span>              | <span data-ttu-id="fddab-124">ישות שילוב למשימת פרויקט</span><span class="sxs-lookup"><span data-stu-id="fddab-124">Integration entity for project task</span></span> |

## <a name="entity-flow"></a><span data-ttu-id="fddab-125">זרימת ישות</span><span class="sxs-lookup"><span data-stu-id="fddab-125">Entity flow</span></span>

<span data-ttu-id="fddab-126">משימות פרויקטים מנוהלות ב- Project Service Automation והם מסונכרנים ל- Finance כפעילויות פרויקט.</span><span class="sxs-lookup"><span data-stu-id="fddab-126">Project tasks are managed in Project Service Automation, and they are synchronized to Finance as project activities.</span></span>

## <a name="prerequisites-and-mapping-setup"></a><span data-ttu-id="fddab-127">דרישות מוקדמות והגדרת מיפוי</span><span class="sxs-lookup"><span data-stu-id="fddab-127">Prerequisites and mapping setup</span></span>

<span data-ttu-id="fddab-128">עליך לסנכרן חוזי פרויקטים ופרויקטים לפני שתוכל לסנכרן משימות פרויקט.</span><span class="sxs-lookup"><span data-stu-id="fddab-128">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="power-query"></a><span data-ttu-id="fddab-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="fddab-129">Power Query</span></span>

<span data-ttu-id="fddab-130">עליך להשתמש ב- Microsoft Power Query for Excel כדי לסנן נתונים אם מתקיים התנאי הזה:</span><span class="sxs-lookup"><span data-stu-id="fddab-130">You must use Microsoft Power Query for Excel to filter data if this condition is met:</span></span>

- <span data-ttu-id="fddab-131">יש לך רשומות ספציפיות למשאבים במשימת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="fddab-131">You have resource-specific records in a project task.</span></span>

<span data-ttu-id="fddab-132">אם עליך להשתמש ב- Power Query, פעל לפי ההנחיה זו:</span><span class="sxs-lookup"><span data-stu-id="fddab-132">If you must use Power Query, follow this guideline:</span></span>

- <span data-ttu-id="fddab-133">תבנית משימות הפרויקט (PSA ל- Fin and Ops) כוללת מסנן ברירת מחדל המסנן רשומות ספציפיות למשאבים ממשימת פרויקט על ידי הגדרת המסנן ל- **IsLineTask** בתור **False**.</span><span class="sxs-lookup"><span data-stu-id="fddab-133">The Project tasks (PSA to Fin and Ops) template has a default filter that excludes resource-specific records from a project task by setting the filter on **IsLineTask** to **False**.</span></span> <span data-ttu-id="fddab-134">אם אתה יוצר תבנית משלך, עליך להוסיף מסנן זה.</span><span class="sxs-lookup"><span data-stu-id="fddab-134">If you create your own template, you must add this filter.</span></span>

## <a name="template-mapping-in-data-integration"></a><span data-ttu-id="fddab-135">מיפוי תבנית בשילוב נתונים</span><span class="sxs-lookup"><span data-stu-id="fddab-135">Template mapping in Data integration</span></span>

<span data-ttu-id="fddab-136">האיור הבא מציג דוגמה למיפויי משימת התבנית בשילוב נתונים.</span><span class="sxs-lookup"><span data-stu-id="fddab-136">The following illustration shows an example of the template task mappings in Data integration.</span></span> <span data-ttu-id="fddab-137">המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="fddab-137">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="fddab-138">[![מיפוי תבנית](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span><span class="sxs-lookup"><span data-stu-id="fddab-138">[![Template mapping](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]