---
title: יצירת מחירון
description: כיצד ליצור מחירון ב- Project Service
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: 08d93ad86d782922df6b22370749628ddbdc0718
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122029"
---
# <a name="create-a-price-list-project-service"></a><span data-ttu-id="917df-103">יצירת מחירון (Project Service)</span><span class="sxs-lookup"><span data-stu-id="917df-103">Create a price list (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="917df-104">מחירונים מספקים תבנית שמנהלי תיקי הלקוחות שלך יכולים להשתמש בה ליצירת הצעות מחיר ופרוייקטים ולקביעת עלויות פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="917df-104">Price lists provide a template your account managers can use for creating quotes and projects, and for establishing the costs of a project.</span></span> <span data-ttu-id="917df-105">הם מספקים רשימת פריטי שורה של תפקידים והוצאות, ואת המחיר שבו תחייב עבור כל אחד מהם.</span><span class="sxs-lookup"><span data-stu-id="917df-105">They provide a line item list of roles and expenses, and the price you will charge for each.</span></span> <span data-ttu-id="917df-106">ניתן ליצור מחירונים מרובים כך שתוכל לנהל מבני מחירים נפרדים עבור אזורים שונים שבהם אתה מוכר את המוצרים או ערוצי מכירות שונים.</span><span class="sxs-lookup"><span data-stu-id="917df-106">You can create multiple price lists so that you can maintain separate price structures for different regions you sell your products in or for different sales channels.</span></span> <span data-ttu-id="917df-107">זהו רעיון טוב ליצור לפחות מחירון אחד עבור כל מטבע שבו אתה מתכוון לחייב את הלקוחות שלך.</span><span class="sxs-lookup"><span data-stu-id="917df-107">It’s a good idea to create at least one price list for every currency you plan to bill your customers in.</span></span>  
  
<span data-ttu-id="917df-108">ליצירת הערכות פיננסיות עבור העבודה למסירה, ודא כי לכל פרוייקט יש גיבוי למחירון מכירות ומחיר עלות.</span><span class="sxs-lookup"><span data-stu-id="917df-108">To create financial estimates for the work to be delivered, make sure every project has a backing cost and sales price list.</span></span> <span data-ttu-id="917df-109">הגדר ברירת מחדל למחירון מכירות ומחיר עלות שחלה על כל הפרוייקטים שנוצרו בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="917df-109">Set up a default cost and sales pricelist that applies to all projects created in your organization.</span></span>  
  
<span data-ttu-id="917df-110">מחירונים מסתמכים על תפקידים וקטגוריות הוצאות, לכן לפני יצירת מחירון, ודא שכבר הגדרת את התפקידים ואת קטגוריות ההוצאות שבהם ברצונך להשתמש בעת יצירת המחירון.</span><span class="sxs-lookup"><span data-stu-id="917df-110">Price lists rely on roles and expense categories, so before you create a price list, make sure you’ve already configured the roles and expense categories you want to use while creating the price list.</span></span>  
  
1.  <span data-ttu-id="917df-111">עבור אל **Project Service > מחירונים**.</span><span class="sxs-lookup"><span data-stu-id="917df-111">Go to **Project Service > Price Lists**.</span></span>  
  
2.  <span data-ttu-id="917df-112">לחץ על **חדש**.</span><span class="sxs-lookup"><span data-stu-id="917df-112">Click **New**.</span></span>  
  
3.  <span data-ttu-id="917df-113">במקטע **הקשר**, בחר אם מחירון זה הוא עבור **עלות**, **רכש**, או **מכירות**.</span><span class="sxs-lookup"><span data-stu-id="917df-113">In **Context**, select whether this price list is for **Cost**, **Purchase**, or **Sales**.</span></span>  
  
4.  <span data-ttu-id="917df-114">במקטע **שם**, הזן שם עבור המחירון.</span><span class="sxs-lookup"><span data-stu-id="917df-114">In **Name**, enter a name for the price list.</span></span>  
  
5.  <span data-ttu-id="917df-115">במקטע **מטבע**, בחר את המטבע שאתה מתכוון להשתמש בו לחיוב או לתמחיר.</span><span class="sxs-lookup"><span data-stu-id="917df-115">In **Currency**, select the currency you’re going to use for billing or costing.</span></span>  
  
6.  <span data-ttu-id="917df-116">במקטע **יחידת זמן**, ציין את תקופת הזמן שעליה חל המחיר, כגון יום או שעה.</span><span class="sxs-lookup"><span data-stu-id="917df-116">In **Time Unit**, specify the period of time the price applies to, such as day or hour.</span></span>  
  
