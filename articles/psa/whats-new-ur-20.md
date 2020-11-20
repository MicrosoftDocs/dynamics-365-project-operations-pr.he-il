---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 20 V3
description: סעיף זה מפרט את התכונות החדשות והתיקונים במהדורה 20, עדכון V3 של Project Service Automation
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 06/12/2020
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
ms.openlocfilehash: ef24c20f3fa520b25a14773a15363a0f04f98d36
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126754"
---
# <a name="project-service-automation-update-release-20-v3"></a><span data-ttu-id="e85cf-103">מהדורה 20, V3 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="e85cf-103">Project Service Automation Update Release 20, V3</span></span>

<span data-ttu-id="e85cf-104">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="e85cf-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="e85cf-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="e85cf-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="e85cf-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="e85cf-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="e85cf-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="e85cf-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="e85cf-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="e85cf-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="e85cf-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 20, עדכון V3 של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="e85cf-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 20.</span></span> <span data-ttu-id="e85cf-110">גירסה זו כוללת מספר build של V3.10.31.37 ובדרך כלל היא זמינה דרך עדכון עצמי ביוני 2020.</span><span class="sxs-lookup"><span data-stu-id="e85cf-110">This version has a build number of V 3.10.31.37 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-20"></a><span data-ttu-id="e85cf-111">הפצת עדכון 20</span><span class="sxs-lookup"><span data-stu-id="e85cf-111">Update Release 20</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="e85cf-112">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="e85cf-112">Bug fixes</span></span>

<span data-ttu-id="e85cf-113">**ניהול פרויקט**</span><span class="sxs-lookup"><span data-stu-id="e85cf-113">**Project Management**</span></span>

<span data-ttu-id="e85cf-114">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="e85cf-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="e85cf-115">ייבוא חברי צוות הפרויקט בשיטת הקצאה הדורשת שעות גורם להודעת שגיאה לא ברורה כאשר השעות שצוינו הן אפס.</span><span class="sxs-lookup"><span data-stu-id="e85cf-115">Importing project team members with an allocation method that requires hours results in an unclear error message when the specified hours are zero.</span></span>
- <span data-ttu-id="e85cf-116">משתמשים מקבלים שגיאה לא נכונה כאשר מספר התווים המרבי הוזן לשדה **תיאור** של משימת פרויקט.</span><span class="sxs-lookup"><span data-stu-id="e85cf-116">Users receive an incorrect error when the maximum number of characters have been entered into the **Description** field for a project task.</span></span>
- <span data-ttu-id="e85cf-117">הדף **הורדת תוספת Microsoft Dynamics 365 Project Service Automation** מפנה לדף ההורדה באנגלית כאשר השפה של המשתמש מוגדרת ליפנית.</span><span class="sxs-lookup"><span data-stu-id="e85cf-117">The **Microsoft Dynamics 365 Project Service Automation add-in download** page redirects to the English download page when the user’s language settings are set to Japanese.</span></span>
- <span data-ttu-id="e85cf-118">כאשר מתרחשת שגיאת שרת, תווית הסנכרון בכרטיסיה **לוח זמנים** בטופס **פרויקטים** לפעמים נשארת.</span><span class="sxs-lookup"><span data-stu-id="e85cf-118">When a server error occurs, the synchronization label on the **Schedule** tab of the **Projects** form sometimes remains.</span></span>
- <span data-ttu-id="e85cf-119">עדכוני משימות מיותרים נשלחים לשרת עם שינוי המשימה.</span><span class="sxs-lookup"><span data-stu-id="e85cf-119">Redundant task updates are being sent to the server when a task is modified.</span></span>

<span data-ttu-id="e85cf-120">**Sales**</span><span class="sxs-lookup"><span data-stu-id="e85cf-120">**Sales**</span></span>

