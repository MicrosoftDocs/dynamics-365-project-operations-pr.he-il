---
title: שדרוג דף הבית
description: נושא זה מראה היכן למצוא מידע חשוב על התכונות החדשות והתכונות שהשתנו ב- Dynamics 365 Project Service Automation, והתהליך לשדרוג לגירסה החדשה ביותר.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 05/30/2019
ms.topic: article
author: rumant
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 29e7b519b61e8709c025e9906d04aed0156f65eb
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077389"
---
# <a name="upgrade-home-page"></a><span data-ttu-id="a4f44-103">שדרוג דף הבית</span><span class="sxs-lookup"><span data-stu-id="a4f44-103">Upgrade home page</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

## <a name="upgrade-from-psa-version-2x-or-1x-to-version-3x"></a><span data-ttu-id="a4f44-104">שדרג מגירסה ‎2.x או ‎1.x של PSA לגירסה ‎3.x</span><span class="sxs-lookup"><span data-stu-id="a4f44-104">Upgrade from PSA version 2.x or 1.x to version 3.x</span></span>

### <a name="new-instances"></a><span data-ttu-id="a4f44-105">מופעים חדשים</span><span class="sxs-lookup"><span data-stu-id="a4f44-105">New instances</span></span>

<span data-ttu-id="a4f44-106">החל מ- 17 במאי 2019, בעת בחירת Project Service Automation במהלך הקצאת מופע חדש, גירסה ‎3.x מותקנת כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="a4f44-106">As of May 17, 2019, when Project Service Automation is selected during the provisioning of a new instance, version 3.x is installed by default.</span></span>

### <a name="existing-instances"></a><span data-ttu-id="a4f44-107">מופעים קיימים</span><span class="sxs-lookup"><span data-stu-id="a4f44-107">Existing instances</span></span>

<span data-ttu-id="a4f44-108">בעבר, לקוחות בעלי PSA גרסה ‎2.x שהיו צריכים לשדרג לגרסה ‎3.x, שהיא גרסת הממשק המאוחד מבוסס-לקוח (UCI) של PSA, היו חייבים לפנות לתמיכה של Microsoft ולספק את פרטי המופע שלהם כדי שהתמיכה תוכל לאפשר שידרוג לגרסה ‎3.x.</span><span class="sxs-lookup"><span data-stu-id="a4f44-108">Previously, customers who have an instance of PSA version 2.x and needed to upgrade to version 3.x, which is the Unified client interface-based (UCI) version of PSA , had to contact Microsoft Support and provide the details of thier instance so that support could enable the instance for upgrade to version 3.x.</span></span> <span data-ttu-id="a4f44-109">החל מה-1 במרץ, 2020, לקוחות שלהם גרסה 2.x של PSA וצריכים לשדרג לגרסה 3.x, יוכלו לשדרג את המופעים שלהם ישירות מפורטל הניהול ללא צורך ביצירת קשר עם התמיכה של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a4f44-109">As of March 1st, 2020, customers who have an instance of PSA version 2.x and need to upgrade to version 3.x, will able to upgrade their instances directly from the Admin portal without having to contact Microsoft Support.</span></span>  

> [!NOTE]
> <span data-ttu-id="a4f44-110">גירסה ‎3.x של PSA כוללת שינויים משמעותיים.</span><span class="sxs-lookup"><span data-stu-id="a4f44-110">PSA version 3.x includes significant changes.</span></span> <span data-ttu-id="a4f44-111">היא נבנתה על בסיס מסגרת הממשק מאוחד כדי לעזור ולספק חוויית משתמש משופרת.</span><span class="sxs-lookup"><span data-stu-id="a4f44-111">It has been built on the Unified Interface framework to help provide an improved user experience.</span></span> <span data-ttu-id="a4f44-112">האפליקציה המחודשת מספקת ממשק משתמש (UI) אחיד ועקבי, והיא פועלת לפי עקרונות העיצוב המגיב לתצוגה מיטבית בכל גודל מסך או מכשיר.</span><span class="sxs-lookup"><span data-stu-id="a4f44-112">The redesigned app delivers a consistent, uniform user interface (UI), and it follows responsive design principles for optimal viewing on any screen size or device.</span></span> <span data-ttu-id="a4f44-113">כמו כן, נעשו שינויים אחרים ברחבי האפליקציה.</span><span class="sxs-lookup"><span data-stu-id="a4f44-113">There have been other changes throughout the application.</span></span> <span data-ttu-id="a4f44-114">חלק מהאזורים שהשתנו כוללים את אזורי התמחור, ההזמנות והקצאת המשאבים, הזמן, ההוצאות והאישורים.</span><span class="sxs-lookup"><span data-stu-id="a4f44-114">Some of the areas that have been changed include pricing, booking and assigning resources, time, expenses, and approvals.</span></span>

<span data-ttu-id="a4f44-115">לפני שתתחיל בתהליך השדרוג, מומלץ להשלים את המשימות הבאות:</span><span class="sxs-lookup"><span data-stu-id="a4f44-115">Before you begin the upgrade process, we recommend that you complete the following tasks:</span></span>

