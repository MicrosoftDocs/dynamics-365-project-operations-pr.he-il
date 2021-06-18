---
title: מדוע ברירת המחדל למחיר היא אפס עבור מכירות זמן בפועל?
description: פתרון בעיות בנושא מדוע ברירת המחדל למחיר היא אפס עבור מכירות הזמן בפועל.
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: e32b4c8113afdc18d9b220b1a8daf5007be93ac8
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6011642"
---
# <a name="why-is-price-defaulting-to-zero-on-time-sales-actuals"></a><span data-ttu-id="91ea2-103">מדוע ברירת המחדל למחיר היא אפס עבור מכירות זמן בפועל?</span><span class="sxs-lookup"><span data-stu-id="91ea2-103">Why is price defaulting to zero on time sales actuals?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="91ea2-104">שאלות נפוצות אלה דנות בנושא ההוצאות בפועל כאשר מחלקת התנועות מוגדרת כ'זמן' וסוג התנועה הוא '‏‫מכירות שלא חויבו‬'.</span><span class="sxs-lookup"><span data-stu-id="91ea2-104">This FAQ applies to actuals where the transaction class is set to Time and transaction type is Unbilled Sales.</span></span> <span data-ttu-id="91ea2-105">שלוש הבדיקות הבאות יסייעו לך להבין מדוע ברירת המחדל למחיר (‏‫תעריף חיוב‬) היא 0 עבור מכירות הזמן בפועל.</span><span class="sxs-lookup"><span data-stu-id="91ea2-105">The following three checks will help you troubleshoot why price (bill rate) is defaulting to 0 on time sales actuals.</span></span>

## <a name="check-1-identify-the-sales-price-list-for-the-project"></a><span data-ttu-id="91ea2-106">בדיקה 1: זיהוי מחירון מכירות עבור הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="91ea2-106">Check 1: Identify the sales price list for the project</span></span>

<span data-ttu-id="91ea2-107">חפש את הפרוייקט משדה הפרוייקט של השעות בפועל ועבור אל דף הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="91ea2-107">Find the project from the project field of the actual and go to the project page.</span></span> <span data-ttu-id="91ea2-108">לאחר מכן עבור אל הכרטיסיה 'מכירות', וברשת 'סעיפי חוזה של פרוייקט', לחץ על הקישור בשדה חוזה הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="91ea2-108">Then go to the Sales tab and on Project Contract lines grid, click on the link in the Project Contract field.</span></span> <span data-ttu-id="91ea2-109">ייפתח דף חוזה הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="91ea2-109">The project Contract page will open.</span></span> <span data-ttu-id="91ea2-110">בדף חוזה הפרוייקט, עבור אל הכרטיסיה 'מחירוני פרוייקט'. בדוק אם קיים לפחות מחירון אחד המצורף כאן.</span><span class="sxs-lookup"><span data-stu-id="91ea2-110">On the Project Contract page, go to the Project Price Lists tab. Check if there is at least one price list attached here.</span></span> <span data-ttu-id="91ea2-111">אם לא מצורף מחירון ברשת 'מחירוני פרוייקט' של חוזה הפרוייקט, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="91ea2-111">If there is no price list attached in the Project Price Lists grid of the Project Contract you have isolated the problem.</span></span> <span data-ttu-id="91ea2-112">צרף מחירון לרשת 'מחירוני פרוייקט'.</span><span class="sxs-lookup"><span data-stu-id="91ea2-112">Attach a price list to the Project Price lists grid.</span></span> <span data-ttu-id="91ea2-113">במחירונים שמותר לצרף כאן שדה ההקשר צריך להיות מוגדר בתור 'מכירות' ושדה המטבע במחירון אמור להתאים לשדה המטבע בחוזה הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="91ea2-113">The price lists allowed to be attached here should have the context field set to Sales and the currency field on the price list should match the currency field on the Project Contract.</span></span> <span data-ttu-id="91ea2-114">לאחר שביצעת את כל התיקונים הנדרשים, צור מחדש ערך זמן, אשר אותו, ווודא שהנתונים בפועל של המכירות שלא חויבו מציגים מחיר חוקי.</span><span class="sxs-lookup"><span data-stu-id="91ea2-114">Once you’ve done made the required fixes, recreate a time entry, approve it, and verify that the unbilled sales actual shows a valid price.</span></span> 

