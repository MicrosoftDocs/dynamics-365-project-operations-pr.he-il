---
title: ניהול משאבים
description: נושא זה מספק מידע אודות אופן ניהול המשאבים.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 05/13/2019
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
ms.openlocfilehash: 5b34ad66750dba9459d551a2527c13111196511e
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077509"
---
# <a name="manage-resources"></a><span data-ttu-id="b34d0-103">ניהול משאבים</span><span class="sxs-lookup"><span data-stu-id="b34d0-103">Manage resources</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="b34d0-104">Dynamics 365 Project Service Automation כולל ‏‫לוח מחוונים של מנהל משאבים‬ שמספק סקירה חזותית של ביקוש משאב וניצול בכל הארגון.</span><span class="sxs-lookup"><span data-stu-id="b34d0-104">Dynamics 365 Project Service Automation includes a resource manager dashboard that provides a visual overview of resource demand and utilization throughout the organization.</span></span> <span data-ttu-id="b34d0-105">תוכל להשתמש בתרשימים בלוח מחוונים זה כדי להציג באופן חזותי את המידע הבא:</span><span class="sxs-lookup"><span data-stu-id="b34d0-105">You can use the charts on this dashboard to visualize the following information:</span></span>

- <span data-ttu-id="b34d0-106">**ביקוש למשאבים** – התרשים **‏‫בקשות למשאבים פעילים‬** מציג משאבים שנשלחו.</span><span class="sxs-lookup"><span data-stu-id="b34d0-106">**Resource demand** – The **Active Resource Request** chart shows resources that have been submitted.</span></span> <span data-ttu-id="b34d0-107">המשאבים מצטברים לפי תפקיד או פרויקט.</span><span class="sxs-lookup"><span data-stu-id="b34d0-107">The resources are aggregated by either role or project.</span></span>
- <span data-ttu-id="b34d0-108">**ביקוש למשאבים שלא נשלח** – התרשים **ביקוש למשאבים שלא הוקצה** מציג את כל הדרישות למשאבים שלא נשלחו.</span><span class="sxs-lookup"><span data-stu-id="b34d0-108">**Unsubmitted resource demand** – The **Unassigned Resource Demand** chart shows all the resource requirements that haven't been submitted.</span></span> <span data-ttu-id="b34d0-109">הוא עוזר למנהלי המשאבים להציג ביקוש שאינו קשיח ועשוי להישלח באמצעות בקשה למשאב.</span><span class="sxs-lookup"><span data-stu-id="b34d0-109">It helps resource managers view demand that isn't firm and might be submitted through a resource request.</span></span>
- <span data-ttu-id="b34d0-110">**ניצול לחיוב עבור השבוע שעבר** – התרשים **ניצול לפי תרשים** מציג את אחוז הניצול לחיוב בפועל של הארגון לפי תפקיד מול יעד הניצול לחיוב לפי תפקיד.</span><span class="sxs-lookup"><span data-stu-id="b34d0-110">**Billable utilization for the past week** – The **Utilization by Role** chart shows the percentage of the organization's actual billable utilization by role against its target billable utilization by role.</span></span>

    > [!NOTE]
    > <span data-ttu-id="b34d0-111">כדי להפוך את התרשים **ניצול לפי תפקיד** לזמין, צור משימה שמפעילה את זרימת העבודה UpdateRoleUtilization.</span><span class="sxs-lookup"><span data-stu-id="b34d0-111">To make the **Utilization by Role** chart available, create a job that runs the UpdateRoleUtilization workflow.</span></span> <span data-ttu-id="b34d0-112">משימה חוזרת זו פועלת כל שבעה ימים כדי לחשב ניצול לחיוב בשבעת הימים הקודמים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-112">This recurring job runs every seven days to calculate billable utilization for the previous seven days.</span></span> <span data-ttu-id="b34d0-113">התוצאות נצברות לפי תפקיד.</span><span class="sxs-lookup"><span data-stu-id="b34d0-113">The results are aggregated by role.</span></span>

## <a name="manage-project-team-members"></a><span data-ttu-id="b34d0-114">ניהול חברי צוות פרויקט</span><span class="sxs-lookup"><span data-stu-id="b34d0-114">Manage project team members</span></span>

<span data-ttu-id="b34d0-115">מנהלי פרויקטים יכולים להשתמש בלוח המחוונים של מנהל המשאבים כדי לנהל את המשאבים בפרויקטים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-115">Project managers can use the resource manager dashboard to manage the resources on projects.</span></span> <span data-ttu-id="b34d0-116">לדוגמה, באפשרותם להוסיף חבר צוות ישירות לפרויקט ולהזמין חבר צוות למלא את דרישות המשאב שנלכדו על-ידי משאב כללי.</span><span class="sxs-lookup"><span data-stu-id="b34d0-116">For example, they can add a team member directly to a project and book a team member to fulfill the resource requirements that were captured by a generic resource.</span></span>

### <a name="add-a-team-member-directly-to-a-project"></a><span data-ttu-id="b34d0-117">הוספת חבר צוות ישירות לפרויקט</span><span class="sxs-lookup"><span data-stu-id="b34d0-117">Add a team member directly to a project</span></span>

<span data-ttu-id="b34d0-118">כדי להוסיף חבר צוות ישירות לפרויקט, בדף **פרויקטים** , בכרטיסיה **צוות** , בחר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-118">To add a team member directly to a project, on the **Projects** page, on the **Team** tab, select **New**.</span></span> <span data-ttu-id="b34d0-119">תיבת הדו-שיח **יצירה מהירה:חבר צוות פרויקט** מופיעה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-119">The **Quick Create:Project Team Member** dialog box appears.</span></span> <span data-ttu-id="b34d0-120">בתיבת דו-שיח זו, באפשרותך לבצע משימות אלו:</span><span class="sxs-lookup"><span data-stu-id="b34d0-120">In this dialog box, you can perform these tasks:</span></span>

- <span data-ttu-id="b34d0-121">**הזמנת משאבל בעל שם** – בשדה **משאב ניתן להזמנה** , בחר את השם של המשאב.</span><span class="sxs-lookup"><span data-stu-id="b34d0-121">**Book a named resource** – In the **Bookable Resource** field, select the name of the resource.</span></span> <span data-ttu-id="b34d0-122">לאחר מכן בחר את התפקיד, קבע את התקופה ובחר שיטת הקצאה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-122">Then select the role, set the period, and select an allocation method.</span></span> <span data-ttu-id="b34d0-123">המשאב בעל השם שבחרת נוסף לפרויקט באמצעות שיטת ההקצאה שנבחרה ולוח השנה של המשאבים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-123">The named resource that you selected is added to the project by using the selected allocation method and the resources calendar.</span></span>
- <span data-ttu-id="b34d0-124">**הוספת משאב כללי** – השאר את השדה **משאב ניתן להזמנה** ריק ולאחר מכן בחר את התפקיד, קבע את התקופה ובחר את שיטת ההקצאה המועדפת.</span><span class="sxs-lookup"><span data-stu-id="b34d0-124">**Add a generic resource** – Leave the **Bookable resource** field blank, and then select the role, set the period, and select the preferred allocation method.</span></span> <span data-ttu-id="b34d0-125">משאב כללי מתווסף לצוות כמציין מיקום כדי לשמור את תבנית הדרישה שמשמשת להזמנת משאבים בעלי שם בצוות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-125">A generic resource is added to the team as a placeholder to hold the demand pattern that is used to book named resources on the team.</span></span> <span data-ttu-id="b34d0-126">הדרישה נעשית בהתאם ללוח השנה של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="b34d0-126">The requirement is made according to the project calendar.</span></span>
- <span data-ttu-id="b34d0-127">**הוספת משאב בעל שם לצוות בלי לצרוך את קיבולת המשאבים** – בשדה **משאב ניתן להזמנה** , בחר משאב.</span><span class="sxs-lookup"><span data-stu-id="b34d0-127">**Add a named resource to the team without consuming resource capacity** – In the **Bookable Resource** field, select a resource.</span></span> <span data-ttu-id="b34d0-128">לאחר מכן בחר את התקופה ובחר **ללא** כשיטת ההקצאה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-128">Then select the period, and select **None** as the allocation method.</span></span> <span data-ttu-id="b34d0-129">המשאב מתווסף לצוות, אך הקיבולת של המשאב אינה נצרכת באמצעות הזמנה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-129">The resource is added to the team, but the resource's capacity isn't consumed through a booking.</span></span>

