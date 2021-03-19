---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 24 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 24, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 10/02/2020
ms.topic: article
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: c789a65f1996d082410b3d8dd9e76e5065e708a2
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280489"
---
# <a name="project-service-automation-update-release-24-v3"></a><span data-ttu-id="f7d08-103">מהדורה 24, V3 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="f7d08-103">Project Service Automation Update Release 24, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="f7d08-104">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="f7d08-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="f7d08-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="f7d08-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="f7d08-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="f7d08-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="f7d08-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="f7d08-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="f7d08-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="f7d08-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="f7d08-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 24, עדכון V3 של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f7d08-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 24.</span></span> <span data-ttu-id="f7d08-110">מספר ה- Build של גירסה זו הוא V 3.10.42.43 והיא זמינה דרך עדכון עצמי החל מאוקטובר 2020.</span><span class="sxs-lookup"><span data-stu-id="f7d08-110">This version has a build number of V 3.10.42.43 and is generally available through a self-update in October 2020.</span></span>

## <a name="update-release-24"></a><span data-ttu-id="f7d08-111">הפצת עדכון 24</span><span class="sxs-lookup"><span data-stu-id="f7d08-111">Update Release 24</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="f7d08-112">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="f7d08-112">Bug fixes</span></span>

<span data-ttu-id="f7d08-113">**Sales**</span><span class="sxs-lookup"><span data-stu-id="f7d08-113">**Sales**</span></span>

<span data-ttu-id="f7d08-114">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="f7d08-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="f7d08-115">בעיה בעת הגדרת מחירון ברירת המחדל של מוצרים.</span><span class="sxs-lookup"><span data-stu-id="f7d08-115">Problem while setting default price list of products.</span></span>
- <span data-ttu-id="f7d08-116">הביצועים של זכייה בהצעת מחיר הם איטיים בגלל מחירון מוטבע ועותק של רשומות מחיר-תפקיד‬.</span><span class="sxs-lookup"><span data-stu-id="f7d08-116">Performance of Quote win is slow due to the embedded price list and role price records copy.</span></span>
- <span data-ttu-id="f7d08-117">**חוזה פרויקט/מרכז המכירות** > **פריט שורת מוצרים/כמות שורות הזמנה** מעוגל אוטומטית למספר השלם הקרוב ביותר.</span><span class="sxs-lookup"><span data-stu-id="f7d08-117">**Project Contract/Sales Hub** > **Product Line Item/Order Line Quantity** is automatically rounded to the nearest integer.</span></span>
- <span data-ttu-id="f7d08-118">הרם להרשאות מערכת בעת קריאת מחירונים.</span><span class="sxs-lookup"><span data-stu-id="f7d08-118">Elevate to system privileges when reading price lists.</span></span>
- <span data-ttu-id="f7d08-119">העתק את שדות כתובת הלקוח **address1_freighttermscode** ו- **address1_shippingmethodcode** להצעת מחיר/הזמנה.</span><span class="sxs-lookup"><span data-stu-id="f7d08-119">Copy customer address fields **address1_freighttermscode** and **address1_shippingmethodcode** to Quote/Order.</span></span> 


<span data-ttu-id="f7d08-120">**זמן והוצאה**</span><span class="sxs-lookup"><span data-stu-id="f7d08-120">**Time and Expense**</span></span>

<span data-ttu-id="f7d08-121">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="f7d08-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="f7d08-122">**רשת ערכי הזמן** לא תומכת בהתנהגות זמן של **תאריך בלבד** .</span><span class="sxs-lookup"><span data-stu-id="f7d08-122">The **Time Entry Grid** doesn't support **Date Only** time behavior.</span></span>
- <span data-ttu-id="f7d08-123">**ערך זמן** אינו מתרענן אוטומטית.</span><span class="sxs-lookup"><span data-stu-id="f7d08-123">**Time Entry** is not refreshing automatically.</span></span> <span data-ttu-id="f7d08-124">נדרש רענון ידני.</span><span class="sxs-lookup"><span data-stu-id="f7d08-124">A manual refresh is required.</span></span>
- <span data-ttu-id="f7d08-125">לא ניתן לייבא את רשומות ערכי הזמן ממשימה כשיש הפסקה (0 שעות) בהקצאות המשאב.</span><span class="sxs-lookup"><span data-stu-id="f7d08-125">Unable to import the time entries from an assignment when there is a break (0 hours) in a resource's assignments.</span></span>
- <span data-ttu-id="f7d08-126">בעת יצירת ערך זמן, הגדר את ההתחלה שתהיה דומה ל- **msdyn_date**.</span><span class="sxs-lookup"><span data-stu-id="f7d08-126">When creating a time entry, set the start to the same as **msdyn_date**.</span></span>
- <span data-ttu-id="f7d08-127">הפעל מחדש עריכה בכמות גדולה לערכי זמן.</span><span class="sxs-lookup"><span data-stu-id="f7d08-127">Re-enable bulk edit for time entry.</span></span>

