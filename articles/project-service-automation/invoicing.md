---
title: הפקת חשבונית ב- Project Service Automation
description: נושא זה מספק מידע על הפקת חשבוניות.
author: rumant
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 03/11/2019
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365  Project Service Automation 2.x and 3.x
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 8d95f17aba0a4cab65a6f020aade5e19568de3be
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751730"
---
# <a name="invoicing-in-project-service-automation"></a><span data-ttu-id="11e1a-103">הפקת חשבונית ב- Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="11e1a-103">Invoicing in Project Service Automation</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="11e1a-104">הפקת חשבונית ב- Dynamics 365 Project Service Automation היא דבר שימושי מכיוון שהיא מעניקה למנהלי פרוייקטים רמת אישור שנייה לפני שהם יוצרים חשבוניות ללקוחות.</span><span class="sxs-lookup"><span data-stu-id="11e1a-104">Invoicing in Dynamics 365 Project Service Automation is useful because it gives project managers a second level of approval before they create invoices for customers.</span></span> <span data-ttu-id="11e1a-105">רמת האישור הראשונה מסתיימת כאשר ערכי הזמן וההוצאות שמגישים חברי צוות הפרוייקט מאושרים.</span><span class="sxs-lookup"><span data-stu-id="11e1a-105">The first level of approval is completed when the time and expense entries that project team members submit are approved.</span></span>

<span data-ttu-id="11e1a-106">PSA אינו מיועד ליצור חשבוניות המוצגות ללקוח, מהסיבות הבאות:</span><span class="sxs-lookup"><span data-stu-id="11e1a-106">PSA isn't designed to generate customer-facing invoices, for the following reasons:</span></span>

- <span data-ttu-id="11e1a-107">הוא לא מכיל מידע בנושא מס.</span><span class="sxs-lookup"><span data-stu-id="11e1a-107">It doesn't contain tax information.</span></span>
- <span data-ttu-id="11e1a-108">הוא לא ממיר מטבעות אחרים למטבע בהפקת החשבונית באמצעות שערי חליפין שתצורתם נקבעה כראוי.</span><span class="sxs-lookup"><span data-stu-id="11e1a-108">It can't convert other currencies to the invoicing currency by using correctly configured exchange rates.</span></span>
- <span data-ttu-id="11e1a-109">הוא לא מעצב כראוי חשבוניות כך שניתן להדפיס אותן.</span><span class="sxs-lookup"><span data-stu-id="11e1a-109">It can't correctly format invoices so that they can be printed.</span></span>

<span data-ttu-id="11e1a-110">במקום זאת, באפשרותך להשתמש במערכת פיננסית או חשבונאית כדי ליצור חשבוניות ללקוח המשתמשות במידע מהצעות לחשבוניות שנוצרות ב- PSA.</span><span class="sxs-lookup"><span data-stu-id="11e1a-110">Instead, you can use a financial or accounting system to create customer-facing invoices that use the information from invoice proposals that are generated in PSA.</span></span>

## <a name="creating-project-invoices-in-psa"></a><span data-ttu-id="11e1a-111">יצירת חשבוניות פרוייקט ב- PSA</span><span class="sxs-lookup"><span data-stu-id="11e1a-111">Creating project invoices in PSA</span></span>

<span data-ttu-id="11e1a-112">ניתן ליצור חשבונית פרוייקט אחת בכל פעם או בצובר.</span><span class="sxs-lookup"><span data-stu-id="11e1a-112">Project invoices can be created one at a time or in bulk.</span></span> <span data-ttu-id="11e1a-113">באפשרותך ליצור אותן באופן ידני או להגדיר אותן כך שייווצרו בהפעלות אוטומטיות.</span><span class="sxs-lookup"><span data-stu-id="11e1a-113">You can create them manually, or they can be configured so that they are generated in automated runs.</span></span>

### <a name="manually-create-project-invoices-in-psa"></a><span data-ttu-id="11e1a-114">יצירה ידנית של חשבוניות פרוייקט ב- PSA</span><span class="sxs-lookup"><span data-stu-id="11e1a-114">Manually create project invoices in PSA</span></span>

<span data-ttu-id="11e1a-115">מדף הרשימה של **חוזי הפרוייקט‬**, תוכל ליצור חשבוניות פרוייקט בנפרד עבור כל חוזה פרוייקט, או שתוכל ליצור חשבוניות בצובר עבור כמה חוזי פרוייקטים.</span><span class="sxs-lookup"><span data-stu-id="11e1a-115">From the **Project Contracts** list page, you can create project invoices separately for each project contract, or you can create invoices in bulk for multiple project contracts.</span></span>

