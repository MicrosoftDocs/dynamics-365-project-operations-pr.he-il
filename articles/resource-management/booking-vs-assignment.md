---
title: הזמנות לעומת הקצאות
description: נושא זה מספק מידע על ההבדלים שבין הזמנת משאבים והקצאות משאבים.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: fa99783e52dbcdeaf80bbfd03df0f458f86b5e99
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896012"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="51ac3-103">הזמנות לעומת הקצאות</span><span class="sxs-lookup"><span data-stu-id="51ac3-103">Bookings vs assignments</span></span>

<span data-ttu-id="51ac3-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="51ac3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="51ac3-105">הזמנות הן הקצאה בטוחה או טנטטיבית של משאבים לפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="51ac3-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="51ac3-106">הזמנות בטוחות צורכות קיבולת של משאב.</span><span class="sxs-lookup"><span data-stu-id="51ac3-106">Hard bookings consume a resource's capacity.</span></span> 

<span data-ttu-id="51ac3-107">הקצאות הן הקצאה של משאבים למשימות פרוייקט בלוח הזמנים של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="51ac3-107">Assignments are the assignment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="51ac3-108">המשאבים יכולים להיות אמיתיים או כלליים.</span><span class="sxs-lookup"><span data-stu-id="51ac3-108">The resources can be real or generic.</span></span> 

<span data-ttu-id="51ac3-109">באופן אידיאלי, עבור משאבים אמיתיים, ההזמנות וההקצאות צריכות להתאים, משום שהן לא שונות.</span><span class="sxs-lookup"><span data-stu-id="51ac3-109">Ideally, for real resources, the bookings and assignments should agree, because they don't differ.</span></span> <span data-ttu-id="51ac3-110">עם זאת, Microsoft Dynamics Project Operations אינו אוכף את הסכם זה.</span><span class="sxs-lookup"><span data-stu-id="51ac3-110">However, Microsoft Dynamics Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="51ac3-111">התצוגה **התאמה** מציגה בפני מנהל פרוייקט מקומות שבהם הזמנות וההקצאות של משאב אינן תואמות.</span><span class="sxs-lookup"><span data-stu-id="51ac3-111">The **Reconciliation** view shows a project manager places where a resource's bookings and assignments don't agree.</span></span>
