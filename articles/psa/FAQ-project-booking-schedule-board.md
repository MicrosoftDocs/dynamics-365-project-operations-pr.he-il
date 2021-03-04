---
title: יצירת הזמנת משאבים בפרוייקט מלוח הזמנים
description: נושא זה מספק מידע אודות אופן היצירה של הזמנת פרוייקט מלוח הזמנים.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
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
ms.openlocfilehash: 7032af78168c742ac64cb2a7174cabcbda579ff8
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5146529"
---
# <a name="create-a-project-booking-from-the-schedule-board"></a><span data-ttu-id="f1ea2-103">יצירת הזמנת משאבים בפרוייקט מלוח הזמנים</span><span class="sxs-lookup"><span data-stu-id="f1ea2-103">Create a project booking from the Schedule board</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="f1ea2-104">באפשרותך להזמין משאב אל פרוייקט ישירות מהכרטיסיה **צוות** של הפרוייקט או על-ידי יצירת דרישת משאב מתוך הקצאת חבר צוות כללי, ולאחר מכן מימוש הדרישה שנוצרה עם חבר צוות הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-104">You can book a resource onto a project directly from the **Team** tab of the project or by generating a resource requirement from a generic team member assignment and then fulfilling the generated requirement with a project team member.</span></span>

<span data-ttu-id="f1ea2-105">באפשרותך גם להזמין משאב אל פרוייקט ישירות מלוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-105">You can also book a resource onto a project directly from the Schedule board.</span></span> <span data-ttu-id="f1ea2-106">ישנן שלוש דרכים לעשות זאת:</span><span class="sxs-lookup"><span data-stu-id="f1ea2-106">There are three ways to do this:</span></span>

- <span data-ttu-id="f1ea2-107">**הזמנה מתוך דרישת משאב שנוצרה:** באפשרותך ליצור דרישת משאב לאחר יצירת משאב כללי והקצאת משימות בתוך פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-107">**Book from a generated resource requirement:** You can generate a resource requirement after you create a generic resource and assign tasks within a project.</span></span>

- <span data-ttu-id="f1ea2-108">**הזמנה מתוך הדרישה הראשית:** הדרישות הראשיות מופיעות בלוח הזמנים בכרטיסיה **פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-108">**Book from the primary requirement:** The primary requirements show up on the Schedule board on the **Project** tab.</span></span> 

- <span data-ttu-id="f1ea2-109">**הזמנה מתוך דרישת משאב חדשה** : באפשרותך ליצור דרישת משאב מאפס ולשייך אותה לפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-109">**Book from a new resource requirement:** You can create a resource requirement from scratch and associate it with a project.</span></span> <span data-ttu-id="f1ea2-110">בלוח הזמנים, דרישת המשאב מופיעה בכרטיסיה **דרישות פתוחות**.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-110">On the Schedule board, the resource requirement shows up on the **Open Requirements** tab.</span></span>

## <a name="book-from-a-generated-resource-requirement"></a><span data-ttu-id="f1ea2-111">הזמנה מתוך דרישת משאב שנוצרה</span><span class="sxs-lookup"><span data-stu-id="f1ea2-111">Book from a generated resource requirement</span></span>

<span data-ttu-id="f1ea2-112">באפשרותך ליצור משאב כללי ולהקצות אותו למשימה אחת או יותר בתוך פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-112">You can create a generic resource and assign it one or more tasks within a project.</span></span> <span data-ttu-id="f1ea2-113">לאחר מכן באפשרותך ליצור דרישת משאב מתוך חבר הצוות הכללי.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-113">Then you can generate a resource requirement from the generic team member.</span></span> 

1.  <span data-ttu-id="f1ea2-114">בלוח הזמנים, משאב זה יופיע בכרטיסיה **דרישות פתוחות**. ייתכן שיהיה עליך להשתמש במסנני עמודה ברשת אם יש לך דרישות פתוחות רבות.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-114">On the Schedule board, this resource will show up on the **Open Requirements** tab. You might need to use column filters on the grid if you have many open requirements.</span></span> 

    <span data-ttu-id="f1ea2-115">![פתח את כרטיסיית הדרישות בלוח הזמנים](media/FAQ-Project-Booking-Schedule-Board-1.png "צילום מסך של טבלת הזמנות והקצאות")</span><span class="sxs-lookup"><span data-stu-id="f1ea2-115">![Open Requirements tab on the Schedule board](media/FAQ-Project-Booking-Schedule-Board-1.png "Screenshot of bookings and assignments table")</span></span>