<span data-ttu-id="11e1a-116">בצע שלב זה כדי ליצור חשבונית עבור חוזה פרוייקט ספציפי.</span><span class="sxs-lookup"><span data-stu-id="11e1a-116">Follow this step to create an invoice for a specific project contract.</span></span>

- <span data-ttu-id="11e1a-117">בדף הרשימה של **חוזי הפרוייקט**, פתח חוזה פרוייקט ולאחר מכן בחר **צור חשבונית**.</span><span class="sxs-lookup"><span data-stu-id="11e1a-117">On the **Project Contracts** list page, open a project contract, and then select **Create Invoice**.</span></span>

    ![יצירת חשבוניות פרוייקט עבור חוזה פרוייקט ספציפי](media/CreateProjectInvoicesOneByOne.png)

    <span data-ttu-id="11e1a-119">חשבונית נוצרת עבור כל העסקאות בחוזה הפרוייקט שנבחר במצב **מוכן להגיש חשבונית‬**.</span><span class="sxs-lookup"><span data-stu-id="11e1a-119">An invoice is generated for all transactions for the selected project contract that have a status of **Ready to Invoice**.</span></span> <span data-ttu-id="11e1a-120">עסקאות אלה כוללות מועד, הוצאות, אבני דרך וסעיפי חוזה מבוססי מוצר.</span><span class="sxs-lookup"><span data-stu-id="11e1a-120">These transactions include time, expenses, milestones, and product-based contract lines.</span></span>

<span data-ttu-id="11e1a-121">בצע את השלבים הבאים כדי ליצור חשבוניות בצובר.</span><span class="sxs-lookup"><span data-stu-id="11e1a-121">Follow these steps to create invoices in bulk.</span></span>

1. <span data-ttu-id="11e1a-122">בדף הרשימה של **חוזי הפרוייקט**, בחר חוזה פרוייקט אחד או יותר שעבורו תרצה ליצור חשבונות ולאחר מכן בחר **‏‫צור חשבוניות פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="11e1a-122">On the **Project Contracts** list page, select one or more project contracts that you must create an invoice for, and then select **Create Project Invoices**.</span></span>

    ![יצירת חשבוניות פרוייקט בצובר](media/CreateProjectInvoicesBulk.png)

    <span data-ttu-id="11e1a-124">הודעת אזהרה מיידעת אותך שייתכן שיהיה עיכוב לפני יצירת חשבוניות.</span><span class="sxs-lookup"><span data-stu-id="11e1a-124">A warning message informs you that there might be a delay before invoices are created.</span></span> <span data-ttu-id="11e1a-125">התהליך גם מוצג.</span><span class="sxs-lookup"><span data-stu-id="11e1a-125">The process is also shown.</span></span>

2. <span data-ttu-id="11e1a-126">בחר **אישור** כדי לסגור את תיבת ההודעה.</span><span class="sxs-lookup"><span data-stu-id="11e1a-126">Select **OK** to close the message box.</span></span>

    <span data-ttu-id="11e1a-127">חשבונית נוצרת עבור כל העסקאות בסעיף חוזה שנמצא במצב **מוכן להגיש חשבונית‬**.</span><span class="sxs-lookup"><span data-stu-id="11e1a-127">An invoice is generated for all transactions on a contract line that have a status of **Ready to Invoice**.</span></span> <span data-ttu-id="11e1a-128">עסקאות אלה כוללות מועד, הוצאות, אבני דרך וסעיפי חוזה מבוססי מוצר.</span><span class="sxs-lookup"><span data-stu-id="11e1a-128">These transactions include time, expenses, milestones, and product-based contract lines.</span></span>

3. <span data-ttu-id="11e1a-129">כדי להציג את החשבוניות שנוצרות, עבור אל **מכירות** \> **חיוב** \> **חשבוניות**.</span><span class="sxs-lookup"><span data-stu-id="11e1a-129">To view the invoices that are generated, go to **Sales** \> **Billing** \> **Invoices**.</span></span> <span data-ttu-id="11e1a-130">אתה תראה חשבונית אחת עבור כל חוזה פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="11e1a-130">You will see one invoice for each project contract.</span></span>

