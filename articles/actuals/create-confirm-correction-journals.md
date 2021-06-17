---
title: יצירה ואישור של יומני תיקון
description: נושא זה מספק מידע לגבי האופן שבו יוצרים ומאשרים יומני תיקון.
author: rumant
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 9d242741b2070f086bf8d3f1d40a5380c2a0f518
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996657"
---
# <a name="create-and-confirm-correction-journals"></a><span data-ttu-id="b6cbd-103">יצירה ואישור של יומני תיקון</span><span class="sxs-lookup"><span data-stu-id="b6cbd-103">Create and confirm Correction journals</span></span>

<span data-ttu-id="b6cbd-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="b6cbd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b6cbd-105">לעיתים, רשומת זמן או הוצאה יוזנו בצורה שגויה.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-105">Occasionally a time or expense entry may be entered incorrectly.</span></span> <span data-ttu-id="b6cbd-106">לדוגמה, יועץ עשוי לבחור בתאריך הלא נכון בעת יצירת ערך זמן או שהוא עשוי להחליף בין המספרים בעת הזנת הוצאה.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-106">For example, a consultant might select the wrong date when creating a time entry or they might transpose the numbers when entering an expense.</span></span> <span data-ttu-id="b6cbd-107">אם יועץ לא יכול לבצע את העדכונים בערכים שהוגשו, מנהל מערכת יכול לתקן את הרשומה בפרויקט ישירות.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-107">If a consultant can’t make the updates to the submitted entries, an administrator can directly correct the entry for a project.</span></span>

<span data-ttu-id="b6cbd-108">כדי להשלים את הנוהל בנושא זה, תצטרך הרשאות מנהל מערכת.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-108">To complete the procedures in this topic, you will need Administrator permissions.</span></span>

## <a name="correct-approved-time-entries"></a><span data-ttu-id="b6cbd-109">תיקון רשומות זמן מאושרות</span><span class="sxs-lookup"><span data-stu-id="b6cbd-109">Correct approved time entries</span></span>     

<span data-ttu-id="b6cbd-110">בצע את הצעדים הבאים כדי לתקן ערכי זמן בודדים או מרובים בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-110">Complete the following steps to correct single or multiple time entries for a project.</span></span>

1. <span data-ttu-id="b6cbd-111">באזור **מכירות**, בחר **"עסקאות** ואז בחר **זמן מאושר**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-111">In the **Sales** area, select **Transactions**, and then select **Approved Time**.</span></span> 

2. <span data-ttu-id="b6cbd-112">ברשימת **זמן מאושר**, אתר ובחר רשומת זמן מאושרת אחת או יותר לתיקון.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-112">In the **Approved Time** list, locate and select one or more approved time entries to correct.</span></span> <span data-ttu-id="b6cbd-113">אתה יכול להשתמש בפילטר כדי לאתר ערכים קשורים.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-113">You can use the filter to locate related entries.</span></span> <span data-ttu-id="b6cbd-114">לדוגמה, אתה יכול לסנן לפי מזהה הפרויקט ולבחור את כל רשומות הזמן המאושרות של מזהה הפרויקט הזה.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-114">For example, you might filter on a Project ID, and select all approved time entries with that Project ID.</span></span>

3. <span data-ttu-id="b6cbd-115">בחר **‏‎תקן רשומות**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-115">Select **Correct entries**.</span></span> <span data-ttu-id="b6cbd-116">יומן תיקון חדש ייווצר אוטומטית, עם **תיקון זמן** מהסוג שהוקצה.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-116">A new correction journal is automatically created, with the assigned type **Time correction**.</span></span> <span data-ttu-id="b6cbd-117">הערכים שבחרת יתווספו ליומן.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-117">The entries you selected are added to the journal.</span></span> 

4. <span data-ttu-id="b6cbd-118">בדף **יומן חדש**, הזן **תיאור** ליומן התיקונים שלך, ואז בחר את כרטיסיית **תיקוני ערכי זמן**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-118">On the **New Journal** page, enter a **Description** for your correction journal, and then select the **Time Entry Corrections** tab.</span></span>  

5. <span data-ttu-id="b6cbd-119">בתוך המקטע **ערכים חדשים לערכי זמן**, עדכן את השדות עם המידע הנכון בהתאם לצורך.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-119">In the **New Values for Time Entries** section, update the fields with the correct information as necessary.</span></span> <span data-ttu-id="b6cbd-120">לדוגמה, באפשרותך לשנות את הפרויקט שהוקצה או את המשאב הניתן להזמנה.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-120">For example, you can change the assigned project or the bookable resource.</span></span>

