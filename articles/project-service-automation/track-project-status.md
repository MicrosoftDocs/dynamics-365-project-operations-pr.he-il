---
title: ‏‫מעקב אחר מצב הפרוייקט
description: כיצד לעקוב אחר מצב הפרוייקט ב- Project Service
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 7610aecb-318c-422b-b626-9106b0736b5f
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: e4d53b6235c3b941bce525dca09ee3d647c3d242
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751877"
---
# <a name="track-a-projects-status-project-service"></a><span data-ttu-id="a1352-103">מעקב אחר מצב הפרוייקט (‏‫Project Service)</span><span class="sxs-lookup"><span data-stu-id="a1352-103">Track a project’s status (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="a1352-104">השתמש ב- [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] כדי לעקוב אחר התקדמות הפרוייקט של לקוח.</span><span class="sxs-lookup"><span data-stu-id="a1352-104">Use the [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] to track the progress of a client’s project.</span></span>  

<span data-ttu-id="a1352-105">עם התקדמות המעורבות, שלבי הפרוייקט מתעדכנים כדי לשקף את שלב המעורבות:</span><span class="sxs-lookup"><span data-stu-id="a1352-105">As the engagement progresses, the project stages update to reflect the stage of the engagement:</span></span>  


|              |                                                                                                                                                                                                                                                                                                  |
|--------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   <span data-ttu-id="a1352-106">**חדש**</span><span class="sxs-lookup"><span data-stu-id="a1352-106">**New**</span></span>    | <span data-ttu-id="a1352-107">בעת יצירת פרוייקט, השלב מוגדר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="a1352-107">When you create a project, the stage is set to **New**.</span></span> <span data-ttu-id="a1352-108">אם יצרת את הפרוייקט מתבנית, בשלב זה הפרוייקט עשוי לכלול לוח זמנים, הערכות ונתוני צוות.</span><span class="sxs-lookup"><span data-stu-id="a1352-108">If you created the project from a template, at this stage the project may have a schedule, estimates, and team data.</span></span> <span data-ttu-id="a1352-109">אחרת, תהיה רק חלוקה לרמות של הפרוייקט ועליך להזין באופן ידני את שאר רכיבי הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="a1352-109">Otherwise, it will be the outline of the project and you need to manually enter the rest of the project components.</span></span> |
|  <span data-ttu-id="a1352-110">**הצעת מחיר**</span><span class="sxs-lookup"><span data-stu-id="a1352-110">**Quote**</span></span>   |      <span data-ttu-id="a1352-111">כאשר אתה משייך פרוייקט להצעת מחיר או יוצר אותו מתוך הצעת מחיר, שלב הפרוייקט מוגדר **הצעת מחיר**, וההערכות של תאריכי ההתחלה והסיום יעודכנו גם כן.</span><span class="sxs-lookup"><span data-stu-id="a1352-111">When you associate a project to a quote or create it from a quote, the project stage is set to **Quote**, and the estimated start and end datesare updated as well.</span></span> <span data-ttu-id="a1352-112">כאשר הפרוייקט בשלב הצעת מחיר, פרטים על הצעת המחיר יופיעו בכרטיסיה **Sales** בדף **פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="a1352-112">When the project is in the quote stage, details on the quote display on the **Sales** tab on the **Project** page.</span></span>      |
|   <span data-ttu-id="a1352-113">**תוכנית**</span><span class="sxs-lookup"><span data-stu-id="a1352-113">**Plan**</span></span>   |                                     <span data-ttu-id="a1352-114">כאשר תזכה בהצעת מחיר המשויכת לפרוייקט, וכאשר המעורבות מתקדמת לשלב החוזה, שלב הפרוייקט מתעדכן ל: **תכנון**.</span><span class="sxs-lookup"><span data-stu-id="a1352-114">When you win a quote associated with a project, and when the engagement progresses to the contract stage, the project stage updates to **Plan**.</span></span> <span data-ttu-id="a1352-115">פרטי החוזה מופיעים בכרטיסיה **Sales** בדף **פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="a1352-115">Contract details display on the **Sales** tab on the **Project** page.</span></span>                                      |
| <span data-ttu-id="a1352-116">**מלא**</span><span class="sxs-lookup"><span data-stu-id="a1352-116">**Complete**</span></span> |                    <span data-ttu-id="a1352-117">בתום העבודה על פרוייקט, באפשרותך להפוך את השלב ל: **הושלם**.</span><span class="sxs-lookup"><span data-stu-id="a1352-117">When the project work is complete, you can flip the stage to **Complete**.</span></span> <span data-ttu-id="a1352-118">כאשר שלב הפרוייקט מוגדר בתור 'הושלם', אפשר להבין שהעבודה בוצעה ב-100%, אך הפרוייקט נשאר פתוח לזמן המתנה או לפי ערכי הוצאות שנרשמו.</span><span class="sxs-lookup"><span data-stu-id="a1352-118">When the project stage is set to complete, it’s understood that the work is 100% complete but the project is kept open for any pending time or expense entries to be recorded.</span></span>                     |
|  <span data-ttu-id="a1352-119">**סגור**</span><span class="sxs-lookup"><span data-stu-id="a1352-119">**Close**</span></span>   |           <span data-ttu-id="a1352-120">כאשר כל התנועות תועדו בפרוייקט ואינך מצפה לתיעוד נוסף, באפשרותך להגדיר באופן ידני את השלב בתור **סגור**.</span><span class="sxs-lookup"><span data-stu-id="a1352-120">When all transactions have been recorded on the project and you don't expect any more to be logged, you can manually set the stage to **Close**.</span></span> <span data-ttu-id="a1352-121">כאשר הפרוייקט מוגדר **סגור**, אינך יכול להכניס תנועות נוספות לפרוייקט והפרוייקט יהיה לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="a1352-121">When the project is set to **Close**, you can’t log any more transactions on the project and the project will be read only.</span></span>           |

