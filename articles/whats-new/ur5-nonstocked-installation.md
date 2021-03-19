---
title: עדכן את Project Operations בסביבת Finance שלך
description: נושא זה מספק מידע על עדכון של Project Operations בסביבת Dynamics 365 Finance שלך.
author: ruhercul
manager: tfehr
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: d68296ec59f0bd58f848154c90e02c58f275ab12
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5291980"
---
# <a name="update-project-operations-in-your-finance-environment"></a><span data-ttu-id="490dd-103">עדכן את Project Operations בסביבת Finance שלך</span><span class="sxs-lookup"><span data-stu-id="490dd-103">Update Project Operations in your Finance environment</span></span>

<span data-ttu-id="490dd-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="490dd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="490dd-105">נושא זה מספק מידע על עדכון של Dynamics 365 Project Operations בסביבת Dynamics 365 Finance שלך.</span><span class="sxs-lookup"><span data-stu-id="490dd-105">This topic provides information about how to update Dynamics 365 Project Operations in your Dynamics 365 Finance environment.</span></span> <span data-ttu-id="490dd-106">יש שלושה נהלים הנדרשים לעדכון Project Operations לעדכון 5 (UR5):</span><span class="sxs-lookup"><span data-stu-id="490dd-106">There are three procedures that are required to update Project Operations to Update 5 (UR5):</span></span>

