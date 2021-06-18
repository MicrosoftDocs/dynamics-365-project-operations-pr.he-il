---
title: יצירה והחלה של תנאי שמירת התשלום של ספק
description: נושא זה מספק מידע על אופן ההגדרה והתחזוקת תנאי השמירה של תשלומי ספק.
author: Yowelle
ms.date: 05/26/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 09bb30f55ee8e1f24634e9d8b7dea95bd3dbd24f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006328"
---
# <a name="create-and-apply-vendor-payment-retention-terms"></a><span data-ttu-id="3e059-103">יצירה והחלה של תנאי שמירת התשלום של ספק</span><span class="sxs-lookup"><span data-stu-id="3e059-103">Create and apply vendor payment retention terms</span></span>

[!include [banner](../includes/banner.md)] 

<span data-ttu-id="3e059-104">הגדרת תנאי שמירת תשלום ספק עבור פרויקט היא שימושית כאשר הארגון שלך רוצה לשמור חלק מהתשלומים ששולמו לספק.</span><span class="sxs-lookup"><span data-stu-id="3e059-104">Setting up vendor payment retention terms for a project is useful when your organization wants to retain part of the payments made to a vendor.</span></span> <span data-ttu-id="3e059-105">לדוגמה, כאשר ברצונך להחזיק בתשלום לספק עד שהמוצרים שנמסרו עונים על ציפיותיך.</span><span class="sxs-lookup"><span data-stu-id="3e059-105">For example, when you want to hold payment to a vendor until the products delivered meet your expectations.</span></span> <span data-ttu-id="3e059-106">ניתן לציין תנאים לשמירת תשלום הספק בעת משא ומתן על חוזה ספק.</span><span class="sxs-lookup"><span data-stu-id="3e059-106">Vendor payment retention terms can be specified when you negotiate a vendor contract.</span></span>

## <a name="create-vendor-payment-retention-terms"></a><span data-ttu-id="3e059-107">יצירה תנאים לשמירת תשלום ספק</span><span class="sxs-lookup"><span data-stu-id="3e059-107">Create vendor payment retention terms</span></span>

<span data-ttu-id="3e059-108">באפשרותך להזין את אחוז התשלום הספק לשמירה ואת אחוז הסכומים שנשמרו בעבר אשר יש לשחררם.</span><span class="sxs-lookup"><span data-stu-id="3e059-108">You can enter the percentage of vendor payment for retention and the percentage of the previously retained amounts to be released.</span></span> <span data-ttu-id="3e059-109">הסכומים נשמרים אוטומטית בחשבוניות הספק עד שהחוזה מגיע למצב ההשלמה שצוין.</span><span class="sxs-lookup"><span data-stu-id="3e059-109">Amounts are automatically retained on vendor invoices until the contract reaches the specified state of completion.</span></span> <span data-ttu-id="3e059-110">לאחר שתגדיר את תנאי השמירה, תוכל להחיל אותם על כל פרויקט עבור אותו ספק.</span><span class="sxs-lookup"><span data-stu-id="3e059-110">After you set up the retention terms, you can apply them to any project for that vendor.</span></span>

<span data-ttu-id="3e059-111">בצע את השלבים הבאים כדי להגדיר ולתחזק תנאי שמירה לתשלומי ספק.</span><span class="sxs-lookup"><span data-stu-id="3e059-111">Use the following steps to set up and maintain retention terms for vendor payments.</span></span> 

