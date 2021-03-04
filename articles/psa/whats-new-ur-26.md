---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 26 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 26, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/12/2021
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
ms.openlocfilehash: 14fcccf5804e5da0926dbc69bdfa040229a7f068
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5143559"
---
# <a name="project-service-automation-update-release-26-v3"></a><span data-ttu-id="5c597-103">מהדורה 26, V3 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="5c597-103">Project Service Automation Update Release 26, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="5c597-104">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="5c597-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="5c597-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="5c597-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="5c597-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="5c597-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="5c597-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="5c597-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="5c597-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="5c597-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="5c597-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 26, עדכון V3 של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="5c597-109">This topic lists the features and fixes that are new or changed for Project Service Automation Update Release 26, V3.</span></span> <span data-ttu-id="5c597-110">לגרסה זו יש מספר build של V3.10.44.59 והיא זמינה בדרך כלל באמצעות עדכון עצמי בדצמבר 2020.</span><span class="sxs-lookup"><span data-stu-id="5c597-110">This version has a build number of V3.10.44.59 and is generally available through a self-update in December 2020.</span></span>

## <a name="update-release-26"></a><span data-ttu-id="5c597-111">הפצת עדכון 26</span><span class="sxs-lookup"><span data-stu-id="5c597-111">Update Release 26</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="5c597-112">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="5c597-112">Bug fixes</span></span>

<span data-ttu-id="5c597-113">**זמן והוצאה**</span><span class="sxs-lookup"><span data-stu-id="5c597-113">**Time and Expense**</span></span>

<span data-ttu-id="5c597-114">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="5c597-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="5c597-115">משתמשים יכולים לשנות את המשימה ברישום זמן שאושר/נשלח.</span><span class="sxs-lookup"><span data-stu-id="5c597-115">Users are able to change the task on a time entry that has been approved/submitted.</span></span>
- <span data-ttu-id="5c597-116">שגיאת "הפניה לאובייקט לא מוגדר" בעת שמירת ערך זמן.</span><span class="sxs-lookup"><span data-stu-id="5c597-116">"Object Reference Not Set" error when saving time entry.</span></span>
- <span data-ttu-id="5c597-117">ייבוא ערך זמן מהקצאות משאבים יוצר ערכי זמן עם ערכי DateTime שגויים.</span><span class="sxs-lookup"><span data-stu-id="5c597-117">Time entry import from resource assignments creates time entries with the incorrect DateTime values.</span></span>
- <span data-ttu-id="5c597-118">כאשר גם Project Service Automation וגם Field Service מותקנים, הלחצן **חדש** מופיע פעמיים בסרגל הפקודות עבור ערכי זמן ביישום Field Service.</span><span class="sxs-lookup"><span data-stu-id="5c597-118">When Project Service Automation and the Field Service app are both installed, the **New** button is displaying twice on the command bar for time entries in the Field Service app.</span></span>
- <span data-ttu-id="5c597-119">עדכונים של התאים **אפשר יחידה** ו **קבוצת יחידות** פועלים כעת ברשת **אומדני הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="5c597-119">**Allow Unit** and **Unit group** cells updates now work on the **Expense Estimates** grid.</span></span>
- <span data-ttu-id="5c597-120">הטופס **עדכן עריכה של ערך זמן** כולל **ציר זמן**.</span><span class="sxs-lookup"><span data-stu-id="5c597-120">**Update Time Entry Edit** form includes **Timeline**.</span></span>
- <span data-ttu-id="5c597-121">אישור זמן לערכי זמן שאינם שייכים לפרויקט חוסם את המערכת בעת חיפוש תפקיד מאשר פרויקט.</span><span class="sxs-lookup"><span data-stu-id="5c597-121">Time approval for non-project time entries blocks the system when searching for a project approver role.</span></span>

<span data-ttu-id="5c597-122">**ניהול משאבים**</span><span class="sxs-lookup"><span data-stu-id="5c597-122">**Resource Management**</span></span>

<span data-ttu-id="5c597-123">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="5c597-123">The following issues have been fixed:</span></span>

