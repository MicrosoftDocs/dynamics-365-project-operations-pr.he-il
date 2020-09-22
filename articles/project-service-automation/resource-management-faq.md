---
title: שאלות נפוצות בנושא ניהול משאבים
description: נושא זה מספק תשובות לשאלות נפוצות לגבי ניהול משאבים.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: fdf7f1e2-e4a2-4c68-aa03-4a41c7b10531
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 87da759b3b30ed6d38866c045194cde79837c209
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751857"
---
# <a name="resource-management-faq"></a><span data-ttu-id="928ac-103">שאלות נפוצות בנושא ניהול משאבים</span><span class="sxs-lookup"><span data-stu-id="928ac-103">Resource management FAQ</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

## <a name="what-is-the-difference-between-a-team-member-and-a-resource-requirement"></a><span data-ttu-id="928ac-104">מה ההבדל בין חבר צוות לדרישת משאב?</span><span class="sxs-lookup"><span data-stu-id="928ac-104">What is the difference between a team member and a resource requirement?</span></span>

<span data-ttu-id="928ac-105">ניתן להקצות חבר צוות של פרוייקט למשימות שהוזמנו או למשימות בהזמנת יתר, ולהגדיר אותו כמאשר.</span><span class="sxs-lookup"><span data-stu-id="928ac-105">A project team member can be assigned to tasks, booked or overbooked, and set as an approver.</span></span> <span data-ttu-id="928ac-106">דרישת משאב יכולה להתקיים ללא חבר צוות של פרוייקט, כטיוטה של דרישה.</span><span class="sxs-lookup"><span data-stu-id="928ac-106">A resource requirement can exist without a project team member, as a draft note of demand.</span></span> 

## <a name="what-is-the-difference-between-proposed-and-soft-booked-hours"></a><span data-ttu-id="928ac-107">מה ההבדל בין שעות מוצעות לשעות בהזמנה טנטטיבית?</span><span class="sxs-lookup"><span data-stu-id="928ac-107">What is the difference between proposed and soft-booked hours?</span></span>

<span data-ttu-id="928ac-108">שעות מוצעות ושעות בהזמנה טנטטיבית שונות בניראות שלהן.</span><span class="sxs-lookup"><span data-stu-id="928ac-108">Proposed hours and soft-booked hours differ in visibility.</span></span> <span data-ttu-id="928ac-109">שעות מוצעות גלויות אך ורק למנהלי משאבים ולמנהל הפרוייקט שיזם את הדרישה באמצעות בקשת משאב.</span><span class="sxs-lookup"><span data-stu-id="928ac-109">Proposed hours are visible only to resource managers and the project manager who initiated the demand by using a resource request.</span></span> <span data-ttu-id="928ac-110">שעות בהזמנה טנטטיבית גלויות לכל מי שיש לו גישה ללוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="928ac-110">Soft-booked hours are visible to anyone who has access to the Schedule Board.</span></span>

## <a name="how-can-i-see-the-soft-booked-hours-for-resources-on-a-team"></a><span data-ttu-id="928ac-111">כיצד ניתן לראות את שעות ההזמנה הטנטטיבית עבור משאבים בצוות?</span><span class="sxs-lookup"><span data-stu-id="928ac-111">How can I see the soft-booked hours for resources on a team?</span></span>

<span data-ttu-id="928ac-112">ניתן ליצור הזמנות טנטטיביות בעת הזמנה של דרישת משאב.</span><span class="sxs-lookup"><span data-stu-id="928ac-112">Soft bookings can made when you book a resource requirement.</span></span> <span data-ttu-id="928ac-113">משאבים המוזמנים בהזמנה טנטטיבית בצוות פרוייקט מופיעים כחברי צוות בעלי שעות הזמנה טנטטיבית.</span><span class="sxs-lookup"><span data-stu-id="928ac-113">Resources that are soft-booked on a project team appear as team members who have soft-booked hours.</span></span> <span data-ttu-id="928ac-114">הם גם מופיעים בלוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="928ac-114">They also appear on the Schedule Board.</span></span>

