---
title: הגדר מדיניות הוצאות
description: אתה יכול להגדיר מדיניות הוצאות שעובדיך חייבים לפעול על פיה בעת הזנה והגשת דוחות הוצאות ודרישות נסיעה.
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
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 30b3a0e1547ca7043b1433da2b4ebf02f2b473a1
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077378"
---
# <a name="define-expense-policies"></a><span data-ttu-id="b055e-103">הגדר מדיניות הוצאות</span><span class="sxs-lookup"><span data-stu-id="b055e-103">Define expense policies</span></span>

<span data-ttu-id="b055e-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="b055e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b055e-105">אתה יכול להגדיר מדיניות שעובדיך חייבים לפעול על פיה בעת הזנה והגשת דוחות הוצאות ודרישות נסיעה.</span><span class="sxs-lookup"><span data-stu-id="b055e-105">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="b055e-106">בעזרת יישום מדיניות הוצאות תוכל לנהל הוצאות בצורה יעילה.</span><span class="sxs-lookup"><span data-stu-id="b055e-106">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="b055e-107">לדוגמה, תוכל לקבוע מדיניות להוצאות על מלונות בניו יורק, שקובעת כי ההוצאה ללילה אינה יכולה לחרוג מ- USD 250.</span><span class="sxs-lookup"><span data-stu-id="b055e-107">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="b055e-108">אם עובד מגיש דוח הוצאות או דרישת נסיעה שבהם מחיר החדר עולה על סכום זה, המערכת תודיע</span><span class="sxs-lookup"><span data-stu-id="b055e-108">If a worker submits an expense report or travel requisition where the room rate exceeds this amount, the system will notify the</span></span>         
<span data-ttu-id="b055e-109">לעובד כי הסכום חורג מהמדיניות המותרת.</span><span class="sxs-lookup"><span data-stu-id="b055e-109">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="b055e-110">אתה יכול להגדיר את ההודעה שהעובד יקבל</span><span class="sxs-lookup"><span data-stu-id="b055e-110">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="b055e-111">בעת הגדרת המדיניות.</span><span class="sxs-lookup"><span data-stu-id="b055e-111">define the policy.</span></span>      
        
<span data-ttu-id="b055e-112">באפשרותך להגדיר שלושה סוגים של מדיניות:</span><span class="sxs-lookup"><span data-stu-id="b055e-112">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="b055e-113">**אזהרה** : מאפשרת לעובד להגיש דוח הוצאות או דרישת נסיעה אך ההוצאה תסומן עבור כל המאשרים</span><span class="sxs-lookup"><span data-stu-id="b055e-113">**Warning** : Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>         
  <span data-ttu-id="b055e-114">ולדיווח מאוחר יותר.</span><span class="sxs-lookup"><span data-stu-id="b055e-114">for later reporting.</span></span>        

- <span data-ttu-id="b055e-115">**שגיאה** : דורשת מהעובד לשנות את ההוצאה כדי לציית למדיניות לפני הגשת דוח ההוצאות או דרישת הנסיעה.</span><span class="sxs-lookup"><span data-stu-id="b055e-115">**Error** : Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>        
 
 - <span data-ttu-id="b055e-116">**הצדקה** : מחייבת את העובד או המנהל להזין הצדקה לחריגה מהסכום לפני הגשת דוח ההוצאות או דרישת הנסיעה.</span><span class="sxs-lookup"><span data-stu-id="b055e-116">**Justification** : Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="b055e-117">טיפים למדיניות</span><span class="sxs-lookup"><span data-stu-id="b055e-117">Policy tips</span></span>
<span data-ttu-id="b055e-118">להלן מספר הצעות שיכולות לסייע לך בעת יצירת מדיניות חדשה לניהול הוצאות:</span><span class="sxs-lookup"><span data-stu-id="b055e-118">Here are a few suggestions that can assist you when creating new policies for expense management:</span></span> 

