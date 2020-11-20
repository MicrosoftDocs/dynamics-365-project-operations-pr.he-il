---
title: ‏‏מוצרים
description: נושא זה מספק מידע על קטלוג המוצרים שבו תוכל להשתמש כדי לספק מידע ללקוחות על המוצרים והתמחור שהארגון שלכם מציע.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
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
ms.openlocfilehash: 30633a7445baaf99af5be5c88e35b24824022b93
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121264"
---
# <a name="products"></a><span data-ttu-id="6e489-103">‏‏מוצרים</span><span class="sxs-lookup"><span data-stu-id="6e489-103">Products</span></span>

<span data-ttu-id="6e489-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="6e489-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="6e489-105">מוצרים הם עמוד השדרה של העסק שלך.</span><span class="sxs-lookup"><span data-stu-id="6e489-105">Products are the backbone of your business.</span></span> <span data-ttu-id="6e489-106">קטלוג המוצרים ב- Dynamics 365 Sales Professional הוא אוסף של מוצרים ופרטי התמחור שלהם.</span><span class="sxs-lookup"><span data-stu-id="6e489-106">The product catalog in Dynamics 365 Sales Professional is a collection of products and pricing information.</span></span> <span data-ttu-id="6e489-107">הקל על נציגי המכירות שלך להגדיל את המכירות שלהם על-ידי יצירה מהירה של קטלוג מוצרים.</span><span class="sxs-lookup"><span data-stu-id="6e489-107">Make it easier for your sales reps to increase their sales by creating a product catalog quickly.</span></span>

## <a name="add-a-product"></a><span data-ttu-id="6e489-108">הוספת מוצר</span><span class="sxs-lookup"><span data-stu-id="6e489-108">Add a product</span></span>

