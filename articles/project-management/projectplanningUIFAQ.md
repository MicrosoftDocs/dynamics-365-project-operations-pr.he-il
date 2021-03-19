---
title: פתרון בעיות בעבודה ברשת המשימות
description: נושא זה מספק מידע לגבי פתרון בעיות הדרוש בעבודה ברשת המשימות.
author: ruhercul
manager: tfehr
ms.date: 01/19/2021
ms.topic: article
ms.product: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: dedd989cc7c959d9ea97a0abfb13f8f1b2150a56
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286564"
---
# <a name="troubleshoot-working-in-the-task-grid"></a><span data-ttu-id="4d0f7-103">פתרון בעיות בעבודה ברשת המשימות</span><span class="sxs-lookup"><span data-stu-id="4d0f7-103">Troubleshoot working in the Task grid</span></span> 

<span data-ttu-id="4d0f7-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="4d0f7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="4d0f7-105">נושא זה מתאר כיצד לתקן בעיות שאתה עלול להיתקל בהן בעת עבודה עם ניהול עלויות.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-105">This topic describes how to fix issues that you might encounter while working with cost management.</span></span>

## <a name="enable-cookies"></a><span data-ttu-id="4d0f7-106">הפעלת קבצי Cookie</span><span class="sxs-lookup"><span data-stu-id="4d0f7-106">Enable cookies</span></span>

<span data-ttu-id="4d0f7-107">Project Operations מחייב הפעלת קובצי Cookie של צד שלישי על מנת לעבד את מבנה התפלגות עבודה.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-107">Project Operations requires that third-party cookies be enabled in order to render the work breakdown structure.</span></span> <span data-ttu-id="4d0f7-108">כאשר קובצי Cookie של צד שלישי אינם מופעלים, במקום לראות משימות, תראה דף ריק כשתבחר את הכרטיסיה **משימות** בדף **פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-108">When third-party cookies aren't enabled, instead of seeing tasks, you will see a blank page when you select the **Tasks** tab on the **Project** page.</span></span>

![כרטיסייה ריקה כאשר קובצי Cookie של צד שלישי אינם מופעלים](media/blankschedule.png)


### <a name="workaround"></a><span data-ttu-id="4d0f7-110">פתרון</span><span class="sxs-lookup"><span data-stu-id="4d0f7-110">Workaround</span></span>
<span data-ttu-id="4d0f7-111">לדפדפנים Microsoft Edge או Google Chrome, הנהלים הבאים מתארים כיצד לעדכן את הגדרת הדפדפן כדי לאפשר קובצי Cookie של צד שלישי.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-111">For Microsoft Edge or Google Chrome browsers, the following procedures outline how to update your browser setting to enable third-party cookies.</span></span>

#### <a name="microsoft-edge"></a><span data-ttu-id="4d0f7-112">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="4d0f7-112">Microsoft Edge</span></span>

1. <span data-ttu-id="4d0f7-113">פתח את דפדפן Edge.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-113">Open your Edge browser.</span></span>
2. <span data-ttu-id="4d0f7-114">בפינה השמאלית העליונה, בחר את **שלוש הנקודות** (...) ולאחר מכן בחר **הגדרות**.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-114">In the upper-right corner, select the **ellipsis** (...), and then select **Settings**.</span></span>
3. <span data-ttu-id="4d0f7-115">באפשרות **קובצי Cookie והרשאות אתרים** בחר **קובצי Cookie ונתוני אתרים**.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-115">Under **Cookies and site permissions**, select **Cookies and site data**.</span></span>
4. <span data-ttu-id="4d0f7-116">כבה את **חסום קובצי Cookie של צד שלישי**.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-116">Turn off **Block third-party cookies**.</span></span>

#### <a name="google-chrome"></a><span data-ttu-id="4d0f7-117">Google Chrome</span><span class="sxs-lookup"><span data-stu-id="4d0f7-117">Google Chrome</span></span>