- <span data-ttu-id="b055e-119">מדיניות נכנסת לתוקף בתאריך מסוים, כלומר מדיניות לא תיכנס לתוקף אם היא נוצרה עם תאריך שהוא לאחר התאריך שבו התרחשה ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="b055e-119">Policies are date effective which means a policy won't take effect if it's created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="b055e-120">לדוגמה, אתה יוצר מדיניות חדשה היום לאכיפת הוצאה מקסימלית לארוחה של $50.</span><span class="sxs-lookup"><span data-stu-id="b055e-120">For example, you create a new policy today to enforce a maximum meal expense of $50.</span></span> <span data-ttu-id="b055e-121">כל ההוצאות הקיימות שהוכנסו אתמול לא ייבדקו מול מדיניות זו.</span><span class="sxs-lookup"><span data-stu-id="b055e-121">Any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
- <span data-ttu-id="b055e-122">בעת יצירת מדיניות עבור קטגוריית הוצאות שניתן לפרט, שקול להוסיף תנאי לסוג שורת ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="b055e-122">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="b055e-123">ייתכן שמדיניות מסוימת, כגון דרישה לקבלה, אינה הגיונית עבור שורות מפורטות.</span><span class="sxs-lookup"><span data-stu-id="b055e-123">Some policies, such as requiring a receipt, may not make sense for itemized lines.</span></span> <span data-ttu-id="b055e-124">במצב זה, המדיניות מוחלת רק על שורת הכותרת או על שורה שאינה פרט.</span><span class="sxs-lookup"><span data-stu-id="b055e-124">In this situation, the policy only is applied to the header line or a non-itemized line.</span></span> 
- <span data-ttu-id="b055e-125">מדיניות ניהול ההוצאות מוערכת מול ישות המקור כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="b055e-125">Expense management policies are evaluated against the source entity by default.</span></span> <span data-ttu-id="b055e-126">עבור תרחישים בין-עסקיים, באפשרותך להגדיר את המדיניות שתיבחן מול ישות היעד (ישות הלווה) במקום זאת.</span><span class="sxs-lookup"><span data-stu-id="b055e-126">For intercompany scenarios, you can set the policy to be evaluated against the destination entity (borrowing entity) instead.</span></span> <span data-ttu-id="b055e-127">להפעלת המדיניות כנגד ישות היעד, הפעל את התכונה **הערך את מדיניות ההוצאות כנגד ישות משפטית לווה** בסביבת העבודה **ניהול תכונות**.</span><span class="sxs-lookup"><span data-stu-id="b055e-127">To run the policies against the destination entity, turn on the **Evaluate Expense policy against borrowing legal entity** feature in the **Feature Management** workspace.</span></span>

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="b055e-128">מתי להעריך מדיניות</span><span class="sxs-lookup"><span data-stu-id="b055e-128">When to evaluate policies</span></span>

<span data-ttu-id="b055e-129">בפרמטרים של ניהול הוצאות, אתה יכול לבחור להעריך את מדיניות ניהול ההוצאות כאשר שורה נשמרת או כאשר מוגש דוח הוצאות.</span><span class="sxs-lookup"><span data-stu-id="b055e-129">In expense management parameters, you can select to evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="b055e-130">אם תבחר להעריך מתי שורה נשמרת, למשתמשים יראו בשלב מוקדם יותר מה עליהם לעשות כדי להשלים את דוח ההוצאות בבת אחת.</span><span class="sxs-lookup"><span data-stu-id="b055e-130">If you choose to evaluate when a line is saved, users will have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="b055e-131">אחרת, אתה יכול לעכב את הערכת המדיניות ולחסוך זמן על ידי אימות בסוף, במהלך ההגשה לזרימת העבודה.</span><span class="sxs-lookup"><span data-stu-id="b055e-131">Otherwise, you can delay policy evaluation and save time by validating at the end, during the submission to workflow.</span></span>
