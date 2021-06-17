---
title: הגדרת שילוב כרטיסי אשראי
description: נושא זה מסביר כיצד לעבוד עם עסקאות כרטיסי אשראי הקשורות להוצאות.
author: suvaidya
ms.date: 04/02/2021
ms.topic: article
ms.prod: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 3555e894e206c2aafb30b0df1e52efadd69b0713
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001818"
---
# <a name="set-up-credit-card-integration"></a><span data-ttu-id="b757f-103">הגדרת שילוב כרטיסי אשראי</span><span class="sxs-lookup"><span data-stu-id="b757f-103">Set up credit card integration</span></span>

<span data-ttu-id="b757f-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="b757f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b757f-105">ניתן להגדיר עסקאות בכרטיסי אשראי הקשורות להוצאות כך שהן יובאו אוטומטית בתזמון חוזר.</span><span class="sxs-lookup"><span data-stu-id="b757f-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="b757f-106">לחלופין, ניתן לייבא את העסקאות באופן ידני לפי הצורך.</span><span class="sxs-lookup"><span data-stu-id="b757f-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="b757f-107">עסקאות כרטיסי האשראי מיובאות באמצעות הישות של נתוני עסקאות בכרטיסי אשראי.</span><span class="sxs-lookup"><span data-stu-id="b757f-107">The credit card transactions are imported through the credit card transactions data entity.</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="b757f-108">ייבוא עסקאות בכרטיסי אשראי</span><span class="sxs-lookup"><span data-stu-id="b757f-108">Import credit card transactions</span></span>

<span data-ttu-id="b757f-109">כדי לייבא עסקאות כרטיסי אשראי, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="b757f-109">To import credit card transactions, follow these steps:</span></span>

1. <span data-ttu-id="b757f-110">בדף **עסקאות בכרטיסי אשראי**, בחר **ייבוא עסקאות**.</span><span class="sxs-lookup"><span data-stu-id="b757f-110">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="b757f-111">אם אתה פותח ניהול נתונים בפעם הראשונה, על המערכת לעדכן את רשימת ישויות הנתונים לפני שתוכל להמשיך.</span><span class="sxs-lookup"><span data-stu-id="b757f-111">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="b757f-112">בשדה **שם**, הזן תיאור ייחודי עבור משימת הייבוא.</span><span class="sxs-lookup"><span data-stu-id="b757f-112">In the **Name** field, enter a unique description for the import job.</span></span>
3. <span data-ttu-id="b757f-113">בשדה **פורמט נתוני מקור**, בחר את הפורמט של הקובץ המכיל את עסקאות כרטיס האשראי לייבוא.</span><span class="sxs-lookup"><span data-stu-id="b757f-113">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="b757f-114">בחר **העלה** ולאחר מכן מצא ובחר את הקובץ לייבוא.</span><span class="sxs-lookup"><span data-stu-id="b757f-114">Select **Upload**, and then find and select the file to import.</span></span>
5. <span data-ttu-id="b757f-115">לאחר העלאת הקובץ, אמת את המיפוי של קובץ העסקאות בכרטיסי אשראי ואת העמודות של ישות נתוני עסקאות בכרטיסי אשראי על ידי בחירה בקישור **צפה במפה** באריח.</span><span class="sxs-lookup"><span data-stu-id="b757f-115">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="b757f-116">אם יש שגיאות מיפוי, או אם עליך לשנות את המיפוי, בצע את שינויי המיפוי מהכרטיסיה **תצוגה חזותית של מיפוי** או הכרטיסיה **פרטי מיפוי**.</span><span class="sxs-lookup"><span data-stu-id="b757f-116">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="b757f-117">כדי להפוך את העסקאות בכרטיס אשראי לאוטומטיות, בחר **צור משימת נתונים חוזרת**.</span><span class="sxs-lookup"><span data-stu-id="b757f-117">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="b757f-118">לאחר מכן תוכל להגדיר כל כמה זמן יבוצא ייבוא של עסקאות בכרטיסי אשראי.</span><span class="sxs-lookup"><span data-stu-id="b757f-118">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="b757f-119">לאחר שתסיים, בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="b757f-119">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="b757f-120">כדי לייבא את הקובץ שנבחר כעת, בחר **ייבוא**.</span><span class="sxs-lookup"><span data-stu-id="b757f-120">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="b757f-121">אם מתרחשות שגיאות במהלך הייבוא, תוכל להציג את יומן הביצוע או את נתוני האחסון כדי לראות את השגיאות שעליך לתקן כדי להבטיח ייבוא מוצלח.</span><span class="sxs-lookup"><span data-stu-id="b757f-121">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help ensure a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="b757f-122">אם עליך לייבא יותר מתבנית קובץ אחת, עליך ליצור משימות ייבוא נפרדות לכל סוג תבנית.</span><span class="sxs-lookup"><span data-stu-id="b757f-122">If you need to import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="b757f-123">הקצה מחדש את עסקאות כרטיסי האשראי לעובדים שעזבו</span><span class="sxs-lookup"><span data-stu-id="b757f-123">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="b757f-124">לאחר ביטול רשומת עובדים, חשבון Active Directory Domain Services‏ (AD DS) של העובד מושבת.</span><span class="sxs-lookup"><span data-stu-id="b757f-124">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="b757f-125">עם זאת, יתכנו עסקאות פעילות בכרטיסי אשראי שעדיין יש לרשום כהוצאות ולזכות עבורן.</span><span class="sxs-lookup"><span data-stu-id="b757f-125">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="b757f-126">בדף **עסקאות בכרטיסי אשראי**, באפשרותך להקצות את העובד מחדש לכל עסקת כרטיס אשראי שבה הקצאת העובד המשויך נפסקה.</span><span class="sxs-lookup"><span data-stu-id="b757f-126">On the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="b757f-127">בחר עסקאות בכרטיסי אשראי, אחת או יותר, ובחר **הקצה מחדש עסקאות**.</span><span class="sxs-lookup"><span data-stu-id="b757f-127">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="b757f-128">לאחר מכן תוכל לבחור עובד אחר שאליו יש להקצות את העסקאות בכרטיס אשראי.</span><span class="sxs-lookup"><span data-stu-id="b757f-128">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="b757f-129">לאחר ההקצאה מחדש של עסקאות כרטיסי האשראי, ניתן לבחור אותן לדוח הוצאות ולשלם עם התהליך הרגיל להחזר דוח הוצאות.</span><span class="sxs-lookup"><span data-stu-id="b757f-129">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>

