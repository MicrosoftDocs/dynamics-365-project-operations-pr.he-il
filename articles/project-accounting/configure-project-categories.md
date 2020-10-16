---
title: קביעת התצורה של קטגוריות פרוייקט
description: נושא זו מספק מידע על הגדרות קטגוריות פרויקט.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 84033182ce047d230724409eef9bc6afcaefd2b4
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/28/2020
ms.locfileid: "3895967"
---
# <a name="configure-project-categories"></a><span data-ttu-id="3de01-103">קביעת התצורה של קטגוריות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="3de01-103">Configure project categories</span></span>

<span data-ttu-id="3de01-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="3de01-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="3de01-105">Project Operations מציע יכולות חזקות לסיווג הכנסות והוצאות בפרויקטים.</span><span class="sxs-lookup"><span data-stu-id="3de01-105">Project Operations offers robust capabilities for categorizing revenue and expenses on projects.</span></span> <span data-ttu-id="3de01-106">קטגוריות מספקות את היכולת לדווח על ניתוח עסקאות הפרויקט, ולהעביר את הרשיום את הספר הראשי.</span><span class="sxs-lookup"><span data-stu-id="3de01-106">Categories provide the ability to report on and analyze project transactions, and drive posting to the general ledger.</span></span>

<span data-ttu-id="3de01-107">התרשים הבא ממחיש את המתאם בין קטגוריות של עסקאות, קטגוריות משותפות וקטגוריות של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="3de01-107">The following diagram illustrates the correlation between transaction categories, shared categories, and project categories.</span></span> 

<span data-ttu-id="3de01-108">קטגוריות של עסקאות הן הקיבוץ הבסיסי לעסקאות פרויקט.</span><span class="sxs-lookup"><span data-stu-id="3de01-108">Transaction categories are the basic grouping for project transactions.</span></span> <span data-ttu-id="3de01-109">בתוך אותה קיבוץ, יש קבוצה של קטגוריות משותפות שניתן לשתף בין יישומים ומודולים.</span><span class="sxs-lookup"><span data-stu-id="3de01-109">Within that grouping, there is a set of shared categories that can be shared across applications and modules.</span></span> <span data-ttu-id="3de01-110">כשיורדים עוד יותר לפרטים, קטגוריות של פרויקטים הן רמת הפירוט הגבוהה ביותר של הקטגורית.</span><span class="sxs-lookup"><span data-stu-id="3de01-110">Getting even further into specifics, project categories are the most granular level of categories.</span></span> <span data-ttu-id="3de01-111">קטגוריות של פרויקטים הן ספציפיות ליישות משפטית, למודול וליישום.</span><span class="sxs-lookup"><span data-stu-id="3de01-111">Project categories are specific to legal entity, module, and application.</span></span>

![מתאם בין קטגוריות של עסקאות, קטגוריות משותפות וקטגוריות של פרויקט](media/project-categories.png)

## <a name="transaction-categories"></a><span data-ttu-id="3de01-113">קטגוריות עסקה</span><span class="sxs-lookup"><span data-stu-id="3de01-113">Transaction categories</span></span>

<span data-ttu-id="3de01-114">קטגוריות של עסקאות מייצגות את הקיבוץ הבסיסי עבור עסקאות פרויקט ואינן ספציפיות לחברה או לסוג העסקה.</span><span class="sxs-lookup"><span data-stu-id="3de01-114">Transaction categories represent the basic grouping for project transactions and are not company or transaction type-specific.</span></span> <span data-ttu-id="3de01-115">לדוגמא, Contoso Robotics משתמש בקטגוריות תכנון, נסיעות, התקנה ועסקאות שירות כדי לקבץ עסקאות פרויקט.</span><span class="sxs-lookup"><span data-stu-id="3de01-115">For example, Contoso Robotics uses Design, Travel, Installation, and Service Transaction categories to group Project transactions.</span></span>

<span data-ttu-id="3de01-116">קטגוריות העסקאות מוגדרות במודול Project Operations.</span><span class="sxs-lookup"><span data-stu-id="3de01-116">Transaction categories are defined in the Project Operations module.</span></span> 
1. <span data-ttu-id="3de01-117">עבור אל **הגדרות** \> **קטגוריות של עסקאות** כדי לפתוח את הטופס.</span><span class="sxs-lookup"><span data-stu-id="3de01-117">Go to **Settings** \> **Transaction Categories** to open the form.</span></span> 
2. <span data-ttu-id="3de01-118">צור קטגוריית עסקאות חדשה על ידי בחירה באפשרות **חדש** או על ידי בחירה באפשרות **ייבא מאקסל**.</span><span class="sxs-lookup"><span data-stu-id="3de01-118">Create a new transaction category either by selecting **New** or by selecting **Import from Excel**.</span></span>

## <a name="shared-categories"></a><span data-ttu-id="3de01-119">קטגוריות משותפות</span><span class="sxs-lookup"><span data-stu-id="3de01-119">Shared categories</span></span>

