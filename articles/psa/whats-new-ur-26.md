---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 26 V3
ms.openlocfilehash: 849e7288ee91d3e9360c0b03f6b8b37ff29338e7
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 11/25/2020
ms.locfileid: "4643264"
---
<a name="project-service-automation-update-release-26-v3"></a><span data-ttu-id="19792-102">מהדורה 26, V3 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="19792-102">Project Service Automation Update Release 26, V3</span></span>
================================================

<span data-ttu-id="19792-103">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="19792-103">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="19792-104">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="19792-104">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="19792-105">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="19792-105">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="19792-106">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="19792-106">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="19792-107">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="19792-107">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="19792-108">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 26, עדכון V3 של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="19792-108">This topic lists the features and fixes that are new or changed for Project Service Automation Update Release 26, V3.</span></span> <span data-ttu-id="19792-109">לגרסה זו יש מספר build של V3.10.44.59 והיא זמינה בדרך כלל באמצעות עדכון עצמי בדצמבר 2020.</span><span class="sxs-lookup"><span data-stu-id="19792-109">This version has a build number of V3.10.44.59 and is generally available through a self-update in December 2020.</span></span>

<a name="update-release-26"></a><span data-ttu-id="19792-110">הפצת עדכון 26</span><span class="sxs-lookup"><span data-stu-id="19792-110">Update Release 26</span></span>
-----------------

### <a name="bug-fixes"></a><span data-ttu-id="19792-111">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="19792-111">Bug fixes</span></span>

<span data-ttu-id="19792-112">**זמן והוצאה**</span><span class="sxs-lookup"><span data-stu-id="19792-112">**Time and Expense**</span></span>

<span data-ttu-id="19792-113">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="19792-113">The following issues have been fixed:</span></span>

-   <span data-ttu-id="19792-114">משתמשים יכולים לשנות את המשימה ברישום זמן שאושר/נשלח.</span><span class="sxs-lookup"><span data-stu-id="19792-114">Users are able to change the task on a time entry that has been approved/submitted.</span></span>

-   <span data-ttu-id="19792-115">שגיאת "הפניה לאובייקט לא מוגדר" בעת שמירת ערך זמן.</span><span class="sxs-lookup"><span data-stu-id="19792-115">"Object Reference Not Set" error when saving time entry.</span></span>

-   <span data-ttu-id="19792-116">ייבוא ערך זמן מהקצאות משאבים יוצר ערכי זמן עם ערכי DateTime שגויים.</span><span class="sxs-lookup"><span data-stu-id="19792-116">Time entry import from resource assignments creates time entries with the incorrect DateTime values.</span></span>

-   <span data-ttu-id="19792-117">כאשר גם Project Service Automation וגם Field Service מותקנים, הלחצן **חדש** מופיע פעמיים בסרגל הפקודות עבור ערכי זמן ביישום Field Service.</span><span class="sxs-lookup"><span data-stu-id="19792-117">When Project Service Automation and the Field Service app are both installed, the **New** button is displaying twice on the command bar for time entries in the Field Service app.</span></span>

-   <span data-ttu-id="19792-118">עדכונים של התאים **אפשר יחידה** ו **קבוצת יחידות** פועלים כעת ברשת **אומדני הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="19792-118">**Allow Unit** and **Unit group** cells updates now work on the **Expense Estimates** grid.</span></span>

-   <span data-ttu-id="19792-119">הטופס **עדכן עריכה של ערך זמן** כולל **ציר זמן**.</span><span class="sxs-lookup"><span data-stu-id="19792-119">**Update Time Entry Edit** form includes **Timeline**.</span></span>

-   <span data-ttu-id="19792-120">אישור זמן לערכי זמן שאינם שייכים לפרויקט חוסם את המערכת בעת חיפוש תפקיד מאשר פרויקט.</span><span class="sxs-lookup"><span data-stu-id="19792-120">Time approval for non-project time entries blocks the system when searching for a project approver role.</span></span>

<span data-ttu-id="19792-121">**ניהול משאבים**</span><span class="sxs-lookup"><span data-stu-id="19792-121">**Resource Management**</span></span>

<span data-ttu-id="19792-122">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="19792-122">The following issues have been fixed:</span></span>

