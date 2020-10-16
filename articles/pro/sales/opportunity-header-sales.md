---
title: כותרת הזדמנות
description: נושא זה מספק מידע על המידע הכולל אודות עסקאות מבוססות פרויקט שורות הזדמנות מבוססיות פרויקט.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 2f08de54767f49c308d0ccc7f2e1c6ef880b7f99
ms.sourcegitcommit: a0f80d024a5d3112a39781815bd31d0c05ddaf6f
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/30/2020
ms.locfileid: "3906183"
---
# <a name="opportunity-header"></a><span data-ttu-id="adcaa-103">כותרת הזדמנות</span><span class="sxs-lookup"><span data-stu-id="adcaa-103">Opportunity header</span></span>

<span data-ttu-id="adcaa-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="adcaa-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="adcaa-105">כותרת ההזדמנות כוללת את המידע הכולל אודות עסקה מבוססת פרויקט החלה על כל השורות בהזדמנות מבוססת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="adcaa-105">The Opportunity header captures the overall information about a project-based deal that applies to all the lines on the project-based opportunity.</span></span>

<span data-ttu-id="adcaa-106">הזדמנויות מבוססות-פרוייקט ב-Dynamics 365 Project Operations הן הרחבות של הזדמנויות Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="adcaa-106">Project-based opportunities in Dynamics 365 Project Operations are extensions of opportunities in Dynamics 365 Sales.</span></span> <span data-ttu-id="adcaa-107">הרחבות אלה מספקות פונקציונליות נוספת ספציפית להזדמנויות מבוססות פרויקט הנדרשת להן.</span><span class="sxs-lookup"><span data-stu-id="adcaa-107">These extensions provide additional functionality that is specific to and required for project-based opportunities.</span></span> <span data-ttu-id="adcaa-108">הרחבות אלה יכולות לכלול שדות חדשים ופעולות סרט הזמינות בהזדמנויות מבוססות פרויקט.</span><span class="sxs-lookup"><span data-stu-id="adcaa-108">These extensions can include new fields and ribbon actions available in project-based opportunities.</span></span> <span data-ttu-id="adcaa-109">יתכן שתמצא שכמה שדות, פונקציונליות ולוגיקת ברירת מחדל הזמינה Sales אינה זמינה ב-Project Operations.</span><span class="sxs-lookup"><span data-stu-id="adcaa-109">You may find some fields, functionality, and defaulting logic that is available in Sales isn't available in Project Operations.</span></span>

<span data-ttu-id="adcaa-110">הטבלה הבאה כוללת את השדות בהזדמנות מבוססת פרויקט שהם ייחודיים ל-Project Operations או שהם כוללים שיוניים חשובים באופן הפעולה מ'הזדמנויות' שב-Sales.</span><span class="sxs-lookup"><span data-stu-id="adcaa-110">The following table includes the fields in a project-based opportunity that are either unique to Project Operations or have some important changes in behavior from the Opportunities in Sales.</span></span>