6. <span data-ttu-id="b6cbd-121">בחר **תצוגה מקדימה**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-121">Select **Preview**.</span></span> <span data-ttu-id="b6cbd-122">בתיבת הדו-שיח, בחר באפשרות **OK**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-122">In the dialog box, select **OK**.</span></span> <span data-ttu-id="b6cbd-123">בכרטיסייה **שורות יומן** תוכל להציג רשימה של הפעולות המקוריות הקשורות לערכי הזמן שנבחרו ושונו ולשורות התואמות שנוצרו ותוקנו.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-123">On the **Journal lines** tab, you can view a list of the original actuals that are related to the selected time entries that have been reversed and the corrected corresponding lines that have been created.</span></span> <span data-ttu-id="b6cbd-124">אם יש צורך לבצע תיקונים נוספים, חזור על שלבים 5 ו -6.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-124">If additional corrections need to be made, repeat steps 5 and 6.</span></span> 

> [!NOTE]
> <span data-ttu-id="b6cbd-125">לכל הפעולות המתוקנות יהיו אותם ערכים שבחרת **ערכים חדשים לערכי זמן**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-125">All the corrected actuals will have the same values that you selected in the **New values for Time Entries** section.</span></span>

7. <span data-ttu-id="b6cbd-126">אם התיקונים מופיעים כצפוי, בחר **אשר**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-126">If the corrections appear as expected, select **Confirm**.</span></span> <span data-ttu-id="b6cbd-127">בתיבת הדו-שיח, בחר באפשרות **OK**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-127">In the dialog box, select **OK**.</span></span>

8. <span data-ttu-id="b6cbd-128">חזור לאזור **מכירות**, בחר **פרויקטים** ואז פתח את הפרויקט שעבורו עדכנת את רשומות הזמן זה עתה.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-128">Return to the **Sales** area, select **Projects**, and then open the project for which you just updated the time entries.</span></span> 

9. <span data-ttu-id="b6cbd-129">בדף **פרויקטים**, בכרטיסייה **פעולות**, צפה בשינויים שביצעת.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-129">On the **Projects** page, on the **Actuals** tab, view the changes that you made.</span></span> 

> [!NOTE]
> <span data-ttu-id="b6cbd-130">אם הכרטיסייה **פעולות** אינה גלויה, בחר **קשורים** > **פעולות**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-130">If the **Actuals** tab is not visible, select **Related** > **Actuals**.</span></span>  

10. <span data-ttu-id="b6cbd-131">ברשימה **תצוגת פעולות משויכות**, אתה יכול לראות שרשומות הזמן המקוריות ששונו עדיין מופיעות ברשימה, וכך גם ערכי הזמן המתוקנים התואמים.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-131">In the **Actual Associated View** list, you can see that the original time entries that have been reversed are still listed, as are the corresponding corrected time entries.</span></span> 

<span data-ttu-id="b6cbd-132">לדוגמה, באיור הבא ישנן שתי שורות פריטים בכמות של 8.00 אשר להם חיובים הרשומים בעמודה "סכום".</span><span class="sxs-lookup"><span data-stu-id="b6cbd-132">For example, in the following graphic, there are two line items with a quantity of 8.00 that have debits listed in the Amount column.</span></span> <span data-ttu-id="b6cbd-133">בנוסף, ישנן שתי שורות פריטים בכמות של 8.00- המציגים סכומי זיכוי בעמודה "סכום".</span><span class="sxs-lookup"><span data-stu-id="b6cbd-133">Additionally, there are two line items with a quantity of -8.00 that show credited amounts in the Amount column.</span></span> <span data-ttu-id="b6cbd-134">תיקונים אלו מביאים את הכמות לאפס.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-134">These corrections bring the quantity to zero.</span></span>

 
## <a name="correct-approved-expense-entries"></a><span data-ttu-id="b6cbd-135">תיקון רשומות זמן מאושרות</span><span class="sxs-lookup"><span data-stu-id="b6cbd-135">Correct approved expense entries</span></span>

<span data-ttu-id="b6cbd-136">בצע את הצעדים הבאים לתיקון רשומת הוצאה אחת או יותר.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-136">Complete the following steps to correct one or more expense entries.</span></span> 

1. <span data-ttu-id="b6cbd-137">באזור **מכירות**, בחלונית הניווט השמאלית, מתחת **עסקאות**, בחר **הוצאות מאושרות**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-137">In the **Sales** area, in the left navigation pane, under **Transactions**, select **Approved Expenses**.</span></span>