1. <span data-ttu-id="4d0f7-118">פתח את הדפדפן Chrome.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-118">Open your Chrome browser.</span></span>
2. <span data-ttu-id="4d0f7-119">בפינה השמאלית העליונה, בחר בסמל שלוש הנקודות האנכיות ולאחר מכן בחר **הגדרות**.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-119">In the upper-right corner, select the three vertical dots, and then select **Settings**.</span></span>
3. <span data-ttu-id="4d0f7-120">באפשרות **אבטחה ופרטיות** בחר **קובצי Cookie ונתוני אתרים**.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-120">Under **Privacy and security**, select **Cookies and other site data**.</span></span>
4. <span data-ttu-id="4d0f7-121">בחר **אפשר את כל קבצי ה-Cookie**.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-121">Select **Allow all cookies**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4d0f7-122">אם תחסום קובצי Cookie של צד שלישי, כל קובצי ה- Cookie והנתונים מאתרים אחרים ייחסמו, גם אם האתר מותר ברשימת החריגים שלך.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-122">If you block third-party cookies, all cookies and site data from other sites will be blocked, even if the site is allowed on your exceptions list.</span></span>

## <a name="pex-endpoint"></a><span data-ttu-id="4d0f7-123">נקודת קצה של PEX</span><span class="sxs-lookup"><span data-stu-id="4d0f7-123">PEX Endpoint</span></span>

<span data-ttu-id="4d0f7-124">Project Operations דורש שפרמטר של הפרוייקט יתייחס לנקודת קצה PEX.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-124">Project Operations requires that a project parameter reference the PEX Endpoint.</span></span> <span data-ttu-id="4d0f7-125">נקודת קצה זו צריכה לתקשר עם השירות המשמש לעיבוד של מבנה התפלגות עבודה.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-125">This endpoint is required to communicate with the service used to render the work breakdown structure.</span></span> <span data-ttu-id="4d0f7-126">אם הפרמטר אינו מופעל, תקבל את השגיאה "הפרמטר של הפרוייקט אינו חוקי".</span><span class="sxs-lookup"><span data-stu-id="4d0f7-126">If the parameter isn't enabled, you will receive the error, "The project parameter is not valid".</span></span> 

### <a name="workaround"></a><span data-ttu-id="4d0f7-127">פתרון</span><span class="sxs-lookup"><span data-stu-id="4d0f7-127">Workaround</span></span>
 ![שדה נקודת קצה PEX בפרמטר הפרוייקט](media/projectparameter.png)

1. <span data-ttu-id="4d0f7-129">הוסף את השדה **נקודת קצה PEX** לדף **פרמטרים של פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-129">Add the **PEX Endpoint** field to the **Project Parameters** page.</span></span>
2. <span data-ttu-id="4d0f7-130">עדכן את השדה בערך הבא: `https://project.microsoft.com/<lang>/?org=<cdsServer>#/taskgrid?projectId=\<id>&type=2`</span><span class="sxs-lookup"><span data-stu-id="4d0f7-130">Update the field with the following value: `https://project.microsoft.com/<lang>/?org=<cdsServer>#/taskgrid?projectId=\<id>&type=2`</span></span>
3. <span data-ttu-id="4d0f7-131">הסר את השדה מדף **פרמטרים של פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-131">Remove the field from the **Project Parameters** page.</span></span>

## <a name="privileges-for-project-for-the-web"></a><span data-ttu-id="4d0f7-132">הרשאות לפרוייקט באינטרנט</span><span class="sxs-lookup"><span data-stu-id="4d0f7-132">Privileges for Project for the Web</span></span>