## <a name="how-do-i-change-the-required-hours-and-the-start-and-end-dates-for-a-resource-generic-or-named-that-i-booked"></a><span data-ttu-id="928ac-115">כיצד ניתן לשנות את השעות הנדרשות ואת תאריכי ההתחלה והסיום, עבור משאב (כללי או בעל שם) שהזמנתי?</span><span class="sxs-lookup"><span data-stu-id="928ac-115">How do I change the required hours, and the start and end dates, for a resource (generic or named) that I booked?</span></span>

<span data-ttu-id="928ac-116">לאחר הזמנת משאבים, בחר **השאר את ההזמנות** כדי לבצע כל שינוי נדרש.</span><span class="sxs-lookup"><span data-stu-id="928ac-116">After resources are booked, select **Maintain Bookings** to make any changes that are required.</span></span>

## <a name="what-resources-types-does-project-service-automation-support"></a><span data-ttu-id="928ac-117">באילו סוגי משאבים תומך Project Service Automation?</span><span class="sxs-lookup"><span data-stu-id="928ac-117">What resources types does Project Service Automation support?</span></span>

<span data-ttu-id="928ac-118">**משתמש** ו**איש קשר** הם סוגי המשאבים היחידים הנתמכים ב- Dynamics 365 Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="928ac-118">**User** and **Contact** are the only resource types that are supported in Dynamics 365 Project Service Automation.</span></span> <span data-ttu-id="928ac-119">על אף שניתן ליצור סוגים אחרים של משאבים (לדוגמה, **ציוד** ו**קבוצה**), הם לא תומכים במקרי שימוש מקצה לקצה.</span><span class="sxs-lookup"><span data-stu-id="928ac-119">Although you can create other types of resources (for example, **Equipment** and **Group**), no end-to-end use case is supported for them.</span></span>

## <a name="what-is-the-difference-between-an-assignment-and-a-booking"></a><span data-ttu-id="928ac-120">מה ההבדל בין הקצאה להזמנה?</span><span class="sxs-lookup"><span data-stu-id="928ac-120">What is the difference between an assignment and a booking?</span></span>

<span data-ttu-id="928ac-121">הקצאות הן הקצאה של משאבים למשימות פרוייקט בלוח הזמנים של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="928ac-121">Assignments are the assignment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="928ac-122">המשאבים יכולים להיות משאבים אמיתיים או משאבים כלליים.</span><span class="sxs-lookup"><span data-stu-id="928ac-122">The resources can be either real or generic resources.</span></span> <span data-ttu-id="928ac-123">הזמנות הן הקצאה בטוחה או טנטטיבית של משאבים לפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="928ac-123">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="928ac-124">הזמנות בטוחות צורכות קיבולת של משאב.</span><span class="sxs-lookup"><span data-stu-id="928ac-124">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="928ac-125">באופן אידיאלי, עבור משאבים אמיתיים, ההזמנות וההקצאות צריכות להתאים, משום שהן לא שונות.</span><span class="sxs-lookup"><span data-stu-id="928ac-125">Ideally, for real resources, the bookings and assignments should agree, because they don't differ.</span></span> <span data-ttu-id="928ac-126">עם זאת, PSA אינו אוכף הסכם זה.</span><span class="sxs-lookup"><span data-stu-id="928ac-126">However, PSA doesn't enforce this agreement.</span></span> <span data-ttu-id="928ac-127">התצוגה 'התאמה' מציגה בפני מנהל פרוייקט מקומות שבהם הזמנות וההקצאות של משאב אינן תואמות.</span><span class="sxs-lookup"><span data-stu-id="928ac-127">The Reconciliation view shows a project manager places where a resource's bookings and assignments don't agree.</span></span>
