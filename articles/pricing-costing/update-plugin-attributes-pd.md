---
title: עדכון תכונות של יישום plug-in עם ממדי תמחור חדשים
description: נושא זה מספק מידע על הדרך לעדכן תכונות של יישום Plug-in עבור ממדי תמחור.
author: rumant
ms.date: 11/18/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 54b87a993929edbf89ef48741ba0a06c6c42ec4e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004622"
---
# <a name="update-plug-in-attributes-with-new-pricing-dimensions"></a><span data-ttu-id="465de-103">עדכון תכונות של יישום plug-in עם ממדי תמחור חדשים</span><span class="sxs-lookup"><span data-stu-id="465de-103">Update plug-in attributes with new pricing dimensions</span></span>

<span data-ttu-id="465de-104">נושא זה מספק מידע על הדרך לעדכן תכונות של יישום Plug-in עבור ממדי תמחור.</span><span class="sxs-lookup"><span data-stu-id="465de-104">This topic provides information about how to update plug-in attributes for pricing dimensions.</span></span>

> [!NOTE]
> <span data-ttu-id="465de-105">נושא זה חל רק על התכונות של הצעות מחיר וחוזה ב- Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="465de-105">This topic is only applicable to the quote and contract features in Dynamics 365 Project Operations.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="465de-106">דרישות מוקדמות</span><span class="sxs-lookup"><span data-stu-id="465de-106">Prerequisites</span></span>
<span data-ttu-id="465de-107">לפני שתשלים את השלבים בנושא זה, עליך להשלים את ההליכים בנושאים הבאים:</span><span class="sxs-lookup"><span data-stu-id="465de-107">Before you complete the steps in this topic, you must have completed the procedures in the following topics:</span></span>

  - [<span data-ttu-id="465de-108">יצירת שדות וישויות מותאמים אישית</span><span class="sxs-lookup"><span data-stu-id="465de-108">Create custom fields and entities</span></span>](create-custom-fields-entities-pricing-dimensions.md) 
  - [<span data-ttu-id="465de-109">הוספת שדות מותאמים אישית לישויות הגדרת מחיר וישויות של עסקאות </span><span class="sxs-lookup"><span data-stu-id="465de-109">Add custom fields to price setup and transactional entities</span></span>](add-custom-fields-price-setup-transactional-entities.md)
  - <span data-ttu-id="465de-110">[הגדרת שדות מותאמים אישית כממדי תמחור](set-up-custom-fields-pricing-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="465de-110">[Set up custom fields as pricing dimensions](set-up-custom-fields-pricing-dimensions.md).</span></span> 
  
<span data-ttu-id="465de-111">אם לא השלמת הליכים אלה, עליך להשלים אותם ולאחר מכן לחזור לנושא זה.</span><span class="sxs-lookup"><span data-stu-id="465de-111">If you haven't completed those procedures, complete them and then return to this topic.</span></span>

## <a name="register-a-plug-in"></a><span data-ttu-id="465de-112">רשום יישום plug-in</span><span class="sxs-lookup"><span data-stu-id="465de-112">Register a plug-in</span></span>
<span data-ttu-id="465de-113">כאשר נוצר פרט של שורת הצעת מחיר בדף **שורת הצעת מחיר** עבור שורת הצעת מחיר של פרויקט, המערכת יוצרת שתי שורות אומדן.</span><span class="sxs-lookup"><span data-stu-id="465de-113">When a quote line detail is created on the **Quote Line** page for a project quote line, the system creates two estimate lines.</span></span> <span data-ttu-id="465de-114">שורה אחת מיועדת לצד העלות של האומדן והשורה השנייה מיועדת למכירות.</span><span class="sxs-lookup"><span data-stu-id="465de-114">One line is for the cost side of the estimate and the other line is for sales the side.</span></span> <span data-ttu-id="465de-115">אותה פעולה מתבצעת עבור סעיפי חוזה של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="465de-115">This is the same  for project contract lines.</span></span>

<span data-ttu-id="465de-116">בעת ביצוע שינוי בכמות או בשדה שבצד העלות, השינוי מופץ גם לצד המכירות.</span><span class="sxs-lookup"><span data-stu-id="465de-116">When you make a change to the quantity or a field on the cost side, that change is also made on the sales side.</span></span> <span data-ttu-id="465de-117">זה אפשרי מכיוון שיישומי plug-in של PreOperation ב- Quotelinedetail ובישויות פרטי חוזה מחוברים עם מאפיינים ספציפיים מצד העלות לצד המכירות של העסקה.</span><span class="sxs-lookup"><span data-stu-id="465de-117">This is possible because the PreOperation plug-ins on Quotelinedetail and contractline detail entities connect specific attributes on the cost side to the sales side of the transaction.</span></span> <span data-ttu-id="465de-118">אם אתה צריך ששינויים בערכי ממד התמחור בצד המכירות ייערכו גם בצד העלות, יש לרשום מחדש את יישומי ה-plug-in הבאים לאחר ביצוע שינויים בממד התמחור.</span><span class="sxs-lookup"><span data-stu-id="465de-118">If you need changes made to the pricing dimension values on the sales side to also be made on the cost side, the following plug-ins must be re-registered after making changes to a pricing dimension.</span></span>

<span data-ttu-id="465de-119">אלה יישומי ה-plug-in לעדכון ורישום מחדש:</span><span class="sxs-lookup"><span data-stu-id="465de-119">These are the plug-ins to update and re-register:</span></span>

- <span data-ttu-id="465de-120">PreOperationContractLineDetailUpdate - **מעדכן את msdyn_orderlinetransaction**</span><span class="sxs-lookup"><span data-stu-id="465de-120">PreOperationContractLineDetailUpdate - **Update msdyn_orderlinetransaction**</span></span>
- <span data-ttu-id="465de-121">PreOperationQuoteLineDetailUpdate - **מעדכן את msdyn_quotelinetransaction**</span><span class="sxs-lookup"><span data-stu-id="465de-121">PreOperationQuoteLineDetailUpdate - **Updates msdyn_quotelinetransaction**</span></span>

<span data-ttu-id="465de-122">השלם את השלבים הבאים לעדכון ורישום מחדש של יישומי plug-in.</span><span class="sxs-lookup"><span data-stu-id="465de-122">Complete the following steps to update and re-register the plug-ins.</span></span>

1. <span data-ttu-id="465de-123">פתח את **PluginRegistrationTool** והתחבר לסביבת Project Operations שלך ב- Dataverse.</span><span class="sxs-lookup"><span data-stu-id="465de-123">Open **PluginRegistrationTool** and connect to your Project Operations Dataverse environment.</span></span>
2. <span data-ttu-id="465de-124">בחר **חפש** והקלד את האותיות הראשונות של יישום plug-in שיעודכן.</span><span class="sxs-lookup"><span data-stu-id="465de-124">Select **Search**, and type in the first few letters of the plug-in to be updated.</span></span>
3. <span data-ttu-id="465de-125">לאחר מציאת יישום ה- Plug-in, בחר אותו ולאחר מכן בחר **בחר בטופס הראשי**.</span><span class="sxs-lookup"><span data-stu-id="465de-125">After the plug-in is found, select it, and then select **Select on Main Form**.</span></span>
4. <span data-ttu-id="465de-126">בחר את השלב **Update msdyn_orderlinetransaction**, לחץ באמצעות לחצן העכבר הימני ולאחר מכן בחר **עדכן**.</span><span class="sxs-lookup"><span data-stu-id="465de-126">Select the **Update msdyn_orderlinetransaction** step, right-click, and then select **Update**.</span></span>
5. <span data-ttu-id="465de-127">בחלון **עדכון**, לחץ על שלוש הנקודות (**...**) בתכונות הסינון.</span><span class="sxs-lookup"><span data-stu-id="465de-127">In the **Update** dialog page, select the ellipsis (**...**) in the filtering attributes.</span></span>
6. <span data-ttu-id="465de-128">חלון מאפייני הסינון נפתח עם רשימה של כל התכונות בישות וממדי התמחור.</span><span class="sxs-lookup"><span data-stu-id="465de-128">The filtering attributes window opens and provides a list of all attributes in the entity and the pricing dimensions.</span></span> <span data-ttu-id="465de-129">בחר את תיבות הסימון עבור מאפייני ממד התמחור.</span><span class="sxs-lookup"><span data-stu-id="465de-129">Select the check boxes for the pricing dimension attributes.</span></span>
7. <span data-ttu-id="465de-130">בחר **אישור** כדי לסגור את הדף ולאחר מכן בחר **עדכן שלב**.</span><span class="sxs-lookup"><span data-stu-id="465de-130">Select **OK** to close the page, and then select **Update Step**.</span></span>
8. <span data-ttu-id="465de-131">חזור על שלבים 2 עד 7 עבור יישום ה-plug-in השני, **PreOperationQuoteLineDetail**.</span><span class="sxs-lookup"><span data-stu-id="465de-131">Repeat steps 2-7 for the second plug-in, **PreOperationQuoteLineDetail**.</span></span> <span data-ttu-id="465de-132">עבור יישום plug-in זה, עליך לעדכן את השלב **Update of msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="465de-132">For this plug-in, you need to update the **Update of msdyn_quotelinetransaction** step.</span></span>
9. <span data-ttu-id="465de-133">סגור את **PluginRegistrationTool**.</span><span class="sxs-lookup"><span data-stu-id="465de-133">Close **PluginRegistrationTool**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]