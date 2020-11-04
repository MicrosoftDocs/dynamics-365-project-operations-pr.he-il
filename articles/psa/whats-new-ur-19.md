---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 19 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 19, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 05/05/2020
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
ms.openlocfilehash: ecc923cccfad21985025ab9d8006aaff16afc25f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077261"
---
# <a name="project-service-automation-update-release-19-v3"></a><span data-ttu-id="db0c0-103">מהדורה 19, V3 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="db0c0-103">Project Service Automation Update Release 19, V3</span></span>

<span data-ttu-id="db0c0-104">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="db0c0-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="db0c0-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="db0c0-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="db0c0-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="db0c0-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="db0c0-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="db0c0-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="db0c0-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="db0c0-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="db0c0-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 19, עדכון V3 של PSA.</span><span class="sxs-lookup"><span data-stu-id="db0c0-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 19.</span></span> <span data-ttu-id="db0c0-110">גירסה זו כוללת מספר build של V3.10.30.41 ובדרך כלל היא זמינה דרך עדכון עצמי במאי 2020.</span><span class="sxs-lookup"><span data-stu-id="db0c0-110">This version has a build number of V3.10.30.41 and is generally available through a self-update in May 2020.</span></span>

## <a name="update-release-19"></a><span data-ttu-id="db0c0-111">הפצת עדכון 19</span><span class="sxs-lookup"><span data-stu-id="db0c0-111">Update Release 19</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="db0c0-112">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="db0c0-112">Bug fixes</span></span>

<span data-ttu-id="db0c0-113">**זמן והוצאה**</span><span class="sxs-lookup"><span data-stu-id="db0c0-113">**Time and Expense**</span></span>

<span data-ttu-id="db0c0-114">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="db0c0-114">The following issues have been fixed:</span></span> 

- <span data-ttu-id="db0c0-115">שגיאות שנגזרות מייבוא של ערכי זמן שלא הוצגו כראוי.</span><span class="sxs-lookup"><span data-stu-id="db0c0-115">Errors derived from time entry imports are not surfaced correctly.</span></span>
- <span data-ttu-id="db0c0-116">רשת הזנת זמן אינה תומכת בהתנהגות שדה **תאריך בלבד**.</span><span class="sxs-lookup"><span data-stu-id="db0c0-116">Time Entry Grid does not support **Date Only** field behavior.</span></span>
- <span data-ttu-id="db0c0-117">משאבי פרויקט אינם יכולים ליצור הוצאה בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="db0c0-117">Project Resources are unable to create an expense with a project.</span></span>

<span data-ttu-id="db0c0-118">**ניהול פרויקט**</span><span class="sxs-lookup"><span data-stu-id="db0c0-118">**Project Management**</span></span>

<span data-ttu-id="db0c0-119">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="db0c0-119">The following issues have been fixed:</span></span> 

-  <span data-ttu-id="db0c0-120">משימת נכד גורמת לאומדן מאמץ שגוי במהלך חישוב ההשלמה (EAC).</span><span class="sxs-lookup"><span data-stu-id="db0c0-120">Grandchild task causes an incorrect effort estimate during the Completion (EAC) Calculation.</span></span>

<span data-ttu-id="db0c0-121">**Sales**</span><span class="sxs-lookup"><span data-stu-id="db0c0-121">**Sales**</span></span>

<span data-ttu-id="db0c0-122">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="db0c0-122">The following issues have been fixed:</span></span> 

