---
title: יצירת צוות פרוייקט
description: נושא זה מספק מידע לגבי האופן יצירת צוות פרויקט חדש וניהולו.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: kdwns
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 121a007d91c2da4f3b9951901781757b8bcca8fe
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5270859"
---
# <a name="create-a-project-team"></a><span data-ttu-id="20e6f-103">יצירת צוות פרויקט</span><span class="sxs-lookup"><span data-stu-id="20e6f-103">Create a project team</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="20e6f-104">כדי להשתמש בתפקידים שהוגדרו בעבר בפרויקט, על מנהל פרויקט לשייך את התפקידים לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="20e6f-104">To use the roles that were previously set up in a project, a project manager must associate the roles with the project.</span></span> <span data-ttu-id="20e6f-105">ניתן להקצות מספר תפקידים לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="20e6f-105">Multiple roles can be assigned for a project.</span></span> <span data-ttu-id="20e6f-106">כדי למנוע בלבול, התפקידים האלה מתויגים אוטומטית במהלך ההזמנה.</span><span class="sxs-lookup"><span data-stu-id="20e6f-106">To prevent confusion, these roles are automatically labeled during reservation.</span></span> <span data-ttu-id="20e6f-107">לדוגמה, אם מנהל הפרויקט דורש שלושה מהנדסי תוכנה, שלושה תפקידים של מהנדסי תוכנה שיש להם **מהנדס תוכנה 1**, **מהנדס תוכנה 2**, ו **מהנדס תוכנה 3** כתוויות שנוצרות באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="20e6f-107">For example, if the project manager requires three software engineers, three Software engineer roles that have **software engineer 1**, **software engineer 2**, and **software engineer 3** as their labels are automatically generated.</span></span> <span data-ttu-id="20e6f-108">אם בעבר הוגדרו מאפייני תפקיד עבור התפקיד, הם מיושמים כמסנן במהלך חיפושים אחר משאב.</span><span class="sxs-lookup"><span data-stu-id="20e6f-108">If role characteristics were previously set for the role, they are applied as a filter during searches for a resource.</span></span> <span data-ttu-id="20e6f-109">ניתן להוסיף מאפיינים נוספים כנדרש כדי לחדד עוד יותר את החיפוש.</span><span class="sxs-lookup"><span data-stu-id="20e6f-109">Additional characteristics can be added as required to further refine the search.</span></span>

<span data-ttu-id="20e6f-110">ניתן להתאים אישית גם את הגדרות התצוגה כדי לתת מבט טוב יותר על זמינות המשאבים.</span><span class="sxs-lookup"><span data-stu-id="20e6f-110">View settings can also be customized to give a better view of resource availability.</span></span> <span data-ttu-id="20e6f-111">ישנן אפשרויות להראות זמינות לפי שעה, יום, שבוע, חודש, רבעון ושנה.</span><span class="sxs-lookup"><span data-stu-id="20e6f-111">There are options to show hourly, daily, weekly, monthly, quarterly, and annual availability.</span></span> <span data-ttu-id="20e6f-112">יש גם אפשרות להציג יכולת זמינה ונותרת על משאבים.</span><span class="sxs-lookup"><span data-stu-id="20e6f-112">There is also an option to show available and remaining capacity on resources.</span></span> <span data-ttu-id="20e6f-113">אפשרות זו שימושית לצורך ניהול זמן כאשר אתה מעריך זמן זמין לפעילויות או לזמינות משאבים.</span><span class="sxs-lookup"><span data-stu-id="20e6f-113">This option is useful for time management, when you're estimating available time for activities or resource availability.</span></span>

