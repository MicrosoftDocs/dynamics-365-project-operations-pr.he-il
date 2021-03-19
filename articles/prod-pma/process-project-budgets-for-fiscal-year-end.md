---
title: העברת תקציבי פרויקט בסוף שנת כספים
description: מאמר זה מספק מידע על אופן העברת סכומי התקציב שנותרו לשנים הבאות ויצירת פרטים בפנקס התקציבים.
author: Yowelle
manager: AnnBe
ms.date: 03/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
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
ms.openlocfilehash: 1f601be072e84fc04246cd55a260c8004f6fb3e5
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289730"
---
# <a name="transfer-project-budgets-at-fiscal-year-end"></a><span data-ttu-id="039e3-103">העברת תקציבי פרויקט בסוף שנת כספים</span><span class="sxs-lookup"><span data-stu-id="039e3-103">Transfer project budgets at fiscal year end</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="039e3-104">כשעובדים על פרויקט רב-שנתי, ייתכן שיישאר תקציב בסוף שנת הכספים.</span><span class="sxs-lookup"><span data-stu-id="039e3-104">When working on a multi-year project, you might have remaining budget at the end of the fiscal year.</span></span> <span data-ttu-id="039e3-105">באפשרותך להעביר את סכומי התקציב הנותרים לשנה עתידית וליצור פרטים בפנקס התקציבים עבור הסכומים בספר החשבונות הראשי המשויך.</span><span class="sxs-lookup"><span data-stu-id="039e3-105">You can transfer the remaining budget amounts to a future year, and create budget register details for the amounts in the associated general ledger accounts.</span></span> <span data-ttu-id="039e3-106">לפני שתעביר את הסכומים הנותרים, בדוק ונתח את סכומי התקציב הנותרים.</span><span class="sxs-lookup"><span data-stu-id="039e3-106">Before you carry forward the remaining amounts, review and analyze the remaining budget amounts.</span></span>

## <a name="review-and-analyze-remaining-budget-amounts"></a><span data-ttu-id="039e3-107">בדיקה וניתוח של סכומי התקציב הנותרים</span><span class="sxs-lookup"><span data-stu-id="039e3-107">Review and analyze remaining budget amounts</span></span>

<span data-ttu-id="039e3-108">בצע את השלבים הבאים כדי לבדוק את סכומי התקציב בסוף השנה עבור הפרויקטים, אך בלי להעביר את הסכומים.</span><span class="sxs-lookup"><span data-stu-id="039e3-108">Complete the following steps to review the year-end budget amounts for projects, but not carry the amounts forward.</span></span>

