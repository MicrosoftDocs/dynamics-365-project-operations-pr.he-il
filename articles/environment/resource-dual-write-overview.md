---
title: שילוב כתיבה כפולה של Project Operations
description: נושא זה מספק מבט על של שילוב כתיבה כפולה ב- Project Operations.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ce4f7bf8185e6f3f942df14d30d7b8d0a3e4444a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998682"
---
# <a name="project-operations-dual-write-integration-overview"></a><span data-ttu-id="f2327-103">מבט על של שילוב כתיבה כפולה ב- Project Operations</span><span class="sxs-lookup"><span data-stu-id="f2327-103">Project Operations dual-write integration overview</span></span>

<span data-ttu-id="f2327-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="f2327-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="f2327-105">Project Operations משתמש ב[יכולות כתיבה כפולה](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) כדי לסנכרן נתונים ב- Microsoft Dataverse ו- Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="f2327-105">Project Operations uses [dual-write capabilities](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) to synchronize data across Microsoft Dataverse and Dynamics 365 Finance.</span></span>

<span data-ttu-id="f2327-106">האיור הבא מראה כיצד נתונים מסונכרנים כחלק משילוב זה בין Dataverse ו- Finance.</span><span class="sxs-lookup"><span data-stu-id="f2327-106">The following illustration shows how data is synchronized as part of this integration between Dataverse and Finance.</span></span>

![מבט כולל על זרימות נתונים ב- Project Operations](./media/ProjectOperationsFlows.jpg)

<span data-ttu-id="f2327-108">Project Operations ב- Dataverse מספק ממשק משתמש (UI) מודרני שניתן להרחבה בקלות ללא קוד או עם מעט קוד באמצעות יכולות Power Platform.</span><span class="sxs-lookup"><span data-stu-id="f2327-108">Project Operations on Dataverse provides a modern user interface (UI) and easy no-code/low-code extensibility using Power Platform capabilities.</span></span> <span data-ttu-id="f2327-109">מנהלי פרויקטים, מנהלי משאבים, אנשי צוות פרוייקטים משתמשי משרד חזיתי אחרים, מבצעים את פעולותיהם ב- Project Operations ב- Dataverse.</span><span class="sxs-lookup"><span data-stu-id="f2327-109">Project managers, Resource managers, Project team members, and other front-office personas, perform their activities in Project Operations on Dataverse.</span></span>

<span data-ttu-id="f2327-110">Project Operations ב- Finance מספקת תמיכה בחשבונאות פרויקט ובהכרת הכנסות.</span><span class="sxs-lookup"><span data-stu-id="f2327-110">Project Operations in Finance provides project accounting and revenue recognition support.</span></span> <span data-ttu-id="f2327-111">Project Operations מתחברות למסגרת הפיננסית ב- Finance לצורך חישוב מע"מ, שערי חליפין, דיווח מימד פיננסי ועוד.</span><span class="sxs-lookup"><span data-stu-id="f2327-111">Project Operations plugs in to the financial framework in Finance for sales tax calculation, currency exchange rates, financial dimension reporting, and more.</span></span> <span data-ttu-id="f2327-112">חוויות רואה החשבון הפרויקט נמצאות בעיקר ב- Finance.</span><span class="sxs-lookup"><span data-stu-id="f2327-112">The Project accountant experiences are mostly based in Finance.</span></span>

<span data-ttu-id="f2327-113">שילוב Project Operations מורכב משילוב הרכיבים הבא:</span><span class="sxs-lookup"><span data-stu-id="f2327-113">Project Operations integration consists of the following component integration:</span></span>


- [<span data-ttu-id="f2327-114">שילוב נתוני התקנה ותצורה של Project Operations</span><span class="sxs-lookup"><span data-stu-id="f2327-114">Project Operations setup and configuration data integration</span></span>](resource-dual-write-setup-integration.md) 
- [<span data-ttu-id="f2327-115">הערכות ונתונים בפועל של פרויקט</span><span class="sxs-lookup"><span data-stu-id="f2327-115">Project estimates and actuals</span></span>](resource-dual-write-estimates-actuals.md)
- [<span data-ttu-id="f2327-116">חשבוניות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="f2327-116">Project invoices</span></span>](resource-dual-write-project-invoice.md)
- [<span data-ttu-id="f2327-117">ניהול הוצאות</span><span class="sxs-lookup"><span data-stu-id="f2327-117">Expense management</span></span>](resource-dual-write-expense.md)
- [<span data-ttu-id="f2327-118">חשבונית ספק</span><span class="sxs-lookup"><span data-stu-id="f2327-118">Vendor invoice</span></span>](resource-dual-write-vendor-invoice.md)
