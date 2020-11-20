---
title: ‏‫מעקב אחר מצב הפרויקט
description: כיצד לעקוב אחר מצב הפרויקט ב- Project Service
author: ruhercul
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: 00b6d874b42a415fe567d17e49c0ea319d8952a0
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127834"
---
# <a name="track-a-projects-status-project-service"></a><span data-ttu-id="a5830-103">מעקב אחר מצב הפרויקט (‏‫Project Service)</span><span class="sxs-lookup"><span data-stu-id="a5830-103">Track a project’s status (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="a5830-104">השתמש ב- [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] כדי לעקוב אחר התקדמות הפרויקט של לקוח.</span><span class="sxs-lookup"><span data-stu-id="a5830-104">Use the [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] to track the progress of a client’s project.</span></span>  

<span data-ttu-id="a5830-105">עם התקדמות המעורבות, שלבי הפרויקט מתעדכנים כדי לשקף את שלב המעורבות:</span><span class="sxs-lookup"><span data-stu-id="a5830-105">As the engagement progresses, the project stages update to reflect the stage of the engagement:</span></span>  


|              |                                                                                                                                                                                                                                                                                                  |
|--------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   <span data-ttu-id="a5830-106">**חדש**</span><span class="sxs-lookup"><span data-stu-id="a5830-106">**New**</span></span>    | <span data-ttu-id="a5830-107">בעת יצירת פרויקט, השלב מוגדר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="a5830-107">When you create a project, the stage is set to **New**.</span></span> <span data-ttu-id="a5830-108">אם יצרת את הפרויקט מתבנית, בשלב זה הפרויקט עשוי לכלול לוח זמנים, הערכות ונתוני צוות.</span><span class="sxs-lookup"><span data-stu-id="a5830-108">If you created the project from a template, at this stage the project may have a schedule, estimates, and team data.</span></span> <span data-ttu-id="a5830-109">אחרת, תהיה רק חלוקה לרמות של הפרויקט ועליך להזין באופן ידני את שאר רכיבי הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a5830-109">Otherwise, it will be the outline of the project and you need to manually enter the rest of the project components.</span></span> |
|  <span data-ttu-id="a5830-110">**הצעת מחיר**</span><span class="sxs-lookup"><span data-stu-id="a5830-110">**Quote**</span></span>   |      <span data-ttu-id="a5830-111">כאשר אתה משייך פרויקט להצעת מחיר או יוצר אותו מתוך הצעת מחיר, שלב הפרויקט מוגדר **הצעת מחיר**, וההערכות של תאריכי ההתחלה והסיום יעודכנו גם כן.</span><span class="sxs-lookup"><span data-stu-id="a5830-111">When you associate a project to a quote or create it from a quote, the project stage is set to **Quote**, and the estimated start and end datesare updated as well.</span></span> <span data-ttu-id="a5830-112">כאשר הפרויקט בשלב הצעת מחיר, פרטים על הצעת המחיר יופיעו בכרטיסיה **Sales** בדף **פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="a5830-112">When the project is in the quote stage, details on the quote display on the **Sales** tab on the **Project** page.</span></span>      |
|   <span data-ttu-id="a5830-113">**תוכנית**</span><span class="sxs-lookup"><span data-stu-id="a5830-113">**Plan**</span></span>   |                                     <span data-ttu-id="a5830-114">כאשר תזכה בהצעת מחיר המשויכת לפרויקט, וכאשר המעורבות מתקדמת לשלב החוזה, שלב הפרויקט מתעדכן ל: **תכנון**.</span><span class="sxs-lookup"><span data-stu-id="a5830-114">When you win a quote associated with a project, and when the engagement progresses to the contract stage, the project stage updates to **Plan**.</span></span> <span data-ttu-id="a5830-115">פרטי החוזה מופיעים בכרטיסיה **Sales** בדף **פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="a5830-115">Contract details display on the **Sales** tab on the **Project** page.</span></span>                                      |
| <span data-ttu-id="a5830-116">**מלא**</span><span class="sxs-lookup"><span data-stu-id="a5830-116">**Complete**</span></span> |                    <span data-ttu-id="a5830-117">בתום העבודה על פרויקט, באפשרותך להפוך את השלב ל: **הושלם**.</span><span class="sxs-lookup"><span data-stu-id="a5830-117">When the project work is complete, you can flip the stage to **Complete**.</span></span> <span data-ttu-id="a5830-118">כאשר שלב הפרויקט מוגדר בתור 'הושלם', אפשר להבין שהעבודה בוצעה ב-100%, אך הפרויקט נשאר פתוח לזמן המתנה או לפי ערכי הוצאות שנרשמו.</span><span class="sxs-lookup"><span data-stu-id="a5830-118">When the project stage is set to complete, it’s understood that the work is 100% complete but the project is kept open for any pending time or expense entries to be recorded.</span></span>                     |
|  <span data-ttu-id="a5830-119">**סגור**</span><span class="sxs-lookup"><span data-stu-id="a5830-119">**Close**</span></span>   |           <span data-ttu-id="a5830-120">כאשר כל התנועות תועדו בפרויקט ואינך מצפה לתיעוד נוסף, באפשרותך להגדיר באופן ידני את השלב בתור **סגור**.</span><span class="sxs-lookup"><span data-stu-id="a5830-120">When all transactions have been recorded on the project and you don't expect any more to be logged, you can manually set the stage to **Close**.</span></span> <span data-ttu-id="a5830-121">כאשר הפרויקט מוגדר **סגור**, אינך יכול להכניס תנועות נוספות לפרויקט והפרויקט יהיה לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="a5830-121">When the project is set to **Close**, you can’t log any more transactions on the project and the project will be read only.</span></span>           |

