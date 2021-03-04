---
title: מה חדש או שונה במהדורה 17.5, Hotfix, V3 של Project Service Automation
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 17.5, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 03/13/2020
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
ms.openlocfilehash: cd4142176258820f4718f457ca8610f19f584a32
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5143717"
---
# <a name="project-service-automation-update-release-175-v3"></a><span data-ttu-id="beddc-103">מהדורה 17.5, V3 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="beddc-103">Project Service Automation Update Release 17.5, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="beddc-104">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="beddc-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="beddc-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="beddc-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="beddc-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="beddc-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="beddc-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="beddc-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="beddc-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="beddc-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="beddc-109">נושא זה מפרט את התכונות החדשות והתיקונים ב-V3, מהדורה 17.5.</span><span class="sxs-lookup"><span data-stu-id="beddc-109">This topic lists the features and fixes that are new or changed for V3, Update Release 17.5.</span></span> <span data-ttu-id="beddc-110">מספר גירסת build של גירסה זו הוא V3.10.7.32 ובדרך כלל היא זמינה באמצעות עדכון עצמי החל ממרץ 2020.</span><span class="sxs-lookup"><span data-stu-id="beddc-110">This version has a build number of V3.10.7.32 and is generally available through a self-update in March 2020.</span></span>


## <a name="update-release-175"></a><span data-ttu-id="beddc-111">הפצת עדכון 17.5</span><span class="sxs-lookup"><span data-stu-id="beddc-111">Update Release 17.5</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="beddc-112">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="beddc-112">Bug fixes</span></span>


<span data-ttu-id="beddc-113">**ניהול פרויקט**</span><span class="sxs-lookup"><span data-stu-id="beddc-113">**Project Management**</span></span>

- <span data-ttu-id="beddc-114">תוקן: טופלו בעיות בסנכרון בצד השרת שמתרחשות במשימות בעלות משך ארוך.</span><span class="sxs-lookup"><span data-stu-id="beddc-114">Fixed: Addressed server-side synchronization issues that occur with long duration tasks.</span></span>
- <span data-ttu-id="beddc-115">תוקן: טופלו תבניות עבודה של 24 שעות שהוסיפו באופן שגוי יום נוסף למשימות.</span><span class="sxs-lookup"><span data-stu-id="beddc-115">Fixed: Addressed 24-hour work hour templates inaccurately adding an additional day to tasks.</span></span>
- <span data-ttu-id="beddc-116">תוקן: טופלו תבניות עבודה +13 GMT שהזיזו משימות יום אחד קדימה באופן שגוי.</span><span class="sxs-lookup"><span data-stu-id="beddc-116">Fixed: Addressed +13 GMT work hour templates inaccurately shifting tasks one day ahead.</span></span>

