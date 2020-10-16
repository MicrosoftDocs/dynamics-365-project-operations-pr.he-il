---
title: מיפוי פרויקטים ומשימות בשורות הצעת מחיר מבוססת פרויקט
description: נושא זה מספק מידע על אופן מיפוי פרויקטים ומשימות בשורת משימות מבוססת פרויקט.
author: rumant
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d726ab09da0e502da99191f7e7469c47f79b6e7c
ms.sourcegitcommit: 6b396ccf5e76230a42a2f933a3aaa5b8149790bb
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/06/2020
ms.locfileid: "3964908"
---
# <a name="map-projects-and-tasks-to-a-project-based-quote-line"></a><span data-ttu-id="2e5f9-103">מיפוי פרויקטים ומשימות בשורות הצעת מחיר מבוססת פרויקט</span><span class="sxs-lookup"><span data-stu-id="2e5f9-103">Map projects and tasks to a project-based quote line</span></span>

<span data-ttu-id="2e5f9-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="2e5f9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="2e5f9-105">בשורות הצעות מחיר מבוססות פרויקט, אפשר למפות את המשימות הספציפיות של פרויקט שכבר משויך לשורת הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-105">On project-based quote lines, you can map the specific tasks of a project that is already associated to a quote line.</span></span>

<span data-ttu-id="2e5f9-106">כשממפים משימות לשורת הצעת מחיר, רק עליהם יכולו הפריטים הבאים, שהגדרת בשורת הצעת המחיר:</span><span class="sxs-lookup"><span data-stu-id="2e5f9-106">When you map tasks to a quote line, the following items you defined on the quote line will only apply to those tasks:</span></span>

- <span data-ttu-id="2e5f9-107">שיטת חיוב</span><span class="sxs-lookup"><span data-stu-id="2e5f9-107">Billing method</span></span>
- <span data-ttu-id="2e5f9-108">אפשרויות של יכולת חיוב</span><span class="sxs-lookup"><span data-stu-id="2e5f9-108">Chargeability options</span></span>
- <span data-ttu-id="2e5f9-109">מגבלות 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="2e5f9-109">Not-to-exceed limits</span></span>
- <span data-ttu-id="2e5f9-110">לקוחות</span><span class="sxs-lookup"><span data-stu-id="2e5f9-110">Customers</span></span>

<span data-ttu-id="2e5f9-111">לדוגמה, ייתכן שיהיה לך פרויקט שבו שלב אחד הוא במחיר קבוע וכל שאר השלבים הם לפי זמן וחומרים.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-111">For example, you might have a project where one phase is fixed price and all the other phases are time and materials.</span></span> <span data-ttu-id="2e5f9-112">במקרה זה, ניתן לשייך את השלב הראשון ואת כל המשימות הבנות שלו לשורת הצעת המחיר של אותו שלב עם שיטת חיוב במחיר קבוע.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-112">In this case, you can associate the first phase, and all of its child tasks, to the quote line for that phase with a fixed price billing method.</span></span> <span data-ttu-id="2e5f9-113">לאחר מכן, ניתן לשייך את כל השלבים האחרים לשורת הצעת המחיר מבוססת זמן וחומרים.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-113">You can then associate all the other phases to the time and materials-based quote line.</span></span>

## <a name="associate-tasks-to-project-based-quote-lines"></a><span data-ttu-id="2e5f9-114">שיוך משימות להצעות מחיר מבוססות פרויקט</span><span class="sxs-lookup"><span data-stu-id="2e5f9-114">Associate tasks to project-based quote lines</span></span>

<span data-ttu-id="2e5f9-115">ניתן לשייך משימות לשורות הצעות מחיר מהמיקומים הבאים:</span><span class="sxs-lookup"><span data-stu-id="2e5f9-115">You can associate tasks with quote lines from the following locations:</span></span>

