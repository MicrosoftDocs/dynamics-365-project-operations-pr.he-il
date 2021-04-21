---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 30 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 30, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 04/01/2021
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
ms.openlocfilehash: 1169ee13c42e982cb30a40d92df660f8933786a9
ms.sourcegitcommit: b4a05c7d5512d60abdb0d05bedd390e288e8adc9
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "5852857"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-30-v3"></a><span data-ttu-id="47a64-103">מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 30 V3</span><span class="sxs-lookup"><span data-stu-id="47a64-103">What's new or changed in Project Service Automation Update Release 30, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="47a64-104">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="47a64-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="47a64-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="47a64-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="47a64-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="47a64-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="47a64-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="47a64-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="47a64-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="47a64-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="47a64-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 30, עדכון V3 של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="47a64-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 30.</span></span> <span data-ttu-id="47a64-110">גירסה זו כוללת מספר build של V3.10.51.61 ובדרך כלל היא זמינה דרך עדכון עצמי באפריל 2021.</span><span class="sxs-lookup"><span data-stu-id="47a64-110">This version has a build number of V3.10.51.61 and is generally available through a self-update in April 2021.</span></span>

## <a name="update-release-30"></a><span data-ttu-id="47a64-111">הפצת עדכון 30</span><span class="sxs-lookup"><span data-stu-id="47a64-111">Update Release 30</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="47a64-112">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="47a64-112">Bug fixes</span></span>

<span data-ttu-id="47a64-113">**זמן והוצאה**</span><span class="sxs-lookup"><span data-stu-id="47a64-113">**Time and Expense**</span></span>

<span data-ttu-id="47a64-114">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="47a64-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="47a64-115">שגיאה מתרחשת כאשר אתה יוצר ושומר ערך זמן בדף **יצירה מהירה** אם השדה **תפקיד** מוסר.</span><span class="sxs-lookup"><span data-stu-id="47a64-115">An error occurs when you create and save a time entry on the **Quick Create** page if the **Role** field is removed.</span></span>
- <span data-ttu-id="47a64-116">מסנן ערכי הזמן מחיל את אופרטור המסנן השגוי.</span><span class="sxs-lookup"><span data-stu-id="47a64-116">The Time Entry filter applies the wrong filter operator.</span></span>
- <span data-ttu-id="47a64-117">גיליונות זמנים שהועתקו אינם מוצגים אוטומטית בעת בחירה באפשרות **העתק שבוע** בפקד הזנת הזמן.</span><span class="sxs-lookup"><span data-stu-id="47a64-117">Copied timesheets aren't automatically displayed when you select **Copy Week** on the time entry control.</span></span>

<span data-ttu-id="47a64-118">**ניהול משאבים**</span><span class="sxs-lookup"><span data-stu-id="47a64-118">**Resource Management**</span></span>

<span data-ttu-id="47a64-119">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="47a64-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="47a64-120">בעת הארכת הזמנה, מצב ההזמנה המוקצה להזמנה הבטוחה שגוי.</span><span class="sxs-lookup"><span data-stu-id="47a64-120">When you extend a booking, the booking status assigned to the hard booking is incorrect.</span></span> <span data-ttu-id="47a64-121">הארכת הזמנה מכבדת את מצב ההזמנה המוגדר בתור **מחויב‬** במטה-נתונים של הגדרת ההזמנה.</span><span class="sxs-lookup"><span data-stu-id="47a64-121">Extending a booking respects the booking status defined as **Committed** in the booking setup metadata.</span></span>
- <span data-ttu-id="47a64-122">כאשר לא מצוין מצב הזמנה תקף, הודעת השגיאה אינה מותאמת נכון לשפה המקומית.</span><span class="sxs-lookup"><span data-stu-id="47a64-122">When a valid booking status isn't specified, the error message is not correctly localized.</span></span>

<span data-ttu-id="47a64-123">**ניהול פרויקט**</span><span class="sxs-lookup"><span data-stu-id="47a64-123">**Project Management**</span></span>

<span data-ttu-id="47a64-124">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="47a64-124">The following issues have been fixed:</span></span>

- <span data-ttu-id="47a64-125">לא ניתן ליצור פרויקטים במטבע אחד ולכלול משימות קשורות במטבע אחר.</span><span class="sxs-lookup"><span data-stu-id="47a64-125">Projects can't be created in one currency and include related tasks in another currency.</span></span>

<span data-ttu-id="47a64-126">**מכירות**</span><span class="sxs-lookup"><span data-stu-id="47a64-126">**Sales**</span></span>

<span data-ttu-id="47a64-127">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="47a64-127">The following issues have been fixed:</span></span>

- <span data-ttu-id="47a64-128">בעת העתקת מחירון, המחירים אינם מעודכנים.</span><span class="sxs-lookup"><span data-stu-id="47a64-128">When a price list is copied, prices aren't updated.</span></span>
- <span data-ttu-id="47a64-129">סגירת הצעת מחיר כזכייה נכשלת כאשר לפרט העלות יש ערך עבור מקור.</span><span class="sxs-lookup"><span data-stu-id="47a64-129">Closing a quote as won fails when the cost detail has a value for origin.</span></span>
- <span data-ttu-id="47a64-130">בישות **משימת פרויקט**, השם **עלות מוערכת** משתנה לשם **עלות מתוכננת (בסיס)**.</span><span class="sxs-lookup"><span data-stu-id="47a64-130">On the **Project Task** entity, **Estimated Cost** has been renamed to **Planned Cost (Base)**.</span></span>
- <span data-ttu-id="47a64-131">חריגה עם הפניה ל- null נוצרת בעת יצירה או מחיקה של חשבוניות.</span><span class="sxs-lookup"><span data-stu-id="47a64-131">A null reference exception is generated when invoices are created or deleted.</span></span>