### <a name="book-a-team-member-to-fulfill-resource-requirements-for-a-generic-resource"></a><span data-ttu-id="b34d0-130">הזמנת חבר צוות למימוש דרישות משאב עבור משאב כללי</span><span class="sxs-lookup"><span data-stu-id="b34d0-130">Book a team member to fulfill resource requirements for a generic resource</span></span>

<span data-ttu-id="b34d0-131">ב- PSA, באפשרותך להזמין משאב כללי בצוות פרויקט ולציין את התפקיד, את הקיבולת הדרושה ואת אופן הפצת הקיבולת.</span><span class="sxs-lookup"><span data-stu-id="b34d0-131">In PSA, you can book a generic resource on a project team, and can specify the role, the required capacity, and how that capacity is distributed.</span></span> <span data-ttu-id="b34d0-132">בדרישת המשאב, תוכל לציין תכונות המשויכות למשאב הכללי.</span><span class="sxs-lookup"><span data-stu-id="b34d0-132">On the resource requirement, you can specify attributes that are associated with the generic resource.</span></span> <span data-ttu-id="b34d0-133">תכונות אלה כוללות כישורים נדרשים, היחידה הארגונית המועדפת ומשאבים מועדפים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-133">These attributes include required skills, the preferred organizational unit, and preferred resources.</span></span>

<span data-ttu-id="b34d0-134">בצע את השלבים הבאים כדי לציין את הכישורים הנדרשים במשאב כללי עבור מפתח.</span><span class="sxs-lookup"><span data-stu-id="b34d0-134">Follow these steps to specify required skills on a generic resource for a developer.</span></span>

1. <span data-ttu-id="b34d0-135">בדף **פרויקטים** , בכרטיסיה **צוות** , בחר **חדש** כדי להזמין משאב כללי.</span><span class="sxs-lookup"><span data-stu-id="b34d0-135">On the **Projects** page, on the **Team** tab, select **New** to book a generic resource.</span></span>

    ![משאב כללי הוזמן בצוות](media/Resource-Management-image9.png)

2. <span data-ttu-id="b34d0-137">בתצוגה **כל חברי הצוות** , בעמודה **דרישת משאב** , בחר את הקישור כדי להוסיף כישורים נדרשים עבור המשאב הכללי.</span><span class="sxs-lookup"><span data-stu-id="b34d0-137">In the **All Team Members** view, in the **Resource Requirement** column, select the link to add required skills for the generic resource.</span></span>

    ![קישור לדרישה](media/Resource-Management-image10.png)

3. <span data-ttu-id="b34d0-139">בדף **דרישת משאב** שמופיע, ברשת **כישורים** , בחר את שלושת הנקודות ( **...** ) ולאחר מכן בחר **הוסף מאפיין דרישה חדש** כדי להוסיף את הכישורים הנדרשים עבור המפתח שלך.</span><span class="sxs-lookup"><span data-stu-id="b34d0-139">On the **Resource Requirement** page that appears, in the **Skills** grid, select the ellipsis ( **...** ) and then select **Add New Requirement Characteristic** to add the required skills for your developer.</span></span>

    ![הוספת פקודה חדשה של מאפיין דרישה](media/Resource-Management-image11.png)

4. <span data-ttu-id="b34d0-141">בתיבת הדו-שיח **יצירה מהירה: מאפיין דרישה** שמופיעה, בשדה **מאפיין** , בחר את הכישורים הנדרשים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-141">In the **Quick Create: Requirement Characteristic** dialog box that appears, in the **Characteristic** field, select the required skill.</span></span> <span data-ttu-id="b34d0-142">לאחר מכן, בשדה **‏‫ערך דירוג‬** , בחר את רמת המומחיות עבור הכישורים האלו.</span><span class="sxs-lookup"><span data-stu-id="b34d0-142">Then, in the **Rating value** field, select the proficiency level for that skill.</span></span> <span data-ttu-id="b34d0-143">לבסוף, בשדה **דרישת משאב** , קבע את הדרישה למשאבי המקור מהיחידות הארגוניות או אפילו משאבים בעלי שם.</span><span class="sxs-lookup"><span data-stu-id="b34d0-143">Finally, in the **Resource Requirement** field, set the requirement to source resources from organizational units or even named resources.</span></span> <span data-ttu-id="b34d0-144">לאחר שתסיים, בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-144">When you've finished, select **Save**.</span></span>

    ![תיבת הדו-שיח 'יצירה מהירה: מאפיין דרישה'](media/Resource-Management-image12.png)

5. <span data-ttu-id="b34d0-146">בדף **דרישת משאב** , בחר **הזמן** כדי לממש את דרישת המשאב.</span><span class="sxs-lookup"><span data-stu-id="b34d0-146">On the **Resource Requirement** page, select **Book** to fulfill the resource requirement.</span></span>

    ![לחצן 'הזמן' בדף 'דרישת משאב'](media/Resource-Management-image13.png)

    <span data-ttu-id="b34d0-148">תוכל גם לבחור את המשאב הכללי ברשת **כל חברי הצוות** ולאחר מכן בחר **הזמן**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-148">You can also select the generic resource in the **All Team Members** grid and then select **Book**.</span></span>

    ![לחצן 'הזמן' מעל הרשת 'כל חברי הצוות'](media/Resource-Management-image14.png)

    > [!NOTE]
    > <span data-ttu-id="b34d0-150">בדוגמה זו, יש 40 שעות נדרשות, אך ללא שעות שהוזמנו בפועל, מכיוון שלמשאבים כלליים אין הזמנות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-150">In this example, there are 40 required hours but no actual booked hours, because generic resources don't have bookings.</span></span> <span data-ttu-id="b34d0-151">בנוסף, אין שעות מוקצות, מכיוון שהמשאב הכללי התווסף ישירות לצוות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-151">Additionally, there are no assigned hours, because the generic resource was added directly to the team.</span></span> <span data-ttu-id="b34d0-152">הוא לא התווסף באמצעות הקצאת משימה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-152">It wasn't added by using task assignment.</span></span>

    <span data-ttu-id="b34d0-153">בדף **‬‏‫מסייע לוח הזמנים** , תוכל לסנן משאבים זמינים לפי הדרישות שצוינו בדרישות המשאב.</span><span class="sxs-lookup"><span data-stu-id="b34d0-153">On the **Scheduling Assistant** page, you can filter available resources by the requirements that are specified on the resource requirement.</span></span> <span data-ttu-id="b34d0-154">המשאבים ממוינים בהתאם לפרמטרי המיון המצוינים בלוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-154">Resources are sorted according to the sorting parameters that are specified on the Schedule Board.</span></span>

    ![דף 'מסייע לוח הזמנים'](media/Resource-Management-image15.png)

    <span data-ttu-id="b34d0-156">להלן מספר מסננים שנמצאים לרוב בשימוש:</span><span class="sxs-lookup"><span data-stu-id="b34d0-156">Here are some filters that are often used:</span></span>

    - <span data-ttu-id="b34d0-157">**מאפיינים יחד עם דירוג** – סינון לפי כישורים, אישורים ואיכויות משאב אחרות, בנוסף לדירוגי מומחיות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-157">**Characteristics along with a rating** – Filter by skills, certifications, and other resource qualities, in addition to ratings of proficiency.</span></span>
    - <span data-ttu-id="b34d0-158">**תפקידים** – סינון לפי תפקידים בברירת המחדל המוקצים למשאבים שניתן להזמין.</span><span class="sxs-lookup"><span data-stu-id="b34d0-158">**Roles** – Filter by the default roles that are assigned to bookable resources.</span></span>
    - <span data-ttu-id="b34d0-159">**יחידות ארגוניות** – סינון משאבים הניתנים להזמנה לפי היחידות הארגוניות שאליהן הם מוקצים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-159">**Organizational units** – Filter bookable resources by the organizational units that they are assigned to.</span></span>

