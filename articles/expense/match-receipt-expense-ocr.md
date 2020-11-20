---
title: התאמת קבלה להוצאה באמצעות OCR
description: נושא זה מספק מידע על עיבוד זיהוי תווים אופטי (OCR) של קבלות.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 55f63c8c092942b73a55c9d86d867bca600f42e5
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4124324"
---
# <a name="match-a-receipt-to-an-expense-using-ocr"></a><span data-ttu-id="356e8-103">התאמת קבלה להוצאה באמצעות OCR</span><span class="sxs-lookup"><span data-stu-id="356e8-103">Match a receipt to an expense using OCR</span></span>

<span data-ttu-id="356e8-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="356e8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="356e8-105">הזנת ההוצאות שופרה באמצעות הכנסת עיבוד זיהוי תווים אופטי (OCR) לקבלות.</span><span class="sxs-lookup"><span data-stu-id="356e8-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="356e8-106">פונקציונליות זו נועדה לשפר את חווית המשתמש בעת יצירת דוחות הוצאות.</span><span class="sxs-lookup"><span data-stu-id="356e8-106">This functionality is designed to improve the user experience when creating expense reports.</span></span>

## <a name="key-features"></a><span data-ttu-id="356e8-107">תכונות מרכזיות</span><span class="sxs-lookup"><span data-stu-id="356e8-107">Key features</span></span>

- <span data-ttu-id="356e8-108">המערכת מחלצת את שם הסוחר, התאריך והסכום הכולל מהתקבולים.</span><span class="sxs-lookup"><span data-stu-id="356e8-108">The system extracts the merchant name, date, and total amount from receipts.</span></span>
- <span data-ttu-id="356e8-109">המערכת תנסה להתאים קבלות שלא שויכו לעסקאות הוצאות שלא שויכו.</span><span class="sxs-lookup"><span data-stu-id="356e8-109">The system will try to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="356e8-110">ניתן ליצור עסקאות הוצאות שהוזנו ידנית מקבלות.</span><span class="sxs-lookup"><span data-stu-id="356e8-110">You can create manually entered expense transactions from receipts.</span></span>

## <a name="attach-receipts-to-an-expense-report"></a><span data-ttu-id="356e8-111">צרף קבלות לדוח הוצאות</span><span class="sxs-lookup"><span data-stu-id="356e8-111">Attach receipts to an expense report</span></span>

<span data-ttu-id="356e8-112">כדי לצרף אוטומטית קבלות הכוללות עסקאות בכרטיסי אשראי בעת יצירת דוח הוצאות, בצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="356e8-112">To automatically attach receipts that include credit card transactions when an expense report is created, complete the following steps.</span></span>

  1. <span data-ttu-id="356e8-113">פתח את סביבת העבודה **ניהול הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="356e8-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="356e8-114">בכרטיסיה **קבלות**, ודא שיש קבלות שלא שויכו.</span><span class="sxs-lookup"><span data-stu-id="356e8-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="356e8-115">ניתן גם להעלות קבלות בכרטיסיה **קבלות**.</span><span class="sxs-lookup"><span data-stu-id="356e8-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="356e8-116">בכרטיסיה **הוצאות**, ודא שיש הוצאות שלא שויכו.</span><span class="sxs-lookup"><span data-stu-id="356e8-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="356e8-117">בדרך כלל, מנהל מערכת של ההוצאות מייבא את ההוצאות האלה מספק כרטיסי האשראי.</span><span class="sxs-lookup"><span data-stu-id="356e8-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="356e8-118">בחר **דוח הוצאות חדש**.</span><span class="sxs-lookup"><span data-stu-id="356e8-118">Select **New expense report**.</span></span> <span data-ttu-id="356e8-119">שים לב שאתה יכול לכלול הוצאות וקבלות גם עכשיו כשאתה יוצר דוח הוצאות.</span><span class="sxs-lookup"><span data-stu-id="356e8-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="356e8-120">אם אתה מוסיף גם הוצאות וגם קבלות, מופעלת התאמה אוטומטית של הקבלות להוצאות.</span><span class="sxs-lookup"><span data-stu-id="356e8-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

