---
title: יצירת תבנית שעות עבודה
description: נושא זה מתאר כיצד ליצור תבנית שעות עבודה ב- Project Service.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: 525f601ad6fee902cb6d5c128b596cc2d33f30c4
ms.sourcegitcommit: c45ceda833b30ad39861f5bcd3ba1bbfff11fe7a
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/04/2021
ms.locfileid: "5981256"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="6ef86-103">יצירת תבנית שעות עבודה (Project Service)</span><span class="sxs-lookup"><span data-stu-id="6ef86-103">Create a work hours template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="6ef86-104">כדי ליצור ולנהל פרויקט, עליך להחיל תבנית לוח שנה על הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="6ef86-104">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="6ef86-105">תבנית לוח השנה מגדירה את התכונות הבאות של הפרויקט:</span><span class="sxs-lookup"><span data-stu-id="6ef86-105">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="6ef86-106">שעות עבודה, כולל שעת התחלה וסיום</span><span class="sxs-lookup"><span data-stu-id="6ef86-106">Working hours, including start and end time</span></span>
- <span data-ttu-id="6ef86-107">ימי עבודה</span><span class="sxs-lookup"><span data-stu-id="6ef86-107">Working days</span></span>
- <span data-ttu-id="6ef86-108">חריגים ביומן כגון ימים שאינם ימי עבודה</span><span class="sxs-lookup"><span data-stu-id="6ef86-108">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="6ef86-109">תבנית לוח השנה המוחלת על פרויקט היא העתק של תבנית לוח השנה המוגדרת בהגדרות הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="6ef86-109">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="6ef86-110">אם תשנה את תבנית לוח השנה, שינויים אלה אינם מופצים לשעות העבודה של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="6ef86-110">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="6ef86-111">כדי לשנות את שעות העבודה של הפרויקט, יש להחיל תבנית חדשה.</span><span class="sxs-lookup"><span data-stu-id="6ef86-111">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="6ef86-112">כדי ליצור תבנית לוח שנה לארגון שלך, ישנן שתי דרישות עיקריות:</span><span class="sxs-lookup"><span data-stu-id="6ef86-112">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="6ef86-113">הגדר את שעות העבודה הרצויות של התבנית באמצעות משאב חדש או קיים שניתן להזמנה.</span><span class="sxs-lookup"><span data-stu-id="6ef86-113">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="6ef86-114">צור תבנית לוח שנה חדשה ושייך את התבנית למשאב שניתן להזמינה.</span><span class="sxs-lookup"><span data-stu-id="6ef86-114">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="6ef86-115">**הגדרת שעות העבודרה של התבנית**</span><span class="sxs-lookup"><span data-stu-id="6ef86-115">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="6ef86-116">עבור אל **משאבים** \> **משאבים**.</span><span class="sxs-lookup"><span data-stu-id="6ef86-116">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="6ef86-117">צור משאב חדש להפניה בתבנית לוח השנה, או בחר משאב קיים.</span><span class="sxs-lookup"><span data-stu-id="6ef86-117">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="6ef86-118">בחר את הכרטיסיה **שעות עבודה** של המשאב והשלם את ההוראות בהסבר: [הגדרת שעות עבודה עבור משאב](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) כדי להגדיר את כללי לוח השנה.</span><span class="sxs-lookup"><span data-stu-id="6ef86-118">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) to configure the calendar rules.</span></span>

<span data-ttu-id="6ef86-119">**צור תבנית לוח שנה חדשה**</span><span class="sxs-lookup"><span data-stu-id="6ef86-119">**Create a new calendar template**</span></span>

1. <span data-ttu-id="6ef86-120">עבור אל **הגדרות** \> **תבנית לוח שנה**.</span><span class="sxs-lookup"><span data-stu-id="6ef86-120">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="6ef86-121">בחר **חדש** והזן שם, תיאור תבנית משאב.</span><span class="sxs-lookup"><span data-stu-id="6ef86-121">Select **New**, and enter a name, description, and template resource.</span></span>


> [!NOTE]
> <span data-ttu-id="6ef86-122">כאשר משאב כולל בהפניה בתבנית לוח שנה, עותק של לוח השנה של המשאב משויך לתבנית לוח השנה.</span><span class="sxs-lookup"><span data-stu-id="6ef86-122">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="6ef86-123">אם ישונו שעות העבודה של תבנית לוח השנה שהועתקה, שינויים אלה אינם מופצים לשעות העבודה של תבנית לוח השנה.</span><span class="sxs-lookup"><span data-stu-id="6ef86-123">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>


### <a name="see-also"></a><span data-ttu-id="6ef86-124">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="6ef86-124">See Also</span></span>  
 [<span data-ttu-id="6ef86-125">הגדרת משאבים</span><span class="sxs-lookup"><span data-stu-id="6ef86-125">Set up resources</span></span>](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
