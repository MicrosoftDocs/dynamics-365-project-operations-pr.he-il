---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 18 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 18, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 04/27/2020
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
ms.openlocfilehash: d6e0bb669513185ca266858ea9b8a89ed6dd4408
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147204"
---
# <a name="project-service-automation-update-release-18-v3"></a><span data-ttu-id="7d658-103">מהדורה 18, V3 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="7d658-103">Project Service Automation Update Release 18, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="7d658-104">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="7d658-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="7d658-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="7d658-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="7d658-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="7d658-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="7d658-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="7d658-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="7d658-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="7d658-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="7d658-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 18, עדכון V3 של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="7d658-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 18.</span></span> <span data-ttu-id="7d658-110">גירסה זו כוללת מספר build של V3.10.8.12 ובדרך כלל היא זמינה דרך עדכון עצמי באפריל 2020.</span><span class="sxs-lookup"><span data-stu-id="7d658-110">This version has a build number of V3.10.8.12 and is generally available through a self-update in April 2020.</span></span>

## <a name="update-release-18"></a><span data-ttu-id="7d658-111">הפצת עדכון 18</span><span class="sxs-lookup"><span data-stu-id="7d658-111">Update Release 18</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="7d658-112">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="7d658-112">Bug fixes</span></span>

<span data-ttu-id="7d658-113">**זמן והוצאה**</span><span class="sxs-lookup"><span data-stu-id="7d658-113">**Time and Expense**</span></span>

- <span data-ttu-id="7d658-114">תוקן: הזרימות **אחזר**, **בקש**, וגם **בטל אישור** יוצרות חריגות עם הודעות שגיאה לא ברורות.</span><span class="sxs-lookup"><span data-stu-id="7d658-114">Fixed: **Recall**, **Request**, and **Cancel Approval** flows throw exceptions with unclear error messages.</span></span>
- <span data-ttu-id="7d658-115">תוקן: כאשר האפשרות **בטל אישור** נכשלת עבור הוצאה, שגיאת חריגה רלוונטית לא מופיעה.</span><span class="sxs-lookup"><span data-stu-id="7d658-115">Fixed: When **Cancel Approval** fails for an expense, a relevant exception error is not thrown.</span></span>
- <span data-ttu-id="7d658-116">תוקן: רשת ערכי הזמן מטפלת בצורה לא נכונה בימים שאינם ימי עבודה באוסטרליה לאחר המעבר לשעון קיץ (DST) באוקטובר.</span><span class="sxs-lookup"><span data-stu-id="7d658-116">Fixed: The Time Entry grid incorrectly handles non-working days in Australia after the daylight savings time (DST) switch in October.</span></span>
- <span data-ttu-id="7d658-117">תוקן: לוגיקה שגויה של ברירת המחדל מונעת הגשת הוצאות.</span><span class="sxs-lookup"><span data-stu-id="7d658-117">Fixed: Incorrect defaulting logic prevents submission of expenses.</span></span>
- <span data-ttu-id="7d658-118">תוקן: כאשר אישור הזנת הזמן נכשל, האישור נשאר במצב **ממתין**.</span><span class="sxs-lookup"><span data-stu-id="7d658-118">Fixed: When time entry approval fails, the approval remains in a state of **Pending**.</span></span>
- <span data-ttu-id="7d658-119">תוקן: שגיאות SQL באישורים בכמות גדולה (מבוי סתום/‏‫זמן קצוב‬).</span><span class="sxs-lookup"><span data-stu-id="7d658-119">Fixed: SQL Errors on bulk approvals (deadlock/timeout).</span></span>
- <span data-ttu-id="7d658-120">תוקן: בעיות ביצועים משמעותיות בחוויית המשתמש שנגרמו כתוצאה מעדכון חברי הצוות תוך אישור ערכי זמן.</span><span class="sxs-lookup"><span data-stu-id="7d658-120">Fixed: Significant performance issues in the user experience caused by updating team members while approving time entries.</span></span>

<span data-ttu-id="7d658-121">**ניהול פרויקט**</span><span class="sxs-lookup"><span data-stu-id="7d658-121">**Project Management**</span></span>

- <span data-ttu-id="7d658-122">תוקן: התראה של אזור זמן הועברה מהתצוגה **יישוב‬** לטופס הראשי **פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="7d658-122">Fixed: Time zone notification moved from the **Reconciliation** view to the **Project** main form.</span></span>
- <span data-ttu-id="7d658-123">תוקן: תבנית לוח השנה אינה מוגדרת כברירת מחדל כשנפתח טופס פרויקט חדש.</span><span class="sxs-lookup"><span data-stu-id="7d658-123">Fixed: Calendar template is not correctly defaulting when a new project form opens.</span></span>
- <span data-ttu-id="7d658-124">תוקן: בדפדפנים מבוססי כרום, המשתמשים אינם יכולים לבחור בקלות משימות קודמות למחיקה.</span><span class="sxs-lookup"><span data-stu-id="7d658-124">Fixed: For chromium-based browsers, users are unable to easily select predecessor tasks to delete.</span></span>
- <span data-ttu-id="7d658-125">תוקן: יצירה או העתקה של **פרויקט מתבנית ריקה** מביאות משימות שאינן קשורות.</span><span class="sxs-lookup"><span data-stu-id="7d658-125">Fixed: Creating or copying **Project from Empty template** fetches unrelated assignments.</span></span>
- <span data-ttu-id="7d658-126">תוקן: במקרי קצה ספציפיים, יצירת משימה חדשה מרשת המשימות מביאה ליצירת רשומות כפולות.</span><span class="sxs-lookup"><span data-stu-id="7d658-126">Fixed: In specific edge cases, creating a new assignment from the task grid results in duplicate records being created.</span></span>
- <span data-ttu-id="7d658-127">תוקן: במצב ידני, המשתמשים אינם יכולים לעדכן את תאריכי התחלת המשימות שיהיו לאחר התאריך הנוכחי שנשמר.</span><span class="sxs-lookup"><span data-stu-id="7d658-127">Fixed: In manual mode, users are unable to update task start dates to be later than the current date saved.</span></span>

<span data-ttu-id="7d658-128">**ניהול משאבים**</span><span class="sxs-lookup"><span data-stu-id="7d658-128">**Resource Management**</span></span>

- <span data-ttu-id="7d658-129">תוקן: שורת סכום ביניים בתצוגה **יישוב** חישבה באופן שגוי את השונות בין הזמנות לאחר הארכת ההזמנות.</span><span class="sxs-lookup"><span data-stu-id="7d658-129">Fixed: **Reconciliation** view subtotal row incorrectly calculates bookings variance after extending bookings.</span></span>
- <span data-ttu-id="7d658-130">תוקן: התצוגה **יישוב** מציגה באופן שגוי משימות משאבים כאשר למשאב הניתן להזמנה יש לוח שנה שאינו תואם ליומן הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="7d658-130">Fixed: **Reconciliation** view incorrectly displays resource assignments when the bookable resource has a calendar that does not match the project calendar.</span></span>

<span data-ttu-id="7d658-131">**Sales**</span><span class="sxs-lookup"><span data-stu-id="7d658-131">**Sales**</span></span>

- <span data-ttu-id="7d658-132">תוקן: כאשר ערכי הזמנים מאושרים מחדש (**אשר> בטל>** אשר שוב), נוצרת כפילות של פריט שאינו ניתן לחיוב בפועל.</span><span class="sxs-lookup"><span data-stu-id="7d658-132">Fixed: When time entries are re-approved (**Approve > Cancel >** approve again), a duplicate non-chargeable actual is created.</span></span>