- <span data-ttu-id="5c597-124">נוסף אימות ביישום plug-in **PostProjectCreate** כדי לבדוק דרישה עיקרית לפני יצירת יישום מסוג זה.</span><span class="sxs-lookup"><span data-stu-id="5c597-124">Added validation in the **PostProjectCreate** plug-in to check for a primary requirement before creating one.</span></span>
- <span data-ttu-id="5c597-125">טופס יצירה מהירה **חבר בצוות הפרויקט** יוצר חריגה להפניה null אם שדות מוסרים מהטופס.</span><span class="sxs-lookup"><span data-stu-id="5c597-125">**Project Team Member** quick create form throws a null reference exception if fields are removed from the form.</span></span>
- <span data-ttu-id="5c597-126">יצירת דרישות למשך 12 שעות מעל לשנה נכשלת.</span><span class="sxs-lookup"><span data-stu-id="5c597-126">Generate requirements for 12 hours over 1 year will fail.</span></span>
- <span data-ttu-id="5c597-127">שופרה הודעת שגיאה על חריגה עם הפניה null במהלך יצירת דרישת משאב.</span><span class="sxs-lookup"><span data-stu-id="5c597-127">Improved error message null reference exception during resource requirement creation.</span></span>

<span data-ttu-id="5c597-128">**ניהול פרויקט**</span><span class="sxs-lookup"><span data-stu-id="5c597-128">**Project Management**</span></span>

<span data-ttu-id="5c597-129">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="5c597-129">The following issues have been fixed:</span></span>

- <span data-ttu-id="5c597-130">אימות משופר לטיפול בחריגות עם הפניה null שנוצרו ביישום plug-in **PreProjectUpdate**.</span><span class="sxs-lookup"><span data-stu-id="5c597-130">Improved validation to address null reference exception generated in the **PreProjectUpdate** plug-in.</span></span>
- <span data-ttu-id="5c597-131">פרויקטים שפורסמו על ידי התוספת השולחנית של Microsoft Project מוחקים מטלות שלא הוקצו.</span><span class="sxs-lookup"><span data-stu-id="5c597-131">Projects published by the Microsoft Project desktop add-in delete unassigned assignments.</span></span>
- <span data-ttu-id="5c597-132">נוסף אימות חדש כאשר הפניה לפרויקט של משימה אינה חוקית עקב חריגה עם הפניה null ביישום plug-in **PreValidateProjectTaskUpdate**.</span><span class="sxs-lookup"><span data-stu-id="5c597-132">Added new validation when a task’s project reference is invalid due to null reference exception in **PreValidateProjectTaskUpdate** plug-in.</span></span>
- <span data-ttu-id="5c597-133">רשת חברי הצוות אינה מציגה משימות נפרדות ברשומת חבר הצוות.</span><span class="sxs-lookup"><span data-stu-id="5c597-133">Team Member grid does not show distinct assignments on the team member record.</span></span>
- <span data-ttu-id="5c597-134">נוספו הודעות אימות והודעות שגיאה חדשות עקב חריגה של הפניה null ביישום plug-in **PreProjectTaskDelete**.</span><span class="sxs-lookup"><span data-stu-id="5c597-134">Added new validation and error messages due to null reference exception in **PreProjectTaskDelete** plug-in.</span></span>

<span data-ttu-id="5c597-135">**Sales**</span><span class="sxs-lookup"><span data-stu-id="5c597-135">**Sales**</span></span>

<span data-ttu-id="5c597-136">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="5c597-136">The following issues have been fixed:</span></span>

- <span data-ttu-id="5c597-137">בעת בחירת שורה מבוססת פרויקט בהצעת מחיר או חוזה, הלחצן **הצעה** אמור להיות גלוי רק כשבוחרים שורה מבוססת מוצר המשויכת למוצר קיים.</span><span class="sxs-lookup"><span data-stu-id="5c597-137">When selecting a project-based line in quote or contract, the **Suggestion** button should only be visible when selecting a product-based line associated with an existing product.</span></span>
- <span data-ttu-id="5c597-138">פיצול הראשה **Create_Product** מהרשאה **Create_ProjectContract**.</span><span class="sxs-lookup"><span data-stu-id="5c597-138">Split **Create_Product** privilege from **Create_ProjectContract** privilege.</span></span>
- <span data-ttu-id="5c597-139">מחיקת שורה בחשבונית גורמת לכשל בהפניה null ב- **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span><span class="sxs-lookup"><span data-stu-id="5c597-139">Deleting an invoice line causes null reference failure on **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span></span>
