---
title: כיצד אני מבצע ‏‫הזמנה טנטטיבית‬‬ של משאבים בגירסת יישום 2.x?
description: מאמר זה מתאר כיצד לבצע הזמנה טנטטיבית של חברי צוות הפרוייקט באמצעות Project Service.
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 9e5d1c91f8ea98117583996552c2f2834be9c537
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077331"
---
# <a name="how-do-i-soft-book-resources-in-the-web-app-project-service-app-v2x"></a><span data-ttu-id="12195-103">כיצד אני מבצע ‏‫הזמנה טנטטיבית‬‬ של משאבים ביישום אינטרנט (Project Service גירסת יישום 2.x)?</span><span class="sxs-lookup"><span data-stu-id="12195-103">How do I "soft book" resources in the web app (Project Service app v2.x)?</span></span>

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="12195-104">באפשרותך לתזמן באופן טנטטיבי או לבצע 'הזמנה טנטטיבית' של משאב אל צוות הפרוייקט כדי להראות את כוונתך להקצות את המשאב בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="12195-104">You can tentatively schedule or "soft book" a resource onto a project team to show you plan to assign the resource to a project.</span></span> <span data-ttu-id="12195-105">הזמנות טנטטיביות לא צורכות קיבולת זמינה של משאב.</span><span class="sxs-lookup"><span data-stu-id="12195-105">Soft bookings don’t consume a resource’s available capacity.</span></span> <span data-ttu-id="12195-106">אין אפשרות להקצות חברי צוות שהוזמנו בהזמנה טנטטיבית למשימות פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="12195-106">Soft-booked team members can’t be assigned to project tasks.</span></span> <span data-ttu-id="12195-107">ניתן להקצות למשימות רק משאבים במצב 'הזמנה בטוחה' וסוג ביצוע 'מוקצה' (בהנחה שיש להם מספיק שעות הזמנה בטוחה כדי לכסות את מאמץ ההקצאה).</span><span class="sxs-lookup"><span data-stu-id="12195-107">Only resources with the Status Hard Booked and Commit Type Committed can be assigned to tasks (assuming they have enough hard booking hours to cover the assignment effort).</span></span>

<span data-ttu-id="12195-108">חברי צוות הפרוייקט שהוזמנו בהזמנה טנטטיבית מופיעים ברשת חברי צוות עם שעות ההזמנה הטנטטיבית שלהם שמוצגות בעמודה 'הזמנה טנטטיבית'.</span><span class="sxs-lookup"><span data-stu-id="12195-108">Soft-booked project team members show up in the Team Member grid with their soft-booked hours shown in the Soft Book column.</span></span> <span data-ttu-id="12195-109">הם מופיעים גם בלוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="12195-109">They also show up on the schedule board.</span></span> <span data-ttu-id="12195-110">שוב, הם לא מציינים אף צריכה של קיבולת מפני שהזמנה טנטטיבית לא צורכת את הקיבולת של משאב.</span><span class="sxs-lookup"><span data-stu-id="12195-110">Again, they don’t indicate any consumption of capacity as soft-booking doesn’t consume capacity of a resource.</span></span>

<span data-ttu-id="12195-111">קיימות שלוש דרכים לבצע הזמנה טנטטיבית של חבר צוות לפרוייקט באמצעות Project Service גירסה 2. x.</span><span class="sxs-lookup"><span data-stu-id="12195-111">There are three ways to soft-book a team member onto a project with Project Service version 2.x.</span></span> <span data-ttu-id="12195-112">באפשרותך לבצע הזמנה טנטטיבית דרך לוח הזמנים, להשתמש בתכונה 'שמור הזמנות', או על ידי יצירת משאב כללי.</span><span class="sxs-lookup"><span data-stu-id="12195-112">You can soft-book with the schedule board, use the Maintain Bookings feature, or by creating a generic resource.</span></span> <span data-ttu-id="12195-113">שיטות אלה מתוארות להלן.</span><span class="sxs-lookup"><span data-stu-id="12195-113">These methods are described below.</span></span>

## <a name="soft-book-with-the-schedule-board"></a><span data-ttu-id="12195-114">הזמנה טנטטיבית דרך לוח הזמנים</span><span class="sxs-lookup"><span data-stu-id="12195-114">Soft-book with the schedule board</span></span>

