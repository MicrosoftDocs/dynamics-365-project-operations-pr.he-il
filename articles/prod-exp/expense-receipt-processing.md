---
title: עיבוד קבלות של הוצאות
description: נושא זה מספק מידע על עיבוד זיהוי תווים אופטי (OCR) של קבלות. תכונה זו נועדה לשפר את חווית המשתמש בעת יצירת דוחות הוצאות ב-Dynamics 365 Finance‏ Microsoft.
author: stsporen
ms.date: 05/14/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Operations, Core
ms.search.region: Global
ms.author: stsporen
ms.search.validFrom: 2019-11-20
ms.dyn365.ops.version: 10.0.8
ms.openlocfilehash: ed9c97ba9cc505106599c2896dc2112358d0c408
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993507"
---
# <a name="expense-receipt-processing"></a><span data-ttu-id="4d609-104">עיבוד קבלות של הוצאות</span><span class="sxs-lookup"><span data-stu-id="4d609-104">Expense receipt processing</span></span>

<span data-ttu-id="4d609-105">הזנת ההוצאות שופרה באמצעות הכנסת עיבוד זיהוי תווים אופטי (OCR) לקבלות.</span><span class="sxs-lookup"><span data-stu-id="4d609-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="4d609-106">תכונה זו נועדה לשפר את חווית המשתמש בעת יצירת דוחות הוצאות.</span><span class="sxs-lookup"><span data-stu-id="4d609-106">This feature is designed to improve the user experience when expense reports are created.</span></span>

## <a name="key-features"></a><span data-ttu-id="4d609-107">תכונות מרכזיות</span><span class="sxs-lookup"><span data-stu-id="4d609-107">Key features</span></span>

- <span data-ttu-id="4d609-108">המערכת מחלצת את שם הסוחר, התאריך והסכום הכולל מהקבלות.</span><span class="sxs-lookup"><span data-stu-id="4d609-108">The merchant name, date, and total amount are extracted from receipts.</span></span>
- <span data-ttu-id="4d609-109">תכונה זו מנסה להתאים קבלות לא מצורפות לעסקאות הוצאות שלא מצורפות.</span><span class="sxs-lookup"><span data-stu-id="4d609-109">The feature tries to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="4d609-110">משתמשים יכולים ליצור עסקאות הוצאות שהוזנו ידנית מקבלות.</span><span class="sxs-lookup"><span data-stu-id="4d609-110">Users can create manually entered expense transactions from receipts.</span></span>

## <a name="usage-examples"></a><span data-ttu-id="4d609-111">דוגמאות שימוש</span><span class="sxs-lookup"><span data-stu-id="4d609-111">Usage examples</span></span>

<span data-ttu-id="4d609-112">כדי לצרף אוטומטית קבלות הכוללות עסקאות בכרטיסי אשראי בעת יצירת דוח הוצאות, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="4d609-112">To automatically attach receipts that include credit card transactions when an expense report is created, do the following:</span></span>

  1. <span data-ttu-id="4d609-113">פתח את סביבת העבודה **ניהול הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="4d609-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="4d609-114">בכרטיסיה **קבלות**, ודא שיש קבלות שלא שויכו.</span><span class="sxs-lookup"><span data-stu-id="4d609-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="4d609-115">ניתן גם להעלות קבלות בכרטיסיה **קבלות**.</span><span class="sxs-lookup"><span data-stu-id="4d609-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="4d609-116">בכרטיסיה **הוצאות**, ודא שיש הוצאות שלא שויכו.</span><span class="sxs-lookup"><span data-stu-id="4d609-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="4d609-117">בדרך כלל, מנהל מערכת של ההוצאות מייבא את ההוצאות האלה מספק כרטיסי האשראי.</span><span class="sxs-lookup"><span data-stu-id="4d609-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="4d609-118">בחר **דוח הוצאות חדש**.</span><span class="sxs-lookup"><span data-stu-id="4d609-118">Select **New expense report**.</span></span> <span data-ttu-id="4d609-119">שים לב שאתה יכול לכלול הוצאות וקבלות גם עכשיו כשאתה יוצר דוח הוצאות.</span><span class="sxs-lookup"><span data-stu-id="4d609-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="4d609-120">אם אתה מוסיף גם הוצאות וגם קבלות, מופעלת התאמה אוטומטית של הקבלות להוצאות.</span><span class="sxs-lookup"><span data-stu-id="4d609-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