6. <span data-ttu-id="b34d0-160">אם אינך מרוצה מהתוצאות של חיפוש הדרישה ההתחלתי, באפשרותך לשנות את קריטריוני הסינון.</span><span class="sxs-lookup"><span data-stu-id="b34d0-160">If you aren't satisfied with the results of the initial requirement search, you can change the filter criteria.</span></span> <span data-ttu-id="b34d0-161">הרחב את החלונית **‏‫סינון תצוגה‬** בצד ימין ולאחר מכן בחר **חיפוש** כדי למצוא משאבים נוספים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-161">Expand the **Filter View** pane on the left, and then select **Search** to find additional resources.</span></span>

    ![חלונית סינון תצוגה](media/Resource-Management-image16.png)

7. <span data-ttu-id="b34d0-163">כדי לשנות את אופן מיון התוצאות, בחר **מיין**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-163">To change how the results are sorted, select **Sort**.</span></span>

    ![הפקודה 'מיין'](media/Resource-Management-image17.png)

8. <span data-ttu-id="b34d0-165">בחר משאבים בהתאם לביקוש שצוין בדרישה, כפי שמצוין בחלק העליון של הרשת.</span><span class="sxs-lookup"><span data-stu-id="b34d0-165">Select resources according to the demand that is specified on the requirement, as indicated at the top of the grid.</span></span> <span data-ttu-id="b34d0-166">תוכל לנקות את בחירת התאים ברשת ולהשאיר את אפשרות קיבולת המשאב פתוחה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-166">You can clear the selection of cells in the grid and leave that resource capacity open.</span></span> <span data-ttu-id="b34d0-167">ניתן לבחור רק משאב אחד בכל פעם כמשאב שהוזמן.</span><span class="sxs-lookup"><span data-stu-id="b34d0-167">Only one resource at a time can be selected as booked.</span></span>

9. <span data-ttu-id="b34d0-168">בחר **הזמן** כדי להזמין את המשאב שנבחר ולהשאיר את לוח הזמנים פתוח, כך שתוכל לבחור משאבים נוספים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-168">Select **Book** to book the selected resource and leave the Schedule Board open, so that you can select additional resources.</span></span> <span data-ttu-id="b34d0-169">לחלופין, בחר **הזמן וצא** כדי להזמין את המשאב שנבחר ולסגור את לוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-169">Alternatively, select **Book & Exit** to book the selected resource and close the Schedule Board.</span></span>

    ![משאב שיש להזמין](media/Resource-Management-image19.png)

    <span data-ttu-id="b34d0-171">תקבל הודעה על שעות שהוזמנו.</span><span class="sxs-lookup"><span data-stu-id="b34d0-171">You receive a notification about booked hours.</span></span> <span data-ttu-id="b34d0-172">מחווני הביקוש יציגו את החלק בדרישת ההזמנה שמומשה ואת החלק שנותר.</span><span class="sxs-lookup"><span data-stu-id="b34d0-172">The demand indicators show how much the booking requirement is satisfied and how much remains.</span></span> <span data-ttu-id="b34d0-173">בנוסף, תוכל לראות את כמות הקיבולת שנצרכה מהמשאב שנבחר.</span><span class="sxs-lookup"><span data-stu-id="b34d0-173">You can also see how much of the selected resource's capacity is consumed.</span></span> <span data-ttu-id="b34d0-174">בחר **הרחב** כדי להציג פרטים נוספים על הזמנות המשאב.</span><span class="sxs-lookup"><span data-stu-id="b34d0-174">Select **Expand** to view more details about resource bookings.</span></span>

9. <span data-ttu-id="b34d0-175">חזור אל התצוגה **כל חברי הצוות**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-175">Return to the **All Team Members** view.</span></span> <span data-ttu-id="b34d0-176">ברשת, שים לב שהמשאב הכללי הוחלף על-ידי המשאב בעל השם, ו- 40 שעות נרשמו כמוזמנות עבור משאב זה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-176">In the grid, notice that the generic resource has been replaced by the named resource, and 40 hours are listed as booked for that resource.</span></span>

    ![רשת מעודכנת של 'כל חברי הצוות'](media/Resource-Management-image20.png)

    > [!NOTE]
    > <span data-ttu-id="b34d0-178">לא מוצגות שעות מוקצות, משום שהן הוזמנו ישירות בצוות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-178">No assigned hours are shown, because they were booked directly on the team.</span></span> <span data-ttu-id="b34d0-179">הן לא הוזמנו באמצעות הקצאת משימה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-179">They weren't booked by using task assignment.</span></span>

## <a name="assign-generic-resources-to-tasks-and-generate-resource-requirements"></a><span data-ttu-id="b34d0-180">הקצאת משאבים כלליים למשימות ויצירת דרישות משאבים</span><span class="sxs-lookup"><span data-stu-id="b34d0-180">Assign generic resources to tasks and generate resource requirements</span></span>

<span data-ttu-id="b34d0-181">ב- PSA, באפשרותך ליצור משימות ולאחר מכן להקצות להן משאבים כלליים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-181">In PSA, you can create tasks and then assign generic resources to them.</span></span> <span data-ttu-id="b34d0-182">בדרך זו, ניתן לייצג את הביקוש למשאב באמצעות מצייני מיקום בזמן שאתה מעריך את לוח הזמנים ואת הצד הפיננסי.</span><span class="sxs-lookup"><span data-stu-id="b34d0-182">In this way, resource demand can be represented by placeholders while you estimate your schedule and financial numbers.</span></span> <span data-ttu-id="b34d0-183">לאחר מכן תוכל ליצור דרישות משאבים עבור המשאבים הכלליים ולממש אותן.</span><span class="sxs-lookup"><span data-stu-id="b34d0-183">You can then generate resource requirements for the generic resources and fulfill them.</span></span>

1. <span data-ttu-id="b34d0-184">בדף **פרויקטים** , בכרטיסיה **לוח זמנים** , בחר **הוסף** כדי ליצור משימה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-184">On the **Projects** page, on the **Schedule** tab, select **Add** to create a task.</span></span>

    ![משימה חדשה נוצרה](media/Resource-Management-image21.png)

2. <span data-ttu-id="b34d0-186">בשדה **משאבים** , בחר את הסמל **בורר המשאבים‬**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-186">In the **Resources** field, select the **Resource Picker** symbol.</span></span> <span data-ttu-id="b34d0-187">בורר המשאבים מופיע ומציג את חברי הצוות הקיימים עבור הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="b34d0-187">The Resource Picker appears and shows existing team members for the project.</span></span>

    ![בורר משאבים](media/Resource-Management-image22.png)

3. <span data-ttu-id="b34d0-189">הזן את השם של המשאב הכללי החדש ולאחר מכן בחר **צור**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-189">Enter the name of the new generic resource, and then select **Create**.</span></span>

    ![השם של משאב כללי חדש הוזן](media/Resource-Management-image23.png)

