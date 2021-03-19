---
title: עדכון פרויקט
description: נושא זה מספק מידע על עדכון פרויקטים ב- Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 27444b072bdf7de55d6b38c30c1ea5fe66ed46ac
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286384"
---
# <a name="update-a-project"></a><span data-ttu-id="8529e-103">עדכון פרויקט</span><span class="sxs-lookup"><span data-stu-id="8529e-103">Update a project</span></span>

<span data-ttu-id="8529e-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="8529e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8529e-105">להלן סיכום השדות שניתן לעדכן בפרויקט לאחר יצירתו וכל ההשלכות החלות על העדכונים.</span><span class="sxs-lookup"><span data-stu-id="8529e-105">Below is a summary of the fields that can be updated on a project after it has been created and any applicable implications of the updates.</span></span>

## <a name="project-detail-fields"></a><span data-ttu-id="8529e-106">שדות פרטי פרויקט</span><span class="sxs-lookup"><span data-stu-id="8529e-106">Project detail fields</span></span>

- <span data-ttu-id="8529e-107">**שם**: שם הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8529e-107">**Name**: The title of the project.</span></span>
- <span data-ttu-id="8529e-108">**תיאור**: מבט כולל על הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8529e-108">**Description**: An overview of the project.</span></span>
- <span data-ttu-id="8529e-109">**לקוח**: החברה לה יסופק הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8529e-109">**Customer**: The company the project will be delivered to.</span></span>
- <span data-ttu-id="8529e-110">**תבנית לוח שנה**: שעות העבודה על הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8529e-110">**Calendar template**: The working hours of the project.</span></span> <span data-ttu-id="8529e-111">כשמתבצע שינוי בשדה, לוח הזמנים כולו מחושב מחדש.</span><span class="sxs-lookup"><span data-stu-id="8529e-111">When the field is changed, the entire schedule is recalculated.</span></span>
- <span data-ttu-id="8529e-112">**מטבע**: המטבע של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8529e-112">**Currency**: The currency for the project.</span></span> <span data-ttu-id="8529e-113">ברירת המחדל עבור שדה זה מתבססת על המטבע שהוגדר ביחידת החוזה.</span><span class="sxs-lookup"><span data-stu-id="8529e-113">This field defaults based on the currency defined in the contracting unit.</span></span> <span data-ttu-id="8529e-114">כאשר יחידת החוזה מתעדכנת, גם השדה מתעדכן.</span><span class="sxs-lookup"><span data-stu-id="8529e-114">When the contracting unit is updated, the field is also updated.</span></span>
- <span data-ttu-id="8529e-115">**יחידת חוזה**: היחידה הארגונית המייצגת את קבוצת החברה או חטיבת החברה האחראית בראש ובראשונה לזכייה במכירה ולניהול אספקת העבודה והשירותים ללקוח.</span><span class="sxs-lookup"><span data-stu-id="8529e-115">**Contracting Unit**: The organizational unit that represents the company group or division that is primarily responsible for winning the sale and managing the delivery of work and services to the customer.</span></span> 
- <span data-ttu-id="8529e-116">**מנהל פרויקט**: החבר בצוות הפרויקט שבסמכותו לבדוק ולאשר ערכי זמן והוצאות.</span><span class="sxs-lookup"><span data-stu-id="8529e-116">**Project Manager**: The project team member who has the authority to review and approve time entries and expenses.</span></span>

## <a name="estimate-fields"></a><span data-ttu-id="8529e-117">שדות הערכה</span><span class="sxs-lookup"><span data-stu-id="8529e-117">Estimate fields</span></span>

- <span data-ttu-id="8529e-118">**תאריך התחלה משוער**: התאריך בו יתחיל הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8529e-118">**Estimated Start Date**: The date that the project will begin.</span></span> <span data-ttu-id="8529e-119">כאשר שדה זה מתעדכן, כל המשימות בפרויקט זזות ביחס לתאריך ההתחלה החדש.</span><span class="sxs-lookup"><span data-stu-id="8529e-119">When this field is updated, any tasks on the project will move proportionately with the start new start date.</span></span>
- <span data-ttu-id="8529e-120">**תאריך סיום**: התאריך בו הפרויקט מתוכנן להסתיים.</span><span class="sxs-lookup"><span data-stu-id="8529e-120">**Finish Date**: The date that the project is scheduled to end.</span></span>
- <span data-ttu-id="8529e-121">**מאמץ**: המאמץ המשוער עבור הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8529e-121">**Effort**: The estimated effort of the project.</span></span> <span data-ttu-id="8529e-122">לאחר שמשימות מתווספות לפרויקט, כבר לא ניתן לערוך שדה זה.</span><span class="sxs-lookup"><span data-stu-id="8529e-122">When tasks are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="8529e-123">**עלות עבודה משוערת**: עלות העבודה המשוערת של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8529e-123">**Estimated Labor Cost**: The estimated labor cost of the project.</span></span> <span data-ttu-id="8529e-124">לאחר שעלויות עבודה מתווספות לפרויקט, כבר לא ניתן לערוך שדה זה.</span><span class="sxs-lookup"><span data-stu-id="8529e-124">When labor costs are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="8529e-125">**הוצאות משוערות**: ההוצאות המשוערות של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8529e-125">**Estimated Expenses**: The estimated expenses of the project.</span></span> <span data-ttu-id="8529e-126">לאחר שהוצאות מתווספות לפרויקט, כבר לא ניתן לערוך שדה זה.</span><span class="sxs-lookup"><span data-stu-id="8529e-126">When expenses are added to the project, this field is no longer editable.</span></span>

## <a name="project-actual-fields"></a><span data-ttu-id="8529e-127">שדות פרויקט בפועל</span><span class="sxs-lookup"><span data-stu-id="8529e-127">Project actual fields</span></span>
- <span data-ttu-id="8529e-128">**התחלה בפועל**: התאריך בו החל הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8529e-128">**Actual Start**: The date that the project started.</span></span>
- <span data-ttu-id="8529e-129">**סיום בפועל**: יעודכן לאחר סיום הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8529e-129">**Actual Finish**: To be updated when a project has been completed.</span></span>

## <a name="project-status-fields"></a><span data-ttu-id="8529e-130">שדות מצב פרויקט</span><span class="sxs-lookup"><span data-stu-id="8529e-130">Project status fields</span></span>

- <span data-ttu-id="8529e-131">**מצב פרויקט כולל**: התקינות הכוללת של הפרויקט לפי מנהל הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8529e-131">**Overall Project Status**: The overall project health provided by the Project manager.</span></span>
- <span data-ttu-id="8529e-132">**הערות**: תיאור התקינות של הפרויקט נכון לאותו רגע, לפי מנהל הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8529e-132">**Comments**: A narrative regarding the current health of the project provided by the Project manager.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]