<span data-ttu-id="12195-115">לביצוע הזמנה טנטטיבית דרך לוח הזמנים, בצע את ההליך הבא:</span><span class="sxs-lookup"><span data-stu-id="12195-115">To soft-book with the schedule board, follow this procedure:</span></span> 
1. <span data-ttu-id="12195-116">פתח את לוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="12195-116">Open the schedule board.</span></span>
2. <span data-ttu-id="12195-117">בחר את הכרטיסיה 'פרוייקט' בתחתית החלון 'דרישות משאבים' של לוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="12195-117">Select the Project tab on the bottom Booking Requirements panel of the schedule board.</span></span>
3. <span data-ttu-id="12195-118">חפש את הפרוייקט שברצונך לבצע הזמנה טנטטיבית של משאב עבורו.</span><span class="sxs-lookup"><span data-stu-id="12195-118">Find the project you wish to soft-book a resource on.</span></span> <span data-ttu-id="12195-119">אם יש לך פרוייקטים רבים, לחץ על כותרת העמודה 'פרוייקט' ולאחר מכן השתמש במסנן כדי למצוא את הפרוייקט שלך.</span><span class="sxs-lookup"><span data-stu-id="12195-119">If you have many projects, click on the Project column header and then use the filter to find your project.</span></span>
4. <span data-ttu-id="12195-120">לחץ על הפרוייקט, ולאחר מכן גרור ושחרר אותו ברשת הזמנים של משאב.</span><span class="sxs-lookup"><span data-stu-id="12195-120">Click on the project, then drag and drop it on the resource’s time grid.</span></span>
5. <span data-ttu-id="12195-121">פעולה זו פותחת את החלונית 'צור הזמנת משאבים' בצד ימין.</span><span class="sxs-lookup"><span data-stu-id="12195-121">This opens the Create Resource Booking panel on the right.</span></span> <span data-ttu-id="12195-122">התאם את תאריכי ההתחלה והסיום, בחר במצב הזמנה 'הזמנה טנטטיבית' והגדר את השעות.</span><span class="sxs-lookup"><span data-stu-id="12195-122">Adjust the start and end date, select the Booking Status as Soft and set the hours.</span></span> 
6. <span data-ttu-id="12195-123">לחץ על הזמנה.</span><span class="sxs-lookup"><span data-stu-id="12195-123">Click Book.</span></span>
7. <span data-ttu-id="12195-124">בפרוייקט, המשאב יוצג כעת בתור חבר צוות עם שעות ההזמנה הטנטטיבית בעמודה 'הזמנה טנטטיבית'.</span><span class="sxs-lookup"><span data-stu-id="12195-124">Back on the project, the resource will now show as a team member with the soft booked hours in the Soft Book column.</span></span>

<span data-ttu-id="12195-125">שים לב שאתה לא יכול להקצות אותו למשימות במבנה התפלגות עבודה (WBS) מפני שמשאבים חייבים להיות מוזמנים בהזמנה בטוחה אל הצוות כדי שניתן יהיה להקצות אותם.</span><span class="sxs-lookup"><span data-stu-id="12195-125">Note that you can’t assign them to tasks on the work breakdown structure (WBS) as resources must be hard booked on the team to be assigned.</span></span>

## <a name="soft-book-using-the-maintain-bookings-feature"></a><span data-ttu-id="12195-126">הזמנה טנטטיבית באמצעות תכונת שמירת ההזמנות</span><span class="sxs-lookup"><span data-stu-id="12195-126">Soft-book using the Maintain Bookings feature</span></span>