<span data-ttu-id="f7d08-128">**ניהול משאבים**</span><span class="sxs-lookup"><span data-stu-id="f7d08-128">**Resource Management**</span></span>

<span data-ttu-id="f7d08-129">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="f7d08-129">The following issues have been fixed:</span></span>

- <span data-ttu-id="f7d08-130">ניסיון לעדכן את סטטוס ההזמנה בין הימים ללא דרישה יגרום לחריגה של ref-null.</span><span class="sxs-lookup"><span data-stu-id="f7d08-130">Trying to update the status of an inter-day booking without a requirement will throw a null-ref exception.</span></span>
- <span data-ttu-id="f7d08-131">שגיאה בטעינת **תצוגת יישוב**.</span><span class="sxs-lookup"><span data-stu-id="f7d08-131">Error loading the **Reconciliation View**.</span></span>


<span data-ttu-id="f7d08-132">**ניהול פרויקט**</span><span class="sxs-lookup"><span data-stu-id="f7d08-132">**Project Management**</span></span>

<span data-ttu-id="f7d08-133">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="f7d08-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="f7d08-134">ב **לוח הזמנים של הפרויקט**, בעת שינוי מ **ידני** ל **אוטומטי**, שמירה אוטומטית לא מסתיימת.</span><span class="sxs-lookup"><span data-stu-id="f7d08-134">In the **Project Schedule**, when changing from **Manual** to **Auto**, auto save is not completing.</span></span>
- <span data-ttu-id="f7d08-135">עלויות ההוצאות לא צריכות לחשב את השונות ב **רשת מעקב אחר פרויקטים**.</span><span class="sxs-lookup"><span data-stu-id="f7d08-135">Expense costs should not calculate toward variance on the **Project Tracking Grid**.</span></span>
- <span data-ttu-id="f7d08-136">התנהגות לא עקבית של עמודות **הערכת תג** במהלך עומס לעומת שינוי בסוג **יחידות זמן עבודה**.</span><span class="sxs-lookup"><span data-stu-id="f7d08-136">Inconsistent behavior for **Estimates tag** columns during load versus changing the **Time-Phase** type.</span></span>
- <span data-ttu-id="f7d08-137">העלות בפועל בפרויקט עשויה שלא לשקף את הסכומים הכוללים **נתונים בפועל**.</span><span class="sxs-lookup"><span data-stu-id="f7d08-137">The actual cost on a project may not reflect the totals from **Actuals**.</span></span>
- <span data-ttu-id="f7d08-138">**תאריך סיום משוער** בכרטיסיה **סיכום** אינו תואם את **לוח הזמנים של WBS**.</span><span class="sxs-lookup"><span data-stu-id="f7d08-138">**Estimated Finish Date** on the **Summary** tab does not match the **WBS Schedule**.</span></span>
- <span data-ttu-id="f7d08-139">**עדכן שעות בפועל** ב-outdent לא עובד כראוי.</span><span class="sxs-lookup"><span data-stu-id="f7d08-139">**Update Actual Hours** on outdent does not work correctly.</span></span>
- <span data-ttu-id="f7d08-140">מנהל פרויקט מחוץ ל- **BU** הבסיסי לא יכול ליצור פרויקט.</span><span class="sxs-lookup"><span data-stu-id="f7d08-140">A Project manager outside of root **BU** can't create a project.</span></span>
- <span data-ttu-id="f7d08-141">שינויים במשימה או בקטגוריה של **אומדני הוצאות** אינם נשמרים.</span><span class="sxs-lookup"><span data-stu-id="f7d08-141">Changes to task or category on **Expense Estimates** are not persisted.</span></span>
- <span data-ttu-id="f7d08-142">**העתק החוזה** מעתיק את לוחות הזמנים של החשבונית ואת סטטוס הריצה.</span><span class="sxs-lookup"><span data-stu-id="f7d08-142">**Copy of contract** copies the invoice schedules and the run status.</span></span>
- <span data-ttu-id="f7d08-143">הלחצן **רענן את הנתונים בפועל** מחשב באופן שגוי משימות סיכום.</span><span class="sxs-lookup"><span data-stu-id="f7d08-143">**Refresh Actuals** button incorrectly calculates summary tasks.</span></span>
- <span data-ttu-id="f7d08-144">תוספת של Microsoft Project: תקן שגיאת התייחסות null אם לחבר צוות כלשהו יש יחידת משאבים ריקה.</span><span class="sxs-lookup"><span data-stu-id="f7d08-144">Microsoft Project Add-in: Fix null reference error if any team member has an empty resourcing unit.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]