1.  <span data-ttu-id="6e489-109">ודא שיש לך את את תפקיד מנהל המערכת או מנהל Sales Professional כדי שתוכל להוסיף מוצרים ב- Dynamics 365 Sales Professional.</span><span class="sxs-lookup"><span data-stu-id="6e489-109">Make sure you have the Sales Manager Professional or a System Administrator role so you can add products in Dynamics 365 Sales Professional.</span></span>
2.  <span data-ttu-id="6e489-110">במפת אתר, תחת **הגדרה**, בחר **מוצרים**.</span><span class="sxs-lookup"><span data-stu-id="6e489-110">In the site map, under **Setup**, select **Products**.</span></span>
3.  <span data-ttu-id="6e489-111">בחר **הוסף מוצר** והזן את המידע הבא:</span><span class="sxs-lookup"><span data-stu-id="6e489-111">Select **Add Product** and fill in the following information:</span></span>

    -  <span data-ttu-id="6e489-112">**שם**</span><span class="sxs-lookup"><span data-stu-id="6e489-112">**Name**</span></span>
    -  <span data-ttu-id="6e489-113">**מזהה מוצר**</span><span class="sxs-lookup"><span data-stu-id="6e489-113">**Product ID**</span></span>
    -  <span data-ttu-id="6e489-114">**הורה**: בחר משפחת מוצרים המהווה אב עבור המוצר.</span><span class="sxs-lookup"><span data-stu-id="6e489-114">**Parent**: Select a parent product family for the product.</span></span> <span data-ttu-id="6e489-115">אם אתה יוצר מוצר צאצא במשפחת מוצרים, השם של משפחת מוצרים המהווה אב מאוכלס כאן.</span><span class="sxs-lookup"><span data-stu-id="6e489-115">If you're creating a child product in a product family, the name of the parent product family is populated here.</span></span> <span data-ttu-id="6e489-116">אין אפשרות לשנות זאת לאחר שמירת הרשומה.</span><span class="sxs-lookup"><span data-stu-id="6e489-116">This can't be changed after the record is saved.</span></span>
    -  <span data-ttu-id="6e489-117">**בתוקף מ**/**בתוקף עד**: הגדר את תקופת התוקף עבור משפחת המוצרים על-ידי בחירת תאריך **בתוקף מ** ו **בתוקף עד**.</span><span class="sxs-lookup"><span data-stu-id="6e489-117">**Valid From**/**Valid To**: Define the period the product is valid for by selecting a **Valid From** and **Valid To** date.</span></span>
    -  <span data-ttu-id="6e489-118">**קבוצת יחידות**: בחר קבוצת יחידות.</span><span class="sxs-lookup"><span data-stu-id="6e489-118">**Unit Group**: Select a unit group.</span></span> <span data-ttu-id="6e489-119">קבוצת יחידות היא אוסף של היחידות השונות שבהן מוצר נמכר והיא מגדירה כיצד יקובצו פריטים בודדים לכמויות גדולות יותר.</span><span class="sxs-lookup"><span data-stu-id="6e489-119">A unit group is a collection of various units a product is sold in and defines how individual items are grouped into larger quantities.</span></span> <span data-ttu-id="6e489-120">לדוגמה, אם אתה מוסיף זרעים כמוצר, ייתכן שיצרת קבוצת יחידות הנקראת "זרעים", והגדרת את היחידה הראשית כ"מנה".</span><span class="sxs-lookup"><span data-stu-id="6e489-120">For example, if you're adding seeds as a product, you might have created a unit group called "Seeds" and defined its primary unit as "packet."</span></span>
    -  <span data-ttu-id="6e489-121">**ברירת מחדל ליחידה**: בחר את היחידה השכיחה ביותר שבה יימכר המוצר.</span><span class="sxs-lookup"><span data-stu-id="6e489-121">**Default Unit**: Select the most common unit in which the product will be sold.</span></span> <span data-ttu-id="6e489-122">יחידות הן הכמויות או המידות שבהן אתה מוכר את המוצרים שלך.</span><span class="sxs-lookup"><span data-stu-id="6e489-122">Units are the quantities or measurements that you sell your products in.</span></span> <span data-ttu-id="6e489-123">לדוגמה, אם אתה מוסיף זרעים כמוצר, תוכל למכור אותם במנות, תיבות או משטחים.</span><span class="sxs-lookup"><span data-stu-id="6e489-123">For example, if you're adding seeds as a product, you can sell it in packets, boxes, or pallets.</span></span> <span data-ttu-id="6e489-124">כל אחד מאלה הופך יחידה של המוצר.</span><span class="sxs-lookup"><span data-stu-id="6e489-124">Each of these becomes a unit of the product.</span></span> <span data-ttu-id="6e489-125">אם הזרעים נמכרים בעיקר במנות, בחר בו כיחידה.</span><span class="sxs-lookup"><span data-stu-id="6e489-125">If seeds are mostly sold in packets, select that as the unit.</span></span>
    -  <span data-ttu-id="6e489-126">**ברירת מחדל למחירון**: אם זהו מוצר חדש, שדה זה מוגדר לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="6e489-126">**Default Price List**: If this is a new product, this field is read-only.</span></span> <span data-ttu-id="6e489-127">לפני שתוכל לבחור מחירון ברירת מחדל, עליך למלא את כל השדות הנדרשים ולאחר מכן לשמור את הרשומה.</span><span class="sxs-lookup"><span data-stu-id="6e489-127">Before you can select a default price list, you must complete all the required fields and then save the record.</span></span> <span data-ttu-id="6e489-128">למרות שמחירון ברירת מחדל אינו נדרש, לאחר שמירת רשומת המוצר, מומלץ להגדיר מחירון ברירת מחדל עבור כל מוצר.</span><span class="sxs-lookup"><span data-stu-id="6e489-128">Although the default price list is not required, after you save the product record, it is a good idea to set a default price list for each product.</span></span> <span data-ttu-id="6e489-129">כך, אם רשומת לקוח אינה מכילה מחירון, Sales יכול להשתמש במחירון ברירת המחדל ליצירת הצעות מחיר, הזמנות וחשבוניות.</span><span class="sxs-lookup"><span data-stu-id="6e489-129">Then, if a customer record does not contain a price list, Sales can use the default price list for generating quotes, orders, and invoices.</span></span>
    -  <span data-ttu-id="6e489-130">**תמיכה במספרים עשרוניים**: עליך להזין מספר שלם בין 0 לבין 5.</span><span class="sxs-lookup"><span data-stu-id="6e489-130">**Decimals Supported**: Enter a whole number between 0 and 5.</span></span> <span data-ttu-id="6e489-131">אם אין אפשרות לחלק את המוצר לכמויות חלקיות, הקלד 0.</span><span class="sxs-lookup"><span data-stu-id="6e489-131">If the product can't be divided into fractional quantities, enter 0.</span></span> <span data-ttu-id="6e489-132">מידת הדיוק של השדה **כמות** בהצעת המחיר, ההזמנה או החשבונית של רשומת המוצר מאומתת כנגד הערך שבשדה זה, אם המוצר אינו כולל מחירון משויך.</span><span class="sxs-lookup"><span data-stu-id="6e489-132">The precision of the **Quantity** field in the quote, order, or invoice product record is validated against the value in this field if the product does not have an associated price list.</span></span>
    -  <span data-ttu-id="6e489-133">**נושא**: באפשרותך לשייך נושא למוצר זה.</span><span class="sxs-lookup"><span data-stu-id="6e489-133">**Subject**: Associate this product with a subject.</span></span> <span data-ttu-id="6e489-134">באפשרותך להשתמש בנושאים כדי לסווג את המוצרים שלך ולסנן דוחות.</span><span class="sxs-lookup"><span data-stu-id="6e489-134">You can use subjects to categorize your products and to filter reports.</span></span>

