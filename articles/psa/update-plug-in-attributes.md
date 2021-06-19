---
title: עדכון תכונות של יישום Plug-in כדי לכלול ממדי תמחור חדשים
description: נושא זה מספק מידע על עדכון תכונות של יישום Plug-in עבור ממדי תמחור.
author: Rumant
ms.custom: ''
ms.date: 11/19/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: b0d50733340f277453f4ef5b52bdd3ee089449cd
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012812"
---
# <a name="update-plug-in-attributes-to-include-new-pricing-dimensions"></a><span data-ttu-id="91154-103">עדכון תכונות של יישום Plug-in כדי לכלול ממדי תמחור חדשים</span><span class="sxs-lookup"><span data-stu-id="91154-103">Update plug-in attributes to include new pricing dimensions</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

> [!NOTE]
> <span data-ttu-id="91154-104">אם אינך משתמש בתכונות 'יצירת הצעת מחיר' ו'חוזה' של Project Service Automation ‏(PSA), אתה מוזמן לדלג על נושא זה.</span><span class="sxs-lookup"><span data-stu-id="91154-104">If you are not using the Project Service Automation (PSA) Quoting and Contracting features, you can skip this topic.</span></span>

<span data-ttu-id="91154-105">נושא זה יוצא מנקודת הנחה שהשלמת את ההליכים בנושאים [יצירת שדות וישויות מותאמים אישית](create-custom-fields-entities.md), [הוספת שדות מותאמים אישית להגדרת מחיר וישויות של עסקאות](field-references.md) ו[הגדרת שדות מותאמים אישית כממדי תמחור](set-up-pricing-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="91154-105">This topic assumes that you have completed the procedures in the topics, [Create custom fields and entities](create-custom-fields-entities.md), [Add custom fields to price setup and transactional entities](field-references.md), and [Set up custom fields as pricing dimensions](set-up-pricing-dimensions.md).</span></span> <span data-ttu-id="91154-106">אם לא השלמת הליכים אלה, חזור והשלם אותם ולאחר מכן חזור לנושא זה.</span><span class="sxs-lookup"><span data-stu-id="91154-106">If you haven't completed those procedures, go back and complete them and then return to this topic.</span></span>

<span data-ttu-id="91154-107">בעת יצירת פרט של שורת הצעת מחיר בדף **שורת הצעת מחיר** של שורת הצעת מחיר של פרויקט, המערכת יוצרת שתי שורות הערכה ברקע – שורה אחת עבור צד העלות של ההערכה ושורה אחת עבור צד המכירות.</span><span class="sxs-lookup"><span data-stu-id="91154-107">When a quote line detail is created on the **Quote Line** page for a project quote line, the system creates two estimate lines in the background -- one line for the cost side of the estimate and one for sales side.</span></span> <span data-ttu-id="91154-108">אותה פעולה מתבצעת עבור סעיפי חוזה של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="91154-108">This is the same  for project contract lines.</span></span>

<span data-ttu-id="91154-109">בעת ביצוע שינוי בכמות או בשדה שבצד העלות, השינוי מופץ לצד המכירות.</span><span class="sxs-lookup"><span data-stu-id="91154-109">When you make a change to the quantity or a field on the cost side, that change is propagated to the sales side.</span></span> <span data-ttu-id="91154-110">הדבר אפשרי בזכות יישומי ה- Plug-in הבאים שיש לרשום מחדש לאחר כל שינוי בממדי התמחור.</span><span class="sxs-lookup"><span data-stu-id="91154-110">This is possible because of the following plug-ins that must be re-registered after a change to pricing dimensions.</span></span>

- <span data-ttu-id="91154-111">PreOperationContractLineDetailUpdate - Updates **msdyn_orderlinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="91154-111">PreOperationContractLineDetailUpdate - Updates **msdyn_orderlinetransaction**.</span></span>
- <span data-ttu-id="91154-112">PreOperationQuoteLineDetailUpdate - Updates **msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="91154-112">PreOperationQuoteLineDetailUpdate - Updates **msdyn_quotelinetransaction**.</span></span>

<span data-ttu-id="91154-113">השלבים הבאים מסבירים לך את תהליך הרישום של יישומי ה- Plug-in.</span><span class="sxs-lookup"><span data-stu-id="91154-113">The following steps walk you through the process of registering the plug-ins.</span></span>

1. <span data-ttu-id="91154-114">פתח את הכלי **PluginRegistrationTool** והתחבר למופע המקוון שלך.</span><span class="sxs-lookup"><span data-stu-id="91154-114">Open the **PluginRegistrationTool** and connect to your online instance.</span></span>
2. <span data-ttu-id="91154-115">לחץ על **חיפוש** וחפש את יישום ה- Plug-in לעדכון.</span><span class="sxs-lookup"><span data-stu-id="91154-115">Click **Search** and search for the plug-in to be updated.</span></span>

 ![צילום מסך של עץ החיפוש](media/PRT-1.png)

3. <span data-ttu-id="91154-117">לאחר מציאת יישום ה- Plug-in, בחר אותו ולאחר מכן לחץ על **בחר בטופס הראשי**.</span><span class="sxs-lookup"><span data-stu-id="91154-117">After the plug-in is found, select it and then click **Select on Main Form**.</span></span>

4. <span data-ttu-id="91154-118">בחר את השלב של יישום ה- plug-in לעדכון, לחץ באמצעות לחצן העכבר הימני ולאחר מכן בחר **עדכן**.</span><span class="sxs-lookup"><span data-stu-id="91154-118">Select the step of the plug-in to be updated, right-click, and then select **Update**.</span></span>

 ![צילום מסך של יישום ה- Plug-in לעדכון](media/PRT-2.png)
 
5. <span data-ttu-id="91154-120">בחלון העדכון, לחץ על שלוש הנקודות (**...**) בתכונות הסינון.</span><span class="sxs-lookup"><span data-stu-id="91154-120">In the update window, click the ellipsis (**...**) in the filtering attributes.</span></span>

 ![צילום מסך של פרטי התצורה של עדכון השלב הנוכחי](media/PRT-3.png)
 
6. <span data-ttu-id="91154-122">בחר את תיבות הסימון של תכונות התמחור.</span><span class="sxs-lookup"><span data-stu-id="91154-122">Select the pricing attribute check boxes.</span></span>

 ![צילום מסך המציג בחירת תיבות סימון של תכונות תמחור](media/PRT-4.png)

7. <span data-ttu-id="91154-124">לחץ על **אישור** כדי לסגור את הדף ולאחר מכן בחר **עדכן שלב**.</span><span class="sxs-lookup"><span data-stu-id="91154-124">Click **OK** to close the page and then select **Update Step**.</span></span>

 ![צילום מסך המציג את הלחצן 'עדכן שלב'](media/PRT-5.png)
 
8. <span data-ttu-id="91154-126">חזור על תהליך זה עבור יישום ה- Plug-in השני, **PreOperationQuoteLineDetail - Update of msdyn_quotelinetransaction**.</span><span class="sxs-lookup"><span data-stu-id="91154-126">Repeat this process for the second plug-in, **PreOperationQuoteLineDetail - Update of msdyn_quotelinetransaction**.</span></span>

9. <span data-ttu-id="91154-127">סגור את כלי הרישום של יישומי ה- Plug-in.</span><span class="sxs-lookup"><span data-stu-id="91154-127">Close the plug-in registration tool.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]