4. <span data-ttu-id="b34d0-191">בתיבת הדו-שיח **יצירה מהירה: חבר צוות** שמופיעה, בשדה **תפקיד** , בחר את התפקיד עבור המשאב הכללי.</span><span class="sxs-lookup"><span data-stu-id="b34d0-191">In the **Quick Create: Project Team Member** dialog box that appears, in the **Role** field, select the role for the generic resource.</span></span> <span data-ttu-id="b34d0-192">בשדה **‏‫יחידת הקצאת משאבים‬** , בחר את היחידה הארגונית עבור המשאב הכללי.</span><span class="sxs-lookup"><span data-stu-id="b34d0-192">In the **Resourcing Unit** field, select the organizational unit for the generic resource.</span></span> <span data-ttu-id="b34d0-193">לאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-193">Then select **Save**.</span></span>

    ![תיבת הדו-שיח 'יצירה מהירה: חבר צוות פרויקט'](media/Resource-Management-image24.png)

    <span data-ttu-id="b34d0-195">חבר הצוות הכללי מוקצה כעת למשימה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-195">The generic team member is now assigned to the task.</span></span>

    ![חבר צוות כללי מוקצה למשימה](media/Resource-Management-image25.png)

    <span data-ttu-id="b34d0-197">בכרטיסיה **צוות** , תראה את חבר הצוות הכללי החדש.</span><span class="sxs-lookup"><span data-stu-id="b34d0-197">On the **Team** tab, you will see the new generic team member.</span></span> <span data-ttu-id="b34d0-198">שים לב שיש לו שעות מוקצות בלבד.</span><span class="sxs-lookup"><span data-stu-id="b34d0-198">Notice that it has only assigned hours.</span></span> <span data-ttu-id="b34d0-199">שעות אלה הן הסכום של כל המשימות המוקצות לחבר הצוות הכללי.</span><span class="sxs-lookup"><span data-stu-id="b34d0-199">These hours are the sum of all tasks that are assigned to the generic team member.</span></span> <span data-ttu-id="b34d0-200">לחבר הצוות הכללי עדיין אין שעות נדרשות או דרישת משאב.</span><span class="sxs-lookup"><span data-stu-id="b34d0-200">The generic team member doesn't yet have required hours or a resource requirement.</span></span>

    ![חבר צוות כללי בכרטיסיה 'צוות'](media/Resource-Management-image26.png)

5. <span data-ttu-id="b34d0-202">כעת תוכל להקצות את חבר הצוות הכללי למשימות אחרות באמצעות בורר המשאבים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-202">You can now assign the generic team member to other tasks by using the Resource Picker.</span></span>

    ![חבר צוות כללי בבוחר המשאבים](media/Resource-Management-image27.png)

    <span data-ttu-id="b34d0-204">לאחר שתסיים להקצות את המשאב הכללי למשימות, תוכל ליצור דרישת משאב עבור המשאב הכללי.</span><span class="sxs-lookup"><span data-stu-id="b34d0-204">When you've finished assigning the generic resource to tasks, you can generate a resource requirement for the generic resource.</span></span>

5. <span data-ttu-id="b34d0-205">בכרטיסיה **צוות** , בחר את המשאב הכללי ולאחר מכן בחר **צור דרישה**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-205">On the **Team** tab, select the generic resource, and then select **Generate Requirement**.</span></span>

    ![הפקודה 'צור דרישה'](media/Resource-Management-image28.png)

    <span data-ttu-id="b34d0-207">כאשר הדרישה נוצרת, לחבר הצוות הכללי יהיו שעות נדרשות וקישור עבור דרישת המשאב.</span><span class="sxs-lookup"><span data-stu-id="b34d0-207">When the requirement is generated, the generic team member will have required hours and a link for the resource requirement.</span></span>

    ![קישור לדרישת משאב](media/Resource-Management-image29.png)

    <span data-ttu-id="b34d0-209">לאחר שתזמין משאב בעל שם, המשאב הכללי מוסר מהצוות ומוחלף על-ידי המשאב בעל השם.</span><span class="sxs-lookup"><span data-stu-id="b34d0-209">After you book a named resource, the generic resource is removed from the team and replaced by the named resource.</span></span>

    ![משאב כללי מוחלף על-ידי המשאב בעל השם](media/Resource-Management-image30.png)

    <span data-ttu-id="b34d0-211">בכרטיסיה **לוח זמנים** , הקצאות המשאב הכללי מוסרות ומוחלפות על-ידי המשאב בעל השם.</span><span class="sxs-lookup"><span data-stu-id="b34d0-211">On the **Schedule** tab, the generic resource assignments are removed and replaced by the named resource.</span></span>

    ![הקצאות המשאב הכללי מוחלפות על-ידי המשאב בעל השם בכרטיסיה 'לוח זמנים'](media/Resource-Management-image31.png)

    > [!NOTE]
    > <span data-ttu-id="b34d0-213">אופן פעולה זה מתרחש רק כאשר משאב בעל שם מוזמן במלואו עבור דרישת המשאב הכללי.</span><span class="sxs-lookup"><span data-stu-id="b34d0-213">This behavior occurs only when a named resource is fully booked for the generic resource requirement.</span></span> <span data-ttu-id="b34d0-214">כאשר משאב בעל שם מחליף באופן חלקי את דרישת המשאב הכללי או כאשר כמה משאבים בעלי שם מחליפים את דרישת המשאב הכללי, המשאב הכללי נשאר מוקצה למשימה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-214">When either a named resource partially replaces the generic resource requirement or multiple named resources replace the generic resource requirement, the generic resource remains assigned to the task.</span></span>

    <span data-ttu-id="b34d0-215">באיור הבא, משימה של 80 שעות תוכננה להימשך חמישה ימים (16 שעות ביום במהלך חמישה ימי עבודה) והוקצתה למשאב הכללי בשם **פונקציונלי**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-215">In the following illustration, an 80-hour task has been planned for a five-day duration (16 hours per day over five days) and assigned to the generic resource that is named **Functional**.</span></span>

    ![משימה של חמישה ימים, 80 שעות, מוקצית למשאב הכללי 'פונקציונלי'](media/Resource-Management-image32.png)

    <span data-ttu-id="b34d0-217">כאשר אתה יוצר את הדרישה, היא עבור 80 שעות במשך חמישה ימים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-217">When you generate the requirement, it's for 80 hours over five days.</span></span>

    ![דרישה שנוצרה עבור 80 שעות במשך חמישה ימים](media/Resource-Management-image33.png)

    <span data-ttu-id="b34d0-219">מכיוון שמשאבים זמינים פועלים רק שמונה שעות ביום, יש צורך בשני משאבים כדי לממש את הדרישה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-219">Because available resources work only eight hours per day, two resources are needed to fulfill the requirement.</span></span>

    ![משאב שני](media/Resource-Management-image35.png)

    <span data-ttu-id="b34d0-221">בכרטיסיה **צוות** , תוכל כעת לראות שלמשאב הכללי אין שעות נדרשות, אך השעות המוקצות עדיין מופיעות יחד עם שני המשאבים בעלי השם שיממשו את הדרישה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-221">On the **Team** tab, you can now see that the generic resource has no required hours, but the assigned hours still appear together with the two named resources that make up the fulfillment.</span></span>

    ![שני משאבים בעלי שם בכרטיסיה 'צוות'](media/Resource-Management-image36.png)

    <span data-ttu-id="b34d0-223">בכרטיסיה **לוח זמנים** , המשאב הכללי נשאר מוקצה למשימה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-223">On the **Schedule** tab, the generic resource remains assigned to the task.</span></span>

    ![משאבים כלליים בכרטיסיה 'לוח זמנים'](media/Resource-Management-image37.png)

<span data-ttu-id="b34d0-225">PSA לא מקצה את שני המשאבים למשימה, מכיוון שאופן פעולה זה יפיק לוח זמנים פחות צפוי.</span><span class="sxs-lookup"><span data-stu-id="b34d0-225">PSA doesn't assign both resources to the task, because that behavior would produce a less predictable schedule.</span></span> <span data-ttu-id="b34d0-226">בדוגמה פשוטה זו, קל לחלק את השעות באופן שווה בין שני משאבים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-226">In this simple example, it's easy to divide the hours equally between two resources.</span></span> <span data-ttu-id="b34d0-227">עם זאת, בתרחישים מורכבים יותר הכוללים משימות רבות וכמה משאבים, PSA יצטרך להניח הנחות על האופן שבו יש להקצות את ההזמנות המתקבלות עבור כמה משאבים במשימות רבות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-227">However, in more complex scenarios that involve multiple tasks and multiple resources, PSA would have to make assumptions about how it should allocate the bookings that are received for multiple resources across multiple tasks.</span></span>