<span data-ttu-id="e85cf-121">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="e85cf-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="e85cf-122">בטופס **חוזה**, לחיצה כפולה על **צור חשבונית** יוצרת שתי חשבוניות עבור רשומה יחידה.</span><span class="sxs-lookup"><span data-stu-id="e85cf-122">On the **Contract** form, double-clicking **Create Invoice** creates two invoices for a single actuals record.</span></span>
- <span data-ttu-id="e85cf-123">ב- Internet Explorer 11, המשתמשים אינם יכולים ליצור ערכי הוצאות.</span><span class="sxs-lookup"><span data-stu-id="e85cf-123">In Internet Explorer 11, users are unable to create expense entries.</span></span>
- <span data-ttu-id="e85cf-124">ביטול עלות והיפוך של פעולות מכירה שלא חויבו אינן קשורות.</span><span class="sxs-lookup"><span data-stu-id="e85cf-124">Reversal of Cost and reversal of Unbilled Sales Actuals are not linked.</span></span>
- <span data-ttu-id="e85cf-125">הלחצן **רענן פעולות** בטופס **פרויקט** לא מרענן **שעות משימה בפועל**.</span><span class="sxs-lookup"><span data-stu-id="e85cf-125">The **Refresh Actuals** button on the **Project** form does not refresh **Task Actual Hours**.</span></span>
- <span data-ttu-id="e85cf-126">יישום plug-in **PreValidateProjectTeamMemberCreate** יכול ליצור משאבים כפולים שניתנים להזמנה כאשר התכונה **msdyn_isgenericresourceprojectscoped** מוגדרת **False**.</span><span class="sxs-lookup"><span data-stu-id="e85cf-126">The **PreValidateProjectTeamMemberCreate** plug-in can create duplicate generic bookable resources when the attribute **msdyn_isgenericresourceprojectscoped** is set to **False**.</span></span>
- <span data-ttu-id="e85cf-127">**חישוב מחדש** מנקה עלויות שניתנות לחיוב של פרטי שורה בהצעות מחיר ופרטי סעיף חוזה.</span><span class="sxs-lookup"><span data-stu-id="e85cf-127">**Recalculate** clears chargeable costs of product-based quote line details and contract line details.</span></span>
- <span data-ttu-id="e85cf-128">בתרחישים ספציפיים, יישום plug-in **PostEstimateLineUpdate** מציג שגיאת חריגה null.</span><span class="sxs-lookup"><span data-stu-id="e85cf-128">In specific scenarios, the **PostEstimateLineUpdate** plug-in displays a null teference exception error.</span></span>
- <span data-ttu-id="e85cf-129">משך שלב זמן ב- **תרשים ניתוח רווחיות** אינו תואם את המשך של עלויות בפרטי שורה בהצעת המחיר במחיר קבוע של הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="e85cf-129">Time phase duration on the **Profitability Analysis Chart** does not match duration of the costs in the fixed-price quote line detail of the quote.</span></span>
- <span data-ttu-id="e85cf-130">ערכי יחידות וקבוצת יחידות אינם חוזרים לברירת המחדל כראוי עבור קטגוריות הוצאות בטפסים **פרטי סעיף חוזה** ו- **פרטי סעיף בהצעת מחיר**.</span><span class="sxs-lookup"><span data-stu-id="e85cf-130">Unit and unit group values do not default correctly for expense categories on the **Contract Line Details** and **Quote Line Details** forms.</span></span>
- <span data-ttu-id="e85cf-131">רשימות **מחיר עלות יחידה ארגונית** מאפשרות חפיפה בתאריך.</span><span class="sxs-lookup"><span data-stu-id="e85cf-131">**Org Unit Cost Price** lists permit overlaps in the date effectivity.</span></span>
- <span data-ttu-id="e85cf-132">משתמשים אינם רשאים לשנות את **OrgUnit** כאשר סוג ההזמנה אינו מבוסס עבודה מכיוון שהוא יוביל לשגיאת חריגה null.</span><span class="sxs-lookup"><span data-stu-id="e85cf-132">Users are not permitted to change the **OrgUnit** when the order type is not work-based because it will lead to a null reference exception error.</span></span>
- <span data-ttu-id="e85cf-133">כאשר מנסים לנווט מהטופס **פרטי סעיף הצעת מחיר**, חזרה אל הכרטיסיה **הצעת מחיר**, הטופס מרענן ומציג את הכרטיסיה **סיכום**.</span><span class="sxs-lookup"><span data-stu-id="e85cf-133">When attempting to navigate from the **Quote Line Details** form, back to the **Quote** tab, the form refreshes and displays the **Summary** tab.</span></span>
