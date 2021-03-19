---
title: יצירת פרויקט חדש
description: נושא זה מספק מידע לגבי האופן יצירת פרויקט חדש.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 9b29340dc88aea888ea2f5ea975eaea59d014279
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5270724"
---
# <a name="create-a-new-project"></a><span data-ttu-id="bf4f1-103">יצירת פרויקט חדש</span><span class="sxs-lookup"><span data-stu-id="bf4f1-103">Create a new project</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="bf4f1-104">השלם את השלבים הבאים ליצירת פרויקט חדש.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-104">Complete the following steps to create a new project.</span></span>

1. <span data-ttu-id="bf4f1-105">בדף **ניהול פרויקט**, בחר **פרויקט חדש** והזן את הערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="bf4f1-105">On the **Project management** page, select **New project**, and enter the following values:</span></span>

    - <span data-ttu-id="bf4f1-106">**סוג הפרויקט:** זמן וחומר</span><span class="sxs-lookup"><span data-stu-id="bf4f1-106">**Project type:** Time and material</span></span>
    - <span data-ttu-id="bf4f1-107">**שם הפרויקט:** שלב 2 לשדרוג XYZ</span><span class="sxs-lookup"><span data-stu-id="bf4f1-107">**Project name:** XYZ Upgrade Phase 2</span></span>
    - <span data-ttu-id="bf4f1-108">**קבוצת פרויקטים:** TM\_WIP</span><span class="sxs-lookup"><span data-stu-id="bf4f1-108">**Project group:** TM\_WIP</span></span>
    - <span data-ttu-id="bf4f1-109">**מזהה חוזה פרויקט:** 00000002</span><span class="sxs-lookup"><span data-stu-id="bf4f1-109">**Project contract ID:** 00000002</span></span>

2. <span data-ttu-id="bf4f1-110">בחר **יצירת פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-110">Select **Create project**.</span></span>

## <a name="assign-a-resource-to-a-project"></a><span data-ttu-id="bf4f1-111">הקצאת משאב לפרויקט</span><span class="sxs-lookup"><span data-stu-id="bf4f1-111">Assign a resource to a project</span></span>

1. <span data-ttu-id="bf4f1-112">בדף **עובדים**, ברשימה **עובדים**, בחר את העובד שהגדרת עבורו יכולות קודם לכן ופתח את רשומת העובד.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-112">On the **Workers** page, in the **Workers** list, select the record for the worker that you previously set up competencies for, and open the worker record.</span></span>
2. <span data-ttu-id="bf4f1-113">בחלונית הפעולות, בכרטיסיה **פרויקט**, בקבוצה **הגדרה**, בחר **הקצה פרויקטים**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-113">On the Action Pane, on the **Project** tab, in the **Setup** group, select **Assign projects**.</span></span>
3. <span data-ttu-id="bf4f1-114">בדף **הקצאות פרויקט לאימות משאבים**, בכרטיסיה **פרויקטים**, בשדה **הוסף את הפרויקט לפרויקטים שנבחרו**, סנן בפרויקט **שלב 2 של שדרוג XYZ**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-114">On the **Resource validation project assignments** page, on the **Projects** tab, in the **Add the project to selected projects** field, filter on the **XYZ Upgrade Phase 2** project.</span></span>
4. <span data-ttu-id="bf4f1-115">בחלונית **פרויקטים שנותרו**, בחר פרויקט ולאחר מכן בחר בלחצן החץ כדי להוסיף אותו לחלונית **פרויקטים שנבחרו**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-115">In the **Remaining projects** pane, select a project, and then select the arrow button to add it to the **Selected projects** pane.</span></span>

<span data-ttu-id="bf4f1-116">תוכל גם להקצות קטגוריות עבור משאב לפי דרישתך.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-116">You can also assign categories for a resource as you require.</span></span> <span data-ttu-id="bf4f1-117">סוג הקטגוריה הוא או **עלות** או **הכנסה**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-117">The category type is either **Cost** or **Revenue**.</span></span> <span data-ttu-id="bf4f1-118">סוג הקטגוריה נקבע על ידי הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-118">The category type is determined by your organization.</span></span> <span data-ttu-id="bf4f1-119">אם לא מוקצות קטגוריות עבור משאב, Finance מחפש את קטגוריית ברירת המחדל במחירי שעות עבור עלות והכנסות.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-119">If no categories are assigned for a resource, Finance looks up the default category on hour prices for cost and revenue.</span></span>

