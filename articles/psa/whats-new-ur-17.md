---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 17 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 17, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 03/06/2020
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
ms.openlocfilehash: bb93208217972639f91b39b7b6705d9897373ef7
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126799"
---
# <a name="project-service-automation-update-release-17-v3"></a><span data-ttu-id="abcb5-103">מהדורה 17, V3 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="abcb5-103">Project Service Automation Update Release 17, V3</span></span>

<span data-ttu-id="abcb5-104">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="abcb5-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="abcb5-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="abcb5-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="abcb5-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="abcb5-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="abcb5-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="abcb5-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="abcb5-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="abcb5-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="abcb5-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 17, עדכון V3 של PSA.</span><span class="sxs-lookup"><span data-stu-id="abcb5-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 17.</span></span> <span data-ttu-id="abcb5-110">מספר גירסת build של גרסה זו הוא V3.10.6.34 ובדרך כלל היא זמינה באמצעות עדכון עצמי החל ממרץ 2020.</span><span class="sxs-lookup"><span data-stu-id="abcb5-110">This version has a build number of V3.10.6.34 and is generally available through a self-update in March 2020.</span></span>


## <a name="update-release-17"></a><span data-ttu-id="abcb5-111">הפצת עדכון 17</span><span class="sxs-lookup"><span data-stu-id="abcb5-111">Update Release 17</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="abcb5-112">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="abcb5-112">Bug fixes</span></span>

<span data-ttu-id="abcb5-113">**כללי**</span><span class="sxs-lookup"><span data-stu-id="abcb5-113">**General**</span></span>

- <span data-ttu-id="abcb5-114">תוקן: עדכן את Project Service Automation כדי לאכוף רישיונות של חברי צוות (Project Resource Hub יכלול מטא-נתונים 3.x על תוכנית השירות של חברי הצוות).</span><span class="sxs-lookup"><span data-stu-id="abcb5-114">Fixed: Update Project Service Automation to enforce Team Member licenses (Project Resource Hub will include Team Member Service plan metadata 3.x)</span></span>
 
<span data-ttu-id="abcb5-115">**זמן והוצאה**</span><span class="sxs-lookup"><span data-stu-id="abcb5-115">**Time and Expense**</span></span>

- <span data-ttu-id="abcb5-116">תוקן: לא ניתן לשנות הערכת הוצאה ממחיר שאינו אפס לאפס (0).</span><span class="sxs-lookup"><span data-stu-id="abcb5-116">Fixed: It is not possible to change an expense estimate from a non-zero price to zero (0).</span></span> <span data-ttu-id="abcb5-117">ניסיון לשינוי לא יבוצע.</span><span class="sxs-lookup"><span data-stu-id="abcb5-117">The change is ignored.</span></span>

<span data-ttu-id="abcb5-118">**ניהול פרויקט**</span><span class="sxs-lookup"><span data-stu-id="abcb5-118">**Project Management**</span></span>

- <span data-ttu-id="abcb5-119">תוקן: נוספה בדיקת ערכי null לשם המשרה של חבר הצוות.</span><span class="sxs-lookup"><span data-stu-id="abcb5-119">Fixed: A check for null values has been added on a team member's position name.</span></span>
- <span data-ttu-id="abcb5-120">תוקן: נמחק שדה **msdyn_userresid** בישות **‎msdyn_resourceassignment**.</span><span class="sxs-lookup"><span data-stu-id="abcb5-120">Fixed: **msdyn_userresourceid** field on the **msdyn_resourceassignment** entity has been deprecated.</span></span>
- <span data-ttu-id="abcb5-121">תוקן: שדרוג מ- 2.x ל- 3.x כעת מטפל בפעולות מתאר ריקות בהקצאת משימות.</span><span class="sxs-lookup"><span data-stu-id="abcb5-121">Fixed: Upgrade from 2.x to 3.x now handles empty effort contours on task assignments.</span></span>

<span data-ttu-id="abcb5-122">**Sales**</span><span class="sxs-lookup"><span data-stu-id="abcb5-122">**Sales**</span></span>

- <span data-ttu-id="abcb5-123">תוקן: **Invoice.PreValidateInvoiceUpdate** כעת מטפל כראוי בתרחיש של הקצאת בעלי תיעוד מחדש.</span><span class="sxs-lookup"><span data-stu-id="abcb5-123">Fixed: **Invoice.PreValidateInvoiceUpdate** now handles the scenario of reassigning record owners properly.</span></span>
- <span data-ttu-id="abcb5-124">תוקן: כאשר מחלקת העסקה היא **זמן**, **UnitGroup** אינו ניתן לעריכה לכל הישויות כולל, **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail**, ו **ContractLineDetails**.</span><span class="sxs-lookup"><span data-stu-id="abcb5-124">Fixed: When the transaction class is **Time**, **UnitGroup** is non-editable for all entities including, **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail**, and **ContractLineDetails**.</span></span> <span data-ttu-id="abcb5-125">למרות זאת, **Unit** אינו ניתן לעריכה רק עבור **JournalLine** ו **InvoiceLineDetails**.</span><span class="sxs-lookup"><span data-stu-id="abcb5-125">However, **Unit** is non-editable only for **JournalLine** and **InvoiceLineDetails**.</span></span>


