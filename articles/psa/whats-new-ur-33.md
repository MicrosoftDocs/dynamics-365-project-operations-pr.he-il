---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 33 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 33, עדכון V3 של Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/30/2021
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
ms.openlocfilehash: 2c96e4abd484bb66285421baaad82ead9589bbe9
ms.sourcegitcommit: be5beba71ee9770c0083b4fe5cc89e7ec6b741b8
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334545"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-33-v3"></a><span data-ttu-id="fff6f-103">מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 33 V3</span><span class="sxs-lookup"><span data-stu-id="fff6f-103">What's new or changed in Project Service Automation Update Release 33, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="fff6f-104">אנו שמחים להכריז על העדכון האחרון עבור האפליקציה Microsoft Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="fff6f-104">We're pleased to announce the latest update for the Microsoft Dynamics 365 Project Service Automation app.</span></span> <span data-ttu-id="fff6f-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="fff6f-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="fff6f-106">הוא תואם ל- Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="fff6f-106">It's compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="fff6f-107">לעדכון למהדורה זו, בקר בדף הפתרונות המקוון של מרכז הניהול עבור Dynamics 365 והתקן את העדכון.</span><span class="sxs-lookup"><span data-stu-id="fff6f-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page, and install the update.</span></span> <span data-ttu-id="fff6f-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="fff6f-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="fff6f-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 33, עדכון V3 של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="fff6f-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 33.</span></span> <span data-ttu-id="fff6f-110">גרסה זו כוללת מספר build של V3.10.54.98 והיא זמינה בדרך כלל באמצעות עדכון עצמי ביולי 2021.</span><span class="sxs-lookup"><span data-stu-id="fff6f-110">This version has a build number of V3.10.54.98 and is generally available through a self-update in July 2021.</span></span>

## <a name="update-release-33"></a><span data-ttu-id="fff6f-111">הפצת עדכון 33</span><span class="sxs-lookup"><span data-stu-id="fff6f-111">Update Release 33</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="fff6f-112">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="fff6f-112">Bug fixes</span></span>

<span data-ttu-id="fff6f-113">**זמן והוצאה**</span><span class="sxs-lookup"><span data-stu-id="fff6f-113">**Time and Expense**</span></span>

<span data-ttu-id="fff6f-114">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="fff6f-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="fff6f-115">שני שדות נעולים, **msdyn_description** ו- **msdyn_externaldescription** ניתנים לעריכה לאחר השליחה.</span><span class="sxs-lookup"><span data-stu-id="fff6f-115">Two locked fields, **msdyn_description** and **msdyn_externaldescription** are editable after submission.</span></span>
- <span data-ttu-id="fff6f-116">הודעת שגיאה מופיעה אם נוצרת הוצאה שאינה קשורה לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="fff6f-116">An error message occurs if an expense is created that isn't related to a project.</span></span>
- <span data-ttu-id="fff6f-117">כאשר נוצר ערך זמן, ברירת המחדל של תפקיד המשאב היא תפקיד לא פעיל.</span><span class="sxs-lookup"><span data-stu-id="fff6f-117">When a time entry is created, the resource role defaults to an inactive role.</span></span>
- <span data-ttu-id="fff6f-118">שורות יומן המשויכות להוצאה שנזכרה ונמחקה אינן נמחקות.</span><span class="sxs-lookup"><span data-stu-id="fff6f-118">Journal lines associated with a recalled and deleted expense aren't deleted.</span></span>
- <span data-ttu-id="fff6f-119">באפשרות **טופס יצירה מהיר של ערך זמן**, עדכן את התצוגה **רשימת משימות פרוייקט** כדי לשנות את התאריך המוצג כברירת מחדל לתאריך ההתחלה של המשימה.</span><span class="sxs-lookup"><span data-stu-id="fff6f-119">On the **Time entry Quick Create Form**, update the **Project Task List** view to change the date displayed by default to the start date of the task.</span></span>
- <span data-ttu-id="fff6f-120">כאשר אתה יוצר ערך זמן מהכרטיסיה **קשור** של המשאב שניתן להזמין, ערך הזמן נוצר באופן שגוי עבור המשתמש המחובר במקום המשאב הניתן להזמנה.</span><span class="sxs-lookup"><span data-stu-id="fff6f-120">When you create a time entry from the **Related** tab of the bookable resource, the time entry is incorrectly created for the signed-in user instead of the parent bookable resource.</span></span>
- <span data-ttu-id="fff6f-121">שדות חדשים מתווספים לתיבת הדו-שיח **אישור בכמויות גדולות MDD**.</span><span class="sxs-lookup"><span data-stu-id="fff6f-121">New fields are added to the **Bulk approval MDD** dialog box.</span></span>

<span data-ttu-id="fff6f-122">**תכנון פרוייקטים**</span><span class="sxs-lookup"><span data-stu-id="fff6f-122">**Project planning**</span></span>

<span data-ttu-id="fff6f-123">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="fff6f-123">The following issues have been fixed:</span></span>
- <span data-ttu-id="fff6f-124">ביצועים איטיים של יצירת פרויקטים כאשר משתמשים בתבניות לשעת העבודה של הפרויקט עם לוחות שנה מורכבים.</span><span class="sxs-lookup"><span data-stu-id="fff6f-124">Slow project creation performance when project work hour templates are applied with complex calendars.</span></span>
- <span data-ttu-id="fff6f-125">כאשר תאריך ההתחלה מאוחר יותר מתאריך הסיום, מופיעה שגיאה בעותק של תבנית הפרויקט בגלל הבדלים ברכיב הזמן של כל שדה.</span><span class="sxs-lookup"><span data-stu-id="fff6f-125">When the start date is greater than the end date, an error displays on the copy project template because of differences in the time component of each field.</span></span>

<span data-ttu-id="fff6f-126">**ניהול משאבים**</span><span class="sxs-lookup"><span data-stu-id="fff6f-126">**Resource management**</span></span>

<span data-ttu-id="fff6f-127">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="fff6f-127">The following issues have been fixed:</span></span>
- <span data-ttu-id="fff6f-128">נעשה שימוש בפרמטר שגוי בשאילתת ניצול המשאבים וה- XML גורם לתוצאות סינון שגויות ברשת **ניצול משאבים**.</span><span class="sxs-lookup"><span data-stu-id="fff6f-128">An incorrect parameter is used in the resource utilization query and the XML leads to incorrect filter results on the **Resource Utilization** grid.</span></span>
- <span data-ttu-id="fff6f-129">האישור **הרחב את ההזמנות** מציג תאריך סיום שגוי להזמנות.</span><span class="sxs-lookup"><span data-stu-id="fff6f-129">The **Extend Bookings** confirmation displays incorrect end date for bookings.</span></span>

<span data-ttu-id="fff6f-130">**מכירות**</span><span class="sxs-lookup"><span data-stu-id="fff6f-130">**Sales**</span></span>

<span data-ttu-id="fff6f-131">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="fff6f-131">The following issues have been fixed:</span></span>
- <span data-ttu-id="fff6f-132">הודעת שגיאה מופיעה אם נוצר מחיר קטגוריה עם ערכים חסרים.</span><span class="sxs-lookup"><span data-stu-id="fff6f-132">An error message occurs if a category price is created with missing values.</span></span>
- <span data-ttu-id="fff6f-133">הודעת שגיאה מופיעה אם נוצר אבן דרך של סעיף חוזה ללא שורת הזמנה.</span><span class="sxs-lookup"><span data-stu-id="fff6f-133">An error message occurs if a contract line milestone is created without an order line.</span></span>
