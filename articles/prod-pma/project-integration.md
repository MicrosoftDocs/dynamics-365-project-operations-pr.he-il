---
title: שילוב Microsoft Project Client
description: תכנון לוח הזמנים של פרויקט ואחזקתו יכולים להיות מורכבים, כך שמנהלי הפרויקטים צריכים להשתמש בכלים שעוזרים להם לנהל משימה זו. שילוב עם Microsoft Project Client מספק תמיכה לפתיחת מבנה התפלגות עבודה וניהולו.
author: Yowelle
ms.date: 06/16/2021
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjWbsTemplate
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2017-12-04
ms.dyn365.ops.version: 7.2999999999999998
ms.openlocfilehash: b312ec5b1f4e6a98a2cbf1667b2f55b758b2d613
ms.sourcegitcommit: 3a4b181be08ef0428104d72b54a3e61ac2782f14
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/17/2021
ms.locfileid: "6269836"
---
# <a name="microsoft-project-client-integration"></a><span data-ttu-id="e4aec-104">שילוב Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="e4aec-104">Microsoft Project client integration</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="e4aec-105">תכנון לוח הזמנים של פרויקט ואחזקתו יכולים להיות מורכבים, כך שמנהלי הפרויקטים צריכים להשתמש בכלים שעוזרים להם לנהל משימה זו.</span><span class="sxs-lookup"><span data-stu-id="e4aec-105">Planning and maintaining a project schedule can be complex, so project managers need to use tools that help them manage this task.</span></span> <span data-ttu-id="e4aec-106">שילוב עם Microsoft Project Client מספק תמיכה לפתיחת מבנה התפלגות עבודה וניהולו.</span><span class="sxs-lookup"><span data-stu-id="e4aec-106">Integration with Microsoft Project Client provides support to open and manage a project work breakdown structure.</span></span> <span data-ttu-id="e4aec-107">מנהל הפרויקט יכול לפרסם כל שינוי בחזרה אל מבנה התפלגות עבודת הפרויקט ב- Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="e4aec-107">The project manager can publish any changes back to the Dynamics 365 Finance project work breakdown structure.</span></span>

> [!NOTE]
> <span data-ttu-id="e4aec-108">אם אתה משתמש בעדכון יולי (גירסה 10.0.4), עליך להתקין את KB 4054797 ואת 4055884.</span><span class="sxs-lookup"><span data-stu-id="e4aec-108">If you are using the July update (version 10.0.4), you must install KB 4054797 and 4055884.</span></span>

## <a name="configure-the-microsoft-project-client-add-in"></a><span data-ttu-id="e4aec-109">הגדרת התוספת Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="e4aec-109">Configure the Microsoft Project Client add-in</span></span>
<span data-ttu-id="e4aec-110">כדי להפעיל את השילוב עם Microsoft Project Client, נדרשת התקנת תוספת Microsoft Dynamics 365 ביישום Microsoft Project בלקוח של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="e4aec-110">To enable the integration with Microsoft Project Client, a Microsoft Dynamics 365 add-in is required to be installed in the user’s client Microsoft Project application.</span></span> <span data-ttu-id="e4aec-111">זה נעשה על-ידי פתיחת **סביבת העבודה לניהול פרויקטים**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-111">This is done by opening the **Project management workspace**.</span></span>

<span data-ttu-id="e4aec-112">•   לחץ על **הגדר תצורת תוספת בלקוח פרויקט** מהמקטע **קישורים** > **הגדרה** בסביבת העבודה.</span><span class="sxs-lookup"><span data-stu-id="e4aec-112">•   Click **Configure project client add-in** from the **Links** > **Setup** section of the workspace.</span></span>

<span data-ttu-id="e4aec-113">•   לחץ **פתח**, וכשתתבקש, לחץ על **הפעל**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-113">•   Click **Open**, then click **Run** when prompted.</span></span>