-   <span data-ttu-id="19792-123">נוסף אימות ביישום plug-in **PostProjectCreate** כדי לבדוק דרישה עיקרית לפני יצירת יישום מסוג זה.</span><span class="sxs-lookup"><span data-stu-id="19792-123">Added validation in the **PostProjectCreate** plug-in to check for a primary requirement before creating one.</span></span>

-   <span data-ttu-id="19792-124">טופס יצירה מהירה **חבר בצוות הפרויקט** יוצר חריגה להפניה null אם שדות מוסרים מהטופס.</span><span class="sxs-lookup"><span data-stu-id="19792-124">**Project Team Member** quick create form throws a null reference exception if fields are removed from the form.</span></span>

-   <span data-ttu-id="19792-125">יצירת דרישות למשך 12 שעות מעל לשנה נכשלת.</span><span class="sxs-lookup"><span data-stu-id="19792-125">Generate requirements for 12 hours over 1 year will fail.</span></span>

-   <span data-ttu-id="19792-126">שופרה הודעת שגיאה על חריגה עם הפניה null במהלך יצירת דרישת משאב.</span><span class="sxs-lookup"><span data-stu-id="19792-126">Improved error message null reference exception during resource requirement creation.</span></span>

<span data-ttu-id="19792-127">**ניהול פרויקט**</span><span class="sxs-lookup"><span data-stu-id="19792-127">**Project Management**</span></span>

<span data-ttu-id="19792-128">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="19792-128">The following issues have been fixed:</span></span>

-   <span data-ttu-id="19792-129">אימות משופר לטיפול בחריגות עם הפניה null שנוצרו ביישום plug-in **PreProjectUpdate**.</span><span class="sxs-lookup"><span data-stu-id="19792-129">Improved validation to address null reference exception generated in the **PreProjectUpdate** plug-in.</span></span>

-   <span data-ttu-id="19792-130">פרויקטים שפורסמו על ידי התוספת השולחנית של Microsoft Project מוחקים מטלות שלא הוקצו.</span><span class="sxs-lookup"><span data-stu-id="19792-130">Projects published by the Microsoft Project desktop add-in delete unassigned assignments.</span></span>

-   <span data-ttu-id="19792-131">נוסף אימות חדש כאשר הפניה לפרויקט של משימה אינה חוקית עקב חריגה עם הפניה null ביישום plug-in **PreValidateProjectTaskUpdate**.</span><span class="sxs-lookup"><span data-stu-id="19792-131">Added new validation when a task’s project reference is invalid due to null reference exception in **PreValidateProjectTaskUpdate** plug-in.</span></span>

-   <span data-ttu-id="19792-132">רשת חברי הצוות אינה מציגה משימות נפרדות ברשומת חבר הצוות.</span><span class="sxs-lookup"><span data-stu-id="19792-132">Team Member grid does not show distinct assignments on the team member record.</span></span>

-   <span data-ttu-id="19792-133">נוספו הודעות אימות והודעות שגיאה חדשות עקב חריגה של הפניה null ביישום plug-in **PreProjectTaskDelete**.</span><span class="sxs-lookup"><span data-stu-id="19792-133">Added new validation and error messages due to null reference exception in **PreProjectTaskDelete** plug-in.</span></span>

<span data-ttu-id="19792-134">**Sales**</span><span class="sxs-lookup"><span data-stu-id="19792-134">**Sales**</span></span>

<span data-ttu-id="19792-135">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="19792-135">The following issues have been fixed:</span></span>

-   <span data-ttu-id="19792-136">בעת בחירת שורה מבוססת פרויקט בהצעת מחיר או חוזה, הלחצן **הצעה** אמור להיות גלוי רק כשבוחרים שורה מבוססת מוצר המשויכת למוצר קיים.</span><span class="sxs-lookup"><span data-stu-id="19792-136">When selecting a project-based line in quote or contract, the **Suggestion** button should only be visible when selecting a product-based line associated with an existing product.</span></span>

-   <span data-ttu-id="19792-137">פיצול הראשה **Create_Product** מהרשאה **Create_ProjectContract**.</span><span class="sxs-lookup"><span data-stu-id="19792-137">Split **Create_Product** privilege from **Create_ProjectContract** privilege.</span></span>

-   <span data-ttu-id="19792-138">מחיקת שורה בחשבונית גורמת לכשל בהפניה null ב- **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span><span class="sxs-lookup"><span data-stu-id="19792-138">Deleting an invoice line causes null reference failure on **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span></span>
