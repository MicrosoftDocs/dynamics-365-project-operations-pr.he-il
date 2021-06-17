---
title: הגדרת תצורה של הפקת חשבונית פרוייקט בין-חברתית
description: נושא זה מראה כיצד להגדיר הפקת חשבונית לפרוייקט בין שתי חברות בארגון.
author: Yowelle
ms.date: 07/29/2019
ms.topic: business-process
ms.prod: ''
ms.technology: ''
ms.search.form: VendTable, InterCompanyTradingRelationSetupVendor, SysDataAreaSelectLookup, ProjParameters, ProjPosting, ProjTransferPrice
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: ad25aba492b7902ddd8955be87f88f96f6d4508f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001202"
---
# <a name="configure-intercompany-project-invoicing"></a><span data-ttu-id="acff9-103">הגדרת תצורה של הפקת חשבונית פרוייקט בין-חברתית</span><span class="sxs-lookup"><span data-stu-id="acff9-103">Configure intercompany project invoicing</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="acff9-104">נושא זה מראה כיצד להגדיר הפקת חשבונית לפרוייקט בין שתי חברות בארגון.</span><span class="sxs-lookup"><span data-stu-id="acff9-104">This topic shows how to set up project invoicing between two companies in your organization.</span></span> <span data-ttu-id="acff9-105">משימה זו משתמשת בערכת נתונים של USSI.</span><span class="sxs-lookup"><span data-stu-id="acff9-105">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="acff9-106">בחלונית הניווט, עבור אל **מודולים > חשבונות זכאים > ספקים > כל הספקים**.</span><span class="sxs-lookup"><span data-stu-id="acff9-106">In the navigation pane, go to **Modules > Accounts payable > Vendors > All vendors**.</span></span>
2. <span data-ttu-id="acff9-107">ברשימה **כל הספקים**, מצא את הרשומה הרצויה ובחר אותה.</span><span class="sxs-lookup"><span data-stu-id="acff9-107">In the **All vendors** list, find and select the desired record.</span></span>
3. <span data-ttu-id="acff9-108">בחלונית הפעולות בחר **כללי**.</span><span class="sxs-lookup"><span data-stu-id="acff9-108">On the Action Pane, select **General**.</span></span>
4. <span data-ttu-id="acff9-109">בחר **בין-חברתי**.</span><span class="sxs-lookup"><span data-stu-id="acff9-109">Select **Intercompany**.</span></span>
5. <span data-ttu-id="acff9-110">הגדר את **פעיל** בתור **כן** כדי להפעיל מסחר בין-חברתי.</span><span class="sxs-lookup"><span data-stu-id="acff9-110">Set **Active** to **Yes** to enable intercompany trading.</span></span>
6. <span data-ttu-id="acff9-111">בשדה **חברת לקוח**, הזן או בחר ערך.</span><span class="sxs-lookup"><span data-stu-id="acff9-111">In the **Customer company** field, enter or select a value.</span></span>
7. <span data-ttu-id="acff9-112">בשדה **החשבון שלי**, הזן או בחר ערך.</span><span class="sxs-lookup"><span data-stu-id="acff9-112">In the **My account** field, enter or select a value.</span></span>
8. <span data-ttu-id="acff9-113">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="acff9-113">Select **Save**.</span></span>
9. <span data-ttu-id="acff9-114">סגור את הדפים כדי לחזור לדף הבית.</span><span class="sxs-lookup"><span data-stu-id="acff9-114">Close the pages to return to the home page.</span></span>
10. <span data-ttu-id="acff9-115">בחלונית הניווט, עבור אל **מודולים > ניהול פרוייקטים וחשבונאות > הגדרה > ניהול פרויקטים ופרמטרים חשבונאיים**.</span><span class="sxs-lookup"><span data-stu-id="acff9-115">In the navigation pane, go to **Modules > Project management and accounting > Setup > Project management and accounting parameters**.</span></span>
11. <span data-ttu-id="acff9-116">בחר בכרטיסיה **בין-חברתי**.</span><span class="sxs-lookup"><span data-stu-id="acff9-116">Select the **Intercompany** tab.</span></span>
12. <span data-ttu-id="acff9-117">הזז את המחוון אל **כן** כדי לאפשר תזמון משאבים בין חברתי וגליונות זמנים.</span><span class="sxs-lookup"><span data-stu-id="acff9-117">Move the slider to **Yes** to enable intercompany resource scheduling and timesheets.</span></span>
13. <span data-ttu-id="acff9-118">ברשימה, סמן את השורה שנבחרה.</span><span class="sxs-lookup"><span data-stu-id="acff9-118">In the list, mark the selected row.</span></span>
14. <span data-ttu-id="acff9-119">בחר **New**.</span><span class="sxs-lookup"><span data-stu-id="acff9-119">Select **New**.</span></span>
15. <span data-ttu-id="acff9-120">בשדה **ישות משפטית לווה**, הזן או בחר ערך.</span><span class="sxs-lookup"><span data-stu-id="acff9-120">In the **Borrowing legal entity** field, enter or select a value.</span></span>
16. <span data-ttu-id="acff9-121">סמן את תיבת הסימון **צבירת הכנסות**.</span><span class="sxs-lookup"><span data-stu-id="acff9-121">Select the **Accrue revenue** check box.</span></span>
17. <span data-ttu-id="acff9-122">בשדה **קטגוריית גליון זמנים בברירת מחדל**, הזן או בחר ערך.</span><span class="sxs-lookup"><span data-stu-id="acff9-122">In the **Default timesheet category** field, enter or select a value.</span></span>
18. <span data-ttu-id="acff9-123">בשדה **קטגוריית הוצאות בברירת מחדל**, הזן או בחר ערך.</span><span class="sxs-lookup"><span data-stu-id="acff9-123">In the **Default expense category** field, enter or select a value.</span></span>
19. <span data-ttu-id="acff9-124">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="acff9-124">Select **Save**.</span></span>
20. <span data-ttu-id="acff9-125">סגור את הדף.</span><span class="sxs-lookup"><span data-stu-id="acff9-125">Close the page.</span></span>
21. <span data-ttu-id="acff9-126">בחלונית הניווט, עבור אל **מודולים > ניהול פרוייקטים וחשבונאות > הגדרה > רישום > הגדרת רישום ספר ראשי**.</span><span class="sxs-lookup"><span data-stu-id="acff9-126">In the navigation pane, go to **Modules > Project management and accounting > Setup > Posting > Ledger posting setup**.</span></span>
22. <span data-ttu-id="acff9-127">בחר אפשרות בשדה **סוגי חשבון ספר ראשי**.</span><span class="sxs-lookup"><span data-stu-id="acff9-127">In the **Ledger account types** field, select an option.</span></span>
23. <span data-ttu-id="acff9-128">בחר **New**.</span><span class="sxs-lookup"><span data-stu-id="acff9-128">Select **New**.</span></span>
24. <span data-ttu-id="acff9-129">בשדה **תיק לקוח ראשי** של השורה החדשה, ציין את הערכים הרצויים.</span><span class="sxs-lookup"><span data-stu-id="acff9-129">In the **Main account** field of the new row, specify the desired values.</span></span>
25. <span data-ttu-id="acff9-130">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="acff9-130">Select **Save**.</span></span>
26. <span data-ttu-id="acff9-131">סגור את הדף.</span><span class="sxs-lookup"><span data-stu-id="acff9-131">Close the page.</span></span>
27. <span data-ttu-id="acff9-132">בחלונית הניווט, עבור אל **מודולים > ניהול פרוייקטים וחשבונאות > הגדרה > מחירים > מחיר העברה**.</span><span class="sxs-lookup"><span data-stu-id="acff9-132">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Transfer price**.</span></span>
28. <span data-ttu-id="acff9-133">בחר **New**.</span><span class="sxs-lookup"><span data-stu-id="acff9-133">Select **New**.</span></span>
29. <span data-ttu-id="acff9-134">בשדה **תאריך כניסה לתוקף**, הזן תאריך.</span><span class="sxs-lookup"><span data-stu-id="acff9-134">In the **Effective date** field, enter a date.</span></span>
30. <span data-ttu-id="acff9-135">בשדה **ישות משפטית לווה**, הזן או בחר ערך.</span><span class="sxs-lookup"><span data-stu-id="acff9-135">In the **Borrowing legal entity** field, enter or select a value.</span></span>
31. <span data-ttu-id="acff9-136">בחר אפשרות בשדה **מודל מחיר העברה**.</span><span class="sxs-lookup"><span data-stu-id="acff9-136">In the **Transfer price model** field, select an option.</span></span>
32. <span data-ttu-id="acff9-137">הזן מספר בשדה **תמחור**.</span><span class="sxs-lookup"><span data-stu-id="acff9-137">In the **Pricing** field, enter a number.</span></span>
33. <span data-ttu-id="acff9-138">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="acff9-138">Select **Save**.</span></span>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]