<span data-ttu-id="b34d0-228">לכן, בתרחישים אלה, מנהל הפרויקט אחראי לניתוח ההזמנות המרובות ולהקצאתן לפי הצורך.</span><span class="sxs-lookup"><span data-stu-id="b34d0-228">Therefore, in these scenarios, the project manager is responsible for parsing the multiple bookings and assigning them as needed.</span></span> <span data-ttu-id="b34d0-229">כדי להקצות את ההזמנות, מנהל הפרויקט מקצה את המשימות מהמשאבים הכלליים אל המשאבים בעלי השם ולאחר מכן משתמש בתצוגה **יישוב** כדי לוודא שההקצאה פועלת עם ההזמנות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-229">To allocate the bookings, the project manager assigns the tasks from the generic resources to the named resources and then uses the **Reconciliation** view to make sure that the allocation works with the bookings.</span></span>

### <a name="edit-a-resource-requirement"></a><span data-ttu-id="b34d0-230">עריכת דרישת משאב</span><span class="sxs-lookup"><span data-stu-id="b34d0-230">Edit a resource requirement</span></span>

<span data-ttu-id="b34d0-231">לאחר שנוצרה דרישת משאב, ייתכן שמנהל הפרויקט או מנהל המשאבים ירצו לערוך את הפרטים כדי למקד את קריטריוני החיפוש כאשר משתמשים בלוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-231">After a resource requirement has been created, a project manager or resource manager might want to edit the details to refine the search criteria when the Schedule Board is used.</span></span> <span data-ttu-id="b34d0-232">כדי לערוך את דרישת המשאב, בצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-232">To edit the resource requirement, follow these steps.</span></span>

1. <span data-ttu-id="b34d0-233">בדף **פרויקטים** , בכרטיסיה **צוות** , בחר את הקישור לדרישה כלשהי במשאב כללי.</span><span class="sxs-lookup"><span data-stu-id="b34d0-233">On the **Projects** page, on the **Team** tab, select the link to any requirement on a generic resource.</span></span>
2. <span data-ttu-id="b34d0-234">בדף **דרישת משאב** שמופיע, תוכל לעדכן כמה תכונות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-234">On the **Resource Requirement** page that appears, you can update several attributes.</span></span> <span data-ttu-id="b34d0-235">להלן מספר דוגמאות:</span><span class="sxs-lookup"><span data-stu-id="b34d0-235">Here are some examples:</span></span>

    - <span data-ttu-id="b34d0-236">שם</span><span class="sxs-lookup"><span data-stu-id="b34d0-236">Name</span></span>
    - <span data-ttu-id="b34d0-237">מתאריך</span><span class="sxs-lookup"><span data-stu-id="b34d0-237">From Date</span></span>
    - <span data-ttu-id="b34d0-238">עד תאריך</span><span class="sxs-lookup"><span data-stu-id="b34d0-238">To Date</span></span>
    - <span data-ttu-id="b34d0-239">משך זמן</span><span class="sxs-lookup"><span data-stu-id="b34d0-239">Duration</span></span>
    - <span data-ttu-id="b34d0-240">סוג משאב</span><span class="sxs-lookup"><span data-stu-id="b34d0-240">Resource Type</span></span>

<span data-ttu-id="b34d0-241">בדף **דרישת משאב** , מנהל הפרויקט או מנהל המשאבים יכולים גם להגדיר את הפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="b34d0-241">On the **Resource Requirement** page, the project manager or resource manager can also define the following information:</span></span>

- <span data-ttu-id="b34d0-242">כישורים</span><span class="sxs-lookup"><span data-stu-id="b34d0-242">Skills</span></span>
- <span data-ttu-id="b34d0-243">תפקידים</span><span class="sxs-lookup"><span data-stu-id="b34d0-243">Roles</span></span>
- <span data-ttu-id="b34d0-244">העדפות משאב</span><span class="sxs-lookup"><span data-stu-id="b34d0-244">Resource preferences</span></span>
- <span data-ttu-id="b34d0-245">יחידה ארגונית מועדפת</span><span class="sxs-lookup"><span data-stu-id="b34d0-245">Preferred organizational unit</span></span>

### <a name="update-resource-bookings-after-they-are-booked-on-a-project"></a><span data-ttu-id="b34d0-246">עדכון הזמנות משאבים לאחר הזמנתם בפרויקט</span><span class="sxs-lookup"><span data-stu-id="b34d0-246">Update resource bookings after they are booked on a project</span></span>

<span data-ttu-id="b34d0-247">לאחר שהוספת משאב כללי או משאב בעל שם לצוות פרויקט, תוכל לשנות את ההזמנות של המשאב.</span><span class="sxs-lookup"><span data-stu-id="b34d0-247">After you've added a generic or named resource to a project team, you can change the resource's bookings.</span></span>

1. <span data-ttu-id="b34d0-248">בדף **פרויקטים** , בכרטיסיה **צוות** , בחר חבר צוות ולאחר מכן בחר **שמור הזמנות**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-248">On the **Projects** page, on the **Team** tab, select a team member, and then select **Maintain Bookings**.</span></span>

    ![לוח זמנים נפתח עבור חבר הצוות שנבחר](media/Resource-Management-image40.png)

    <span data-ttu-id="b34d0-250">לוח הזמנים מופיע ומציג את ההזמנות של חבר צוות הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="b34d0-250">The Schedule Board appears and shows the project team member's bookings.</span></span> <span data-ttu-id="b34d0-251">הרחב את הרשומה של חבר הצוות כדי להציג את השעות שהוזמנו כנגד פרויקט זה ופרויקטים אחרים שצורכים את הקיבולת של חבר הצוות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-251">Expand the team member's record to view the hours that have been booked against this project and other projects that are consuming the team member's capacity.</span></span>

2. <span data-ttu-id="b34d0-252">בחר וגרור את ההזמנה כדי להאריך או לקצר אותו.</span><span class="sxs-lookup"><span data-stu-id="b34d0-252">Select and drag the booking to extend or shorten it.</span></span> <span data-ttu-id="b34d0-253">תיבת הדו-שיח **צור הזמנת משאב** שמופיעה מאפשרת לך להתאים את ההזמנה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-253">A **Create Resource Booking** dialog box appears that lets you adjust the booking.</span></span>

    ![תיבת הדו-שיח 'צור הזמנת משאב'](media/Resource-Management-image41.png)

3. <span data-ttu-id="b34d0-255">‏‫לחץ באמצעות לחצן העכבר הימני על ההזמנה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-255">Right-click the booking.</span></span> <span data-ttu-id="b34d0-256">לאחר מכן תוכל להשתמש בתפריט הקיצור כדי להשלים את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="b34d0-256">You can then use the shortcut menu to complete the following actions:</span></span>

    - <span data-ttu-id="b34d0-257">שינוי מצב ההזמנה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-257">Change the booking status.</span></span>
    - <span data-ttu-id="b34d0-258">עריכת ההזמנה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-258">Edit the booking.</span></span>
    - <span data-ttu-id="b34d0-259">החלפת משאב בצוות הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="b34d0-259">Substitute a resource on the project team.</span></span>

### <a name="change-the-booking-status"></a><span data-ttu-id="b34d0-260">שינוי מצב ההזמנה</span><span class="sxs-lookup"><span data-stu-id="b34d0-260">Change the booking status</span></span>

<span data-ttu-id="b34d0-261">באפשרותך לשנות כל מצב הזמנה מותאם אישית או בברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="b34d0-261">You can change any default or custom booking status.</span></span>

![הפקודה 'שנה מצב'](media/Resource-Management-image42.png)

<span data-ttu-id="b34d0-263">המצבים הבאים כלולים ב- PSA:</span><span class="sxs-lookup"><span data-stu-id="b34d0-263">The following statuses are included in PSA:</span></span>