## <a name="to-track-a-projects-status"></a><span data-ttu-id="a5830-122">כדי לעקוב אחר מצב הפרויקט</span><span class="sxs-lookup"><span data-stu-id="a5830-122">To track a project’s status</span></span>  

1.  <span data-ttu-id="a5830-123">עבור אל **Project Service > פרויקטים**.</span><span class="sxs-lookup"><span data-stu-id="a5830-123">Go to **Project Service > Projects**.</span></span>  

2.  <span data-ttu-id="a5830-124">לחץ על הפרויקט שברצונך לעבוד עליו.</span><span class="sxs-lookup"><span data-stu-id="a5830-124">Click the project you want to work on.</span></span>  

3.  <span data-ttu-id="a5830-125">בסרגל שלרוחב חלקו העליון של המסך, בחר את החץ למטה לצד שם הפרויקט, ולאחר מכן לחץ על **מעקב אחר פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="a5830-125">In the bar across the top of the screen, select the down arrow next to the project name, and then click **Project Tracking**.</span></span>  

4.  <span data-ttu-id="a5830-126">בחר **מעקב אחר המאמץ** או **מעקב אחר עלות** ברשימה הנפתחת מעל רשימת המשימות.</span><span class="sxs-lookup"><span data-stu-id="a5830-126">Select **Effort Tracking** or **Cost Tracking** in the drop-down list above the task list.</span></span>  

5.  <span data-ttu-id="a5830-127">לחץ פעמיים על פעילות כלשהי כדי לערוך אותה.</span><span class="sxs-lookup"><span data-stu-id="a5830-127">Double-click any task to edit it.</span></span> <span data-ttu-id="a5830-128">באפשרותך גם להעביר או לשנות גודל של הסרגלים בתרשים בגנט כדי לשנות את הזמן ואת ההתקדמות עבור פעילות.</span><span class="sxs-lookup"><span data-stu-id="a5830-128">You can also move or resize the bars in the Gantt chart to change the time and progress for a task.</span></span>  

### <a name="see-also"></a><span data-ttu-id="a5830-129">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="a5830-129">See Also</span></span>  
 [<span data-ttu-id="a5830-130">מדריך למנהל פרויקט</span><span class="sxs-lookup"><span data-stu-id="a5830-130">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