### <a name="set-up-automated-creation-of-project-invoices-in-psa"></a><span data-ttu-id="11e1a-131">הגדרת יצירה אוטומטית של חשבוניות פרוייקט ב- PSA</span><span class="sxs-lookup"><span data-stu-id="11e1a-131">Set up automated creation of project invoices in PSA</span></span>

<span data-ttu-id="11e1a-132">בצע את השלבים הבאים כדי לקבוע את התצורה של הפעלת חשבונית אוטומטית ב- PSA.</span><span class="sxs-lookup"><span data-stu-id="11e1a-132">Follow these steps to configure an automated invoice run in PSA.</span></span>

1. <span data-ttu-id="11e1a-133">עבור אל **Project Service** \> **הגדרות** \> **משימות אצווה**.</span><span class="sxs-lookup"><span data-stu-id="11e1a-133">Go to **Project Service** \> **Settings** \> **Batch jobs**.</span></span>
2. <span data-ttu-id="11e1a-134">צור משימת אצווה ושנה את שמה ל- **צור חשבוניות ב- PSA**.</span><span class="sxs-lookup"><span data-stu-id="11e1a-134">Create a batch job, and name it **PSA Create Invoices**.</span></span> <span data-ttu-id="11e1a-135">שם משימת האצווה חייב לכלול את המונח "צור חשבוניות".</span><span class="sxs-lookup"><span data-stu-id="11e1a-135">The name of the batch job must include the term "Create Invoices."</span></span>
3. <span data-ttu-id="11e1a-136">בשדה **סוג משימה**, בחר **ללא**.</span><span class="sxs-lookup"><span data-stu-id="11e1a-136">In the **Job type** field, select **None**.</span></span> <span data-ttu-id="11e1a-137">כברירת מחדל, האפשרות **תדירות יומית** והאפשרות **הוא פעיל** מוגדרות בתור **כן**.</span><span class="sxs-lookup"><span data-stu-id="11e1a-137">By default, the **Frequency Daily** and **Is Active** options are set to **Yes**.</span></span>
4. <span data-ttu-id="11e1a-138">בחר **הפעל זרימת עבודה**.</span><span class="sxs-lookup"><span data-stu-id="11e1a-138">Select **Run Workflow**.</span></span> <span data-ttu-id="11e1a-139">בתיבת הדו-שיח **חיפוש רשומה** תראה שלוש זרימות עבודה:</span><span class="sxs-lookup"><span data-stu-id="11e1a-139">In the **Look Up Record** dialog box, you will see three workflows:</span></span>

    - <span data-ttu-id="11e1a-140">ProcessRunCaller</span><span class="sxs-lookup"><span data-stu-id="11e1a-140">ProcessRunCaller</span></span>
    - <span data-ttu-id="11e1a-141">ProcessRunner</span><span class="sxs-lookup"><span data-stu-id="11e1a-141">ProcessRunner</span></span>
    - <span data-ttu-id="11e1a-142">UpdateRoleUtilization</span><span class="sxs-lookup"><span data-stu-id="11e1a-142">UpdateRoleUtilization</span></span>

5. <span data-ttu-id="11e1a-143">בחר את **ProcessRunCaller** ולאחר מכן בחר **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="11e1a-143">Select **ProcessRunCaller**, and then select **Add**.</span></span>
6. <span data-ttu-id="11e1a-144">בתיבת הדו-שיח הבאה, בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="11e1a-144">In the next dialog box, select **OK**.</span></span> <span data-ttu-id="11e1a-145">אחרי זרימת עבודה **שינה** תופיע זרימת עבודה **תהליך**.</span><span class="sxs-lookup"><span data-stu-id="11e1a-145">A **Sleep** workflow is followed by a **Process** workflow.</span></span>

    <span data-ttu-id="11e1a-146">תוכל גם לבחור את **ProcessRunner** בשלב 5.</span><span class="sxs-lookup"><span data-stu-id="11e1a-146">You can also select **ProcessRunner** in step 5.</span></span> <span data-ttu-id="11e1a-147">לאחר מכן, כשתבחר **אישור**, אחרי זרימת העבודה **תהליך** תופיע זרימת עבודה **שינה**.</span><span class="sxs-lookup"><span data-stu-id="11e1a-147">Then, when you select **OK**, a **Process** workflow is followed by a **Sleep** workflow.</span></span>

