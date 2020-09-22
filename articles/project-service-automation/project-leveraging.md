---
title: הערכות של מכירות ופרוייקטים
description: נושא זו מספק מידע על הפקת המרב מלוח הזמנים ומהערכות בתהליך המכירות.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: eb5ab6a1-fdff-490e-9c2a-19aef493de11
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 4431c1c894a01bfecc132575d8981ebc9fe50b51
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751784"
---
# <a name="sales-estimates-and-projects"></a><span data-ttu-id="d523c-103">הערכות של מכירות ופרוייקטים</span><span class="sxs-lookup"><span data-stu-id="d523c-103">Sales estimates and projects</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="d523c-104">במהלך תהליך המכירות, תוכל ליצור הערכות מכירה על-ידי קישור פרוייקט להצעת מחיר של מכירות.</span><span class="sxs-lookup"><span data-stu-id="d523c-104">During the sales process, you can create sales estimates by linking a project to a sales quote.</span></span> <span data-ttu-id="d523c-105">כך ניתן לבצע הערכה דטרמיניסטית במהלך תהליך המכירות כדי להפיק את המרב מיכולות ההערכה והתזמון של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="d523c-105">In this way, deterministic estimation can occur during the sales process, to take advantage of project scheduling and estimation capabilities.</span></span> <span data-ttu-id="d523c-106">אם המכירה מתבצעת, ניתן להשתמש בלוח הזמנים ששימש למטרת הערכת המכירות כבסיס לכוונון נוסף של תוכנית הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="d523c-106">If the sale goes through, the schedule that was used for sales estimation purposes can be used as the basis for further refinement of the project plan.</span></span>

## <a name="linking-a-project-to-a-quote-line"></a><span data-ttu-id="d523c-107">קישור פרוייקט לשורת הצעת המחיר</span><span class="sxs-lookup"><span data-stu-id="d523c-107">Linking a project to a quote line</span></span>

<span data-ttu-id="d523c-108">בעת יצירת שורת הצעת מחיר מבוססת פרוייקט, תוכל ליצור פרויקט חדש או לשייך פרוייקט קיים בדף **שורת הצעת מחיר**.</span><span class="sxs-lookup"><span data-stu-id="d523c-108">When you create a project-based quote line, you can create a new project or associate an existing project pn the **Quote Line** page.</span></span> 

> ![טופס שורת הצעת מחיר](media/project-8.png)
 
<span data-ttu-id="d523c-110">בעת יצירת פרוייקט חדש מפרטי שורת הצעת המחיר,תוכל להשתמש בתבניות הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="d523c-110">When you create a new project from the quote line details, you can take advantage of project templates.</span></span> <span data-ttu-id="d523c-111">תבניות פרוייקט הן פרוייקטים לדוגמה המייצגים תוכניות פרוייקט סטנדרטיות והערכות פיננסיות האופייניות לארגון.</span><span class="sxs-lookup"><span data-stu-id="d523c-111">Project templates are model projects that represent standard project plans and financial estimates that are typical in an organization.</span></span> <span data-ttu-id="d523c-112">הן יכולות לייצג גם העתקים של תוכניות פרוייקט והערכות מפרוייקטי עבר.</span><span class="sxs-lookup"><span data-stu-id="d523c-112">They can also represent copies of project plans and estimates from past projects.</span></span>

> ![פרטים בשורת הצעת מחיר](media/project-9.png)
  
<span data-ttu-id="d523c-114">בעת יצירת הפרוייקט מהצעת המחיר, הפרוייקט משויך באופן אוטומטי לשורת הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="d523c-114">When you create the project from the quote, the project is automatically associated with the quote line.</span></span>

## <a name="components-of-estimates-in-a-project"></a><span data-ttu-id="d523c-115">רכיבי הערכות בפרוייקט</span><span class="sxs-lookup"><span data-stu-id="d523c-115">Components of estimates in a project</span></span>

<span data-ttu-id="d523c-116">לוח זמנים מאפשר לך לחלק את העבודה למשימות, לשמור על הירארכיה של משימות, לקבוע אילו משאבים נדרשים כדי להשלים משימה ולהקצות הערכה של המאמץ הדרוש להשלמת פעילות.</span><span class="sxs-lookup"><span data-stu-id="d523c-116">A schedule lets you divide work into tasks, maintain a hierarchy of tasks, determine what resources are required to complete a task, and assign an estimate of the effort that is required to complete a task.</span></span>

<span data-ttu-id="d523c-117">באפשרותך להגדיר את הערכות לוח הזמנים ומאמץ העבודה באמצעות השדות בכרטיסיה **לוח זמנים** בדף **פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="d523c-117">You can define the work effort and schedule estimates by using the fields on the **Schedule** tab of the **Project** page.</span></span> <span data-ttu-id="d523c-118">מאחר שמחירון משויך לפרוייקט, הערכות פיננסיות מחושבות באמצעות מחירי העלות והמכירה המוגדרים במחירון.</span><span class="sxs-lookup"><span data-stu-id="d523c-118">Because a price list is associated with the project, financial estimates are calculated by using cost and sales prices that are defined in the price list.</span></span>

## <a name="importing-estimates-from-a-project-into-a-quote"></a><span data-ttu-id="d523c-119">ייבוא הערכות מפרוייקט לתוך הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="d523c-119">Importing estimates from a project into a quote</span></span>

<span data-ttu-id="d523c-120">לאחר שתגדיר הערכות פרוייקט, תוכל לייבא אותן לשורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="d523c-120">After you define project estimates, you can import them into the quote line.</span></span> <span data-ttu-id="d523c-121">בדף **פרטי שורת הצעת מחיר**, בחר **יבא מהערכות** ברצועת הכלים כדי לסכם את הערכות בפרוייקט לפי סוג עסקה, תפקיד ורמת משימה.</span><span class="sxs-lookup"><span data-stu-id="d523c-121">On the **Quote Line Details** page, select **Import from estimates** on the ribbon to summarize project estimates by transaction type, role, or task level.</span></span>
