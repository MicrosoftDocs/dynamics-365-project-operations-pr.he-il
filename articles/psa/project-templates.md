---
title: תבניות פרויקט
description: נושא זה מספק מידע על אופן השימוש בתבניות פרויקטים להגדרת פרויקט מהירה.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: db42c9ea7280274cdc9cc90f1487f27e08f892e5
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148059"
---
# <a name="project-templates"></a><span data-ttu-id="a5c9f-103">תבניות פרויקט</span><span class="sxs-lookup"><span data-stu-id="a5c9f-103">Project templates</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a5c9f-104">תבנית פרויקט היא מסגרת מוגדרת מראש שעוזרת לך להתחיל פרויקט במהירות ובקלות.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-104">A project template is a predefined framework that helps you quickly and easily start a project.</span></span> <span data-ttu-id="a5c9f-105">באפשרותך להשתמש בתבנית מוגדרת מראש כדי ליצור פרויקט חדש בלחיצה אחת.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-105">You can use a predefined template to create a new project with a single click.</span></span> <span data-ttu-id="a5c9f-106">באשר לפרויקטים, עליך להגדיר את הדרישות המוקדמות עבור תבניות פרויקט.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-106">As for projects, you must define the prerequisites for project templates.</span></span> <span data-ttu-id="a5c9f-107">עליך להגדיר את לוח השנה של הפרויקט עבור כל תבנית פרויקט ויש להגדיר מראש את התפקידים ואת המחירונים בארגון כדי שלרכיבי התבנית יהיו נתונים שימושיים.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-107">You must define a project calendar for each project template, and roles and price lists must be predefined in the organization, so that the components of the template have useful data.</span></span>

<span data-ttu-id="a5c9f-108">תבנית פרויקט מורכבת משלושה רכיבים: לוח זמנים, הערכות פרויקט וחברי צוות פרויקט.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-108">A project template consists of three components: a schedule, project estimates, and project team members.</span></span>

## <a name="schedule"></a><span data-ttu-id="a5c9f-109">תזמן</span><span class="sxs-lookup"><span data-stu-id="a5c9f-109">Schedule</span></span>

<span data-ttu-id="a5c9f-110">ללוח זמנים בתבנית פרויקט יש את אותה קבוצת רכיבים כמו לוח זמנים בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-110">A schedule in a project template has the same set of elements as a schedule in a project.</span></span> <span data-ttu-id="a5c9f-111">באפשרותך ליצור הירארכיית משימות, לשייך תפקידים למשימות, להגדיר תכונות של לוח זמנים ולהגדיר יחסי תלות.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-111">You can create a task hierarchy, associate roles with tasks, define schedule attributes, and set dependencies.</span></span> <span data-ttu-id="a5c9f-112">לוח זמנים בתבנית פרויקט תומך גם במצבי משימות עבור כל משימה.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-112">A schedule in a project template also supports task modes for each task.</span></span> <span data-ttu-id="a5c9f-113">לכן, הוא תומך במנוע התזמון.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-113">Therefore, it supports the scheduling engine.</span></span> <span data-ttu-id="a5c9f-114">עליך לשייך לוח שנה של פרויקט לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-114">You must associate a project calendar with the project.</span></span> <span data-ttu-id="a5c9f-115">בעת יצירת לוח זמנים לעבודה, אין כל הבדל בין תבנית פרויקט ופרויקט.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-115">When you create a work schedule, there is no difference between a project template and a project.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="a5c9f-116">הערכות פרויקט</span><span class="sxs-lookup"><span data-stu-id="a5c9f-116">Project estimates</span></span>

<span data-ttu-id="a5c9f-117">הערכות פרויקט בתבנית פרויקט פועלות באותו אופן כמו הערכות פרויקט בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-117">Project estimates in a project template work the same way as project estimates in a project.</span></span> <span data-ttu-id="a5c9f-118">עם זאת, מחירי העלות והמכירה שנשלפים מהמחירונים בברירת מחדל של עלות ומכירות מוגדרים בפרמטרים.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-118">However, the cost and sales prices are pulled from the default cost and sales price lists that are defined in the parameters.</span></span>

## <a name="creating-a-project-from-a-template"></a><span data-ttu-id="a5c9f-119">יצירת פרויקט מתבנית</span><span class="sxs-lookup"><span data-stu-id="a5c9f-119">Creating a project from a template</span></span>
 
<span data-ttu-id="a5c9f-120">קיימות כמה דרכים ליצירת פרויקט מתבנית פרויקט:</span><span class="sxs-lookup"><span data-stu-id="a5c9f-120">There are several ways to create a project from a project template:</span></span>

- <span data-ttu-id="a5c9f-121">בעת יצירת פרויקט מהצעת המחיר, באפשרותך לבחור תבנית פרויקט בתיבת הדן-שיח **יצירה מהירה: פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-121">When you create a project from a quote, you can select a project template in the **Quick Create: Project** dialog box.</span></span>