<span data-ttu-id="3de01-120">Dynamics 365 משתמש במושג קטגוריות משותפות כדי לסווג הוצאות ביישומים שונים, כגון Dynamics 365 Finance, Dynamics 365 Supply Chain ו- Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="3de01-120">Dynamics 365 uses the Shared categories concept to categorize expenses in different applications, such as Dynamics 365 Finance, Dynamics 365 Supply Chain, and Dynamics 365 Project Operations.</span></span> <span data-ttu-id="3de01-121">עבור כל קטגוריית עסקאות שנוצרה, Project Operations יוצרת באופן אוטומטי ארבע קטגוריות משותפות קשורות: שעות, הוצאות, ,תשלומים ופריט.</span><span class="sxs-lookup"><span data-stu-id="3de01-121">For each Transaction category created, Project Operations automatically creates four related Shared categories: Hours, Expense, Fees, and Item.</span></span> <span data-ttu-id="3de01-122">תוכל לסקור ולהתאים את הקטגוריות המשותפות על ידי מעבר אל **ניהול פרויקטים וחשבונאות** \> **הגדרה** \> **קטגוריות** \> **קטגוריות משותפות**.</span><span class="sxs-lookup"><span data-stu-id="3de01-122">You can review and adjust the shared categories by going to **Project management and accounting** \> **Setup** \> **Categories** \> **Shared Categories**.</span></span>

## <a name="project-categories"></a><span data-ttu-id="3de01-123">קטגוריות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="3de01-123">Project categories</span></span>

<span data-ttu-id="3de01-124">קטגוריות הפרויקט מייצגות את הרמה המפורטת ביותר של תצורת הקטגוריות ויש להגדירן בנפרד ועבור כל חברה, על ידי רואה חשבון של הפרויקטים.</span><span class="sxs-lookup"><span data-stu-id="3de01-124">Project categories represent most granular level of category configuration and must be configured separately, and for each company, by a Project accountant.</span></span>

1. <span data-ttu-id="3de01-125">עבור אל **ניהול פרויקטים וחשבונאות** \> **הגדרה** \> **קטגוריות** \> **קטגוריות פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="3de01-125">Go to **Project Management and Accounting** \> **Setup** \> **Categories** \> **Project categories**.</span></span>
2. <span data-ttu-id="3de01-126">בחר **New**.</span><span class="sxs-lookup"><span data-stu-id="3de01-126">Select **New**.</span></span>
3. <span data-ttu-id="3de01-127">בחר את **מזהה הקטגוריה** של הקטגוריה המשותפת שיצרת בסעיף הקודם.</span><span class="sxs-lookup"><span data-stu-id="3de01-127">Select the **Category ID** of the Shared category you created in the previous section.</span></span> <span data-ttu-id="3de01-128">Project Operations מאפשרות להשתמש רק באותן קטגוריות משותפות המשויכות לקטגוריות של עסקאות.</span><span class="sxs-lookup"><span data-stu-id="3de01-128">Project Operations allows using only those shared categories that are associated with transaction categories.</span></span>
4. <span data-ttu-id="3de01-129">בחר קבוצת קטגוריות.</span><span class="sxs-lookup"><span data-stu-id="3de01-129">Select a category group.</span></span>

## <a name="category-groups"></a><span data-ttu-id="3de01-130">קבוצות קטגוריות</span><span class="sxs-lookup"><span data-stu-id="3de01-130">Category groups</span></span>

<span data-ttu-id="3de01-131">קבוצות קטגוריות משמשות לשיתוף מאפיינים, בעיקר פרופילים לרישום, בין קטגוריות פרויקט קשורות.</span><span class="sxs-lookup"><span data-stu-id="3de01-131">Category groups are used to share properties, primarily posting profiles, between related Project categories.</span></span> <span data-ttu-id="3de01-132">חייבת להיות לפחות קבוצת קטגוריות אחת לכל סוג עסקאות וכל קטגוריית פרויקט מוקצה קבוצה.</span><span class="sxs-lookup"><span data-stu-id="3de01-132">There must be at least one category group for each transaction type and each project category is assigned a group.</span></span>

<span data-ttu-id="3de01-133">מפרטי הרישום שב-Project Operations מוגדרים על ידי כללי פרופיל עלות והכנסות הפרויקט וקבוצות הקטגוריות.</span><span class="sxs-lookup"><span data-stu-id="3de01-133">The posting specifications in Project Operations are defined by the project cost and revenue profile rules, project categories, and category groups.</span></span> <span data-ttu-id="3de01-134">תוכל להגדיר קבוצות קטגוריות על ידי מעבר אל **ניהול פרויקטים וחשבונאות** \> **הגדרה** \> **קטגוריות** \> **קבוצות של קטגוריות**.</span><span class="sxs-lookup"><span data-stu-id="3de01-134">You can set up category groups by going to **Project management and accounting** \> **Setup** \> **Categories** \> **Category groups**.</span></span>