2. <span data-ttu-id="f1ea2-116">בחר את הדרישה.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-116">Select the requirement.</span></span> <span data-ttu-id="f1ea2-117">הכרטיסיה **חפש זמינות** תופיע בחלק העליון של השורה הנבחרת.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-117">The **Find Availability** tab will appear at the top of the selected row.</span></span>
 
3. <span data-ttu-id="f1ea2-118">כאשר תבחר את הכרטיסיה, מצב מסייע לוח הזמנים של לוח הזמנים ייפתח ולאחר מכן יסנן את המשאבים הזמינים העונים על דרישת המשאבים.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-118">When you select the tab, the Schedule Assistant mode of the Schedule board opens and then filters the available resources that meet the resource requirement.</span></span> <span data-ttu-id="f1ea2-119">לאחר מכן, ניתן להזמין משאב.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-119">After that, you can book a resource.</span></span>

4. <span data-ttu-id="f1ea2-120">באפשרותך גם לגרור ולשחרר את השורה הנבחרת מהחלק התחתון של לוח הזמנים לתא משאב ברשת לעיל.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-120">You can also drag and drop the selected row from the bottom of the Schedule board to a resource cell in the grid above.</span></span> <span data-ttu-id="f1ea2-121">כאשר אתה משחרר אותה, נפתחת חלונית **צור הזמנת משאבים** בצד ימין.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-121">When you drop it, it opens the **Create Resource Booking** panel on the right.</span></span>

    <span data-ttu-id="f1ea2-122">בחירה באפשרות **הזמנה** מזמינה את המשאב אל צוות הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-122">Selecting **Book** books the resource onto the project team.</span></span>

![לוח 'צור הזמנת משאבים'](media/FAQ-Project-Booking-Schedule-Board-6.png "")
 

## <a name="book-from-the-primary-requirement"></a><span data-ttu-id="f1ea2-124">הזמנה מתוך הדרישה הראשית</span><span class="sxs-lookup"><span data-stu-id="f1ea2-124">Book from the Primary Requirement</span></span>

<span data-ttu-id="f1ea2-125">יצירת פרוייקט ב- Project Service באופן אוטומטי יוצרת דרישת משאב הנקראת דרישה ראשית.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-125">Creating a project in Project Service automatically creates a resource requirement called the Primary Requirement.</span></span> <span data-ttu-id="f1ea2-126">זוהי דרישה ריקה המשמשת להזמנה מהירה של משאב באמצעות לוח הזמנים ללא ניפוק דרישה או יצירת דרישה מן היסוד.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-126">This is an empty requirement that is used to quickly book a resource with the Schedule board without generating a requirement or creating one from scratch.</span></span> <span data-ttu-id="f1ea2-127">מאחר שהדרישה ריקה, יהיה עליך לציין תאריכים ואת שיטת ההקצאה והשעות אם רלוונטי.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-127">Because the requirement is empty, you’ll need to specify dates as well as the allocation method and hours, if applicable.</span></span> 

1. <span data-ttu-id="f1ea2-128">להזמנת משאב דרך הדרישה הראשית, בלוח הזמנים בחר בכרטיסיה **פרוייקט**. אם יש לך פרוייקטים רבים, ייתכן שתצטרך להשתמש במסנני עמודה בעמודה **פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-128">To book a resource with the Primary Requirement, on the Schedule board, select the **Project** tab. You might need to use the column filter on the **Project** column if you have many projects.</span></span>

   <span data-ttu-id="f1ea2-129">![מסננים לעמודות בלוח הזמנים](media/FAQ-Project-Booking-Schedule-Board-2.png "צילום מסך של טבלת הזמנות והקצאות")</span><span class="sxs-lookup"><span data-stu-id="f1ea2-129">![Column filters on the Schedule board](media/FAQ-Project-Booking-Schedule-Board-2.png "Screenshot of bookings and assignments table")</span></span>

