---
title: יצירת הצעות מחיר לפרויקט מהזדמנויות
description: נושא זה מספק מידע על יצירת הצעת מחיר לפוריקט מהזדמנות.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 606098473db479d0015e3a7a3c01a3d3b6de9db1
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077220"
---
# <a name="create-project-quotes-from-opportunities"></a><span data-ttu-id="920ae-103">יצירת הצעות מחיר לפרויקט מהזדמנויות</span><span class="sxs-lookup"><span data-stu-id="920ae-103">Create project quotes from opportunities</span></span>

<span data-ttu-id="920ae-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="920ae-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="920ae-105">ניתן ליצור הצעות מחיר מהזדמנויות פרויקט בדרכים הבאות:</span><span class="sxs-lookup"><span data-stu-id="920ae-105">Quotes can be created from project opportunities in the following ways:</span></span>

- <span data-ttu-id="920ae-106">מהכרטיסיה **הצעות מחיר** בדף **הזדמנות בפרויקט**</span><span class="sxs-lookup"><span data-stu-id="920ae-106">From the **Quotes** tab on the **Project Opportunity** page</span></span>
- <span data-ttu-id="920ae-107">מזרימת התהליך מכירות של ההזדמנות</span><span class="sxs-lookup"><span data-stu-id="920ae-107">From the Opportunity sales process flow</span></span>
- <span data-ttu-id="920ae-108">על ידי עדכון הפניה להזדמנות בהצעת מחיר קיימת</span><span class="sxs-lookup"><span data-stu-id="920ae-108">By updating the opportunity reference on an existing quote</span></span>

## <a name="from-the-quotes-tab-of-the-project-opportunity-page"></a><span data-ttu-id="920ae-109">מהכרטיסיה הצעות מחיר בדף הזדמנות בפרויקט</span><span class="sxs-lookup"><span data-stu-id="920ae-109">From the Quotes tab of the Project Opportunity page</span></span>

<span data-ttu-id="920ae-110">כדי ליצור הצעת מחיר מהזדמנות, בצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="920ae-110">To create a project quote from an opportunity, complete the following steps.</span></span>

1. <span data-ttu-id="920ae-111">פתח את הדף **הזדמנות בפרויקט** ובחר בכרטיסיה **הצעות מחיר**.</span><span class="sxs-lookup"><span data-stu-id="920ae-111">Open the **Project Opportunity** page and select the **Quotes** tab.</span></span> 
2. <span data-ttu-id="920ae-112">ברשת המשנה **הצעות מחיר** , בחר את הסימן **+** ליצרת הצעת מחיר חדשה שמבוססת על ההזדמנות.</span><span class="sxs-lookup"><span data-stu-id="920ae-112">On the **Quotes** sub-grid, select the **+** to create a new project quote based on the opportunity.</span></span> <span data-ttu-id="920ae-113">כל שורות ההזדמנות ומחירוני הפרויקט הקשורים מועתקים אל הצעת המחיר החדשה מההזדמנות.</span><span class="sxs-lookup"><span data-stu-id="920ae-113">All of the opportunity lines and related Project price lists are copied to the new quote from the opportunity.</span></span>

## <a name="from-the-opportunity-sales-process-flow"></a><span data-ttu-id="920ae-114">מזרימת התהליך מכירות של ההזדמנות</span><span class="sxs-lookup"><span data-stu-id="920ae-114">From the Opportunity sales process flow</span></span>

<span data-ttu-id="920ae-115">כדי ליצור הצעת מחיר מזרימת תהליך המכירות של הזדמנות, בצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="920ae-115">To create a quote from the Opportunity sales process flow, complete the following steps.</span></span>