<span data-ttu-id="91ea2-115">אם יש לך מחירון אחד או יותר שמצורפים לרשת 'מחירוני פרוייקט' של חוזה הפרוייקט, עבור לבדיקה הבאה במסמך.</span><span class="sxs-lookup"><span data-stu-id="91ea2-115">If you have one or more price lists attached in the Project Price Lists grid of the Project Contract, proceed to the next check in the document.</span></span>

## <a name="check-2-are-any-of-the-price-lists-identified-above-valid-for-the-specific-date-of-the-time-sales-actual"></a><span data-ttu-id="91ea2-116">בדיקה 2: האם מחירון כלשהו מבין המחירונים שזוהו לעיל תקפים עבור התאריך המסוים של מכירות הזמן בפועל?</span><span class="sxs-lookup"><span data-stu-id="91ea2-116">Check 2: Are any of the price lists identified above valid for the specific date of the time sales actual?</span></span>

<span data-ttu-id="91ea2-117">כדי ש- Project Service ישקול מחירון עבור מחיר ברירת מחדל, מחירון זה צריך להיות ישים עבור התאריך במכירות הזמן בפועל.</span><span class="sxs-lookup"><span data-stu-id="91ea2-117">For Project Service to consider a price list for defaulting price, that price list should be applicable for the date on the time sales actual.</span></span> <span data-ttu-id="91ea2-118">בדוק את הפרטים הבאים כדי לראות אם המחירונים שתוארו לעיל ישימים:</span><span class="sxs-lookup"><span data-stu-id="91ea2-118">Check the following to see if the price list(s) identified above are applicable:</span></span>
- <span data-ttu-id="91ea2-119">בדוק אם תאריכי ההתחלה והסיום בכרטיסיה 'כללי' עבור המחירונים המצורפים אינם ריקים.</span><span class="sxs-lookup"><span data-stu-id="91ea2-119">Check if the start and end dates on the general tab for the price lists attached aren’t empty.</span></span> <span data-ttu-id="91ea2-120">אם תאריכי ההתחלה והסיום עבור המחירונים שתוארו לעיל ריקים, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="91ea2-120">If the start and end dates on price lists identified above are empty, you have isolated the problem.</span></span> 
- <span data-ttu-id="91ea2-121">רשום לעצמך את שדה תאריך ההתחלה במכירות הזמן בפועל שלך ובדוק אם מחירון כלשהו מבין המחירונים שזוהו ישים עבור תאריך זה.</span><span class="sxs-lookup"><span data-stu-id="91ea2-121">Make a note of the start date field on your time sales actual and check if any of the price lists identified is applicable for that date.</span></span> <span data-ttu-id="91ea2-122">לדוגמה, תאריך מכירות הזמן בפועל אמור להימצא בטווח תאריך התחלה ותאריך הסיום במחירון.</span><span class="sxs-lookup"><span data-stu-id="91ea2-122">For example, the date of the time sales actual should fall within the start date and end date on the price list.</span></span> 
    - <span data-ttu-id="91ea2-123">אם לא קיים מחירון המכסה תאריך זה במכירות הזמן בפועל, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="91ea2-123">If there is no price list that covers that date on the time sales actual, you have isolated the problem.</span></span> <span data-ttu-id="91ea2-124">שנה את תאריכי ההתחלה והסיום של המחירון כדי להבטיח שהמחירון מכסה את תאריך מכירות הזמן בפועל.</span><span class="sxs-lookup"><span data-stu-id="91ea2-124">Modify the start and end dates of the price list to ensure that the price list covers the date of the time sales actual.</span></span> 
    - <span data-ttu-id="91ea2-125">אם קיים יותר ממחירון אחד המכסה את תאריך מכירות הזמן בפועל, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="91ea2-125">If there is more than one price list that covers the date on the time sales actual, you have isolated the problem.</span></span> <span data-ttu-id="91ea2-126">באפשרותך לתקן זאת על-ידי עריכת תאריכי ההתחלה והסיום של המחירונים כך שיהיה מחירון אחד בלבד שמכסה את תאריך מכירות הזמן בפועל.</span><span class="sxs-lookup"><span data-stu-id="91ea2-126">You can fix this by editing the start and end dates of the price list(s) so that there is only one price list that covers the date of the time sales actual.</span></span> 
    - <span data-ttu-id="91ea2-127">אם ישנו מחירון אחד בלבד שמכסה את תאריך מכירות הזמן בפועל, עבור לבדיקה 3.</span><span class="sxs-lookup"><span data-stu-id="91ea2-127">If there is only one price list that covers that date of the time sales actual, go to Check 3.</span></span>