## <a name="delete-credit-card-transactions"></a><span data-ttu-id="b757f-130">מחיקת עסקאות בכרטיסי אשראי</span><span class="sxs-lookup"><span data-stu-id="b757f-130">Delete credit card transactions</span></span> 

<span data-ttu-id="b757f-131">לפעמים, לאחר ייבוא עסקאות בכרטיסי אשראי, ייתכן שיהיה צורך למחוק עסקאות מסוימות.</span><span class="sxs-lookup"><span data-stu-id="b757f-131">Sometimes, after credit card transactions are imported, certain transactions may need to be deleted.</span></span> <span data-ttu-id="b757f-132">זה יכול להיות בגלל שהעסקאות כפולות או שהנתונים עשויים לא להיות מדויקים.</span><span class="sxs-lookup"><span data-stu-id="b757f-132">This could be because the transactions are duplicates or because the data might isn't accurate.</span></span> <span data-ttu-id="b757f-133">מנהלי מערכת יכולים להשתמש בתכונה **"מחיקת עסקאות בכרטיס אשראי"** כדי לבחור ולמחוק עסקאות בכרטיסי אשראי ש **לא מצורפות** לדוח הוצאות.</span><span class="sxs-lookup"><span data-stu-id="b757f-133">Admins can use the **"Delete credit card transactions"** feature to select and delete credit card transactions that are **not attached** to an expense report.</span></span> 

1. <span data-ttu-id="b757f-134">עבור אל **משימות תקופתיות** > **מחיקת עסקאות בכרטיס אשראי**.</span><span class="sxs-lookup"><span data-stu-id="b757f-134">Go to **Periodic tasks** > **Delete credit card transactions**.</span></span>
2. <span data-ttu-id="b757f-135">בחר **סינון** וספק מידע לזיהוי הרשומות שיכללו.</span><span class="sxs-lookup"><span data-stu-id="b757f-135">Select **Filter** and provide information to identify the records to include.</span></span>
3. <span data-ttu-id="b757f-136">בחר **אישור** כדי למחוק את הרשומות.</span><span class="sxs-lookup"><span data-stu-id="b757f-136">Select **OK** to delete the records.</span></span> 

[!INCLUDE[footer-include](../includes/footer-banner.md)]
