---
title: הגדרת משאבים לפרויקט
description: נושא זה מספק מידע על הגדרה או בקשה של משאבי פרויקטים.
author: Yowelle
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 49e0ca6254518079d2e01d92ac2e31d119468c4b
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997692"
---
# <a name="set-up-project-resources"></a><span data-ttu-id="ebe36-103">הגדרת משאבים לפרויקט</span><span class="sxs-lookup"><span data-stu-id="ebe36-103">Set up project resources</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="ebe36-104">עליך להגדיר לוח שנה ולשייך אותו לעובד.</span><span class="sxs-lookup"><span data-stu-id="ebe36-104">You must set up a calendar and associate it with an employee or a worker.</span></span> <span data-ttu-id="ebe36-105">לוח השנה משמש לתזמון הפרויקט ולזמן העבודה של המשאבים השמורים לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ebe36-105">The calendar is used to schedule the project and the working time of the resources that are reserved for the project.</span></span> <span data-ttu-id="ebe36-106">במהלך הגדרת לוח השנה, מנהלי פרויקטים יכולים לבצע פילוס משאבים כחלק ממיטוב המשאבים.</span><span class="sxs-lookup"><span data-stu-id="ebe36-106">During calendar setup, project managers can do resource leveling as part of resource optimization.</span></span> <span data-ttu-id="ebe36-107">בהתבסס על לוח הזמנים של לוח השנה, ניתן להציב מגבלות על המשאבים.</span><span class="sxs-lookup"><span data-stu-id="ebe36-107">Based on the calendar schedule, restrictions can be put on resources.</span></span> <span data-ttu-id="ebe36-108">אתה יכול להגדיר לוח שנה בדף **לוחות שנה**.</span><span class="sxs-lookup"><span data-stu-id="ebe36-108">You can set up a calendar on the **Calendars** page.</span></span>

<span data-ttu-id="ebe36-109">כאשר אתה מגדיר עובד כמשאב פרויקט, אתה יכול לבחור בין עובדים שעובדים בחברה שאתה מגדיר עבורה משאבים.</span><span class="sxs-lookup"><span data-stu-id="ebe36-109">When you set up a worker as a project resource, you can select from workers who work in the company that you're setting up resources for.</span></span> <span data-ttu-id="ebe36-110">לחלופין, תוכל לבחור עובדים מחברות אחרות בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="ebe36-110">Alternatively, you can select workers from other companies in your organization.</span></span> <span data-ttu-id="ebe36-111">עובדים אלה ידועים כמשאבים בין-חברות.</span><span class="sxs-lookup"><span data-stu-id="ebe36-111">These workers are known as intercompany resources.</span></span>

<span data-ttu-id="ebe36-112">הנהלים הבאים מסבירים כיצד להגדיר עובד כמשאב פרויקט בחברה שלך וכיצד להקים משאב פרויקט בין-חברות.</span><span class="sxs-lookup"><span data-stu-id="ebe36-112">The following procedures explain how to set up a worker as a project resource in your company and how to set up an intercompany project resource.</span></span>

## <a name="set-up-a-worker-as-a-project-resource"></a><span data-ttu-id="ebe36-113">הגדר עובד כמשאב פרויקט</span><span class="sxs-lookup"><span data-stu-id="ebe36-113">Set up a worker as a project resource</span></span>

1. <span data-ttu-id="ebe36-114">בדף **עובדים**, ברשימה **עובדים**, בחר את העובד שאתה מוסיף כמשאב פרויקט ופתח את רשומת העובד.</span><span class="sxs-lookup"><span data-stu-id="ebe36-114">On the **Workers** page, in the **Workers** list, select the worker that you're adding as a project resource, and open the worker record.</span></span>
2. <span data-ttu-id="ebe36-115">בחלונית הפעולה בחר **פרויקט** &gt; **הגדרה** &gt; **הגדרת הפרויקט**.</span><span class="sxs-lookup"><span data-stu-id="ebe36-115">On the Action Pane, select **Project** &gt; **Setup** &gt; **Project setup**.</span></span>
3. <span data-ttu-id="ebe36-116">בחר לוח שנה ואז סגור את הדף.</span><span class="sxs-lookup"><span data-stu-id="ebe36-116">Select a calendar, and then close the page.</span></span>

