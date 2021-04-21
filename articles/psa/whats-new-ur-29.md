---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 29 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 29, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/22/2021
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 0e1ff0db42adb8b991b26dca1585bd603b2e2276
ms.sourcegitcommit: f57408d6637f670b920d7ce95f8ace8eb1963093
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/17/2021
ms.locfileid: "5664644"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-29-v3"></a><span data-ttu-id="edf84-103">מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 29 V3</span><span class="sxs-lookup"><span data-stu-id="edf84-103">What's new or changed in Project Service Automation Update Release 29, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="edf84-104">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="edf84-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="edf84-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="edf84-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="edf84-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="edf84-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="edf84-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="edf84-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="edf84-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="edf84-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="edf84-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 29, עדכון V3 של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="edf84-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 29.</span></span> <span data-ttu-id="edf84-110">לגרסה זו יש מספר build של V3.10.47.7 והיא זמינה בדרך כלל באמצעות עדכון עצמי בפברואר 2021.</span><span class="sxs-lookup"><span data-stu-id="edf84-110">This version has a build number of V3.10.47.7 and is generally available through a self-update in February 2021.</span></span>

## <a name="update-release-29"></a><span data-ttu-id="edf84-111">הפצת עדכון 29</span><span class="sxs-lookup"><span data-stu-id="edf84-111">Update Release 29</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="edf84-112">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="edf84-112">Bug fixes</span></span>

<span data-ttu-id="edf84-113">**זמן והוצאה**</span><span class="sxs-lookup"><span data-stu-id="edf84-113">**Time and Expense**</span></span>

<span data-ttu-id="edf84-114">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="edf84-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="edf84-115">משתמשים לא יכולים לראות את שעות העבודה המחוברות לימי עבודה שאינם ברשת ערכי הזמן.</span><span class="sxs-lookup"><span data-stu-id="edf84-115">Users can't see working hours logged on non-working days in the time entry grid.</span></span>
- <span data-ttu-id="edf84-116">ניתן לערוך רשומות הוצאות מאושרות ברשת.</span><span class="sxs-lookup"><span data-stu-id="edf84-116">Approved expense entries can be edited on the grid.</span></span>

<span data-ttu-id="edf84-117">**ניהול פרויקט**</span><span class="sxs-lookup"><span data-stu-id="edf84-117">**Project Management**</span></span>

<span data-ttu-id="edf84-118">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="edf84-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="edf84-119">לוגיקה של אימות חסר כדי להבטיח שעות עבודה של הקצאת משאבים לא יכולה להיות שלילית.</span><span class="sxs-lookup"><span data-stu-id="edf84-119">Missing validation logic to ensure resource assignment effort hours can't be negative.</span></span>
- <span data-ttu-id="edf84-120">הפעולה המותאמת אישית, **AssignResourcesForTask**, מעדכנת את כל השדות במקום רק שדות שהשתנו.</span><span class="sxs-lookup"><span data-stu-id="edf84-120">The custom action, **AssignResourcesForTask** updates all fields instead of only changed fields.</span></span>
- <span data-ttu-id="edf84-121">בעת העתקת פרויקט בסביבה עם תוספים או תהליכי עבודה הרשומים באירוע **CreateProject**, התכונה **msdyn_bulkgenerationstatus** לא מעודכנת אם הפעולה **CopyWBSToProject** נכשלה.</span><span class="sxs-lookup"><span data-stu-id="edf84-121">When copying a project in an environment with plug-ins or workflows that are registered on the **CreateProject** event, the **msdyn_bulkgenerationstatus** attribute isn't updated if the **CopyWBSToProject** fails.</span></span>
- <span data-ttu-id="edf84-122">כשאתה מרחיב את לוח השנה של הפרויקט, ימי העבודה אינם ממוינים בסדר עולה וגורמים לכמה עדכונים של משימות הפרויקט להיכשל.</span><span class="sxs-lookup"><span data-stu-id="edf84-122">When you expand the project calendar, the working days aren't sorted in ascending order causing some project task updates to fail.</span></span>
- <span data-ttu-id="edf84-123">שינוי מנהל הפרויקט בפרויקט קיים מפעיל את ברירת המחדל של הלוגיקה של היחידה הארגונית.</span><span class="sxs-lookup"><span data-stu-id="edf84-123">Changing the Project Manager on an existing project triggers the organizational unit defaulting logic.</span></span>

<span data-ttu-id="edf84-124">**מכירות**</span><span class="sxs-lookup"><span data-stu-id="edf84-124">**Sales**</span></span>

<span data-ttu-id="edf84-125">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="edf84-125">The following issues have been fixed:</span></span>

- <span data-ttu-id="edf84-126">הכרטיסיה **ביצועי חוזה** בדף **חוזה** נכשלת באופן שקט במהלך האתחול כאשר לא קיימים סעיפי חוזה.</span><span class="sxs-lookup"><span data-stu-id="edf84-126">The **Contract Performance** tab on the **Contract** page fails silently during initialization when no contract lines are present.</span></span>
