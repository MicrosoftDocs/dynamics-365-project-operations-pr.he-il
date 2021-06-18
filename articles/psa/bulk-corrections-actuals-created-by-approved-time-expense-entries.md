---
title: תיקונים בכמויות גדולות של פעולות שנוצרו על ידי ערכי זמן והוצאות מאושרים
description: נושא זה מסביר כיצד מנהל מערכת יכול לבצע תיקונים בודדים או רבים לערכי זמן או הוצאה שאושרו בעבר אם החיוב לא הושלם.
author: rumant
ms.date: 04/02/2020
ms.topic: article
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
search.app:
- ProjectOperations
ms.openlocfilehash: c6d849e4be9e3687396cd6a0c4158d92f25c7879
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012047"
---
# <a name="bulk-corrections-of-actuals-created-by-approved-time-and-expense-entries"></a><span data-ttu-id="13659-103">תיקונים בכמויות גדולות של פעולות שנוצרו על ידי ערכי זמן והוצאות מאושרים</span><span class="sxs-lookup"><span data-stu-id="13659-103">Bulk corrections of actuals created by approved time and expense entries</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="13659-104">לעיתים, רשומת זמן או הוצאה יוזנו בצורה שגויה.</span><span class="sxs-lookup"><span data-stu-id="13659-104">Occasionally a time or expense entry may be entered incorrectly.</span></span> <span data-ttu-id="13659-105">לדוגמה, יועץ עשוי לבחור בתאריך הלא נכון בעת יצירת ערך זמן או שהוא עשוי להחליף בין המספרים בעת הזנת הוצאה.</span><span class="sxs-lookup"><span data-stu-id="13659-105">For example, a consultant might select the wrong date when creating a time entry or they might transpose the numbers when entering an expense.</span></span> <span data-ttu-id="13659-106">אם יועץ לא יכול לבצע את העדכונים בערכים שהוגשו, מנהל מערכת יכול לתקן את הרשומה בפרויקט ישירות.</span><span class="sxs-lookup"><span data-stu-id="13659-106">If a consultant can’t make the updates to the submitted entries, an administrator can directly correct the entry for a project.</span></span>

<span data-ttu-id="13659-107">כדי להשלים את הנוהל בנושא זה, תצטרך הרשאות מנהל מערכת.</span><span class="sxs-lookup"><span data-stu-id="13659-107">To complete the procedures in this topic, you will need Administrator permissions.</span></span>

## <a name="correct-approved-time-entries"></a><span data-ttu-id="13659-108">תיקון רשומות זמן מאושרות</span><span class="sxs-lookup"><span data-stu-id="13659-108">Correct approved time entries</span></span>     

<span data-ttu-id="13659-109">בצע את הצעדים הבאים כדי לתקן ערכי זמן בודדים או מרובים בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="13659-109">Complete the following steps to correct single or multiple time entries for a project.</span></span>

1. <span data-ttu-id="13659-110">באזור **מכירות**, בחר **"עסקאות** ואז בחר **זמן מאושר**.</span><span class="sxs-lookup"><span data-stu-id="13659-110">In the **Sales** area, select **Transactions**, and then select **Approved Time**.</span></span> 

2. <span data-ttu-id="13659-111">ברשימת **זמן מאושר**, אתר ובחר רשומת זמן מאושרת אחת או יותר לתיקון.</span><span class="sxs-lookup"><span data-stu-id="13659-111">In the **Approved Time** list, locate and select one or more approved time entries to correct.</span></span> <span data-ttu-id="13659-112">אתה יכול להשתמש בפילטר כדי לאתר ערכים קשורים.</span><span class="sxs-lookup"><span data-stu-id="13659-112">You can use the filter to locate related entries.</span></span> <span data-ttu-id="13659-113">לדוגמה, אתה יכול לסנן לפי מזהה הפרויקט ולבחור את כל רשומות הזמן המאושרות של מזהה הפרויקט הזה.</span><span class="sxs-lookup"><span data-stu-id="13659-113">For example, you might filter on a Project ID, and select all approved time entries with that Project ID.</span></span>