2. <span data-ttu-id="f1ea2-130">בחר את הדרישה שיש לה רק את שם הפרוייקט בשמה ומשך זמן של אפס (0).</span><span class="sxs-lookup"><span data-stu-id="f1ea2-130">Select the requirement that only has the project name as its name and has a duration of zero (0).</span></span>

3. <span data-ttu-id="f1ea2-131">בחר בכרטיסיה **חפש זמינות** המופיעה בשורה.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-131">Select the **Find Availability** tab that appears on the row.</span></span> <span data-ttu-id="f1ea2-132">פעולה זו מעבירה את לוח הזמנים למצב מסייע לוח הזמנים ומציגה את המשאבים הזמינים שניתן להזמין אל הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-132">This puts the Schedule board in Schedule Assistant mode and shows the available resources that can be booked onto the project.</span></span>

4. <span data-ttu-id="f1ea2-133">מכיוון ש **דרישה ראשית** היא דרישה ריקה עם משך זמן של אפס (0), יהיה עליך להגדיר את משך הזמן בלוח **צור הזמנת משאבים** בעת בחירה והזמנת משאב.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-133">Because a **Primary Requirement** is an empty requirement with zero (0) duration, you’ll need to set the duration on the **Create Resource Booking** panel when selecting and booking a resource.</span></span>

5. <span data-ttu-id="f1ea2-134">ניתן לבחור גם את **הדרישה הראשית של פרוייקט** בחלק התחתון של לוח הזמנים ולגרור ולשחרר אותה במשאב כדי להזמין אותו.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-134">You can also select the **Project Primary Requirement** at the bottom of the Schedule board and drag and drop it on a resource to book it.</span></span>
 
    <span data-ttu-id="f1ea2-135">מכיוון ש **דרישה ראשית** היא דרישה ריקה עם משך זמן של אפס (0), יהיה עליך להגדיר את משך הזמן בלוח **צור הזמנת משאבים** כאשר תבחר משאב ותזמין אותו.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-135">Because the **Primary Requirement** is an empty requirement that has zero (0) duration, you’ll need to set the duration on the **Create Resource Booking** panel when you select and book a resource.</span></span>
 
    <span data-ttu-id="f1ea2-136">בעת הזמנת משאב באמצעות **הדרישה הראשית** בלוח הזמנים, אתה מוסיף אותה לצוות הפרוייקט ללא כל הקצאות.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-136">When you book a resource through the **Primary Requirement** on the Schedule board, you add it to the project team without any assignments.</span></span>
 
## <a name="book-from-a-new-resource-requirement"></a><span data-ttu-id="f1ea2-137">הזמנה מתוך דרישת משאב חדשה</span><span class="sxs-lookup"><span data-stu-id="f1ea2-137">Book from a new resource requirement</span></span>
<span data-ttu-id="f1ea2-138">בצע את השלבים הבאים כדי להזמין מדרישת משאב חדשה.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-138">Complete the following steps to book from a new resource requirement.</span></span> 

1. <span data-ttu-id="f1ea2-139">עבור אל **דרישות משאבים** ובחר **חדש** כדי ליצור דרישת משאב חדשה.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-139">Go to **Resource Requirements**, and then select **New** to create a new resource requirement.</span></span>

2. <span data-ttu-id="f1ea2-140">בכרטיסיה **פרוייקט**, בחר פרוייקט כדי לשייך את הדרישה לפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-140">On the **Project** tab, select a project to associate the requirement to the project.</span></span>
 
    <span data-ttu-id="f1ea2-141">בלוח הזמנים, הדרישה החדשה מוצגת כ **דרישה פתוחה** שניתן לממש.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-141">On the Schedule board, this new requirement shows as an **Open Requirement** that you can fulfill.</span></span>

3. <span data-ttu-id="f1ea2-142">הזמן את המשאב כדי להוסיף אותו לצוות הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-142">Book the resource to add it to the project team.</span></span>

4. <span data-ttu-id="f1ea2-143">כעת כשהמשאב מוזמן, עליך להקצות משימות באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="f1ea2-143">Now that the resource is booked, you must assign tasks manually.</span></span>

