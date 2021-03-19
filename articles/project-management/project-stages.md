---
title: שלבי פרויקט
description: נושא זה מספק מידע על שלבי הפרויקט הקיימים ב- Microsoft Dynamics Project Operations.
author: ruhercul
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: a5c695e0cd39f8a222e719cc6c9ffe984fe80b07
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286789"
---
# <a name="project-stages"></a><span data-ttu-id="4950f-103">שלבי פרויקט</span><span class="sxs-lookup"><span data-stu-id="4950f-103">Project stages</span></span>

<span data-ttu-id="4950f-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="4950f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="4950f-105">שלבי פרויקט מיועדים לשקף את מצב הפרויקט במהלך התקדמותו.</span><span class="sxs-lookup"><span data-stu-id="4950f-105">Project stages are designed to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="4950f-106">ניתן להשתמש בהתאמות אישיות כדי לעדכן אוטומטית את השלבים בזרימת תהליכים עסקיים, Power Automate, או תוספים של יישום plug-in.</span><span class="sxs-lookup"><span data-stu-id="4950f-106">Customizations can be used to automatically update the stages with business process flows, Power Automate, or plug-in extensions.</span></span>

<span data-ttu-id="4950f-107">השלבים הבאים מוגדרים ב- זרימת תהליך עסקי המוגדרת כברירת מחדל:</span><span class="sxs-lookup"><span data-stu-id="4950f-107">The following stages are defined in the default business process flow:</span></span>

- <span data-ttu-id="4950f-108">משתמשים חדשים</span><span class="sxs-lookup"><span data-stu-id="4950f-108">New</span></span>
- <span data-ttu-id="4950f-109">הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="4950f-109">Quote</span></span>
- <span data-ttu-id="4950f-110">תוכנית</span><span class="sxs-lookup"><span data-stu-id="4950f-110">Plan</span></span>
- <span data-ttu-id="4950f-111">מסירה</span><span class="sxs-lookup"><span data-stu-id="4950f-111">Deliver</span></span>
- <span data-ttu-id="4950f-112">מלא</span><span class="sxs-lookup"><span data-stu-id="4950f-112">Complete</span></span>
- <span data-ttu-id="4950f-113">סגורה</span><span class="sxs-lookup"><span data-stu-id="4950f-113">Close</span></span> 

## <a name="new"></a><span data-ttu-id="4950f-114">משתמשים חדשים</span><span class="sxs-lookup"><span data-stu-id="4950f-114">New</span></span>

<span data-ttu-id="4950f-115">בעת יצירת פרויקט, השלב בפרויקט מוגדר בתור **חדש**.</span><span class="sxs-lookup"><span data-stu-id="4950f-115">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="4950f-116">אם הפרויקט נוצר מתבנית, ייתכן שהוא כוללנתונים של לוח זמנים, הערכה וצוות.</span><span class="sxs-lookup"><span data-stu-id="4950f-116">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="4950f-117">אם לא, זהו מיתאר של הפרויקט ויש להזין את הרכיבים הנותרים.</span><span class="sxs-lookup"><span data-stu-id="4950f-117">Otherwise, it's an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="4950f-118">הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="4950f-118">Quote</span></span>

<span data-ttu-id="4950f-119">כאשר אתה משייך פרויקט להצעת מחיר או יוצר אותו מתוך הצעת מחיר, שלב הפרויקט מוגדר **הצעת מחיר**, וההערכות של תאריכי ההתחלה והסיום יעודכנו.</span><span class="sxs-lookup"><span data-stu-id="4950f-119">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="4950f-120">בזמן שהפרויקט נמצא בשלב **הצעת מחיר**, הכרטיסיה **מכירות** בדף **ישות פרויקט** מציגה פרטים לל הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="4950f-120">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="4950f-121">תוכנית</span><span class="sxs-lookup"><span data-stu-id="4950f-121">Plan</span></span>

<span data-ttu-id="4950f-122">כאשר תזכה בהצעת מחיר המשויכת לפרויקט והוא יתקדם לשלב **חוזה**, שלב הפרויקט מתעדכן ל **תוכנית**.</span><span class="sxs-lookup"><span data-stu-id="4950f-122">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="4950f-123">בזמן שהפרויקט נמצא בשלב **תוכנית**, הדף **ישות פרויקט** מציגה פרטים על החוזה.</span><span class="sxs-lookup"><span data-stu-id="4950f-123">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="4950f-124">מסירה</span><span class="sxs-lookup"><span data-stu-id="4950f-124">Deliver</span></span>

<span data-ttu-id="4950f-125">כאשר תוכנית הפרויקט תושלם ותהיה מוכן להתחיל את הפרויקט, מנהל הפרויקט צריך לעדכן את השלב ל **מסירה** כדי להראות שהפרויקט התחיל.</span><span class="sxs-lookup"><span data-stu-id="4950f-125">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="4950f-126">הושלם</span><span class="sxs-lookup"><span data-stu-id="4950f-126">Complete</span></span> 

<span data-ttu-id="4950f-127">כאשר העבודה עבור הפרויקט מסתיימת, מנהל הפרויקט יכול לעדכן את השלב ל **הושלם**.</span><span class="sxs-lookup"><span data-stu-id="4950f-127">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="4950f-128">על-ידי עדכון שלב הפרויקט ל **הושלם**, מנהל הפרויקט מציין שהעבודה הושלמה ב-100 אחוזים, אבל הפרויקט נשאר פתוח כדי שניתן יהיה לתעד ערכי שעות או הוצאות שנמצאים בהמתנה.</span><span class="sxs-lookup"><span data-stu-id="4950f-128">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="4950f-129">סגור</span><span class="sxs-lookup"><span data-stu-id="4950f-129">Close</span></span>

<span data-ttu-id="4950f-130">כאשר כל התנועות תועדו עבור הפרויקט, מנהל הפרויקט יכול לעדכן את השלב ל **סגור**.</span><span class="sxs-lookup"><span data-stu-id="4950f-130">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="4950f-131">בשלב זה, לא ניתן לתעד תנועות והפרויקט מוגדר לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="4950f-131">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]