- <span data-ttu-id="b34d0-264">**בוטל** – מצב זה מבטל הזמנת המשאב ומשחרר את קיבולת המשאב.</span><span class="sxs-lookup"><span data-stu-id="b34d0-264">**Canceled** – This status cancels a resource's booking and frees up the resource's capacity.</span></span>
- <span data-ttu-id="b34d0-265">**הזמנה בטוחה** – מצב זה צורך את קיבולת המשאב.</span><span class="sxs-lookup"><span data-stu-id="b34d0-265">**Hard Book** – This status consumes a resource's capacity.</span></span> <span data-ttu-id="b34d0-266">הזמנה נמצאת בדרך כלל במצב זה כאשר פותחים את **שמור הזמנות** מהרשת **כל חברי הצוות** בדף **פרויקטים**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-266">A booking typically has this status when you open **Maintain Bookings** from the **All Team Members** grid on the **Projects** page.</span></span>
- <span data-ttu-id="b34d0-267">**הזמנה טנטטיבית** – מצב זה מוסיף משאב לצוות אבל לא צורך את קיבולת המשאב.</span><span class="sxs-lookup"><span data-stu-id="b34d0-267">**Soft Book** – This status adds a resource to a team but doesn't consume the resource's capacity.</span></span> <span data-ttu-id="b34d0-268">הוא מציין שהמשאב שמור לעבודה פוטנציאלית, אך עדיין יש לו קיבולת אם צריך אותו למשימות אחרות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-268">It indicates that the resource has been reserved for potential work but still has capacity if it's needed on other jobs.</span></span> <span data-ttu-id="b34d0-269">בתצוגה של זמינות משאבים כוללת, להזמנות טנטטיביות יש מצב שונה מאשר הזמנות בטוחות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-269">In the view of overall resource availability, soft bookings have a different status than hard bookings.</span></span>
- <span data-ttu-id="b34d0-270">**מוצע** – מצב זה מייצג את הצעת מנהל המשאבים או מנהל הפרויקט למשאב.</span><span class="sxs-lookup"><span data-stu-id="b34d0-270">**Proposed** – This status represents a resource manager's or project manager's proposal for a resource.</span></span> <span data-ttu-id="b34d0-271">הצעות אינן צורכות את הקיבולת של משאב והמשאב אינו מתווסף לצוות הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="b34d0-271">Proposals don't consume the capacity of a resource, and the resource isn't added to the project team.</span></span> <span data-ttu-id="b34d0-272">כדי לבצע הזמנה בטוחה של המשאב בצוות, מנהל הפרויקט חייב לקבל את ההצעה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-272">To hard-book the resource on the team, the project manager must accept the proposal.</span></span>

### <a name="submit-resource-requests"></a><span data-ttu-id="b34d0-273">הגשת בקשות משאב</span><span class="sxs-lookup"><span data-stu-id="b34d0-273">Submit resource requests</span></span>

<span data-ttu-id="b34d0-274">בקשות למשאבים משמשות למילוי הביקוש (דרישת משאב) שמנהל המשאבים חייב לממש.</span><span class="sxs-lookup"><span data-stu-id="b34d0-274">Resource requests are used to carry the demand (resource requirement) that must be fulfilled by a resource manager.</span></span> <span data-ttu-id="b34d0-275">עבור משאב כללי שכבר נמצא בצוות, באפשרותך לשלוח ישירות בקשת משאב.</span><span class="sxs-lookup"><span data-stu-id="b34d0-275">For a generic resource that is already on the team, you can submit a resource request directly.</span></span> <span data-ttu-id="b34d0-276">ניתן לממש בקשה למשאב בשתי דרכים:</span><span class="sxs-lookup"><span data-stu-id="b34d0-276">A resource request can be fulfilled in two ways:</span></span>

- <span data-ttu-id="b34d0-277">מנהל המשאבים מממש באופן ישיר את הבקשה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-277">The resource manager directly fulfills the request.</span></span> <span data-ttu-id="b34d0-278">במקרה זה, המשאב הכללי מוחלף בהזמנה בטוחה עם משאב בעל שם.</span><span class="sxs-lookup"><span data-stu-id="b34d0-278">In this case, the generic resource is replaced by a hard booking that has a named resource.</span></span>
- <span data-ttu-id="b34d0-279">מנהל המשאבים מציע משאב למנהל הפרויקט ומנהל הפרויקט מאשר או דוחה את המשאב המוצע.</span><span class="sxs-lookup"><span data-stu-id="b34d0-279">The resource manager proposes a resource to the project manager, and the project manager approves or rejects the proposed resource.</span></span>

#### <a name="direct-fulfillment-of-resource-requests"></a><span data-ttu-id="b34d0-280">מימוש ישיר של בקשות למשאבים</span><span class="sxs-lookup"><span data-stu-id="b34d0-280">Direct fulfillment of resource requests</span></span>

<span data-ttu-id="b34d0-281">כאשר דרישת משאב נוצרת, מנהל פרויקט יכול לשלוח בקשה למשאב עבור משאב כללי כל-ידי בחירה במשאב ולאחר מכן בחירה באפשרות **שלח בקשה**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-281">When a resource requirement is generated, a project manager can submit a resource request for a generic resource by selecting the resource and then selecting **Submit Request**.</span></span>

![לחצן 'שלח בקשה'](media/Resource-Management-image45.png)

<span data-ttu-id="b34d0-283">ניתן לספק הערות על המשאב למנהל המשאבים אשר מממש את הבקשה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-283">Comments about the resource can be provided to the resource manager who is fulfilling the request.</span></span> <span data-ttu-id="b34d0-284">לאחר שליחת הבקשה, השדה **מצב** עבור חבר הצוות משתנה ל **נשלח**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-284">After the request is submitted, the **Status** field for the team member is changed to **Submitted**.</span></span>

![הזנת הערות אופציונליות](media/Resource-Management-image46.png)

<span data-ttu-id="b34d0-286">כאשר מנהל המשאבים מממש את הבקשה, חבר הצוות הכללי מוחלף על-ידי המשאב בעל השם ברשת **כל חברי הצוות**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-286">When the resource manager fulfills the request, the generic team member is replaced by the named resource in the **All Team Members** grid.</span></span>

![חבר צוות כללי מוחלף על-ידי המשאב בעל השם ברשת 'כל חברי הצוות'](media/Resource-Management-image47.png)

#### <a name="use-a-resource-proposal-for-resource-requests"></a><span data-ttu-id="b34d0-288">שימוש בהצעת משאב עבור בקשות למשאבים</span><span class="sxs-lookup"><span data-stu-id="b34d0-288">Use a resource proposal for resource requests</span></span>

<span data-ttu-id="b34d0-289">במקום להזמין משאב ישירות בבקשת משאב, מנהל משאבים יכול להציע משאב למנהל הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="b34d0-289">Instead of directly booking a resource on a resource request, a resource manager can propose a resource to the project manager.</span></span> <span data-ttu-id="b34d0-290">מנהל משאבים עשוי להשתמש באפשרות זו כאשר התאמה מדויקת עבור הדרישות אינה זמינה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-290">A resource manager might use this option when an exact match for the requirements isn't available.</span></span> <span data-ttu-id="b34d0-291">כאשר מנהל משאבים מציע משאב, מנהל הפרויקט רואה שהשדה **מצב** עבור חבר הצוות הכללי השתנה ל **נחוצה סקירה**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-291">When a resource manager proposes a resource, the project manager sees that the **Status** field for the generic team member is changed to **Needs Review**.</span></span>

![המצב של חבר צוות כללי השתנה ל'נחוצה סקירה'](media/Resource-Management-image48.png)

<span data-ttu-id="b34d0-293">כדי להציג את המשאב המוצע יחד עם תצוגה חזותית של השפעת ההזמנה של ההצעה, לחץ פעמיים על חבר הצוות שיש לו את המצב **נחוצה סקירה**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-293">To view the proposed resource together with a visualization of the effect of the proposal's booking, double-click the team member that has a status of **Needs Review**.</span></span> <span data-ttu-id="b34d0-294">לאחר מכן בחר את הכרטיסיה **משאבים מוצעים**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-294">Then select the **Proposed Resources** tab.</span></span>

![הכרטיסיה 'משאבים מוצעים'](media/Resource-Management-image49.png)

