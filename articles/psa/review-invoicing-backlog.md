---
title: סקירת המצבור להפקת חשבוניות בפרויקטים ובחוזים של פרויקטים
description: נושא זה מספק מידע המתאר כיצד לסקור מצבורי פריטי עבודה של זמן, הוצאה ומוצר, וכיצד לסמן אותם כמוכנים להפקת חשבונית.
author: rumant
ms.custom: ''
ms.author: rumant
ms.date: 03/11/2019
ms.topic: article
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: cec09ca39563e3faf0f3b2c10cf9bde3feb020b0
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6008537"
---
# <a name="review-the-invoicing-backlog-on-projects-and-project-contracts"></a><span data-ttu-id="ff460-103">סקירת המצבור להפקת חשבוניות בפרויקטים ובחוזים של פרויקטים</span><span class="sxs-lookup"><span data-stu-id="ff460-103">Review the invoicing backlog on projects and project contracts</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="ff460-104">כאשר עסקה מוכנה ליצירה ולעיבוד של חשבונית, יש לסמן את העסקה כ **מוכן להגיש חשבונית**.</span><span class="sxs-lookup"><span data-stu-id="ff460-104">When a transaction is ready to have an invoice created and processed, the transaction should be marked **Ready to invoice**.</span></span> <span data-ttu-id="ff460-105">נושא זה מתאר את סוגי העסקאות שניתן ליצור.</span><span class="sxs-lookup"><span data-stu-id="ff460-105">This topic describes the types of transactions that can be created.</span></span>

## <a name="review-the-time-and-material-billing-backlog"></a><span data-ttu-id="ff460-106">סקירה של מצבור חיוב הזמן והחומרים</span><span class="sxs-lookup"><span data-stu-id="ff460-106">Review the time and material billing backlog</span></span>

<span data-ttu-id="ff460-107">כאשר ערך זמן או הוצאה נשלחים ומאושרים עבור פרויקט כלשהו, PSA יוצר פרויקט בפועל.</span><span class="sxs-lookup"><span data-stu-id="ff460-107">When a time or expense entry is submitted and approved for a project, PSA creates a project actual.</span></span> <span data-ttu-id="ff460-108">אם השילוב של הפרויקט ומחלקת העסקה ממופים לסעיף חוזה עבור פרויקט של זמן וחומרים, נוצרים שני נתונים בפועל בעת אישור הערך:</span><span class="sxs-lookup"><span data-stu-id="ff460-108">If the combination of the project and the transaction class are mapped to a contract line for a time-and-materials project, two actuals are created when the entry is approved:</span></span>

- <span data-ttu-id="ff460-109">נתון בפועל של עלות</span><span class="sxs-lookup"><span data-stu-id="ff460-109">Cost actual</span></span> 
- <span data-ttu-id="ff460-110">נתון בפועל של מכירות שלא חויבו</span><span class="sxs-lookup"><span data-stu-id="ff460-110">Unbilled sales actual</span></span>

<span data-ttu-id="ff460-111">נתונים בפועל של מכירות שלא חויבו מייצגים את מצבור החיובים, ויש להגדיר את מצב החיוב שלהם ל **מוכן להגיש חשבונית**.</span><span class="sxs-lookup"><span data-stu-id="ff460-111">Unbilled sales actuals represent the billing backlog, and their billing status must be set to **Ready to Invoice**.</span></span> <span data-ttu-id="ff460-112">בעת יצירת חשבונית של פרויקט, נתונים בפועל של מכירות שלא חויבו, המסומנים כ **מוכן להגיש חשבונית**, מועתקים כפרטי שורת חשבונית.</span><span class="sxs-lookup"><span data-stu-id="ff460-112">When a project invoice is created, unbilled sales actuals that are marked **Ready to Invoice** are copied over as invoice line details.</span></span>

<span data-ttu-id="ff460-113">כדי לסקור את מצבור החיובים עבור זמן וחומרים, עבור אל **מכירות** \> **חיוב** \> **מצבור פריטי עבודה של חיוב זמן וחומרים‬**.</span><span class="sxs-lookup"><span data-stu-id="ff460-113">To review the billing backlog for time and materials, go to **Sales** \> **Billing** \> **Time and Material Billing Backlog**.</span></span> <span data-ttu-id="ff460-114">בחר את כל הנתונים בפועל של המכירות שלא חויבו, המוכנים להגשת חשבונית, ולאחר מכן בחר **מוכן להגיש חשבונית**.</span><span class="sxs-lookup"><span data-stu-id="ff460-114">Select all the unbilled sales actuals that are ready to be invoiced, and then select **Ready to Invoice**.</span></span> <span data-ttu-id="ff460-115">מצב החיוב של הנתונים בפועל משתנה ל **מוכן להגיש חשבונית**.</span><span class="sxs-lookup"><span data-stu-id="ff460-115">The billing status of these actuals is changed to **Ready to Invoice**.</span></span>