<span data-ttu-id="91ea2-128">לאחר שביצעת את כל התיקונים הנדרשים, צור מחדש ערך זמן, אשר אותו, וודא שמכירות הזמן בפועל מציגות מחיר חוקי.</span><span class="sxs-lookup"><span data-stu-id="91ea2-128">Once you’ve done made the required fixes, recreate a time entry, approve it, and verify that the time sales actual shows a valid price.</span></span>

## <a name="check-3-is-there-a-price-in-the-price-list-for-the-pricing-dimensions-on-the-time-sales-actual"></a><span data-ttu-id="91ea2-129">בדיקה 3: האם קיים מחיר במחירון עבור ממדי התמחור במכירות הזמן בפועל?</span><span class="sxs-lookup"><span data-stu-id="91ea2-129">Check 3: Is there a price in the price list for the pricing dimensions on the time sales actual?</span></span>

<span data-ttu-id="91ea2-130">אם השלמת בהצלחה בדיקה 1 ובדיקה 2, כעת צריך להיות לך מחירון אחד בלבד שישים עבור התאריך של מכירות הזמן בפועל.</span><span class="sxs-lookup"><span data-stu-id="91ea2-130">If you have successfully completed Check 1 and Check 2, you should now have only one price list that is applicable for the date of the time sales actual.</span></span> <span data-ttu-id="91ea2-131">פתח מחירון זה ונווט אל הכרטיסיה 'מחירי תפקיד'. ודא שקיימת שורה ברשת עבור ממדי התמחור במכירות הזמן בפועל.</span><span class="sxs-lookup"><span data-stu-id="91ea2-131">Open this Price List and navigate to the Role Prices tab. Make sure that there is a row in the grid for the pricing dimensions on the Time sales actual.</span></span>

<span data-ttu-id="91ea2-132">אם אין ברשת 'מחיר תפקיד' שורה עבור ממדי התמחור במכירות הזמן בפועל, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="91ea2-132">If there is no row in the role price grid for the pricing dimensions on the time sales actual, then you have isolated the problem.</span></span> <span data-ttu-id="91ea2-133">צור שורה ברשת 'מחירי תפקיד' עבור ממדי התמחור במכירות הזמן בפועל.</span><span class="sxs-lookup"><span data-stu-id="91ea2-133">Create a row in the Role prices grid for the pricing dimensions on your time sales actual.</span></span> <span data-ttu-id="91ea2-134">לאחר שביצעת זאת, צור מחדש ערך זמן, אשר אותו, וודא שמכירות הזמן בפועל מציגות מחיר חוקי.</span><span class="sxs-lookup"><span data-stu-id="91ea2-134">Once this is done, recreate time entry, approve it, and verify that the time sales actual shows a valid price.</span></span>

<span data-ttu-id="91ea2-135">אם עדיין אינך רואה מחיר חוקי במכירות הזמן בפועל שלך לאחר ביצוע שלוש הבדיקות לעיל, צור כרטיס תמיכה.</span><span class="sxs-lookup"><span data-stu-id="91ea2-135">If you still don't see a valid price on your time sales actual after following the three checks above, please log a support ticket.</span></span> 



[!INCLUDE[footer-include](../includes/footer-banner.md)]