## <a name="set-up-project-resource-and-role-characteristics"></a><span data-ttu-id="bf4f1-120">הגדר מאפייני משאב ותפקידים לפרויקט</span><span class="sxs-lookup"><span data-stu-id="bf4f1-120">Set up project resource and role characteristics</span></span>

<span data-ttu-id="bf4f1-121">מנהל פרויקט יכול להשתמש בפונקציונליות משאבי הפרויקט כדי ליצור את התפקידים הנדרשים לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-121">A project manager can use the project resourcing functionality to create the roles that are required for the project.</span></span> <span data-ttu-id="bf4f1-122">ניתן להשתמש בתפקידים אם משאבים מאושרים עדיין אינם ידועים בעת שמירת משאבים.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-122">Roles can be used if confirmed resources are still unknown when resources are being reserved.</span></span> <span data-ttu-id="bf4f1-123">ניתן לשמור זמנית תפקידים כמשאבים מתוכננים, כך שתוכלו להמשיך בשלבי תכנון הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-123">Roles can be temporarily reserved as planned resources, so that you can continue the project planning stages.</span></span>

<span data-ttu-id="bf4f1-124">[![דוגמה לתפקיד](./media/projectresourcing05.jpg)](./media/projectresourcing05.jpg)</span><span class="sxs-lookup"><span data-stu-id="bf4f1-124">[![Example of a role](./media/projectresourcing05.jpg)](./media/projectresourcing05.jpg)</span></span> 

<span data-ttu-id="bf4f1-125">**תרחיש:** בר-אילן נשכר להשלמת פרויקט זמן וחומר שיש בו אמנת פרויקט שאושרה.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-125">**Scenario:** Contoso was hired to complete a Time and material project that has an approved project charter.</span></span> <span data-ttu-id="bf4f1-126">מנהל הפרויקט הזוטר עדיין משלים את היקף הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-126">The junior project manager is still completing the scope of the project.</span></span> <span data-ttu-id="bf4f1-127">מנהל המשאבים מזהה כרגע משאבים ספציפיים שיישמרו לעבודה על הפרויקט החדש.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-127">The resource manager is currently identifying specific resources that will be reserved to work on the new project.</span></span> <span data-ttu-id="bf4f1-128">בגלל האופי הקריטי של הפרויקט, ביקש נותן החסות את מנהל הפרויקט הבכיר כאחד התפקידים.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-128">Because of the critical nature of the project, the project sponsor requested Senior project manager as one of the roles.</span></span> <span data-ttu-id="bf4f1-129">על מנהל המשאבים לרכוש את המשאב החדש ולהגדיר את התפקיד במערכת במקרה שמנהל הפרויקט הזוטר זקוק למידע על המשאבים במהלך תכנון הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-129">The resource manager must acquire the new resource and define the role in the system in case the junior project manager requires the resource information during project planning.</span></span>

<span data-ttu-id="bf4f1-130">השלבים הבאים מראים כיצד מנהל המשאבים יכול להגדיר את תפקיד מנהל הפרויקט הבכיר ולשייך אליו מאפייני משאבים.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-130">The following steps show how the resource manager can set up the Senior project manager role and associate resource characteristics with it.</span></span> <span data-ttu-id="bf4f1-131">בהמשך ניתן להשתמש בתפקיד לחיפוש משאבים זמינים התואמים את יכולות המשאבים הנדרשות.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-131">Later, the role can be used to search for available resources that match the required resource competencies.</span></span>

1. <span data-ttu-id="bf4f1-132">בדף **הגדרת תפקידים**, בחר **חדש** והזן את הערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="bf4f1-132">On the **Setup roles** page, select **New**, and enter the following values:</span></span>

    - <span data-ttu-id="bf4f1-133">**מזהה תפקיד:** מנהל פרויקט בכיר</span><span class="sxs-lookup"><span data-stu-id="bf4f1-133">**Role ID:** Senior Project Manager</span></span>
    - <span data-ttu-id="bf4f1-134">**תיאור:** מנהל פרויקט בכיר</span><span class="sxs-lookup"><span data-stu-id="bf4f1-134">**Description:** Senior Project Manager</span></span>

