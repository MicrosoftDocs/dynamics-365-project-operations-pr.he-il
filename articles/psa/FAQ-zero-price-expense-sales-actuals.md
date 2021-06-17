---
title: מדוע ברירת המחדל למחיר היא אפס עבור הוצאות המכירות בפועל?
description: שלוש הבדיקות הבאות יסייעו לך להבין מדוע ברירת המחדל למחיר היא 0 עבור הוצאות מכירות בפועל.
author: rumant
ms.prod: ''
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
ms.openlocfilehash: 92b507d8e5605c01f1a9235233b3cd2885070749
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993012"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-sales-actuals"></a><span data-ttu-id="255f1-103">מדוע ברירת המחדל למחיר היא אפס עבור הוצאות המכירות בפועל?</span><span class="sxs-lookup"><span data-stu-id="255f1-103">Why is the price defaulting to zero on expense sales actuals?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="255f1-104">שאלות נפוצות אלה דנות בנושא ההוצאות בפועל כאשר מחלקת התנועות מוגדרת כ'הוצאה' וסוג התנועה הוא '‏‫מכירות שלא חויבו‬'.</span><span class="sxs-lookup"><span data-stu-id="255f1-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Unbilled Sales.</span></span> <span data-ttu-id="255f1-105">שלוש הבדיקות הבאות יסייעו לך להבין מדוע ברירת המחדל למחיר (‏‫תעריף חיוב‬) היא 0 עבור הוצאות מכירות בפועל.</span><span class="sxs-lookup"><span data-stu-id="255f1-105">The following three checks will help you troubleshoot why price (bill rate) is defaulting to 0 on expense sales actuals.</span></span>

## <a name="check-1-identify-the-sales-price-list-for-project"></a><span data-ttu-id="255f1-106">בדיקה 1: זיהוי מחירון מכירות עבור פרוייקט</span><span class="sxs-lookup"><span data-stu-id="255f1-106">Check 1: Identify the sales price list for project</span></span>

<span data-ttu-id="255f1-107">חפש את הפרוייקט משדה הפרוייקט של השעות בפועל ועבור אל דף הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="255f1-107">Find the project from the project field of the actual and go to the project page.</span></span> <span data-ttu-id="255f1-108">לאחר מכן עבור אל הכרטיסיה 'מכירות'. ברשת 'סעיפי חוזה של פרוייקט', לחץ על הקישור בשדה חוזה הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="255f1-108">Then go to the Sales tab. On the Project Contract lines grid, click on the link in the Project Contract field.</span></span> <span data-ttu-id="255f1-109">ייפתח דף חוזה הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="255f1-109">The Project Contract page will open.</span></span> <span data-ttu-id="255f1-110">בדף חוזה הפרוייקט, עבור אל הכרטיסיה 'מחירוני פרוייקט'. בדוק אם קיים לפחות מחירון אחד המצורף כאן.</span><span class="sxs-lookup"><span data-stu-id="255f1-110">On the Project Contract page, go to the Project Price Lists tab. Check if there is at least one price list attached here.</span></span>

<span data-ttu-id="255f1-111">אם לא מצורף מחירון ברשת 'מחירוני פרוייקט' של חוזה הפרוייקט:</span><span class="sxs-lookup"><span data-stu-id="255f1-111">If there is no price list attached in the Project Price Lists grid of the Project Contract:</span></span>