3. <span data-ttu-id="13659-114">בחר **‏‎תקן רשומות**.</span><span class="sxs-lookup"><span data-stu-id="13659-114">Select **Correct entries**.</span></span> <span data-ttu-id="13659-115">יומן תיקון חדש ייווצר אוטומטית, עם **תיקון זמן** מהסוג שהוקצה.</span><span class="sxs-lookup"><span data-stu-id="13659-115">A new correction journal is automatically created, with the assigned type **Time correction**.</span></span> <span data-ttu-id="13659-116">הערכים שבחרת יתווספו ליומן.</span><span class="sxs-lookup"><span data-stu-id="13659-116">The entries you selected are added to the journal.</span></span> 

4. <span data-ttu-id="13659-117">בדף **יומן חדש**, הזן **תיאור** ליומן התיקונים שלך, ואז בחר את כרטיסיית **תיקוני ערכי זמן**.</span><span class="sxs-lookup"><span data-stu-id="13659-117">On the **New Journal** page, enter a **Description** for your correction journal, and then select the **Time Entry Corrections** tab.</span></span>  
5. <span data-ttu-id="13659-118">בתוך המקטע **ערכים חדשים לערכי זמן**, עדכן את השדות עם המידע הנכון בהתאם לצורך.</span><span class="sxs-lookup"><span data-stu-id="13659-118">In the **New Values for Time Entries** section, update the fields with the correct information as necessary.</span></span> <span data-ttu-id="13659-119">לדוגמה, באפשרותך לשנות את הפרויקט שהוקצה או את המשאב הניתן להזמנה.</span><span class="sxs-lookup"><span data-stu-id="13659-119">For example, you can change the assigned project or the bookable resource.</span></span>

6. <span data-ttu-id="13659-120">בחר **תצוגה מקדימה**.</span><span class="sxs-lookup"><span data-stu-id="13659-120">Select **Preview**.</span></span> <span data-ttu-id="13659-121">בתיבת הדו-שיח, בחר באפשרות **OK**.</span><span class="sxs-lookup"><span data-stu-id="13659-121">In the dialog box, select **OK**.</span></span> <span data-ttu-id="13659-122">בכרטיסייה **שורות יומן** תוכל להציג רשימה של הפעולות המקוריות הקשורות לערכי הזמן שנבחרו ושונו ולשורות התואמות שנוצרו ותוקנו.</span><span class="sxs-lookup"><span data-stu-id="13659-122">On the **Journal lines** tab, you can view a list of the original actuals that are related to the selected time entries that have been reversed and the corrected corresponding lines that have been created.</span></span> <span data-ttu-id="13659-123">אם יש צורך לבצע תיקונים נוספים, חזור על שלבים 5 ו -6.</span><span class="sxs-lookup"><span data-stu-id="13659-123">If additional corrections need to be made, repeat steps 5 and 6.</span></span> 

> [!NOTE]
> <span data-ttu-id="13659-124">לכל הפעולות המתוקנות יהיו אותם ערכים שבחרת **ערכים חדשים לערכי זמן**.</span><span class="sxs-lookup"><span data-stu-id="13659-124">All the corrected actuals will have the same values that you selected in the **New values for Time Entries** section.</span></span>

7. <span data-ttu-id="13659-125">אם התיקונים מופיעים כצפוי, בחר **אשר**.</span><span class="sxs-lookup"><span data-stu-id="13659-125">If the corrections appear as expected, select **Confirm**.</span></span> <span data-ttu-id="13659-126">בתיבת הדו-שיח, בחר באפשרות **OK**.</span><span class="sxs-lookup"><span data-stu-id="13659-126">In the dialog box, select **OK**.</span></span>

8. <span data-ttu-id="13659-127">חזור לאזור **מכירות**, בחר **פרויקטים** ואז פתח את הפרויקט שעבורו עדכנת את רשומות הזמן זה עתה.</span><span class="sxs-lookup"><span data-stu-id="13659-127">Return to the **Sales** area, select **Projects**, and then open the project for which you just updated the time entries.</span></span> 