- <span data-ttu-id="2e5f9-116">מהדף **פרויקט** > לשונית **חיוב משימות** (אופטימלי)</span><span class="sxs-lookup"><span data-stu-id="2e5f9-116">**Project** page > **Task billing** tab (optimal)</span></span>
- <span data-ttu-id="2e5f9-117">מהדף **שורת הצעת מחיר** > כרטיסיה **משימות הניתנות לחיוב**</span><span class="sxs-lookup"><span data-stu-id="2e5f9-117">**Quote Line** page > **Chargeable tasks** tab</span></span> 

### <a name="from-the-project-page"></a><span data-ttu-id="2e5f9-118">מדך הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e5f9-118">From the Project page</span></span>

<span data-ttu-id="2e5f9-119">הדף **פרויקט** מספק את החוויה האופטימלית עבור שיוך משימות לשורות הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-119">The **Project** page provides the optimal experience for associating tasks to quote lines.</span></span> <span data-ttu-id="2e5f9-120">אפשר להשתמש בדף זה כדי לבחור מספר משימות ולשייך את כולן, בתוספת המשימות הבנות שלהן, לשורת הצעת המחיר שנבחרה.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-120">You can use this page to select multiple tasks and associate all of them, plus their child tasks, to the selected quote line.</span></span>

1. <span data-ttu-id="2e5f9-121">בכרטיסיה **כללי** של שורת הצעת מחיר מבוססת פרויקט, אמת שהשדה **פרויקט** מלא.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-121">On the **General** tab of a project–based quote line, verify the **Project** field is filled out.</span></span>
2. <span data-ttu-id="2e5f9-122">בשדה **משימות כלולות**, בחר **משימות נבחרות בלבד**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-122">In the **Included tasks** field, select **Selected tasks only**.</span></span>
3. <span data-ttu-id="2e5f9-123">שמור את שורות הצעת המחיר מבוססות הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-123">Save the project-based quote line.</span></span> <span data-ttu-id="2e5f9-124">לאחר ריענון הטופס, תוצג הכרטיסיה **משימות הניתנות לחיוב**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-124">When the form refreshes, the **Chargeable tasks** tab displays.</span></span>
4. <span data-ttu-id="2e5f9-125">בכרטיסיה **כללי**, בחר את הקישור לפרויקט מתוך השדה **פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-125">On the **General** tab, select the link for the project from the **Project** field.</span></span>
5. <span data-ttu-id="2e5f9-126">בדף **פרוייקט**, בחר בכרטיסיה **חיוב משימות**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-126">On the **Project** page, select the **Task billing** tab.</span></span>
6. <span data-ttu-id="2e5f9-127">ברשת השנייה, שחלה על הגדרת חיוב ספציפי למשימה, בחר משימה אחת או יותר ואז בחר **שורות הצעות מחיר משויכות**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-127">In the second grid, which applies to task-specific billing setup, select one or more tasks and then select **Associate quote lines**.</span></span>
7. <span data-ttu-id="2e5f9-128">בדף הדו-שיח שמופיע, בחר שורת הצעת מחיר המציגה שורות הצעת מחיר מבוססות פרויקט על הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-128">In the dialog page that appears, select a quote line that displays project-based quote lines on the quote.</span></span>
8. <span data-ttu-id="2e5f9-129">בשדה **סוג החיוב**, ציין אם אלה משימות הניתנות לחיוב או משימות שאינן ניתנות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-129">In the **Billing type** field, indicate if these tasks are chargeable or non-chargeable.</span></span>
9. <span data-ttu-id="2e5f9-130">בחר בתיבת הסימון כדי לציין אם השיוך צריך לכלול את המשימות הבנות של המשימות שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-130">Select the check box to indicate if the association should include child tasks of the selected tasks.</span></span> <span data-ttu-id="2e5f9-131">סימון תיבת הסימון ישייך את המשימות הבנות של המשימות שנבחרו לשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-131">Checking the box will associate the child tasks of the selected tasks to the quote line.</span></span>
10. <span data-ttu-id="2e5f9-132">בחר **אישור** כדי לסגור את הדו-שיח.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-132">Select **OK** to close the dialog.</span></span>

