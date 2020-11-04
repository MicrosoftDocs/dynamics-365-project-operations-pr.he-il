---
title: הגדרת שילוב כרטיסי אשראי
description: נושא זה מסביר כיצד לייבא ולתחזק עסקאות הקשורות להוצאות בכרטיסי אשראי.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 12c7971204b485ee7cb222cd9cffdfdfde93dcf4
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077271"
---
# <a name="set-up-credit-card-integration"></a><span data-ttu-id="df0d5-103">הגדרת שילוב כרטיסי אשראי</span><span class="sxs-lookup"><span data-stu-id="df0d5-103">Set up credit card integration</span></span>

<span data-ttu-id="df0d5-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="df0d5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="df0d5-105">ניתן להגדיר עסקאות בכרטיסי אשראי הקשורות להוצאות כך שהן יובאו אוטומטית בתזמון חוזר.</span><span class="sxs-lookup"><span data-stu-id="df0d5-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="df0d5-106">לחלופין, ניתן לייבא את העסקאות באופן ידני לפי הצורך.</span><span class="sxs-lookup"><span data-stu-id="df0d5-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="df0d5-107">עסקאות כרטיסי האשראי מיובאות באמצעות הישות של נתוני עסקאות בכרטיסי אשראי.</span><span class="sxs-lookup"><span data-stu-id="df0d5-107">The credit card transactions are imported through the Credit card transactions data entity.</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="df0d5-108">ייבוא עסקאות בכרטיסי אשראי</span><span class="sxs-lookup"><span data-stu-id="df0d5-108">Import credit card transactions</span></span>

1. <span data-ttu-id="df0d5-109">בדף **עסקאות בכרטיסי אשראי** , בחר **ייבוא עסקאות**.</span><span class="sxs-lookup"><span data-stu-id="df0d5-109">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="df0d5-110">אם אתה פותח ניהול נתונים בפעם הראשונה, על המערכת לעדכן את רשימת ישויות הנתונים לפני שתוכל להמשיך.</span><span class="sxs-lookup"><span data-stu-id="df0d5-110">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="df0d5-111">בשדה **שם** , הזן תיאור ייחודי של משימת הייבוא.</span><span class="sxs-lookup"><span data-stu-id="df0d5-111">In the **Name** field, enter a unique description of the import job.</span></span>
3. <span data-ttu-id="df0d5-112">בשדה **פורמט נתוני מקור** , בחר את הפורמט של הקובץ המכיל את עסקאות כרטיס האשראי לייבוא.</span><span class="sxs-lookup"><span data-stu-id="df0d5-112">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="df0d5-113">בחר **העלה** ולאחר מכן מצא ובחר את הקובץ לייבוא.</span><span class="sxs-lookup"><span data-stu-id="df0d5-113">Select **Upload** , and then find and select the file to import.</span></span>
5. <span data-ttu-id="df0d5-114">לאחר העלאת הקובץ, אמת את המיפוי של קובץ העסקאות בכרטיסי אשראי ואת העמודות של ישות נתוני עסקאות בכרטיסי אשראי על ידי בחירה בקישור **צפה במפה** באריח.</span><span class="sxs-lookup"><span data-stu-id="df0d5-114">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the Credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="df0d5-115">אם יש שגיאות מיפוי, או אם עליך לשנות את המיפוי, בצע את שינויי המיפוי מהכרטיסיה **תצוגה חזותית של מיפוי** או הכרטיסיה **פרטי מיפוי**.</span><span class="sxs-lookup"><span data-stu-id="df0d5-115">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="df0d5-116">כדי להפוך את העסקאות בכרטיס אשראי לאוטומטיות, בחר **צור משימת נתונים חוזרת**.</span><span class="sxs-lookup"><span data-stu-id="df0d5-116">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="df0d5-117">לאחר מכן תוכל להגדיר כל כמה זמן יבוצא ייבוא של עסקאות בכרטיסי אשראי.</span><span class="sxs-lookup"><span data-stu-id="df0d5-117">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="df0d5-118">לאחר שתסיים, בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="df0d5-118">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="df0d5-119">כדי לייבא את הקובץ שנבחר כעת, בחר **ייבוא**.</span><span class="sxs-lookup"><span data-stu-id="df0d5-119">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="df0d5-120">אם מתרחשות שגיאות במהלך הייבוא, תוכל להציג את יומן הביצוע או את נתוני האחסון כדי לראות את השגיאות שעליך לתקן כדי להבטיח ייבוא מוצלח.</span><span class="sxs-lookup"><span data-stu-id="df0d5-120">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help guarantee a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="df0d5-121">אם עליך לייבא יותר מתבנית קובץ אחת, יש ליצור עבודות ייבוא נפרדות לכל סוג פורמט.</span><span class="sxs-lookup"><span data-stu-id="df0d5-121">If you must import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="df0d5-122">הקצה מחדש את עסקאות כרטיסי האשראי לעובדים שעזבו</span><span class="sxs-lookup"><span data-stu-id="df0d5-122">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="df0d5-123">לאחר ביטול רשומת עובדים, חשבון Active Directory Domain Services‏ (AD DS) של העובד מושבת.</span><span class="sxs-lookup"><span data-stu-id="df0d5-123">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="df0d5-124">עם זאת, יתכנו עסקאות פעילות בכרטיסי אשראי שעדיין יש לרשום כהוצאות ולזכות עבורן.</span><span class="sxs-lookup"><span data-stu-id="df0d5-124">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="df0d5-125">מהדף **עסקאות בכרטיסי אשראי** , באפשרותך להקצות את העובד מחדש לכל עסקה בכרטיס אשראי שבה העובד המשויך כבר עזב.</span><span class="sxs-lookup"><span data-stu-id="df0d5-125">From the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="df0d5-126">בחר עסקאות בכרטיסי אשראי, אחת או יותר, ובחר **הקצה מחדש עסקאות**.</span><span class="sxs-lookup"><span data-stu-id="df0d5-126">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="df0d5-127">לאחר מכן תוכל לבחור עובד אחר שאליו יש להקצות את העסקאות בכרטיס אשראי.</span><span class="sxs-lookup"><span data-stu-id="df0d5-127">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="df0d5-128">לאחר ההקצאה מחדש של עסקאות כרטיסי האשראי, ניתן לבחור אותן לדוח הוצאות ולשלם עם התהליך הרגיל להחזר דוח הוצאות.</span><span class="sxs-lookup"><span data-stu-id="df0d5-128">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>