<span data-ttu-id="20e6f-114">מנהל הפרויקט יכול לבחור תפקיד בדף ואז, אם יש משאב זמין המתאים לדרישה, לבחור לשריין משאב למילוי התפקיד.</span><span class="sxs-lookup"><span data-stu-id="20e6f-114">The project manager can select a role on the page and then, if there is an available resource that fits the requirement, select to reserve a resource to fill the role.</span></span> <span data-ttu-id="20e6f-115">שים לב כי בשלב זה אין צורך לשמור את המשאבים בשלב התכנון.</span><span class="sxs-lookup"><span data-stu-id="20e6f-115">Note that the resources don't have to be reserved at this point in the planning stage.</span></span> <span data-ttu-id="20e6f-116">כשאתה יוצר WBS, אתה יכול להחליף תפקידים במשאבים מאוישים עבור הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="20e6f-116">When you create a WBS, you can replace roles with staffed resources for the project.</span></span> <span data-ttu-id="20e6f-117">אם תפקידים מוחלפים במשאבים מאוישים ב- WBS, הגדרת המשאבים מעדכנת אוטומטית את רישום ותזמון צוות הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="20e6f-117">If roles are replaced with staffed resources in the WBS, the resource setup automatically updates the project team listing and scheduling.</span></span>

<span data-ttu-id="20e6f-118">[![רישום צוות הפרויקט הכולל גם תפקידים וגם משאבים בפועל](./media/projectresourcing03-1024x368.jpg)](./media/projectresourcing03.jpg)</span><span class="sxs-lookup"><span data-stu-id="20e6f-118">[![Project team listing that includes both roles and actual resources](./media/projectresourcing03-1024x368.jpg)](./media/projectresourcing03.jpg)</span></span> 

<span data-ttu-id="20e6f-119">למנהל הפרויקט אפשרויות שונות להזמנת משאב לפרויקט, כגון **יכולת שנותרה**, **תפוסה מלאה**, **אחוז קיבולת**, ו **ציון שעות**.</span><span class="sxs-lookup"><span data-stu-id="20e6f-119">The project manager has various options for booking a resource for a project, such as **Remaining capacity**, **Full capacity**, **Capacity percentage**, and **Specify hours**.</span></span> <span data-ttu-id="20e6f-120">ניתן לבטל אפשרויות הזמנה אלה בכל עת אם הקצאות המשאבים משתנות.</span><span class="sxs-lookup"><span data-stu-id="20e6f-120">These booking options can be canceled at any time if resource assignments change.</span></span> <span data-ttu-id="20e6f-121">שני סוגי הזמנות נתמכים:</span><span class="sxs-lookup"><span data-stu-id="20e6f-121">Two types of booking are supported:</span></span>

- <span data-ttu-id="20e6f-122">**הזמנה בטוחה** - הזמנת המשאב אושרה ואושר לעבוד על ההתקשרות למשך הזמן שצוין.</span><span class="sxs-lookup"><span data-stu-id="20e6f-122">**Hard Book** – The resource reservation was approved and confirmed to work on the engagement for the specified duration.</span></span>
- <span data-ttu-id="20e6f-123">**הזמנה טנטטיבית** - הזמנות המשאב הוגדרו באופן טנטטיבי לעבוד על ההתקשרות למשך הזמן שצוין.</span><span class="sxs-lookup"><span data-stu-id="20e6f-123">**Soft book** – The resource reservations was tentatively set to work on the engagement for the specified duration.</span></span>

<span data-ttu-id="20e6f-124">ההליך הבא מסביר כיצד ליצור צוות פרויקט:</span><span class="sxs-lookup"><span data-stu-id="20e6f-124">The following procedure explains how to create a project team.</span></span>

## <a name="create-a-project-team"></a><span data-ttu-id="20e6f-125">יצירת צוות פרויקט</span><span class="sxs-lookup"><span data-stu-id="20e6f-125">Create a project team</span></span>

