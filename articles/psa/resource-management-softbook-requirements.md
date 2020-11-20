---
title: דרישות של הזמנה טנטטיבית
description: נושא זה מספק מידע אודות דרישות של הזמנה טנטטיבית.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
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
ms.openlocfilehash: e753dd2f5635d1e9d0d6a02ea5d1d537879dd3a5
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4124099"
---
# <a name="soft-book-requirements"></a><span data-ttu-id="9acbc-103">דרישות של הזמנה טנטטיבית</span><span class="sxs-lookup"><span data-stu-id="9acbc-103">Soft-book requirements</span></span>

<span data-ttu-id="9acbc-104">ניתן להזמין בהזמנה בטוחה דרישה למשאב.</span><span class="sxs-lookup"><span data-stu-id="9acbc-104">A resource requirement can be hard-booked.</span></span> <span data-ttu-id="9acbc-105">הזמנה בטוחה יוצרת הצעה שצורכת קיבולת של משאב.</span><span class="sxs-lookup"><span data-stu-id="9acbc-105">A hard booking creates a proposal that consumes a resource's capacity.</span></span> <span data-ttu-id="9acbc-106">לאחר מכן נשלחת ההצעה בחזרה למבקש לצורך אישור.</span><span class="sxs-lookup"><span data-stu-id="9acbc-106">The proposal is then sent back to the requester for approval.</span></span> <span data-ttu-id="9acbc-107">הזמנה טנטטיבית מוסיפה באופן זמני משאב לצוות פרויקט והיא כוללת מצב שונה בלוח הזמנים, אך היא אינה צורכת את קיבולת המשאב.</span><span class="sxs-lookup"><span data-stu-id="9acbc-107">A soft booking tentatively adds a resource to a project team and has a different status on the Schedule Board, but it doesn't consume the resource's capacity.</span></span> <span data-ttu-id="9acbc-108">כדי להזמין משאב בהזמנה טנטטיבית מלוח הזמנים, הגדר את השדה **מצב הזמנה** ל **זמני**.</span><span class="sxs-lookup"><span data-stu-id="9acbc-108">To soft-book a resource from the Schedule Board, set the **Booking Status** field to **Soft**.</span></span>

![מצב ההזמנה מוגדר כ'זמני'](media/Resource-Management-image77.png)

<span data-ttu-id="9acbc-110">כאשר הכרטיסיה **צוות** נמצאת בתצוגה **חברי צוות בעלי שם**, המשאב מופיע שם.</span><span class="sxs-lookup"><span data-stu-id="9acbc-110">When the **Team** tab is in the **Named Team Members** view, the resource appears there.</span></span> <span data-ttu-id="9acbc-111">שעות ההזמנה הטנטטיבית מדווחות בעמודה **שעות שהוזמנו בהזמנה טנטטיבית**.</span><span class="sxs-lookup"><span data-stu-id="9acbc-111">The soft-booked hours are reported in the **Soft Booked Hours** column.</span></span>

![שעות שהוזמנו בהזמנה טנטטיבית בתצוגה 'חברי צוות בעלי שם'](media/Resource-Management-image78.png)

<span data-ttu-id="9acbc-113">ניתן להקצות חברי צוות שהוזמנו בהזמנה טנטטיבית למשימות.</span><span class="sxs-lookup"><span data-stu-id="9acbc-113">Soft-booked team members can be assigned to tasks.</span></span>

![חבר צוות שהוזמן בהזמנה טנטטיבית הוקצה למשימה](media/Resource-Management-image79.png)

<span data-ttu-id="9acbc-115">בכרטיסיה **התאמה**, לא מוצגות הזמנות עבור משאב שהוזמן בהזמנה טנטטיבית, משום שהכרטיסיה **התאמה** לוקחת בחשבון הזמנות בטוחות בלבד.</span><span class="sxs-lookup"><span data-stu-id="9acbc-115">On the **Reconciliation** tab, no bookings are shown for a soft-book resource, because the **Reconciliation** tab considers only hard-bookings.</span></span>

![משאב שהוזמן בהזמנה טנטטיבית ללא הזמנות בכרטיסיה 'התאמה'](media/Resource-Management-image80.png)

> [!NOTE]
> <span data-ttu-id="9acbc-117">לא ניתן להזמין משאב בהזמנה טנטטיבית מדרישה שנוצרה מחבר צוות כללי.</span><span class="sxs-lookup"><span data-stu-id="9acbc-117">You can't soft-book a resource from a requirement that was generated from a generic team member.</span></span>

<span data-ttu-id="9acbc-118">בלוח הזמנים, צבע שונה משמש להזמנות טנטטיביות של משאב.</span><span class="sxs-lookup"><span data-stu-id="9acbc-118">On the Schedule Board, a different coloring is used for soft bookings for a resource.</span></span>

![הזמנות טנטטיביות בלוח הזמנים](media/Resource-Management-image81.png)

<span data-ttu-id="9acbc-120">כדי להמיר הזמנה טנטטיבית להזמנה בטוחה, בלוח הזמנים, לחץ באמצעות לחצן העכבר הימני על ההזמנה הטנטטיבית ולאחר מכן בחר **שנה מצב** \> **הזמן כהזמנה בטוחה** \> **הזמנה בטוחה**.</span><span class="sxs-lookup"><span data-stu-id="9acbc-120">To convert a soft booking to a hard booking, on the Schedule Board, right-click the soft booking, and then select **Change Status** \> **Hard Book** \> **Hard**.</span></span>

![שינוי מצב ההזמנה להזמנה בטוחה](media/Resource-Management-image82.png)

<span data-ttu-id="9acbc-122">ההזמנה משתנה והמצב משתנה בלוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="9acbc-122">The booking is changed, and the status is changed on the Schedule Board.</span></span> <span data-ttu-id="9acbc-123">מכיוון שמצב ההזמנה הוא כעת **הזמנה בטוחה**, המשאב מוצג כמשאב שהוזמן, והקיבולת והזמינות שלו מותאמות.</span><span class="sxs-lookup"><span data-stu-id="9acbc-123">Because the booking status is now **Hard**, the resource is shown as booked, and its capacity and availability are adjusted.</span></span>

<span data-ttu-id="9acbc-124">ניתן להשתמש באותה שיטה כדי לבטל הזמנה בטוחה או הזמנה טנטטיבית מלוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="9acbc-124">You can use the same method to cancel a hard booking or a soft booking from the Schedule Board.</span></span>

<span data-ttu-id="9acbc-125">כדי להמיר משאב שהוזמן בהזמנה טנטטיבית למשאב שהוזמן בהזמנה בטוחה בכרטיסיה **צוות** של הפרויקט, בחר את המשאב ולאחר מכן בחר **אשר**.</span><span class="sxs-lookup"><span data-stu-id="9acbc-125">To convert a resource that is soft-booked to hard-booked on the project's **Team** tab, select the resource, and then select **Confirm**.</span></span>

![הפקודה 'אשר'](media/Resource-Management-image83.png)
