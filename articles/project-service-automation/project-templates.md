---
title: תבניות פרוייקט
description: נושא זה מספק מידע על אופן השימוש בתבניות פרוייקטים להגדרת פרוייקט מהירה.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: f0161bf9-af4c-4a21-b767-ac20a8e30688
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5a3112c2eef9525946314bdb587c44904557fa52
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751779"
---
# <a name="project-templates"></a><span data-ttu-id="b7991-103">תבניות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="b7991-103">Project templates</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="b7991-104">תבנית פרוייקט היא מסגרת מוגדרת מראש שעוזרת לך להתחיל פרוייקט במהירות ובקלות.</span><span class="sxs-lookup"><span data-stu-id="b7991-104">A project template is a predefined framework that helps you quickly and easily start a project.</span></span> <span data-ttu-id="b7991-105">באפשרותך להשתמש בתבנית מוגדרת מראש כדי ליצור פרוייקט חדש בלחיצה אחת.</span><span class="sxs-lookup"><span data-stu-id="b7991-105">You can use a predefined template to create a new project with a single click.</span></span> <span data-ttu-id="b7991-106">באשר לפרוייקטים, עליך להגדיר את הדרישות המוקדמות עבור תבניות פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b7991-106">As for projects, you must define the prerequisites for project templates.</span></span> <span data-ttu-id="b7991-107">עליך להגדיר את לוח השנה של הפרוייקט עבור כל תבנית פרוייקט ויש להגדיר מראש את התפקידים ואת המחירונים בארגון כדי שלרכיבי התבנית יהיו נתונים שימושיים.</span><span class="sxs-lookup"><span data-stu-id="b7991-107">You must define a project calendar for each project template, and roles and price lists must be predefined in the organization, so that the components of the template have useful data.</span></span>

<span data-ttu-id="b7991-108">תבנית פרוייקט מורכבת משלושה רכיבים: לוח זמנים, הערכות פרוייקט וחברי צוות פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b7991-108">A project template consists of three components: a schedule, project estimates, and project team members.</span></span>

## <a name="schedule"></a><span data-ttu-id="b7991-109">תזמן</span><span class="sxs-lookup"><span data-stu-id="b7991-109">Schedule</span></span>

<span data-ttu-id="b7991-110">ללוח זמנים בתבנית פרוייקט יש את אותה קבוצת רכיבים כמו לוח זמנים בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b7991-110">A schedule in a project template has the same set of elements as a schedule in a project.</span></span> <span data-ttu-id="b7991-111">באפשרותך ליצור הירארכיית משימות, לשייך תפקידים למשימות, להגדיר תכונות של לוח זמנים ולהגדיר יחסי תלות.</span><span class="sxs-lookup"><span data-stu-id="b7991-111">You can create a task hierarchy, associate roles with tasks, define schedule attributes, and set dependencies.</span></span> <span data-ttu-id="b7991-112">לוח זמנים בתבנית פרוייקט תומך גם במצבי משימות עבור כל משימה.</span><span class="sxs-lookup"><span data-stu-id="b7991-112">A schedule in a project template also supports task modes for each task.</span></span> <span data-ttu-id="b7991-113">לכן, הוא תומך במנוע התזמון.</span><span class="sxs-lookup"><span data-stu-id="b7991-113">Therefore, it supports the scheduling engine.</span></span> <span data-ttu-id="b7991-114">עליך לשייך לוח שנה של פרוייקט לפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b7991-114">You must associate a project calendar with the project.</span></span> <span data-ttu-id="b7991-115">בעת יצירת לוח זמנים לעבודה, אין כל הבדל בין תבנית פרוייקט ופרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b7991-115">When you create a work schedule, there is no difference between a project template and a project.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="b7991-116">הערכות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="b7991-116">Project estimates</span></span>

<span data-ttu-id="b7991-117">הערכות פרוייקט בתבנית פרוייקט פועלות באותו אופן כמו הערכות פרוייקט בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b7991-117">Project estimates in a project template work the same way as project estimates in a project.</span></span> <span data-ttu-id="b7991-118">עם זאת, מחירי העלות והמכירה שנשלפים מהמחירונים בברירת מחדל של עלות ומכירות מוגדרים בפרמטרים.</span><span class="sxs-lookup"><span data-stu-id="b7991-118">However, the cost and sales prices are pulled from the default cost and sales price lists that are defined in the parameters.</span></span>

## <a name="creating-a-project-from-a-template"></a><span data-ttu-id="b7991-119">יצירת פרוייקט מתבנית</span><span class="sxs-lookup"><span data-stu-id="b7991-119">Creating a project from a template</span></span>
 
<span data-ttu-id="b7991-120">קיימות כמה דרכים ליצירת פרוייקט מתבנית פרוייקט:</span><span class="sxs-lookup"><span data-stu-id="b7991-120">There are several ways to create a project from a project template:</span></span>

- <span data-ttu-id="b7991-121">בעת יצירת פרוייקט מהצעת המחיר, באפשרותך לבחור תבנית פרוייקט בתיבת הדן-שיח **יצירה מהירה: פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="b7991-121">When you create a project from a quote, you can select a project template in the **Quick Create: Project** dialog box.</span></span>

> ![תיבת הדו-שיח 'יצירה מהירה: פרוייקט'](media/project-11.png)

