---
title: מדוע ברירת המחדל למחיר היא אפס עבור עלות זמן בפועל?
description: פתרון בעיות בנושא מדוע ברירת המחדל למחיר היא אפס עבור עלות הזמן בפועל.
author: rumant
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.prod: Project Service
ms.technology: ''
ms.assetid: 597d75b7-fadf-4947-8d52-95425ff90324
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 448c6c0569a40e1d7cb133561435811ecedb4356
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751910"
---
# <a name="why-is-the-price-defaulting-to-zero-on-time-cost-actuals"></a><span data-ttu-id="70c68-103">מדוע ברירת המחדל למחיר היא אפס עבור עלות זמן בפועל?</span><span class="sxs-lookup"><span data-stu-id="70c68-103">Why is the price defaulting to zero on time cost actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="70c68-104">שאלות נפוצות אלה דנות בנושא נתונים בפועל כאשר מחלקת התנועות מוגדרת כ'זמן' וסוג התנועה הוא 'עלות'.</span><span class="sxs-lookup"><span data-stu-id="70c68-104">This FAQ applies to actuals where the transaction class is set to Time and transaction type is Cost.</span></span> <span data-ttu-id="70c68-105">שלוש הבדיקות הבאות יסייעו לך להבין מדוע ברירת המחדל למחיר היא 0 עבור הוצאות הזמן בפועל.</span><span class="sxs-lookup"><span data-stu-id="70c68-105">The following three checks will help you troubleshoot why the price is defaulting to 0 on time cost actuals.</span></span>
 
## <a name="check-1-identify-the-cost-price-list-for-the-project"></a><span data-ttu-id="70c68-106">בדיקה 1: זיהוי מחירון העלות עבור הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="70c68-106">Check 1: Identify the cost price list for the project</span></span>

<span data-ttu-id="70c68-107">חפש את הפרוייקט משדה הפרוייקט של השעות בפועל ועבור אל דף הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="70c68-107">Find the project from the project field of the actual and then go to the project page.</span></span> <span data-ttu-id="70c68-108">לחץ על קישור יחידת החוזה בשדה.</span><span class="sxs-lookup"><span data-stu-id="70c68-108">Click on the contracting unit link in the field.</span></span> <span data-ttu-id="70c68-109">בדף יחידת החוזה, בדוק אם ליחידת החוזה יש מחירון ברשת 'מחירוני עלות'.</span><span class="sxs-lookup"><span data-stu-id="70c68-109">On the Contracting Unit page, check if the contracting unit has a price list in the Cost Price Lists grid.</span></span>

<span data-ttu-id="70c68-110">אם קיים יותר ממחירון אחד, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="70c68-110">If there is more than one price list, you have isolated the problem.</span></span> <span data-ttu-id="70c68-111">Project Service תומך רק במחירון אחד לכל יחידה ארגונית.</span><span class="sxs-lookup"><span data-stu-id="70c68-111">Project Service only supports one price list per organizational unit.</span></span> <span data-ttu-id="70c68-112">הסר את כל המחירונים מישות זו עד שיישאר מחירון אחד בלבד המצורף לרשת 'מחירוני עלות' של היחידה הארגונית.</span><span class="sxs-lookup"><span data-stu-id="70c68-112">Remove all prices lists from this entity until there is only one price list attached in the Cost Price Lists grid of the Organizational Unit.</span></span>

<span data-ttu-id="70c68-113">אם לא מצורפים מחירונים ליחידה הארגונית, רשום לעצמך את המטבע של היחידה הארגונית.</span><span class="sxs-lookup"><span data-stu-id="70c68-113">If there are no price lists attached to the Organizational Unit, make a note of the currency of the Organizational unit.</span></span> <span data-ttu-id="70c68-114">עבור אל Project Service ולאחר מכן אל 'פרמטרים' ופתח את הכרטיסיה 'מחירונים'. בדוק אם קיימים מחירונים כלשהם עם הקשר שמוגדר בתור 'עלות' ומטבע שתואם למטבע של היחידה הארגונית.</span><span class="sxs-lookup"><span data-stu-id="70c68-114">Go to the Project Service and then Parameters and open the Price Lists tab. Check if there are any price lists with context set to Cost and currency that matches the currency of the Organizational Unit.</span></span>
 