1. <span data-ttu-id="3e059-112">עבור אל **ניהול פרויקטים וחשבונאות** > **שמירה** > **תנאי שמירת תשלום ספק**.</span><span class="sxs-lookup"><span data-stu-id="3e059-112">Go to **Project management and accounting** > **Retention** > **Vendor payment retention terms**.</span></span>
2. <span data-ttu-id="3e059-113">בחר **חדש** כדי להוסיף תנאי שמירה חדש לספק.</span><span class="sxs-lookup"><span data-stu-id="3e059-113">Select **New** to add a new vendor retention term.</span></span> <span data-ttu-id="3e059-114">הערך **מזהה כלל** עבור התנאי החדש מוזן באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="3e059-114">The **Rule ID** value for the new term is automatically entered.</span></span> 
3. <span data-ttu-id="3e059-115">הזן תיאור קצר בשדה **תיאור**, וב-FastTab **תנאים** בחר **הוסף שורה** כדי להזין ערכים עבור הדברים הבאים:</span><span class="sxs-lookup"><span data-stu-id="3e059-115">Enter a brief description in the **Description** field, and on the **Terms** FastTab, select **Add line** to enter term values for the following:</span></span>

   - <span data-ttu-id="3e059-116">**אחוז היחידות שנמסרו**: הזן אחוז השלמה לתנאי.</span><span class="sxs-lookup"><span data-stu-id="3e059-116">**Percentage of units delivered**: Enter a percentage of completion for the term.</span></span> <span data-ttu-id="3e059-117">הסכומים נשמרים אוטומטית בחשבוניות הספק עד ששלת השלמת הפרויקט שווה לאחוז שצוין.</span><span class="sxs-lookup"><span data-stu-id="3e059-117">Amounts are automatically retained on vendor invoices until the project stage of completion is equal to the specified percentage.</span></span> <span data-ttu-id="3e059-118">לדוגמה, אם תזין 50.00, הסכומים נשמרים עד להשלמה של 50 אחוז מהפרויקט.</span><span class="sxs-lookup"><span data-stu-id="3e059-118">For example, if you enter 50.00, amounts are retained until the project is 50 percent completed.</span></span>
   - <span data-ttu-id="3e059-119">**אחוז לשמירה**: הזן האחוז מסכום חשבונית הספק שיש לשמור.</span><span class="sxs-lookup"><span data-stu-id="3e059-119">**Percentage to retain**: Enter a percentage of the vendor invoice amount to be retained.</span></span> <span data-ttu-id="3e059-120">לדוגמה, אם אתה מזין 10.00, אז 10 אחוז מהסכום בחשבונית ספק יישמר עד שהפרויקט יגיע לאחוז ההשלמה כפי שנקבע בשדה **אחוז היחידות שנמסרו**.</span><span class="sxs-lookup"><span data-stu-id="3e059-120">For example, if you enter 10.00, then 10 percent of the amount on a vendor invoice is retained until the project reaches the percentage of completion as set in the **Percentage of units delivered field**.</span></span>
   - <span data-ttu-id="3e059-121">**אחוז לשחרור**: בחר **הוסף שורה** כדי להזין אחוז מכל סכום שנשמר בעבר לשחרור עבור רמת השלמת הפרויקט שנבחרה.</span><span class="sxs-lookup"><span data-stu-id="3e059-121">**Percentage to release**: Select **Add line** to enter a percentage of any previously retained amounts to be released for the selected level of project completion.</span></span>

> [!NOTE]
> <span data-ttu-id="3e059-122">אם יש לך יותר מאבן דרך אחת עבור רמות שונות של השלמת פרויקט, הזן שורה נפרדת לתנאי שמירה לספק עבור כל כלל שמירה.</span><span class="sxs-lookup"><span data-stu-id="3e059-122">If you have more than one milestone for different levels of project completion, enter a separate vendor retention term line for each retention rule.</span></span> <span data-ttu-id="3e059-123">כל שורה יכולה לציין אחוז שמירה שונה ואחוז שחרור שונה עבור כל רמת השלמה מיועדת של השלמת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="3e059-123">Each line can specify a different retention percentage and a different release percentage for each designated level of project completion.</span></span>

<span data-ttu-id="3e059-124">לאחר הגדרת תנאי השמירה עבור ספק, ניתן להחיל את התנאים על פרויקט.</span><span class="sxs-lookup"><span data-stu-id="3e059-124">After you create vendor retention terms for a vendor, you can apply the terms to a project.</span></span>

