---
title: אספקת הערכות עבודה עבור פרויקט במהלך תהליך המכירה
description: כיצד לספק הערכות עבודה עבור פרויקט במהלך תהליך המכירה ב- ‏‫Project Service
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
ms.openlocfilehash: ddb7f8c0ff8c7fd7e51edb42f9d227f2b91a811b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077358"
---
# <a name="provide-work-estimates-for-a-project-during-the-sales-process-project-service"></a><span data-ttu-id="68de6-103">אספקת הערכות עבודה עבור פרויקט במהלך תהליך המכירה (Project Service)</span><span class="sxs-lookup"><span data-stu-id="68de6-103">Provide work estimates for a project during the sales process (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="68de6-104">במהלך תהליך מכירה תוכל ליצור הערכות מכירות באופן יסודי עם שורות הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="68de6-104">During the sales process, you can work out sales estimates from the ground up with quote lines.</span></span> <span data-ttu-id="68de6-105">יכולות [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ב- [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] מספקות דרך דטרמיניסטית ומדעית יותר ליצור הערכות מכירות על-ידי זיהוי פריטי עבודה ושיוך תכונות רלוונטיות התורמות להערכות עבור הפרויקט במבנה התפלגות העבודה.</span><span class="sxs-lookup"><span data-stu-id="68de6-105">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] provide a more scientific and deterministic way of coming up with sales estimates by breaking down work items and associating relevant attributes that contribute toward the estimates for the project in the work breakdown structure.</span></span>  
  
 <span data-ttu-id="68de6-106">לאחר שתזכה במכירה, באפשרותך להשתמש במבנה התפלגות העבודה המשויך לתוכנית הפרויקט שלך, לשכלל אותה לפי הצורך כדי להשלים בהצלחה את הפרויקט שלך.</span><span class="sxs-lookup"><span data-stu-id="68de6-106">Once you win the sale, you can use the associated work breakdown structure in your project plan, refining it as necessary for successful completion of your project.</span></span>  
  
## <a name="link-a-project-to-a-quote-line"></a><span data-ttu-id="68de6-107">קישור פרויקט לשורת הצעת המחיר</span><span class="sxs-lookup"><span data-stu-id="68de6-107">Link a project to a quote line</span></span>  
 <span data-ttu-id="68de6-108">בעת יצירה של שורת הצעת המחיר המבוססת על פרויקט, באפשרותך ליצור פרויקט חדש מתוך שורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="68de6-108">When creating a project-based quote line, you can create a new project from the quote line.</span></span> <span data-ttu-id="68de6-109">תוכל להשתמש בתבניות פרויקט, שהן תוכניות פרויקט רגילות שתצורתן נקבעה מראש וכן הערכות פיננסיות המשותפות לכל הארגון שלך, או עותק של תוכנית פרויקט והערכות מפרויקט קודם.</span><span class="sxs-lookup"><span data-stu-id="68de6-109">You can then use project templates, which are either pre-configured standard project plans and financial estimates common to your organization, or a copy of a project plan and estimates from a past project.</span></span> <span data-ttu-id="68de6-110">בעת יצירת פרויקט, בחירת תבנית פרויקט מספקת בסיס לתוכנית הפרויקט, ההערכות, התפקיד והדרישות.</span><span class="sxs-lookup"><span data-stu-id="68de6-110">When you create a project, choosing a project template provides a basis to refine the project plan, estimates, and role requirements.</span></span> <span data-ttu-id="68de6-111">על-ידי יצירת הפרויקט מהצעת המחיר, הפרויקט משויך באופן אוטומטי לשורת הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="68de6-111">By creating your project from the quote, the project is automatically associated with the quote line.</span></span>  
  
## <a name="project-estimate-components"></a><span data-ttu-id="68de6-112">רכיבים של הערכת פרויקט</span><span class="sxs-lookup"><span data-stu-id="68de6-112">Project estimate components</span></span>  
 <span data-ttu-id="68de6-113">מבנה התפלגות העבודה בפרויקט מספק דרך לחלק את העבודה למשימות, לשמור על היררכיה של משימות ולהקצות הערכה של המאמץ הנדרש להשלמת כל פעילות.</span><span class="sxs-lookup"><span data-stu-id="68de6-113">The work breakdown structure in a project provides a way to break down work into tasks, maintain a hierarchy of tasks, and assign an estimate of effort required to complete each task.</span></span> <span data-ttu-id="68de6-114">באפשרותך גם לשייך תפקידים לפעילות כדי לציין הערכה של סוג המשאב הדרוש להשלמת משימה ולוח זמנים.</span><span class="sxs-lookup"><span data-stu-id="68de6-114">You can also associate roles to a task to indicate an estimate of the type of resource required to complete a task and a schedule.</span></span>  
  
 <span data-ttu-id="68de6-115">מבנה התפלגות העבודה מסייע לך לקבוע את העבודה הנדרשת ואת הערכת לוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="68de6-115">The work breakdown structure helps you determine work effort and schedule estimates.</span></span> <span data-ttu-id="68de6-116">כברירת מחדל, הפרויקט משתמש במחירוני ברירת המחדל שהגדרת קודם לכן.</span><span class="sxs-lookup"><span data-stu-id="68de6-116">By default, the project uses default price lists that you defined earlier.</span></span> <span data-ttu-id="68de6-117">המחירים והמכירות המוגדרים במחירונים מסייעים לקבוע הערכות פיננסיות עבור התפלגות העבודה של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="68de6-117">The cost and sales prices defined in the price lists help determine financial estimates for the project’s work breakdown.</span></span>  
  
 <span data-ttu-id="68de6-118">אם הפרויקט משויך להצעת מחיר, והצעת המחיר כוללת מחירון שונה מברירת המחדל, המחירון של הצעת המחיר משמש להערכות פיננסיות.</span><span class="sxs-lookup"><span data-stu-id="68de6-118">If your project is associated with a quote, and the quote has a different price list from the default, the quote’s price list is used for financial estimates.</span></span>  
  
## <a name="import-estimates-from-a-project-into-a-quote"></a><span data-ttu-id="68de6-119">ייבוא הערכות מפרויקט לתוך הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="68de6-119">Import estimates from a project into a quote</span></span>  
 <span data-ttu-id="68de6-120">לאחר שיצרת הערכות פרויקט בפרויקט, באפשרותך לייבא הערכות אלה לשורת הצעת מחיר:</span><span class="sxs-lookup"><span data-stu-id="68de6-120">Once you have project estimates in the project, you can import these estimates into the quote line:</span></span>  
  
-   <span data-ttu-id="68de6-121">ב- **פרטי שורת הצעת מחיר** , לחץ על **ייבוא מתוך הערכות**.</span><span class="sxs-lookup"><span data-stu-id="68de6-121">In **Quote Line Details** , click **Import from estimates**.</span></span> 

-   <span data-ttu-id="68de6-122">בחר אם לייבא הערכות פרויקט עם סיכום לפי סוג תנועה, תפקיד או רמת צומת של מבנה התפלגות העבודה.</span><span class="sxs-lookup"><span data-stu-id="68de6-122">Select whether to import project estimates summarized by transaction type, role, or work breakdown structure node level.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="68de6-123">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="68de6-123">See Also</span></span>  
 [<span data-ttu-id="68de6-124">מדריך למנהל פרויקט</span><span class="sxs-lookup"><span data-stu-id="68de6-124">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
