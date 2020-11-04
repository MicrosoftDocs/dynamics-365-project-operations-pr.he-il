---
title: הקצאת סביבה חדשה
description: נושא זה מספק מידע אודות אופן הקצאת סביבת Project Operations חדשה.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a43b947207b6d4276ef27ec996713bf3883e7906
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077195"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="811b7-103">הקצאת סביבה חדשה</span><span class="sxs-lookup"><span data-stu-id="811b7-103">Provision a new environment</span></span>

<span data-ttu-id="811b7-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="811b7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="811b7-105">נושא זה מספק מידע אודות אופן הקצאת סביבת Dynamics 365 Project Operations חדשה לתרחישים מבוססי משאבים/ללא מלאי.</span><span class="sxs-lookup"><span data-stu-id="811b7-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="811b7-106">הפוך הקצאת משאבים אוטומטית של Project Operations לזמינה בפרויקט LCS</span><span class="sxs-lookup"><span data-stu-id="811b7-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="811b7-107">השתמש בשלבים הבאים כדי להפוך את זרימת הקצאת המשאבים האוטומטית של Project Operations לאוטומטית עבור פרויקט LCS שלך.</span><span class="sxs-lookup"><span data-stu-id="811b7-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="811b7-108">עבור אל [LCS](https://lcs.dynamics.com/v2) ובחר את האריח **ניהול תכונת תצוגה מקדימה**.</span><span class="sxs-lookup"><span data-stu-id="811b7-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="811b7-109">ברשימת **תכונות התצוגה המקדימה** , בחר **תכונת Project Operations** ואז בחר **תכונת Preview זמינה** כדי להפוך את Project Operations לזמין.</span><span class="sxs-lookup"><span data-stu-id="811b7-109">In the **Preview feature** list, select **Project Operations Feature** , and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="811b7-110">שלב זה מבוצע פעם אחת בלבד לכל פרויקט LCS.</span><span class="sxs-lookup"><span data-stu-id="811b7-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="811b7-111">הקצאת סביבת Project Operations</span><span class="sxs-lookup"><span data-stu-id="811b7-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="811b7-112">פתח פריסה חדשה של Dynamics 365 Finance [סביבת הדגמה](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) או [סביבת ארגז חול/ ייצור](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure).</span><span class="sxs-lookup"><span data-stu-id="811b7-112">Open a new Dynamics 365 Finance [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="811b7-113">הסבר על אשף **הקצאת הסביבה**.</span><span class="sxs-lookup"><span data-stu-id="811b7-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="811b7-114">ודא שגירסת היישום שנבחרה היא 10.0.13 ומעלה.</span><span class="sxs-lookup"><span data-stu-id="811b7-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="811b7-115">להקצאת Project Operations, תחת **הגדרות מתקדמות** , בחר **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="811b7-115">To provision Project Operations, under **Advance settings** , select **Common Data Service**.</span></span> 
4. <span data-ttu-id="811b7-116">הפוך את **הגדרת Common Data Service** לזמינה על-ידי בחירת **כן** ואז הזן מידע בשדות הנדרשים:</span><span class="sxs-lookup"><span data-stu-id="811b7-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="811b7-117">שם</span><span class="sxs-lookup"><span data-stu-id="811b7-117">Name</span></span>
  - <span data-ttu-id="811b7-118">אזור</span><span class="sxs-lookup"><span data-stu-id="811b7-118">Region</span></span>
  - <span data-ttu-id="811b7-119">שפה</span><span class="sxs-lookup"><span data-stu-id="811b7-119">Language</span></span>
  - <span data-ttu-id="811b7-120">מטבע</span><span class="sxs-lookup"><span data-stu-id="811b7-120">Currency</span></span>
 
5. <span data-ttu-id="811b7-121">בשדה **תבנית Common Data Service** , בחר **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="811b7-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="811b7-122">בחר את סוג הסביבה לפריסה.</span><span class="sxs-lookup"><span data-stu-id="811b7-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="811b7-123">גירסת ניסיון מבוססת-מנוי תאפשר לך לפרוס סביבת CDS למשך 30 יום.</span><span class="sxs-lookup"><span data-stu-id="811b7-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![הגדרות פריסה](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="811b7-125">בחר **מסכים** כדי להסכם לתנאי השירות ואז בחר **סיום** כדי לחזור להגדרות הפריסה.</span><span class="sxs-lookup"><span data-stu-id="811b7-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![הסכמת פריסה](./media/2DeploymentConsent.png)

7. <span data-ttu-id="811b7-127">מלא את שאר השדות הנדרשים באשף ואשר את הפריסה.</span><span class="sxs-lookup"><span data-stu-id="811b7-127">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="811b7-128">זמן הקצאת הסביבה משתנה בהתאם לסוג הסביבה.</span><span class="sxs-lookup"><span data-stu-id="811b7-128">Environment provisioning time varies based on the environment type.</span></span> <span data-ttu-id="811b7-129">ההקצאה עשויה להימשך עד שש שעות.</span><span class="sxs-lookup"><span data-stu-id="811b7-129">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="811b7-130">לאחר השלמת הפריסה בהצלחה, הסביבה תוצג בתור **פרוסה**.</span><span class="sxs-lookup"><span data-stu-id="811b7-130">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

8. <span data-ttu-id="811b7-131">כדי לאשר שהסביבה נפרסה בהצלחה, בחר **כניסה** והיכנס לסביבה כדי לאשר.</span><span class="sxs-lookup"><span data-stu-id="811b7-131">To confirm the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![פרטי סביבת ](./media/3EnvironmentDetails.png)

## <a name="apply-project-operations-finance-demo-data-optional-step"></a><span data-ttu-id="811b7-133">החל את נתוני ההדגמה של Project Operations Finance (שלב אופציונלי)</span><span class="sxs-lookup"><span data-stu-id="811b7-133">Apply Project Operations Finance demo data (optional step)</span></span>

<span data-ttu-id="811b7-134">החל את נתוני ההדגמה של Project Operations Finance בסביבה המתארחת בענן במהדורת שירות 10.0.13 כמתואר [במאמר הזה](resource-apply-finance-demo-data.md).</span><span class="sxs-lookup"><span data-stu-id="811b7-134">Apply Project Operations Finance demo data to 10.0.13 service release Cloud Hosted Environment as described in [this article](resource-apply-finance-demo-data.md).</span></span>

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="811b7-135">החל עדכונים על סביבת Finance</span><span class="sxs-lookup"><span data-stu-id="811b7-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="811b7-136">ל- Project Operations נדרשת סביבת Finance עם גירסת יישום **10.0.13 (10.0.569.20009)** ומעלה.</span><span class="sxs-lookup"><span data-stu-id="811b7-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="811b7-137">ייתכן שתצטרך להחיל עדכוני איכות על סביבת Finance שלך כדי לקבל גירסה זו.</span><span class="sxs-lookup"><span data-stu-id="811b7-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="811b7-138">ב- LCS, בדף **פרטי הסביבה** , במקטע **עדכונים זמינים** , בחר **הצג עדכון**.</span><span class="sxs-lookup"><span data-stu-id="811b7-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![הצג עדכונים](./media/5ViewUpdates.png)

2. <span data-ttu-id="811b7-140">בדף **עדכונים בינאריים** , בחר **שמור חבילה.**</span><span class="sxs-lookup"><span data-stu-id="811b7-140">On the **Binary updates** page, select **Save package.**</span></span>

![שמור חבילה](./media/6SavePackage.png)

3. <span data-ttu-id="811b7-142">לחץ על **בחר הכל** ולאחר מכן בחר **שמור חבילה**.</span><span class="sxs-lookup"><span data-stu-id="811b7-142">Click **Select all** and then select **Save package**.</span></span>

![סקור ושמור עדכונים](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="811b7-144">הזן שם ותיאור לחבילה ולאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="811b7-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="811b7-145">בהתאם לחיבור האינטרנט, תהליך זה עשוי להימשך זמן מה.</span><span class="sxs-lookup"><span data-stu-id="811b7-145">Depending on the internet connection, this process might take some time.</span></span>

![העלה חבילה לספריית הנכסים](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="811b7-147">לאחר שמירת החבילה, בחר **סיום** ושמור חבילה זו בספריית הנכסים בפרויקט LCS שלך.</span><span class="sxs-lookup"><span data-stu-id="811b7-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="811b7-148">שמירת ואימות החבילה עשויה לארוך כ- 15 דקות.</span><span class="sxs-lookup"><span data-stu-id="811b7-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="811b7-149">כדי להחיל את העדכון, נווט אל הדף **פרטי הסביבה** ב- LCS ובחר **תחזק** > **החל עדכונים**.</span><span class="sxs-lookup"><span data-stu-id="811b7-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![תחזק סביבות](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="811b7-151">ברשימת העדכונים, בחר את החבילה שיצרת ובחר **החל**.</span><span class="sxs-lookup"><span data-stu-id="811b7-151">In the updates list select the package you created, and select **Apply**.</span></span>

![החל עדכונים](./media/10ApplyUpdates.png)

<span data-ttu-id="811b7-153">מתן השירות לסביבה ייקח זמן מה.</span><span class="sxs-lookup"><span data-stu-id="811b7-153">Environment servicing will take some time.</span></span> <span data-ttu-id="811b7-154">לאחר ההשלמה, הסביבה תחזור למצב פרוס.</span><span class="sxs-lookup"><span data-stu-id="811b7-154">After it is complete, the environment will return to a deployed state.</span></span>

![סביבה פרוסה](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="811b7-156">יצירת חיבור כתיבה כפולה</span><span class="sxs-lookup"><span data-stu-id="811b7-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="811b7-157">בפרויקט LCS שלך, עבור אל הדף **פרטי סביבה**.</span><span class="sxs-lookup"><span data-stu-id="811b7-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="811b7-158">בקטע **פרטי סביבה של Common Data Service** , בחר **קישור ל- CDS עבור יישומים**.</span><span class="sxs-lookup"><span data-stu-id="811b7-158">Under **Common Data Service Environment Information** , select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="811b7-159">לאחר השלמת הקישור, בחר **קישור ל- CDS עבור יישומים** שוב.</span><span class="sxs-lookup"><span data-stu-id="811b7-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="811b7-160">תועבר לכתיבה כפולה ב- Finance.</span><span class="sxs-lookup"><span data-stu-id="811b7-160">You will be redirected to Dual Write in Finance.</span></span>

![קישור ל- CDS](./media/12LinktoCDS.png)

4. <span data-ttu-id="811b7-162">בחר **החל פתרון** כדי לגשת לישויות אשר ימופו בשילוב.</span><span class="sxs-lookup"><span data-stu-id="811b7-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![החל פתרונות](./media/13ApplySolutions.png)

5. <span data-ttu-id="811b7-164">בחר בשני הפתרונות **מפת ישות כתיבה כפולה ב- Dynamics 365 Finance and Operations** ו **מפות ישות כתיבה כפולה ב- Dynamics 365 Project Operations** ולאחר מכן בחר **החל**.</span><span class="sxs-lookup"><span data-stu-id="811b7-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps** , and then select **Apply**.</span></span>

![אשר פתרונות](./media/14ConfirmSolutions.png)

<span data-ttu-id="811b7-166">לאחר החלת הפתרונות, ישויות הכתיבה הכפולה מוחלות על הסביבה.</span><span class="sxs-lookup"><span data-stu-id="811b7-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![מחיל פתרונות](./media/15ApplyingSolutions.png)

<span data-ttu-id="811b7-168">לאחר החלת הישויות, כל המיפויים הזמינים רשומים בסביבה.</span><span class="sxs-lookup"><span data-stu-id="811b7-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![מפות של כתיבה כפולה](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="811b7-170">רענן את ישויות הנתונים לאחר העדכון</span><span class="sxs-lookup"><span data-stu-id="811b7-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="811b7-171">ב- Finance, עבור אל סביבת העבודה **ניהול נתונים**.</span><span class="sxs-lookup"><span data-stu-id="811b7-171">In Finance, go to the **Data management** workspace.</span></span>

![סביבת עבודה של ניהול נתונים](./media/16DataManagement.png)

2. <span data-ttu-id="811b7-173">בחר את האריח **פרמטרים של מסגרת**.</span><span class="sxs-lookup"><span data-stu-id="811b7-173">Select the **Framework parameters** tile.</span></span>

![פרמטרים של מסגרת](./media/17FrameworkParameters.png)

3. <span data-ttu-id="811b7-175">בדף **הגדרות ישות** , בחר **רענן את רשימת הישויות**.</span><span class="sxs-lookup"><span data-stu-id="811b7-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![רענן את רשימת הישויות](./media/18RefreshEntityList.png)

<span data-ttu-id="811b7-177">הרענון יימשך כ- 20 דקות.</span><span class="sxs-lookup"><span data-stu-id="811b7-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="811b7-178">תקבל התראה כשהוא יסתיים.</span><span class="sxs-lookup"><span data-stu-id="811b7-178">You will receive an alert when it is complete.</span></span>

![רענן אישור](./media/19RefreshConfirmation.png)

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="811b7-180">הפעל את מפות כתיבה כפולה ב- Project Operations</span><span class="sxs-lookup"><span data-stu-id="811b7-180">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="811b7-181">בפרויקט LCS שלך, עבור אל הדף **פרטי סביבה**.</span><span class="sxs-lookup"><span data-stu-id="811b7-181">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="811b7-182">בקטע **פרטי סביבה של Common Data Service** , בחר **קישור ל- CDS עבור יישומים.**</span><span class="sxs-lookup"><span data-stu-id="811b7-182">Under **Common Data Service Environment Information** , select **Link to CDS for Apps.**</span></span> <span data-ttu-id="811b7-183">לאחר שתבחרו בקישור, תועברו לרשימת הישויות במיפויים.</span><span class="sxs-lookup"><span data-stu-id="811b7-183">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="811b7-184">התחל את המפות כמתואר בטבלה הבאה.</span><span class="sxs-lookup"><span data-stu-id="811b7-184">Start the maps as described in the following table.</span></span> <span data-ttu-id="811b7-185">הקפד לעקוב אחר הרצף כמפורט.</span><span class="sxs-lookup"><span data-stu-id="811b7-185">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="811b7-186">**מפת ישויות**</span><span class="sxs-lookup"><span data-stu-id="811b7-186">**Entity Map**</span></span> | <span data-ttu-id="811b7-187">**רענן ישות**</span><span class="sxs-lookup"><span data-stu-id="811b7-187">**Refresh entity**</span></span> | <span data-ttu-id="811b7-188">**סינכרון ראשוני**</span><span class="sxs-lookup"><span data-stu-id="811b7-188">**Initial sync**</span></span> | <span data-ttu-id="811b7-189">**פריט ראשי לסינכרון ראשוני**</span><span class="sxs-lookup"><span data-stu-id="811b7-189">**Master for initial sync**</span></span> | <span data-ttu-id="811b7-190">**הפעל דרישות מוקדמות**</span><span class="sxs-lookup"><span data-stu-id="811b7-190">**Run prerequisites**</span></span> | <span data-ttu-id="811b7-191">**סינכרון ראשוני של דרישות מוקדמות**</span><span class="sxs-lookup"><span data-stu-id="811b7-191">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="811b7-192">**תפקידי משאבי פרויקט לכל החברות (bookableresourcecategories)**</span><span class="sxs-lookup"><span data-stu-id="811b7-192">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="811b7-193">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-193">No</span></span> | <span data-ttu-id="811b7-194">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="811b7-194">Yes</span></span> | <span data-ttu-id="811b7-195">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="811b7-195">Common Data Service</span></span> | <span data-ttu-id="811b7-196">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-196">No</span></span> | <span data-ttu-id="811b7-197">לא זמין</span><span class="sxs-lookup"><span data-stu-id="811b7-197">N\A</span></span> |
| <span data-ttu-id="811b7-198">**ישויות משפטיות (cdm\_companies)**</span><span class="sxs-lookup"><span data-stu-id="811b7-198">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="811b7-199">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-199">No</span></span> | <span data-ttu-id="811b7-200">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="811b7-200">Yes</span></span> | <span data-ttu-id="811b7-201">יישומי Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="811b7-201">Finance and Operations apps</span></span> | <span data-ttu-id="811b7-202">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-202">No</span></span> | <span data-ttu-id="811b7-203">לא זמין</span><span class="sxs-lookup"><span data-stu-id="811b7-203">N\A</span></span> |
| <span data-ttu-id="811b7-204">**שילוב Project Operations בפועל (msdyn\_actuals)**</span><span class="sxs-lookup"><span data-stu-id="811b7-204">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="811b7-205">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-205">No</span></span> | <span data-ttu-id="811b7-206">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-206">No</span></span> | <span data-ttu-id="811b7-207">לא זמין</span><span class="sxs-lookup"><span data-stu-id="811b7-207">N\A</span></span> | <span data-ttu-id="811b7-208">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="811b7-208">Yes</span></span> | <span data-ttu-id="811b7-209">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-209">No</span></span> |
| <span data-ttu-id="811b7-210">**סעיפי חוזה של פרויקט (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="811b7-210">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="811b7-211">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-211">No</span></span> | <span data-ttu-id="811b7-212">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-212">No</span></span> | <span data-ttu-id="811b7-213">לא זמין</span><span class="sxs-lookup"><span data-stu-id="811b7-213">N\A</span></span> | <span data-ttu-id="811b7-214">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-214">No</span></span> | <span data-ttu-id="811b7-215">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-215">No</span></span> |
| <span data-ttu-id="811b7-216">**‏‫ישות שילוב ליחסי גומלין של עסקה בפרויקט‬ (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="811b7-216">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="811b7-217">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-217">No</span></span> | <span data-ttu-id="811b7-218">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-218">No</span></span> | <span data-ttu-id="811b7-219">לא זמין</span><span class="sxs-lookup"><span data-stu-id="811b7-219">N\A</span></span> | <span data-ttu-id="811b7-220">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-220">No</span></span> | <span data-ttu-id="811b7-221">לא זמין</span><span class="sxs-lookup"><span data-stu-id="811b7-221">N\A</span></span> |
| <span data-ttu-id="811b7-222">**אבני דרך בסעיף חוזה לשילוב Project Operations (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="811b7-222">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="811b7-223">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-223">No</span></span> | <span data-ttu-id="811b7-224">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-224">No</span></span> | <span data-ttu-id="811b7-225">לא זמין</span><span class="sxs-lookup"><span data-stu-id="811b7-225">N\A</span></span> | <span data-ttu-id="811b7-226">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-226">No</span></span> | <span data-ttu-id="811b7-227">לא זמין</span><span class="sxs-lookup"><span data-stu-id="811b7-227">N\A</span></span> |
| <span data-ttu-id="811b7-228">**ישות שילוב Project Operations להערכת הוצאות (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="811b7-228">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="811b7-229">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-229">No</span></span> | <span data-ttu-id="811b7-230">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-230">No</span></span> | <span data-ttu-id="811b7-231">לא זמין</span><span class="sxs-lookup"><span data-stu-id="811b7-231">N\A</span></span> | <span data-ttu-id="811b7-232">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-232">No</span></span> | <span data-ttu-id="811b7-233">לא זמין</span><span class="sxs-lookup"><span data-stu-id="811b7-233">N\A</span></span> |
| <span data-ttu-id="811b7-234">**ישות ייצוא הוצאות פרויקט בשילוב Project Operations (msdyn\_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="811b7-234">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="811b7-235">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-235">No</span></span> | <span data-ttu-id="811b7-236">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-236">No</span></span> | <span data-ttu-id="811b7-237">לא זמין</span><span class="sxs-lookup"><span data-stu-id="811b7-237">N\A</span></span> | <span data-ttu-id="811b7-238">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-238">No</span></span> | <span data-ttu-id="811b7-239">לא זמין</span><span class="sxs-lookup"><span data-stu-id="811b7-239">N\A</span></span> |
| <span data-ttu-id="811b7-240">**ישות ייצוא הוצאות פרויקט בשילוב Project Operations (msdyn\_expenses)**</span><span class="sxs-lookup"><span data-stu-id="811b7-240">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="811b7-241">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="811b7-241">Yes</span></span> | <span data-ttu-id="811b7-242">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-242">No</span></span> | <span data-ttu-id="811b7-243">לא זמין</span><span class="sxs-lookup"><span data-stu-id="811b7-243">N\A</span></span> | <span data-ttu-id="811b7-244">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-244">No</span></span> | <span data-ttu-id="811b7-245">לא זמין</span><span class="sxs-lookup"><span data-stu-id="811b7-245">N\A</span></span> |
| <span data-ttu-id="811b7-246">**ישות שילוב Project Operations להערכת שעות (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="811b7-246">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="811b7-247">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="811b7-247">Yes</span></span> | <span data-ttu-id="811b7-248">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-248">No</span></span> | <span data-ttu-id="811b7-249">לא זמין</span><span class="sxs-lookup"><span data-stu-id="811b7-249">N\A</span></span> | <span data-ttu-id="811b7-250">Yes</span><span class="sxs-lookup"><span data-stu-id="811b7-250">No</span></span> | <span data-ttu-id="811b7-251">לא זמין</span><span class="sxs-lookup"><span data-stu-id="811b7-251">N\A</span></span> |


4. <span data-ttu-id="811b7-252">כדי לרענן את הישות, בחר את שם המפה ואז בחר **רענן ישויות**.</span><span class="sxs-lookup"><span data-stu-id="811b7-252">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![רענן מפה](./media/20RefreshMapping.png)

5. <span data-ttu-id="811b7-254">לאחר השלמת הרענון, הפעל את המפה.</span><span class="sxs-lookup"><span data-stu-id="811b7-254">After the refresh is complete, run the map.</span></span> <span data-ttu-id="811b7-255">לפני הפיכת המפה הבאה לזמינה, ודא שהמפה בטבלה במצב **פועלת**.</span><span class="sxs-lookup"><span data-stu-id="811b7-255">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="811b7-256">הפעלת מפות עם מספר גדול יותר של תנאים מוקדמים עשויה להימשך זמן מה.</span><span class="sxs-lookup"><span data-stu-id="811b7-256">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="811b7-257">להפעלת מפה עם תנאים מוקדמים, החלף את המצב של הלחצן **הצג מפות ישויות קשורות** לפועל.</span><span class="sxs-lookup"><span data-stu-id="811b7-257">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="811b7-258">אם הטבלה מציינת כי **סינכרון ראשוני של דרישות מוקדמות** הוא במצב **לא** , ודא שהדגל **סינכרון ראשוני** הוא **כבוי** בכל מפות הדרישה המוקדמת לפני שתפעיל אותה.</span><span class="sxs-lookup"><span data-stu-id="811b7-258">If the table indicates **Prerequisite initial sync** is **No** , verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![הפעל מפה](./media/21RunMap.png)

6. <span data-ttu-id="811b7-260">ודא שכל המפות הקשורות לפרויקט במצב פועל.</span><span class="sxs-lookup"><span data-stu-id="811b7-260">Validate all project related maps are in the running state.</span></span>

![כל המפות פועלות](./media/22AllMapsRunning.png)

<span data-ttu-id="811b7-262">סביבת Project Operations שלך מוקצית ומוגדרת כעת.</span><span class="sxs-lookup"><span data-stu-id="811b7-262">Your Project Operations environment is now provisioned and configured.</span></span>
