---
title: הערכות של מכירות ופרויקטים
description: נושא זו מספק מידע על הפקת המרב מלוח הזמנים ומהערכות בתהליך המכירות.
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
ms.openlocfilehash: d8bb380519759659dc1b4151b62228a626ee7a26
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4120679"
---
# <a name="sales-estimates-and-projects"></a><span data-ttu-id="a2fca-103">הערכות של מכירות ופרויקטים</span><span class="sxs-lookup"><span data-stu-id="a2fca-103">Sales estimates and projects</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a2fca-104">במהלך תהליך המכירות, תוכל ליצור הערכות מכירה על-ידי קישור פרויקט להצעת מחיר של מכירות.</span><span class="sxs-lookup"><span data-stu-id="a2fca-104">During the sales process, you can create sales estimates by linking a project to a sales quote.</span></span> <span data-ttu-id="a2fca-105">כך ניתן לבצע הערכה דטרמיניסטית במהלך תהליך המכירות כדי להפיק את המרב מיכולות ההערכה והתזמון של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a2fca-105">In this way, deterministic estimation can occur during the sales process, to take advantage of project scheduling and estimation capabilities.</span></span> <span data-ttu-id="a2fca-106">אם המכירה מתבצעת, ניתן להשתמש בלוח הזמנים ששימש למטרת הערכת המכירות כבסיס לכוונון נוסף של תוכנית הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a2fca-106">If the sale goes through, the schedule that was used for sales estimation purposes can be used as the basis for further refinement of the project plan.</span></span>

## <a name="linking-a-project-to-a-quote-line"></a><span data-ttu-id="a2fca-107">קישור פרויקט לשורת הצעת המחיר</span><span class="sxs-lookup"><span data-stu-id="a2fca-107">Linking a project to a quote line</span></span>

<span data-ttu-id="a2fca-108">בעת יצירת שורת הצעת מחיר מבוססת פרויקט, תוכל ליצור פרויקט חדש או לשייך פרויקט קיים בדף **שורת הצעת מחיר**.</span><span class="sxs-lookup"><span data-stu-id="a2fca-108">When you create a project-based quote line, you can create a new project or associate an existing project pn the **Quote Line** page.</span></span> 

> ![טופס שורת הצעת מחיר](media/project-8.png)
 
<span data-ttu-id="a2fca-110">בעת יצירת פרויקט חדש מפרטי שורת הצעת המחיר,תוכל להשתמש בתבניות הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a2fca-110">When you create a new project from the quote line details, you can take advantage of project templates.</span></span> <span data-ttu-id="a2fca-111">תבניות פרויקט הן פרויקטים לדוגמה המייצגים תוכניות פרויקט סטנדרטיות והערכות פיננסיות האופייניות לארגון.</span><span class="sxs-lookup"><span data-stu-id="a2fca-111">Project templates are model projects that represent standard project plans and financial estimates that are typical in an organization.</span></span> <span data-ttu-id="a2fca-112">הן יכולות לייצג גם העתקים של תוכניות פרויקט והערכות מפרויקטי עבר.</span><span class="sxs-lookup"><span data-stu-id="a2fca-112">They can also represent copies of project plans and estimates from past projects.</span></span>

> ![פרטים בשורת הצעת מחיר](media/project-9.png)
  
<span data-ttu-id="a2fca-114">בעת יצירת הפרויקט מהצעת המחיר, הפרויקט משויך באופן אוטומטי לשורת הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="a2fca-114">When you create the project from the quote, the project is automatically associated with the quote line.</span></span>

## <a name="components-of-estimates-in-a-project"></a><span data-ttu-id="a2fca-115">רכיבי הערכות בפרויקט</span><span class="sxs-lookup"><span data-stu-id="a2fca-115">Components of estimates in a project</span></span>

<span data-ttu-id="a2fca-116">לוח זמנים מאפשר לך לחלק את העבודה למשימות, לשמור על הירארכיה של משימות, לקבוע אילו משאבים נדרשים כדי להשלים משימה ולהקצות הערכה של המאמץ הדרוש להשלמת פעילות.</span><span class="sxs-lookup"><span data-stu-id="a2fca-116">A schedule lets you divide work into tasks, maintain a hierarchy of tasks, determine what resources are required to complete a task, and assign an estimate of the effort that is required to complete a task.</span></span>

<span data-ttu-id="a2fca-117">באפשרותך להגדיר את הערכות לוח הזמנים ומאמץ העבודה באמצעות השדות בכרטיסיה **לוח זמנים** בדף **פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="a2fca-117">You can define the work effort and schedule estimates by using the fields on the **Schedule** tab of the **Project** page.</span></span> <span data-ttu-id="a2fca-118">מאחר שמחירון משויך לפרויקט, הערכות פיננסיות מחושבות באמצעות מחירי העלות והמכירה המוגדרים במחירון.</span><span class="sxs-lookup"><span data-stu-id="a2fca-118">Because a price list is associated with the project, financial estimates are calculated by using cost and sales prices that are defined in the price list.</span></span>

## <a name="importing-estimates-from-a-project-into-a-quote"></a><span data-ttu-id="a2fca-119">ייבוא הערכות מפרויקט לתוך הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="a2fca-119">Importing estimates from a project into a quote</span></span>

<span data-ttu-id="a2fca-120">לאחר שתגדיר הערכות פרויקט, תוכל לייבא אותן לשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="a2fca-120">After you define project estimates, you can import them into the quote line.</span></span> <span data-ttu-id="a2fca-121">בדף **פרטי שורת הצעת מחיר**, בחר **יבא מהערכות** ברצועת הכלים כדי לסכם את הערכות בפרויקט לפי סוג עסקה, תפקיד ורמת משימה.</span><span class="sxs-lookup"><span data-stu-id="a2fca-121">On the **Quote Line Details** page, select **Import from estimates** on the ribbon to summarize project estimates by transaction type, role, or task level.</span></span>