<span data-ttu-id="ebe36-117">ניתן גם לציין פרויקטים של ברירת מחדל עבור משאב כסוג של הקצאה מראש.</span><span class="sxs-lookup"><span data-stu-id="ebe36-117">You can also specify default projects for a resource as a type of pre-assignment.</span></span> <span data-ttu-id="ebe36-118">ניתן להשתמש במטלות מקדימות כאשר מנהל המשאבים או מנהל הפרויקט יודעים על אילו פרויקטים יעבוד המשאב מראש.</span><span class="sxs-lookup"><span data-stu-id="ebe36-118">Pre-assignments can be used when the resource manager or project manager knows which projects the resource will be working on in advance.</span></span> <span data-ttu-id="ebe36-119">משימות מקדימות יכולות להתבסס גם על בקשת נותן חסות או לקוח.</span><span class="sxs-lookup"><span data-stu-id="ebe36-119">Pre-assignments can also be based on the request of a project sponsor or customer.</span></span> <span data-ttu-id="ebe36-120">כדי להקצות מראש פרויקט, בחר את הפרויקט המתאים בדף **הקצאת פרויקטים**, בכרטיסיה **פרויקטים**, ברשימה **פרויקטים שנותרו**.</span><span class="sxs-lookup"><span data-stu-id="ebe36-120">To pre-assign a project, on the **Assign projects** page, on the **Projects** tab, in the **Remaining projects** list, select the appropriate project.</span></span>

## <a name="set-up-an-intercompany-resource"></a><span data-ttu-id="ebe36-121">הגדר משאב בין חברות</span><span class="sxs-lookup"><span data-stu-id="ebe36-121">Set up an intercompany resource</span></span>

<span data-ttu-id="ebe36-122">כאשר אתה מגדיר עובד כמשאב בין חברות, עליך להשלים את ההגדרה הן בחברה המלווה והן בחברה הלווה.</span><span class="sxs-lookup"><span data-stu-id="ebe36-122">When you set up a worker as an intercompany resource, you must complete the setup in both the lending company and the borrowing company.</span></span>

### <a name="in-the-lending-company"></a><span data-ttu-id="ebe36-123">בחברה המלווה</span><span class="sxs-lookup"><span data-stu-id="ebe36-123">In the lending company</span></span>

1. <span data-ttu-id="ebe36-124">בכספים, ודא כי החברה המלווה נבחרה, ולאחר מכן השלם את ההליך במקטע הקודם, "הגדר עובד כמשאב פרויקט."</span><span class="sxs-lookup"><span data-stu-id="ebe36-124">In Finance, verify that the lending company is selected, and then complete the procedure in the previous section, "Set up a worker as a project resource."</span></span>
2. <span data-ttu-id="ebe36-125">בדף **חשבונאות בין חברות**, בחר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="ebe36-125">On the **Intercompany accounting** page, select **New**.</span></span>
3. <span data-ttu-id="ebe36-126">בשדה **מזהה ישות משפטית** בחר את החברה המלווה.</span><span class="sxs-lookup"><span data-stu-id="ebe36-126">In the **Legal entity ID** field, select the lending company.</span></span> <span data-ttu-id="ebe36-127">מלא את השדות הנותרים כנדרש ולאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="ebe36-127">Fill in the remaining fields as appropriate, and then select **Save**.</span></span>
4. <span data-ttu-id="ebe36-128">בדף **מחיר העברה**, בחר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="ebe36-128">On the **Transfer price** page, select **New**.</span></span>
5. <span data-ttu-id="ebe36-129">בשדה **ישות משפטית לווה** בחר את החברה המתאימה.</span><span class="sxs-lookup"><span data-stu-id="ebe36-129">In the **Borrowing legal entity** field, select the appropriate company.</span></span>
6. <span data-ttu-id="ebe36-130">ניתן להלוות לחברה הלווה רק את המשאב שיצרת בתחילת מקטע זה, בשדה **משאב**, בחר את שם המשאב שיצרת.</span><span class="sxs-lookup"><span data-stu-id="ebe36-130">To lend the borrowing company only the resource that you created at the beginning of this section, in the **Resource** field, select the name of the resource that you created.</span></span> <span data-ttu-id="ebe36-131">כדי להעמיד לרשות החברה הלווה את כל המשאבים של חברה המלווה, השאר את השדה **משאב** ריק.</span><span class="sxs-lookup"><span data-stu-id="ebe36-131">To make all resources in the lending company available to the borrowing company, leave the **Resource** field blank.</span></span>
7. <span data-ttu-id="ebe36-132">בדף **ניהול פרויקטים ופרמטרים חשבונאיים**, בכרטיסיה **בין חברות**, הגדר את האפשרות **אפשר תזמון משאבים בין-חברות וגליונות זמנים** כ **כן**.</span><span class="sxs-lookup"><span data-stu-id="ebe36-132">On the **Project management and accounting parameters** page, on the **Intercompany** tab, set the **Enable intercompany resource scheduling and timesheets** option to **Yes**.</span></span>

