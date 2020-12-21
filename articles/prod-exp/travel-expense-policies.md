---
title: הגדרת מדיניות הוצאות
description: אתה יכול להגדיר מדיניות הוצאות שעובדיך חייבים לפעול על פיה בעת הזנה והגשת דוחות הוצאות ודרישות נסיעה ב- Microsoft Dynamics 365 Finance.
author: suvaidya
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysPolicyListPage, TrvPolicyRule
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 6240a7be175800ce6f3b066de9e935ab370629ef
ms.sourcegitcommit: 13a4e58eddbb0f81aca07c1ff452c420dbd8a68f
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 11/30/2020
ms.locfileid: "4650095"
---
# <a name="set-up-expense-policies"></a><span data-ttu-id="f32a7-103">הגדרת מדיניות הוצאות</span><span class="sxs-lookup"><span data-stu-id="f32a7-103">Set up expense policies</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="f32a7-104">אתה יכול להגדיר מדיניות שעובדיך חייבים לפעול על פיה בעת הזנה והגשת דוחות הוצאות ודרישות נסיעה.</span><span class="sxs-lookup"><span data-stu-id="f32a7-104">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="f32a7-105">בעזרת יישום מדיניות הוצאות תוכל לנהל הוצאות בצורה יעילה.</span><span class="sxs-lookup"><span data-stu-id="f32a7-105">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="f32a7-106">לדוגמה, תוכל לקבוע מדיניות להוצאות על מלונות בניו יורק, שקובעת כי ההוצאה ללילה אינה יכולה לחרוג מ- USD 250.</span><span class="sxs-lookup"><span data-stu-id="f32a7-106">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="f32a7-107">אם עובד מגיש דוח הוצאות או דרישת נסיעה שבהם מחיר החדר עולה על סכום זה, המערכת תודיע</span><span class="sxs-lookup"><span data-stu-id="f32a7-107">If a worker submits an expense report or a travel requisition in which the room rate exceeds this amount, the system will notify the</span></span>        
<span data-ttu-id="f32a7-108">לעובד כי הסכום חורג מהמדיניות המותרת.</span><span class="sxs-lookup"><span data-stu-id="f32a7-108">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="f32a7-109">אתה יכול להגדיר את ההודעה שהעובד יקבל</span><span class="sxs-lookup"><span data-stu-id="f32a7-109">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="f32a7-110">בעת הגדרת המדיניות.</span><span class="sxs-lookup"><span data-stu-id="f32a7-110">define the policy.</span></span>      
        
<span data-ttu-id="f32a7-111">באפשרותך להגדיר שלושה סוגים של מדיניות:</span><span class="sxs-lookup"><span data-stu-id="f32a7-111">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="f32a7-112">אזהרה - מאפשרת לעובד להגיש דוח הוצאות או דרישת נסיעה אך ההוצאה תסומן עבור כל המאשרים</span><span class="sxs-lookup"><span data-stu-id="f32a7-112">Warning – Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>        
  <span data-ttu-id="f32a7-113">ולדיווח מאוחר יותר.</span><span class="sxs-lookup"><span data-stu-id="f32a7-113">for later reporting.</span></span>        

- <span data-ttu-id="f32a7-114">שגיאה - דורשת מהעובד לשנות את ההוצאה כדי לציית למדיניות לפני הגשת דוח ההוצאות או דרישת הנסיעה.</span><span class="sxs-lookup"><span data-stu-id="f32a7-114">Error – Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>       
 
 - <span data-ttu-id="f32a7-115">הצדקה - מחייבת את העובד או המנהל להזין הצדקה לחריגה מהסכום לפני הגשת דוח ההוצאות או דרישת הנסיעה.</span><span class="sxs-lookup"><span data-stu-id="f32a7-115">Justification – Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="f32a7-116">טיפים למדיניות</span><span class="sxs-lookup"><span data-stu-id="f32a7-116">Policy tips</span></span>
