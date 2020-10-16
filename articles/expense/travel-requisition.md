---
title: דרישות נסיעה
description: נושא זה מספק מידע על דרישות הקשורות לנסיעות.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 0261405abb9305d7f6abcde9cb90d9b184868580
ms.sourcegitcommit: a0f80d024a5d3112a39781815bd31d0c05ddaf6f
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/30/2020
ms.locfileid: "3906184"
---
# <a name="travel-requisitions"></a><span data-ttu-id="6c067-103">דרישות נסיעה</span><span class="sxs-lookup"><span data-stu-id="6c067-103">Travel requisitions</span></span>

<span data-ttu-id="6c067-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="6c067-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="6c067-105">דרישת נסיעה מפרטת את ההוצאות שיהיו כרוכות בנסיעה.</span><span class="sxs-lookup"><span data-stu-id="6c067-105">A travel requisition lists the expenses that will be incurred for the purpose of travel.</span></span> <span data-ttu-id="6c067-106">דרישת נסיעה מוגשת לבדיקה וניתן להשתמש בה כדי לאשר הוצאות.</span><span class="sxs-lookup"><span data-stu-id="6c067-106">A travel requisition is submitted for review and can be used to authorize expenses.</span></span>

<span data-ttu-id="6c067-107">ייתכן שתידרש להגיש דרישת נסיעה לפני ביצוע תשלום שנגבה מהארגון.</span><span class="sxs-lookup"><span data-stu-id="6c067-107">You may be required to submit a travel requisition before you incur any expense that is charged to the organization.</span></span> <span data-ttu-id="6c067-108">דרישה זו חלה, בין אם אתה מחייב את הארגון באמצעות כרטיס אשראי ארגוני שקיבלת, משלם במזומן שקיבלת כמקדמה או משלם מכיסך וגובה החזר מהארגון מאוחר יותר.</span><span class="sxs-lookup"><span data-stu-id="6c067-108">This requirement applies, regardless of whether you charge expenses to a corporate credit card, spend cash that you received from a cash advance, or incur out-of-pocket expenses that will be reimbursed by the organization.</span></span>

<span data-ttu-id="6c067-109">ניתן להשתמש בדרישות נסיעה ובמדיניות לגבי נסיעות כדי לנהל את הוצאות הארגון בצורה טובה יותר.</span><span class="sxs-lookup"><span data-stu-id="6c067-109">Travel requisitions and policies can be used to help manage organization expenditures.</span></span> <span data-ttu-id="6c067-110">למשל, נניח שהארגון עובד על פרוייקט במחיר קבוע אשר מחייב נסיעות – הוצאות הנסיעה של החברים בצוות הפרוייקט חייבות להיות כלולות בתקציב הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="6c067-110">For example, if your organization is working on a fixed-price project that requires travel, the travel expenses of the project's team members must fit within the project budget.</span></span> <span data-ttu-id="6c067-111">על ידי דרישה לאשר הוצאות נסיעה לפני שהן משולמות בפועל, הארגון יכול להבטיח שלא תהיה חריגה מהתקציב שהוקצה לפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="6c067-111">By requiring that travel expenses be approved before they are incurred, the organization can help make sure that the project remains within budget.</span></span>

## <a name="configuration"></a><span data-ttu-id="6c067-112">תצורה</span><span class="sxs-lookup"><span data-stu-id="6c067-112">Configuration</span></span> 

<span data-ttu-id="6c067-113">ניתן להגדיר דרישות נסיעה כ"חובה" על ידי הפעלת הפרמטר "מתן הרשאה מראש לנסיעה הוא חובה" בפרמטרי ניהול הוצאות.</span><span class="sxs-lookup"><span data-stu-id="6c067-113">Travel Requisitions can be configured as "mandatory" by enabling the "Pre-authorization of travel is mandatory" parameter in Expense Management Parameters.</span></span> 

## <a name="create-and-submit-a-travel-requisition"></a><span data-ttu-id="6c067-114">יצירה והגשה של דרישת נסיעה</span><span class="sxs-lookup"><span data-stu-id="6c067-114">Create and submit a travel requisition</span></span>

