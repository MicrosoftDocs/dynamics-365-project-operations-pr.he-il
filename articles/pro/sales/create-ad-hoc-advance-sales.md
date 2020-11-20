---
title: יצירת מקדמה אד הוק על חוזה - לייט
description: נושא זה מספק מידע על יצירת מקדמה במזומן על חוזה לפי הצורך.
author: rumant
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a6bf02c2e2ab2f3c696b1eab1b92a20272187bf5
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181363"
---
# <a name="creating-an-ad-hoc-advance-on-a-contract---lite"></a><span data-ttu-id="067e7-103">יצירת מקדמה אד הוק על חוזה - לייט</span><span class="sxs-lookup"><span data-stu-id="067e7-103">Creating an ad hoc advance on a contract - lite</span></span>

<span data-ttu-id="067e7-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="067e7-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="067e7-105"> Microsoft Dynamics 365 Project Operations ‏תומך בתרחישים של חשבוניות הכוללים תשלומים מקדמים ומקדמות.</span><span class="sxs-lookup"><span data-stu-id="067e7-105">Microsoft Dynamics 365 Project Operations supports invoicing scenarios that involve pre-payments and advances.</span></span> <span data-ttu-id="067e7-106">תהליך השימוש ב **מקדמות במזומן** ב-**Project Operations** דומה לחוזי **ריטיינר**.</span><span class="sxs-lookup"><span data-stu-id="067e7-106">The process for using **Advances** in **Project Operations** is similar to **Retainer** contracts.</span></span> 

<span data-ttu-id="067e7-107">בצע את השלבים הבאים כדי להגיש ללקוח חשבונית על מקדמה במזומן.</span><span class="sxs-lookup"><span data-stu-id="067e7-107">Complete the following steps to invoice the customer for an advance.</span></span>

1. <span data-ttu-id="067e7-108">עבור אל הדף **חוזה פרויקט** ולאחר מכן בחר את הכרטיסיה **מקדמות במזומן וריטיינרים**.</span><span class="sxs-lookup"><span data-stu-id="067e7-108">Go to the **Project Contract** page, and then select the **Advances and Retainers** tab.</span></span>
2. <span data-ttu-id="067e7-109">ברשת-המשנה המפרטת את כל המקדמות במזומן ותשלומי המקדמה שנרשמו בעבר, בחר **+ ריטיינר חדש לחוזה פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="067e7-109">In the subgrid that lists all the previously recorded advances and prepayments, select **+ New Project contract retainer**.</span></span> 

    <span data-ttu-id="067e7-110">הטופס **יצירה מהירה** נפתח לרישום של תשלום מקדמה או מקדמה במזומן.</span><span class="sxs-lookup"><span data-stu-id="067e7-110">The **Quick Create** form opens for recording a prepayment or advance.</span></span>
    