- <span data-ttu-id="a4f44-116">בדוק אם Dynamics 365 Field Service ו- Project Service Automation מותקנים שניהם במופע המזוהה.</span><span class="sxs-lookup"><span data-stu-id="a4f44-116">Verify whether both Dynamics 365 Field Service and Project Service Automation are installed on the identified instance.</span></span> <span data-ttu-id="a4f44-117">אם שני הפתרונות מותקנים, עליך לתכנן לשדרג את שניהם לפני שתחדש את השימוש הרגיל במופע.</span><span class="sxs-lookup"><span data-stu-id="a4f44-117">If both solutions are installed, you should plan to upgrade both before you resume regular use of the instance.</span></span>
- <span data-ttu-id="a4f44-118">עיין היטב בנושאים הבאים.</span><span class="sxs-lookup"><span data-stu-id="a4f44-118">Carefully review the following topics.</span></span> <span data-ttu-id="a4f44-119">מודעות לשינויים בין הגירסאות והבנה שלהם יעזרו לך בתהליך השדרוג.</span><span class="sxs-lookup"><span data-stu-id="a4f44-119">Awareness and understanding of the changes between versions will help you with the upgrade process.</span></span> <span data-ttu-id="a4f44-120">נושאים אלה מספקים מידע על השינויים העיקריים ב- PSA, יחד עם שיקולים והמלצות לתכנון השדרוג לגירסה ‎3.x.</span><span class="sxs-lookup"><span data-stu-id="a4f44-120">These topics provide information about the major changes in PSA, together with considerations and recommendations for planning your upgrade to version 3.x.</span></span>

    - [<span data-ttu-id="a4f44-121">מה חדש או השתנה בגירסה 3 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="a4f44-121">What's new or changed in Project Service Automation version 3</span></span>](whats-new-changed-v3.md)
    - [<span data-ttu-id="a4f44-122">שיקולים לשדרוג – גירסה ‎2.x או ‎1.x של Project Service Automation לגירסה ‎3.x</span><span class="sxs-lookup"><span data-stu-id="a4f44-122">Upgrade considerations - Project Service Automation version 2.x or 1.x to version 3</span></span>](upgrade-v3.md)

- <span data-ttu-id="a4f44-123">שדרג את מופע ארגז החול (Sandbox) כדי להעריך את השינויים בהטמעה לפני שתשדרג את מופע הייצור.</span><span class="sxs-lookup"><span data-stu-id="a4f44-123">Upgrade your sandbox instance to evaluate the changes in your implementation before you upgrade your production instance.</span></span>

<span data-ttu-id="a4f44-124">לאחר שעיינת בנושאים שהוזכרו קודם לכן ואתה מוכן לשדרג לגירסה ‎3.x של PSA או לגירסה המבוססת על UCI, שלח בקשה לתמיכה של Microsoft כדי להפוך את השדרוג לזמין ממרכז הניהול.</span><span class="sxs-lookup"><span data-stu-id="a4f44-124">After you've reviewed the topics that were mentioned earlier and are ready to upgrade to PSA version 3.x or the UCI-based version, submit a request to Microsoft support to make the upgrade available from Admin center.</span></span> <span data-ttu-id="a4f44-125">במסגרת הבקשה, ספק את פרטי המופע שלך.</span><span class="sxs-lookup"><span data-stu-id="a4f44-125">In your request, provide the details of your instance.</span></span>

## <a name="older-versions-of-psa-psa-version-2x-in-a-newly-created-instance"></a><span data-ttu-id="a4f44-126">גירסאות קודמות של PSA ‏(PSA גירסה ‎2.x) במופע חדש שנוצר</span><span class="sxs-lookup"><span data-stu-id="a4f44-126">Older versions of PSA (PSA version 2.x) in a newly created instance</span></span>

<span data-ttu-id="a4f44-127">החל מ- 17 במאי 2019, כל המופעים החדשים יכללו את UCI בתור לקוח ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="a4f44-127">As of May 17, 2019, all new instances will have UCI as the default client.</span></span> <span data-ttu-id="a4f44-128">כדי להיערך לשינוי זה, גירסה ‎3.x של PSA וגירסה ‎8.x של Field Service יהיו מוקצות כברירת מחדל, משום שגירסאות אלה מיועדות לעבוד עם לקוח UCI.</span><span class="sxs-lookup"><span data-stu-id="a4f44-128">For alignment with this change, PSA version 3.x and Field Service version 8.x will be provisioned by default, because these versions are designed to work with the UCI client.</span></span>

<span data-ttu-id="a4f44-129">החל מה-1 במרץ 2020, לקוחות Dynamics PSA לא יוכלו עוד ליצור סביבות חדשות עם גרסאות ישנות יותר של PSA, למשל PSA גרסה 2.x ומטה.</span><span class="sxs-lookup"><span data-stu-id="a4f44-129">Starting March 1st 2020, customers of Dynamics PSA will no longer be able to create a new environments with older versions of PSA, for example PSA version 2.x or lower.</span></span> <span data-ttu-id="a4f44-130">כל סביבה חדשה תדרוש גרסה 3.x של PSA.</span><span class="sxs-lookup"><span data-stu-id="a4f44-130">Any new environment will be to get only version 3.x of PSA.</span></span>

> [!NOTE]
> <span data-ttu-id="a4f44-131">לקבלת החוויה הטובה ביותר בעת השימוש בגירסאות ישנות יותר של האפליקציות Field Service ו- PSA, עבור אל **הגדרות המערכת** ובשדה **‏‫השתמש בממשק המאוחד החדש בלבד (מומלץ)** , בחר **לא** הואיל וגירסאות אלה אינן מיועדות להיטען כראוי ב- UCI.</span><span class="sxs-lookup"><span data-stu-id="a4f44-131">For the best experience when you use older versions of the Field Service and PSA applications, go to the **System settings** page and for the field, **Use the new Unified Interface only (recommended)** field, select **No** as these versions aren't designed to be correctly loaded in UCI.</span></span> <span data-ttu-id="a4f44-132">לאחר הביטול של UCI, תוכל לפתוח ולהפעיל גירסאות אלה של Field Service ו- PSA באמצעות לקוח האינטרנט הישן.</span><span class="sxs-lookup"><span data-stu-id="a4f44-132">After you have turned off UCI, you can open and run these versions of Field Service and PSA by using the old web client.</span></span> 
