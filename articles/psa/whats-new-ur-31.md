---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 31 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 31, עדכון V3 של Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/26/2021
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
ms.openlocfilehash: 160187ba7b96547e85a7a4ec4bf84c86d8fd8257
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999132"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-31-v3"></a><span data-ttu-id="6abdd-103">מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 31 V3</span><span class="sxs-lookup"><span data-stu-id="6abdd-103">What's new or changed in Project Service Automation Update Release 31, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="6abdd-104">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="6abdd-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="6abdd-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="6abdd-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="6abdd-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="6abdd-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="6abdd-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="6abdd-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="6abdd-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="6abdd-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="6abdd-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 31, עדכון V3 של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="6abdd-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 31.</span></span> <span data-ttu-id="6abdd-110">גירסה זו כוללת מספר build של V3.10.52.77 ובדרך כלל היא זמינה דרך עדכון עצמי במאי 2021.</span><span class="sxs-lookup"><span data-stu-id="6abdd-110">This version has a build number of V3.10.52.77 and is generally available through a self-update in May 2021.</span></span>

## <a name="update-release-31"></a><span data-ttu-id="6abdd-111">הפצת עדכון 31</span><span class="sxs-lookup"><span data-stu-id="6abdd-111">Update Release 31</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="6abdd-112">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="6abdd-112">Bug fixes</span></span>

<span data-ttu-id="6abdd-113">**זמן והוצאה**</span><span class="sxs-lookup"><span data-stu-id="6abdd-113">**Time and Expense**</span></span>

<span data-ttu-id="6abdd-114">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="6abdd-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="6abdd-115">לחצני פקודה לערכי זמן בדף **משאבים הניתנים להזמנה** היו מבלבלים.</span><span class="sxs-lookup"><span data-stu-id="6abdd-115">Time entry control command buttons on the **Bookable Resource** page were confusing.</span></span>
- <span data-ttu-id="6abdd-116">נוצר חריג הפניה null ב **Project.SetTrackingFields** באישור ערך זמן.</span><span class="sxs-lookup"><span data-stu-id="6abdd-116">A null reference exception was generated in **Project.SetTrackingFields** when approving a time entry.</span></span>

<span data-ttu-id="6abdd-117">**ניהול משאבים**</span><span class="sxs-lookup"><span data-stu-id="6abdd-117">**Resource Management**</span></span>

<span data-ttu-id="6abdd-118">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="6abdd-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="6abdd-119">**צור חבר צוות** אינו מציג כראוי את הגדרת המטא נתונים של הגדרת ההזמנה עבור **מצב ברירת המחדל 'מוקצה'**.</span><span class="sxs-lookup"><span data-stu-id="6abdd-119">**Create Team Member** doesn't correctly display the booking setup metadata setting for **Default Booking Committed Status**.</span></span>
- <span data-ttu-id="6abdd-120">בעת השדרוג מ- PSA 1.X ל- X‏.3, תהליך השדרוג נכשל ב-**UpgradeResourceRequirements**.</span><span class="sxs-lookup"><span data-stu-id="6abdd-120">When upgrading from PSA 1.X to 3.X, the upgrade process fails at **UpgradeResourceRequirements**.</span></span>


<span data-ttu-id="6abdd-121">**מכירות**</span><span class="sxs-lookup"><span data-stu-id="6abdd-121">**Sales**</span></span>

<span data-ttu-id="6abdd-122">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="6abdd-122">The following issues have been fixed:</span></span>

- <span data-ttu-id="6abdd-123">הכנסות בפועל ממירות את הסכומים למטבע הפרויקט ברשת המעקב.</span><span class="sxs-lookup"><span data-stu-id="6abdd-123">Actual revenue converts the amounts to the project currency in the tracking grid.</span></span>
- <span data-ttu-id="6abdd-124">ברירת המחדל של המטבע אינה ברורה בעת יצירת שורות יומן, שורות הצעות מחיר וסעיפי חוזה בתרחישים שבהם מטבע הבסיס של הארגון שונה ממטבע הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="6abdd-124">The currency default is unclear when creating journal lines, quote lines, and contract lines in scenarios where an organization's base currency differs from the project currency.</span></span>
- <span data-ttu-id="6abdd-125">**ממתין לאימות יומן התיקון** שאילתה אינה מסננת לפי פרויקט.</span><span class="sxs-lookup"><span data-stu-id="6abdd-125">**Pending correction journal validation** query doesn't filter by project.</span></span>
- <span data-ttu-id="6abdd-126">המכירות הנותרות מחושבות באופן שגוי בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="6abdd-126">Remaining sales are calculated incorrectly on a project.</span></span>
- <span data-ttu-id="6abdd-127">הצעות מחיר המבוססות על איש קשר נכשלות כאשר הן נוצרות ללא מחירון.</span><span class="sxs-lookup"><span data-stu-id="6abdd-127">Quotes based on a contact fail when they are created without a price list.</span></span>
- <span data-ttu-id="6abdd-128">לא מופיע מחוון התקדמות לעיבוד בעת הבחירה באפשרות **אשר חשבונית**.</span><span class="sxs-lookup"><span data-stu-id="6abdd-128">No processing spinner is shown when you select **Confirm Invoice**.</span></span>
- <span data-ttu-id="6abdd-129">לא מופיע מחוון התקדמות בעת הבחירה באפשרות **צור חשבונית**.</span><span class="sxs-lookup"><span data-stu-id="6abdd-129">No processing spinner is shown when you select **Create Invoice**.</span></span>
- <span data-ttu-id="6abdd-130">סגירת הצעת מחיר כאבודה אינה מבטלת את ההזמנות.</span><span class="sxs-lookup"><span data-stu-id="6abdd-130">Closing a quote as lost doesn't cancel the bookings.</span></span>