1. <span data-ttu-id="920ae-116">מתהליך מכירת ההזדמנות, פתח את ההזדמנות.</span><span class="sxs-lookup"><span data-stu-id="920ae-116">From the Opportunity sales process flow, open the Opportunity.</span></span>
2. <span data-ttu-id="920ae-117">בחר את השלב **אישור**.</span><span class="sxs-lookup"><span data-stu-id="920ae-117">Select the **Qualify** stage.</span></span> 
3. <span data-ttu-id="920ae-118">בחר **הבא** ואז בחר **+ צור** כדי ליצור הצעת מחיר חדשה.</span><span class="sxs-lookup"><span data-stu-id="920ae-118">Select **Next** and then select **+ Create** to create a new quote.</span></span> <span data-ttu-id="920ae-119">רוב המידע בכרטיסיה **סיכום** עבור הצעת מחיר חדשה זו תוגדר כברירת מחדל מההזדמנות.</span><span class="sxs-lookup"><span data-stu-id="920ae-119">Most of the information on the **Summary** tab for this new quote will have defaulted from the opportunity.</span></span> 
4. <span data-ttu-id="920ae-120">הזן מידע נדרש שחסר, או עדכן את ערכי ברירת המחדל לפי הצורך בכרטיסיה **סיכום** ,</span><span class="sxs-lookup"><span data-stu-id="920ae-120">Enter in any required information that is missing, or update defaulted values as necessary on the **Summary** tab,</span></span>
5. <span data-ttu-id="920ae-121">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="920ae-121">Select **Save**.</span></span> <span data-ttu-id="920ae-122">הצעת המחיר החדשה נוצרה ומשויכת להזדמנות.</span><span class="sxs-lookup"><span data-stu-id="920ae-122">The new quote is created and associated to the opportunity.</span></span> <span data-ttu-id="920ae-123">כעת תוכל להציג את פרטי הצעת המחיר בכרטיסיה **הצעות מחיר** שבדף **הזדמנות**.</span><span class="sxs-lookup"><span data-stu-id="920ae-123">You can now view the quote information on the **Quotes** tab of the **Opportunity** page.</span></span> 

   <span data-ttu-id="920ae-124">תהליך המכירה של ההזדמנות עובר לשלב הבא, **הצעה**.</span><span class="sxs-lookup"><span data-stu-id="920ae-124">The Opportunity sales process moves to the next stage, **Propose**.</span></span>


## <a name="by-updating-the-opportunity-reference-on-an-existing-quote"></a><span data-ttu-id="920ae-125">על ידי עדכון הפניה להזדמנות בהצעת מחיר קיימת</span><span class="sxs-lookup"><span data-stu-id="920ae-125">By updating the opportunity reference on an existing quote</span></span>

<span data-ttu-id="920ae-126">ניתן לקשר הצעת מחיר קיימת להזדמנות.</span><span class="sxs-lookup"><span data-stu-id="920ae-126">An existing quote can be linked to an Opportunity.</span></span> <span data-ttu-id="920ae-127">בצע את השלבים הבאים כדי לעדכן את פרטי ההזדמנות בהצעת מחיר קיימת.</span><span class="sxs-lookup"><span data-stu-id="920ae-127">Complete the following steps to update the Opportunity information on an existing quote.</span></span>

1. <span data-ttu-id="920ae-128">פתח את הדף **הצעת מחיר** ובחר בכרטיסיה **סיכום**.</span><span class="sxs-lookup"><span data-stu-id="920ae-128">Open the **Quote** page and select the **Summary** tab.</span></span>
2. <span data-ttu-id="920ae-129">בשדה **הזדמנות** , בחר את ההזדמנות שברצונך לקשר להצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="920ae-129">In the **Opportunity** field, select the opportunity that you want to link to the quote.</span></span> <span data-ttu-id="920ae-130">ניתן לראות את הצעת המחיר ברשת **הצעות מחיר** של ההזדמנות.</span><span class="sxs-lookup"><span data-stu-id="920ae-130">You can see the quote in the **Quotes** grid of the Opportunity.</span></span> 
3. <span data-ttu-id="920ae-131">באמצעות תהליך המכירה של ההזדמנות, ניתן להעביר את ההזדמנות לשלב הבא, **הצעה**.</span><span class="sxs-lookup"><span data-stu-id="920ae-131">Using the Opportunity sales process, the opportunity can be moved to the next stage, **Propose**.</span></span> 

   <span data-ttu-id="920ae-132">כאשר מעבירים הזדמנות לשלב זה, ניתן לבחור בהצעת מחיר זו מתוך רשימת הצעות מחיר המשויכות להזדמנות זו.</span><span class="sxs-lookup"><span data-stu-id="920ae-132">When you move an opportunity to this stage, you can select this quote from a list of quotes associated with this opportunity.</span></span> <span data-ttu-id="920ae-133">בחירה בהצעת מחיר זו מצביעה על כך שאתה מתקדם איתה.</span><span class="sxs-lookup"><span data-stu-id="920ae-133">Selecting this quote indicates that you're moving forward with it.</span></span>

   <span data-ttu-id="920ae-134">כל שאר הצעות המחיר הקשורות להזדמנות עדיין יהיו זמינות ופעילות עד שאחת מהן זוכה.</span><span class="sxs-lookup"><span data-stu-id="920ae-134">All the other quotes associated with the Opportunity will still be available and active until one of them is won.</span></span> <span data-ttu-id="920ae-135">ניתן להחזיר את תהליך המכירה לשלב הקודם **אישור** , ולבחור הצעת מחיר אחרת להתקדם איתה.</span><span class="sxs-lookup"><span data-stu-id="920ae-135">You can move the sales process back to the previous stage **Qualify** , and pick another quote to move forward with.</span></span>