1. <span data-ttu-id="039e3-109">עבור אל **ניהול פרויקטים וחשבונאות** > **תקופתי** > **תקציבים** > **העבר תקציבים**.</span><span class="sxs-lookup"><span data-stu-id="039e3-109">Go to **Project management and accounting** > **Periodic** > **Budgets** > **Carry forward budgets**.</span></span> 
2. <span data-ttu-id="039e3-110">בדף **תהליך העברת תקציב של פרויקט**, בכרטיסיה **אפשרויות סוף שנה**, ודא שהאפשרות **העבר סכומי תקציב נותרים של פרויקט** אינה זמינה.</span><span class="sxs-lookup"><span data-stu-id="039e3-110">On the **Project budget carry-forward process** page, on the **Year-end options** tab, verify that **Carry forward remaining project budget amounts** is not enabled.</span></span>
3. <span data-ttu-id="039e3-111">בכרטיסיה **פרמטרים**, בשדה **שנת תקציב פרויקט**, בחר את שנת הכספים עבורה אתה רוצה לראות את סכום התקציב הנותר.</span><span class="sxs-lookup"><span data-stu-id="039e3-111">On the **Parameters** tab, in the **Project budget year** field, select the fiscal year for which you want to view the remaining budget amount.</span></span> 
4. <span data-ttu-id="039e3-112">בשדה **שנת כספים פותחת**, בחר את שנת הכספים עבורה אתה רוצה לראות את סכום התקציב הנותר.</span><span class="sxs-lookup"><span data-stu-id="039e3-112">In the **Opening fiscal year** field, select the fiscal year for which you want to view the remaining budget amount.</span></span> 
5. <span data-ttu-id="039e3-113">בשדה **ממודל תחזית**, בחר באפשרות **תקציב שנותר**.</span><span class="sxs-lookup"><span data-stu-id="039e3-113">In the **From forecast model** field, select **Remaining budget**.</span></span> 
6. <span data-ttu-id="039e3-114">כדי לכלול פרויקטים העומדים בקריטריונים שבחרת ושלא נותר בהם תקציב, בחר באפשרות **הצג 'נותר אפס'**.</span><span class="sxs-lookup"><span data-stu-id="039e3-114">To include projects that meet your selected criteria and have no remaining budget, select **Show zero remaining**.</span></span>  
7. <span data-ttu-id="039e3-115">בכרטיסיה **בחר תקציבים**, בחר באפשרות **אחזר את כל התקציבים** כדי לטעון את כל התקציבים שתואמים לקריטריונים שבחרת ולאחר מכן בחר **עבד**.</span><span class="sxs-lookup"><span data-stu-id="039e3-115">On the **Select Budgets** tab, select **Retrieve all budgets** to load all budgets that match your selected criteria, and then select **Process**.</span></span> 
8. <span data-ttu-id="039e3-116">כדי לעצב שאילתת מסד נתונים הטוענת קבוצה ספציפית של תקציבים בחלונית, בחר באפשרות **אחזר את התקציבים שנבחרו**.</span><span class="sxs-lookup"><span data-stu-id="039e3-116">To design a database query that loads a specific set of budgets into the pane, select **Retrieve selected budgets**.</span></span>

<span data-ttu-id="039e3-117">לקבלת מידע נוסף אודות שורה ספציפית בחלונית, בחר את השורה ולאחר מכן בחר באפשרות **הצג פרטי תקציב** או **הצג חשבונות**.</span><span class="sxs-lookup"><span data-stu-id="039e3-117">For more information about a specific line in the pane, select the line, and then select **View budget details** or **View accounts**.</span></span>

## <a name="carry-forward-remaining-budget-amounts"></a><span data-ttu-id="039e3-118">העברת סכומי תקציב שנותרו</span><span class="sxs-lookup"><span data-stu-id="039e3-118">Carry forward remaining budget amounts</span></span> 