- <span data-ttu-id="b7991-123">בעת יצירת פרוייקט על-ידי בחירה באפשרות **פרוייקט חדש**, הדף **פרוייקט** מופיעה לפני שהרשומה נשמרת.</span><span class="sxs-lookup"><span data-stu-id="b7991-123">When you create a project by selecting **New Project**, the **Project** page appears before the record is saved.</span></span> <span data-ttu-id="b7991-124">בשדה **בחר תבנית**, בחר תבנית אחת מתוך תבניות הפרוייקט שהוגדרו מראש בארגון.</span><span class="sxs-lookup"><span data-stu-id="b7991-124">In the **Pick a Template** field, select one of the predefined project templates in the organization.</span></span>
- <span data-ttu-id="b7991-125">השתמש באפשרות **צור פרוייקט מתבנית** שבדף **ישות תבנית**.</span><span class="sxs-lookup"><span data-stu-id="b7991-125">Use **Create Project from a Template** on the **Template Entity** page.</span></span>

## <a name="copying-components-of-template-to-project"></a><span data-ttu-id="b7991-126">העתקת רכיבי תבנית לפרוייקט</span><span class="sxs-lookup"><span data-stu-id="b7991-126">Copying components of template to project</span></span>

<span data-ttu-id="b7991-127">בעת העתקת הרכיבים של תבנית פרוייקט לפרוייקט, כמה עקיפות עשויות להתרחש, בהתאם להגדרות בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b7991-127">When you copy the components of a project template to a project, a few overrides can occur, depending on the settings in the project.</span></span>

### <a name="copying-the-schedule"></a><span data-ttu-id="b7991-128">העתקת לוח הזמנים</span><span class="sxs-lookup"><span data-stu-id="b7991-128">Copying the schedule</span></span>

<span data-ttu-id="b7991-129">בעת העתקת לוח הזמנים מתבנית פרוייקט, אם לפרוייקט יש לוח שנה שונה מהתבנית, שעות העבודה מלוח השנה של הפרוייקט מוחלות על לוח הזמנים של המשימה.</span><span class="sxs-lookup"><span data-stu-id="b7991-129">When you copy the schedule from a project template, if the project has a different project calendar than the template, work hours from the project's calendar are applied to the task schedule.</span></span> <span data-ttu-id="b7991-130">כך ניתן להתאים את לוח הזמנים ללוח השנה של הפרוייקט המהווה גיבוי.</span><span class="sxs-lookup"><span data-stu-id="b7991-130">In this way, the schedule is adjusted to match the backing project calendar.</span></span> <span data-ttu-id="b7991-131">באופן דומה, המשימה הראשונה בלוח הזמנים מקבלת את תאריך ההתחלה של הפרוייקט ולוח הזמנים של שאר ההירארכיה מתעדכן בהתאם למשך הזמן וליחסי התלות שצוינו בתבנית.</span><span class="sxs-lookup"><span data-stu-id="b7991-131">Similarly, the first task on the schedule takes the project's start date, and the schedule of the rest of the hierarchy is updated based on the duration and dependencies that are specified in the template.</span></span> 

### <a name="copying-project-estimates"></a><span data-ttu-id="b7991-132">העתקת הערכות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="b7991-132">Copying project estimates</span></span> 

<span data-ttu-id="b7991-133">בעת העתקה בין שורות הערכת פרוייקט, המחירונים מתעדכנים.</span><span class="sxs-lookup"><span data-stu-id="b7991-133">When you copy across project estimate lines, the price lists are updated.</span></span> <span data-ttu-id="b7991-134">עבור מחירון העלות, עדכונים אלה מבוססים על יחידת הבעלות של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b7991-134">For the cost price list, these updates are based on the owning unit of the project.</span></span> <span data-ttu-id="b7991-135">עבור מחירון המכירות, הם מבוססים על הלקוח.</span><span class="sxs-lookup"><span data-stu-id="b7991-135">For the sales price list, they are based on the customer.</span></span> <span data-ttu-id="b7991-136">בפרוייקטים שמשויכים לישות מכירות, עלות יחידה ומחירי מכירה נקבעים בהתאם למחירונים אלה.</span><span class="sxs-lookup"><span data-stu-id="b7991-136">For projects that are associated with a sales entity, the unit cost and sales prices are determined based on these price lists.</span></span>

### <a name="copying-a-project-team"></a><span data-ttu-id="b7991-137">העתקת צוות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="b7991-137">Copying a project team</span></span>

<span data-ttu-id="b7991-138">בעת העתקה של צוות פרוייקט מתבנית פרוייקט, המשאבים הכלליים מועתקים יחד עם הכישורים והמומחיות שהוגדרו בתבנית.</span><span class="sxs-lookup"><span data-stu-id="b7991-138">When a project team is copied from a project template to a project, the generic resources are copied, together with the skills and proficiencies that are defined in the template.</span></span> <span data-ttu-id="b7991-139">גם אופן הטיפול בהקצאות המשאבים הכלליים זהה לזה שבתבנית הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b7991-139">Generic resource assignments are also maintained as they were in the project template.</span></span> <span data-ttu-id="b7991-140">משאבים בעלי שם אינם נתמכים בתבניות פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b7991-140">Named resources aren't supported in project templates.</span></span>
