---
title: יצירת פתרון עבור ממדי תמחור מותאם אישית
description: נושא זה מספק מידע על הדרך ליצור פתרונות של ממדי תמחור מותאמים אישית.
author: Rumant
manager: tfehr
ms.date: 11/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 441501dff23d16960381b3f9fb4b2cceba2b3ba5
ms.sourcegitcommit: 869bde007805ef255f61b03937e4a44aeef61df9
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 11/12/2020
ms.locfileid: "4513987"
---
# <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="1f8a2-103">יצירת פתרון עבור ממדי תמחור מותאם אישית</span><span class="sxs-lookup"><span data-stu-id="1f8a2-103">Create a solution for custom pricing dimensions</span></span>

 <span data-ttu-id="1f8a2-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="1f8a2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span> 

>[!IMPORTANT]
><span data-ttu-id="1f8a2-105">כל השינויים בממדי התמחור המותאמים אישית צריכים להיות בפתרון נפרד.</span><span class="sxs-lookup"><span data-stu-id="1f8a2-105">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="1f8a2-106">שיטת עבודה מומלצת וחשובה זו מספקת את הגמישות לעדכן או להסיר שינויים בהתאם לצורך, היא מסייעת להשתמש מחדש בעבודה שכבר בוצעה והיא מאפשרת להפנות את השינויים הללו אל מופעים אחרים.</span><span class="sxs-lookup"><span data-stu-id="1f8a2-106">This important best practice allows the flexibility to update or remove changes as needed, helps with re-use of your work, and makes it easier to port changes to other instances.</span></span> <span data-ttu-id="1f8a2-107">לאחר ביצוע כל השינויים הדרושים, יצא פתרון זה כ **פתרון מנוהל** ויבא אותו אל מופעים אחרים לצורך שימוש חוזר.</span><span class="sxs-lookup"><span data-stu-id="1f8a2-107">After you make the required changes, export this solution as a **Managed** solution, and then import into other instances for reuse.</span></span>

## <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="1f8a2-108">יצירת פתרון עבור ממדי תמחור מותאם אישית</span><span class="sxs-lookup"><span data-stu-id="1f8a2-108">Create a solution for custom pricing dimensions</span></span>

1.  <span data-ttu-id="1f8a2-109">בחר **הגדרות** > **פתרונות**, ולאחר מכן בחר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="1f8a2-109">Select **Settings** > **Solutions**, and then select **New**.</span></span>
2.  <span data-ttu-id="1f8a2-110">תן שם לפתרון, *ממדי תמחור של <your organization name>*.</span><span class="sxs-lookup"><span data-stu-id="1f8a2-110">Name the solution, *<your organization name> pricing dimensions*.</span></span>
3. <span data-ttu-id="1f8a2-111">הזן את המידע הדרוש שנותר ולאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="1f8a2-111">Enter the remaining required information, and then select **Save**.</span></span>

  ![יצירת פתרון של ממד תמחור מותאם אישית](./media/Creation-of-custom-pricing-dimension-solution.png)
 
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="1f8a2-113">הוסף את כל הישויות הנדרשות ואת הרכיבים הקשורים לפתרון ממד התמחור</span><span class="sxs-lookup"><span data-stu-id="1f8a2-113">Add all required entities and related components to the Pricing dimension solution</span></span>

<span data-ttu-id="1f8a2-114">הוסף את הישויות הבאות של Project Service לפתרון התמחור שלך כדי לבצע שינויים חשובים בסכמה של פתרון התמחור.</span><span class="sxs-lookup"><span data-stu-id="1f8a2-114">Add the following Project Service entities to your pricing solution to make important schema changes in the pricing solution.</span></span> <span data-ttu-id="1f8a2-115">לאחר שתסיים תהליך זה, הישויות יזהו את ממדי התמחור החדשים.</span><span class="sxs-lookup"><span data-stu-id="1f8a2-115">After you have completed this procedure, the entities will recognize the new pricing dimensions.</span></span>