<span data-ttu-id="4d0f7-133">Project Operations מסתמך על שירות תזמון חיצוני.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-133">Project Operations relies on an external scheduling service.</span></span> <span data-ttu-id="4d0f7-134">השירות דורש שלמשתמש יוקצו מספר תפקידים של קריאה וכתיבה לישויות הקשורות למבנה התפלגות עבודה.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-134">The service requires that a user have several roles assigned to read and write to entities related to the work breakdown structure.</span></span> <span data-ttu-id="4d0f7-135">ישויות אלה כוללות משימות פרוייקט, הקצאות משאבים ותלות במשימה.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-135">These entities include project tasks, resource assignments, and task dependencies.</span></span> <span data-ttu-id="4d0f7-136">אם משתמש לא יכול לעבד את מבנה התפלגות עבודה כאשר הוא עובר לכרטיסיה **משימות**, זה כנראה בגלל שלא הופעל Project for Project Operations.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-136">If a user can't render the work breakdown structure when they go to the **Tasks** tab, it's probably because Project for Project Operations hasn't been enabled.</span></span> <span data-ttu-id="4d0f7-137">משתמש עלול לקבל שגיאת תפקיד אבטחה, או שגיאה הקשורה לשלילת גישה.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-137">A user might receive either a security role error, or an error related to a denial of access.</span></span>


## <a name="workaround"></a><span data-ttu-id="4d0f7-138">פתרון</span><span class="sxs-lookup"><span data-stu-id="4d0f7-138">Workaround</span></span>

1. <span data-ttu-id="4d0f7-139">עבור אל **הגדרות > אבטחה > משתמשים > משתמשי יישומים**.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-139">Go to **Setting > Security > Users > Application Users**.</span></span>  

   ![קורא יישום](media/applicationuser.jpg)
   
2. <span data-ttu-id="4d0f7-141">לחץ פעמיים על רשומת המשתמש כדי לאמת:</span><span class="sxs-lookup"><span data-stu-id="4d0f7-141">Double-click the application user record to verify the following:</span></span>

 - <span data-ttu-id="4d0f7-142">למשתמש יש גישה לפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-142">The user has access to the project.</span></span> <span data-ttu-id="4d0f7-143">אימות זה נעשה בדרך כלל על ידי הקפדה על כך שיש למשתמש תפקיד אבטחה של **מנהל פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-143">This verification is typically done by ensuring that the user has **Project Manager** security role.</span></span>
 - <span data-ttu-id="4d0f7-144">המשתמש ביישום Microsoft Project קיים ומוגדר כהלכה.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-144">The Microsoft Project application user exists and is configured correctly.</span></span>
 
3. <span data-ttu-id="4d0f7-145">אם המשתמש לא קיים אפשר ליצור רשומת משתמש חדשה.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-145">If this user doesn't exist, you can create a new user record.</span></span> <span data-ttu-id="4d0f7-146">בחר **משתמשים חדשים**.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-146">Select **New Users**.</span></span> <span data-ttu-id="4d0f7-147">שנה את טופס הערך שיהיה **משתמש באפליקציה** ולאחר מכן הוסף את **מזהה היישום**.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-147">Change the entry form to **Application User**, and then add the **Application ID**.</span></span>

   ![פרטי משתמש ביישום](media/applicationuserdetails.jpg)

4. <span data-ttu-id="4d0f7-149">ודא כי למשתמש הוקצה הרישיון הנכון וכי השירות מופעל בפרטי תוכניות השירות של הרישיון.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-149">Verify that the user has been assigned the correct license and that the service is enabled in the service plans details of the license.</span></span>
5. <span data-ttu-id="4d0f7-150">ודא שהמשתמש יכול לפתוח את project.microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-150">Verify that the user can open project.microsoft.com.</span></span>
6. <span data-ttu-id="4d0f7-151">ודא באמצעות הפרמטרים של הפרוייקט שהמערכת מצביעה על נקודת קצה של הפרוייקט הנכון.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-151">Verify through the project parameters that the system is pointing to the correct project endpoint.</span></span>
7. <span data-ttu-id="4d0f7-152">ודא שמשתמש יישום הפרוייקט נוצר.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-152">Verify that the project application user is created.</span></span>
8. <span data-ttu-id="4d0f7-153">החל את תפקידי האבטחה הבאים על המשתמש:</span><span class="sxs-lookup"><span data-stu-id="4d0f7-153">Apply the following security roles to the user:</span></span>

  - <span data-ttu-id="4d0f7-154">משתמש Dataverse</span><span class="sxs-lookup"><span data-stu-id="4d0f7-154">Dataverse User</span></span>
  - <span data-ttu-id="4d0f7-155">מערכת Project Operations</span><span class="sxs-lookup"><span data-stu-id="4d0f7-155">Project Operations System</span></span>
  - <span data-ttu-id="4d0f7-156">מערכת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="4d0f7-156">Project System</span></span>

