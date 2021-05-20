---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 25 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 25, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 10/26/2020
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
ms.openlocfilehash: 3aa10e1d4b23fbe6c2743d71497bdef840776008
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948872"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-25-v3"></a><span data-ttu-id="f2cdc-103">מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 25 V3</span><span class="sxs-lookup"><span data-stu-id="f2cdc-103">What's new or changed in Project Service Automation Update Release 25, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="f2cdc-104">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="f2cdc-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="f2cdc-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="f2cdc-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="f2cdc-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="f2cdc-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="f2cdc-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="f2cdc-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="f2cdc-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="f2cdc-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="f2cdc-109">נושא זה מפרט את התכונות והתיקונים שהם חדשים או ששונו עבור Project Service Automation V3, מהדורת עדכון 25. לגרסה זו יש מספר Build ‏ V 3.10.43.76 והיא זמינה לכלל ציבור המשתמשים באמצעות עדכון עצמי באוקטובר 2020.</span><span class="sxs-lookup"><span data-stu-id="f2cdc-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 25 This version has a build number of V 3.10.43.76 and is generally available through a self-update in October 2020.</span></span>

## <a name="update-release-25"></a><span data-ttu-id="f2cdc-110">הפצת עדכון 25</span><span class="sxs-lookup"><span data-stu-id="f2cdc-110">Update Release 25</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="f2cdc-111">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="f2cdc-111">Bug fixes</span></span>

<span data-ttu-id="f2cdc-112">**זמן והוצאה**</span><span class="sxs-lookup"><span data-stu-id="f2cdc-112">**Time and Expense**</span></span>

<span data-ttu-id="f2cdc-113">הבעיה הבאה תוקנה:</span><span class="sxs-lookup"><span data-stu-id="f2cdc-113">The following issue has been fixed:</span></span>

- <span data-ttu-id="f2cdc-114">תרשים ערכי זמן המציג נתונים נוספים בהתבסס על מרווח גדול מדי של אחזור.</span><span class="sxs-lookup"><span data-stu-id="f2cdc-114">Time entry chart showing additional data based on too large of an interval being retrieved.</span></span>

<span data-ttu-id="f2cdc-115">**ניהול משאבים**</span><span class="sxs-lookup"><span data-stu-id="f2cdc-115">**Resource Management**</span></span>

<span data-ttu-id="f2cdc-116">הבעיה הבאה תוקנה:</span><span class="sxs-lookup"><span data-stu-id="f2cdc-116">The following issue has been fixed:</span></span>

- <span data-ttu-id="f2cdc-117">נוסף קוד Package Deployer כדי לדלג על יצוא התיקון Universal Resource Scheduling אם כבר קיים תיקון בגרסה גבוהה יותר.</span><span class="sxs-lookup"><span data-stu-id="f2cdc-117">Added package deployer code to skip the Universal Resource Scheduling patch import if a higher version patch already exists.</span></span>

<span data-ttu-id="f2cdc-118">**ניהול פרויקט**</span><span class="sxs-lookup"><span data-stu-id="f2cdc-118">**Project Management**</span></span>

<span data-ttu-id="f2cdc-119">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="f2cdc-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="f2cdc-120">תוקנו פערים בעיגול ובשער החליפין שגרמו לעלות מתוכננת שגויה ברשת המעקב אחר הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="f2cdc-120">Corrected rounding and exchange rate discrepancies resulting in incorrect planned cost in the project tracking grid.</span></span>
- <span data-ttu-id="f2cdc-121">תומך ביכולת להציג שני רשתות תגובה או יותר בטופס **פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="f2cdc-121">Support the ability to display two or more react grids on the **Project** form.</span></span>
- <span data-ttu-id="f2cdc-122">ניתן אימות לטיפול ביכולת להקצות משימה מעבר לתאריך הסיום של היומן, מה שמביא להקצאת משאבים כושלת.</span><span class="sxs-lookup"><span data-stu-id="f2cdc-122">Provided validation to address the ability to assign a task past the calendar end date, which results in a failed resource assignment.</span></span>
- <span data-ttu-id="f2cdc-123">טיפול משופר בשגיאות לטיפול בחריגת הפניות Null שנוצרות מהבאים:</span><span class="sxs-lookup"><span data-stu-id="f2cdc-123">Improved error handling to address Null Reference Exception generated from the following:</span></span>

    - <span data-ttu-id="f2cdc-124">תוסף **PreValidateProjectTeamMemberCreate**</span><span class="sxs-lookup"><span data-stu-id="f2cdc-124">**PreValidateProjectTeamMemberCreate** plug-in</span></span>
    - <span data-ttu-id="f2cdc-125">**PreValidateProjectTaskCreate** כאשר נוצרת משימת פרויקט ללא פרויקט משויך</span><span class="sxs-lookup"><span data-stu-id="f2cdc-125">**PreValidateProjectTaskCreate** when a project task is created without an associated project</span></span>
    - <span data-ttu-id="f2cdc-126">תוסף **PreProjectTeamMemberCreate**</span><span class="sxs-lookup"><span data-stu-id="f2cdc-126">**PreProjectTeamMemberCreate** plug-in</span></span>
    - <span data-ttu-id="f2cdc-127">תוסף **PostProjectTeamMemberCreate**</span><span class="sxs-lookup"><span data-stu-id="f2cdc-127">**PostProjectTeamMemberDelete** plug-in</span></span>
    - <span data-ttu-id="f2cdc-128">תוסף **PreValidateProjectTaskDelete**</span><span class="sxs-lookup"><span data-stu-id="f2cdc-128">**PreValidateProjectTaskDelete** plug-in</span></span>

<span data-ttu-id="f2cdc-129">**Sales**</span><span class="sxs-lookup"><span data-stu-id="f2cdc-129">**Sales**</span></span>

<span data-ttu-id="f2cdc-130">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="f2cdc-130">The following issues have been fixed:</span></span>

- <span data-ttu-id="f2cdc-131">טיפול משופר בשגיאות כדי לטפל בחריגות הפניה Null שנוצרות מ **העתקת פרויקט: ניהול הערכות HelperResource**.</span><span class="sxs-lookup"><span data-stu-id="f2cdc-131">Improved error handling to address Null Reference Exceptions generated from **Copy Project: Estimates HelperResource Management**.</span></span>
- <span data-ttu-id="f2cdc-132">**לא מוכן להפקת חשבונית** ב **מצבור פרטי עבודה של חיוב זמן ומומרים** אינו מנקה את מצב החיוב.</span><span class="sxs-lookup"><span data-stu-id="f2cdc-132">**Not ready to Invoice** on a **Time and Material Billing Backlog** doesn't clear the billing status.</span></span>
- <span data-ttu-id="f2cdc-133">תוקן שגיאה בתויות לחצני ה **מחירים** בכרטיסיה **מחיר תפקיד** ו **פריטי קטלוג**.</span><span class="sxs-lookup"><span data-stu-id="f2cdc-133">Corrected mislabeled **Prices** buttons on the **Role Price** and **Catalog Items** tab.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]