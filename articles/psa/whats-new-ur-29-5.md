---
title: מה חדש או שונה במהדורה Project Service Automation Update Release 29.5 Hotfix, V3
description: נושא זה מפרט את התכונות והתיקונים שזמינים במהדורה 29.5, עדכון Hotfix V3 של Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 03/26/2021
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
ms.openlocfilehash: d5050945c4ab7c1da61b07ec08bed20f32e166b9
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999177"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-295-v3"></a><span data-ttu-id="051ae-103">מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 29.5 V3</span><span class="sxs-lookup"><span data-stu-id="051ae-103">What's new or changed in Project Service Automation Update Release 29.5, V3</span></span>

<span data-ttu-id="051ae-104">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="051ae-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="051ae-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="051ae-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="051ae-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="051ae-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="051ae-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="051ae-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="051ae-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution.md).</span><span class="sxs-lookup"><span data-stu-id="051ae-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution.md).</span></span>

<span data-ttu-id="051ae-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 29.5, עדכון V3 של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="051ae-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 29.5.</span></span> <span data-ttu-id="051ae-110">מספר ה-build של גירסה זו הוא V3.10.47.150 והיא זמינה דרך עדכון עצמי החל מינואר 2021.</span><span class="sxs-lookup"><span data-stu-id="051ae-110">This version has a build number of V3.10.47.150 and is generally available through a self-update in January 2021.</span></span>

## <a name="update-release-295"></a><span data-ttu-id="051ae-111">הפצת עדכון 29.5</span><span class="sxs-lookup"><span data-stu-id="051ae-111">Update Release 29.5</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="051ae-112">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="051ae-112">Bug fixes</span></span>


<span data-ttu-id="051ae-113">**מכירות**</span><span class="sxs-lookup"><span data-stu-id="051ae-113">**Sales**</span></span>

<span data-ttu-id="051ae-114">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="051ae-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="051ae-115">חריגה אפשרית עם הפניה ל- null מתרחשת ב- **ContractLineMapHelper.UpdateContractLineDetailPriceListReference** בעת סגירת הצעת מחיר כזכייה, ואין מחירון להצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="051ae-115">A possible null reference exception occurs in **ContractLineMapHelper.UpdateContractLineDetailPriceListReference** when you close a quote as won and the quote has no price list.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
