---
title: יצירת פתרונות מותאמים אישית עבור ממדי תמחור
description: נושא זה מסביר כיצד ליצור פתרון מותאם אישית בעת יצירת ממדי תמחור מותאמים אישית.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 1d8117d6f6bcedc97264401fc941470f34efb1ae
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5284989"
---
# <a name="create-custom-solutions-for-pricing-dimensions"></a><span data-ttu-id="a66e2-103">יצירת פתרונות מותאמים אישית עבור ממדי תמחור</span><span class="sxs-lookup"><span data-stu-id="a66e2-103">Create custom solutions for pricing dimensions</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

> [!IMPORTANT]
> <span data-ttu-id="a66e2-104">כל השינויים בממדי התמחור המותאמים אישית צריכים להיות בפתרון נפרד.</span><span class="sxs-lookup"><span data-stu-id="a66e2-104">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="a66e2-105">שיטת עבודה מומלצת וחשובה זו מספקת גמישות בעתיד כדי לעדכן או להסיר שינויים בהתאם לצורך, היא תסייע לך להשתמש מחדש בעבודתך ומאפשרת להפנות את השינויים הללו אל מופע אחר בקלות רבה יותר.</span><span class="sxs-lookup"><span data-stu-id="a66e2-105">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="a66e2-106">לאחר ביצוע כל השינויים הדרושים, ייצא פתרון זה כ **פתרון מנוהל** ויבא אותו אל מופעים אחרים כדי להשתמש שוב בהגדרת התמחור.</span><span class="sxs-lookup"><span data-stu-id="a66e2-106">After you make the required changes, export this solution as a **Managed solution**, and import it into other instances to reuse your pricing setup.</span></span>

1. <span data-ttu-id="a66e2-107">בחר **הגדרות** > **פתרונות**, ולאחר מכן בחר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="a66e2-107">Select **Settings** > **Solutions**, and then select **New**.</span></span> 
2. <span data-ttu-id="a66e2-108">תן שם לפתרון, **\<your organization name> ממדי תמחור**, הזן את המידע הדרוש שנותר ובחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="a66e2-108">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then select **Save**.</span></span>

> ![יצירת פתרון מותאם אישית עבור ממדי תמחור](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="a66e2-110">הוסף את כל הישויות הנדרשות ואת הרכיבים הקשורים לפתרון ממד התמחור</span><span class="sxs-lookup"><span data-stu-id="a66e2-110">Add all required entities and related components to the Pricing dimension solution</span></span>
<span data-ttu-id="a66e2-111">יהיה עליך להוסיף את הישויות הבאות של Project Service לפתרון התמחור שלך.</span><span class="sxs-lookup"><span data-stu-id="a66e2-111">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="a66e2-112">השלם את השלבים שבהליך זה כדי לבצע שינויים חשובים בסכימה בפתרון התמחור כך שהישויות יהיו מודעות לממדי התמחור החדשים.</span><span class="sxs-lookup"><span data-stu-id="a66e2-112">Complete the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="a66e2-113">בחר **הגדרות** > **פתרונות** ולחץ פעמיים על **\<your organization name> ממדי תמחור**.</span><span class="sxs-lookup"><span data-stu-id="a66e2-113">Select **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="a66e2-114">בסייר הפתרונות, בחלונית הניווט הימנית בחר **הוסף קיים**  > **ישויות**.</span><span class="sxs-lookup"><span data-stu-id="a66e2-114">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="a66e2-115">בתיבת הדו-שיח **רכיבי פתרון**, בחר את הישויות הבאות:</span><span class="sxs-lookup"><span data-stu-id="a66e2-115">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="a66e2-116">בפועל</span><span class="sxs-lookup"><span data-stu-id="a66e2-116">Actual</span></span>
- <span data-ttu-id="a66e2-117">משאב הניתן להזמנה</span><span class="sxs-lookup"><span data-stu-id="a66e2-117">Bookable Resource</span></span>
- <span data-ttu-id="a66e2-118">שורת הערכה</span><span class="sxs-lookup"><span data-stu-id="a66e2-118">Estimate Line</span></span>
- <span data-ttu-id="a66e2-119">משימת פרויקט</span><span class="sxs-lookup"><span data-stu-id="a66e2-119">Project Task</span></span>
- <span data-ttu-id="a66e2-120">פרט בשורת חשבונית</span><span class="sxs-lookup"><span data-stu-id="a66e2-120">Invoice Line Detail</span></span>
- <span data-ttu-id="a66e2-121">שורת יומן</span><span class="sxs-lookup"><span data-stu-id="a66e2-121">Journal Line</span></span>
- <span data-ttu-id="a66e2-122">פרט סעיף חוזה של פרויקט</span><span class="sxs-lookup"><span data-stu-id="a66e2-122">Project Contract Line Detail</span></span>
- <span data-ttu-id="a66e2-123">חבר צוות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="a66e2-123">Project Team Member</span></span>
- <span data-ttu-id="a66e2-124">פרטים בשורת הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="a66e2-124">Quote Line Detail</span></span>
- <span data-ttu-id="a66e2-125">ייקור מחיר תפקיד</span><span class="sxs-lookup"><span data-stu-id="a66e2-125">Role Price Markup</span></span>
- <span data-ttu-id="a66e2-126">מחיר תפקיד</span><span class="sxs-lookup"><span data-stu-id="a66e2-126">Role Price</span></span> 
- <span data-ttu-id="a66e2-127">ערך זמן</span><span class="sxs-lookup"><span data-stu-id="a66e2-127">Time Entry</span></span> 

> ![הוספת ישויות קיימות לפתרון ממדי התמחור](media/Existing-entities-to-PD-solution.png)

> ![בחירת רכיבי פתרון](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="a66e2-130">הקפד לכלול את כל הטפסים והתצוגות עבור כל אחת מהישויות שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="a66e2-130">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="a66e2-131">כאשר תתבקש לכלול ישויות תלויות עבור הישויות שנבחרו, בחר **לא**.</span><span class="sxs-lookup"><span data-stu-id="a66e2-131">When prompted to include any dependent entities for the selected entities, select **No**.</span></span>

> ![אל תכלול את כל הרכיבים הקשורים](media/Do-not-include-required.png)




[!INCLUDE[footer-include](../includes/footer-banner.md)]