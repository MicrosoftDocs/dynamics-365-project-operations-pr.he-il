---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 21 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 21, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 06/19/2020
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
ms.openlocfilehash: 799be481c365e82e8ffb59ba242e30378644008b
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126709"
---
# <a name="project-service-automation-update-release-21-v3"></a><span data-ttu-id="cf2f7-103">מהדורה 21, V3 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="cf2f7-103">Project Service Automation Update Release 21, V3</span></span>

<span data-ttu-id="cf2f7-104">אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="cf2f7-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="cf2f7-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="cf2f7-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="cf2f7-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="cf2f7-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="cf2f7-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 21, עדכון V3 של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 21.</span></span> <span data-ttu-id="cf2f7-110">גירסה זו כוללת מספר build של V 3.10.32.50 ובדרך כלל היא זמינה דרך עדכון עצמי ביוני 2020.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-110">This version has a build number of V 3.10.32.50 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-21"></a><span data-ttu-id="cf2f7-111">הפצת עדכון 21</span><span class="sxs-lookup"><span data-stu-id="cf2f7-111">Update Release 21</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="cf2f7-112">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="cf2f7-112">Bug fixes</span></span>

<span data-ttu-id="cf2f7-113">**זמן והוצאה**</span><span class="sxs-lookup"><span data-stu-id="cf2f7-113">**Time and Expense**</span></span>

<span data-ttu-id="cf2f7-114">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="cf2f7-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="cf2f7-115">בעת אירוח **פקד רשת ערכי זמן** בלוח המחוונים, הרשת אינה מנצלת את הרוחב המלא של מיכל רשת לוח המחוונים.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-115">When hosting the **Time Entry Grid Control** in Dashboards, the grid does not utilize the full width of the dashboard grid container.</span></span>
- <span data-ttu-id="cf2f7-116">עבור אזורי זמן ספציפיים, פקד הרשת **ערכי זמן** לא מציג רשומות.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-116">For specific time zones, the **Time Entry** grid control does not display records.</span></span>
- <span data-ttu-id="cf2f7-117">ערכי זמן שאחרי 21:00 מופיעים ביום הלא נכון.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-117">Time entries that are after 9:00 PM appear on the wrong day.</span></span>
- <span data-ttu-id="cf2f7-118">משתמשים אינם יכולים להגיש הוצאות אם בקטגוריית ההוצאות, **נדרשת קבלה על הוצאות** אין ערך.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-118">Users are unable to submit expenses if the expense category, **Expense receipt required** has no value.</span></span>

<span data-ttu-id="cf2f7-119">**ניהול משאבים**</span><span class="sxs-lookup"><span data-stu-id="cf2f7-119">**Resource Management**</span></span>

<span data-ttu-id="cf2f7-120">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="cf2f7-120">The following issues have been fixed:</span></span>

- <span data-ttu-id="cf2f7-121">הזמנות לא פעילות מוצגות בתצוגה **פיוס‬**.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-121">Inactive bookings are displayed in the **Reconciliation** view.</span></span>
- <span data-ttu-id="cf2f7-122">למימוש משאב כללי אין אימות כדי להבטיח שקיים סטטוס הזמנה תקף.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-122">Generic resource fulfillment was missing validation to ensure that a valid booking status exists.</span></span>

<span data-ttu-id="cf2f7-123">**ניהול פרויקט**</span><span class="sxs-lookup"><span data-stu-id="cf2f7-123">**Project Management**</span></span>

<span data-ttu-id="cf2f7-124">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="cf2f7-124">The following issues have been fixed:</span></span>