## <a name="create-or-match-receipts-to-an-expense-report"></a><span data-ttu-id="356e8-121">צור או התאם קבלות לדוח הוצאות</span><span class="sxs-lookup"><span data-stu-id="356e8-121">Create or match receipts to an expense report</span></span>
<span data-ttu-id="356e8-122">כדי ליצור הוצאה, או להתאים הוצאה מקבלה, בצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="356e8-122">To create an expense, or match an expense from a receipt, complete the following steps.</span></span>

  1. <span data-ttu-id="356e8-123">בדוח הוצאות, בכרטיסיה **קבלות**, צרף קבלה על ידי בחירה באפשרות **הוסף קבלות**.</span><span class="sxs-lookup"><span data-stu-id="356e8-123">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="356e8-124">מתחת לתמונה שהועלתה של הקבלה, שים לב לאפשרויות **יצירה** ו **התאמה**.</span><span class="sxs-lookup"><span data-stu-id="356e8-124">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="356e8-125">בחר **יצירה** כדי ליצור עסקת הוצאות שהוזנה ידנית ולמלא את הערכים שחולצו מהקבלה.</span><span class="sxs-lookup"><span data-stu-id="356e8-125">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="356e8-126">אם תבחר **התאמה**, המערכת מנסה להתאים הוצאה קיימת לקבלה.</span><span class="sxs-lookup"><span data-stu-id="356e8-126">If you select **Match**, the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="356e8-127">התקנה</span><span class="sxs-lookup"><span data-stu-id="356e8-127">Installation</span></span>

<span data-ttu-id="356e8-128">כדי להשתמש ביכולות המתקדמות של הוצאות, התקן את תוספת השירות של ניהול הוצאות עבור Microsoft Dynamics 365 Finance והפעל את התכונות במופע שלך.</span><span class="sxs-lookup"><span data-stu-id="356e8-128">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="356e8-129">אתה יכול לגשת לתוספת מהפרויקט שלך ב- Microsoft Dynamics Lifecycle Services (LCS).</span><span class="sxs-lookup"><span data-stu-id="356e8-129">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="356e8-130">היכנס ל- LCS ופתח את הסביבה הרצויה.</span><span class="sxs-lookup"><span data-stu-id="356e8-130">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="356e8-131">עבור אל **פרטים מלאים**.</span><span class="sxs-lookup"><span data-stu-id="356e8-131">Go to **Full details**.</span></span>
3. <span data-ttu-id="356e8-132">בחר **תחזק** או גלול מטה אל **תוספות לסביבה** FastTab.</span><span class="sxs-lookup"><span data-stu-id="356e8-132">Select **Maintain**, or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="356e8-133">בחר **התקן תוסף חדש**.</span><span class="sxs-lookup"><span data-stu-id="356e8-133">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="356e8-134">בחר **שירות ניהול הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="356e8-134">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="356e8-135">עקוב אחר מדריך ההתקנה והסכם לתנאים ולהגבלות.</span><span class="sxs-lookup"><span data-stu-id="356e8-135">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="356e8-136">בחר **התקנה**.</span><span class="sxs-lookup"><span data-stu-id="356e8-136">Select **Install**.</span></span>

