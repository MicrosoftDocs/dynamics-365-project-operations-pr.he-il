---
title: מבט כולל על Project Service Automation
description: נושא זה מספק מידע על פתרון השילוב של Dynamics 365 Project Service Automation אל Dynamics 365 Finance.
author: ruhercul
ms.date: 07/25/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: ruhercul
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: ruhercul
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 5ca459b99881b612e4656be112c8a2e420b4196e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005882"
---
# <a name="project-service-automation-overview"></a><span data-ttu-id="39ae5-103">מבט כולל על Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="39ae5-103">Project Service Automation overview</span></span>

[!include[banner](../includes/banner.md)]
[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="39ae5-104">פתרון השילוב Project Service Automation ל- Finance משתמש בתכונת שילוב הנתונים לסנכרון נתונים במופעים של Dynamics 365 Finance ו- Dynamics 365 Project Service Automation באמצעות Common Data Service.</span><span class="sxs-lookup"><span data-stu-id="39ae5-104">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Dynamics 365 Finance and Dynamics 365 Project Service Automation via Common Data Service.</span></span> <span data-ttu-id="39ae5-105">תבניות השילוב שזמינות עם תכונת שילוב הנתונים מאפשרות זרימה של פרויקטים, חוזי פרויקט, סעיפי חוזה של פרויקט, אבני דרך בסעיפי חוזה של פרויקט, משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="39ae5-105">The integration templates that are available with the Data integration feature enable the flow of projects, project contracts, project contract lines, project contract line milestones, project tasks, expense transaction categories, hour estimates, and expense estimates from Project Service Automation to Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="39ae5-106">אם אתה משתמש בגירסה 7.3.0, עליך להתקין את KB 4074835.</span><span class="sxs-lookup"><span data-stu-id="39ae5-106">If you're using version 7.3.0, you must install KB 4074835.</span></span> <span data-ttu-id="39ae5-107">לאחר מכן תוכל לשלב פרויקטים במחיר קבוע.</span><span class="sxs-lookup"><span data-stu-id="39ae5-107">You will then be able to integrate fixed price projects.</span></span>
> - <span data-ttu-id="39ae5-108">אם אתה משתמש בגירסה 7.3.0 ואתה מעביר עסקאות עמלה מ- Project Service Automation, עליך להתקין את KB 4345320 כדי לכלול את העמלות בחשבונית הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="39ae5-108">If you're using version 7.3.0, and you are bringing fee transactions over from Project Service Automation, you must install KB 4345320 in order to include those fees in the project invoice.</span></span>
> - <span data-ttu-id="39ae5-109">אם אתה משתמש בגירסה 8.0, תוכל להשתמש בשילוב משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונעילת פונקציונליות.</span><span class="sxs-lookup"><span data-stu-id="39ae5-109">If you're using version 8.0, you will be able to use project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking.</span></span>
> - <span data-ttu-id="39ae5-110">אם אתה משתמש בגרסה 8.0.1 ואילך, תוכל לסנכרן את הנתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="39ae5-110">If you're using version 8.0.1 or later, you will be able to synchronize actuals.</span></span>

<span data-ttu-id="39ae5-111">לפני שתוכל לשלב את Project Service Automation Finance, עליך להגדיר את פרמטרי השילוב של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="39ae5-111">Before you can integrate Project Service Automation Finance, you must configure the Project Service Automation integration parameters.</span></span> <span data-ttu-id="39ae5-112">לקבלת מידע נוסף, ראה [פרמטרי שילוב של Project Service Automation](PSA-parameters.md).</span><span class="sxs-lookup"><span data-stu-id="39ae5-112">For more information, see [Project Service Automation integration parameters](PSA-parameters.md).</span></span>

<span data-ttu-id="39ae5-113">פתרון שילוב זה מאפשר סנכרון ישיר בתרחישים הבאים:</span><span class="sxs-lookup"><span data-stu-id="39ae5-113">This integration solution enables direct synchronization in the following scenarios:</span></span>

- <span data-ttu-id="39ae5-114">אחזקת חוזי פרויקט ב- Project Service Automation וסנכרון שלהם ישירות מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="39ae5-114">Maintain project contracts in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="39ae5-115">יצירת פרויקטים ב- Project Service Automation וסנכרון שלהם ישירות מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="39ae5-115">Create projects in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="39ae5-116">אחזקת סעיפי חוזים בפרויקט ב- Project Service Automation וסנכרון שלהם ישירות מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="39ae5-116">Maintain project contract lines in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="39ae5-117">אחזקת אבני דרך בסעיפי חוזים בפרויקט ב- Project Service Automation וסנכרון שלהם ישירות מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="39ae5-117">Maintain project contract line milestones in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="39ae5-118">אחזקת משימות פרויקט ב- Project Service Automation וסנכרון שלהן ישירות מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="39ae5-118">Maintain project tasks in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="39ae5-119">אחזקת קטגוריות של עסקאות הוצאות ב- Finance וסנכרון שלהן ישירות מ- Finance ל- Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="39ae5-119">Maintain expense transaction categories in Finance, and synchronize them directly from Finance to Project Service Automation.</span></span>
- <span data-ttu-id="39ae5-120">יצירת הערכות של שעות בפרויקטים ב- Project Service Automation וסנכרון שלהם ישירות מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="39ae5-120">Create project hour estimates in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="39ae5-121">יצירת הערכות של הוצאות בפרוייקטים ב- Project Service Automation וסנכרון שלהם ישירות מ- Project Service Automation ל- Finance.</span><span class="sxs-lookup"><span data-stu-id="39ae5-121">Create project expense estimates in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="39ae5-122">יצירת שעות בפרויקט, הוצאות ונתונים בפועל של עמלות ב- Project Service Automation, ויצירת עסקאות פרויקט ביומן שילוב של Project Service Automation כך שניתן יהיה לרשום אותם ב- Finance.</span><span class="sxs-lookup"><span data-stu-id="39ae5-122">Create project time, expense, and fee actuals in Project Service Automation, and create project transactions in the Project Service Automation integration journal so that they can be posted in Finance.</span></span>

## <a name="data-synchronization"></a><span data-ttu-id="39ae5-123">‏‏סינכרון נתונים</span><span class="sxs-lookup"><span data-stu-id="39ae5-123">Data synchronization</span></span>

<span data-ttu-id="39ae5-124">האיור הבא מראה כיצד נתונים מסונכרנים כחלק מהשילוב בין Project Service Automation ו- Finance.</span><span class="sxs-lookup"><span data-stu-id="39ae5-124">The following illustration shows how data is synchronized as part of the integration between Project Service Automation and Finance.</span></span>

> [!NOTE]
> <span data-ttu-id="39ae5-125">לא כל התבניות זמינות כרגע.</span><span class="sxs-lookup"><span data-stu-id="39ae5-125">Not all templates are currently available.</span></span> <span data-ttu-id="39ae5-126">התבניות ישוחררו עם השלמתן.</span><span class="sxs-lookup"><span data-stu-id="39ae5-126">Templates will be released as they are completed.</span></span>

<span data-ttu-id="39ae5-127">[![שילוב Project Service Automation עם Finance](./media/PSA-integration.png)](./media/PSA-integration.png)</span><span class="sxs-lookup"><span data-stu-id="39ae5-127">[![Project Service Automation integration with Finance](./media/PSA-integration.png)](./media/PSA-integration.png)</span></span>

## <a name="system-requirements-for-finance"></a><span data-ttu-id="39ae5-128">דרישות מערכת עבור Finance</span><span class="sxs-lookup"><span data-stu-id="39ae5-128">System requirements for Finance</span></span>

<span data-ttu-id="39ae5-129">כדי להשתמש בפתרון השילוב של Project Service Automation ל- Finance, עליך להתקין את Enterprise edition 7.3 עם עדכון 12 ואילך של הפלטפורמה.</span><span class="sxs-lookup"><span data-stu-id="39ae5-129">To use the Project Service Automation to Finance integration solution, you must install Enterprise edition 7.3 with Platform update 12 or later.</span></span>

## <a name="system-requirements-for-project-service-automation"></a><span data-ttu-id="39ae5-130">דרישות מערכת עבור Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="39ae5-130">System requirements for Project Service Automation</span></span>

<span data-ttu-id="39ae5-131">כדי להשתמש בפתרון השילוב Project Service Automation ל- Finance, עליך להתקין את הרכיבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="39ae5-131">To use the Project Service Automation to Finance integration solution, you must install the following components:</span></span>

- <span data-ttu-id="39ae5-132">Dynamics 365 Project Service Automation גירסה 9.0.0.0 ואילך</span><span class="sxs-lookup"><span data-stu-id="39ae5-132">Dynamics 365 Project Service Automation version 9.0.0.0 or later</span></span>
- <span data-ttu-id="39ae5-133">פתרון Prospect to Cash עבור Dynamics 365 Sales, גירסה 1.14.0.0 (v14) ואילך</span><span class="sxs-lookup"><span data-stu-id="39ae5-133">Prospect to cash solution for Dynamics 365 Sales, version 1.14.0.0 (v14) or later</span></span>
- <span data-ttu-id="39ae5-134">פתרון Project Service Automation ל- Finance solution עבור Dynamics 365 Project Service Automation גירסה 1.0.0.0 ואילך</span><span class="sxs-lookup"><span data-stu-id="39ae5-134">Project Service Automation to Finance solution for Dynamics 365 Project Service Automation version 1.0.0.0 or later</span></span>

## <a name="install-the-project-service-automation-to-finance-integration-solution-in-your-project-service-automation-instance"></a><span data-ttu-id="39ae5-135">התקן את פתרון השילוב Project Service Automation ל- Finance במופע Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="39ae5-135">Install the Project Service Automation to Finance integration solution in your Project Service Automation instance</span></span>

<span data-ttu-id="39ae5-136">הןרד את פתרון השילוב Project Service Automation ל- Finance מ[מרכז ההורדות של Microsoft](https://www.microsoft.com/download/details.aspx?id=57016), ופעל לפי ההנחיות הכלולות בפתרון.</span><span class="sxs-lookup"><span data-stu-id="39ae5-136">Download the Project Service Automation to Finance integration solution from [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=57016), and follow the instructions that are included with the solution.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]