1. <span data-ttu-id="20e6f-126">בדף הרשימה **כל הפרויקטים**, בחר פרויקט ולאחר מכן בחר **עריכה**.</span><span class="sxs-lookup"><span data-stu-id="20e6f-126">On the **All projects** list page, select a project, and then select **Edit**.</span></span>
2. <span data-ttu-id="20e6f-127">בכרטיסיה **צוות פרויקט ותזמון**, בשדה **קביעת תאריך סיום**, הזן את תאריך ההתחלה של לוח הזמנים בתוספת חודש.</span><span class="sxs-lookup"><span data-stu-id="20e6f-127">On the **Project team and scheduling** tab, in the **Schedule end date** field, enter the schedule start date plus one month.</span></span> <span data-ttu-id="20e6f-128">לדוגמה, אם תאריך התחלת לוח הזמנים הוא 24 ביוני 2017 (24/06/2017), הזן **24/07/2017**.</span><span class="sxs-lookup"><span data-stu-id="20e6f-128">For example, if the schedule start date is June 24, 2017 (24/06/2017), enter **24/07/2017**.</span></span>
3. <span data-ttu-id="20e6f-129">בחר **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="20e6f-129">Select **Add**.</span></span>
4. <span data-ttu-id="20e6f-130">בחלונית **הוסף תפקידים לפרויקט**, בשדה **תפקיד**, בחר **מנהל פרויקט בכיר**.</span><span class="sxs-lookup"><span data-stu-id="20e6f-130">In the **Add roles to the project** pane, in the **Role** field, select **Senior Project Manager**.</span></span>
5. <span data-ttu-id="20e6f-131">בחר **יכולות נדרשות**.</span><span class="sxs-lookup"><span data-stu-id="20e6f-131">Select **Required competencies**.</span></span>
6. <span data-ttu-id="20e6f-132">בדף **בחר מאפיינים**, המאפיינים שקבעת בעבר לתפקיד מנהל הפרויקט הבכיר נבחרים כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="20e6f-132">On the **Choose characteristics** page, the characteristics that you previously set for the Senior project manager role are selected by default.</span></span> <span data-ttu-id="20e6f-133">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="20e6f-133">Select **OK**.</span></span>
7. <span data-ttu-id="20e6f-134">בדף **הוסף תפקידים לפרויקט**, בשדה **מספר משאבים**, הזן **1**.</span><span class="sxs-lookup"><span data-stu-id="20e6f-134">On the **Add roles to project** page, in the **Number of resources** field, enter **1**.</span></span>
8. <span data-ttu-id="20e6f-135">בשדה **משאב**, החיפוש מציג את כל המשאבים שיש להם את היכולות הנדרשות.</span><span class="sxs-lookup"><span data-stu-id="20e6f-135">In the **Resource** field, the lookup shows all resources that have the required competencies.</span></span> <span data-ttu-id="20e6f-136">בחר **דניאל גולדשמידט** ולאחר מכן בחר **צור**.</span><span class="sxs-lookup"><span data-stu-id="20e6f-136">Select **Daniel Goldschmidt**, and then select **Create**.</span></span>
9. <span data-ttu-id="20e6f-137">בדף **פרויקט**, בחר **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="20e6f-137">On the **Project** page, select **Add**.</span></span>
10. <span data-ttu-id="20e6f-138">בחלונית **הוסף תפקידים לפרויקט**, בשדה **תפקיד**, בחר **חבר צוות**.</span><span class="sxs-lookup"><span data-stu-id="20e6f-138">In the **Add roles to the project** pane, in the **Role** field, select **Team member**.</span></span> <span data-ttu-id="20e6f-139">בשדה **מספר משאבים**, הזן **5**.</span><span class="sxs-lookup"><span data-stu-id="20e6f-139">In the **Number of resources** field, enter **5**.</span></span>
11. <span data-ttu-id="20e6f-140">בחר **Create** (צור).</span><span class="sxs-lookup"><span data-stu-id="20e6f-140">Select **Create**.</span></span>
12. <span data-ttu-id="20e6f-141">בדף **פרויקטים**, בחר **מימוש משאב**.</span><span class="sxs-lookup"><span data-stu-id="20e6f-141">On the **Projects** page, select **Fulfill resource**.</span></span>

## <a name="monitor-project-teams"></a><span data-ttu-id="20e6f-142">נטר את צוותי הפרויקט</span><span class="sxs-lookup"><span data-stu-id="20e6f-142">Monitor project teams</span></span>
1. <span data-ttu-id="20e6f-143">בדף **כל הפרויקטים**, בחר בקישור **מזהה פרויקט** עבור הפרויקט **שדרוג XYZ שלב 2**.</span><span class="sxs-lookup"><span data-stu-id="20e6f-143">On the **All projects** page, select the **Project ID** link for the **XYZ Upgrade Phase 2** project.</span></span>
2. <span data-ttu-id="20e6f-144">ב- FastTab **צוות פרויקט ותזמון**, ודא שמשאבי הפרויקט המפורטים נכונים.</span><span class="sxs-lookup"><span data-stu-id="20e6f-144">On the **Project team and scheduling** FastTab, verify that the project resources that are listed are correct.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]