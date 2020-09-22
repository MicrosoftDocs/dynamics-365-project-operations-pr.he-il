---
title: שלבי פרוייקט
description: נושא זו מספק מידע על שלבי פרוייקט.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 983c25a0-ed21-4151-a109-b385a88285fa
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 70aa057e127df7ba925e84f5d056a06a4cc8833e
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751780"
---
# <a name="project-stages"></a><span data-ttu-id="94cc5-103">שלבי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="94cc5-103">Project stages</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="94cc5-104">שלבי פרוייקט מתעדכנים כדי לשקף את מצב הפרוייקט במהלך התקדמותו.</span><span class="sxs-lookup"><span data-stu-id="94cc5-104">Project stages are updated to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="94cc5-105">זרימת התהליך העסקי בברירת המחדל מעדכנת באופן אוטומטי שלבים מסוימים של הפרוייקט בזמן ששלבים אחרים מתעדכנים באופן ידני על-ידי מנהל הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="94cc5-105">The default business process flow automatically updates some stages of the project while others are manually updated by the project manager.</span></span> 

<span data-ttu-id="94cc5-106">השלבים הבאים מוגדרים ב- BPF המוגדר כברירת מחדל:</span><span class="sxs-lookup"><span data-stu-id="94cc5-106">The following stages are defined in the default BPF:</span></span>

- <span data-ttu-id="94cc5-107">חדש</span><span class="sxs-lookup"><span data-stu-id="94cc5-107">New</span></span>
- <span data-ttu-id="94cc5-108">הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="94cc5-108">Quote</span></span>
- <span data-ttu-id="94cc5-109">תוכנית</span><span class="sxs-lookup"><span data-stu-id="94cc5-109">Plan</span></span>
- <span data-ttu-id="94cc5-110">מסירה</span><span class="sxs-lookup"><span data-stu-id="94cc5-110">Deliver</span></span>
- <span data-ttu-id="94cc5-111">הושלם</span><span class="sxs-lookup"><span data-stu-id="94cc5-111">Complete</span></span>
- <span data-ttu-id="94cc5-112">סגור</span><span class="sxs-lookup"><span data-stu-id="94cc5-112">Close</span></span> 

## <a name="new"></a><span data-ttu-id="94cc5-113">חדש</span><span class="sxs-lookup"><span data-stu-id="94cc5-113">New</span></span>

<span data-ttu-id="94cc5-114">בעת יצירת פרוייקט, השלב בפרוייקט מוגדר בתור **חדש**.</span><span class="sxs-lookup"><span data-stu-id="94cc5-114">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="94cc5-115">אם הפרוייקט נוצר מתבנית, ייתכן שהוא כוללנתונים של לוח זמנים, הערכה וצוות.</span><span class="sxs-lookup"><span data-stu-id="94cc5-115">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="94cc5-116">אחרת, זהו רק מיתאר של הפרוייקט ויש להזין את הרכיבים הנותרים.</span><span class="sxs-lookup"><span data-stu-id="94cc5-116">Otherwise, it's just an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="94cc5-117">הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="94cc5-117">Quote</span></span>

<span data-ttu-id="94cc5-118">כאשר אתה משייך פרוייקט להצעת מחיר או יוצר אותו מתוך הצעת מחיר, שלב הפרוייקט מוגדר **הצעת מחיר**, וההערכות של תאריכי ההתחלה והסיום יעודכנו.</span><span class="sxs-lookup"><span data-stu-id="94cc5-118">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="94cc5-119">בזמן שהפרוייקט נמצא בשלב **הצעת מחיר**, הכרטיסיה **מכירות** בדף **ישות פרוייקט** מציגה פרטים לל הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="94cc5-119">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="94cc5-120">תוכנית</span><span class="sxs-lookup"><span data-stu-id="94cc5-120">Plan</span></span>

<span data-ttu-id="94cc5-121">כאשר תזכה בהצעת מחיר המשויכת לפרוייקט והוא יתקדם לשלב **חוזה**, שלב הפרוייקט מתעדכן ל**תוכנית**.</span><span class="sxs-lookup"><span data-stu-id="94cc5-121">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="94cc5-122">בזמן שהפרוייקט נמצא בשלב **תוכנית**, הדף **ישות פרוייקט** מציגה פרטים על החוזה.</span><span class="sxs-lookup"><span data-stu-id="94cc5-122">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="94cc5-123">מסירה</span><span class="sxs-lookup"><span data-stu-id="94cc5-123">Deliver</span></span>

<span data-ttu-id="94cc5-124">כאשר תוכנית הפרוייקט תושלם ותהיה מוכן להתחיל את הפרוייקט, מנהל הפרוייקט צריך לעדכן את השלב ל**מסירה** כדי להראות שהפרוייקט התחיל.</span><span class="sxs-lookup"><span data-stu-id="94cc5-124">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="94cc5-125">הושלם</span><span class="sxs-lookup"><span data-stu-id="94cc5-125">Complete</span></span> 

<span data-ttu-id="94cc5-126">כאשר העבודה עבור הפרוייקט מסתיימת, מנהל הפרוייקט יכול לעדכן את השלב ל**הושלם**.</span><span class="sxs-lookup"><span data-stu-id="94cc5-126">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="94cc5-127">על-ידי עדכון שלב הפרוייקט ל**הושלם**, מנהל הפרוייקט מציין שהעבודה הושלמה ב-100 אחוזים, אבל הפרוייקט נשאר פתוח כדי שניתן יהיה לתעד ערכי שעות או הוצאות שנמצאים בהמתנה.</span><span class="sxs-lookup"><span data-stu-id="94cc5-127">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="94cc5-128">סגור</span><span class="sxs-lookup"><span data-stu-id="94cc5-128">Close</span></span>

<span data-ttu-id="94cc5-129">כאשר כל התנועות תועדו עבור הפרוייקט, מנהל הפרוייקט יכול לעדכן את השלב ל**סגור**.</span><span class="sxs-lookup"><span data-stu-id="94cc5-129">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="94cc5-130">בשלב זה, לא ניתן לתעד תנועות והפרוייקט מוגדר לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="94cc5-130">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>