<span data-ttu-id="12195-127">לביצוע הזמנה טנטטיבית באמצעות התכונה 'שמור הזמנות', בצע את ההליך הבא:</span><span class="sxs-lookup"><span data-stu-id="12195-127">To soft-book with Maintain Bookings follow this procedure:</span></span>
1. <span data-ttu-id="12195-128">מרשת חברי הצוות, לחץ על חדש.</span><span class="sxs-lookup"><span data-stu-id="12195-128">From the team member grid, Click New.</span></span>
2. <span data-ttu-id="12195-129">בחר את המשאב הניתן להזמנה, תפקיד, מ-/עד.</span><span class="sxs-lookup"><span data-stu-id="12195-129">Select the bookable resource, role, from/to.</span></span>
3. <span data-ttu-id="12195-130">בחר שיטת הקצאה שאינה 'ללא':</span><span class="sxs-lookup"><span data-stu-id="12195-130">Select an allocation method other than None:</span></span>
- <span data-ttu-id="12195-131">קיבולת מלאה</span><span class="sxs-lookup"><span data-stu-id="12195-131">Full Capacity</span></span>
- <span data-ttu-id="12195-132">קיבולת באחוזים</span><span class="sxs-lookup"><span data-stu-id="12195-132">Percentage Capacity</span></span>
- <span data-ttu-id="12195-133">לפי שעות - הפץ באופן שווה</span><span class="sxs-lookup"><span data-stu-id="12195-133">By Hours Distribute Evenly</span></span>
- <span data-ttu-id="12195-134">לפי שעות - עומס חזיתי</span><span class="sxs-lookup"><span data-stu-id="12195-134">By Hours Front Load</span></span>
4. <span data-ttu-id="12195-135">לחץ על שמור.</span><span class="sxs-lookup"><span data-stu-id="12195-135">Click Save.</span></span> <span data-ttu-id="12195-136">תראה את המשאב ברשת הצוות ואת השעות שלו במצב 'בטוח'.</span><span class="sxs-lookup"><span data-stu-id="12195-136">You’ll see the resource on the team grid and their hours indicated as Hard.</span></span>
5. <span data-ttu-id="12195-137">שמור את הזמנות המשאב על-ידי לחיצה על 'שמור הזמנות'.</span><span class="sxs-lookup"><span data-stu-id="12195-137">Maintain the resource’s bookings by clicking Maintain Bookings.</span></span>
6. <span data-ttu-id="12195-138">כאשר נפתח לוח הזמנים, הרחב את המשאב כדי להציג את ההזמנות שלו.</span><span class="sxs-lookup"><span data-stu-id="12195-138">When the schedule board opens, expand the resource to show their bookings.</span></span> <span data-ttu-id="12195-139">תראה את ההזמנה במצב 'בטוח'.</span><span class="sxs-lookup"><span data-stu-id="12195-139">You will see the booking indicated as Hard.</span></span>
7. <span data-ttu-id="12195-140">לחץ לחיצה ימנית על ההזמנה, תחת 'שינוי מצב', בחר 'הזמנה טנטטיבית' ואז 'טנטטיבית'.</span><span class="sxs-lookup"><span data-stu-id="12195-140">Right-click the booking, under Change Status, select Soft Book and then Soft.</span></span> <span data-ttu-id="12195-141">מצב ההזמנה הוא כעת 'טנטטיבית'.</span><span class="sxs-lookup"><span data-stu-id="12195-141">The booking status is now Soft.</span></span>
8. <span data-ttu-id="12195-142">לאחר סגירת לוח הזמנים, תראה שהשעות עבור המשאב השתנו מ'בטוח' ל'טנטטיבי' ברשת חברי הצוות.</span><span class="sxs-lookup"><span data-stu-id="12195-142">After closing the schedule board, you’ll see that the hours for the resource have changed from Hard to Soft on the team member grid.</span></span>
<span data-ttu-id="12195-143">שים לב כי אם אתה מזמין משאב אל הצוות בהזמנה בטוחה, ולאחר מכן מקצה לו משימות ב- WBS, בעת שימוש בתכונה 'שמור הזמנות' כדי לשנות את המצב מ'בטוח' ל'טנטטיבי', זה יסיר את ההקצאות מהמשימות עבור משאב זה, מפני שניתן להקצות רק משאבים בהזמנה בטוחה למשימות.</span><span class="sxs-lookup"><span data-stu-id="12195-143">Note that if you hard book a resource onto the team and then assign them tasks in the WBS, when you use maintain bookings to change the status of Hard to Soft, it will remove the assignments from the tasks for that resource, as only hard booked resources can be assigned to tasks.</span></span>

## <a name="soft-book-by-creating-a-generic-resource"></a><span data-ttu-id="12195-144">הזמנה טנטטיבית על-ידי יצירת משאב כללי</span><span class="sxs-lookup"><span data-stu-id="12195-144">Soft-book by creating a generic resource</span></span>

<span data-ttu-id="12195-145">באפשרותך ליצור הזמנה טנטטיבית על-ידי יצירת חבר צוות משאב כללי, שתואם את לוח הזמנים או דרישת משאבים, ושינוי הסוג במהלך ההזמנה.</span><span class="sxs-lookup"><span data-stu-id="12195-145">You can create a soft-booking by generating a generic resource team member, fulfilling with schedule board or Resource Request and changing the type during the booking.</span></span>
<span data-ttu-id="12195-146">לשם כך, בצע את ההליך הבא:</span><span class="sxs-lookup"><span data-stu-id="12195-146">To do this, use the following procedure:</span></span>