4.  <span data-ttu-id="6e489-135">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="6e489-135">Select **Save**.</span></span>
5.  <span data-ttu-id="6e489-136">בכרטיסיה **פרטים נוספים**, במקטע **פריטי מחירון** בחר את הסמל **פקודות נוספות**, ולאחר מכן בחר **הוסף פריט מחירון חדש**.</span><span class="sxs-lookup"><span data-stu-id="6e489-136">On the **Additional Details** tab, in the **Price List Items** section, select **More commands**, and then select **Add New Price List Item**.</span></span>
7.  <span data-ttu-id="6e489-137">בכרטיסיה **פרטים נוספים**, במקטע **קשר מוצר** בחר את הסמל **פקודות נוספות**, ולאחר מכן בחר **הוסף קשר מוצר חדש.**</span><span class="sxs-lookup"><span data-stu-id="6e489-137">On the **Additional Details** tab, in the **Product Relationship** section, select the **More commands** icon, and then select **Add New Product Relationship.**</span></span>
8.  <span data-ttu-id="6e489-138">בטופס **קשר מוצר חדש**, הזן את הפרטים הבאים, ובסרגל הפקודות בחר **שמור וסגור**:</span><span class="sxs-lookup"><span data-stu-id="6e489-138">In the **New Product Relationship** form, enter the following details, and on the command bar, select **Save and Close**:</span></span>

    -   <span data-ttu-id="6e489-139">**מוצר קשור**: בחר מוצר שברצונך להוסיף כמוצר קשור לרשומה קיימת של המוצר שעליו אתה עובד.</span><span class="sxs-lookup"><span data-stu-id="6e489-139">**Related Product**: Select a product that you want to add as a related product to the existing product record you're working on.</span></span>
    -   <span data-ttu-id="6e489-140">**סוג קשר מכירות**: בחר אם ברצונך להוסיף את המוצר למכירה משודרגת, מכירה צולבת, עזר, או מוצר תחליף.</span><span class="sxs-lookup"><span data-stu-id="6e489-140">**Sales Relation Type**: Select whether you want to add the product as an up-sell, cross-sell, accessory, or substitute product.</span></span>
    -   <span data-ttu-id="6e489-141">**כיוון**: בחר אם קשר הגומלין בין המוצרים יהיה חד-כיווני או דו-כיווני.</span><span class="sxs-lookup"><span data-stu-id="6e489-141">**Direction**:Select whether the relationship between the products will be unidirectional or bidirectional.</span></span> <span data-ttu-id="6e489-142">כאשר תבחר חד-כיווני, המוצר שבחרת בתיבה **מוצר קשור** יוצג כהמלצה עבור המוצר הקיים, אך לא להיפך.</span><span class="sxs-lookup"><span data-stu-id="6e489-142">When you select unidirectional, the product that you select in **Related Product** will be shown as a recommendation for the existing product but not vice versa.</span></span>