- <span data-ttu-id="255f1-112">צרף מחירון לרשת 'מחירוני פרוייקט'.</span><span class="sxs-lookup"><span data-stu-id="255f1-112">Attach a price list to the Project Price lists grid.</span></span> <span data-ttu-id="255f1-113">במחירונים שמותר לצרף כאן שדה ההקשר צריך להיות מוגדר בתור 'מכירות' ושדה המטבע במחירון אמור להתאים לשדה המטבע בחוזה הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="255f1-113">The price lists allowed to be attached here should have the context field set to Sales and the currency field on the price list should match the currency field on the Project Contract.</span></span> <span data-ttu-id="255f1-114">לאחר שביצעת את כל התיקונים הנדרשים, צור מחדש ערך הוצאות, אשר אותו, ווודא שהנתונים בפועל של המכירות שלא חויבו מציגים מחיר חוקי.</span><span class="sxs-lookup"><span data-stu-id="255f1-114">Once you’ve made the required fixes, recreate an expense entry, approve it, and verify that the unbilled sales actual shows a valid price.</span></span>
- <span data-ttu-id="255f1-115">אם יש לך מחירון אחד או יותר שמצורפים לרשת 'מחירוני פרוייקט' של חוזה הפרוייקט, עבור לבדיקה 2.</span><span class="sxs-lookup"><span data-stu-id="255f1-115">If you have one or more price lists attached in the Project Price Lists grid of the Project Contract, go to Check 2.</span></span>

## <a name="check-2-are-any-of-the-price-lists-identified-above-valid-for-the-specific-date-of-the-expense-actual"></a><span data-ttu-id="255f1-116">בדיקה 2: האם מחירון כלשהו מבין המחירונים שזוהו לעיל תקפים עבור התאריך המסוים של הוצאות בפועל?</span><span class="sxs-lookup"><span data-stu-id="255f1-116">Check 2: Are any of the price lists identified above valid for the specific date of the expense actual?</span></span>

<span data-ttu-id="255f1-117">כדי ש- Project Service ישקול מחירון עבור מחיר ברירת מחדל, מחירון זה צריך להיות ישים עבור התאריך בהוצאות המכירות בפועל.</span><span class="sxs-lookup"><span data-stu-id="255f1-117">For Project Service to consider a price list for defaulting price, that price list should be applicable for the date on the expense sales actual.</span></span> <span data-ttu-id="255f1-118">בדוק את הפרטים הבאים כדי לראות אם המחירונים שתוארו לעיל ישימים:</span><span class="sxs-lookup"><span data-stu-id="255f1-118">Check the following to see if the price list(s) identified above are applicable:</span></span>

- <span data-ttu-id="255f1-119">התחל על-ידי בדיקה אם תאריכי ההתחלה והסיום בכרטיסיה 'כללי' עבור המחירונים המצורפים אינם ריקים.</span><span class="sxs-lookup"><span data-stu-id="255f1-119">Start by checking if start and end dates on the general tab for the price lists attached aren’t empty.</span></span> <span data-ttu-id="255f1-120">אם תאריכי ההתחלה והסיום עבור המחירונים שתוארו לעיל ריקים, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="255f1-120">If the start and end dates on the price lists identified above are empty, you have isolated the problem.</span></span> 
- <span data-ttu-id="255f1-121">רשום לעצמך את שדה תאריך ההתחלה בהוצאות המכירות בפועל שלך ובדוק אם מחירון כלשהו מבין המחירונים שזוהו ישים עבור תאריך זה.</span><span class="sxs-lookup"><span data-stu-id="255f1-121">Make a note of the start date field on your expense sales actual and check if any of the price lists identified is applicable for that date.</span></span> <span data-ttu-id="255f1-122">לדוגמה, תאריך ההוצאה בפועל אמור להימצא בטווח תאריך התחלה ותאריך הסיום במחירון.</span><span class="sxs-lookup"><span data-stu-id="255f1-122">For example, the date of the expense actual should fall within the start date and end date on the price list.</span></span> 
    - <span data-ttu-id="255f1-123">אם לא קיים מחירון המכסה תאריך זה בהוצאות מכירות בפועל, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="255f1-123">If there is no price list that covers that date on the expense sales actual, you have isolated the problem.</span></span> <span data-ttu-id="255f1-124">שנה את תאריכי ההתחלה והסיום של המחירון כדי להבטיח שהמחירון מכסה את תאריך ההוצאה בפועל.</span><span class="sxs-lookup"><span data-stu-id="255f1-124">Modify the start and end dates of the price list to ensure that the price list covers the date of the expense actual.</span></span> 
    - <span data-ttu-id="255f1-125">אם קיים יותר ממחירון אחד המכסה את תאריך הוצאות המכירות בפועל, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="255f1-125">If there is more than one price list that covers the date on the expense sales actual, you have isolated the problem.</span></span> <span data-ttu-id="255f1-126">ערוך את תאריכי ההתחלה והסיום של המחירונים כך שיהיה מחירון אחד בלבד שמכסה את תאריך ההוצאה בפועל.</span><span class="sxs-lookup"><span data-stu-id="255f1-126">Edit the start and end dates of the price list(s) so that there is only one price list that covers the date of the expense actual.</span></span> 
    - <span data-ttu-id="255f1-127">אם ישנו מחירון אחד בלבד שמכסה את תאריך ההוצאה בפועל, עבור לבדיקה 3.</span><span class="sxs-lookup"><span data-stu-id="255f1-127">If there is only one price list that covers that date of the expense actual, move to Check 3.</span></span>