### <a name="from-the-quote-line-page"></a><span data-ttu-id="2e5f9-133">מדף שורת הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="2e5f9-133">From the Quote line page</span></span>

<span data-ttu-id="2e5f9-134">ניתן לשייך משימות פרויקט לשורות הצעות מחיר מהכרטיסיה **משימות הניתנות לחיוב** בדף **שורת הצעות מחיר**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-134">You can associate project tasks to quote lines from the **Chargeable tasks** tab on **Quote line** page.</span></span>

>[!NOTE]
><span data-ttu-id="2e5f9-135">המקום האופטימלי לשיוך משימות פרויקט לשורות הצעת מחיר הוא בחרטיסיה **חיוב משימות** שבדף **פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-135">The optimal place to associate project tasks to quote lines is on the **Task billing** tab on the **Project** page.</span></span> <span data-ttu-id="2e5f9-136">אם אתה משייך משימות מהכרטיסיה **משימות הניתנות לחיוב** שבדף **שורת הצעת מחיר**, עליך לשייך ידנית כל פרויקט.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-136">If you associate tasks from the **Chargeable tasks** tab on **Quote line** page, you must manually associate each project.</span></span>

1. <span data-ttu-id="2e5f9-137">בכרטיסיה **כללי** של שורת הצעת מחיר מבוססת פרויקט, אמת שנבחרה פרויקט בשדה **פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-137">On the **General** tab of a project–based quote line, verify that there is a project selected in the **Project** field.</span></span>
2. <span data-ttu-id="2e5f9-138">בשדה **משימות כלולות**, בחר **משימות נבחרות בלבד**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-138">In the **Included tasks** field, select **Selected tasks only**.</span></span>
3. <span data-ttu-id="2e5f9-139">שמור את שורות הצעת המחיר מבוססות הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-139">Save the project-based quote line.</span></span> <span data-ttu-id="2e5f9-140">לאחר ריענון הטופס, תוצג הכרטיסיה **משימות הניתנות לחיוב**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-140">When the form refreshes, the **Chargeable tasks** tab displays.</span></span>
4. <span data-ttu-id="2e5f9-141">בכרטיסיה **משימות הניתנות לחיוב**, בחר **הוסף משימה של שורת הצעת מחיר**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-141">On the **Chargeable tasks** tab, select **Add a quote line task**.</span></span>
5. <span data-ttu-id="2e5f9-142">בדף **שורת הצעת מחיר** , בשדה **משימות**, בחר את המשימה ובשדה **סוג החיוב** בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-142">On the **Quote line task** page, in the **Tasks** field, select the task and in the **Billing type** field, select **Save**.</span></span> 
6. <span data-ttu-id="2e5f9-143">סגור את הדף.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-143">Close the page.</span></span> <span data-ttu-id="2e5f9-144">המשימה שנבחרה משויכת כעת לשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-144">The selected task is now associated to the quote line.</span></span>

## <a name="disassociate-tasks-from-projectbased-quote-lines"></a><span data-ttu-id="2e5f9-145">ביטול השיוך של משימות להצעות מחיר מבוססות פרויקט</span><span class="sxs-lookup"><span data-stu-id="2e5f9-145">Disassociate tasks from project–based quote lines</span></span>

### <a name="from-the-project-page"></a><span data-ttu-id="2e5f9-146">מדך הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="2e5f9-146">From the Project page</span></span>

<span data-ttu-id="2e5f9-147">שיטה זו מספק תאת החוויה האופטימלית ביותר עבור ביטול השיוך של משימות לשורות הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-147">This method provides the most optimal experience for disassociating tasks from quote lines.</span></span> <span data-ttu-id="2e5f9-148">אפשר לבחור משימות מרובות ולבטל את השיוך של כולן, ושל המשימות הבנות שלהן, לשורת הצעת המחיר שנבחרה.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-148">You can select multiple tasks and disassociate all of the them, plus their child tasks, from the selected quote line.</span></span>

