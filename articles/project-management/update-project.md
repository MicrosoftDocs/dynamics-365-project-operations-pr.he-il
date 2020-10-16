---
title: עדכון פרוייקט
description: נושא זה מספק מידע על עדכון פרוייקטים ב- Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 5c9cd0c7c6886bd454c5f2ef2ae7f20d1707293f
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897813"
---
# <a name="update-a-project"></a><span data-ttu-id="faea8-103">עדכון פרוייקט</span><span class="sxs-lookup"><span data-stu-id="faea8-103">Update a project</span></span>

<span data-ttu-id="faea8-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="faea8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="faea8-105">להלן סיכום השדות שניתן לעדכן בפרוייקט לאחר יצירתו וכל ההשלכות החלות על העדכונים.</span><span class="sxs-lookup"><span data-stu-id="faea8-105">Below is a summary of the fields that can be updated on a project after it has been created and any applicable implications of the updates.</span></span>

## <a name="project-detail-fields"></a><span data-ttu-id="faea8-106">שדות פרטי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="faea8-106">Project detail fields</span></span>

- <span data-ttu-id="faea8-107">**שם**: שם הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="faea8-107">**Name**: The title of the project.</span></span>
- <span data-ttu-id="faea8-108">**תיאור**: מבט כולל על הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="faea8-108">**Description**: An overview of the project.</span></span>
- <span data-ttu-id="faea8-109">**לקוח**: החברה לה יסופק הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="faea8-109">**Customer**: The company the project will be delivered to.</span></span>
- <span data-ttu-id="faea8-110">**תבנית לוח שנה**: שעות העבודה על הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="faea8-110">**Calendar template**: The working hours of the project.</span></span> <span data-ttu-id="faea8-111">כשמתבצע שינוי בשדה, לוח הזמנים כולו מחושב מחדש.</span><span class="sxs-lookup"><span data-stu-id="faea8-111">When the field is changed, the entire schedule is recalculated.</span></span>
- <span data-ttu-id="faea8-112">**מטבע**: המטבע של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="faea8-112">**Currency**: The currency for the project.</span></span> <span data-ttu-id="faea8-113">ברירת המחדל עבור שדה זה מתבססת על המטבע שהוגדר ביחידת החוזה.</span><span class="sxs-lookup"><span data-stu-id="faea8-113">This field defaults based on the currency defined in the contracting unit.</span></span> <span data-ttu-id="faea8-114">כאשר יחידת החוזה מתעדכנת, גם השדה מתעדכן.</span><span class="sxs-lookup"><span data-stu-id="faea8-114">When the contracting unit is updated, the field is also updated.</span></span>
- <span data-ttu-id="faea8-115">**יחידת חוזה**: היחידה הארגונית המייצגת את קבוצת החברה או חטיבת החברה האחראית בראש ובראשונה לזכייה במכירה ולניהול אספקת העבודה והשירותים ללקוח.</span><span class="sxs-lookup"><span data-stu-id="faea8-115">**Contracting Unit**: The organizational unit that represents the company group or division that is primarily responsible for winning the sale and managing the delivery of work and services to the customer.</span></span> 
- <span data-ttu-id="faea8-116">**מנהל פרוייקט**: החבר בצוות הפרוייקט שבסמכותו לבדוק ולאשר ערכי זמן והוצאות.</span><span class="sxs-lookup"><span data-stu-id="faea8-116">**Project Manager**: The project team member who has the authority to review and approve time entries and expenses.</span></span>

## <a name="estimate-fields"></a><span data-ttu-id="faea8-117">שדות הערכה</span><span class="sxs-lookup"><span data-stu-id="faea8-117">Estimate fields</span></span>

- <span data-ttu-id="faea8-118">**תאריך התחלה משוער**: התאריך בו יתחיל הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="faea8-118">**Estimated Start Date**: The date that the project will begin.</span></span> <span data-ttu-id="faea8-119">כאשר שדה זה מתעדכן, כל המשימות בפרוייקט זזות ביחס לתאריך ההתחלה החדש.</span><span class="sxs-lookup"><span data-stu-id="faea8-119">When this field is updated, any tasks on the project will move proportionately with the start new start date.</span></span>
- <span data-ttu-id="faea8-120">**תאריך סיום**: התאריך בו הפרוייקט מתוכנן להסתיים.</span><span class="sxs-lookup"><span data-stu-id="faea8-120">**Finish Date**: The date that the project is scheduled to end.</span></span>
- <span data-ttu-id="faea8-121">**מאמץ**: המאמץ המשוער עבור הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="faea8-121">**Effort**: The estimated effort of the project.</span></span> <span data-ttu-id="faea8-122">לאחר שמשימות מתווספות לפרוייקט, כבר לא ניתן לערוך שדה זה.</span><span class="sxs-lookup"><span data-stu-id="faea8-122">When tasks are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="faea8-123">**עלות עבודה משוערת**: עלות העבודה המשוערת של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="faea8-123">**Estimated Labor Cost**: The estimated labor cost of the project.</span></span> <span data-ttu-id="faea8-124">לאחר שעלויות עבודה מתווספות לפרוייקט, כבר לא ניתן לערוך שדה זה.</span><span class="sxs-lookup"><span data-stu-id="faea8-124">When labor costs are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="faea8-125">**הוצאות משוערות**: ההוצאות המשוערות של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="faea8-125">**Estimated Expenses**: The estimated expenses of the project.</span></span> <span data-ttu-id="faea8-126">לאחר שהוצאות מתווספות לפרוייקט, כבר לא ניתן לערוך שדה זה.</span><span class="sxs-lookup"><span data-stu-id="faea8-126">When expenses are added to the project, this field is no longer editable.</span></span>

## <a name="project-actual-fields"></a><span data-ttu-id="faea8-127">שדות פרוייקט בפועל</span><span class="sxs-lookup"><span data-stu-id="faea8-127">Project actual fields</span></span>
- <span data-ttu-id="faea8-128">**התחלה בפועל**: התאריך בו החל הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="faea8-128">**Actual Start**: The date that the project started.</span></span>
- <span data-ttu-id="faea8-129">**סיום בפועל**: יעודכן לאחר סיום הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="faea8-129">**Actual Finish**: To be updated when a project has been completed.</span></span>

## <a name="project-status-fields"></a><span data-ttu-id="faea8-130">שדות מצב פרוייקט</span><span class="sxs-lookup"><span data-stu-id="faea8-130">Project status fields</span></span>

- <span data-ttu-id="faea8-131">**מצב פרוייקט כולל**: התקינות הכוללת של הפרוייקט לפי מנהל הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="faea8-131">**Overall Project Status**: The overall project health provided by the Project manager.</span></span>
- <span data-ttu-id="faea8-132">**הערות**: תיאור התקינות של הפרוייקט נכון לאותו רגע, לפי מנהל הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="faea8-132">**Comments**: A narrative regarding the current health of the project provided by the Project manager.</span></span>

