---
title: מבט כולל על הפקת חשבוניות בין-חברות
description: נושא זה מספק מידע ודוגמאות של חשבונית בין-חברות לפרויקטים.
author: sigitac
manager: tfehr
ms.date: 11/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 670b5d15ecf1ef7dcc034064e625814cbe6d54b0
ms.sourcegitcommit: addbe0647619413e85e7cde80f6a21db95ab623e
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 11/20/2020
ms.locfileid: "4595479"
---
# <a name="intercompany-invoicing-overview"></a><span data-ttu-id="f19dc-103">מבט כולל על הפקת חשבוניות בין-חברות</span><span class="sxs-lookup"><span data-stu-id="f19dc-103">Intercompany invoicing overview</span></span>

<span data-ttu-id="f19dc-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="f19dc-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="f19dc-105">ייתכן שלארגון שלך יש כמה חטיבות, חברות בנות וישויות משפטיות אחרות שמעבירות מוצרים ושירותים אחת לשנייה עבור פרוייקטים.</span><span class="sxs-lookup"><span data-stu-id="f19dc-105">Your organization might have multiple divisions, subsidiaries, and other legal entities that transfer products and services to each other for projects.</span></span> <span data-ttu-id="f19dc-106">הישות המשפטית שמספקת את השירות או המוצר נקראת *ישות משפטית מלווה*.</span><span class="sxs-lookup"><span data-stu-id="f19dc-106">The legal entity that provides the service or product is called the *lending legal entity*.</span></span> <span data-ttu-id="f19dc-107">הישות המשפטית שמקבלת את השירות או המוצר נקראת *ישות משפטית לווה*.</span><span class="sxs-lookup"><span data-stu-id="f19dc-107">The legal entity that receives the service or product is called the *borrowing legal entity*.</span></span>

<span data-ttu-id="f19dc-108">האיור הבא מציג תרחיש אופייני שבו שתי ישויות משפטיות, Contoso Robotics USA (הישות המשפטית הלווה) ו- Contoso Robotics UK (הישות המשפטית המלווה) חולקות משאבים להעברת פרויקט עבור הלקוח, Adventure Works.</span><span class="sxs-lookup"><span data-stu-id="f19dc-108">The following illustration shows a typical scenario where two legal entities, Contoso Robotics USA (the borrowing legal entity) and Contoso Robotics UK (the lending legal entity) share resources to deliver a project for the customer, Adventure works.</span></span> <span data-ttu-id="f19dc-109">עבור תרחיש זה, Contoso Robotics USA אמורה לספק את העבודה ל- Adventure Works.</span><span class="sxs-lookup"><span data-stu-id="f19dc-109">For this scenario, Contoso Robotics USA is contracted to deliver the work to Adventure Works.</span></span>

![הפקת חשבוניות בין-חברתית](./media/IntercompanyScenario.png) 

<span data-ttu-id="f19dc-111">Dynamics 365 Project Operations משתמש בזרימה הבאה לעיבוד עסקאות בין-חברות:</span><span class="sxs-lookup"><span data-stu-id="f19dc-111">Dynamics 365 Project Operations uses the following flow to process intercompany transactions:</span></span>