<span data-ttu-id="039e3-119">כאשר אתה מעבד את סכומי התקציב שנותרו, תוכל ליצור טרנזקציות בספר החשבונות הראשי עבור הסכומים שאתה מעביר.</span><span class="sxs-lookup"><span data-stu-id="039e3-119">When you process remaining budget amounts, you can create transactions in the general ledger for the amounts that you are carrying forward.</span></span> <span data-ttu-id="039e3-120">כדי ליצור טרנזקציות של ספר חשבונות ראשי, השלם את השלבים בסעיף [העברת סכומי תקציב ויצירת טרנזקציות בספר החשבונות הראשי](#carry-forward).</span><span class="sxs-lookup"><span data-stu-id="039e3-120">To create general ledger transactions, complete the steps in the section, [Carry forward budget amounts and create general ledger transactions](#carry-forward).</span></span> 

> [!NOTE]
> <span data-ttu-id="039e3-121">סכומי התקציב המועברים מועברים למודל התחזית שנבחר בדף **מודלי תחזית** בתור מודל התחזית להעברה.</span><span class="sxs-lookup"><span data-stu-id="039e3-121">Budget amounts that are carried forward are transferred to the forecast model that is selected in the **Forecast models** page as the carry-forward forecast model.</span></span>  

## <a name="carry-forward-budget-amounts-and-create-general-ledger-transactions"></a><a name="carry-forward"></a><span data-ttu-id="039e3-122">העברת סכומי תקציב ויצירת טרנזקציות בספר החשבונות הראשי</span><span class="sxs-lookup"><span data-stu-id="039e3-122">Carry forward budget amounts and create general ledger transactions</span></span>

1.  <span data-ttu-id="039e3-123">בחר **ניהול פרויקטים וחשבונאות** > **תקופתי** > **תקציבים** > **העבר תקציבים**.</span><span class="sxs-lookup"><span data-stu-id="039e3-123">Select **Project management and accounting** > **Periodic** > **Budgets** > **Carry forward budgets**.</span></span> 
2. <span data-ttu-id="039e3-124">בדף **תהליך העברת תקציב של פרויקט‬‏‫**, בחר באפשרות **סוף שנה** ואז הפוך את **העבר סכומי תקציב נותרים של פרויקט** ואת **צור הזנות של פנקס תקציבים בספר החשבונת הראשי** לזמינים.</span><span class="sxs-lookup"><span data-stu-id="039e3-124">On the **Project budget carry-forward process** page, select **Year-end**, and then enable **Carry forward remaining project budget amounts** and **Create budget register entries in general ledger**.</span></span> 
3. <span data-ttu-id="039e3-125">בכרטיסיה **פרמטרים**, בקבוצת השדות **פרמטרי פרויקט**, בחר את האפשרויות הבאות:</span><span class="sxs-lookup"><span data-stu-id="039e3-125">On the **Parameters** tab, in the **Project parameters** field group, select the following:</span></span>

   - <span data-ttu-id="039e3-126">**שנת תקציב פרויקט**: בחר את תחילת שנת הכספים עבורה אתה רוצה לראות את סכומי התקציב הנותרים.</span><span class="sxs-lookup"><span data-stu-id="039e3-126">**Project budget year**: Select the beginning of the fiscal year for which you want to view the remaining budget amounts.</span></span> 
   - <span data-ttu-id="039e3-127">**רווח והפסד**: צור טרנזקציות רווח והפסד בספר החשבונות הראשי.</span><span class="sxs-lookup"><span data-stu-id="039e3-127">**Profit and loss**: Create profit and loss transactions in the general ledger.</span></span> 
   -  <span data-ttu-id="039e3-128">**WIP**: צור טרנזקציות Work in Progress ‏(WIP) בספר החשבונות הראשי.</span><span class="sxs-lookup"><span data-stu-id="039e3-128">**WIP**: Create Work in Progress (WIP) transactions in the general ledger.</span></span>
   -  <span data-ttu-id="039e3-129">**שכר**: צור טרנזקציות להקצאת שכר בספר החשבונות הראשי.</span><span class="sxs-lookup"><span data-stu-id="039e3-129">**Payroll**: Create payroll allocation transactions in the general ledger.</span></span> 

5. <span data-ttu-id="039e3-130">בקבוצת השדות **ספר חשבונות ראשי**, ספק את הפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="039e3-130">In the **General ledger** field group, provide the following information:</span></span> 

   - <span data-ttu-id="039e3-131">בשדה **שנת כספים פותחת**, בחר את שנת הכספים אליה אתה רוצה להעביר את סכומי התקציב הנותרים עבור הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="039e3-131">In the **Opening fiscal year** field, select the fiscal year that you want to transfer remaining budget amounts to for the projects.</span></span> <span data-ttu-id="039e3-132">ערך ברירת המחדל הוא שנה לאחר הערך בשדה **שנת תקציב הפרויקט**.</span><span class="sxs-lookup"><span data-stu-id="039e3-132">The default value is one year after the value in the **Project budget year** field.</span></span>
   -  <span data-ttu-id="039e3-133">בשדה **תקופת העברה**, בחר את התקופה שעבורה אתה רוצה ליצור את פרטי פנקס התקציבים בספר החשבונות הראשי.</span><span class="sxs-lookup"><span data-stu-id="039e3-133">In the **Carry-forward period** field, select the period that you want to create the budget register details for in the general ledger.</span></span> <span data-ttu-id="039e3-134">זו בדרך כלל התקופה הראשונה בשנת הכספים הפותחת.</span><span class="sxs-lookup"><span data-stu-id="039e3-134">This is typically the first period in the opening fiscal year.</span></span>

6. <span data-ttu-id="039e3-135">בקבוצת השדות **העתק מ/אל**, ספק את הפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="039e3-135">In the **Copy from/to** field group, provide the following information:</span></span>

   - <span data-ttu-id="039e3-136">בשדה **ממודל התחזית**, בחר את מודל התחזית של תקציב הפרויקט המשויך לסכומי התקציב הנותרים שברצונך להעביר עבור הפרויקטים.</span><span class="sxs-lookup"><span data-stu-id="039e3-136">In the **From forecast model** field, select the project budget forecast model associated with the remaining budget amounts you want to transfer for the projects.</span></span> 
   - <span data-ttu-id="039e3-137">בשדה **אל מודל של תקציב ספר ראשי**, בחר את המודל של תקציב הספר הראשי המשויך לסכומי התקציב שברצונך להעביר אל ספר החשבונות הראשי.</span><span class="sxs-lookup"><span data-stu-id="039e3-137">In the **To ledger budget model** field, select the ledger budget model associated with the budget amounts you want to transfer to the general ledger.</span></span> 
   -  <span data-ttu-id="039e3-138">בחר באפשרות **העבר מטבע מכירות** כדי להשתמש במטבע המכירות של הפרויקט עבור הטרנזקציות בספר החשבונות הראשי שנוצרות בעת העברת סכומי התקציב לפרויקטים.</span><span class="sxs-lookup"><span data-stu-id="039e3-138">Select **Transfer sales currency** to use the project's sales currency for the general ledger transactions that are created when you transfer the budget amounts for the projects.</span></span> <span data-ttu-id="039e3-139">אם אפשרות זו לא נבחרת, הטרנזקציות משתמשות במטבע החשבונאות.</span><span class="sxs-lookup"><span data-stu-id="039e3-139">When the option is not selected, the transactions use the accounting currency.</span></span> 
   -  <span data-ttu-id="039e3-140">בחר באפשרות **הצג 'נותר אפס'** כדי לכלול פרויקטים שלא נותרו בהם סכומי תקציב אבל הם עומדים בקריטריונים האחרים שתבחר בפרויקטים המוצגים בחלונית התחתונה.</span><span class="sxs-lookup"><span data-stu-id="039e3-140">Select **Show zero remaining** to include projects that have no remaining budget amounts, but meet the other criteria that you select in the projects displayed in the bottom pane.</span></span>

7. <span data-ttu-id="039e3-141">בכרטיסיה **בחר תקציבים**, בחר באפשרות **אחזר את כל התקציבים** כדי לטעון את כל התקציבים שתואמים לקריטריונים שבחרת.</span><span class="sxs-lookup"><span data-stu-id="039e3-141">On the **Select Budgets** tab, select **Retrieve all budgets** to load all budgets that match the criteria you selected.</span></span> <span data-ttu-id="039e3-142">אם אתה מעדיף לעצב שאילתת מסד נתונים הטוענת קבוצה ספציפית של תקציבי פרויקט בחלונית, בחר באפשרות **אחזר את התקציבים שנבחרו**.</span><span class="sxs-lookup"><span data-stu-id="039e3-142">If you prefer to design a database query that loads a specific set of project budgets into the pane, select **Retrieve selected budgets**.</span></span>
8. <span data-ttu-id="039e3-143">עבור כל פרויקט שאתה רוצה לעבד, בחר באפשרות בתחילת השורה עבור הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="039e3-143">For each project that you want to process, select the option at the beginning of the line for the project.</span></span>

    > [!TIP]
    > <span data-ttu-id="039e3-144">כדי לבחור את כל הפרויקטים או את רובם, בחר את סימן הביקורת בפינה השמאלית העליונה.</span><span class="sxs-lookup"><span data-stu-id="039e3-144">To select all or most of the projects, select the check mark in the top upper-left corner.</span></span> <span data-ttu-id="039e3-145">כדי לא לעבד אף פרויקט, נקה את סימן הביקורת עבור אותו פרויקט.</span><span class="sxs-lookup"><span data-stu-id="039e3-145">To exclude processing any project, clear the check mark for that project.</span></span>

9. <span data-ttu-id="039e3-146">להעברת סכומי התקציב הנותרים עבור הפרויקטים שנבחרו אל שנת הכספים שנבחרה וליצירת פרטים של פנקס תקציבים בספר החשבונות הראשי, בחר באפשרות **עבד**.</span><span class="sxs-lookup"><span data-stu-id="039e3-146">To transfer the remaining budget amounts for the selected projects to the selected fiscal year and create budget register details in the general ledger, select **Process**.</span></span>

## <a name="carry-forward-budget-amounts-without-creating-general-ledger-transactions"></a><span data-ttu-id="039e3-147">העברת סכומי תקציב ללא יצירת טרנזקציות בספר החשבונות הראשי</span><span class="sxs-lookup"><span data-stu-id="039e3-147">Carry forward budget amounts without creating general ledger transactions</span></span>

1. <span data-ttu-id="039e3-148">עבור אל **ניהול פרויקטים וחשבונאות** > **תקופתי** > **תקציבים** > **העבר תקציבים**.</span><span class="sxs-lookup"><span data-stu-id="039e3-148">Go to **Project management and accounting** > **Periodic** > **Budgets** > **Carry forward budgets**.</span></span>
2. <span data-ttu-id="039e3-149">בדף **תהליך העברת תקציב של פרויקט**, בשדה **אפשרויות סוף שנה**, בחר באפשרות **העבר סכומי תקציב נותרים של פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="039e3-149">On the **Project budget carry-forward process** page, in the **Year-end options** field, select **Carry forward remaining project budget amounts**.</span></span>
3. <span data-ttu-id="039e3-150">בקבוצה **פרמטרים**, בשדה **שנת תקציב פרויקט**, בחר את שנת הכספים עבורה אתה רוצה לראות את סכומי התקציב הנותרים.</span><span class="sxs-lookup"><span data-stu-id="039e3-150">In the **Parameters** group, in the **Project budget year** field, select the fiscal year for which you want to view the remaining budget amounts.</span></span>
4. <span data-ttu-id="039e3-151">בקבוצה **העתק מ/אל**, ספק את הפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="039e3-151">In the **Copy from/to** group, provide the following information:</span></span>

   - <span data-ttu-id="039e3-152">בשדה **ממודל התחזית**, בחר את מודל התחזית של תקציב הפרויקט המשויך לסכומי התקציב הנותרים שברצונך להעביר עבור הפרויקטים.</span><span class="sxs-lookup"><span data-stu-id="039e3-152">In the **From forecast model** field, select the project budget forecast model that is associated with the remaining budget amounts that you want to transfer for the projects.</span></span> 
   - <span data-ttu-id="039e3-153">בחר באפשרות **הצג 'נותר אפס'** כדי לכלול פרויקטים העומדים בשאר הקריטריונים שבחרת ושלא נותרו בהם סכומי תקציב.</span><span class="sxs-lookup"><span data-stu-id="039e3-153">Select **Show zero remaining** to include projects that have no remaining budget amounts, but that meet the other criteria you selected.</span></span>
   - <span data-ttu-id="039e3-154">בקבוצה **בחר תקציבים**, בחר באפשרות **אחזר את כל התקציבים** כדי לטעון את כל התקציבים שתואמים לקריטריונים שבחרת.</span><span class="sxs-lookup"><span data-stu-id="039e3-154">In the **Select Budgets** group, select **Retrieve all budgets** to load all budgets that match the criteria that you selected.</span></span> <span data-ttu-id="039e3-155">כדי לעצב שאילתת מסד נתונים הטוענת קבוצה ספציפית של תקציבי פרויקט בחלונית, בחר באפשרות **אחזר את התקציבים שנבחרו**.</span><span class="sxs-lookup"><span data-stu-id="039e3-155">To design a database query that loads a specific set of project budgets into the pane, select **Retrieve selected budgets**.</span></span>

5. <span data-ttu-id="039e3-156">עבור כל פרויקט שאתה רוצה לעבד, בחר באפשרות בתחילת השורה עבור הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="039e3-156">For each project that you want to process, select the option at the beginning of the line for the project.</span></span> 
6. <span data-ttu-id="039e3-157">בחר באפשרות **עבד** כדי להעביר את סכומי התקציב הנותרים של הפרויקטים שנבחרו אל שנת הכספים שנבחרה.</span><span class="sxs-lookup"><span data-stu-id="039e3-157">Select **Process** to transfer the remaining budget amounts for the selected projects to the selected fiscal year.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]