2. <span data-ttu-id="bf4f1-135">בחר **Create** (צור).</span><span class="sxs-lookup"><span data-stu-id="bf4f1-135">Select **Create**.</span></span>
3. <span data-ttu-id="bf4f1-136">בחר את התפקיד **מנהל פרויקט בכיר** ולאחר מכן בחר **הגדר מאפיינים**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-136">Select the **Senior Project Manager** role, and then select **Configure characteristics**.</span></span>
4. <span data-ttu-id="bf4f1-137">בשדה **סוג מאפיינים**, בחר **כישור**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-137">In the **Characteristics type** field, select **Skill**.</span></span>
5. <span data-ttu-id="bf4f1-138">בשדה **מאפיינים זמינים**, הזן את הכישור לחיפוש.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-138">In the **Available characteristics** field, enter the skill to search for.</span></span>
6. <span data-ttu-id="bf4f1-139">בשדה **סוג מאפיין**, בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-139">In the **Characteristic type** field, select **Certificate**.</span></span>
7. <span data-ttu-id="bf4f1-140">בשדה **מאפיינים זמינים**, הזן את סוג האישור לחיפוש.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-140">In the **Available characteristics** field, enter the certificate type to search for.</span></span>

## <a name="assign-a-project-resource-to-a-project"></a><span data-ttu-id="bf4f1-141">הקצאת משאב פרויקט לפרויקט</span><span class="sxs-lookup"><span data-stu-id="bf4f1-141">Assign a project resource to a project</span></span>

1. <span data-ttu-id="bf4f1-142">בדף **כל הפרויקטים** בחר בפרויקט **שלב 2 לשדרוג XYZ**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-142">On the **All projects** page, select the **XYZ Upgrade Phase 2** project.</span></span>
2. <span data-ttu-id="bf4f1-143">בכרטיסיה **צוות פרויקט ולוח זמנים** בחר **הוספה**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-143">On the **Project team and scheduling** tab, select **Add**.</span></span>
3. <span data-ttu-id="bf4f1-144">בשדה **תפקיד**, בחר **חבר צוות**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-144">In the **Role** field, select **Team member**.</span></span>
4. <span data-ttu-id="bf4f1-145">בחר **הזמנה מלוח השנה**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-145">Select **Book from calendar**.</span></span>
5. <span data-ttu-id="bf4f1-146">בדף **זמינות משאבים**, בחר **הצגת הגדרות**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-146">On the **Resource availability** page, select **View settings**.</span></span>
6. <span data-ttu-id="bf4f1-147">בדף **התאמת הגדרות תצוגה**, הזן את הערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="bf4f1-147">On the **Adjust view settings** page, enter the following values:</span></span>

    - <span data-ttu-id="bf4f1-148">**פורמט לתצוגת טווח תאריכים:** יום</span><span class="sxs-lookup"><span data-stu-id="bf4f1-148">**Format for date range view:** Day</span></span>
    - <span data-ttu-id="bf4f1-149">**הצגת תיאורי זמינות:** כן</span><span class="sxs-lookup"><span data-stu-id="bf4f1-149">**Display availability descriptions:** Yes</span></span>
    - <span data-ttu-id="bf4f1-150">**הצגת קיבולת שנותרה:** כן</span><span class="sxs-lookup"><span data-stu-id="bf4f1-150">**Display remaining capacity:** Yes</span></span>

7. <span data-ttu-id="bf4f1-151">בחר משאב מרשימת המשאבים.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-151">In the list of resources, select a resource.</span></span>
8. <span data-ttu-id="bf4f1-152">בחר **הזמנה בטוחה** ו **תפוסה מלאה**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-152">Select **Hard book** and **Full capacity**.</span></span>

## <a name="assign-a-resource-to-a-default-role"></a><span data-ttu-id="bf4f1-153">הקצאת משאב לתפקיד ברירת מחדל</span><span class="sxs-lookup"><span data-stu-id="bf4f1-153">Assign a resource to a default role</span></span>