1. <span data-ttu-id="f19dc-112">משאבים מהישות המשפטית המלווה מתעדים עסקאות של זמן או הוצאות בין חברות על ידי קביעת זמן והוצאות על פרויקטים בישות המשפטית הלווה.</span><span class="sxs-lookup"><span data-stu-id="f19dc-112">Resources from the lending legal entity record intercompany time or expense transactions by booking time and expense against projects in the borrowing legal entity.</span></span>
2. <span data-ttu-id="f19dc-113">עלויות של זמן והוצאות נרשמות בחברה המלווה באמצעות מחירון העלות ליחידה של החברה הלווה.</span><span class="sxs-lookup"><span data-stu-id="f19dc-113">Time and expense costs are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
3. <span data-ttu-id="f19dc-114">עסקאות מכירות שלא חויבו בין החברות נרשמות בחברה המלווה באמצעות מחירון העלות ליחידה של החברה הלווה.</span><span class="sxs-lookup"><span data-stu-id="f19dc-114">Intercompany unbilled sale transactions are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
4. <span data-ttu-id="f19dc-115">הכנסות שלא חויבו נרשמות בחברה הלווה באמצעות מחירון המכירות של חוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="f19dc-115">Unbilled revenue is recorded in the borrowing company using the project contract sales price list.</span></span> <span data-ttu-id="f19dc-116">ניתן לחייב את הלקוח כאשר נרשמות הכנסות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="f19dc-116">The customer can be billed when unbilled revenue is recorded.</span></span> <span data-ttu-id="f19dc-117">הלקוח לא צריך לחכות עד לסיום העיבוד של חשבוניות בין-חברות.</span><span class="sxs-lookup"><span data-stu-id="f19dc-117">The customer doesn't have to wait until intercompany invoice processing is complete.</span></span>
5. <span data-ttu-id="f19dc-118">חשבוניות לקוחות בין חברות נוצרות על בסיס תקופתי בחברה המלווה.</span><span class="sxs-lookup"><span data-stu-id="f19dc-118">Intercompany customer invoices are created on a periodic basis in the lending company.</span></span> <span data-ttu-id="f19dc-119">החשבוניות נוצרות באופן ידני או בתהליך אוטומטי תקופתי.</span><span class="sxs-lookup"><span data-stu-id="f19dc-119">The invoices are created manually or by using a periodic automated process.</span></span> <span data-ttu-id="f19dc-120">ניתן ליצור חשבונית אחת עבור כל ישות משפטית לווה או ליצור חשבוניות נפרדות לפי פרויקט.</span><span class="sxs-lookup"><span data-stu-id="f19dc-120">A single invoice can be created for each borrowing legal entity or separate invoices can be created by project.</span></span>
6. <span data-ttu-id="f19dc-121">כאשר חשבונית הלקוח בין-חברות מתועדת בישות המשפטית המלווה, נוצרת חשבונית ספק מתאימה שממתינה בישות המשפטית הלווה.</span><span class="sxs-lookup"><span data-stu-id="f19dc-121">When the intercompany customer invoice is posted in the lending legal entity, the corresponding pending vendor invoice is created in the borrowing legal entity.</span></span> <span data-ttu-id="f19dc-122">העלויות בחשבונית הספק שבהמתנה יירשמו בספר המשני של הפרויקט עם רישום החשבונית.</span><span class="sxs-lookup"><span data-stu-id="f19dc-122">The costs in the pending vendor invoice will be recorded to the project subledger when the invoice is posted.</span></span>

<span data-ttu-id="f19dc-123">התרשים הבא מציג חשבוניות בין חברות כשהן קשורות לאירועים חשבונאיים ורישומים צפויים בספר הכללי.</span><span class="sxs-lookup"><span data-stu-id="f19dc-123">The following diagram illustrates intercompany invoicing as it relates to accounting events and expected postings to the general ledger.</span></span>

![זרימה בין-חברות](./media/IntercompanyFlow.png)

## <a name="additional-resources"></a><span data-ttu-id="f19dc-125">משאבים נוספים</span><span class="sxs-lookup"><span data-stu-id="f19dc-125">Additional resources</span></span>

- [<span data-ttu-id="f19dc-126">קביעת תצורה של הפקת חשבוניות בין-חברות</span><span class="sxs-lookup"><span data-stu-id="f19dc-126">Configure intercompany invoicing</span></span>](configure-intercompany-invoicing.md)
- [<span data-ttu-id="f19dc-127">תיעוד עסקאות בין-חברות</span><span class="sxs-lookup"><span data-stu-id="f19dc-127">Record intercompany transactions</span></span>](create-intercompany-transactions.md)
- [<span data-ttu-id="f19dc-128">יצירת חשבוניות לקוחות וספקים בין-חברות</span><span class="sxs-lookup"><span data-stu-id="f19dc-128">Create intercompany customer and vendor invoices</span></span>](create-intercompany-customer-vendor-invoices.md)
