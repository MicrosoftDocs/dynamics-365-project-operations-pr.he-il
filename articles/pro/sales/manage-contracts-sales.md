---
title: ניהול חוזי פרויקט
description: נושא זה מספק מידע על הצגת חוזים מבוססי פרויקט.
author: rumant
ms.date: 10/26/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5e2f182f66bd1f4fe57d19e4bf82525ac8b84c29
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003092"
---
# <a name="manage-project-contracts"></a><span data-ttu-id="3abc4-103">ניהול חוזי פרויקט</span><span class="sxs-lookup"><span data-stu-id="3abc4-103">Manage project contracts</span></span>

<span data-ttu-id="3abc4-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="3abc4-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="3abc4-105">חוזי פרויקט ב- Dynamics 365 Project Operations לוכדים ומנהלים את המחוייבויות עליהם סוכם בחוזים ואת פרטי החיוב של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="3abc4-105">Project contracts in Dynamics 365 Project Operations capture and manage the contractually agreed on commitments and billing details of a project.</span></span> <span data-ttu-id="3abc4-106">מבנה חוזה הפרויקט ב-Project Operations מותאם לעבודה מבוססת פרויקט עם המרכיבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="3abc4-106">The structure of a project contract in Project Operations is tailored to project-based work with the following components:</span></span>

- <span data-ttu-id="3abc4-107">סעיפי חוזה המזהים את רכיבי העבודה הנפרדים שיוצגו כרכיבים ברמה גבוהה בחשבונית פרויקט.</span><span class="sxs-lookup"><span data-stu-id="3abc4-107">Contract lines that identify the discrete components of work that will be presented as high-level components on a project invoice.</span></span>
- <span data-ttu-id="3abc4-108">פרטי סעיף חוזה המזהים ומעריכים את העבודה עבור כל רכיב או סעיף חוזה ברמה גבוהה.</span><span class="sxs-lookup"><span data-stu-id="3abc4-108">Contract line details that identify and estimate the work for each high-level component or contract line.</span></span> <span data-ttu-id="3abc4-109">ההערכה כוללת את לוח הזמנים ואת ההיבטים הכספיים של עבודות הקשורות לסעיף החוזה.</span><span class="sxs-lookup"><span data-stu-id="3abc4-109">The estimate includes the schedule and the financial aspects for the work tied to the contract line.</span></span>
- <span data-ttu-id="3abc4-110">מודלים של חוזים ורכיבים הניתנים לחיוב מוגדרים לכל סעיף חוזה המכיל את הסדר החיוב עבור כל סעיף חוזה ועבור החוזה המלא.</span><span class="sxs-lookup"><span data-stu-id="3abc4-110">Contracting models and chargeable components are set up for each contract line that holds the billing arrangement for each contract line and the overall contract.</span></span>

## <a name="view-all-project-based-contracts"></a><span data-ttu-id="3abc4-111">תצוגה של כל החוזים המבוססים על פרוייקטים</span><span class="sxs-lookup"><span data-stu-id="3abc4-111">View all project-based contracts</span></span>

<span data-ttu-id="3abc4-112">ניתן לראות רשימה של כל חוזים של פרויקטים בדף הרשימה **חוזים**.</span><span class="sxs-lookup"><span data-stu-id="3abc4-112">A list of all project contracts can be seen on the **Contracts** list page.</span></span> 

1. <span data-ttu-id="3abc4-113">עבור אל **מכירות** > **חוזים**.</span><span class="sxs-lookup"><span data-stu-id="3abc4-113">Go to **Sales** > **Contracts**.</span></span> <span data-ttu-id="3abc4-114">מוצגת רשימה של כל חוזי הפרויקט שלך במערכת.</span><span class="sxs-lookup"><span data-stu-id="3abc4-114">A list of all your project Contracts in the system are shown.</span></span> 
2. <span data-ttu-id="3abc4-115">בחר את **מחליף התצוגות** (החץ הנפתח לצד שם התצוגה) לבחירת תצוגות מסוננות אחרות.</span><span class="sxs-lookup"><span data-stu-id="3abc4-115">Select the **View switcher** (the drop-down arrow next to the name of the view) to select other filtered views.</span></span> <span data-ttu-id="3abc4-116">ניתן ליצור תצוגות משלך עם קריטריוני סינון מותאמים אישית.</span><span class="sxs-lookup"><span data-stu-id="3abc4-116">You can create your own views with custom filter criteria.</span></span>

<span data-ttu-id="3abc4-117">ניתן ליצור או למחוק חוזים מדף רשימה זה או מדפי הפרטים.</span><span class="sxs-lookup"><span data-stu-id="3abc4-117">Contracts can be created or deleted from this list page or detail pages.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]