1.  <span data-ttu-id="1f8a2-116">בחר **הגדרות** > **פתרונות**, ולאחר מכן לחץ לחיצה כפולה על **<*שם הארגון שלך*> ממדי תמחור**.</span><span class="sxs-lookup"><span data-stu-id="1f8a2-116">Select **Settings** > **Solutions**, and then double-click **<*your organization name*> pricing dimensions**.</span></span>
2.  <span data-ttu-id="1f8a2-117">בסייר הפתרונות, בחלונית הניווט הימנית בחר **הוסף קיים**  > **ישויות**.</span><span class="sxs-lookup"><span data-stu-id="1f8a2-117">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3.  <span data-ttu-id="1f8a2-118">בתיבת הדו-שיח **רכיבי פתרון**, בחר את הישויות הבאות:</span><span class="sxs-lookup"><span data-stu-id="1f8a2-118">In the **Solution Components** dialog box, select the following entities:</span></span>
 
   - <span data-ttu-id="1f8a2-119">**בפועל**</span><span class="sxs-lookup"><span data-stu-id="1f8a2-119">**Actual**</span></span>
   - <span data-ttu-id="1f8a2-120">**משאב הניתן להזמנה**</span><span class="sxs-lookup"><span data-stu-id="1f8a2-120">**Bookable Resource**</span></span>
   - <span data-ttu-id="1f8a2-121">**שורת הערכה**</span><span class="sxs-lookup"><span data-stu-id="1f8a2-121">**Estimate Line**</span></span>
   - <span data-ttu-id="1f8a2-122">**משימת פרויקט**</span><span class="sxs-lookup"><span data-stu-id="1f8a2-122">**Project Task**</span></span>
   - <span data-ttu-id="1f8a2-123">**פרט בשורת חשבונית**</span><span class="sxs-lookup"><span data-stu-id="1f8a2-123">**Invoice Line Detail**</span></span>
   - <span data-ttu-id="1f8a2-124">**שורת יומן**</span><span class="sxs-lookup"><span data-stu-id="1f8a2-124">**Journal Line**</span></span>
   - <span data-ttu-id="1f8a2-125">**פרט סעיף חוזה של פרויקט**</span><span class="sxs-lookup"><span data-stu-id="1f8a2-125">**Project Contract Line Detail**</span></span>
   - <span data-ttu-id="1f8a2-126">**חבר צוות פרוייקט**</span><span class="sxs-lookup"><span data-stu-id="1f8a2-126">**Project Team Member**</span></span>
   - <span data-ttu-id="1f8a2-127">**פרטים בשורת הצעת מחיר**</span><span class="sxs-lookup"><span data-stu-id="1f8a2-127">**Quote Line Detail**</span></span>
   - <span data-ttu-id="1f8a2-128">**ייקור מחיר תפקיד**</span><span class="sxs-lookup"><span data-stu-id="1f8a2-128">**Role Price Markup**</span></span>
   - <span data-ttu-id="1f8a2-129">**מחיר תפקיד**</span><span class="sxs-lookup"><span data-stu-id="1f8a2-129">**Role Price**</span></span>
   - <span data-ttu-id="1f8a2-130">**ערך זמן**</span><span class="sxs-lookup"><span data-stu-id="1f8a2-130">**Time Entry**</span></span>
 
   ![הוסף ישויות קיימות לפתרון ממדי התמחור המותאם](./media/Existing-entities-to-PD-solution.png)
 
 4. <span data-ttu-id="1f8a2-132">עבור כל ישות, בדוק את הרכיבים שנוספו ואת הרשימה הסופית של נכסי הישות עבור כל ישות.</span><span class="sxs-lookup"><span data-stu-id="1f8a2-132">For each entity, review the components being added and the final list of entity assets for each entity.</span></span> 

   >[!NOTE]
   > <span data-ttu-id="1f8a2-133">כלול את כל הטפסים והתצוגות עבור כל אחת מהישויות שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="1f8a2-133">Include all forms and views for each of the selected entities.</span></span>

  ![ישויות שנוספו](./media/solution-component-selection.png)


5.  <span data-ttu-id="1f8a2-135">כאשר תתבקש לכלול ישויות תלויות עבור הישויות שנבחרו, בחר **לא, אל תכלול רכיבים נדרשים.**</span><span class="sxs-lookup"><span data-stu-id="1f8a2-135">When prompted to include any dependent entities for the selected entities, select **No, do not include required components.**</span></span>

    ![כולל ישויות תלויות](./media/Do-not-include-required.png)