9.  <span data-ttu-id="6e489-143">בטופס המוצר, בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="6e489-143">On the Product form, select **Save**.</span></span>

## <a name="import-products"></a><span data-ttu-id="6e489-144">ייבוא מוצרים</span><span class="sxs-lookup"><span data-stu-id="6e489-144">Import products</span></span>

<span data-ttu-id="6e489-145">ניתן להשתמש בתבניות ייבוא כדי להביא נתוני מוצר בכמות גדולה אל Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="6e489-145">You can use import templates to bring bulk product data into Dynamics 365 Sales.</span></span>

## <a name="revise-a-product"></a><span data-ttu-id="6e489-146">תקן‬ מוצר</span><span class="sxs-lookup"><span data-stu-id="6e489-146">Revise a product</span></span>

<span data-ttu-id="6e489-147">שמור על רשימת מלאי המוצרים מעודכנת על-ידי תיקון מהיר של מאפיינים עבור המוצרים כנדרש, ופרסום מחדש של המידע כך שסוכני המכירות שלך יוכלו לראות את השינויים האחרונים שנערכו במלאי.</span><span class="sxs-lookup"><span data-stu-id="6e489-147">Keep the product inventory updated by quickly revising properties for the products, as required, and republishing the information so that your sales agents can see the latest changes to the inventory.</span></span>

1.  <span data-ttu-id="6e489-148">ודא שקיבלת אחד מתפקידי האבטחה הבאים או הרשאות שוות ערך: 'מנהל מערכת', 'אחראי על התאמה אישית של המערכת', 'מנהל מכירות', 'סמנכ"ל מכירות', 'סמנכ"ל שיווק' או 'מנכ''ל-מנהל עסק'.</span><span class="sxs-lookup"><span data-stu-id="6e489-148">Make sure that you have one of the following security roles or equivalent permissions: System Administrator, System Customizer, Sales Manager, Vice President of Sales, Vice President of Marketing, or CEO-Business Manager.</span></span>
2.  <span data-ttu-id="6e489-149">במפת אתר, בחר **מוצרים**.</span><span class="sxs-lookup"><span data-stu-id="6e489-149">In the site map, select **Products**.</span></span>
3.  <span data-ttu-id="6e489-150">פתח מוצר פעיל שברצונך לשנות, ובסרגל הפקודות בחר **תיקון**.</span><span class="sxs-lookup"><span data-stu-id="6e489-150">Open an active product that you want to change, and on the command bar, select **Revise**.</span></span>
4.  <span data-ttu-id="6e489-151">בתיבת הדו-שיח **אישור תיקון**, בחר **אישור‏**.</span><span class="sxs-lookup"><span data-stu-id="6e489-151">In the **Confirm Revise** dialog box, select **Confirm**.</span></span> <span data-ttu-id="6e489-152">פעולה זו תשנה את מצב המוצר ל **בתיקון**.</span><span class="sxs-lookup"><span data-stu-id="6e489-152">This will change the product status to **Under Revision**.</span></span>
5.  <span data-ttu-id="6e489-153">לאחר שתסיים לבצע שינויים, בסרגל הפקודות, בחר **פרסם**.</span><span class="sxs-lookup"><span data-stu-id="6e489-153">After you're done making changes, on the command bar, select **Publish**.</span></span>

    > [!TIP]
    > <span data-ttu-id="6e489-154">כדי לבטל את השינויים ולהמשיך בגירסה הפעילה האחרונה של המוצר, בחר **‏‫בטל‬**.</span><span class="sxs-lookup"><span data-stu-id="6e489-154">To revert the changes and continue with the last active version of the product, select **Revert**.</span></span> <span data-ttu-id="6e489-155">זה משנה המצב של המוצר בחזרה אל **פעיל**.</span><span class="sxs-lookup"><span data-stu-id="6e489-155">This changes the status of the product back to **Active**.</span></span>

