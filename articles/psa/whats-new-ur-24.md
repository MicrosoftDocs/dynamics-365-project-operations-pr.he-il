---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 24 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 24, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 6c8348e65307f63a251f97bf1ea17578e7026da8
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077260"
---
# <a name="project-service-automation-update-release-24-v3"></a><span data-ttu-id="82285-103">מהדורה 24, V3 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="82285-103">Project Service Automation Update Release 24, V3</span></span>

<span data-ttu-id="82285-104">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="82285-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="82285-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="82285-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="82285-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="82285-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="82285-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="82285-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="82285-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="82285-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="82285-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 24, עדכון V3 של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="82285-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 24.</span></span> <span data-ttu-id="82285-110">מספר ה- Build של גירסה זו הוא V 3.10.42.43 והיא זמינה דרך עדכון עצמי החל מאוקטובר 2020.</span><span class="sxs-lookup"><span data-stu-id="82285-110">This version has a build number of V 3.10.42.43 and is generally available through a self-update in October 2020.</span></span>

## <a name="update-release-24"></a><span data-ttu-id="82285-111">הפצת עדכון 24</span><span class="sxs-lookup"><span data-stu-id="82285-111">Update Release 24</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="82285-112">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="82285-112">Bug fixes</span></span>

<span data-ttu-id="82285-113">**Sales**</span><span class="sxs-lookup"><span data-stu-id="82285-113">**Sales**</span></span>

<span data-ttu-id="82285-114">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="82285-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="82285-115">בעיה בעת הגדרת מחירון ברירת המחדל של מוצרים.</span><span class="sxs-lookup"><span data-stu-id="82285-115">Problem while setting default price list of products.</span></span>
- <span data-ttu-id="82285-116">הביצועים של זכייה בהצעת מחיר הם איטיים בגלל מחירון מוטבע ועותק של רשומות מחיר-תפקיד‬.</span><span class="sxs-lookup"><span data-stu-id="82285-116">Performance of Quote win is slow due to the embedded price list and role price records copy.</span></span>
- <span data-ttu-id="82285-117">**חוזה פרויקט/מרכז המכירות** > **פריט שורת מוצרים/כמות שורות הזמנה** מעוגל אוטומטית למספר השלם הקרוב ביותר.</span><span class="sxs-lookup"><span data-stu-id="82285-117">**Project Contract/Sales Hub** > **Product Line Item/Order Line Quantity** is automatically rounded to the nearest integer.</span></span>
- <span data-ttu-id="82285-118">הרם להרשאות מערכת בעת קריאת מחירונים.</span><span class="sxs-lookup"><span data-stu-id="82285-118">Elevate to system privileges when reading price lists.</span></span>
- <span data-ttu-id="82285-119">העתק את שדות כתובת הלקוח **address1_freighttermscode** ו- **address1_shippingmethodcode** להצעת מחיר/הזמנה.</span><span class="sxs-lookup"><span data-stu-id="82285-119">Copy customer address fields **address1_freighttermscode** and **address1_shippingmethodcode** to Quote/Order.</span></span> 


<span data-ttu-id="82285-120">**זמן והוצאה**</span><span class="sxs-lookup"><span data-stu-id="82285-120">**Time and Expense**</span></span>

<span data-ttu-id="82285-121">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="82285-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="82285-122">**רשת ערכי הזמן** לא תומכת בהתנהגות זמן של **תאריך בלבד** .</span><span class="sxs-lookup"><span data-stu-id="82285-122">The **Time Entry Grid** doesn't support **Date Only** time behavior.</span></span>
- <span data-ttu-id="82285-123">**ערך זמן** אינו מתרענן אוטומטית.</span><span class="sxs-lookup"><span data-stu-id="82285-123">**Time Entry** is not refreshing automatically.</span></span> <span data-ttu-id="82285-124">נדרש רענון ידני.</span><span class="sxs-lookup"><span data-stu-id="82285-124">A manual refresh is required.</span></span>
- <span data-ttu-id="82285-125">לא ניתן לייבא את רשומות ערכי הזמן ממשימה כשיש הפסקה (0 שעות) בהקצאות המשאב.</span><span class="sxs-lookup"><span data-stu-id="82285-125">Unable to import the time entries from an assignment when there is a break (0 hours) in a resource's assignments.</span></span>
- <span data-ttu-id="82285-126">בעת יצירת ערך זמן, הגדר את ההתחלה שתהיה דומה ל- **msdyn_date**.</span><span class="sxs-lookup"><span data-stu-id="82285-126">When creating a time entry, set the start to the same as **msdyn_date**.</span></span>
- <span data-ttu-id="82285-127">הפעל מחדש עריכה בכמות גדולה לערכי זמן.</span><span class="sxs-lookup"><span data-stu-id="82285-127">Re-enable bulk edit for time entry.</span></span>