1. <span data-ttu-id="2e5f9-149">בכרטיסיה **כללי** של שורת הצעת מחיר מבוססת פרויקט, בשדה **פרויקט** בחר את קישור הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-149">On the **General** tab of a project–based quote line, in the **Project** field, select the project link.</span></span>
2. <span data-ttu-id="2e5f9-150">בדף **פרוייקט**, בחר בכרטיסיה **חיוב משימות**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-150">On the **Project** page, select the **Task billing** tab.</span></span>
3. <span data-ttu-id="2e5f9-151">ברשת השנייה, שחלה על הגדרה של חיוב ספציפי למשימה, בחר משימה אחת או יותר ואז בחר **בטל את השיוך של שורות הצעות מחיר**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-151">In the second grid, which applies to task-specific billing setup, select one or more tasks, and then select **Disassociate quote lines**.</span></span>
4. <span data-ttu-id="2e5f9-152">בדף הדו-שיח שמוצג, בחר בשורת הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-152">In the dialog page that appears, select a quote line.</span></span>
5. <span data-ttu-id="2e5f9-153">בחר בתיבת הסימון כדי לציין אם יש להסיר את השיוך גם מהמשימות הבנות של המשימות שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-153">Select the check box to indicate whether the association should also be removed from child tasks of the selected tasks.</span></span> <span data-ttu-id="2e5f9-154">סימון תיבת הסימון יבטל גם את השיוך של המשימות הבנות של המשימות שנבחרו לשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-154">Checking the box will also disassociate the child tasks of the selected tasks to the quote line.</span></span>
6. <span data-ttu-id="2e5f9-155">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-155">Select **OK**.</span></span> <span data-ttu-id="2e5f9-156">הודעת אזהרה מודיעה לך שאם תסיר שיוך זה, רישום של נתונים בפועל שנרשמו בעבר במשימה עשוי להתבטל.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-156">A warning message informs you that if you remove this association, any actuals previously recorded on the task could be reversed.</span></span> 
7. <span data-ttu-id="2e5f9-157">בחר **אישור** כדי להמשיך ולהסיר את השיוק שבין המשימה לשורת הצעת המחיר מבוססת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-157">Select **OK** to continue and remove the association between the task and the project-based quote line.</span></span>

### <a name="from-the-quote-line-page"></a><span data-ttu-id="2e5f9-158">מדף שורת הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="2e5f9-158">From the Quote line page</span></span>

<span data-ttu-id="2e5f9-159">ניתן גם לבטל את השיוך של משימות פרויקט לשורות הצעות מחיר מהכרטיסיה **משימות הניתנות לחיוב** בדף **שורת הצעת מחיר**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-159">You can also disassociate project tasks to quote lines from the **Chargeable tasks** tab on **Quote line** page.</span></span>

1. <span data-ttu-id="2e5f9-160">בכרטיסיה **משימות הניתנות לחיוב**, בחר **מחק משימה של שורת הצעת מחיר**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-160">On the **Chargeable tasks** tab, select **Delete a quote line task**.</span></span>
2. <span data-ttu-id="2e5f9-161">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-161">Select **OK**.</span></span> <span data-ttu-id="2e5f9-162">הודעת אזהרה מודיעה לך שאם תסיר שיוך זה, רישום של נתונים בפועל שנרשמו בעבר במשימה עשוי להתבטל.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-162">A warning message informs you that if you remove this association, any actuals previously recorded on the task could be reversed.</span></span> 
3. <span data-ttu-id="2e5f9-163">בחר **אישור** כדי להמשיך ולהסיר את השיוק שבין המשימה לשורת הצעת המחיר מבוססת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-163">Select **OK** to continue and remove the association between the task and the project-based quote line.</span></span>

>[!NOTE]
> <span data-ttu-id="2e5f9-164">הליך זה אינו מוחק את המשימה מהפרויקט.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-164">This procedure doesn't delete the task from the project.</span></span> <span data-ttu-id="2e5f9-165">אלא רק מסיר את שיוך המשימות משורת הצעת המחיר מבוססת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="2e5f9-165">It only removes the task association from the project-based quote line.</span></span>