| <span data-ttu-id="adcaa-111">**שדה**</span><span class="sxs-lookup"><span data-stu-id="adcaa-111">**Field**</span></span> | <span data-ttu-id="adcaa-112">**מיקום**</span><span class="sxs-lookup"><span data-stu-id="adcaa-112">**Location**</span></span> | <span data-ttu-id="adcaa-113">**רלוונטיות, מטרה והכוונה**</span><span class="sxs-lookup"><span data-stu-id="adcaa-113">**Relevance, purpose, and guidance**</span></span> | <span data-ttu-id="adcaa-114">**השפעה במורד הזרם**</span><span class="sxs-lookup"><span data-stu-id="adcaa-114">**Downstream impact**</span></span> |
| --- | --- | --- | --- |
| <span data-ttu-id="adcaa-115">סוג</span><span class="sxs-lookup"><span data-stu-id="adcaa-115">Type</span></span> | <span data-ttu-id="adcaa-116">כרטיסיה כללית (מוסתרת)</span><span class="sxs-lookup"><span data-stu-id="adcaa-116">General tab (hidden)</span></span> | <span data-ttu-id="adcaa-117">שדה קבוצת אפשרויות מכיל את האפשרויות הבאות:</span><span class="sxs-lookup"><span data-stu-id="adcaa-117">This option set field has the following options:</span></span></br><span data-ttu-id="adcaa-118">- מבוססת עבודה (זמין רק כאשר Project Operations מותקן)</span><span class="sxs-lookup"><span data-stu-id="adcaa-118">- Work-based (available only with Project Operations)</span></span></br><span data-ttu-id="adcaa-119">- מבוססת פריט (זמין רק Project Operations ו-Sales מותקנים)</span><span class="sxs-lookup"><span data-stu-id="adcaa-119">- Item-based (available only when Project Operations and Sales are installed)</span></span></br><span data-ttu-id="adcaa-120">- מבוססת תחזוקת שירות (זמין רק כאשר Field Service מותקן)</span><span class="sxs-lookup"><span data-stu-id="adcaa-120">- Service maintenance-based (available when Field Service is installed)</span></span> | <span data-ttu-id="adcaa-121">כאשר אתה משתמש ביישום Project Operations, הערך של שדה זה מוגדר אוטומטית ל**מבוססת עבודה** שמסווג את הזדמנות להזדמנות מבוססת פרויקט.</span><span class="sxs-lookup"><span data-stu-id="adcaa-121">When you use Project Operations, this field value is automatically set to **Work-based** which classifies the Opportunity as project-based.</span></span> <span data-ttu-id="adcaa-122">על ההזדמנות להיות מבוססת פרויקט כדי לאפשר את כל ההרחבות והפונקציונליות הספציפיות לפרויקט בתהליך המכירה במורד הזרם עבור עסקה זו.</span><span class="sxs-lookup"><span data-stu-id="adcaa-122">An Opportunity should be project-based to enable all project-specific extensions and functionality in the downstream sales process for this deal.</span></span> |
| <span data-ttu-id="adcaa-123">איש קשר</span><span class="sxs-lookup"><span data-stu-id="adcaa-123">Contact</span></span> | <span data-ttu-id="adcaa-124">הכרטיסיה 'כללי'</span><span class="sxs-lookup"><span data-stu-id="adcaa-124">General tab</span></span> | <span data-ttu-id="adcaa-125">הפניה לאיש הקשר העיקרי של הלקוח לעסקה זו.</span><span class="sxs-lookup"><span data-stu-id="adcaa-125">Reference to the customer's primary contact for this deal.</span></span> | |
| <span data-ttu-id="adcaa-126">חשבון</span><span class="sxs-lookup"><span data-stu-id="adcaa-126">Account</span></span> | <span data-ttu-id="adcaa-127">הכרטיסיה 'כללי'</span><span class="sxs-lookup"><span data-stu-id="adcaa-127">General tab</span></span> | <span data-ttu-id="adcaa-128">הפניה לחברת הלקוח או לרשומת תיק הלקוח.</span><span class="sxs-lookup"><span data-stu-id="adcaa-128">Reference to the customer's company or account record.</span></span> | |
| <span data-ttu-id="adcaa-129">מנהל תיק לקוח</span><span class="sxs-lookup"><span data-stu-id="adcaa-129">Account Manager</span></span> | <span data-ttu-id="adcaa-130">הכרטיסיה 'כללי'</span><span class="sxs-lookup"><span data-stu-id="adcaa-130">General tab</span></span> | <span data-ttu-id="adcaa-131">השם של מנהל תיק הלקוח עבור הזדמנות מבוססת פרויקט זו.</span><span class="sxs-lookup"><span data-stu-id="adcaa-131">The name of the Account manager for this project-based opportunity.</span></span> | <span data-ttu-id="adcaa-132">מנהל תיק הלקוח אחראי על ניהול הקשר עם הלקוח במהלך השלמת פרויקט זה.</span><span class="sxs-lookup"><span data-stu-id="adcaa-132">The Account manager is responsible for managing the relationship with the customer through the completion of this project.</span></span> <span data-ttu-id="adcaa-133">יחידת החוזה נוצרת כברירת מחדל, בהתבסס על רשומת להצעת המחיר הקשורה למנהל תיק הלקוח.</span><span class="sxs-lookup"><span data-stu-id="adcaa-133">Based on the bookable resource record tied to the Account manager, the contracting unit is defaulted.</span></span> |
| <span data-ttu-id="adcaa-134">יחידת החוזה</span><span class="sxs-lookup"><span data-stu-id="adcaa-134">Contracting Unit</span></span> | <span data-ttu-id="adcaa-135">הכרטיסיה 'כללי'</span><span class="sxs-lookup"><span data-stu-id="adcaa-135">General tab</span></span> | <span data-ttu-id="adcaa-136">יחידת הארגון האחראית להגשת הפרויקט או הפרויקטים הקשורים לעסקה זו.</span><span class="sxs-lookup"><span data-stu-id="adcaa-136">The Organization unit that is responsible for the delivery of the project or projects associated with this deal.</span></span> | <span data-ttu-id="adcaa-137">יחידת החוזה היא החטיבה בחברה שתשלים את הפרויקטים לאחר סגירת העסקה.</span><span class="sxs-lookup"><span data-stu-id="adcaa-137">The contracting unit is the division of the company that will complete the project(s) after the deal is closed.</span></span> <span data-ttu-id="adcaa-138">לכל יחידת חוזה יש מטבע, מטבע זה משמש לדיווח על עלויות משוערות ועלויות בפועל שנגרמו במהלך הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="adcaa-138">Every contracting unit has a currency, and this currency is used to report estimated and actual costs incurred during the project.</span></span> |

<span data-ttu-id="adcaa-139">לכל שאר השדות והמקטעים בכרטיסיה **סיכום** של ההזדמנות, ראה [צור או ערוך הזדמנויות (מרכז המכירות ומכירות)](https://docs.microsoft.com/dynamics365/sales-enterprise/create-edit-opportunity-sales)</span><span class="sxs-lookup"><span data-stu-id="adcaa-139">For all the other fields and sections on the **Summary** tab of the opportunity, see [Create or edit opportunities (Sales and Sales hub)](https://docs.microsoft.com/dynamics365/sales-enterprise/create-edit-opportunity-sales)</span></span>