- <span data-ttu-id="db0c0-123">הפעולה **חישוב מחדש** לא עובדת עם פרטי סעיף חוזה הוצאות או פרטי שורה בהצעות מחיר.</span><span class="sxs-lookup"><span data-stu-id="db0c0-123">The **Recalculate** action does not work with expense contract line details or quote line details.</span></span>
- <span data-ttu-id="db0c0-124">**עדכן מחירים** חסר לאומדני הוצאות.</span><span class="sxs-lookup"><span data-stu-id="db0c0-124">**Update Prices** is missing for expense estimates.</span></span>
-  <span data-ttu-id="db0c0-125">לקוחות אינם יכולים לבחור סיבות מותאמות אישית למצב חוזה מהדף **חוזה של פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="db0c0-125">Customers are unable to select custom contract status reasons from the **Project Contract** page.</span></span>
- <span data-ttu-id="db0c0-126">לקוחות חווים ביצועים פחות טובים בעת יצירת מחירון מותאם אישית מהצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="db0c0-126">Customers experience degraded performance when creating a custom price list from a quote.</span></span>
- <span data-ttu-id="db0c0-127">לקוחות חווים חוסר עקביות עם ברירת מחדל של **יחידה** בדפים **פרטי סעיף בהצעת מחיר** ו- **פרטי סעיף בחוזה**.</span><span class="sxs-lookup"><span data-stu-id="db0c0-127">Customers experience inconsistency with **unit** defaults on **Quote Line Details** and **Contract Line Details** pages.</span></span>
- <span data-ttu-id="db0c0-128">הוספת פריטים בקטגוריית עסקאות שלא ניתן לחייב לסעיף חוזה הניתן לחיוב לא תכבד את סוג החיוב **ללא חיוב** של קטגוריית העסקה.</span><span class="sxs-lookup"><span data-stu-id="db0c0-128">Adding non-chargeable transaction category items to a chargeable contract line will not respect the **Non-chargeable** billing type of the transaction category.</span></span>
- <span data-ttu-id="db0c0-129">לקוחות אינם יכולים להשתמש בתפקידים ובקטגוריה בחוזים שנוצרו בעבר.</span><span class="sxs-lookup"><span data-stu-id="db0c0-129">Customers can't use the newly added roles and category on previously created contracts.</span></span>
- <span data-ttu-id="db0c0-130">לקוחות חווים ביצועים גרועים ואחזור מיותר ב- PreValidateProjectTeamMemberUpdate.cs</span><span class="sxs-lookup"><span data-stu-id="db0c0-130">Customers experience degraded performance Unnecessary retrieve in PreValidateProjectTeamMemberUpdate.cs</span></span>
- <span data-ttu-id="db0c0-131">יש להוסיף תפקידים שהוגדרו ככאלו שאינם חייבים בתשלום ברשימה **קטגוריות משאבים** לכרטיסיה **תפקידים שניתנים לחיוב** כ- **לא לחיוב** בסעיף החוזה של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="db0c0-131">Roles set up as non-chargeable in the **Resource Categories** list should be added to the **Chargeable Roles** tab as **Non0chargeable** on the contract line for a project.</span></span>
- <span data-ttu-id="db0c0-132">לקוחות עשויים לחוות ביצועים גרועים בעת יצירת פרויקט מכיוון ש- **GetBookableResourceIdFromUser** מאחזר את כל העמודות של משאבים שניתנים להזמנה במקום רק את המזהה הראשי.</span><span class="sxs-lookup"><span data-stu-id="db0c0-132">Customers may experience degraded performance when creating a project because **GetBookableResourceIdFromUser** retrieves all columns of bookable resources instead of just the primary ID.</span></span>
- <span data-ttu-id="db0c0-133">בישות **TransactionType** חסר יישום plug-in לעדכון אימות מראש כדי למנוע ממשתמשים להזין **יחידות** ו- **UnitGroups** שאינן חוקיות לסוגי הטרנזקציות.</span><span class="sxs-lookup"><span data-stu-id="db0c0-133">**TransactionType** entity missing the pre-validation update plug-in to prevent users from entering **Units** and **UnitGroups** that are not valid for transaction types.</span></span>
- <span data-ttu-id="db0c0-134">השלב **הסר** אינו פועל לייבוא ערך זמן.</span><span class="sxs-lookup"><span data-stu-id="db0c0-134">The **Remove** step does not work for time entry import.</span></span>