<span data-ttu-id="4d609-121">כדי ליצור הוצאה, או להתאים הוצאה מקבלה, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="4d609-121">To create an expense, or match an expense from a receipt, do the following:</span></span>

  1. <span data-ttu-id="4d609-122">בדוח הוצאות, בכרטיסיה **קבלות**, צרף קבלה על ידי בחירה באפשרות **הוסף קבלות**.</span><span class="sxs-lookup"><span data-stu-id="4d609-122">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="4d609-123">מתחת לתמונה שהועלתה של הקבלה, שים לב לאפשרויות **יצירה** ו **התאמה**.</span><span class="sxs-lookup"><span data-stu-id="4d609-123">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="4d609-124">בחר **יצירה** כדי ליצור עסקת הוצאות שהוזנה ידנית ולמלא את הערכים שחולצו מהקבלה.</span><span class="sxs-lookup"><span data-stu-id="4d609-124">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="4d609-125">אם תבחר **התאמה**, המערכת מנסה להתאים הוצאה קיימת לקבלה.</span><span class="sxs-lookup"><span data-stu-id="4d609-125">If you select **Match**, the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="4d609-126">התקנה</span><span class="sxs-lookup"><span data-stu-id="4d609-126">Installation</span></span>

<span data-ttu-id="4d609-127">תכונה זו פועלת בשילוב עם התכונה **דוחות ההוצאות החדשניות** המסייעת לפשט את חוויית ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="4d609-127">This feature works in combination with the **Expense reports re-imagined** feature to help simplify the expense experience.</span></span> <span data-ttu-id="4d609-128">תכונה זו זמינה רק בסביבות Tier 2+‎, שהן ארגז חול וייצור.</span><span class="sxs-lookup"><span data-stu-id="4d609-128">This feature is only available for Tier 2+ environments, which are Sandbox and Production.</span></span>

<span data-ttu-id="4d609-129">כדי להשתמש ביכולות המתקדמות של הוצאות, התקן את תוספת השירות של ניהול הוצאות עבור Microsoft Dynamics 365 Finance והפעל את התכונות במופע שלך.</span><span class="sxs-lookup"><span data-stu-id="4d609-129">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="4d609-130">אתה יכול לגשת לתוספת מהפרויקט שלך ב- Microsoft Dynamics Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="4d609-130">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="4d609-131">היכנס ל- LCS ופתח את הסביבה הרצויה.</span><span class="sxs-lookup"><span data-stu-id="4d609-131">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="4d609-132">עבור אל **פרטים מלאים**.</span><span class="sxs-lookup"><span data-stu-id="4d609-132">Go to **Full details**.</span></span>
3. <span data-ttu-id="4d609-133">בחר **תחזק** או גלול מטה אל **תוספות לסביבה** FastTab.</span><span class="sxs-lookup"><span data-stu-id="4d609-133">Select **Maintain**, or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="4d609-134">בחר **התקן תוסף חדש**.</span><span class="sxs-lookup"><span data-stu-id="4d609-134">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="4d609-135">בחר **שירות ניהול הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="4d609-135">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="4d609-136">עקוב אחר מדריך ההתקנה והסכם לתנאים ולהגבלות.</span><span class="sxs-lookup"><span data-stu-id="4d609-136">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="4d609-137">בחר **התקנה**.</span><span class="sxs-lookup"><span data-stu-id="4d609-137">Select **Install**.</span></span>

