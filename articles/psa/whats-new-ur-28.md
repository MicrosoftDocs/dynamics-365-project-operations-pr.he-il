---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 28 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 28, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/26/2021
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
ms.openlocfilehash: 079679302b2d8dac3074732b2392a7b811ac9711
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280219"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-28-v3"></a><span data-ttu-id="801ad-103">מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 28 V3</span><span class="sxs-lookup"><span data-stu-id="801ad-103">What's new or changed in Project Service Automation Update Release 28, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="801ad-104">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="801ad-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="801ad-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="801ad-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="801ad-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="801ad-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="801ad-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="801ad-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="801ad-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="801ad-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="801ad-109">נושא זה מפרט את התכונות והתיקונים שהם חדשים או ששונו עבור Project Service Automation V3, מהדורת עדכון 28. לגרסה זו יש מספר Build ‏ V 3.10.46.32 והיא זמינה לכלל ציבור המשתמשים באמצעות עדכון עצמי בינואר 2021.</span><span class="sxs-lookup"><span data-stu-id="801ad-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 28 This version has a build number of V3.10.46.32 and is generally available through a self-update in January 2021.</span></span>

## <a name="update-release-28"></a><span data-ttu-id="801ad-110">הפצת עדכון 28</span><span class="sxs-lookup"><span data-stu-id="801ad-110">Update Release 28</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="801ad-111">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="801ad-111">Bug fixes</span></span>

<span data-ttu-id="801ad-112">**זמן והוצאה**</span><span class="sxs-lookup"><span data-stu-id="801ad-112">**Time and Expense**</span></span>

<span data-ttu-id="801ad-113">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="801ad-113">The following issues have been fixed:</span></span>

- <span data-ttu-id="801ad-114">משתמשים יכולים להשתמש ב **עריכה בכמות גדולה** לעדכון רשומות זמן שאושרו והוגשו.</span><span class="sxs-lookup"><span data-stu-id="801ad-114">Users can use **Bulk Edit** to update time entries that have been approved and submitted.</span></span>

<span data-ttu-id="801ad-115">**ניהול פרויקט**</span><span class="sxs-lookup"><span data-stu-id="801ad-115">**Project Management**</span></span>

<span data-ttu-id="801ad-116">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="801ad-116">The following issues have been fixed:</span></span>

- <span data-ttu-id="801ad-117">במקרים שבהם ה-GUID של המשימה נקרא כמספר, לא ניתן לפתוח משימות לעריכה באמצעות **ערוך את המשימה** ברצועת הכלים בדף **מבנה התפלגות עבודה**.</span><span class="sxs-lookup"><span data-stu-id="801ad-117">In cases where the task GUID is interpreted as a number, tasks can't be opened for edit using **Edit Task** in the ribbon on the **Work Breakdown Structure** page.</span></span>

<span data-ttu-id="801ad-118">**Sales**</span><span class="sxs-lookup"><span data-stu-id="801ad-118">**Sales**</span></span>

<span data-ttu-id="801ad-119">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="801ad-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="801ad-120">חריג של התייחסות null נוצר כאשר יישום plug-in **GetEstimatesForProject** מופעל.</span><span class="sxs-lookup"><span data-stu-id="801ad-120">A null reference exception is generated when the **GetEstimatesForProject** plug-in is invoked.</span></span>
- <span data-ttu-id="801ad-121">**סמן מוכן לחשבונית** ברשת אבני הדרך מעדכנת חלקית בלבד את התכונות, למעט המאפיין **InvoiceStatus** שמתעדכן.</span><span class="sxs-lookup"><span data-stu-id="801ad-121">**Mark ready to invoice** on the milestone grid only partially updates attributes, except for the **InvoiceStatus** attribute, which is updated.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]