- <span data-ttu-id="cf2f7-125">רשתות הטפסים **פרויקט** (**הקצאת משאב**, **משימה**, **פיוס**, **הערכת הוצאות**) ניתנות לעריכה אפילו אם הפרויקט לא פעיל.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-125">The **Project** form grids (**Resource Assignment**, **Task**, **Reconciliation** view, **Expense Estimates**) remain editable even when a project is not active.</span></span>
- <span data-ttu-id="cf2f7-126">לא ניתן למזג לקוחות כפולים עם לקוחות המקושרים לחוזי פרויקט שאושרו.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-126">Duplicate customers can't be merged with customers that are linked to confirmed project contracts.</span></span>
- <span data-ttu-id="cf2f7-127">כאשר נוסף משאב שאין לו לוח שנה תקף, המערכת לא מחזירה הודעת שגיאה ידידותית למשתמש.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-127">When a resource who does not have a valid calendar is added, the system does not return a user friendly-error message.</span></span>
- <span data-ttu-id="cf2f7-128">הלחצן **הוסף משימה** ברשת המשימות מופעל כאשר הפרויקט מקושר אל **תוסף Microsoft Project**.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-128">The **Add Task** button on the task grid is enabled when the project is linked to **Microsoft Project add-in**.</span></span>
- <span data-ttu-id="cf2f7-129">המאמץ גדל ללא שליטה כאשר משימה עם קטגוריה מוקצית למשאב עם תפקיד שעבורו מוגדר מחיר עלות.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-129">Effort grows uncontrollably when a task with a category is assigned to a resource with a role for which there is a cost price defined.</span></span>

<span data-ttu-id="cf2f7-130">**Sales**</span><span class="sxs-lookup"><span data-stu-id="cf2f7-130">**Sales**</span></span>

<span data-ttu-id="cf2f7-131">השיפורים הבאים בוצעו:</span><span class="sxs-lookup"><span data-stu-id="cf2f7-131">The following enhancements have been made:</span></span>

- <span data-ttu-id="cf2f7-132">**תדירות חשבוניות** וגם **התחלת חיוב** הועברו אל הכרטיסיה **לוח זמנים לחשבוניות**.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-132">**Invoice Frequency** and **Billing Start** have been moved to the **Invoice Schedule** tab.</span></span>

<span data-ttu-id="cf2f7-133">הבעיות הבאות תוקנו:</span><span class="sxs-lookup"><span data-stu-id="cf2f7-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="cf2f7-134">**מחיר מכירה כולל** הוא אפס (0) עבור **קטגוריה** למרות של- **תפקיד** יש מחיר מכירה כולל שאינו אפס.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-134">**Total Sales Price** is zero (0) for **Category** even though **Role** has a total sales price that is not zero.</span></span>
- <span data-ttu-id="cf2f7-135">לקוחות אינם יכולים לשנות את השדה **סטטוס חשבונית** לערך **מוכן להגשת חשבונית** כאשר תהליך מותאם אישית אחר מעדכן שדה נוסף.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-135">Customers can't change the value of the **Invoice Status** field to **Ready for invoicing** when another customized process is updating an additional field.</span></span>
- <span data-ttu-id="cf2f7-136">הלחצן **רענן שורות בחשבונת** יכול ליצור שורות כפולות מרובות אם הוא נבחר שוב ושוב.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-136">The **Refresh Invoice Lines** button can create multiple duplicated lines if it is repeatedly selected.</span></span>
- <span data-ttu-id="cf2f7-137">הלחצן **עדכן מחירים** לא עובד רשת המשנה **מחירי תפקידים** בטופס **תצוגה מהירה**.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-137">The **Update Prices** button doesn't work on the **Role Prices** subgrid in the **Quick View** form.</span></span>
- <span data-ttu-id="cf2f7-138">הלוגיקה **החלטת מחירון מכירות** מטפלת באופן לא נכון באזורי זמן, וכתוצאה מכך יש בחירה שגויה של מחירונים.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-138">The **Sales Price List Resolution** logic improperly handles time zones, resulting in the incorrect selection of price lists.</span></span>
- <span data-ttu-id="cf2f7-139">**עלות בפועל** של פרויקט יכולה להיות שגויה לאחר אישור של ערך זמן בודד.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-139">A project’s **Total Actual Cost** can be off by a fractional amount after a single time entry is approved.</span></span>
- <span data-ttu-id="cf2f7-140">הלוגיקה של **רזולוציית מחירים** אינה מספקת הודעת שגיאה ידידותית למשתמש אם אין ערכים של **מחיר תפקיד שאוחזר** בשדות **היחידה הראשית** ו- **מחיר ביחידה ראשונית**.</span><span class="sxs-lookup"><span data-stu-id="cf2f7-140">The **Price Resolution** logic does not provide a user-friendly error message if **Retrieved RolePrice** doesn't have values in **'Primary Unit'** and **'Price In Primary Unit'** fields.</span></span>