## <a name="apply-vendor-retention-terms-to-a-project"></a><span data-ttu-id="3e059-125">החלת תנאי שמירה של ספק על פרויקט</span><span class="sxs-lookup"><span data-stu-id="3e059-125">Apply vendor retention terms to a project</span></span>

1. <span data-ttu-id="3e059-126">עבור אל **ניהול פרויקטים וחשבונאות** > **פרויקטים** > **כל הפרויקטים** ופתח פרויקט מדף רשימת הפרויקטים.</span><span class="sxs-lookup"><span data-stu-id="3e059-126">Go to **Project management and accounting** > **Projects** > **All projects** and open a project from the project list page.</span></span>
2. <span data-ttu-id="3e059-127">ב- FastTab **הסכמי ספק**, בחר באפשרות **הוסף שורה**.</span><span class="sxs-lookup"><span data-stu-id="3e059-127">On the **Vendor agreements** FastTab, select **Add line**.</span></span>
3. <span data-ttu-id="3e059-128">ב **‏‫בשדה קוד תיק לקוח‬**, בחר אחת מהאפשרויות הבאות:</span><span class="sxs-lookup"><span data-stu-id="3e059-128">In the **Account code field**, select one of the following options:</span></span> 

   - <span data-ttu-id="3e059-129">**טבלה**: תנאי שמירה של ספק חלים על ספק יחיד.</span><span class="sxs-lookup"><span data-stu-id="3e059-129">**Table**: The vendor retention terms apply to a single vendor.</span></span>
   - <span data-ttu-id="3e059-130">**קבוצה**: תנאי השמירת של ספק חלים על כל הספקים בקבוצת ספקים.</span><span class="sxs-lookup"><span data-stu-id="3e059-130">**Group**: The vendor retention terms apply to all vendors in a vendor group.</span></span>
   - <span data-ttu-id="3e059-131">**כולם**: תנאי שמירה של ספק חלים על ספק כל הספקים.</span><span class="sxs-lookup"><span data-stu-id="3e059-131">**All**: The vendor retention terms apply to all vendors.</span></span>

4. <span data-ttu-id="3e059-132">ב **שדה ספק / קבוצת ספקים** בחר בספק או בקבוצת הספקים שעליהם חלים תנאי השמירה של הספק.</span><span class="sxs-lookup"><span data-stu-id="3e059-132">In the **Vendor/Vendor group field**, select the vendor or vendor group to which the vendor retention terms apply.</span></span> <span data-ttu-id="3e059-133">אם בחרת **כולם** בשלב הקודם, שדה זה אינו זמין.</span><span class="sxs-lookup"><span data-stu-id="3e059-133">If you selected **All** in the previous step, this field is unavailable.</span></span>
5. <span data-ttu-id="3e059-134">בשדה **תנאי שמירה של ספק** בחר את תנאי השמירה שיצרת בהליך הקודם.</span><span class="sxs-lookup"><span data-stu-id="3e059-134">In the **Vendor retention terms** field, select the retention terms that you created in the previous procedure.</span></span>
6. <span data-ttu-id="3e059-135">אם בפרויקט מוגדרים תנאי תשלום גב-אל-גב (PWP) עבור הספק, הזן את אחוז הסף עבור הפרויקט בשדה **אחוז הסף של גב-אל-גב**.</span><span class="sxs-lookup"><span data-stu-id="3e059-135">If the project also has pay-when-paid (PWP) terms set up for the vendor, enter the threshold percentage for the project in the **PWP threshold percentage** field.</span></span>

<span data-ttu-id="3e059-136">תנאי השמירת של הספק מוצגים גם בהזמנות רכש שאתה יוצר עבור הספק.</span><span class="sxs-lookup"><span data-stu-id="3e059-136">The vendor retention terms are also displayed on purchase orders that you create for the vendor.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]