1. <span data-ttu-id="6c067-115">עבור אל **ההוצאות שלי: דרישת נסיעה** ובחר **דרישת נסיעה חדשה**.</span><span class="sxs-lookup"><span data-stu-id="6c067-115">Go to **My expenses: Travel Requisition**, and select **New travel Requisition**.</span></span>
2. <span data-ttu-id="6c067-116">הזן מטרה ויעד עבור דרישת הנסיעה.</span><span class="sxs-lookup"><span data-stu-id="6c067-116">Enter a purpose and destination for the requisition.</span></span>
3. <span data-ttu-id="6c067-117">בשדה **תיאור הנסיעה**, הזן פרטים נוספים, ככל שישנם כאלה.</span><span class="sxs-lookup"><span data-stu-id="6c067-117">In the  **Travel description** field, enter any additional information.</span></span> 
4. <span data-ttu-id="6c067-118">עבור כל אחת מההוצאות הצפויות, כגון טיסה, ארוחות או רכב שכור, יש ליצור פריט שורה של הוצאה.</span><span class="sxs-lookup"><span data-stu-id="6c067-118">For each of the expected expenses, such as Flight, meals, or car rental, create an expense line item.</span></span> <span data-ttu-id="6c067-119">עבור כל הוצאה, יש לכלול את התאריך המשוער, הסכום המשוער ומטבע התשלום.</span><span class="sxs-lookup"><span data-stu-id="6c067-119">Include the estimated date, estimated amount, and the currency for each expense.</span></span> 
5. <span data-ttu-id="6c067-120">לאחר הוספת ההוצאות הצפויות, בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="6c067-120">When you have finished adding the expected expenses, select **Save**.</span></span>
6. <span data-ttu-id="6c067-121">כאשר אתה מוכן להגשת דרישת הנסיעה, בחר **זרימת עבודה** > **שלח**.</span><span class="sxs-lookup"><span data-stu-id="6c067-121">When you are ready to submit the travel requisition, select **Workflow** > **Submit**.</span></span>

<span data-ttu-id="6c067-122">ניתן לצפות בדרישות הנסיעה שאושרו תחת **ההוצאות שלי: דרישת נסיעה**.</span><span class="sxs-lookup"><span data-stu-id="6c067-122">You can view your approved travel requisitions under **My Expenses: Travel Requisition**.</span></span> 

## <a name="view-available-travel-requisitions"></a><span data-ttu-id="6c067-123">הצגת דרישות נסיעה זמינות</span><span class="sxs-lookup"><span data-stu-id="6c067-123">View available travel requisitions</span></span>

<span data-ttu-id="6c067-124">ניתן לצפות בכל דרישות הנסיעה שלך תחת **ההוצאות שלי: דרישות נסיעה**.</span><span class="sxs-lookup"><span data-stu-id="6c067-124">You can view all of your travel requisitions under **My Expenses: Travel Requisitions**.</span></span>

## <a name="approve-travel-requisitions"></a><span data-ttu-id="6c067-125">אישור דרישות נסיעה</span><span class="sxs-lookup"><span data-stu-id="6c067-125">Approve travel requisitions</span></span>

<span data-ttu-id="6c067-126">בחר את דרישת הנסיעה שברצונך לאשר ואז בחר **זרימת עבודה** > **אישור**.</span><span class="sxs-lookup"><span data-stu-id="6c067-126">Select the travel requisition that you want to approve, and then select **Workflow** > **Approve**.</span></span>  

## <a name="submit-an-expense-report-using-your-approved-travel-requisition"></a><span data-ttu-id="6c067-127">הגשת דוח הוצאות באמצעות דרישת הנסיעה שאושרה</span><span class="sxs-lookup"><span data-stu-id="6c067-127">Submit an expense report using your approved travel requisition</span></span>

1. <span data-ttu-id="6c067-128">צור דוח הוצאות חדש. ברשימה של דרישות נסיעות שאושרו, בחר **מפה לדרישת נסיעה**.</span><span class="sxs-lookup"><span data-stu-id="6c067-128">Create a new expense report and in the expense report header, and from the list of approved travel requisitions, select **Map to Travel requisition**.</span></span>
2. <span data-ttu-id="6c067-129">השדה **סכום דרישת נסיעה** מתעדכן אוטומטית בכותרת של דוח ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="6c067-129">The **Travel requisition amount** field is automatically updated in the expense report header.</span></span>
3. <span data-ttu-id="6c067-130">הוסף כל הוצאה שהייתה בנסיעה.</span><span class="sxs-lookup"><span data-stu-id="6c067-130">Add each expense incurred for the trip.</span></span> <span data-ttu-id="6c067-131">אם השדה **אושר מראש** פעיל, הסכום בפועל והסכום שאושר בקטגוריית ההוצאות הספציפית יתעדכנו.</span><span class="sxs-lookup"><span data-stu-id="6c067-131">If the **Pre-authorized** field is enabled, the reconciled amount and authorized amount for the specific expense category will be updated.</span></span>

> [!NOTE]
> <span data-ttu-id="6c067-132">כשממפים דוח הוצאות לדרישת נסיעה שאושרה, סכום העסקה לא יכול להיות גדול מהסכום שאושר.</span><span class="sxs-lookup"><span data-stu-id="6c067-132">When you map an expense report to an approved travel requisition, the transaction amount can't be greater than the authorized amount.</span></span> 