![מצבור פריטי עבודה של חיוב זמן וחומרים](media/TMBacklog.png)

## <a name="review-the-product-billing-backlog"></a><span data-ttu-id="ff460-117">סקירה של מצבור פריטי עבודה של חיוב מוצר</span><span class="sxs-lookup"><span data-stu-id="ff460-117">Review the product billing backlog</span></span>

<span data-ttu-id="ff460-118">ב- PSA, כאשר חוזה פרויקט כולל סעיפי חוזה מבוססי-מוצר, שורות אלה נחשבות להפקת חשבונית בכל פעם שנוצרת חשבונית עבור חוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ff460-118">In PSA, when a project contract has product-based contract lines, those lines are considered for invoicing whenever an invoice is created for the project contract.</span></span> <span data-ttu-id="ff460-119">כל מוצר שכולל סעיפי חוזה המסומנים כ **מוכן להגיש חשבונית** מועתק לחשבונית הפרויקט כשורות חשבונית של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="ff460-119">Any product that has contract lines that are marked **Ready to Invoice** is copied over to the project invoice as project invoice lines.</span></span>

<span data-ttu-id="ff460-120">כדי לסקור את מצבור פריטי העבודה של חיובי המוצרים, עבור אל **מכירות** \> **חיוב** \> **מצבור פריטי עבודה של חיוב מוצר‬**.</span><span class="sxs-lookup"><span data-stu-id="ff460-120">To review the billing backlog for products, go to **Sales** \> **Billing** \> **Product Billing Backlog**.</span></span> <span data-ttu-id="ff460-121">בחר את כל סעיפי החוזה מבוססי-המוצר המוכנים להגשת חשבונית, ולאחר מכן בחר **מוכן להגיש חשבונית**.</span><span class="sxs-lookup"><span data-stu-id="ff460-121">Select all the product-based contract lines that are ready to be invoiced, and then select **Ready to Invoice**.</span></span> <span data-ttu-id="ff460-122">מצב החיוב של סעיפים אלה משתנה ל **מוכן להגיש חשבונית**.</span><span class="sxs-lookup"><span data-stu-id="ff460-122">The billing status of these lines is changed to **Ready to Invoice**.</span></span>

![מצבור פריטי עבודה של חיוב מוצר](media/ProductBacklog.png)

## <a name="review-billing-milestones-on-fixed-price-contracts"></a><span data-ttu-id="ff460-124">סקירה של אבני דרך לחיוב בחוזי מחירים קבועים</span><span class="sxs-lookup"><span data-stu-id="ff460-124">Review billing milestones on fixed-price contracts</span></span>

<span data-ttu-id="ff460-125">כל סעיף חוזה של פרויקט הכולל שיטת חיוב של מחיר קבוע חייב להגדיר אבני דרך של חוזה.</span><span class="sxs-lookup"><span data-stu-id="ff460-125">Each project contract line that has a fixed-price billing method must define contract milestones.</span></span> <span data-ttu-id="ff460-126">ניתן להגיש חשבונית עבור אבני הדרך של חוזים אלה רק אם הם מסומנים כ **מוכן להגיש חשבונית**.</span><span class="sxs-lookup"><span data-stu-id="ff460-126">These contract milestones can be invoiced only if they are marked **Ready to Invoice**.</span></span> 

<span data-ttu-id="ff460-127">כדי לסקור אבני דרך של חיוב, עבור אל **מכירות** \> **חיוב** \> **אבני דרך של מחיר קבוע‬**.</span><span class="sxs-lookup"><span data-stu-id="ff460-127">To review billing milestones, go to **Sales** \> **Billing** \> **Fixed Price Milestones**.</span></span> <span data-ttu-id="ff460-128">בחר את אבני הדרך המוכנים להגשת חשבונית, ולאחר מכן בחר **מוכן להגיש חשבונית**.</span><span class="sxs-lookup"><span data-stu-id="ff460-128">Select the milestones that are ready to be invoiced, and then select **Ready to invoice**.</span></span> <span data-ttu-id="ff460-129">מצב החיוב של אבני דרך אלה משתנה ל **מוכן להגיש חשבונית**.</span><span class="sxs-lookup"><span data-stu-id="ff460-129">The billing status of these milestones is changed to **Ready to Invoice**.</span></span>

![אבני דרך של מחיר קבוע](media/FPBacklog.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]