## <a name="open-and-edit-an-existing-draft-work-breakdown-structure-in-microsoft-project-client"></a><span data-ttu-id="e4aec-114">פתיחת טיוטה קיימת של מבנה התפלגות עבודה ב- Microsoft Project Client ועריכתה</span><span class="sxs-lookup"><span data-stu-id="e4aec-114">Open and edit an existing draft work breakdown structure in Microsoft Project Client</span></span>
<span data-ttu-id="e4aec-115">אם לפרויקט ב- Dynamics 365 Finance כבר נוצר מבנה התפלגות עבודה, ניתן לפתוח את מבנה התפלגות העבודה ביישום Microsoft Project Client אם מבנה התפלגות העבודה נמצא במצב טיוטה.</span><span class="sxs-lookup"><span data-stu-id="e4aec-115">If a project in Dynamics 365 Finance already has a work breakdown structure created, the work breakdown structure can be opened in the Microsoft Project Client application if the work breakdown structure is in a draft status.</span></span> <span data-ttu-id="e4aec-116">כדי לפתוח את הדף **פרויקט**, לחץ על הקישור **פתח ב- Microsoft Project** מהכרטיסיה **תכנון**. בנוסף, ניתן לפתוח דך זה מתוך יישום Microsoft Project Client על-ידי לחיצה על **פתח** בכרטיסיה **Microsoft Dynamics 365**. בחר **ישות משפטית** ו **פרויקט** מהרשימה.</span><span class="sxs-lookup"><span data-stu-id="e4aec-116">To open from the **Project** page, click **Open in Microsoft Project** link from the **Plan** tab. This page can also be opened from within the Microsoft Project Client application by clicking **Open** in the **Microsoft Dynamics 365** tab. Select the **Legal entity** and **Project** from the list.</span></span>

> [!NOTE]
> <span data-ttu-id="e4aec-117">אם אתה משתמש ב- Internet Explorer כדפדפן שלך, עליך ללחוץ על **שמור** כדי לפתוח ידנית מהמיקום שאליו הקובץ הורד.</span><span class="sxs-lookup"><span data-stu-id="e4aec-117">If you're using Internet Explorer as your browser, you will need to click **Save** to manually open from the location that the file is downloaded to.</span></span> <span data-ttu-id="e4aec-118">לחלופין, לחץ על **שמור ופתח** כדי לפתוח את הקובץ ב- Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="e4aec-118">Or, click **Save and open** to open the file in Microsoft Project Client.</span></span> <span data-ttu-id="e4aec-119">אל תשנה את השם של הקובץ בעת השמירה.</span><span class="sxs-lookup"><span data-stu-id="e4aec-119">Do not rename the file name when saving.</span></span>

<span data-ttu-id="e4aec-120">לפני ביצוע פעולות עריכה בקובץ בעת שימוש ב- Microsoft Project Client, עליך להוציא אותו. לחץ על **הוצא קובץ** בכרטיסיה **Microsoft Dynamics 365**. פעולה זו תמנע ממשתמשים אחרים לערוך את מבנה התפלגות העבודה מתוך Finance במקביל.</span><span class="sxs-lookup"><span data-stu-id="e4aec-120">Before making any edits to the file using Microsoft Project Client, you need to check it out. Click **Check out** in the **Microsoft Dynamics 365** tab. This will prevent other users from editing the work breakdown structure from within Finance at the same time.</span></span> <span data-ttu-id="e4aec-121">כדי לפרסם את מבנה התפלגות העבודה לאחר השלמת העריכה, לחץ על **הכנס קובץ** בכרטיסיה **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-121">To publish the work breakdown structure after completing any edits, click **Check in** on the **Microsoft Dynamics 365** tab.</span></span>

<span data-ttu-id="e4aec-122">אם צוות פרויקט כבר נוסף לפרויקט ב- Finance, רשימת המשאבים תאוכלס עם חברי הצוות.</span><span class="sxs-lookup"><span data-stu-id="e4aec-122">If a project team has already been added to the project in Finance, the resource list will be populated with the team members.</span></span> <span data-ttu-id="e4aec-123">אם טרם התווסף צוות פרויקט לפרויקט, באפשרותך לבחור משאבים ולבנות את הצוות בתוך Microsoft Project Client על ידי לחיצה על לחצן **משאבים‏‎** בכרטיסיה **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-123">If a project team has not yet been added to the project, you can select resources and build the team within Microsoft Project Client by clicking the **Resources** button on the **Microsoft Dynamics 365** tab.</span></span> 

<span data-ttu-id="e4aec-124">הנתונים הבאים יסונכרנו בחזרה ל- Finance כחלק מתהליך הכנסת הקובץ:</span><span class="sxs-lookup"><span data-stu-id="e4aec-124">The following data will be synced back to Finance as part of the check-in process:</span></span>