## <a name="clone-a-product"></a><span data-ttu-id="6e489-156">שכפול‬ מוצר</span><span class="sxs-lookup"><span data-stu-id="6e489-156">Clone a product</span></span> 

<span data-ttu-id="6e489-157">כאשר אתה יוצר מוצר חדש, חסוך זמן על-ידי שכפול הקיים.</span><span class="sxs-lookup"><span data-stu-id="6e489-157">When you're creating a new product, save time by cloning an existing one.</span></span> <span data-ttu-id="6e489-158">פעולה זו יוצרת עותק של הרשומה המקורית עם כל הפרטים פרט לשם והמזהה.</span><span class="sxs-lookup"><span data-stu-id="6e489-158">This creates a copy of the original record with all the details except for the name and ID.</span></span>

1.  <span data-ttu-id="6e489-159">ודא שקיבלת אחד מתפקידי האבטחה הבאים או הרשאות שוות ערך: 'מנהל מערכת', 'אחראי על התאמה אישית של המערכת', 'מנהל מכירות', 'סמנכ"ל מכירות', 'סמנכ"ל שיווק' או 'מנכ''ל-מנהל עסק'.</span><span class="sxs-lookup"><span data-stu-id="6e489-159">Make sure that you have one of the following security roles or equivalent permissions: System Administrator, System Customizer, Sales Manager, Vice President of Sales, Vice President of Marketing, or CEO-Business Manager.</span></span>
2.  <span data-ttu-id="6e489-160">במפת אתר, בחר **מוצרים**.</span><span class="sxs-lookup"><span data-stu-id="6e489-160">In the site map, select **Products**.</span></span>
3.  <span data-ttu-id="6e489-161">בחר רשומת מוצר שברצונך לשכפל, ובסרגל הפקודות, בחר **שכפל**.</span><span class="sxs-lookup"><span data-stu-id="6e489-161">Select a product record that you want to clone, and on the command bar, select **Clone**.</span></span> <span data-ttu-id="6e489-162">תופיע תיבת הדו-שיח לאישור.</span><span class="sxs-lookup"><span data-stu-id="6e489-162">A confirmation dialog box appears.</span></span>
4.  <span data-ttu-id="6e489-163">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="6e489-163">Select **Confirm**.</span></span>

<span data-ttu-id="6e489-164">רשומת מוצר חדשה תיפתח עם אותם הפרטים כמו הרשומה המקורית פרט לשם והמזהה.</span><span class="sxs-lookup"><span data-stu-id="6e489-164">A new product record opens with the same details as the original one except for the name and ID.</span></span>

## <a name="retire-a-product"></a><span data-ttu-id="6e489-165">הוצאת מוצר משימוש</span><span class="sxs-lookup"><span data-stu-id="6e489-165">Retire a product</span></span> 

<span data-ttu-id="6e489-166">אם הארגון שלך אינו מוכר מוצר יותר, הוצא אותו משימוש כך המוצר לא יהיה זמין יותר לסוכני המכירות שלך.</span><span class="sxs-lookup"><span data-stu-id="6e489-166">If your organization doesn't sell a product anymore, retire it so that the product is no longer available to your sales agents.</span></span>

