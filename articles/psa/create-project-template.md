---
title: ליצור תבנית פרוייקט
description: כיצד ליצור תבנית פרוייקט ב- Project Service
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: 700d1bb1fd7299b49b6c6f8e4d84d14bc1d52c1a
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077321"
---
# <a name="create-a-project-template-project-service"></a><span data-ttu-id="3ce01-103">יצירת תבנית פרוייקט (Project Service)</span><span class="sxs-lookup"><span data-stu-id="3ce01-103">Create a project template (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="3ce01-104">תבניות פרוייקטים חוסכות לך זמן אם החברה שלך באופן קבוע משתתפת במכרזים עבור סוגים דומים של פרוייקטים.</span><span class="sxs-lookup"><span data-stu-id="3ce01-104">Project templates save you time if your company regularly bids on similar types of projects.</span></span> <span data-ttu-id="3ce01-105">הן מספקות קבוצת תפקידים רגילה ושעות משוערות‬ עבור סוג של פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="3ce01-105">They provide a standard set of roles and estimated hours for a type of project.</span></span> <span data-ttu-id="3ce01-106">מנהלי פרוייקטים ומנהלי תיקי לקוחות יכולים ליצור פרוייקטים בהתבסס על תבנית פרוייקט, או הם יכולים להעתיק את התבנית וליצור אחת משלהם.</span><span class="sxs-lookup"><span data-stu-id="3ce01-106">Account managers and project managers can create projects based on a project template, or they can copy the template and make one of their own.</span></span>  
  
## <a name="components-of-project-template"></a><span data-ttu-id="3ce01-107">רכיבים של תבנית פרוייקט</span><span class="sxs-lookup"><span data-stu-id="3ce01-107">Components of project template</span></span>
 <span data-ttu-id="3ce01-108">תבנית פרוייקט כוללת שלושה מרכיבים:</span><span class="sxs-lookup"><span data-stu-id="3ce01-108">A project template consists of three components:</span></span>  
  
- <span data-ttu-id="3ce01-109">**מבנה התפלגות עבודה** : מבנה התפלגות עבודה בתבנית הפרוייקט מכיל אותה קבוצת רכיבים כמו בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="3ce01-109">**Work breakdown structure** : A work breakdown structure in a project template has the same set of elements as in the project.</span></span> <span data-ttu-id="3ce01-110">באפשרותך ליצור היררכיית משימות, לשייך תפקידים למשימה, להגדיר תכונות של לוח זמנים, להגדיר יחסי תלות ולהציג את כל הנתונים ב- Gantt.</span><span class="sxs-lookup"><span data-stu-id="3ce01-110">You can create a task hierarchy, associate roles to task, define schedule attributes, set dependencies and view all the data in the Gantt.</span></span> <span data-ttu-id="3ce01-111">מבנה התפלגות העבודה בתבניות פרוייקט תומך גם במצבי משימה עבור כל משימה.</span><span class="sxs-lookup"><span data-stu-id="3ce01-111">The work breakdown structure in project templates also support task modes for each task.</span></span> <span data-ttu-id="3ce01-112">אין כל הבדל בין תבנית פרוייקט ופרוייקט בעת יצירת לוח זמנים לעבודה.</span><span class="sxs-lookup"><span data-stu-id="3ce01-112">There is no difference between a project template and a project when creating work schedule.</span></span>  
  
- <span data-ttu-id="3ce01-113">**הערכות פרוייקט** : הערכות פרוייקט בתבניות פועלות באותו האופן כמו בפרוייקטים, מלבד העובדה שמחירונים המשמשים להגדרת ברירת המחדל של העלות ומחירי המכירה הם תמיד העלות ומחירוני המכירות שהוגדרו כברירת מחדל בפרמטרים של [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="3ce01-113">**Project estimates** : Project estimates in templates work the same way as they do in projects, except the price lists for defaulting the cost and sales prices are always the default cost and sales price lists defined in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] parameters.</span></span> <span data-ttu-id="3ce01-114">שאר הפונקציונליות היא כמו בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="3ce01-114">The rest of the functionality is the same as in a project.</span></span>  
  
- <span data-ttu-id="3ce01-115">**יצירת צוות פרוייקט** : בעת יצירת צוות פרוייקט עבור תבנית פרוייקט, אין אפשרות להזמין משאב בעל שם בתבנית.</span><span class="sxs-lookup"><span data-stu-id="3ce01-115">**Project team formation** : When forming a project team for a project template, you can’t book a named resource in a template.</span></span> <span data-ttu-id="3ce01-116">באפשרותך להשתמש באפשרות **צור צוות פרוייקט** במבנה התפלגות העבודה כדי ליצור קבוצת משאבים כלליים.</span><span class="sxs-lookup"><span data-stu-id="3ce01-116">You can use **Generate Project Team** in the work breakdown structure to generate a set of generic resources.</span></span> <span data-ttu-id="3ce01-117">באפשרותך גם לציין את הכישורים והמומחיות הנדרשים עבור משאבים כלליים.</span><span class="sxs-lookup"><span data-stu-id="3ce01-117">You can also specify required skills and proficiencies for generic resources.</span></span> <span data-ttu-id="3ce01-118">לא ניתן להחליף משאב כללי במשאב הניתן להזמנה בתבניות פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="3ce01-118">You can’t substitute a generic resource with a bookable resource in project templates.</span></span>  
  