<span data-ttu-id="e4aec-125">•   שם משימה</span><span class="sxs-lookup"><span data-stu-id="e4aec-125">•   Task name</span></span>

<span data-ttu-id="e4aec-126">•   תאריך התחלה</span><span class="sxs-lookup"><span data-stu-id="e4aec-126">•   Start date</span></span>

<span data-ttu-id="e4aec-127">•   תאריך סיום</span><span class="sxs-lookup"><span data-stu-id="e4aec-127">•   Finish date</span></span>

<span data-ttu-id="e4aec-128">•   ‏‏פעילויות קדם</span><span class="sxs-lookup"><span data-stu-id="e4aec-128">•   Predecessors</span></span>

<span data-ttu-id="e4aec-129">•   שמות משאבים</span><span class="sxs-lookup"><span data-stu-id="e4aec-129">•   Resource names</span></span>

<span data-ttu-id="e4aec-130">•   קטגוריה</span><span class="sxs-lookup"><span data-stu-id="e4aec-130">•   Category</span></span>

<span data-ttu-id="e4aec-131">•   קטגוריית משאבים</span><span class="sxs-lookup"><span data-stu-id="e4aec-131">•   Resource category</span></span>

<span data-ttu-id="e4aec-132">•   שעות עבודה</span><span class="sxs-lookup"><span data-stu-id="e4aec-132">•   Work hours</span></span>

<span data-ttu-id="e4aec-133">•   הערות</span><span class="sxs-lookup"><span data-stu-id="e4aec-133">•   Notes</span></span>

<span data-ttu-id="e4aec-134">•   עדיפות</span><span class="sxs-lookup"><span data-stu-id="e4aec-134">•   Priority</span></span>

> [!NOTE]
> <span data-ttu-id="e4aec-135">אם תוסיף עמודות אחרות לקובץ Microsoft Project Client שלך, הן לא יישמרו בקובץ ולא יוצגו עם פתיחת הקובץ שוב.</span><span class="sxs-lookup"><span data-stu-id="e4aec-135">If you add any other columns to your Microsoft Project Client file, they will not be saved to the file and will not be displayed when the file is opened again.</span></span>

## <a name="create-the-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a><span data-ttu-id="e4aec-136">יצירת מבנה התפלגות העבודה עבור פרויקט קיים באמצעות Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="e4aec-136">Create the work breakdown structure for an existing project using Microsoft Project Client</span></span>
<span data-ttu-id="e4aec-137">כדי ליצור מבנה התפלגות עבודה חדש באמצעות Microsoft Project Client, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="e4aec-137">To create a new work breakdown structure using Microsoft Project Client, follow these steps:</span></span>


1.  <span data-ttu-id="e4aec-138">פתח את Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="e4aec-138">Open Microsoft Project Client.</span></span>

2.  <span data-ttu-id="e4aec-139">בכרטיסיה **Microsoft Dynamics 365**, לחץ על **פתח**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-139">On the **Microsoft Dynamics 365** tab, click **Open**.</span></span>

3.  <span data-ttu-id="e4aec-140">בחר את **הישות המשפטית** עבור הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="e4aec-140">Select the **Legal entity** for the project.</span></span>

4.  <span data-ttu-id="e4aec-141">בחר את ה **פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-141">Select the **Project**.</span></span>

5.  <span data-ttu-id="e4aec-142">לחץ על **הוצא קובץ** בכרטיסיה **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-142">Click **Check out** on the **Microsoft Dynamics 365** tab.</span></span>

6.  <span data-ttu-id="e4aec-143">כשתהיה מוכן לפרסם ב- Finance, לחץ על **הכנס קובץ** בכרטיסיה **Microsoft Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-143">When ready to publish to Finance, click **Check in** on the **Microsoft Dynamics 365** tab.</span></span>

## <a name="replace-the-existing-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a><span data-ttu-id="e4aec-144">החלפת את מבנה התפלגות העבודה הקיים עבור פרויקט קיים באמצעות Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="e4aec-144">Replace the existing work breakdown structure for an existing project using Microsoft Project Client</span></span>
<span data-ttu-id="e4aec-145">כדי ליצור מבנה התפלגות עבודה חדש באמצעות Microsoft Project Client ולהחליף מבנה התפלגות עבודה קיים לפרויקט קיים, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="e4aec-145">To create a new work breakdown structure using Microsoft Project Client and replace an existing work breakdown structure for an existing project, follow these steps:</span></span>