1.  <span data-ttu-id="6e489-167">ודא שקיבלת את תפקיד האבטחה 'מנהל מערכת' או 'מהנל Sales Professional' או הרשאות שוות ערך.</span><span class="sxs-lookup"><span data-stu-id="6e489-167">Make sure that you have the System Administrator or Sales Professional Manager role or equivalent permissions.</span></span>
2.  <span data-ttu-id="6e489-168">במפת אתר, בחר **מוצרים**.</span><span class="sxs-lookup"><span data-stu-id="6e489-168">In the site map, select **Products**.</span></span>
3.  <span data-ttu-id="6e489-169">פתח מוצר פעיל שברצונך להוציא משימוש, ובסרגל הפקודות בחר **הוצא משימוש**.</span><span class="sxs-lookup"><span data-stu-id="6e489-169">Open an active product that you want to retire, and on the command bar, select **Retire**.</span></span>
4.  <span data-ttu-id="6e489-170">בתיבת הדו-שיח **אישור הוצאה משימוש**, בחר **אישור‏**.</span><span class="sxs-lookup"><span data-stu-id="6e489-170">In the **Confirm Retire** dialog box, select **Confirm**.</span></span>


## <a name="delete-a-product"></a><span data-ttu-id="6e489-171">מחיקת מוצר</span><span class="sxs-lookup"><span data-stu-id="6e489-171">Delete a product</span></span>

<span data-ttu-id="6e489-172">כדי להפסיק את מכירת מוצר, מחק אותו.</span><span class="sxs-lookup"><span data-stu-id="6e489-172">To stop selling a product, delete it.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="6e489-173">אין באפשרותך לשחזר רשומה שנמחקה.</span><span class="sxs-lookup"><span data-stu-id="6e489-173">You can't recover a deleted record.</span></span>

1.  <span data-ttu-id="6e489-174">ודא שקיבלת את תפקיד האבטחה 'מנהל מערכת' או 'מהנל Sales Professional' או הרשאות שוות ערך.</span><span class="sxs-lookup"><span data-stu-id="6e489-174">Make sure that you have the System Administrator or Sales Professional Manager role or equivalent permissions.</span></span>
2.  <span data-ttu-id="6e489-175">במפת אתר, בחר **מוצרים**.</span><span class="sxs-lookup"><span data-stu-id="6e489-175">In the site map, select **Products**.</span></span>
3.  <span data-ttu-id="6e489-176">בחר רשומת מוצר שברצונך למחוק, ובסרגל הפקודות, בחר **מחק**.</span><span class="sxs-lookup"><span data-stu-id="6e489-176">Select a product record you want to delete, and on the command bar, select **Delete**.</span></span>
4.  <span data-ttu-id="6e489-177">בתיבת הדו-שיח **אישור מחיקה**, בחר **המשך‏**.</span><span class="sxs-lookup"><span data-stu-id="6e489-177">In the **Confirm Deletion** dialog box, select **Continue**.</span></span>
 
 ## <a name="quantity-factors-for-products"></a><span data-ttu-id="6e489-178">גורמי כמות למוצרים</span><span class="sxs-lookup"><span data-stu-id="6e489-178">Quantity factors for products</span></span>

<span data-ttu-id="6e489-179">גורמי כמות תומכים במכירה של מוצרים מבוססי מנוי.</span><span class="sxs-lookup"><span data-stu-id="6e489-179">Quantity factors support the sale of subscription-based products.</span></span> <span data-ttu-id="6e489-180">עבור מוצרים מבוססי מנוי, הכמות בהצעת המחיר או בסעיף החוזה של הפרויקט מבוטאת כמספר החודשים של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="6e489-180">For subscription-based products, the quantity on the quote or project contract line is expressed as the number of user months.</span></span>