## <a name="error-when-updating-the-work-breakdown-structure"></a><span data-ttu-id="4d0f7-157">שגיאה בעת עדכון מבנה התפלגות עבודה</span><span class="sxs-lookup"><span data-stu-id="4d0f7-157">Error when updating the work breakdown structure</span></span>

<span data-ttu-id="4d0f7-158">כאשר מתבצע עדכון אחד או יותר למבנה התפלגות עבודה, השינויים בסופו של דבר נכשלים ואינם נשמרים.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-158">When one or more updates are made to the work breakdown structure, the changes eventually fail and aren't saved.</span></span> <span data-ttu-id="4d0f7-159">שגיאה מתרחשת ברשת לוח הזמנים המציינת כי "לא ניתן היה לשמור את השינוי האחרון שביצעת."</span><span class="sxs-lookup"><span data-stu-id="4d0f7-159">An error occurs in the schedule grid noting that “Recent change you’ve made couldn’t be saved.”</span></span>

### <a name="workaround"></a><span data-ttu-id="4d0f7-160">פתרון</span><span class="sxs-lookup"><span data-stu-id="4d0f7-160">Workaround</span></span>

1. <span data-ttu-id="4d0f7-161">ודא כי למשתמש הוקצה הרישיון הנכון וכי השירות מופעל בפרטי תוכניות השירות של הרישיון.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-161">Verify that the user has been assigned the correct license and that the service is enabled in the service plans details of the license.</span></span>
2. <span data-ttu-id="4d0f7-162">ודא שהמשתמש יכול לפתוח את project.microsoft.com.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-162">Verify that the user can open project.microsoft.com.</span></span>
3. <span data-ttu-id="4d0f7-163">ודא שהמערכת מצביעה על נקודת קצה של הפרוייקט הנכון.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-163">Verify that the system is pointing to the correct project endpoint,.</span></span>
4. <span data-ttu-id="4d0f7-164">ודא שהמשתמש ביישום הפרוייקט נוצר.</span><span class="sxs-lookup"><span data-stu-id="4d0f7-164">Verify that the Project Application user has been created.</span></span>
5. <span data-ttu-id="4d0f7-165">החל את תפקידי האבטחה הבאים על המשתמש:</span><span class="sxs-lookup"><span data-stu-id="4d0f7-165">Apply the following security roles to the user:</span></span>
  
  - <span data-ttu-id="4d0f7-166">משתמש Dataverse או משתמש בסיס</span><span class="sxs-lookup"><span data-stu-id="4d0f7-166">Dataverse user or Base user</span></span>
  - <span data-ttu-id="4d0f7-167">מערכת Project Operations</span><span class="sxs-lookup"><span data-stu-id="4d0f7-167">Project Operations System</span></span>
  - <span data-ttu-id="4d0f7-168">מערכת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="4d0f7-168">Project System</span></span>
  - <span data-ttu-id="4d0f7-169">מערכת כתיבה כפולה של Project Operations (תפקיד זה נדרש אם אתה פורס את התרחיש מבוסס המשאב/שאינו מלאי של Project Operations.)</span><span class="sxs-lookup"><span data-stu-id="4d0f7-169">Project Operations Dual Write System (This role is required if you are deploying the resource/non-stocked based scenario of Project Operations.)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]