<span data-ttu-id="11e1a-148">זרימת העבודה **ProcessRunCaller** וזרימת העבודה **ProcessRunner** יוצרות חשבוניות.</span><span class="sxs-lookup"><span data-stu-id="11e1a-148">The **ProcessRunCaller** and **ProcessRunner** workflows create invoices.</span></span> <span data-ttu-id="11e1a-149">**ProcessRunCaller** קורא ל- **ProcessRunner**.</span><span class="sxs-lookup"><span data-stu-id="11e1a-149">**ProcessRunCaller** calls **ProcessRunner**.</span></span> <span data-ttu-id="11e1a-150">**ProcessRunner** היא למעשה זרימת העבודה שיוצרת למעשה את החשבוניות.</span><span class="sxs-lookup"><span data-stu-id="11e1a-150">**ProcessRunner** is the workflow that actually creates the invoices.</span></span> <span data-ttu-id="11e1a-151">היא עוברת על כל סעיפי החוזה שעבורם יש ליצור חשבונית, והיא יוצרת שורות עבור שורות אלו.</span><span class="sxs-lookup"><span data-stu-id="11e1a-151">It goes through all the contract lines that invoices must be created for, and it creates invoices for those lines.</span></span> <span data-ttu-id="11e1a-152">כדי לקבוע את סעיפי החוזה שעבורם יש ליצור חשבוניות, המשימה מחפשת תאריכים של הפעלת חשבוניות עבור סעיפי החוזה.</span><span class="sxs-lookup"><span data-stu-id="11e1a-152">To determine the contract lines that invoices must be created for, the job looks at invoice run dates for the contract lines.</span></span> <span data-ttu-id="11e1a-153">אם לסעיפי חוזה השייכים לחוזה אחד יש תאריך הפעלת חשבונית זהה, העסקאות משולבות לחשבונית אחת הכוללת שתי שורות בחשבונית.</span><span class="sxs-lookup"><span data-stu-id="11e1a-153">If contract lines that belong to one contract have the same invoice run date, the transactions are combined into one invoice that has two invoice lines.</span></span> <span data-ttu-id="11e1a-154">אם אין עסקאות שעבורן יש ליצור חשבוניות, המשימה מדלגת על יצירת חשבונית.</span><span class="sxs-lookup"><span data-stu-id="11e1a-154">If there are no transactions to create invoices for, the job skips invoice creation.</span></span>

<span data-ttu-id="11e1a-155">לאחר שהפעלת **ProcessRunner** הסתיימה, היא קוראת ל- **ProcessRunCaller**, מספקת את שעת הסיום ונסגרת.</span><span class="sxs-lookup"><span data-stu-id="11e1a-155">After **ProcessRunner** has finished running, it calls **ProcessRunCaller**, provides the end time, and is closed.</span></span> <span data-ttu-id="11e1a-156">לאחר מכן, **ProcessRunCaller** מפעילה שעון עצר הפועל במשך 24 שעות משעת הסיום שצוינה.</span><span class="sxs-lookup"><span data-stu-id="11e1a-156">**ProcessRunCaller** then starts a timer that runs for 24 hours from the specified end time.</span></span> <span data-ttu-id="11e1a-157">כששעון העצר מפסיק, **ProcessRunCaller** נסגרת.</span><span class="sxs-lookup"><span data-stu-id="11e1a-157">At the end of the timer, **ProcessRunCaller** is closed.</span></span>

<span data-ttu-id="11e1a-158">משימת תהליך האצווה ליצירת חשבוניות היא משימה חוזרת.</span><span class="sxs-lookup"><span data-stu-id="11e1a-158">The batch process job for creating invoices is a recurrent job.</span></span> <span data-ttu-id="11e1a-159">אם תהליך אצווה זה מופעל פעמים רבות, נוצרים מופעים מרובים של המשימה וגורמים לשגיאות.</span><span class="sxs-lookup"><span data-stu-id="11e1a-159">If this batch process is run many times, multiple instances of the job are created and cause errors.</span></span> <span data-ttu-id="11e1a-160">לכן עליך להתחיל את תהליך האצווה רק פעם אחת, ועליך להפעיל אותו מחדש רק אם הוא מפסיק לפעול.</span><span class="sxs-lookup"><span data-stu-id="11e1a-160">Therefore, you should start the batch process only one time, and you should restart it only if it stops running.</span></span>
 