<span data-ttu-id="82285-128">**ניהול משאבים**</span><span class="sxs-lookup"><span data-stu-id="82285-128">**Resource Management**</span></span>

<span data-ttu-id="82285-129">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="82285-129">The following issues have been fixed:</span></span>

- <span data-ttu-id="82285-130">ניסיון לעדכן את סטטוס ההזמנה בין הימים ללא דרישה יגרום לחריגה של ref-null.</span><span class="sxs-lookup"><span data-stu-id="82285-130">Trying to update the status of an inter-day booking without a requirement will throw a null-ref exception.</span></span>
- <span data-ttu-id="82285-131">שגיאה בטעינת **תצוגת יישוב**.</span><span class="sxs-lookup"><span data-stu-id="82285-131">Error loading the **Reconciliation View**.</span></span>


<span data-ttu-id="82285-132">**ניהול פרויקט**</span><span class="sxs-lookup"><span data-stu-id="82285-132">**Project Management**</span></span>

<span data-ttu-id="82285-133">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="82285-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="82285-134">ב **לוח הזמנים של הפרויקט** , בעת שינוי מ **ידני** ל **אוטומטי** , שמירה אוטומטית לא מסתיימת.</span><span class="sxs-lookup"><span data-stu-id="82285-134">In the **Project Schedule** , when changing from **Manual** to **Auto** , auto save is not completing.</span></span>
- <span data-ttu-id="82285-135">עלויות ההוצאות לא צריכות לחשב את השונות ב **רשת מעקב אחר פרויקטים**.</span><span class="sxs-lookup"><span data-stu-id="82285-135">Expense costs should not calculate toward variance on the **Project Tracking Grid**.</span></span>
- <span data-ttu-id="82285-136">התנהגות לא עקבית של עמודות **הערכת תג** במהלך עומס לעומת שינוי בסוג **יחידות זמן עבודה**.</span><span class="sxs-lookup"><span data-stu-id="82285-136">Inconsistent behavior for **Estimates tag** columns during load versus changing the **Time-Phase** type.</span></span>
- <span data-ttu-id="82285-137">העלות בפועל בפרויקט עשויה שלא לשקף את הסכומים הכוללים **נתונים בפועל**.</span><span class="sxs-lookup"><span data-stu-id="82285-137">The actual cost on a project may not reflect the totals from **Actuals**.</span></span>
- <span data-ttu-id="82285-138">**תאריך סיום משוער** בכרטיסיה **סיכום** אינו תואם את **לוח הזמנים של WBS**.</span><span class="sxs-lookup"><span data-stu-id="82285-138">**Estimated Finish Date** on the **Summary** tab does not match the **WBS Schedule**.</span></span>
- <span data-ttu-id="82285-139">**עדכן שעות בפועל** ב-outdent לא עובד כראוי.</span><span class="sxs-lookup"><span data-stu-id="82285-139">**Update Actual Hours** on outdent does not work correctly.</span></span>
- <span data-ttu-id="82285-140">מנהל פרויקט מחוץ ל- **BU** הבסיסי לא יכול ליצור פרויקט.</span><span class="sxs-lookup"><span data-stu-id="82285-140">A Project manager outside of root **BU** can't create a project.</span></span>
- <span data-ttu-id="82285-141">שינויים במשימה או בקטגוריה של **אומדני הוצאות** אינם נשמרים.</span><span class="sxs-lookup"><span data-stu-id="82285-141">Changes to task or category on **Expense Estimates** are not persisted.</span></span>
- <span data-ttu-id="82285-142">**העתק החוזה** מעתיק את לוחות הזמנים של החשבונית ואת סטטוס הריצה.</span><span class="sxs-lookup"><span data-stu-id="82285-142">**Copy of contract** copies the invoice schedules and the run status.</span></span>
- <span data-ttu-id="82285-143">הלחצן **רענן את הנתונים בפועל** מחשב באופן שגוי משימות סיכום.</span><span class="sxs-lookup"><span data-stu-id="82285-143">**Refresh Actuals** button incorrectly calculates summary tasks.</span></span>
- <span data-ttu-id="82285-144">תוספת של Microsoft Project: תקן שגיאת התייחסות null אם לחבר צוות כלשהו יש יחידת משאבים ריקה.</span><span class="sxs-lookup"><span data-stu-id="82285-144">Microsoft Project Add-in: Fix null reference error if any team member has an empty resourcing unit.</span></span>

