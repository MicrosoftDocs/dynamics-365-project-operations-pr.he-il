---
title: ניהול חברי צוות
description: נושא זה מספק מידע אודות הזמנת משאבים בעלי שם לצוותי פרויקט והקצאתם למשימות.
author: ruhercul
manager: AnnBe
ms.date: 10/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: abab21ff98481166517be0c74a2c14c36d5e9d1d
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131524"
---
# <a name="maintain-team-members"></a><span data-ttu-id="994af-103">ניהול חברי צוות</span><span class="sxs-lookup"><span data-stu-id="994af-103">Maintain team members</span></span>

<span data-ttu-id="994af-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="994af-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="994af-105">באפשרותך להוסיף משאב בעל שם לצוות הפרויקט על ידי הזמנתו ישירות אל הצוות.</span><span class="sxs-lookup"><span data-stu-id="994af-105">You can add a named resource to your project team by booking them directly to the team.</span></span>

1. <span data-ttu-id="994af-106">ב-Dynamics 365 Project Operations, עבור אל **פרויקטים**, ובחר את הפרויקט הפתוח שעבורו מתבצעת ההזמנה.</span><span class="sxs-lookup"><span data-stu-id="994af-106">In Dynamics 365 Project Operations, go to **Projects**, and select the open the project that you're booking for.</span></span>
2. <span data-ttu-id="994af-107">בדף **פרויקט**, בכרטיסיה **צוות**, בחר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="994af-107">On the **Project** page, on the **Team** tab, select **New**.</span></span> 
3. <span data-ttu-id="994af-108">בתיבת הדו-שיח **יצירה מהירה של חבר צוות**, בחר את המשאב הניתן להזמנה.</span><span class="sxs-lookup"><span data-stu-id="994af-108">In the **Quick Create Project Team Member** dialog box, select the bookable resource.</span></span> <span data-ttu-id="994af-109">השדה **תפקיד** יאוכלס בתפקיד ברירת המחדל של המשאב, אם יש תפקיד שהוקצה לו.</span><span class="sxs-lookup"><span data-stu-id="994af-109">The **Role** field will populate with the resource's default role if they have one assigned.</span></span> <span data-ttu-id="994af-110">ניתן לשנות את התפקיד.</span><span class="sxs-lookup"><span data-stu-id="994af-110">You can change the role.</span></span> 
4. <span data-ttu-id="994af-111">בחר את תאריכי ה'מ' ו'עד' שבהם ידרש המשאב, ובחר את שיטת ההקצאה של קיבולת המשאב.</span><span class="sxs-lookup"><span data-stu-id="994af-111">Select the from and to dates that the resource will be needed, and select the allocation method of the resource's capacity.</span></span> 
5. <span data-ttu-id="994af-112">אם ברצונך שחבר הצוות יהיה מאשר פרויקט, בחר **כן** בשדה **מאשר פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="994af-112">In the **Project Approver** field, select **Yes** if you want the team member to be a project approver.</span></span> <span data-ttu-id="994af-113">חבר הצוות יוכל לאשר ערכי זמן והוצאה שנשלחו עבור פרויקט זה.</span><span class="sxs-lookup"><span data-stu-id="994af-113">The team member can approve submitted time and expense entries for this project.</span></span> 
6. <span data-ttu-id="994af-114">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="994af-114">Select **Save**.</span></span>

<span data-ttu-id="994af-115">כעת באפשרותך להקצות את המשאב שהוזמן למשימות בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="994af-115">You can now assign the booked resource to tasks on the project.</span></span> <span data-ttu-id="994af-116">בדף **פרויקט**, בכרטיסיה **לוח זמנים**, הקצה משימות למשאב החדש.</span><span class="sxs-lookup"><span data-stu-id="994af-116">On the **Project** page, on the **Schedule** tab, assign tasks to the new resource.</span></span> <span data-ttu-id="994af-117">בורר המשאבים שמופעל מהשדה **משאבים** ברשת המשימה יציג את חברי הצוות שבאפשרותך לבחור.</span><span class="sxs-lookup"><span data-stu-id="994af-117">The resource picker that is launched from the **Resources** field in the task grid will show the team members that you can select.</span></span>


<span data-ttu-id="994af-118">ב-Project Operations, הזמנות משאבים והקצאות משימות אינן משולבות באופן הדוק.</span><span class="sxs-lookup"><span data-stu-id="994af-118">In Project Operations, resource bookings and task assignments aren't tightly coupled.</span></span> <span data-ttu-id="994af-119">כאשר משתמשים בבורר המשאבים בלוח הזמנים, ניתן להקצות משימות לחברי צוות במספר שעות גדול יותר מכפי שההזמנות שלהם מכסות בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="994af-119">When you use the resource picker in the schedule, you can assign tasks to team members for more hours than their bookings cover on the project.</span></span>

<span data-ttu-id="994af-120">ההבדלים בין ההזמנות והמטלות של חברי הצוות מוצגים בכרטיסיות **צוות** ו **התאמה משאבים**.</span><span class="sxs-lookup"><span data-stu-id="994af-120">The differences between team member bookings and assignments are shown on the **Team** and **Resource Reconciliation** tabs.</span></span> <span data-ttu-id="994af-121">ניתן גם ליישב את ההבדלים שבין הזמנות והקצאות של משאבים ברמה מפורטת יותר.</span><span class="sxs-lookup"><span data-stu-id="994af-121">You can also reconcile the differences between bookings and assignments for resources at a more detailed level.</span></span>

<span data-ttu-id="994af-122">השתמש בבורר המשאבים בכרטיסיה **לוח זמנים** כדי לחפש ולבחור משאבים הניתנים להזמנה שאינם עדיין חלק מצוות הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="994af-122">Use the resource picker on the **Schedule** tab to search for and select bookable resources that are not already part of the project team.</span></span> <span data-ttu-id="994af-123">משאבים אלה מוצגים בבורר המשאבים כ **משאבים אחרים**.</span><span class="sxs-lookup"><span data-stu-id="994af-123">These resources are shown in the resource picker as **Other Resources**.</span></span>

<span data-ttu-id="994af-124">כאשר אתה בחור משאב, המשאב מתווסף לצוות הפרויקט ומוקצה למשימה, אבל לא נוצרות הזמנות.</span><span class="sxs-lookup"><span data-stu-id="994af-124">When you make a selection, the resource is added to the project team and assigned to the task, but no bookings are generated.</span></span>

<span data-ttu-id="994af-125">באפשרותך להשתמש ביכולת הארכת ההזמנה של הכרטיסיה  **פיוס** או ב **לוח זמנים** כדי להזמין את קיבולת המשאב לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="994af-125">You can use the **Reconciliation** tab’s extend booking capability or the **Schedule Board** to book the resource’s capacity to the project.</span></span>

<span data-ttu-id="994af-126">לאחר שחבר צוות הוזמן בפרויקט, ניתן להשתמש באפשרות **השאר הזמנות** או  להשתמש ב **לוח הזמנים** ישירות כדי לנהל את ההזמנות שלו.</span><span class="sxs-lookup"><span data-stu-id="994af-126">After a team member is booked on your project, you can use **Maintain bookings** or the **Schedule Board** directly to manage their bookings.</span></span>