<span data-ttu-id="70c68-115">אם אין מחירונים שתואמים לקריטריונים אלה, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="70c68-115">If there are no price lists that match that criteria, you have isolated the problem.</span></span> <span data-ttu-id="70c68-116">ודא כי יש לפחות מחירון אחד שההקשר שלו מוגדר כ'עלות' ושהמטבע שלו תואם למטבע של היחידה הארגונית.</span><span class="sxs-lookup"><span data-stu-id="70c68-116">Make sure to have at least one price list whose context is set to Cost and whose currency matches the currency of the Organizational Unit.</span></span>

<span data-ttu-id="70c68-117">אם ישנו יותר ממחירון אחד שתואם לקריטריונים אלה, המשך לקרוא מסמך זה כדי לבצע בדיקות נוספות.</span><span class="sxs-lookup"><span data-stu-id="70c68-117">If there is more than one price list that match that criteria, continue reading this document to make more checks.</span></span>

## <a name="check-2-are-any-of-the-price-lists-identified-above-valid-for-the-specific-date-of-the-time-cost-actual"></a><span data-ttu-id="70c68-118">בדיקה 2: האם מחירון כלשהו מבין המחירונים שזוהו לעיל תקפים עבור התאריך המסוים של עלות הזמן בפועל?</span><span class="sxs-lookup"><span data-stu-id="70c68-118">Check 2: Are any of the price lists identified above valid for the specific date of the time cost actual?</span></span>

<span data-ttu-id="70c68-119">כדי ש- Project Service ישקול מחירון עבור מחיר ברירת מחדל, מחירון זה צריך להיות ישים עבור התאריך בעלות הזמן בפועל.</span><span class="sxs-lookup"><span data-stu-id="70c68-119">For Project Service to consider a price list for defaulting price, that price list should be applicable for the date on the time cost actual.</span></span> <span data-ttu-id="70c68-120">בדוק את הפרטים הבאים כדי לראות אם המחירונים שתוארו לעיל ישימים:</span><span class="sxs-lookup"><span data-stu-id="70c68-120">Check the following to see if the price list(s) identified above are applicable:</span></span>

- <span data-ttu-id="70c68-121">בדוק אם תאריכי ההתחלה והסיום בכרטיסיה 'כללי' עבור המחירונים המצורפים אינם ריקים.</span><span class="sxs-lookup"><span data-stu-id="70c68-121">Check if the start and end dates on the general tab for the price lists attached aren’t empty.</span></span> <span data-ttu-id="70c68-122">אם תאריכי ההתחלה והסיום עבור המחירונים שתוארו לעיל ריקים, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="70c68-122">If the start and end dates on price lists identified above are empty, you have isolated the problem.</span></span> 
- <span data-ttu-id="70c68-123">רשום לעצמך את שדה תאריך ההתחלה בעלות הזמן בפועל שלך ובדוק אם מחירון כלשהו מבין המחירונים שזוהו ישים עבור תאריך זה.</span><span class="sxs-lookup"><span data-stu-id="70c68-123">Make a note of the start date field on your time cost actual and check if any of the price lists identified is applicable for that date.</span></span> <span data-ttu-id="70c68-124">לדוגמה, תאריך עלות הזמן בפועל אמור להימצא בטווח תאריך התחלה ותאריך הסיום במחירון.</span><span class="sxs-lookup"><span data-stu-id="70c68-124">For example, the date of the time cost actual should fall within the start date and end date on the price list.</span></span> 
    - <span data-ttu-id="70c68-125">אם לא קיים מחירון המכסה תאריך זה בעלות הזמן בפועל, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="70c68-125">If there is no price list that covers that date on the time cost actual, you have isolated the problem.</span></span> <span data-ttu-id="70c68-126">שנה את תאריכי ההתחלה והסיום של המחירון כדי להבטיח שהמחירון מכסה את תאריך עלות הזמן בפועל.</span><span class="sxs-lookup"><span data-stu-id="70c68-126">Modify the start and end dates of the price list to ensure that the price list covers the date of the time cost actual.</span></span> 
    - <span data-ttu-id="70c68-127">אם קיים יותר ממחירון אחד המכסה את תאריך עלות הזמן בפועל, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="70c68-127">If there is more than one price list that covers the date on the time cost actual, you have isolated the problem.</span></span> <span data-ttu-id="70c68-128">באפשרותך לתקן זאת על-ידי עריכת תאריכי ההתחלה והסיום של המחירונים כך שיהיה מחירון אחד בלבד שמכסה את תאריך עלות הזמן בפועל.</span><span class="sxs-lookup"><span data-stu-id="70c68-128">You can fix this by editing the start and end dates of the price list(s) so that there is only one price list that covers the date of the time cost actual.</span></span> 
    - <span data-ttu-id="70c68-129">אם ישנו מחירון אחד בלבד שמכסה את התאריך של עלות הזמן בפועל, עבור לבדיקה הבאה במסמך.</span><span class="sxs-lookup"><span data-stu-id="70c68-129">If there is only one price list that covers that date of the time cost actual, move to the next check in the document.</span></span>