## <a name="to-track-a-projects-status"></a><span data-ttu-id="a1352-122">כדי לעקוב אחר מצב הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="a1352-122">To track a project’s status</span></span>  

1.  <span data-ttu-id="a1352-123">עבור אל **Project Service > פרוייקטים**.</span><span class="sxs-lookup"><span data-stu-id="a1352-123">Go to **Project Service > Projects**.</span></span>  

2.  <span data-ttu-id="a1352-124">לחץ על הפרוייקט שברצונך לעבוד עליו.</span><span class="sxs-lookup"><span data-stu-id="a1352-124">Click the project you want to work on.</span></span>  

3.  <span data-ttu-id="a1352-125">בסרגל שלרוחב חלקו העליון של המסך, בחר את החץ למטה לצד שם הפרויקט, ולאחר מכן לחץ על **מעקב אחר פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="a1352-125">In the bar across the top of the screen, select the down arrow next to the project name, and then click **Project Tracking**.</span></span>  

4.  <span data-ttu-id="a1352-126">בחר **מעקב אחר המאמץ** או **מעקב אחר עלות** ברשימה הנפתחת מעל רשימת המשימות.</span><span class="sxs-lookup"><span data-stu-id="a1352-126">Select **Effort Tracking** or **Cost Tracking** in the drop-down list above the task list.</span></span>  

5.  <span data-ttu-id="a1352-127">לחץ פעמיים על פעילות כלשהי כדי לערוך אותה.</span><span class="sxs-lookup"><span data-stu-id="a1352-127">Double-click any task to edit it.</span></span> <span data-ttu-id="a1352-128">באפשרותך גם להעביר או לשנות גודל של הסרגלים בתרשים בגנט כדי לשנות את הזמן ואת ההתקדמות עבור פעילות.</span><span class="sxs-lookup"><span data-stu-id="a1352-128">You can also move or resize the bars in the Gantt chart to change the time and progress for a task.</span></span>  

### <a name="see-also"></a><span data-ttu-id="a1352-129">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="a1352-129">See Also</span></span>  
 [<span data-ttu-id="a1352-130">מדריך למנהל פרוייקט</span><span class="sxs-lookup"><span data-stu-id="a1352-130">Project Manager Guide</span></span>](../project-service/project-manager-guide.md)