7.  <span data-ttu-id="917df-117">מלא **תאריך התחלה**, **תאריך סיום**, ו **תיאור** לפי הצורך.</span><span class="sxs-lookup"><span data-stu-id="917df-117">Fill in the **Start Date**, **End Date**, and **Description** as needed.</span></span>  
  
8.  <span data-ttu-id="917df-118">לחץ על **שמור** כדי ליצור את הרשומה כך שתוכל להמשיך לערוך אותה.</span><span class="sxs-lookup"><span data-stu-id="917df-118">Click **Save** to create the record so you can continue editing it.</span></span>  
  
9. <span data-ttu-id="917df-119">כדי להוסיף מחיר תפקיד למחירון, לחץ על **+** תחת **מחירי תפקיד**.</span><span class="sxs-lookup"><span data-stu-id="917df-119">To add a role price to the price list, click **+** under **Role prices**.</span></span>  
  
10. <span data-ttu-id="917df-120">בחלונית **מחיר תפקיד** , מלא את הפרטים ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="917df-120">In the **Role Price** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="917df-121">המשך להוסיף מחירי תפקיד לפי הצורך.</span><span class="sxs-lookup"><span data-stu-id="917df-121">Continue adding role prices as necessary.</span></span> <span data-ttu-id="917df-122">אחרי שתסיים, לחץ על **שמור** בפינה הימנית התחתונה של המסך.</span><span class="sxs-lookup"><span data-stu-id="917df-122">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
11. <span data-ttu-id="917df-123">כדי להוסיף מחיר קטגוריית הוצאה למחירון, לחץ על **+** תחת **מחירי קטגוריה**.</span><span class="sxs-lookup"><span data-stu-id="917df-123">To add an expense category price to the price list, click **+** under **Category prices**.</span></span>  
  
12. <span data-ttu-id="917df-124">בחלונית **מחיר קטגוריית עסקה** , מלא את הפרטים ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="917df-124">In the **Transaction Category Price** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="917df-125">המשך להוסיף מחירי קטגוריה לפי הצורך.</span><span class="sxs-lookup"><span data-stu-id="917df-125">Continue adding category prices as necessary.</span></span> <span data-ttu-id="917df-126">אחרי שתסיים, לחץ על **שמור** בפינה הימנית התחתונה של המסך.</span><span class="sxs-lookup"><span data-stu-id="917df-126">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
13. <span data-ttu-id="917df-127">כדי להוסיף פריטי מחירון למחירון, לחץ על **+** תחת **פריטי מחירון**.</span><span class="sxs-lookup"><span data-stu-id="917df-127">To add price list items to the price list, click **+** under **Price List Items**.</span></span>  
  
14. <span data-ttu-id="917df-128">בחלונית **פריט מחירון** , מלא את הפרטים ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="917df-128">In the **Price List Item** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="917df-129">המשך להוסיף פריטי מחירון לפי הצורך.</span><span class="sxs-lookup"><span data-stu-id="917df-129">Continue adding price list items as necessary.</span></span> <span data-ttu-id="917df-130">אחרי שתסיים, לחץ על **שמור** בפינה הימנית התחתונה של המסך.</span><span class="sxs-lookup"><span data-stu-id="917df-130">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
15. <span data-ttu-id="917df-131">כדי להוסיף קשרים בין אזורים למחירון, לחץ על **+** תחת **קשרים בין אזורים**.</span><span class="sxs-lookup"><span data-stu-id="917df-131">To add territory relationships to the price list, click **+** under **Territory Relationships**.</span></span>  
  
16. <span data-ttu-id="917df-132">בחלונית **חיבור חדש** , מלא את הפרטים ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="917df-132">In the **New Connection** window, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="917df-133">המשך להוסיף קשרים בין אזורים לפי הצורך.</span><span class="sxs-lookup"><span data-stu-id="917df-133">Continue adding territory relationships as necessary.</span></span> <span data-ttu-id="917df-134">אחרי שתסיים, לחץ על **שמור** בפינה הימנית התחתונה של המסך.</span><span class="sxs-lookup"><span data-stu-id="917df-134">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="917df-135">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="917df-135">See Also</span></span>  
 [<span data-ttu-id="917df-136">הגדרת Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="917df-136">Configure Project Service Automation</span></span>](../psa/configure.md)