<span data-ttu-id="6e489-181">בדרך כלל, המחיר של תוכנת המנוי מאוחסן בקטלוג כמחיר לכל משתמש בחודש.</span><span class="sxs-lookup"><span data-stu-id="6e489-181">Usually, the price of subscription software is stored in the catalog as the price per user per month.</span></span> <span data-ttu-id="6e489-182">אולם, תוכל להשתמש בתיאורי זמן אחרים במקום זאת.</span><span class="sxs-lookup"><span data-stu-id="6e489-182">However, you can use other time descriptions instead.</span></span> <span data-ttu-id="6e489-183">במהלך תהליך המכירה, המחיר בשורת הצעת המחיר הוא בדרך כלל מחיר לפי משתמש, לפי חודש, בתאם למשא ומתן שנוהל על-ידי סוכן מכירות של מחלקת ה- IT.</span><span class="sxs-lookup"><span data-stu-id="6e489-183">During the sales process, the price on the quote line is usually the per-user, per-month price that was negotiated and discounted by the IT sales agent.</span></span> <span data-ttu-id="6e489-184">לכל עסקה יש מספר שונה של משתמשים ומספר שונה של חודשי מנוי.</span><span class="sxs-lookup"><span data-stu-id="6e489-184">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="6e489-185">הכמות המשמשת לחישוב הסכום בשורת הצעת המחיר היא תוצר של מספר המשתמשים ומספר חודשי המנוי.</span><span class="sxs-lookup"><span data-stu-id="6e489-185">The quantity that is used to compute the amount of the quote line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="6e489-186">גורמי כמות מסתמכים על תכונות המוצר.</span><span class="sxs-lookup"><span data-stu-id="6e489-186">Quantity factors rely on product attributes.</span></span> <span data-ttu-id="6e489-187">בעת קביעת תצורה של מאפיינים מסוימים עבור מוצר, אפשר לסמן קבוצת משנה של מאפיינים אלה, או את כל המאפיינים, כגורמי כמות.</span><span class="sxs-lookup"><span data-stu-id="6e489-187">When you configure specific properties for a product, you can flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="6e489-188">המערכת מאמתת שרק מאפיינים מספריים או מאפייני מוצר בעלי סוג נתונים מספרי מסומנים כגורמי כמות.</span><span class="sxs-lookup"><span data-stu-id="6e489-188">The system validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="6e489-189">כאשר למוצר מוגדרים גורמי כמות והוא מתווסף לשורת הצעת מחיר, השדה **כמות** בשורת הצעת מחיר הופך לשדה לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="6e489-189">When a product that quantity factors are configured for is added to a quote line, the **Quantity** field on the quote line becomes a read-only field.</span></span> <span data-ttu-id="6e489-190">לאחר הזנת ערכים עבור מאפייני מוצר שהם גורמי כמות, מבוצע חישוב של הכמות בשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="6e489-190">After you enter values for product properties that are quantity factors, the quantity of the quote line is calculated.</span></span>

<span data-ttu-id="6e489-191">לדוגמה, אם המאפיינים הבאים קיימים:</span><span class="sxs-lookup"><span data-stu-id="6e489-191">For example, if there are the following properties:</span></span> 

- <span data-ttu-id="6e489-192">**מס' המשתמשים**: מספר המשתמשים</span><span class="sxs-lookup"><span data-stu-id="6e489-192">**No of users**: The number of users</span></span> 
- <span data-ttu-id="6e489-193">**מס' החודשים**: מספר חודשי המנוי</span><span class="sxs-lookup"><span data-stu-id="6e489-193">**No of Months**: The number of subscription months</span></span>
- <span data-ttu-id="6e489-194">**SKU של מוצר**</span><span class="sxs-lookup"><span data-stu-id="6e489-194">**Product SKU**</span></span> 

<span data-ttu-id="6e489-195">ניתן לסמן את המאפיין **מס' המשתמשים** ואת המאפיין **מס' החודשים** כגורמי כמות על-ידי עריכת המאפיינים של שורת המוצר.</span><span class="sxs-lookup"><span data-stu-id="6e489-195">The **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span> 