### <a name="in-the-borrowing-company"></a><span data-ttu-id="ebe36-133">בחברה הלווה</span><span class="sxs-lookup"><span data-stu-id="ebe36-133">In the borrowing company</span></span>

- <span data-ttu-id="ebe36-134">בדף **רשימת משאבים**, במסנן החיפוש, הזן את שם המשאב שיצרת עבור החברה המלווה, כדי לוודא שהשם נכלל ברשימת המשאבים של החברה הלווה.</span><span class="sxs-lookup"><span data-stu-id="ebe36-134">On the **Resources list** page, in the search filter, enter the name of the resource that you created for the lending company, to verify that the name is included in the resource list for the borrowing company.</span></span>

## <a name="request-project-resources"></a><span data-ttu-id="ebe36-135">בקשה של משאבי פרויקט</span><span class="sxs-lookup"><span data-stu-id="ebe36-135">Request project resources</span></span>
<span data-ttu-id="ebe36-136">הפונקציונליות לתזמון משאבי הפרויקט מאפשרת למנהלי משאבים להפיץ משאבים מאוישים בהתקשרויות או בפרויקטים.</span><span class="sxs-lookup"><span data-stu-id="ebe36-136">The functionality for project resource scheduling only lets resource managers distribute staffed resources on engagements or projects.</span></span> <span data-ttu-id="ebe36-137">כדי לאפשר פונקציונליות זו, השלם את המשימות הבאות, או ודא שהן הושלמו:</span><span class="sxs-lookup"><span data-stu-id="ebe36-137">To enable this functionality, complete the following tasks, or verify that they have been completed:</span></span>

- <span data-ttu-id="ebe36-138">הגדר רצפי מספרים.</span><span class="sxs-lookup"><span data-stu-id="ebe36-138">Set up number sequences.</span></span>
- <span data-ttu-id="ebe36-139">הגדר תהליכי עבודה של ניהול פרויקטים וחשבונאות.</span><span class="sxs-lookup"><span data-stu-id="ebe36-139">Set up project management and accounting workflows.</span></span>
- <span data-ttu-id="ebe36-140">אפשר זרימות עבודה של בקשת משאבים.</span><span class="sxs-lookup"><span data-stu-id="ebe36-140">Enable resource request workflows.</span></span>

<span data-ttu-id="ebe36-141">לאחר השלמת המשימות הקודמות, תוכל לבצע את המשימות הבאות כנדרש:</span><span class="sxs-lookup"><span data-stu-id="ebe36-141">After the preceding tasks have been completed, you can complete the following tasks as you require:</span></span>

- <span data-ttu-id="ebe36-142">צור בקשת משאבים ממשאב מאויש שהוזמן בהזמנה טנטטיבית.</span><span class="sxs-lookup"><span data-stu-id="ebe36-142">Create a resource request from a soft-booked staffed resource.</span></span>
- <span data-ttu-id="ebe36-143">ניטור בקשות למשאבים.</span><span class="sxs-lookup"><span data-stu-id="ebe36-143">Monitor resource requests.</span></span>
- <span data-ttu-id="ebe36-144">מימוש בקשות למשאבים.</span><span class="sxs-lookup"><span data-stu-id="ebe36-144">Fulfill resource requests.</span></span>
- <span data-ttu-id="ebe36-145">בקש משאב מאויש מ- WBS.</span><span class="sxs-lookup"><span data-stu-id="ebe36-145">Request a staffed resource from a WBS.</span></span>
- <span data-ttu-id="ebe36-146">הזמן משאבים לפרויקט ללא בקשה למשאב מאויש.</span><span class="sxs-lookup"><span data-stu-id="ebe36-146">Book resources to a project without having a request for a staffed resource.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]