- [<span data-ttu-id="490dd-107">ייבא את החבילה לפרוייקט Preview שלך</span><span class="sxs-lookup"><span data-stu-id="490dd-107">Import the package into your preview project</span></span>](#import)
- [<span data-ttu-id="490dd-108">החל את העדכון</span><span class="sxs-lookup"><span data-stu-id="490dd-108">Apply the update</span></span>](#apply)
- [<span data-ttu-id="490dd-109">עדכן את סביבת Dataverse שלך</span><span class="sxs-lookup"><span data-stu-id="490dd-109">Update your Dataverse environment</span></span>](#update)

## <a name="import-the-package-into-your-lcs-project"></a><a name="import"></a><span data-ttu-id="490dd-110">ייבא את החבילה לפרוייקט LCS שלך</span><span class="sxs-lookup"><span data-stu-id="490dd-110">Import the package into your LCS project</span></span>

1. <span data-ttu-id="490dd-111">היכנס אל [Lifecycle Services ‏(LCS)](https://lcs.dynamics.com/) בתור בעל פרוייקט או מנהל סביבה.</span><span class="sxs-lookup"><span data-stu-id="490dd-111">Sign in to [Lifecycle Services (LCS)](https://lcs.dynamics.com/) as a Project Owner or Environment manager.</span></span>
2. <span data-ttu-id="490dd-112">בחר פרוייקט LCS מרשימת הפרוייקטים.</span><span class="sxs-lookup"><span data-stu-id="490dd-112">From the list of projects, select your LCS project.</span></span>
3. <span data-ttu-id="490dd-113">בדף **פרוייקטים**, בקבוצה **סביבות**, פתח את הסביבה שברצונך לעדכן.</span><span class="sxs-lookup"><span data-stu-id="490dd-113">On the **Project** page, in the **Environments** group, open the environment that you want to update.</span></span>
4. <span data-ttu-id="490dd-114">ודא שהסביבה פועלת.</span><span class="sxs-lookup"><span data-stu-id="490dd-114">Verify that the environment is running.</span></span> <span data-ttu-id="490dd-115">אם זה לא התחיל, התחל את הסביבה.</span><span class="sxs-lookup"><span data-stu-id="490dd-115">If it isn't started, start the environment.</span></span>
5. <span data-ttu-id="490dd-116">במקטע **הוצאה חדשה** תחת **עדכונים זמינים**, בחר **הצג עדכון** עבור 10.0.15.</span><span class="sxs-lookup"><span data-stu-id="490dd-116">In the **New release** section under **Available updates**, select **View update** for 10.0.15.</span></span>

![הצג את לחצן עדכון](media/view-update.png)

6. <span data-ttu-id="490dd-118">בדף **עדכונים בינאריים**, בחר **שמור חבילה**.</span><span class="sxs-lookup"><span data-stu-id="490dd-118">On the **Binary updates** page, select **Save package**.</span></span>
7. <span data-ttu-id="490dd-119">בדף **בדוק ושמור עדכונים**, בחר **שמור חבילה**.</span><span class="sxs-lookup"><span data-stu-id="490dd-119">On the **Review and save updates** page, select **Save package**.</span></span>
8. <span data-ttu-id="490dd-120">בחלונית **שמור חבילה בספריית הנכסים** שנפתחת, הזן את שם החבילה ובחר **שמור חבילה**.</span><span class="sxs-lookup"><span data-stu-id="490dd-120">On the **Save package to asset library** pane that opens, enter the package name and then select **Save package**.</span></span>
9. <span data-ttu-id="490dd-121">כאשר LCS סיים לשמור את החבילה, לחצן **בוצע** פעיל.</span><span class="sxs-lookup"><span data-stu-id="490dd-121">When LCS has finished saving the package, the **Done** button is enabled.</span></span> <span data-ttu-id="490dd-122">בחר **סיום**.</span><span class="sxs-lookup"><span data-stu-id="490dd-122">Select **Done**.</span></span> <span data-ttu-id="490dd-123">LCS יאמת את החבילה.</span><span class="sxs-lookup"><span data-stu-id="490dd-123">LCS will verify the package.</span></span> <span data-ttu-id="490dd-124">האימות יכול לקחת מספר דקות או עד שעה.</span><span class="sxs-lookup"><span data-stu-id="490dd-124">Verification can take a few minutes or up to one hour.</span></span>


## <a name="apply-the-package-update"></a><a name="apply"></a><span data-ttu-id="490dd-125">החל את עדכון החבילה</span><span class="sxs-lookup"><span data-stu-id="490dd-125">Apply the package update</span></span>

1. <span data-ttu-id="490dd-126">ב-LCS, בדף **פרטי סביבה** בחר **תחזוקה** > **החל עדכונים**.</span><span class="sxs-lookup"><span data-stu-id="490dd-126">In LCS, on the **Environment details** page, select **Maintain** > **Apply Updates**.</span></span>
2. <span data-ttu-id="490dd-127">ברשימה בחר את החבילה ששמרת קודם לכן ובחר **החל**.</span><span class="sxs-lookup"><span data-stu-id="490dd-127">From the list, select the package that you saved earlier, and then select **Apply**.</span></span>
3. <span data-ttu-id="490dd-128">בחר **כן** כדי לאשר שברצונך לפרוס את החבילה.</span><span class="sxs-lookup"><span data-stu-id="490dd-128">Select **Yes** to confirm that you want to deploy the package.</span></span>

![אשר את תיבת הדו-שיח של פריסת החבילה](media/confirm-package-deployment.png)

4. <span data-ttu-id="490dd-130">בחר **כן** כדי לאשר שברצונך לעדכן את היישום.</span><span class="sxs-lookup"><span data-stu-id="490dd-130">Select **Yes** to confirm that you want to update the application.</span></span>

![אשר את תיבת הדו-שיח של עדכון היישום](media/confirm-application-update.png)

<span data-ttu-id="490dd-132">הפריסה ועדכון היישום יתחילו.</span><span class="sxs-lookup"><span data-stu-id="490dd-132">The deployment and application update will start.</span></span> 

<span data-ttu-id="490dd-133">בדף **פרטי סביבה**, בפינה השמאלית העליונה, מצב הסביבה יתעדכן ויהיה **מתן שירות**.</span><span class="sxs-lookup"><span data-stu-id="490dd-133">On the **Environment details** page, in the top-right corner, the environment status will update to **Servicing**.</span></span> <span data-ttu-id="490dd-134">בעוד כשעתיים העדכון יושלם.</span><span class="sxs-lookup"><span data-stu-id="490dd-134">In approximately two hours, the update will be complete.</span></span> <span data-ttu-id="490dd-135">המידע על שחרור היישום יתעדכן ויהיה **Microsoft Dynamics 365 for Finance and Operations 10.0.15)** ומצב הסביבה יתעדכן ויהיה **נפרס**.</span><span class="sxs-lookup"><span data-stu-id="490dd-135">The application release information will update to **Microsoft Dynamics 365 for Finance and Operations 10.0.15)** and the environment status will update to **Deployed**.</span></span>


## <a name="update-your-dataverse-environment"></a><span data-ttu-id="490dd-136"><a name="update">עדכן את</a> סביבת Dataverse שלך</span><span class="sxs-lookup"><span data-stu-id="490dd-136"><a name="update"></a>Update your Dataverse environment</span></span>

1. <span data-ttu-id="490dd-137">היכנס אל [מרכז הניהול של Power Platform](https://admin.powerplatform.com/).</span><span class="sxs-lookup"><span data-stu-id="490dd-137">Sign in to the [Power Platform admin center](https://admin.powerplatform.com/).</span></span>
2. <span data-ttu-id="490dd-138">ברשימה, מצא ופתח את הסביבה שבה השתמשת להתקנת Project Operations.</span><span class="sxs-lookup"><span data-stu-id="490dd-138">In the list, find and open the environment that you used to install Project Operations.</span></span>
3. <span data-ttu-id="490dd-139">בדף **סביבות** בחר **משאב** > **יישומי Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="490dd-139">On the **Environments** page, select **Resource** > **Dynamics 365 apps**.</span></span>
4. <span data-ttu-id="490dd-140">ברשימה מצא את **Microsoft Dynamics 365 Project Operations**, ובעמודה **מצב** בחר **עדכון זמין**.</span><span class="sxs-lookup"><span data-stu-id="490dd-140">In the list, locate **Microsoft Dynamics 365 Project Operations**, and in the **Status** column, select **Update Available**.</span></span>
5. <span data-ttu-id="490dd-141">בחר את תיבת הסימון **אני מסכים לתנאי השימוש** ובחר **עדכון**.</span><span class="sxs-lookup"><span data-stu-id="490dd-141">Select the **I agree to the terms of service** check box, and then select **Update**.</span></span> <span data-ttu-id="490dd-142">הגרסה האחרונה של הפתרון תותקן.</span><span class="sxs-lookup"><span data-stu-id="490dd-142">The latest version of the solution will be installed.</span></span>

<span data-ttu-id="490dd-143">לאחר השלמת ההתקנה, תהיה לך גירסה 4.5.0.134.</span><span class="sxs-lookup"><span data-stu-id="490dd-143">After the installation is complete, you'll have version 4.5.0.134 installed.</span></span>

## <a name="configure-new-features"></a><span data-ttu-id="490dd-144">הגדרת תכונות חדשות</span><span class="sxs-lookup"><span data-stu-id="490dd-144">Configure new features</span></span>

### <a name="enable-dual-write-mapping"></a><span data-ttu-id="490dd-145">אפשר מיפוי כתיבה כפולה</span><span class="sxs-lookup"><span data-stu-id="490dd-145">Enable dual-write mapping</span></span>

<span data-ttu-id="490dd-146">אחרי השלמת העדכון בסביבות Finance ו- Dataverse, תוכל להפעיל את מיפויי הכתיבה הכפולה הנדרשים.</span><span class="sxs-lookup"><span data-stu-id="490dd-146">After you complete the update on the Finance and Dataverse environments, you can enable the required dual-write mappings.</span></span> <span data-ttu-id="490dd-147">השלם את הפרוצדורות הבאות כדי להפעיל מיפויי כתיבה כפולה.</span><span class="sxs-lookup"><span data-stu-id="490dd-147">Complete the following procedures to enable dual-write mappings.</span></span>

- [<span data-ttu-id="490dd-148">עדכן את הגדרות האבטחה בסביבת Customer Engagement</span><span class="sxs-lookup"><span data-stu-id="490dd-148">Update security settings on Customer Engagement environment</span></span>](#security)
- [<span data-ttu-id="490dd-149">רענון ישויות נתונים</span><span class="sxs-lookup"><span data-stu-id="490dd-149">Refresh data entities</span></span>](#refresh)
- [<span data-ttu-id="490dd-150">עדכן והפעל את מיפויי הכתיבה הכפולה</span><span class="sxs-lookup"><span data-stu-id="490dd-150">Update and run the dual-write mappings</span></span>](#run)

### <a name="update-security-settings-on-the-dataverse-environment"></a><a name="security"></a><span data-ttu-id="490dd-151">עדכן את הגדרות האבטחה בסביבת Dataverse</span><span class="sxs-lookup"><span data-stu-id="490dd-151">Update security settings on the Dataverse environment</span></span>

<span data-ttu-id="490dd-152">העדכונים הבאים להרשאות האבטחה עבור ישויות נדרשים כחלק מהעדכון ל- UR5.</span><span class="sxs-lookup"><span data-stu-id="490dd-152">The following updates to the security privileges for entities are required as part of the update to UR5.</span></span>

1. <span data-ttu-id="490dd-153">בסביבת Dataverse שלך עבור אל **הגדרות**, ובקבוצה **מערכת** בחר **אבטחה**.</span><span class="sxs-lookup"><span data-stu-id="490dd-153">In your Dataverse environment, go to **Settings**, and in the **System** group, select **Security**.</span></span>

![Dataverse הגדרות סביבה](media/Picture21.png)

2. <span data-ttu-id="490dd-155">בחר **תפקידי אבטחה**.</span><span class="sxs-lookup"><span data-stu-id="490dd-155">Select **Security Roles**.</span></span>
3. <span data-ttu-id="490dd-156">ברשימת התפקידים, בחר **משתמש באפליקציה עם כתיבה כפולה** ובחר את הכרטיסיה **ישויות מותאמות אישית**.</span><span class="sxs-lookup"><span data-stu-id="490dd-156">From the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span> 
4. <span data-ttu-id="490dd-157">ודא שיש לתפקיד הרשאות **קריאה** ו **צירוף** עבור:</span><span class="sxs-lookup"><span data-stu-id="490dd-157">Verify that the role has **Read** and **Append To** permissions for:</span></span>

      - <span data-ttu-id="490dd-158">**סוג שער החליפין של מטבע**</span><span class="sxs-lookup"><span data-stu-id="490dd-158">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="490dd-159">**תרשים של תיקי לקוחות**</span><span class="sxs-lookup"><span data-stu-id="490dd-159">**Chart Of Accounts**</span></span> 
      - <span data-ttu-id="490dd-160">**לוח שנה כספי**</span><span class="sxs-lookup"><span data-stu-id="490dd-160">**Fiscal Calendar**</span></span> 
      - <span data-ttu-id="490dd-161">**ספר חשבונות**</span><span class="sxs-lookup"><span data-stu-id="490dd-161">**Ledger**</span></span>

5. <span data-ttu-id="490dd-162">לאחר עדכון תפקיד האבטחה, עבור אל **הגדרות** > **אבטחה** > **Teams**.</span><span class="sxs-lookup"><span data-stu-id="490dd-162">After the security role is updated, go to **Settings** > **Security** > **Teams**.</span></span> <span data-ttu-id="490dd-163">ודא שהתפקיד **משתמש באפליקציה עם כתיבה כפולה** הוחל על הצוות.</span><span class="sxs-lookup"><span data-stu-id="490dd-163">Verify that the **dual-write app user** role has been applied to the team.</span></span> 

### <a name="refresh-data-entities-from-the-update"></a><a name="refresh"></a><span data-ttu-id="490dd-164">רענן ישויות נתונים מהעדכון</span><span class="sxs-lookup"><span data-stu-id="490dd-164">Refresh data entities from the update</span></span>

1. <span data-ttu-id="490dd-165">בסביבת Finance שלך, פתח את סביבת העבודה **ניהול נתונים** ופתח את הדף **פרמטרים של מסגרת**.</span><span class="sxs-lookup"><span data-stu-id="490dd-165">In your Finance environment, open the **Data management** workspace, and then open the **Framework parameters** page.</span></span>
2. <span data-ttu-id="490dd-166">בכרטיסיה **הגדרות ישויות** בחר **רענן רשימת ישויות**.</span><span class="sxs-lookup"><span data-stu-id="490dd-166">On the **Entity settings** tab, select **Refresh entity list**.</span></span>
3. <span data-ttu-id="490dd-167">בחר **סגור** כדי לאשר את רענון הישות.</span><span class="sxs-lookup"><span data-stu-id="490dd-167">Select **Close** to confirm the entity refresh.</span></span>

 > [!NOTE]
 > <span data-ttu-id="490dd-168">תהליך זה יימשך כ- 20 דקות.</span><span class="sxs-lookup"><span data-stu-id="490dd-168">This process will take approximately 20 minutes to complete.</span></span> <span data-ttu-id="490dd-169">תקבל הודעה על סיום הרענון.</span><span class="sxs-lookup"><span data-stu-id="490dd-169">You will be notified when the refresh is complete.</span></span>

### <a name="update-dual-write-mappings"></a><a name="run"></a><span data-ttu-id="490dd-170">עדכן מיפויי כתיבה כפולה</span><span class="sxs-lookup"><span data-stu-id="490dd-170">Update dual-write mappings</span></span>

1. <span data-ttu-id="490dd-171">בסביבת העבודה **ניהול נתונים** בחר **כתיבה כפולה**.</span><span class="sxs-lookup"><span data-stu-id="490dd-171">In the **Data management** workspace, select **Dual-write**.</span></span>
2. <span data-ttu-id="490dd-172">בחר **החל פתרונות**, בחר את שני הפתרונות ברשימה ובחר **החל**.</span><span class="sxs-lookup"><span data-stu-id="490dd-172">Select **Apply solutions**, select both solutions in the list, and then select **Apply**.</span></span>
3. <span data-ttu-id="490dd-173">בדף **כתיבה כפולה** בחר את מפות הטבלה הבאות ולאחר מכן בחר **הפסק**.</span><span class="sxs-lookup"><span data-stu-id="490dd-173">On the **Dual-write** page, select the following table maps, and then select **Stop**.</span></span>

    - <span data-ttu-id="490dd-174">**שילוב Project Operations עם נתונים בפועל (msdyn_actuals)**</span><span class="sxs-lookup"><span data-stu-id="490dd-174">**Project Operations integration actuals (msdyn_actuals)**</span></span>
    - <span data-ttu-id="490dd-175">**קטגוריות הוצאות של פרוייקט שילוב Project Operations ‏(msdyn_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="490dd-175">**Project Operations integration project expense categories (msdyn_expensecategories)**</span></span>
    - <span data-ttu-id="490dd-176">**ישות הוצאות של פרוייקט עם שילוב נתונים בפועל של Project Operations ‏(msdyn_expenses)**</span><span class="sxs-lookup"><span data-stu-id="490dd-176">**Project Operations integration actuals project expenses export entity (msdyn_expenses)**</span></span>

4. <span data-ttu-id="490dd-177">בדף **גרסת מפת טבלה**, החל גרסה חדשה של המפה על כל אחת משלוש הישויות.</span><span class="sxs-lookup"><span data-stu-id="490dd-177">On the **Table map version** page, apply a new version of the map to each of the three entities.</span></span>
5. <span data-ttu-id="490dd-178">בדף **כתיבה כפולה**, בחר 'הפעל' כדי להפעיל מחדש את המפות.</span><span class="sxs-lookup"><span data-stu-id="490dd-178">On the **Dual-write** page, select run to restart the maps.</span></span>
6. <span data-ttu-id="490dd-179">מרשימת המפות בחר את המפה **ספר חשבונות (msdyn_ledgers)** עם כל התנאים המוקדמים ובחר את תיבת הסימון **סנכרון ראשוני**.</span><span class="sxs-lookup"><span data-stu-id="490dd-179">From the list of maps, select the **Ledger (msdyn_ledgers)** map with all prerequisites and select the **Initial sync** check box.</span></span> 
7. <span data-ttu-id="490dd-180">בשדה **פריט ראשוני לסנכרון ראשוני**, בחר **יישומי Finance and Operations** ובחר **הפעל**.</span><span class="sxs-lookup"><span data-stu-id="490dd-180">In the **Master for initial sync** field, select **Finance and Operations apps** and then select **Run**.</span></span>
 
 ![סנכרון מפת ספר חשבונאות](media/DW6.png)
 


[!INCLUDE[footer-include](../includes/footer-banner.md)]