9. <span data-ttu-id="13659-128">בדף **פרויקטים**, בכרטיסייה **פעולות**, צפה בשינויים שביצעת.</span><span class="sxs-lookup"><span data-stu-id="13659-128">On the **Projects** page, on the **Actuals** tab, view the changes that you made.</span></span> 

> [!NOTE]
> <span data-ttu-id="13659-129">אם הכרטיסייה **פעולות** אינה גלויה, בחר **קשורים** > **פעולות**.</span><span class="sxs-lookup"><span data-stu-id="13659-129">If the **Actuals** tab is not visible, select **Related** > **Actuals**.</span></span>  

10. <span data-ttu-id="13659-130">ברשימה **תצוגת פעולות משויכות**, אתה יכול לראות שרשומות הזמן המקוריות ששונו עדיין מופיעות ברשימה, וכך גם ערכי הזמן המתוקנים התואמים.</span><span class="sxs-lookup"><span data-stu-id="13659-130">In the **Actual Associated View** list, you can see that the original time entries that have been reversed are still listed, as are the corresponding corrected time entries.</span></span> 

<span data-ttu-id="13659-131">לדוגמה, באיור הבא ישנן שתי שורות פריטים בכמות של 8.00 אשר להם חיובים הרשומים בעמודה "סכום".</span><span class="sxs-lookup"><span data-stu-id="13659-131">For example, in the following graphic, there are two line items with a quantity of 8.00 that have debits listed in the Amount column.</span></span> <span data-ttu-id="13659-132">בנוסף, ישנן שתי שורות פריטים בכמות של 8.00- המציגים סכומי זיכוי בעמודה "סכום".</span><span class="sxs-lookup"><span data-stu-id="13659-132">Additionally, there are two line items with a quantity of -8.00 that show credited amounts in the Amount column.</span></span> <span data-ttu-id="13659-133">תיקונים אלו מביאים את הכמות לאפס.</span><span class="sxs-lookup"><span data-stu-id="13659-133">These corrections bring the quantity to zero.</span></span>