<span data-ttu-id="4d609-138">בסביבת העבודה **ניהול תכונות**, הפעל את התכונות הבאות:</span><span class="sxs-lookup"><span data-stu-id="4d609-138">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="4d609-139">דוחות הוצאות שעוצבו מחדש</span><span class="sxs-lookup"><span data-stu-id="4d609-139">Expense reports re-imagined</span></span>
- <span data-ttu-id="4d609-140">התאמה אוטומטית ויצירת הוצאה מקבלה</span><span class="sxs-lookup"><span data-stu-id="4d609-140">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="4d609-141">כאשר אתה מפעיל תכונות אלה מתרחשות הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="4d609-141">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="4d609-142">סביבת העבודה הקיימת של **ניהול הוצאות** מוחלפת בסביבת העבודה החדשה.</span><span class="sxs-lookup"><span data-stu-id="4d609-142">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="4d609-143">נוסף פריט תפריט חדש שבו ניתן לראות את שדות ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="4d609-143">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="4d609-144">אתה עדיין יכול לפתוח את דף **דוחות הוצאות** הקודם על ידי מעבר אל **ניהול הוצאות > ההוצאות שלי > דוחות הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="4d609-144">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="4d609-145">זרימות עבודה וכל האישורים עדיין מעבירים אותך לדף דוחות ההוצאות הקיים.</span><span class="sxs-lookup"><span data-stu-id="4d609-145">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="4d609-146">הקבלות יעובדו באמצעות Microsoft Azure Cognitive Services, ומטא נתונים יחולצו ויתווספו.</span><span class="sxs-lookup"><span data-stu-id="4d609-146">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="4d609-147">מתווספת אפשרות שמאפשרת ליצור דוח הוצאות הכולל קבלות תואמות שלא שויכו.</span><span class="sxs-lookup"><span data-stu-id="4d609-147">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="4d609-148">אפשרות שמתווספת לדוחות הוצאות כדי ליצור שורת הוצאות מתוך קבלה, או שמנסה להתאים קבלה קיימת לשורת הוצאות קיימת.</span><span class="sxs-lookup"><span data-stu-id="4d609-148">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

<span data-ttu-id="4d609-149">לקבלת מידע נוסף אודות תכונת דוחות הוצאות החדשניות, ראה [דוחות הוצאות חדשניות](ExpenseWorkspaceNew.md).</span><span class="sxs-lookup"><span data-stu-id="4d609-149">For more information about the Expense reports re-imagined feature, see [Expense reports reimagined](ExpenseWorkspaceNew.md).</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="4d609-150">שאלות נפוצות</span><span class="sxs-lookup"><span data-stu-id="4d609-150">Frequently asked questions</span></span>

<span data-ttu-id="4d609-151">**האם Microsoft משתמשת בנתונים שלי עבור המודלים שלה?**</span><span class="sxs-lookup"><span data-stu-id="4d609-151">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="4d609-152">לא, Microsoft בנתה מודל למידת מכונה כללי לשירות עיבוד הקבלות שלה.</span><span class="sxs-lookup"><span data-stu-id="4d609-152">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="4d609-153">מודל זה אינו מבוסס על הקבלות שאתה מעלה.</span><span class="sxs-lookup"><span data-stu-id="4d609-153">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="4d609-154">**היכן תכונה זו זמינה ומעובדת?**</span><span class="sxs-lookup"><span data-stu-id="4d609-154">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="4d609-155">נכון לעכשיו, היא פועלת בארצות הברית.</span><span class="sxs-lookup"><span data-stu-id="4d609-155">Currently, the United States is supported.</span></span>

<span data-ttu-id="4d609-156">**לאן עוברות הקבלות שלי?**</span><span class="sxs-lookup"><span data-stu-id="4d609-156">**Where do my receipts go?**</span></span>

<span data-ttu-id="4d609-157">Finance ייצור קשר עם Cognitive Services כדי לחלץ את נתוני השדות.</span><span class="sxs-lookup"><span data-stu-id="4d609-157">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="4d609-158">Cognitive Services ישמור עותק של הקבלה למשך עד 24 שעות תוך כדי העיבוד.</span><span class="sxs-lookup"><span data-stu-id="4d609-158">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="4d609-159">לאחר סיום העיבוד, Cognitive Services יסיר את הקבלה.</span><span class="sxs-lookup"><span data-stu-id="4d609-159">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="4d609-160">הקבלות עדיין מאוחסנות ב- Finance.</span><span class="sxs-lookup"><span data-stu-id="4d609-160">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="4d609-161">למידע נוסף ראה [אפשר הבנת קבלות באמצעות היכולת החדשה של Form Recognizer](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span><span class="sxs-lookup"><span data-stu-id="4d609-161">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]