> ![תיבת הדו-שיח 'יצירה מהירה: פרויקט'](media/project-11.png)

- <span data-ttu-id="a5c9f-123">בעת יצירת פרויקט על-ידי בחירה באפשרות **פרויקט חדש**, הדף **פרויקט** מופיעה לפני שהרשומה נשמרת.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-123">When you create a project by selecting **New Project**, the **Project** page appears before the record is saved.</span></span> <span data-ttu-id="a5c9f-124">בשדה **בחר תבנית**, בחר תבנית אחת מתוך תבניות הפרויקט שהוגדרו מראש בארגון.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-124">In the **Pick a Template** field, select one of the predefined project templates in the organization.</span></span>
- <span data-ttu-id="a5c9f-125">השתמש באפשרות **צור פרויקט מתבנית** שבדף **ישות תבנית**.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-125">Use **Create Project from a Template** on the **Template Entity** page.</span></span>

## <a name="copying-components-of-template-to-project"></a><span data-ttu-id="a5c9f-126">העתקת רכיבי תבנית לפרויקט</span><span class="sxs-lookup"><span data-stu-id="a5c9f-126">Copying components of template to project</span></span>

<span data-ttu-id="a5c9f-127">בעת העתקת הרכיבים של תבנית פרויקט לפרויקט, כמה עקיפות עשויות להתרחש, בהתאם להגדרות בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-127">When you copy the components of a project template to a project, a few overrides can occur, depending on the settings in the project.</span></span>

### <a name="copying-the-schedule"></a><span data-ttu-id="a5c9f-128">העתקת לוח הזמנים</span><span class="sxs-lookup"><span data-stu-id="a5c9f-128">Copying the schedule</span></span>

<span data-ttu-id="a5c9f-129">בעת העתקת לוח הזמנים מתבנית פרויקט, אם לפרויקט יש לוח שנה שונה מהתבנית, שעות העבודה מלוח השנה של הפרויקט מוחלות על לוח הזמנים של המשימה.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-129">When you copy the schedule from a project template, if the project has a different project calendar than the template, work hours from the project's calendar are applied to the task schedule.</span></span> <span data-ttu-id="a5c9f-130">כך ניתן להתאים את לוח הזמנים ללוח השנה של הפרויקט המהווה גיבוי.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-130">In this way, the schedule is adjusted to match the backing project calendar.</span></span> <span data-ttu-id="a5c9f-131">באופן דומה, המשימה הראשונה בלוח הזמנים מקבלת את תאריך ההתחלה של הפרויקט ולוח הזמנים של שאר ההירארכיה מתעדכן בהתאם למשך הזמן וליחסי התלות שצוינו בתבנית.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-131">Similarly, the first task on the schedule takes the project's start date, and the schedule of the rest of the hierarchy is updated based on the duration and dependencies that are specified in the template.</span></span> 

### <a name="copying-project-estimates"></a><span data-ttu-id="a5c9f-132">העתקת הערכות פרויקט</span><span class="sxs-lookup"><span data-stu-id="a5c9f-132">Copying project estimates</span></span> 

<span data-ttu-id="a5c9f-133">בעת העתקה בין שורות הערכת פרויקט, המחירונים מתעדכנים.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-133">When you copy across project estimate lines, the price lists are updated.</span></span> <span data-ttu-id="a5c9f-134">עבור מחירון העלות, עדכונים אלה מבוססים על יחידת הבעלות של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-134">For the cost price list, these updates are based on the owning unit of the project.</span></span> <span data-ttu-id="a5c9f-135">עבור מחירון המכירות, הם מבוססים על הלקוח.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-135">For the sales price list, they are based on the customer.</span></span> <span data-ttu-id="a5c9f-136">בפרויקטים שמשויכים לישות מכירות, עלות יחידה ומחירי מכירה נקבעים בהתאם למחירונים אלה.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-136">For projects that are associated with a sales entity, the unit cost and sales prices are determined based on these price lists.</span></span>

### <a name="copying-a-project-team"></a><span data-ttu-id="a5c9f-137">העתקת צוות פרויקט</span><span class="sxs-lookup"><span data-stu-id="a5c9f-137">Copying a project team</span></span>

<span data-ttu-id="a5c9f-138">בעת העתקה של צוות פרויקט מתבנית פרויקט, המשאבים הכלליים מועתקים יחד עם הכישורים והמומחיות שהוגדרו בתבנית.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-138">When a project team is copied from a project template to a project, the generic resources are copied, together with the skills and proficiencies that are defined in the template.</span></span> <span data-ttu-id="a5c9f-139">גם אופן הטיפול בהקצאות המשאבים הכלליים זהה לזה שבתבנית הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-139">Generic resource assignments are also maintained as they were in the project template.</span></span> <span data-ttu-id="a5c9f-140">משאבים בעלי שם אינם נתמכים בתבניות פרויקט.</span><span class="sxs-lookup"><span data-stu-id="a5c9f-140">Named resources aren't supported in project templates.</span></span>