<span data-ttu-id="356e8-137">בסביבת העבודה **ניהול תכונות**, הפעל את התכונות הבאות:</span><span class="sxs-lookup"><span data-stu-id="356e8-137">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="356e8-138">דוחות הוצאות שעוצבו מחדש</span><span class="sxs-lookup"><span data-stu-id="356e8-138">Expense reports re-imagined</span></span>
- <span data-ttu-id="356e8-139">התאמה אוטומטית ויצירת הוצאה מקבלה</span><span class="sxs-lookup"><span data-stu-id="356e8-139">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="356e8-140">כאשר אתה מפעיל תכונות אלה מתרחשות הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="356e8-140">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="356e8-141">סביבת העבודה הקיימת של **ניהול הוצאות** מוחלפת בסביבת העבודה החדשה.</span><span class="sxs-lookup"><span data-stu-id="356e8-141">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="356e8-142">נוסף פריט תפריט חדש שבו ניתן לראות את שדות ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="356e8-142">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="356e8-143">אתה עדיין יכול לפתוח את דף **דוחות הוצאות** הקודם על ידי מעבר אל **ניהול הוצאות > ההוצאות שלי > דוחות הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="356e8-143">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="356e8-144">זרימות עבודה וכל האישורים עדיין מעבירים אותך לדף דוחות ההוצאות הקיים.</span><span class="sxs-lookup"><span data-stu-id="356e8-144">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="356e8-145">הקבלות יעובדו באמצעות Microsoft Azure Cognitive Services, ומטא נתונים יחולצו ויתווספו.</span><span class="sxs-lookup"><span data-stu-id="356e8-145">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="356e8-146">מתווספת אפשרות שמאפשרת ליצור דוח הוצאות הכולל קבלות תואמות שלא שויכו.</span><span class="sxs-lookup"><span data-stu-id="356e8-146">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="356e8-147">אפשרות שמתווספת לדוחות הוצאות כדי ליצור שורת הוצאות מתוך קבלה, או שמנסה להתאים קבלה קיימת לשורת הוצאות קיימת.</span><span class="sxs-lookup"><span data-stu-id="356e8-147">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="356e8-148">שאלות נפוצות</span><span class="sxs-lookup"><span data-stu-id="356e8-148">Frequently asked questions</span></span>

<span data-ttu-id="356e8-149">**האם Microsoft משתמשת בנתונים שלי עבור המודלים שלה?**</span><span class="sxs-lookup"><span data-stu-id="356e8-149">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="356e8-150">לא, Microsoft בנתה מודל למידת מכונה כללי לשירות עיבוד הקבלות שלה.</span><span class="sxs-lookup"><span data-stu-id="356e8-150">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="356e8-151">מודל זה אינו מבוסס על הקבלות שאתה מעלה.</span><span class="sxs-lookup"><span data-stu-id="356e8-151">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="356e8-152">**היכן תכונה זו זמינה ומעובדת?**</span><span class="sxs-lookup"><span data-stu-id="356e8-152">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="356e8-153">נכון לעכשיו, היא פועלת בארצות הברית.</span><span class="sxs-lookup"><span data-stu-id="356e8-153">Currently, the United States is supported.</span></span>

<span data-ttu-id="356e8-154">**לאן עוברות הקבלות שלי?**</span><span class="sxs-lookup"><span data-stu-id="356e8-154">**Where do my receipts go?**</span></span>

<span data-ttu-id="356e8-155">Finance ייצור קשר עם Cognitive Services כדי לחלץ את נתוני השדות.</span><span class="sxs-lookup"><span data-stu-id="356e8-155">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="356e8-156">Cognitive Services ישמור עותק של הקבלה למשך עד 24 שעות תוך כדי העיבוד.</span><span class="sxs-lookup"><span data-stu-id="356e8-156">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="356e8-157">לאחר סיום העיבוד, Cognitive Services יסיר את הקבלה.</span><span class="sxs-lookup"><span data-stu-id="356e8-157">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="356e8-158">הקבלות עדיין מאוחסנות ב- Finance.</span><span class="sxs-lookup"><span data-stu-id="356e8-158">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="356e8-159">למידע נוסף ראה [אפשר הבנת קבלות באמצעות היכולת החדשה של Form Recognizer](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span><span class="sxs-lookup"><span data-stu-id="356e8-159">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>