## <a name="create-a-project-from-a-template"></a><span data-ttu-id="3ce01-119">יצירת פרוייקט מתבנית</span><span class="sxs-lookup"><span data-stu-id="3ce01-119">Create a project from a template</span></span>  
 <span data-ttu-id="3ce01-120">ניתן ליצור פרוייקט מתבנית בדרכים הבאות:</span><span class="sxs-lookup"><span data-stu-id="3ce01-120">You can create a project from a template in these following ways:</span></span>  
  
-   <span data-ttu-id="3ce01-121">בעת יצירת פרוייקט מהצעת המחיר, באפשרותך לבחור תבנית פרוייקט בטופס יצירה מהירה של פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="3ce01-121">When creating a project from the quote, you can choose a project template in the project quick create form.</span></span>  
  
-   <span data-ttu-id="3ce01-122">בעת יצירת פרוייקט על-ידי לחיצה על **פרוייקט חדש** , יוצג טופס הפרוייקט לפני שמירת הרשומה.</span><span class="sxs-lookup"><span data-stu-id="3ce01-122">When creating a project by clicking **New Project** , the project form displays before you save the record.</span></span> <span data-ttu-id="3ce01-123">מכאן, באפשרותך ללחוץ על השדה **בחר תבנית** כדי לבחור מתוך רשימת תבניות פרוייקט מוגדרות מראש בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="3ce01-123">From here, you can click **Pick a template** field to choose from the list of pre-defined project templates in your organization.</span></span>  
  
-   <span data-ttu-id="3ce01-124">לחץ על **צור פרוייקט מתבנית** בדף **תבנית פרוייקט** כדי ליצור פרוייקט מהתבנית.</span><span class="sxs-lookup"><span data-stu-id="3ce01-124">Click **Create project from a template** on the **Project Template** page to create a project from the template.</span></span>  
  
## <a name="copying-components-of-a-template-to-a-project"></a><span data-ttu-id="3ce01-125">העתקת רכיבי תבנית לפרוייקט</span><span class="sxs-lookup"><span data-stu-id="3ce01-125">Copying components of a template to a project</span></span>  
 <span data-ttu-id="3ce01-126">בעת העתקת רכיבי תבנית לפרוייקט, ישנם כמה דברים שעליך לדעת.</span><span class="sxs-lookup"><span data-stu-id="3ce01-126">When you copy components of a template into a project, there are a few things you should know about.</span></span>  
  
 <span data-ttu-id="3ce01-127">**העתקת מבנה התפלגות עבודה** : כאשר מעתיקים את מבנה התפלגות העבודה מתבנית פרוייקט, אם הפרוייקט כולל לוח תאריכים של פרוייקט השונה מזה של התבנית, שעות העבודה מלוח התאריכים של הפרוייקט יחולו על לוח הזמנים של משימות.</span><span class="sxs-lookup"><span data-stu-id="3ce01-127">**Copying a work breakdown structure** : When you copy the work breakdown structure from a project template, if the project has a different project calendar than the template, the work hours from the project’s calendar will be applied to the schedule of tasks.</span></span> <span data-ttu-id="3ce01-128">פעולה זו מתאימה את לוח הזמנים ללוח התאריכים של פרוייקט גיבוי.</span><span class="sxs-lookup"><span data-stu-id="3ce01-128">This adjusts the schedule to the backing project calendar.</span></span> <span data-ttu-id="3ce01-129">באופן דומה, המשימה הראשונה במבנה התפלגות העבודה מקבלת את תאריך ההתחלה של הפרוייקט, כך ששאר לוח הזמנים של הירארכיית המשימות מתעדכן בהתאם למשך הזמן וליחסי התלות שצוינו במבנה התפלגות עבודה של התבנית.</span><span class="sxs-lookup"><span data-stu-id="3ce01-129">Similarly, the first task on the work breakdown structure takes the project’s start date, so the rest of the task hierarchy schedule is updated based on the duration and dependencies specified in the template’s work breakdown structure.</span></span>  
  
 <span data-ttu-id="3ce01-130">**העתקת הערכות פרוייקט** : בעת העתקה בשורות הערכה עבור פרוייקט, מחירונים מתעדכנים על בסיס יחידת הבעלות של הפרוייקט עבור מחירון העלות והלקוח עבור מחירון המכירות.</span><span class="sxs-lookup"><span data-stu-id="3ce01-130">**Copying project estimates** : When you copy across project estimate lines, price lists are updated based on the owning unit of the project for the cost price list and customer for the sales price list.</span></span> <span data-ttu-id="3ce01-131">עלות יחידה ומחירי מכירה נקבעים מתוך מחירונים אלה בפרוייקטים המשויכים ליישות מכירות.</span><span class="sxs-lookup"><span data-stu-id="3ce01-131">The unit cost and sales prices are determined from these price lists on projects that are associated to a sales entity.</span></span>  
  
 <span data-ttu-id="3ce01-132">**העתקת צוות הפרוייקט** : בעת העתקה של צוות הפרוייקט מהתבנית לפרוייקט, המשאבים הכלליים מועתקים, יחד עם הכישורים והמיומנויות שהוגדרו בתבנית.</span><span class="sxs-lookup"><span data-stu-id="3ce01-132">**Copying a project team** : When you copy the project team from the template to a project, the generic resources are copied across, along with the skills and proficiencies defined in the template.</span></span> <span data-ttu-id="3ce01-133">גם אופן הטיפול בהקצאות המשאבים הכלליים זהה לזה שבתבנית הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="3ce01-133">Generic resource assignments are also maintained as in the project template.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="3ce01-134">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="3ce01-134">See Also</span></span>  
 [<span data-ttu-id="3ce01-135">מדריך למנהל פרוייקט</span><span class="sxs-lookup"><span data-stu-id="3ce01-135">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
