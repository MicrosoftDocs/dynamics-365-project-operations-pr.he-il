---
title: ניהול חברי צוות
description: נושא זה מספק מידע אודות הזמנת משאבים בעלי שם לצוותי פרוייקט והקצאתם למשימות.
author: ruhercul
manager: AnnBe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: f5b36628e90896c9fe6570de71c95eab83a44ebd
ms.sourcegitcommit: 396e0fea2f1598a5313cb0128eca4fe0bb5aade9
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961873"
---
# <a name="maintain-team-members"></a><span data-ttu-id="0530e-103">ניהול חברי צוות</span><span class="sxs-lookup"><span data-stu-id="0530e-103">Maintain team members</span></span>

<span data-ttu-id="0530e-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="0530e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="0530e-105">באפשרותך להוסיף משאב בעל שם לצוות הפרוייקט על ידי הזמנתו ישירות אל הצוות.</span><span class="sxs-lookup"><span data-stu-id="0530e-105">You can add a named resource to your project team by booking them directly to the team.</span></span>

1. <span data-ttu-id="0530e-106">ב-Dynamics 365 Project Operations, עבור אל **פרוייקטים**, ובחר את הפרויקט הפתוח שעבורו מתבצעת ההזמנה.</span><span class="sxs-lookup"><span data-stu-id="0530e-106">In Dynamics 365 Project Operations, go to **Projects**, and select the open the project that you're booking for.</span></span>
2. <span data-ttu-id="0530e-107">בדף **פרוייקט**, בכרטיסיה **צוות**, בחר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="0530e-107">On the **Project** page, on the **Team** tab, select **New**.</span></span> 
3. <span data-ttu-id="0530e-108">בתיבת הדו-שיח **יצירה מהירה של חבר צוות**, בחר את המשאב הניתן להזמנה.</span><span class="sxs-lookup"><span data-stu-id="0530e-108">In the **Quick Create Project Team Member** dialog box, select the bookable resource.</span></span> <span data-ttu-id="0530e-109">השדה **תפקיד** יאוכלס בתפקיד ברירת המחדל של המשאב, אם יש תפקיד שהוקצה לו.</span><span class="sxs-lookup"><span data-stu-id="0530e-109">The **Role** field will populate with the resource's default role if they have one assigned.</span></span> <span data-ttu-id="0530e-110">ניתן לשנות את התפקיד.</span><span class="sxs-lookup"><span data-stu-id="0530e-110">You can change the role.</span></span> 
4. <span data-ttu-id="0530e-111">בחר את תאריכי ה'מ' ו'עד' שבהם ידרש המשאב, ובחר את שיטת ההקצאה של קיבולת המשאב.</span><span class="sxs-lookup"><span data-stu-id="0530e-111">Select the from and to dates that the resource will be needed, and select the allocation method of the resource's capacity.</span></span> 
5. <span data-ttu-id="0530e-112">אם ברצונך שחבר הצוות יהיה מאשר פרוייקט, בחר **כן** בשדה **מאשר פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="0530e-112">In the **Project Approver** field, select **Yes** if you want the team member to be a project approver.</span></span> <span data-ttu-id="0530e-113">חבר הצוות יוכל לאשר ערכי זמן והוצאה שנשלחו עבור פרוייקט זה.</span><span class="sxs-lookup"><span data-stu-id="0530e-113">The team member can approve submitted time and expense entries for this project.</span></span> 
6. <span data-ttu-id="0530e-114">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="0530e-114">Select **Save**.</span></span>

<span data-ttu-id="0530e-115">כעת באפשרותך להקצות את המשאב שהוזמן למשימות בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0530e-115">You can now assign the booked resource to tasks on the project.</span></span> <span data-ttu-id="0530e-116">בדף **פרוייקט**, בכרטיסיה **לוח זמנים**, הקצה משימות למשאב החדש.</span><span class="sxs-lookup"><span data-stu-id="0530e-116">On the **Project** page, on the **Schedule** tab, assign tasks to the new resource.</span></span> <span data-ttu-id="0530e-117">בורר המשאבים שמופעל מהשדה **משאבים** ברשת המשימה יציג את חברי הצוות שבאפשרותך לבחור.</span><span class="sxs-lookup"><span data-stu-id="0530e-117">The resource picker that is launched from the **Resources** field in the task grid will show the team members that you can select.</span></span>


<span data-ttu-id="0530e-118">ב-Project Operations, הזמנות משאבים והקצאות משימות אינן משולבות באופן הדוק.</span><span class="sxs-lookup"><span data-stu-id="0530e-118">In Project Operations, resource bookings and task assignments aren't tightly coupled.</span></span> <span data-ttu-id="0530e-119">כאשר משתמשים בבורר המשאבים בלוח הזמנים, ניתן להקצות משימות לחברי צוות במספר שעות גדול יותר מכפי שההזמנות שלהם מכסות בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0530e-119">When you use the resource picker in the schedule, you can assign tasks to team members for more hours than their bookings cover on the project.</span></span>

<span data-ttu-id="0530e-120">ההבדלים בין ההזמנות והמטלות של חברי הצוות מוצגים בכרטיסיות **צוות** ו**התאמה משאבים**.</span><span class="sxs-lookup"><span data-stu-id="0530e-120">The differences between team member bookings and assignments are shown on the **Team** and **Resource Reconciliation** tabs.</span></span> <span data-ttu-id="0530e-121">ניתן גם ליישב את ההבדלים שבין הזמנות והקצאות של משאבים ברמה מפורטת יותר.</span><span class="sxs-lookup"><span data-stu-id="0530e-121">You can also reconcile the differences between bookings and assignments for resources at a more detailed level.</span></span>

<span data-ttu-id="0530e-122">השתמש בבורר המשאבים בכרטיסיה **לוח זמנים** כדי לחפש ולבחור משאבים הניתנים להזמנה שאינם עדיין חלק מצוות הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0530e-122">Use the resource picker on the **Schedule** tab to search for and select bookable resources that are not already part of the project team.</span></span> <span data-ttu-id="0530e-123">משאבים אלה מוצגים בבורר המשאבים כ**משאבים אחרים**.</span><span class="sxs-lookup"><span data-stu-id="0530e-123">These resources are shown in the resource picker as **Other Resources**.</span></span>

<span data-ttu-id="0530e-124">כאשר אתה בחור משאב, המשאב מתווסף לצוות הפרוייקט ומוקצה למשימה, אבל לא נוצרות הזמנות.</span><span class="sxs-lookup"><span data-stu-id="0530e-124">When you make a selection, the resource is added to the project team and assigned to the task, but no bookings are generated.</span></span>

<span data-ttu-id="0530e-125">באפשרותך להשתמש ביכולת הארכת ההזמנה של הכרטיסיה  **פיוס** או ב**לוח זמנים** כדי להזמין את קיבולת המשאב לפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0530e-125">You can use the **Reconciliation** tab’s extend booking capability or the **Schedule Board** to book the resource’s capacity to the project.</span></span>

<span data-ttu-id="0530e-126">לאחר שחבר צוות הוזמן בפרוייקט, ניתן להשתמש באפשרות **השאר הזמנות** או  להשתמש ב**לוח הזמנים** ישירות כדי לנהל את ההזמנות שלו.</span><span class="sxs-lookup"><span data-stu-id="0530e-126">After a team member is booked on your project, you can use **Maintain bookings** or the **Schedule Board** directly to manage their bookings.</span></span>