### <a name="edit-a-draft-psa-invoice"></a><span data-ttu-id="11e1a-161">עריכת טיוטת חשבונית של PSA</span><span class="sxs-lookup"><span data-stu-id="11e1a-161">Edit a draft PSA invoice</span></span>

<span data-ttu-id="11e1a-162">בעת יצירת טיוטה של חשבונית פרוייקט, כל עסקאות המכירה שלא חויבו ושנוצרו בעת אישור ערכי הזמן וההוצאה יוכנסו לחשבונית.</span><span class="sxs-lookup"><span data-stu-id="11e1a-162">When you create a draft project invoice, all unbilled sales transactions that were created when the time and expense entries were approved are pulled onto the invoice.</span></span> <span data-ttu-id="11e1a-163">באפשרותך לבצע את ההתאמות הבאות כאשר החשבונית עדיין נמצאת בשלב טיוטה:</span><span class="sxs-lookup"><span data-stu-id="11e1a-163">You can make the following adjustments while the invoice is still in a draft stage:</span></span>

- <span data-ttu-id="11e1a-164">מחיקה או עריכה של פרטי שורת חשבונית.</span><span class="sxs-lookup"><span data-stu-id="11e1a-164">Delete or edit invoice line details.</span></span>
- <span data-ttu-id="11e1a-165">עריכה והתאמה של הכמות וסוג החיוב.</span><span class="sxs-lookup"><span data-stu-id="11e1a-165">Edit and adjust the quantity and billing type.</span></span>
- <span data-ttu-id="11e1a-166">הוספה ישירה של זמן, הוצאה ועמלות כעסקאות בחשבונית.</span><span class="sxs-lookup"><span data-stu-id="11e1a-166">Directly add time, expense, and fees as transactions on the invoice.</span></span> <span data-ttu-id="11e1a-167">תוכל להשתמש בתכונה זו אם שורת החשבונית מופתה אל סעיף חוזה שמאפשר את סיווגי העסקאות האלו.</span><span class="sxs-lookup"><span data-stu-id="11e1a-167">You can use this feature if the invoice line is mapped to a contract line that allows for these transaction classes.</span></span>

<span data-ttu-id="11e1a-168">בחר **אשר** כדי לאשר חשבונית.</span><span class="sxs-lookup"><span data-stu-id="11e1a-168">Select **Confirm** to confirm an invoice.</span></span> <span data-ttu-id="11e1a-169">פעולת האישור היא פעולה חד-סטרית.</span><span class="sxs-lookup"><span data-stu-id="11e1a-169">The Confirm action is a one-way action.</span></span> <span data-ttu-id="11e1a-170">בעת בחירה באפשרות **אשר**, המערכת הופכת את החשבונית לקריאה בלבד ויוצרת נתונים בפועל של מכירות שחויבו מכל פירוט של שורת חשבונית עבור כל שורת חשבונית.</span><span class="sxs-lookup"><span data-stu-id="11e1a-170">When you select **Confirm**, the system makes the invoice read-only and creates billed sales actuals from each invoice line detail for each invoice line.</span></span> <span data-ttu-id="11e1a-171">אם הפירוט בשורת החשבונית מפנה לנתונים בפועל של מכירות שלא חויבו, המערכת גם מבטלת את הנתונים בפועל של מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="11e1a-171">If the invoice line detail references an unbilled sales actual, the system also reverses the unbilled sales actual.</span></span> <span data-ttu-id="11e1a-172">(כל פירוט בשורת חשבונית שנוצר מערך זמן או הוצאה יפנה לנתונים בפועל של מכירות שלא חויבו.) מערכות שילוב של ספר ראשי יכולות להשתמש בביטול זה כדי לבטל עבודת פרוייקט בתהליך (WIP) למטרה חשבונאית.</span><span class="sxs-lookup"><span data-stu-id="11e1a-172">(Any invoice line detail that was created from a time or expense entry will reference an unbilled sales actual.) General ledger integration systems can use this reversal to reverse project work in progress (WIP) for accounting purposes.</span></span>

### <a name="correct-a-confirmed-psa-invoice"></a><span data-ttu-id="11e1a-173">תיקון חשבונית PSA מאושרת</span><span class="sxs-lookup"><span data-stu-id="11e1a-173">Correct a confirmed PSA invoice</span></span>