2. <span data-ttu-id="b6cbd-138">ברשימה **הוצאות מאושרות**, בחר את הפרויקט שברצונך לתקן ואז בחר **תיקון רשומות**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-138">In the **Approved Expenses** list, select the project that you want to correct, and then select **Correct entries**.</span></span> <span data-ttu-id="b6cbd-139">יומן תיקון חדש ייווצר אוטומטית, עם **תיקון הוצאה** מהסוג שהוקצה.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-139">A new correction journal will be created automatically with the assigned type of **Expense correction**.</span></span> 

3. <span data-ttu-id="b6cbd-140">בדף **יומן חדש**, הזן **תיאור** לתיקון, ובכרטיסייה **תיקון הוצאות**, במקטע **ערכים חדשים להוצאות**, בחר בשדות הנתונים שברצונך לתקן עבור שורות ההוצאות שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-140">On the **New Journal** page, enter a **Description** for the correction, and on the **Expense Correction** tab, in the **New Values for Expenses** section, select the data fields that you want to correct for the selected expense lines.</span></span> <span data-ttu-id="b6cbd-141">לדוגמה, אתה יכול להקצות את ההוצאה **פרויקט** אחר, או לתקן את **קטגוריית הוצאות**, **תאריך ההוצאה**, או **משאב הניתן להזמנה**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-141">For example, you can assign the expense to another **Project**, or correct the **Expense Category**, **Expense Date**, or **Bookable Resource**.</span></span>

4. <span data-ttu-id="b6cbd-142">בחר **תצוגה מקדימה**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-142">Select **Preview**.</span></span> <span data-ttu-id="b6cbd-143">בתיבת הדו-שיח, בחר באפשרות **OK**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-143">In the dialog box, select **OK**.</span></span> 

5. <span data-ttu-id="b6cbd-144">אשר את התיקונים בכרטיסייה **שורות יומן**. באפשרותך להציג רשימה של הפעולות המקוריות הקשורות לערכי ההוצאות שנבחרו ושונו, כמו גם לשורות התואמות שנוצרו ותוקנו.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-144">Verify the corrections on the **Journal lines** tab. You can view a list of the original actuals that are related to the selected expense entries that have been reversed and the corrected corresponding lines that have been created.</span></span>

6. <span data-ttu-id="b6cbd-145">אם התיקונים מופיעים כצפוי, בחר **OK**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-145">If the corrected values are as expected, select **Confirm**.</span></span> <span data-ttu-id="b6cbd-146">בתיבת הדו-שיח, בחר באפשרות **אשר**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-146">In the dialog box, select **OK.**</span></span> <span data-ttu-id="b6cbd-147">אם הערכים אינם מוצגים כצפוי, בחר **בטל** כדי לחזור לרשימה **הוצאות מאושרות**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-147">If the values are not showing as expected, select **Cancel** to return to the **Approved Expenses** list.</span></span> <span data-ttu-id="b6cbd-148">חזור על שלבים 2 עד 5.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-148">Repeat steps 2 through 5.</span></span> 

> [!NOTE]
> <span data-ttu-id="b6cbd-149">לכל הפעולות המתוקנות יהיו אותם ערכים שבחרת במקטע **ערכים חדשים עבור הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-149">The corrected actuals will have the same values that you selected in the **New values for Expenses** section.</span></span>

7. <span data-ttu-id="b6cbd-150">לאחר שתאשר את יומן התיקונים, נווט בחזרה לפרויקט או לפרויקטים שעדכנת כדי להציג את השינויים שלך.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-150">After you confirm the correction journal, navigate back to the project or projects that you updated, to view your changes.</span></span>  

8. <span data-ttu-id="b6cbd-151">בדף הפרויקט, בכרטיסייה **פעולות**, סקור את **תצוגת פעולות משויכות**.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-151">In the project page, on the **Actuals** tab, review the **Actual Associated View**.</span></span> <span data-ttu-id="b6cbd-152">הרשומות המקוריות והרשומות המתוקנות יוצגו.</span><span class="sxs-lookup"><span data-stu-id="b6cbd-152">The original entries and the corrected entries are listed.</span></span> <span data-ttu-id="b6cbd-153">האיור הבא מציג את סכומי רשומות ההוצאות המקוריים ואת הסכומים התואמים של רשומות ההוצאות המתוקנות. </span><span class="sxs-lookup"><span data-stu-id="b6cbd-153">The following graphic shows original expense entry amounts and the corresponding corrected expense entry amounts.</span></span> 




[!INCLUDE[footer-include](../includes/footer-banner.md)]