1.  <span data-ttu-id="e4aec-146">פתח את Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="e4aec-146">Open the Microsoft Project Client.</span></span>

2.  <span data-ttu-id="e4aec-147">צור את לוח הזמנים ב- Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="e4aec-147">Create the schedule in Microsoft Project Client.</span></span>

3.  <span data-ttu-id="e4aec-148">בכרטיסיה **Microsoft Dynamics 365**, לחץ על **שמור שינויים** > **החלף פרויקט קיים**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-148">On the **Microsoft Dynamics 365** tab, click **Save changes** > **Replace existing project**.</span></span>

4.  <span data-ttu-id="e4aec-149">בחר את **הישות המשפטית** עבור הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="e4aec-149">Select the **Legal entity** for the project.</span></span>

5.  <span data-ttu-id="e4aec-150">בחר את ה **פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-150">Select the **Project**.</span></span>

6.  <span data-ttu-id="e4aec-151">לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-151">Click **OK**.</span></span>

## <a name="create-a-new-project-from-within-microsoft-project-client"></a><span data-ttu-id="e4aec-152">יצירת פרויקט חדש מתוך Microsoft Project Client</span><span class="sxs-lookup"><span data-stu-id="e4aec-152">Create a new project from within Microsoft Project Client</span></span>


1.  <span data-ttu-id="e4aec-153">פתח את Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="e4aec-153">Open the Microsoft Project Client.</span></span>

2.  <span data-ttu-id="e4aec-154">צור את לוח הזמנים ב- Microsoft Project Client.</span><span class="sxs-lookup"><span data-stu-id="e4aec-154">Create the schedule in Microsoft Project Client.</span></span>

3.  <span data-ttu-id="e4aec-155">בכרטיסיה **Microsoft Dynamics 365**, לחץ על **שמור שינויים** > **שמור לפרויקט חדש**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-155">On the **Microsoft Dynamics 365** tab, click **Save changes** > **Save to new Project**.</span></span>

4.  <span data-ttu-id="e4aec-156">בחר את **הישות המשפטית** עבור הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="e4aec-156">Select the **Legal entity** for the project.</span></span>

5.  <span data-ttu-id="e4aec-157">בעת הצורך, הזן את **מזהה הפרויקט**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-157">Enter the **Project ID**, if necessary.</span></span>

6.  <span data-ttu-id="e4aec-158">הזן את **שם הפרויקט**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-158">Enter the **Project name**.</span></span>

7.  <span data-ttu-id="e4aec-159">בחר את **סוג הפרויקט**, **קבוצת הפרויקטים** ואת **מזהה חוזה הפרויקט**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-159">Select the **Project type**, **Project group** and the **Project contract ID**.</span></span> <span data-ttu-id="e4aec-160">לחלופין, תוכל ליצור חוזה פרויקט חדש על ידי לחיצה על **חדש**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-160">Alternatively, you can create a new project contract by clicking **New**.</span></span>

8.  <span data-ttu-id="e4aec-161">בחר את **לוח השנה** שבו יש להשתמש להקצאת משאבים.</span><span class="sxs-lookup"><span data-stu-id="e4aec-161">Select the **Calendar** to be used for resourcing.</span></span>

11. <span data-ttu-id="e4aec-162">לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="e4aec-162">Click **OK**.</span></span>

> [!NOTE]
> <span data-ttu-id="e4aec-163">התוספת 'לקוח פרויקט' אינה תומכת בתווים הבאים בתבנית מזהה הפרוייקט:</span><span class="sxs-lookup"><span data-stu-id="e4aec-163">The Project Client add-in doesn’t support the following characters in the project ID format:</span></span>
> 
>   - <span data-ttu-id="e4aec-164">מקף תחתון</span><span class="sxs-lookup"><span data-stu-id="e4aec-164">Underscore</span></span>
>   - <span data-ttu-id="e4aec-165">נקודה</span><span class="sxs-lookup"><span data-stu-id="e4aec-165">Period</span></span>
>   - <span data-ttu-id="e4aec-166">רווח</span><span class="sxs-lookup"><span data-stu-id="e4aec-166">Space</span></span>
>   - <span data-ttu-id="e4aec-167">קו נטוי</span><span class="sxs-lookup"><span data-stu-id="e4aec-167">Slash</span></span>

[!INCLUDE[footer-include](../includes/footer-banner.md)]