<span data-ttu-id="11e1a-174">ניתן לערוך חשבוניות PSA מאושרות (מתוקנות).</span><span class="sxs-lookup"><span data-stu-id="11e1a-174">Confirmed PSA invoices can be edited (corrected).</span></span> <span data-ttu-id="11e1a-175">בעת תיקון חשבונית מאושרת, נוצרת טיוטה חדשה לחשבונית תיקון.</span><span class="sxs-lookup"><span data-stu-id="11e1a-175">When you correct a confirmed invoice, a new draft corrective invoice is created.</span></span> <span data-ttu-id="11e1a-176">מכיוון שההנחה היא שברצונך לבטל את כל העסקאות והכמויות מהחשבונית המקורית, חשבונית תיקון זו כוללת את כל העסקאות מהחשבונית המקורית וכל הכמויות שבה הן 0 (אפס).</span><span class="sxs-lookup"><span data-stu-id="11e1a-176">Because the assumption is that you want to reverse all the transactions and quantities from the original invoice, this corrective invoice includes all the transactions from the original invoice, and all the quantities on it are 0 (zero).</span></span>

<span data-ttu-id="11e1a-177">אם יש עסקאות כלשהן שלא דורשות תיקון, תוכל להסיר אותן מהטיוטה של חשבונית התיקון.</span><span class="sxs-lookup"><span data-stu-id="11e1a-177">If any transactions don't require correction, you can remove them from the draft corrective invoice.</span></span> <span data-ttu-id="11e1a-178">אם ברצונך לבטל או להחזיר כמות חלקית בלבד, תוכל לערוך את השדה **כמות** בפירוט השורה.</span><span class="sxs-lookup"><span data-stu-id="11e1a-178">If you want to reverse or return only a partial quantity, you can edit the **Quantity** field on the line detail.</span></span> <span data-ttu-id="11e1a-179">אם תפתח את הפירוט בשורת החשבונית, תוכל לראות את הכמות בחשבונית המקורית.</span><span class="sxs-lookup"><span data-stu-id="11e1a-179">If you open the invoice line detail, you can see the original invoice quantity.</span></span> <span data-ttu-id="11e1a-180">לאחר מכן תוכל לערוך את הכמות בחשבונית הנוכחית כך שתהיה קטנה או גדולה מהכמות בחשבונית המקורית.</span><span class="sxs-lookup"><span data-stu-id="11e1a-180">You can then edit the current invoice quantity so that it's less than or more than the original invoice quantity.</span></span>

<span data-ttu-id="11e1a-181">בעת אישור חשבונית תיקון, הנתונים בפועל המקוריים של המכירות שחויבו מבוטלים, ונוצרים נתונים בפועל חדשים למכירות שחויבו.</span><span class="sxs-lookup"><span data-stu-id="11e1a-181">When you confirm a corrective invoice, the original billed sales actual is reversed, and a new billed sales actual is created.</span></span> <span data-ttu-id="11e1a-182">אם הכמות הופחתה, ההפרש יגרום גם ליצירה של נתונים בפועל חדשים של מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="11e1a-182">If the quantity was reduced, the difference will cause a new unbilled sales actual to be created too.</span></span> <span data-ttu-id="11e1a-183">לדוגמה, אם המכירה המקורית שחויבה היתה עבור שמונה שעות, ובפרטי שורת חשבונית התיקון יש כמות מופחתת של שש שעות, PSA יבטל את השורה המקורית של המכירות שחויבו ויצור שני נתונים בפועל חדשים:</span><span class="sxs-lookup"><span data-stu-id="11e1a-183">For example, if the original billed sales was for eight hours, and the corrective invoice line detail has a reduced quantity of six hours, PSA reverses the original billed sales line and creates two new actuals:</span></span>

- <span data-ttu-id="11e1a-184">נתונים בפועל למכירות שחויבו עבור שש שעות.</span><span class="sxs-lookup"><span data-stu-id="11e1a-184">A billed sales actual for six hours.</span></span>
- <span data-ttu-id="11e1a-185">נתונים בפועל למכירות שלא חויבו עבור השעתיים שנותרו.</span><span class="sxs-lookup"><span data-stu-id="11e1a-185">An unbilled sales actual for the remaining two hours.</span></span> <span data-ttu-id="11e1a-186">ניתן לחייב עסקה זו במועד מאוחר יותר או לסמנה כלא ניתנת לחיוב, בהתאם למשא ומתן עם הלקוח.</span><span class="sxs-lookup"><span data-stu-id="11e1a-186">This transaction can either be billed later or marked as non-chargeable, depending on the negotiations with the customer.</span></span>
