---
title: הגדרת לוחות שנה של פרוייקטים
description: נושא זה מספק מידע על אופן החלת תבנית לוח שנה על פרויקט כדי לעקוב אחר לוח הזמנים של הפרויקט.
author: ruhercul
manager: AnnBe
ms.date: 02/05/2021
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
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 1d5642d7a2246dc878b2bc4f504f138b71d29a69
ms.sourcegitcommit: c45ceda833b30ad39861f5bcd3ba1bbfff11fe7a
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/04/2021
ms.locfileid: "5981301"
---
# <a name="define-project-calendars"></a><span data-ttu-id="1c60f-103">הגדרת לוחות שנה של פרוייקטים</span><span class="sxs-lookup"><span data-stu-id="1c60f-103">Define project calendars</span></span>

<span data-ttu-id="1c60f-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="1c60f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1c60f-105">כדי ליצור ולנהל פרויקט, עליך להחיל תבנית לוח שנה על הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="1c60f-105">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="1c60f-106">תבנית לוח השנה מגדירה את התכונות הבאות של הפרויקט:</span><span class="sxs-lookup"><span data-stu-id="1c60f-106">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="1c60f-107">שעות עבודה, כולל שעת התחלה וסיום</span><span class="sxs-lookup"><span data-stu-id="1c60f-107">Working hours, including start and end time</span></span>
- <span data-ttu-id="1c60f-108">ימי עבודה</span><span class="sxs-lookup"><span data-stu-id="1c60f-108">Working days</span></span>
- <span data-ttu-id="1c60f-109">חריגים ביומן כגון ימים שאינם ימי עבודה</span><span class="sxs-lookup"><span data-stu-id="1c60f-109">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="1c60f-110">תבנית לוח השנה המוחלת על פרויקט היא העתק של תבנית לוח השנה המוגדרת בהגדרות הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="1c60f-110">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="1c60f-111">אם תשנה את תבנית לוח השנה, שינויים אלה אינם מופצים לשעות העבודה של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="1c60f-111">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="1c60f-112">כדי לשנות את שעות העבודה של הפרויקט, יש להחיל תבנית חדשה.</span><span class="sxs-lookup"><span data-stu-id="1c60f-112">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="1c60f-113">כדי ליצור תבנית לוח שנה לארגון שלך, ישנן שתי דרישות עיקריות:</span><span class="sxs-lookup"><span data-stu-id="1c60f-113">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="1c60f-114">הגדר את שעות העבודה הרצויות של התבנית באמצעות משאב חדש או קיים שניתן להזמנה.</span><span class="sxs-lookup"><span data-stu-id="1c60f-114">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="1c60f-115">צור תבנית לוח שנה חדשה ושייך את התבנית למשאב שניתן להזמינה.</span><span class="sxs-lookup"><span data-stu-id="1c60f-115">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="1c60f-116">**הגדרת שעות העבודרה של התבנית**</span><span class="sxs-lookup"><span data-stu-id="1c60f-116">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="1c60f-117">עבור אל **משאבים** \> **משאבים**.</span><span class="sxs-lookup"><span data-stu-id="1c60f-117">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="1c60f-118">צור משאב חדש להפניה בתבנית לוח השנה, או בחר משאב קיים.</span><span class="sxs-lookup"><span data-stu-id="1c60f-118">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="1c60f-119">בחר את הכרטיסיה **שעות עבודה** של המשאב והשלם את ההוראות בהסבר: [הגדרת שעות עבודה עבור משאב](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) כדי להגדיר את כללי לוח השנה.</span><span class="sxs-lookup"><span data-stu-id="1c60f-119">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](https://docs.microsoft.com/dynamics365/field-service/set-work-hours-resource) to configure the calendar rules.</span></span>

<span data-ttu-id="1c60f-120">**צור תבנית לוח שנה חדשה**</span><span class="sxs-lookup"><span data-stu-id="1c60f-120">**Create a new calendar template**</span></span>

1. <span data-ttu-id="1c60f-121">עבור אל **הגדרות** \> **תבנית לוח שנה**.</span><span class="sxs-lookup"><span data-stu-id="1c60f-121">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="1c60f-122">בחר **חדש** והזן שם, תיאור תבנית משאב.</span><span class="sxs-lookup"><span data-stu-id="1c60f-122">Select **New**, and enter a name, description, and template resource.</span></span>

> [!NOTE]
> <span data-ttu-id="1c60f-123">כאשר משאב כולל בהפניה בתבנית לוח שנה, עותק של לוח השנה של המשאב משויך לתבנית לוח השנה.</span><span class="sxs-lookup"><span data-stu-id="1c60f-123">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="1c60f-124">אם ישונו שעות העבודה של תבנית לוח השנה שהועתקה, שינויים אלה אינם מופצים לשעות העבודה של תבנית לוח השנה.</span><span class="sxs-lookup"><span data-stu-id="1c60f-124">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>

<span data-ttu-id="1c60f-125">כעת תוכל לשייך את תבנית העבודה לתבנית לוח שנה של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="1c60f-125">You can now associate the work template with a project calendar template.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]