<span data-ttu-id="bf4f1-154">כדי לעזור, מנהלי פרויקטים או משאבים יכולים להסתעף לעוד משאבים שניתן להזמין לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-154">To help project or resource managers can drill down further on the resources that can be reserved for a project.</span></span> <span data-ttu-id="bf4f1-155">באפשרותך לשייך תפקיד ברירת מחדל למשאב קיים או למשאב שנרכש לאחרונה.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-155">You can associate a default role with an existing resource or a newly acquired resource.</span></span> <span data-ttu-id="bf4f1-156">לדוגמה, כשדניאל התקבל לעבודה, היו לו את הניסיון והכישורים למלא את תפקיד האנליסט העסקי.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-156">For example, when Daniel was hired, he had the experience and skills to fill the Business analyst role.</span></span> <span data-ttu-id="bf4f1-157">מנהל המשאבים הקצה תפקיד זה כתפקיד ברירת המחדל של דניאל.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-157">The resource manager assigned this role as Daniel's default role.</span></span> <span data-ttu-id="bf4f1-158">לכן, מנהל המשאבים הוסיף את דניאל למאגר של אנליסטים עסקיים שזמינים לעבודה בפרויקטים.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-158">Therefore, the resource manager added Daniel to a pool of business analysts who are available to work on projects.</span></span>

<span data-ttu-id="bf4f1-159">במהלך הזמנת משאבים, מנהלי פרויקטים יכולים לסנן את משאבי התפקיד הזמינים לעבודה על פרויקטים.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-159">During resource reservation, project managers can filter the role resources that are available to work on projects.</span></span> <span data-ttu-id="bf4f1-160">הם יכולים להשתמש במידע זה כקריטריון אחד כאשר הם מבצעים ניתוח החלטות רב קריטריונים במהלך מימוש המשאבים.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-160">They can use this information as one criterion when they perform multi-criteria decision analysis during resource fulfillment.</span></span> <span data-ttu-id="bf4f1-161">הם יכולים גם להוסיף מאפייני משאבים אחרים למסנן כדי לחפש משאבים בעלי כישורים, השכלה וניסיון ספציפיים עבור פרויקט נתון.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-161">They can also add other resource characteristics to the filter to search for resources that have specific skills, education, and experience for a given project.</span></span>

<span data-ttu-id="bf4f1-162">**תרחיש:** פרויקט מאושר החל, ותפקיד מנהל הפרויקט הבכיר נשמר כמשאב מתוכנן בשלב תכנון הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-162">**Scenario:** An approved project has started, and the Senior project manager role was reserved as a planned resource during the project planning stage.</span></span> <span data-ttu-id="bf4f1-163">מנהל המשאבים רכש כעת משאב למילוי תפקיד מנהל הפרויקט הבכיר.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-163">The resource manager has now acquired a resource to fulfill the Senior project manager role.</span></span>

1. <span data-ttu-id="bf4f1-164">בדף **רשימת משאבים**, בחר **דניאל גולדשמידט**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-164">On the **Resources list** page, select **Daniel Goldschmidt**.</span></span>
2. <span data-ttu-id="bf4f1-165">בדף **תפקיד משאב**, בחר **חדש** והזן את הערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="bf4f1-165">On the **Resource role** page, select **New**, and enter the following values:</span></span>

    - <span data-ttu-id="bf4f1-166">**יעיל:** הזן את התאריך הנוכחי.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-166">**Effective:** Enter the current date.</span></span>
    - <span data-ttu-id="bf4f1-167">**תפוגה:** הזן **לעולם לא**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-167">**Expiration:** Enter **Never**.</span></span>
    - <span data-ttu-id="bf4f1-168">**תפקיד:** הזן **מנהל פרויקט בכיר**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-168">**Role:** Enter **Senior Project Manager**.</span></span>

3. <span data-ttu-id="bf4f1-169">בחר **שמור**, ולאחר מכן סגור את הדף.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-169">Select **Save**, and then close the page.</span></span>
4. <span data-ttu-id="bf4f1-170">בכרטיסיה **יכולות**, הוסף את הכישור **ProjectMgmt** ואת האישור **PMP**.</span><span class="sxs-lookup"><span data-stu-id="bf4f1-170">On the **Competencies** tab, add the **ProjectMgmt** skill and the **PMP** certificate.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]