<span data-ttu-id="255f1-128">לאחר שביצעת את כל התיקונים הנדרשים, צור מחדש ערך הוצאות, אשר אותו, ווודא שהנתונים בפועל של המכירות שלא חויבו מציגים מחיר חוקי.</span><span class="sxs-lookup"><span data-stu-id="255f1-128">Once you’ve done made the required fixes, recreate an expense entry, approve it, and verify that the unbilled sales actual shows a valid price.</span></span>

## <a name="check-3-is-there-a-valid-price-for-the-expense-category-in-the-applicable-project-price-list"></a><span data-ttu-id="255f1-129">בדיקה 3: האם יש מחיר חוקי עבור קטגוריית ההוצאות במחירון הפרוייקט הישים?</span><span class="sxs-lookup"><span data-stu-id="255f1-129">Check 3: Is there a valid price for the expense category in the applicable project price list?</span></span> 

<span data-ttu-id="255f1-130">אם השלמת בהצלחה בדיקה 1 ובדיקה 2, כעת צריך להיות לך מחירון אחד בלבד של פרוייקט שישים עבור התאריך של הוצאות המכירות בפועל.</span><span class="sxs-lookup"><span data-stu-id="255f1-130">If you have successfully completed Check 1 and Check 2, you should now have only one project price list that is applicable for the date of the expense sales actual.</span></span> <span data-ttu-id="255f1-131">פתח את מחירון פרוייקט זה ועבור אל הכרטיסיה 'מחירי קטגוריה'. ודא שקיימת שורה ברשת עבור קטגוריית ההוצאות הספציפית בהוצאה בפועל.</span><span class="sxs-lookup"><span data-stu-id="255f1-131">Open this Project Price List and go to the Category Prices tab. Make sure that there is a row in the grid for the specific expense category on the Expense actual.</span></span>
 
- <span data-ttu-id="255f1-132">אם אין שורה, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="255f1-132">If there is no row, then you have isolated the problem.</span></span> <span data-ttu-id="255f1-133">צור שורה ברשת 'מחיר קטגוריה' עבור הקטגוריה בהוצאות בפועל שלך.</span><span class="sxs-lookup"><span data-stu-id="255f1-133">Create a row in the Category price grid for the category on your expense actual.</span></span> <span data-ttu-id="255f1-134">לאחר מכן צור מחדש ערך הוצאות, אשר אותו, ווודא שהנתונים בפועל של המכירות שלא חויבו מציגים מחיר חוקי.</span><span class="sxs-lookup"><span data-stu-id="255f1-134">Then, recreate an expense entry, approve it, and verify that the unbilled sales actual shows a valid price.</span></span> 
- <span data-ttu-id="255f1-135">אם יש שורה עבור קטגוריית הוצאות ברשת 'מחירי קטגוריה', בדוק אם יש לה מחיר חוקי.</span><span class="sxs-lookup"><span data-stu-id="255f1-135">If there is a row for the expense category in the category prices grid, check if it has a valid price.</span></span>