<span data-ttu-id="b34d0-296">בחר **קבל את כל ההצעות** כדי לקבל את כל המשאבים המוצעים או בחר **דחה את כל ההצעות** כדי לדחות אותם.</span><span class="sxs-lookup"><span data-stu-id="b34d0-296">Select **Accept All Proposals** to accept all proposed resources or **Reject All Proposals** to reject them.</span></span> <span data-ttu-id="b34d0-297">אם תקבל את המשאבים המוצעים, הם יהפכו להזמנה בטוחה בפרויקט כחברי צוות ויחליפו את המשאבים הכלליים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-297">If you accept the proposed resources, they are hard-booked on the project as team members and replace the generic resources.</span></span>

> [!NOTE]
> <span data-ttu-id="b34d0-298">עליך לקבל או לדחות את כל המשאבים המוצעים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-298">You must either accept or reject all proposed resources.</span></span> <span data-ttu-id="b34d0-299">אינך יכול לקבל או לדחות אותם באופן חלקי.</span><span class="sxs-lookup"><span data-stu-id="b34d0-299">You can't partially accept or reject them.</span></span>

### <a name="substitute-a-resource-on-the-project-team"></a><span data-ttu-id="b34d0-300">החלפת משאב בצוות הפרויקט</span><span class="sxs-lookup"><span data-stu-id="b34d0-300">Substitute a resource on the project team</span></span>

<span data-ttu-id="b34d0-301">לפעמים מנהל פרויקט צריך להחליף חבר צוות שהוזמן בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="b34d0-301">Sometimes, a project manager must substitute a booked team member on a project.</span></span>

1. <span data-ttu-id="b34d0-302">בדף **פרויקטים** , בכרטיסיה **צוות** , בחר את המשאב שיש להחליף ולאחר מכן בחר **שמור הזמנות**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-302">On the **Projects** page, on the **Team** tab, select the resource that needs a substitute, and then select **Maintain Bookings**.</span></span>
2. <span data-ttu-id="b34d0-303">הרחב את המשאב כדי להציג את הפרויקטים שאליהם הוא מוקצה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-303">Expand the resource to view the projects that it's assigned to.</span></span>

    ![משאב שהורחב כדי להציג פרויקטים שהוקצו](media/Resource-Management-image50.png)

3. <span data-ttu-id="b34d0-305">לחץ באמצעות לחצן העכבר הימני על הפרויקט ולאחר מכן בחר **החלף משאב**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-305">Right-click the project, and then select **Substitute Resource**.</span></span>
4. <span data-ttu-id="b34d0-306">אם אתה יודע מהו המשאב שברצונך להחליף עבור המשאב הנוכחי, בחר או הקלד את השם ולאחר מכן בחר **הקצה מחדש**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-306">If you know the resource that you want to substitute for the current resource, select or type the name, and then select **Re-assign**.</span></span>

    ![ציון משאב חלופי](media/Resource-Management-image51.png)

    <span data-ttu-id="b34d0-308">לחלופין, בצע את השלבים הבאים כדי לחפש משאב:</span><span class="sxs-lookup"><span data-stu-id="b34d0-308">Alternatively, follow these steps to search for a resource:</span></span>

    1. <span data-ttu-id="b34d0-309">בחר **חפש תחליף**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-309">Select **Find Substitution**.</span></span>

        ![חיפוש משאב חלופי](media/Resource-Management-image52.png)

        <span data-ttu-id="b34d0-311">מסייע לוח הזמנים מחזיר רשימה של תחליפים זמינים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-311">The Schedule Assistant returns a list of available substitutes.</span></span> <span data-ttu-id="b34d0-312">במסייע לוח הזמנים תוכל לבצע סינון נוסף למשאבים הזמינים כדי למצוא תחליף מתאים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-312">In the Schedule Assistant, you can further filter the available resources to find a suitable substitute.</span></span>

        ![רשיה של תחליפים זמינים](media/Resource-Management-image53.png)

    2. <span data-ttu-id="b34d0-314">כדי להחליף את המשאב, בחר את המשאב הרצוי ולאחר מכן בחר **החלף**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-314">To substitute the resource, select the resource that you want, and then select **Substitute**.</span></span>

        ![האפשרות 'החלף משאב' נבחרה](media/Resource-Management-image54.png)

    <span data-ttu-id="b34d0-316">ההזמנות וההקצאות מוחלפות במשאב החדש.</span><span class="sxs-lookup"><span data-stu-id="b34d0-316">The bookings and assignments are substituted with the new resource.</span></span>

    ![הזמנות והקצאות מוחלפות במשאב החדש](media/Resource-Management-image55.png)

## <a name="reconcile-team-member-bookings-and-assignments"></a><span data-ttu-id="b34d0-318">התאמת הזמנות והקצאות של חבר צוות</span><span class="sxs-lookup"><span data-stu-id="b34d0-318">Reconcile team member bookings and assignments</span></span>

<span data-ttu-id="b34d0-319">עבור חברי צוות, הזמנות והקצאות משולבות באופן רופף.</span><span class="sxs-lookup"><span data-stu-id="b34d0-319">For team members, bookings and assignments are loosely coupled.</span></span> <span data-ttu-id="b34d0-320">במילים אחרות, משאבים יכולים לקבל הקצאות אך לא הזמנות, או שהם יכולים לקבל הזמנות אך לא הקצאות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-320">In other words, resources can have assignments but no bookings, or they can have bookings but no assignments.</span></span> <span data-ttu-id="b34d0-321">באופן אידיאלי, יש ליישר הזמנות והקצאות, כך שלמשאבים תהיה קיבולת בהתחייבות לביצוע הקצאות המשימה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-321">Ideally, bookings and assignments should be aligned, so that resources have committed capacity to perform the task assignments.</span></span> <span data-ttu-id="b34d0-322">עם זאת, ייתכן שההזמנות מבוססות על זמינות, ותזמוני המשימות עשויים להשתנות עם המשך הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="b34d0-322">However, the bookings might be based on availability, and task timings might change as the project continues.</span></span> <span data-ttu-id="b34d0-323">לכן, שילוב רופף של הזמנות והקצאות מספק גמישות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-323">Therefore, the loose coupling of bookings and assignments provides flexibility.</span></span>

<span data-ttu-id="b34d0-324">ל- PSA יש כרטיסיה **יישוב** שמאפשרת למנהלי פרויקטים ליישב הזמנות של חברי צוות ואת ההקצאות שלהם עבור צוותי פרויקטים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-324">PSA has a **Reconciliation** tab that lets project managers reconcile team members' bookings and their assignments for project teams.</span></span>

![הכרטיסיה 'יישוב'](media/Resource-Management-image56.png)

<span data-ttu-id="b34d0-326">הכרטיסיה **יישוב** מציגה הזמנות והקצאות עד לרמת ההקצאה של משימה בודדת עבור כל חבר צוות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-326">The **Reconciliation** tab shows bookings and assignments down to the level of the individual task assignment for each team member.</span></span> <span data-ttu-id="b34d0-327">היא מציגה שעות בתאים שמייצגים תקופות זמן, החל מחודשים ועד לימים.</span><span class="sxs-lookup"><span data-stu-id="b34d0-327">It shows hours in cells that represent time periods from months down to days.</span></span>

<span data-ttu-id="b34d0-328">הכרטיסיה מציגה גם את סך הנטו הכולל עבור הפרויקט, יחד עם עמודת סכום.</span><span class="sxs-lookup"><span data-stu-id="b34d0-328">The tab also shows an overall net total for the project, together with a total column.</span></span>