![רשימת "תצוגת פעולות משויכות"](https://github.com/MicrosoftDocs/dynamics-365-customer-engagement-pr/blob/bulk-corrections-actuals-created-by-approved-time-expense-entries.md/time-actuals.png)
 
## <a name="correct-approved-expense-entries"></a><span data-ttu-id="13659-135">תיקון רשומות זמן מאושרות</span><span class="sxs-lookup"><span data-stu-id="13659-135">Correct approved expense entries</span></span>

<span data-ttu-id="13659-136">בצע את הצעדים הבאים לתיקון רשומת הוצאה אחת או יותר.</span><span class="sxs-lookup"><span data-stu-id="13659-136">Complete the following steps to correct one or more expense entries.</span></span> 

1. <span data-ttu-id="13659-137">באזור **מכירות**, בחלונית הניווט השמאלית, מתחת **עסקאות**, בחר **הוצאות מאושרות**.</span><span class="sxs-lookup"><span data-stu-id="13659-137">In the **Sales** area, in the left navigation pane, under **Transactions**, select **Approved Expenses**.</span></span>

2. <span data-ttu-id="13659-138">ברשימה **הוצאות מאושרות**, בחר את הפרויקט שברצונך לתקן ואז בחר **תיקון רשומות**.</span><span class="sxs-lookup"><span data-stu-id="13659-138">In the **Approved Expenses** list, select the project that you want to correct, and then select **Correct entries**.</span></span> <span data-ttu-id="13659-139">יומן תיקון חדש ייווצר אוטומטית, עם **תיקון הוצאה** מהסוג שהוקצה.</span><span class="sxs-lookup"><span data-stu-id="13659-139">A new correction journal will be created automatically with the assigned type of **Expense correction**.</span></span> 

3. <span data-ttu-id="13659-140">בדף **יומן חדש**, הזן **תיאור** לתיקון, ובכרטיסייה **תיקון הוצאות**, במקטע **ערכים חדשים להוצאות**, בחר בשדות הנתונים שברצונך לתקן עבור שורות ההוצאות שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="13659-140">On the **New Journal** page, enter a **Description** for the correction, and on the **Expense Correction** tab, in the **New Values for Expenses** section, select the data fields that you want to correct for the selected expense lines.</span></span> <span data-ttu-id="13659-141">לדוגמה, אתה יכול להקצות את ההוצאה **פרויקט** אחר, או לתקן את **קטגוריית הוצאות**, **תאריך ההוצאה**, או **משאב הניתן להזמנה**.</span><span class="sxs-lookup"><span data-stu-id="13659-141">For example, you can assign the expense to another **Project**, or correct the **Expense Category**, **Expense Date**, or **Bookable Resource**.</span></span>

4. <span data-ttu-id="13659-142">בחר **תצוגה מקדימה**.</span><span class="sxs-lookup"><span data-stu-id="13659-142">Select **Preview**.</span></span> <span data-ttu-id="13659-143">בתיבת הדו-שיח, בחר באפשרות **OK**.</span><span class="sxs-lookup"><span data-stu-id="13659-143">In the dialog box, select **OK**.</span></span> 

5. <span data-ttu-id="13659-144">אשר את התיקונים בכרטיסייה **שורות יומן**. באפשרותך להציג רשימה של הפעולות המקוריות הקשורות לערכי ההוצאות שנבחרו ושונו, כמו גם לשורות התואמות שנוצרו ותוקנו.</span><span class="sxs-lookup"><span data-stu-id="13659-144">Verify the corrections on the **Journal lines** tab. You can view a list of the original actuals that are related to the selected expense entries that have been reversed and the corrected corresponding lines that have been created.</span></span>

6. <span data-ttu-id="13659-145">אם התיקונים מופיעים כצפוי, בחר **OK**.</span><span class="sxs-lookup"><span data-stu-id="13659-145">If the corrected values are as expected, select **Confirm**.</span></span> <span data-ttu-id="13659-146">בתיבת הדו-שיח, בחר באפשרות **אשר**.</span><span class="sxs-lookup"><span data-stu-id="13659-146">In the dialog box, select **OK.**</span></span> <span data-ttu-id="13659-147">אם הערכים אינם מוצגים כצפוי, בחר **בטל** כדי לחזור לרשימה **הוצאות מאושרות**.</span><span class="sxs-lookup"><span data-stu-id="13659-147">If the values are not showing as expected, select **Cancel** to return to the **Approved Expenses** list.</span></span> <span data-ttu-id="13659-148">חזור על שלבים 2 עד 5.</span><span class="sxs-lookup"><span data-stu-id="13659-148">Repeat steps 2 through 5.</span></span> 

> [!NOTE]
> <span data-ttu-id="13659-149">לכל הפעולות המתוקנות יהיו אותם ערכים שבחרת במקטע **ערכים חדשים עבור הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="13659-149">The corrected actuals will have the same values that you selected in the **New values for Expenses** section.</span></span>

7. <span data-ttu-id="13659-150">לאחר שתאשר את יומן התיקונים, נווט בחזרה לפרויקט או לפרויקטים שעדכנת כדי להציג את השינויים שלך.</span><span class="sxs-lookup"><span data-stu-id="13659-150">After you confirm the correction journal, navigate back to the project or projects that you updated, to view your changes.</span></span>  

8. <span data-ttu-id="13659-151">בדף הפרויקט, בכרטיסייה **פעולות**, סקור את **תצוגת פעולות משויכות**.</span><span class="sxs-lookup"><span data-stu-id="13659-151">In the project page, on the **Actuals** tab, review the **Actual Associated View**.</span></span> <span data-ttu-id="13659-152">הרשומות המקוריות והרשומות המתוקנות יוצגו.</span><span class="sxs-lookup"><span data-stu-id="13659-152">The original entries and the corrected entries are listed.</span></span> <span data-ttu-id="13659-153">האיור הבא מציג את סכומי רשומות ההוצאות המקוריים ואת הסכומים התואמים של רשומות ההוצאות המתוקנות. </span><span class="sxs-lookup"><span data-stu-id="13659-153">The following graphic shows original expense entry amounts and the corresponding corrected expense entry amounts.</span></span> 

![פעולות הוצאה](https://user-images.githubusercontent.com/60806505/77122219-4cd52900-69fa-11ea-8349-ccd2ffebf640.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]