<span data-ttu-id="255f1-136">כדי להבין מה הוא מחיר חוקי, השתמש באחת מהשיטות הבאות:</span><span class="sxs-lookup"><span data-stu-id="255f1-136">To understand what a valid price is, use these methods:</span></span>

- <span data-ttu-id="255f1-137">אם השדה 'שיטת תמחור' בשורת מחיר 'קטגוריה' מוגדר בתור 'לפי עלות', שיעור היחידה בהוצאות המכירות בפועל שלך הופך כברירת מחדל לערך בהוצאה.</span><span class="sxs-lookup"><span data-stu-id="255f1-137">If the Pricing Method field on the Category price line is set to At Cost, then the unit rate on your Expense sales actual will be defaulted to the value in the Expense entry.</span></span>
- <span data-ttu-id="255f1-138">אם השדה 'שיטת תמחור' בשורת המחיר 'קטגוריה' מוגדר בתור 'אחוזי ייקור', בדוק אם שדה האחוז מוגדר לערך חוקי.</span><span class="sxs-lookup"><span data-stu-id="255f1-138">If the Pricing Method field on the Category price line is set to Markup Percentage, then check if the Percent field is set to a valid value.</span></span> <span data-ttu-id="255f1-139">שיעור היחידה בהוצאות המכירות בפועל שלך מוגדר כברירת מחדל על-ידי החלת אחוז ייקור זה על המחיר בערך ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="255f1-139">The unit rate on your Expense sales actual is defaulted by applying this markup percent to the price in the Expense entry.</span></span>
- <span data-ttu-id="255f1-140">אם השדה 'שיטת תמחור' בשורת המחיר 'קטגוריה' מוגדר בתור '‏‫מחיר ליחידה‬', בדוק אם שדה המחיר מוגדר לערך חוקי.</span><span class="sxs-lookup"><span data-stu-id="255f1-140">If the Pricing Method field on the Category price line is set to Price per Unit, then check if the Price field is set to a valid value.</span></span> <span data-ttu-id="255f1-141">שיעור היחידה בהוצאות המכירות בפועל שלך יוגדר כברירת מחדל כסכום המטבע שצוין בשדה המחיר.</span><span class="sxs-lookup"><span data-stu-id="255f1-141">The unit rate on your Expense sales actual will be defaulted to the currency amount specified in the Price field.</span></span>

<span data-ttu-id="255f1-142">אם הגדרת המחיר עבור קטגוריית ההוצאות אינה חוקית, גילית את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="255f1-142">If the price setup for the expense category isn't valid, then you have isolated the problem.</span></span> <span data-ttu-id="255f1-143">הפתרון הוא לעדכן את שורת מחיר הקטגוריה במחיר חוקי עבור קטגוריית ההוצאות בהתאם לכללים לעיל.</span><span class="sxs-lookup"><span data-stu-id="255f1-143">The solution is to edit the category price line with a valid price for the expense category in accordance with the rules above.</span></span> <span data-ttu-id="255f1-144">לאחר שביצעת זאת, צור מחדש ערך הוצאות, אשר אותו, ואז בדוק שהנתונים בפועל של המכירות שלא חויבו מציגים מחיר חוקי.</span><span class="sxs-lookup"><span data-stu-id="255f1-144">Once you’ve done that, recreate an expense entry, approve it, and then check that the unbilled sales actual gets a valid price.</span></span>

<span data-ttu-id="255f1-145">אם עדיין אינך רואה מחיר חוקי בהוצאות המכירות בפועל לאחר ביצוע שלוש הבדיקות לעיל, צור כרטיס תמיכה.</span><span class="sxs-lookup"><span data-stu-id="255f1-145">If you still don't see a valid price on your expense sales actual after doing the three checks above, log a support ticket.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]