3. <span data-ttu-id="067e7-111">הטבלה שלהלן מפרטת את השדות לרישום מקדמה במזומן ואת השיקולים שיש לקחת בחשבון בעת יצירת מקדמות חדשות:</span><span class="sxs-lookup"><span data-stu-id="067e7-111">The table below lists the fields for recording an advance and the considerations to keep in mind as you create new ones:</span></span>

    | <span data-ttu-id="067e7-112">שדה</span><span class="sxs-lookup"><span data-stu-id="067e7-112">Field</span></span> | <span data-ttu-id="067e7-113">תיאור</span><span class="sxs-lookup"><span data-stu-id="067e7-113">Description</span></span> | <span data-ttu-id="067e7-114">השפעה במורד הזרם</span><span class="sxs-lookup"><span data-stu-id="067e7-114">Downstream impact</span></span> |
    | --- | --- | --- |
    | <span data-ttu-id="067e7-115">**לקוח חוזה הפרויקט**</span><span class="sxs-lookup"><span data-stu-id="067e7-115">**Project Contract Customer**</span></span> | <span data-ttu-id="067e7-116">שדה זה מציין לאיזה לקוח בחוזה יוגש חשבונית בגין מקדמה במזומן זו.</span><span class="sxs-lookup"><span data-stu-id="067e7-116">This field indicates which customer on the contract will be invoiced for this advance.</span></span> | <span data-ttu-id="067e7-117">אם יש לך מספר לקוחות בחוזה וברצונך לחייב כל אחד מהם עבור ריטיינר או סכום של מקדמה במזומן ספציפי, צור מקדמה במזומן עבור כל לקוח בנפרד.</span><span class="sxs-lookup"><span data-stu-id="067e7-117">If you have multiple customers on the contract and want to invoice each of them for a specific retainer or advance amount, create an advance for each customer individually.</span></span> |
    | <span data-ttu-id="067e7-118">**תיאור**</span><span class="sxs-lookup"><span data-stu-id="067e7-118">**Description**</span></span> | <span data-ttu-id="067e7-119">תיאור המטרה או העיתוי של המקדמה במזומן בכדי לסייע בזיהוי מקדמה במזומן זו.</span><span class="sxs-lookup"><span data-stu-id="067e7-119">The description of the purpose or timing of the advance to help identify this advance.</span></span> | <span data-ttu-id="067e7-120">תיאור זה מוצג בשורת החשבונית בגין מקדמה במזומן זו.</span><span class="sxs-lookup"><span data-stu-id="067e7-120">This description is displayed on the invoice line for this advance.</span></span> |
    | <span data-ttu-id="067e7-121">**סכום**</span><span class="sxs-lookup"><span data-stu-id="067e7-121">**Amount**</span></span> | <span data-ttu-id="067e7-122">סכום תשלום המקדמה או המקדמה במזומן.</span><span class="sxs-lookup"><span data-stu-id="067e7-122">The amount for the pre-payment or advance.</span></span> | <span data-ttu-id="067e7-123">סכום זה מוצג בשורת החשבונית בגין מקדמה במזומן זו.</span><span class="sxs-lookup"><span data-stu-id="067e7-123">This amount is displayed on the invoice line for this advance.</span></span> |
    | <span data-ttu-id="067e7-124">**תאריך חשבונית**</span><span class="sxs-lookup"><span data-stu-id="067e7-124">**Invoice Date**</span></span> | <span data-ttu-id="067e7-125">המועד בו מוגש חשבונית הלקוח עבור מקדמה במזומן זו.</span><span class="sxs-lookup"><span data-stu-id="067e7-125">The date on which this advance is invoiced to the customer.</span></span> | <span data-ttu-id="067e7-126">זהו התאריך לתהליך יצירת החשבונית האוטומטית ליצירת שורת חשבונית עבור מקדמה במזומן זו.</span><span class="sxs-lookup"><span data-stu-id="067e7-126">This is the date for the automated invoice creation process to create an invoice line for this advance.</span></span> |
    | <span data-ttu-id="067e7-127">**מצב חשבונית**</span><span class="sxs-lookup"><span data-stu-id="067e7-127">**Invoice Status**</span></span> | <span data-ttu-id="067e7-128">זוהי הגדרת אפשרות המציינת אם מקדמה במזומן זו מתווספת לטיוטת חשבונית עבור לקוח זה.</span><span class="sxs-lookup"><span data-stu-id="067e7-128">This is an option setting that indicates whether this advance is added to a draft invoice for this customer.</span></span> <span data-ttu-id="067e7-129">הערכים האפשריים הם:</span><span class="sxs-lookup"><span data-stu-id="067e7-129">The possible values are:</span></span></br><span data-ttu-id="067e7-130">- **לא מוכן להגיש חשבונית**</span><span class="sxs-lookup"><span data-stu-id="067e7-130">- **Not ready to invoice**</span></span></br><span data-ttu-id="067e7-131">- **מוכן להגיש חשבונית**</span><span class="sxs-lookup"><span data-stu-id="067e7-131">- **Ready to invoice**</span></span> | <span data-ttu-id="067e7-132">כאשר מקדמה במזומן או תשלום מקדמה מסומנים כ **מוכן להגשת חשבונית**, הוא מתווסף כשעת שורה בחשבונית טיוטה.</span><span class="sxs-lookup"><span data-stu-id="067e7-132">When an advance or pre-payment is marked as **Ready to invoice**, it is added as a line time on a draft invoice.</span></span> <span data-ttu-id="067e7-133">ניתן להשתמש רק במקדמה במזומן שחויבה במלואה להתאמה מול עלויות הפרויקט לתקופת החשבונית הבאה.</span><span class="sxs-lookup"><span data-stu-id="067e7-133">Only a fully invoiced advance can be used to reconcile against project costs for the next invoice period.</span></span> |

4. <span data-ttu-id="067e7-134">בחר **שמור וסגור** בתיבת הדו-שיח יצירה מהירה כדי לרשום את המקדמה במזומן או את תשלום המקדמה.</span><span class="sxs-lookup"><span data-stu-id="067e7-134">Select **Save and close** on the quick create dialog to record the advance or the pre-payment.</span></span>
