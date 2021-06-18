---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 16 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 16, עדכון V3 של Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/18/2020
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
ms.openlocfilehash: 5d4851ed27028117d25efb0610c25a5aac9c8b70
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006782"
---
# <a name="project-service-automation-update-release-16-v3"></a><span data-ttu-id="61f43-103">מהדורה 16, V3 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="61f43-103">Project Service Automation Update Release 16, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="61f43-104">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="61f43-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="61f43-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="61f43-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="61f43-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="61f43-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="61f43-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="61f43-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="61f43-108">למידע נוסף: [התקנה, עדכון של פתרון מועדף](/dynamics365/project-service/upgrade-psa-home-page).</span><span class="sxs-lookup"><span data-stu-id="61f43-108">For more information, see [Install, Update a Preferred Solution](/dynamics365/project-service/upgrade-psa-home-page).</span></span>
<span data-ttu-id="61f43-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 16, עדכון V3 של PSA.</span><span class="sxs-lookup"><span data-stu-id="61f43-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 16.</span></span> <span data-ttu-id="61f43-110">מספר ה-build של גירסה זו הוא V3.10.6.34 והיא זמינה דרך עדכון עצמי החל מינואר 2020.</span><span class="sxs-lookup"><span data-stu-id="61f43-110">This version has a build number of V3.10.6.34 and is generally available through a self-update in January 2020.</span></span>


## <a name="update-release-16"></a><span data-ttu-id="61f43-111">הפצת עדכון 16</span><span class="sxs-lookup"><span data-stu-id="61f43-111">Update Release 16</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="61f43-112">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="61f43-112">Bug fixes</span></span>

-   <span data-ttu-id="61f43-113">זמן והוצאה</span><span class="sxs-lookup"><span data-stu-id="61f43-113">Time and Expense</span></span>

    -   <span data-ttu-id="61f43-114">תוקן: משתמשים שמנסים להגיש לאישור פעולות זמן והוצאות שנמחקו יקבלו כעת הודעות שגיאה רלוונטיות.</span><span class="sxs-lookup"><span data-stu-id="61f43-114">Fixed: Users attempting to submit deleted time and expense entries for approvals will now receive relevant error messages.</span></span>

-   <span data-ttu-id="61f43-115">ניהול פרויקט</span><span class="sxs-lookup"><span data-stu-id="61f43-115">Project Management</span></span>

    -   <span data-ttu-id="61f43-116">תוקן: יחידות המשאבים שהוגדרו עבור חברי צוות בתבניות מוחלות על פרויקט חדש.</span><span class="sxs-lookup"><span data-stu-id="61f43-116">Fixed: The resourcing units defined for team members in templates are respected with the templates are applied to a new project.</span></span>

    -   <span data-ttu-id="61f43-117">תוקן: טיפול משופר בהקצאה מחודשת של בעלות על רשומות.</span><span class="sxs-lookup"><span data-stu-id="61f43-117">Fixed: Improved handling of the re-assignment of record ownership.</span></span>

    -   <span data-ttu-id="61f43-118">תוקן: פרויקטים שנמצאים בתהליך העתקה לא יורשו להעתיק עד שכל פעולות ההעתקה הושלמו.</span><span class="sxs-lookup"><span data-stu-id="61f43-118">Fixed: Projects that are in the process of being copied will not be permitted to copied until all copy operations are complete.</span></span>

-   <span data-ttu-id="61f43-119">ניהול משאבים</span><span class="sxs-lookup"><span data-stu-id="61f43-119">Resource Management</span></span>

    -   <span data-ttu-id="61f43-120">תוקן: "הרחב הזמנות" כעת מטפל נכון בתקופות קצרות וכבר לא יוצר אפס שעות להזמנות מורחבות.</span><span class="sxs-lookup"><span data-stu-id="61f43-120">Fixed: Extend bookings now handles short durations correctly and no longer creates zero hours for extended bookings.</span></span>

    -   <span data-ttu-id="61f43-121">תוקן: תצוגת ההתאמות משתנה כעת כאשר אזור הזמן של הפרויקט הוא שעון גריניץ' + 5.30 (GMT+5.30) והזמן של המשתמש שונה.</span><span class="sxs-lookup"><span data-stu-id="61f43-121">Fixed: The reconciliation view now renders when the project time zone is +5:30 GMT and the user’s time aone is different.</span></span>

-   <span data-ttu-id="61f43-122">Sales</span><span class="sxs-lookup"><span data-stu-id="61f43-122">Sales</span></span>

    -   <span data-ttu-id="61f43-123">תוקן: כאשר מסירים פרויקט המשויך לסעיף חוזה ומשייכים לסעיף פרויקט חדש, הפעולות בפרויקט החדש לא קיבלו הערכה מחודשת על סמך כללי החיוב והתמחור שהוגדרו בסעיף החוזה.</span><span class="sxs-lookup"><span data-stu-id="61f43-123">Fixed: When a project mapped to a contract line is removed and a new project is mapped, the actual records on the new project were not getting re-evaluated based on the billing and pricing rules defined on the contract line.</span></span> <span data-ttu-id="61f43-124">זה תוקן במהדורה זו.</span><span class="sxs-lookup"><span data-stu-id="61f43-124">This has been fixed in this release.</span></span> <span data-ttu-id="61f43-125">תמחור ורישומים של פעולות בפרויקט ששויך לאחרונה יתהפכו וייווצרו מחדש בצורה נכונה בהתבסס על כללי התמחור והחיוב של סעיף החוזה.</span><span class="sxs-lookup"><span data-stu-id="61f43-125">Pricing and actual records on the newly mapped project will get reversed and re-created correctly based on the pricing and billing rules of the contract line.</span></span> <span data-ttu-id="61f43-126">רישומי הפעולות של הפרויקט שלא שויך ייערכו גם הן מחדש וייווצרו מחדש כתוצאה מכך.</span><span class="sxs-lookup"><span data-stu-id="61f43-126">The actual records of the un-mapped project will also get re-evaluated and re-created as a consequence.</span></span>

    -   <span data-ttu-id="61f43-127">תוקן: אישור נוסף התווסף לשורת ההערכה בשדה **כמות** כדי להבטיח שערכי האפס לא יישארו.</span><span class="sxs-lookup"><span data-stu-id="61f43-127">Fixed: Additional validation has been added to an estimate line’s **Amount** field to ensure that null values are not persisted.</span></span>

    -   <span data-ttu-id="61f43-128">תוקן: כאשר עודכנו פעולות בפרויקט, נוסף כפתור רענון לטופס הראשי של הפרויקט כדי לאפשר למשתמשים לסנכרן מחדש את הפעולות.</span><span class="sxs-lookup"><span data-stu-id="61f43-128">Fixed: When actuals have been updated on a project, a refresh button has been added to the project main form to allow users to re-sync the actuals.</span></span>

    -   <span data-ttu-id="61f43-129">תוקן: כאשר משתמשים משדרגים מ- 2.X ל- 3.X, פרויקטים עם הערך NULL בתור שם הפרויקט יהיו מורשים.</span><span class="sxs-lookup"><span data-stu-id="61f43-129">Fixed: When users upgrade from 2.X to 3.X, projects with a NULL value for project name will be permitted.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]