<span data-ttu-id="70c68-130">לאחר שביצעת את כל התיקונים הנדרשים, צור מחדש ערך זמן, אשר אותו, וודא שעלות הזמן בפועל מציגה מחיר חוקי.</span><span class="sxs-lookup"><span data-stu-id="70c68-130">Once you’ve done made the required fixes, recreate a time entry, approve it, and verify that the time cost actual shows a valid price.</span></span>

## <a name="check-3-is-there-a-price-in-the-price-list-for-the-pricing-dimensions-on-the-time-cost-actual"></a><span data-ttu-id="70c68-131">בדיקה 3: האם קיים מחיר במחירון עבור ממדי התמחור בעלות הזמן בפועל?</span><span class="sxs-lookup"><span data-stu-id="70c68-131">Check 3: Is there a price in the price list for the pricing dimensions on the time cost actual?</span></span>

<span data-ttu-id="70c68-132">אם השלמת בהצלחה בדיקה 1 ובדיקה 2, כעת צריך להיות לך מחירון אחד בלבד שישים עבור התאריך של עלות הזמן בפועל.</span><span class="sxs-lookup"><span data-stu-id="70c68-132">If you have successfully completed Check 1 and Check 2, you should now have only one price list that is applicable for the date of the time cost actual.</span></span> <span data-ttu-id="70c68-133">פתח מחירון זה ועבור אל הכרטיסיה 'מחירי תפקיד'. ודא שקיימת שורה ברשת עבור ממדי התמחור בעלות הזמן בפועל.</span><span class="sxs-lookup"><span data-stu-id="70c68-133">Open this Price List and go to the Role Prices tab. Make sure that there is a row in the grid for the pricing dimensions on the time cost actual.</span></span>

<span data-ttu-id="70c68-134">אם אין ברשת 'מחיר תפקיד' שורה עבור ממדי התמחור בעלות הזמן בפועל, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="70c68-134">If there is no row in the role price grid for the pricing dimensions on the time cost actual, then you have isolated the problem.</span></span> <span data-ttu-id="70c68-135">צור שורה ברשת 'מחירי תפקיד' עבור ממדי התמחור בעלות הזמן בפועל.</span><span class="sxs-lookup"><span data-stu-id="70c68-135">Create a row in the Role prices grid for the pricing dimensions on your time cost actual.</span></span> <span data-ttu-id="70c68-136">לאחר שביצעת זאת, צור מחדש ערך זמן, אשר אותו, וודא שעלות הזמן בפועל מציגה מחיר חוקי.</span><span class="sxs-lookup"><span data-stu-id="70c68-136">Once this is done, recreate time entry, approve it, and verify that the time cost actual shows a valid price.</span></span>
 
<span data-ttu-id="70c68-137">אם עדיין אינך רואה מחיר חוקי בעלות הזמן בפועל שלך לאחר ביצוע שלוש הבדיקות לעיל, צור כרטיס תמיכה.</span><span class="sxs-lookup"><span data-stu-id="70c68-137">If you still don't see a valid price on your time cost actual after you’ve done the three checks above, please log a support ticket.</span></span>