<span data-ttu-id="b34d0-329">עבור כל משאב, הכרטיסיה מחשבת את ההפרש בין ההזמנות של חבר הצוות לבין סיכום של הקצאות המשימה של חבר הצוות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-329">For each resource, the tab calculates the difference between the team member's bookings and a rollup of the team member's task assignments.</span></span> <span data-ttu-id="b34d0-330">באופן אידיאלי, ההפרש צריך להיות 0 (אפס).</span><span class="sxs-lookup"><span data-stu-id="b34d0-330">Ideally, this difference should be 0 (zero).</span></span> <span data-ttu-id="b34d0-331">במילים אחרות, לא צריך להיות הפרש בין הזמנות והקצאות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-331">In other words, there should be no difference between bookings and assignments.</span></span> <span data-ttu-id="b34d0-332">ההפרשים צבועים ומוצללים כדי למשוך תשומת לב לשני מצבים:</span><span class="sxs-lookup"><span data-stu-id="b34d0-332">Differences are colored and shaded to draw attention to two conditions:</span></span>

- <span data-ttu-id="b34d0-333">**מחסור בהזמנות** – מחסור בהזמנות מתרחש כאשר למשאב יש יותר הקצאות מהזמנות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-333">**Booking shortage** – A booking shortage occurs when a resource has more assignments than bookings.</span></span> <span data-ttu-id="b34d0-334">מאחר שקיבולת זו אינה שמורה, ייתכן שמנהל הפרויקט ירצה לתקן מצב זה על-ידי הרחבת ההזמנות של המשאב כדי לכסות על המחסור.</span><span class="sxs-lookup"><span data-stu-id="b34d0-334">Because this capacity hasn't been reserved, a project manager might want to correct this condition by extending the resource's bookings to cover the deficit.</span></span>
- <span data-ttu-id="b34d0-335">**הזמנות עודפות** - הזמנות עודפות מתרחשות כאשר משאב הוזמן לפרויקט אך לא הוקצה למשימות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-335">**Excess bookings** – Excess bookings occur when a resource has been booked to the project but hasn't been assigned to tasks.</span></span> <span data-ttu-id="b34d0-336">מצב זה עשוי להיות מקובל במקרים שבהם המשאב הוזמן לפרויקט לפני שהקצאת המשימה התרחשה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-336">This condition might be acceptable in the cases where the resource was booked to the project before task assignment occurred.</span></span> <span data-ttu-id="b34d0-337">יחד עם זאת, במקרים אחרים, המשאב אינו מתוכנן להיות מוקצה למשימות.</span><span class="sxs-lookup"><span data-stu-id="b34d0-337">However, in other cases, the resource isn't planned to be assigned to tasks.</span></span> <span data-ttu-id="b34d0-338">במקרים אלה, מנהל הפרויקט צריך לשקול לבטל את הזמנות המשאב, כך שניתן יהיה להשתמש בקיבולת עבור פרויקט אחר.</span><span class="sxs-lookup"><span data-stu-id="b34d0-338">In these cases, the project manager should consider canceling the resource's bookings, so that the capacity can be used for another project.</span></span>

<span data-ttu-id="b34d0-339">במקרים מסוימים, כשתציג זמן ברמה גבוהה יותר מהרמה היומית (לדוגה, הרמה החודשית), אתה עשוי לראות הפרש נטו של אפס עבור משאב (במילים אחרות, הזמנות = הקצאות).</span><span class="sxs-lookup"><span data-stu-id="b34d0-339">In some cases, when you view time at a higher level than the day level (for example, the month level), you might see a net difference of zero for a resource (in other words, bookings = assignments).</span></span> <span data-ttu-id="b34d0-340">אולם, אם תציג זמן ברמה השבועית, אתה עשוי לראות שישנן הקצאות עם אפס שעות והזמנות של 40 שעות בשבוע הראשון, אך הקצאות של 40 שעות והזמנות של אפס שעות בשבוע השני.</span><span class="sxs-lookup"><span data-stu-id="b34d0-340">However, if you view time at the week level, you might see that there are assignments of zero hours and bookings of 40 hours in the first week, but assignments of 40 hours and bookings of zero hours in the second week.</span></span> <span data-ttu-id="b34d0-341">בסך הכל, ההזמנות וההקצאות מיושבות, אך הן משתנות משבוע אחד למשנהו.</span><span class="sxs-lookup"><span data-stu-id="b34d0-341">Overall, the bookings and assignments are reconciled, but they differ from one week to the next.</span></span>

<span data-ttu-id="b34d0-342">בעת הצגת זמן ברמות גבוהות יותר, לתאים בכרטיסיה **יישוב** יש מחוון שיודיע לך שיש הפרשים ברמות נמוכות יותר.</span><span class="sxs-lookup"><span data-stu-id="b34d0-342">When you view time at higher levels, cells in the **Reconciliation** tab have an indicator to inform you that there are differences at lower levels.</span></span> <span data-ttu-id="b34d0-343">על-ידי לחיצה כפולה בתא, תוכל להגדיל כדי להציג את ההפרש.</span><span class="sxs-lookup"><span data-stu-id="b34d0-343">By double-clicking in a cell, you can zoom in to view the difference.</span></span> <span data-ttu-id="b34d0-344">לאחר מכן תוכל ללחוץ באמצעות לחצן העכבר הימני כדי להקטין. על-ידי בחירת משאב ולאחר מכן שימוש בבקרה **ההפרש הבא** בסרגל הכלים של הרשת, תוכל לעבור להפרש הבא בין הזמנות והקצאות עבור אותו משאב.</span><span class="sxs-lookup"><span data-stu-id="b34d0-344">You can then right-click to zoom out. By selecting a resource and then using the **Next difference** control on the grid toolbar, you can go to the next difference between bookings and assignments for that resource.</span></span> <span data-ttu-id="b34d0-345">תוכל מכן תוכל להשתמש בבקרה **ההפרש הקודם** כדי לחזור אחורה.</span><span class="sxs-lookup"><span data-stu-id="b34d0-345">You can then use the **Previous difference** control to go back.</span></span> <span data-ttu-id="b34d0-346">בנוסף, תוכל לבטל את מחוון ההפרש ואופן פעולת הניווט תחת **הגדרות**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-346">You can also turn off the difference indicator and navigation behavior under **Settings**.</span></span>

![מחוון הפרש](media/Resource-Management-image57.png)

<span data-ttu-id="b34d0-348">אם יש לך הקצאות משימה עבור משאב אך ללא הזמנות, בדף **פרויקטים** , בכרטיסיה **יישוב** , בחר את המחסור בהזמנות ולאחר מכן בחר **‏‫הארך הזמנה**.</span><span class="sxs-lookup"><span data-stu-id="b34d0-348">If you have task assignments for a resource but no bookings, on the **Projects** page, on the **Reconciliation** tab, select the booking shortage, and then select **Extend Booking**.</span></span> <span data-ttu-id="b34d0-349">תיבת הדו-שיח **‏‫הארך הזמנה** מופיעה ומציגה את ההזמנה הדרושה כדי לטפל במחסור של המשאב.</span><span class="sxs-lookup"><span data-stu-id="b34d0-349">The **Extend Booking** dialog box appears and shows the booking that is needed to address the resource's shortage.</span></span> <span data-ttu-id="b34d0-350">היא גם מציגה את ההזמנות הקיימות של המשאב בכל הפרויקטים או בשאר הישויות הניתנות לתזמון.</span><span class="sxs-lookup"><span data-stu-id="b34d0-350">It also shows the resource's existing bookings across all projects or other schedulable entities.</span></span> <span data-ttu-id="b34d0-351">אם תבחר **אישור** כדי ליצור את ההזמנה עבור המשאב, ללא קשר לזמינות המשאב, ייתכן שתגרום להזמנת יתר.</span><span class="sxs-lookup"><span data-stu-id="b34d0-351">If you select **OK** to create the booking for the resource, regardless of that resource's availability, you might cause overbooking.</span></span>

![תיבת הדו-שיח 'הארך הזמנה'](media/Resource-Management-image58.png)

<span data-ttu-id="b34d0-353">מנהל הפרויקט או מנהל המשאבים יכולים אחר כך להשתמש בלוח הזמנים כדי לנהל מצבים שבהם משאב מוזמן מעבר לקיבולת שלו.</span><span class="sxs-lookup"><span data-stu-id="b34d0-353">The project manager or resource manager can then use the Schedule Board to manage any situations where a resource is overbooked beyond its capacity.</span></span>