<span data-ttu-id="f32a7-117">להלן מספר הצעות שיכולות לסייע לך בעת יצירת מדיניות חדשה לניהול הוצאות.</span><span class="sxs-lookup"><span data-stu-id="f32a7-117">Here are a few suggestions that can assist you when creating new policies for expense management.</span></span> 
* <span data-ttu-id="f32a7-118">מדיניות נכנסת לתוקף בתאריך מסוים, והיא לא תיכנס לתוקף אם המדיניות נוצרה עם תאריך שהוא לאחר התאריך שבו התרחשה ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="f32a7-118">Policies are date effective and won't take effect if the policy is created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="f32a7-119">לדוגמא, אם אתה יוצר מדיניות חדשה היום לאכיפת הוצאה מקסימלית של ארוחה בסכום של $50, אז ההוצאות הקיימות שהוזנו החל מאתמול לא ייבדקו מול מדיניות זו.</span><span class="sxs-lookup"><span data-stu-id="f32a7-119">For example, if you are creating a new policy today to enforce a maximum meal expense of $50, then any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
* <span data-ttu-id="f32a7-120">בעת יצירת מדיניות עבור קטגוריית הוצאות שניתן לפרט, שקול להוסיף תנאי לסוג שורת ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="f32a7-120">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="f32a7-121">ייתכן שמדיניות מסוימת, כגון דרישת קבלה, אינה הגיונית עבור שורות מפורטות, ויש להחיל אותן רק על שורת הכותרת או על שורה שאינה ממוינת.</span><span class="sxs-lookup"><span data-stu-id="f32a7-121">Some policies such as requiring a receipt may not make sense for itemized lines and should only be applied to the header line or a non-itemized line.</span></span> 
* <span data-ttu-id="f32a7-122">מדיניות ניהול ההוצאות מוערכת מול ישות המקור כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="f32a7-122">Expense management policies are evaluated against the source entity by default.</span></span> <span data-ttu-id="f32a7-123">עבור תרחישים בין-עסקיים, באפשרותך להגדיר את המדיניות שתיבחן מול ישות היעד (ישות הלווה) במקום זאת.</span><span class="sxs-lookup"><span data-stu-id="f32a7-123">For intercompany scenarios, you can set the policy to be evaluated against the destination entity (borrowing entity) instead.</span></span> <span data-ttu-id="f32a7-124">להפעלת המדיניות כנגד ישות היעד, הפעל את התכונה "הערך את מדיניות ההוצאות כנגד ישות משפטית לווה" בסביבת העבודה **ניהול תכונות**.</span><span class="sxs-lookup"><span data-stu-id="f32a7-124">To run the policies against the destination entity, turn on the "Evaluate Expense policy against borrowing legal entity" feature in the **Feature Management** workspace.</span></span>

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="f32a7-125">מתי להעריך מדיניות</span><span class="sxs-lookup"><span data-stu-id="f32a7-125">When to evaluate policies</span></span>

<span data-ttu-id="f32a7-126">בפרמטרים של ניהול הוצאות, יש אפשרות לבחור להעריך את מדיניות ניהול ההוצאות כאשר שורה נשמרת או כאשר מוגש דוח הוצאות.</span><span class="sxs-lookup"><span data-stu-id="f32a7-126">In expense management parameters, there is an option to either evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="f32a7-127">אם תבחר להעריך מתי שורה נשמרת, זה מבטיח שהמשתמשים יראו בשלב מוקדם יותר מה עליהם לעשות כדי להשלים את דוח ההוצאות בבת אחת.</span><span class="sxs-lookup"><span data-stu-id="f32a7-127">If you choose to evaluate when a line is saved this ensures that users have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="f32a7-128">אחרת, אתה יכול לעכב את הערכת המדיניות ולחסוך זמן אם יש לך אימות בסוף, במהלך ההגשה לזרימת העבודה.</span><span class="sxs-lookup"><span data-stu-id="f32a7-128">Otherwise, you can delay policy evaluation and save time if you have validation occur at the end, during submission to workflow.</span></span>