1. <span data-ttu-id="12195-147">ב- WBS של פרוייקט, הקצה תפקידים למשימות שברצונך ליצור עבורן חברי צוות כלליים.</span><span class="sxs-lookup"><span data-stu-id="12195-147">On the project WBS, assign roles to the tasks you wish to generate generic team members for.</span></span>
2. <span data-ttu-id="12195-148">לחץ על 'צור צוות פרוייקט'.</span><span class="sxs-lookup"><span data-stu-id="12195-148">Click Generate Project Team.</span></span>
3. <span data-ttu-id="12195-149">ברשת חברי צוות הפרוייקט, בחר במשאב הכללי ולחץ על 'הזמנה'.</span><span class="sxs-lookup"><span data-stu-id="12195-149">On the project team member grid, select the generic resource and click Book.</span></span>
4. <span data-ttu-id="12195-150">בלוח הזמנים, בחר את המשאב שברצונך להזמין.</span><span class="sxs-lookup"><span data-stu-id="12195-150">On the schedule board, select the resource that you wish to book.</span></span>
5. <span data-ttu-id="12195-151">בחלונית 'צור הזמנת משאבים' של לוח הזמנים, שנה את מצב ההזמנה ל'טנטטיבית'.</span><span class="sxs-lookup"><span data-stu-id="12195-151">On the schedule board’s Create Resource Booking panel, change the Booking Status to Soft.</span></span>
6. <span data-ttu-id="12195-152">לחץ על 'הזמנה' או 'הזמנה ויציאה'.</span><span class="sxs-lookup"><span data-stu-id="12195-152">Click Book or Book and Exit.</span></span>

<span data-ttu-id="12195-153">לאחר סגירת לוח הזמנים, תראה שהמשאב הנבחר התווסף לצוות עם שעות ההזמנה הטנטטיבית והשעות המוקצות.</span><span class="sxs-lookup"><span data-stu-id="12195-153">After closing the schedule board, you’ll see the selected resource added to the team with Soft booked hours as well as assigned hours.</span></span> <span data-ttu-id="12195-154">תראה גם שהמשאב נכללי נשאר בצוות כמחוון לכך שהמשימות מוקצות לחבר צוות בהזמנה טנטטיבית.</span><span class="sxs-lookup"><span data-stu-id="12195-154">You’ll also see that the generic resource remains on the team as an indicator that the tasks are assigned to a soft-booked team member.</span></span>

<span data-ttu-id="12195-155">כאשר תהיה מוכן לשנות משאב חבר צוות בהזמנה טנטטיבית לחבר צוות בהזמנה בטוחה כדי שניתן יהיה להקצות לו משימות, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="12195-155">When you’re ready to change a soft-booked team member resource to a hard-booked team member so that you can assign them to tasks, do the following:</span></span>

1. <span data-ttu-id="12195-156">בחר את המשאב ולחץ על 'שמור הזמנות'.</span><span class="sxs-lookup"><span data-stu-id="12195-156">Select that resource and click Maintain Bookings.</span></span>
2. <span data-ttu-id="12195-157">כאשר נפתח לוח הזמנים, הרחב את המשאב כדי להציג את ההזמנות שלו.</span><span class="sxs-lookup"><span data-stu-id="12195-157">When the schedule board opens, expand the resource to show their bookings.</span></span> <span data-ttu-id="12195-158">תראה שההזמנה מסומנת בתור 'טנטטיבית'.</span><span class="sxs-lookup"><span data-stu-id="12195-158">You’ll see the booking marked as Soft.</span></span>
3. <span data-ttu-id="12195-159">לחץ לחיצה ימנית על ההזמנה, תחת 'שינוי מצב', בחר 'הזמנה בטוחה' ואז 'בטוחה'.</span><span class="sxs-lookup"><span data-stu-id="12195-159">Right-click the booking, under Change Status, select Hard Book and then Hard.</span></span> <span data-ttu-id="12195-160">מצב ההזמנה הוא כעת 'בטוחה'.</span><span class="sxs-lookup"><span data-stu-id="12195-160">The booking status is now Hard.</span></span>
4. <span data-ttu-id="12195-161">לאחר סגירת לוח הזמנים, תראה שהשעות עבור המשאב השתנו מ'טנטטיבי' ל'בטוח' ברשת חברי הצוות.</span><span class="sxs-lookup"><span data-stu-id="12195-161">After closing the schedule board, you’ll see that the hours for the resource have changed from Soft to Hard on the team member grid.</span></span> <span data-ttu-id="12195-162">כעת, אתה יכול להקצות את המשאב למשימות (בתנאי שיש התאמה בין השעות בהזמנה בטוחה ושעות המאמץ של המשימה להקצאה).</span><span class="sxs-lookup"><span data-stu-id="12195-162">You may now assign the resource to tasks (provided there is alignment between the hard-booked hours and the effort hours of the task for assignment).</span></span> <span data-ttu-id="12195-163">שים לב כי אם ביצעת את השלבים למימוש משאב כללי בפריט #3 לעיל, כאשר תשנה את המצב של המשאב הניתן להזמנה שהוזמן בהזמנה טנטטיבית למצב של הזמנה בטוחה, חבר הצוות כללי יוסר מהצוות.</span><span class="sxs-lookup"><span data-stu-id="12195-163">Note that if you followed the generic resource fulfilment steps in item #3 above, when you change the status of the soft-booked bookable resource to hard, the generic team member is removed from the team.</span></span>
