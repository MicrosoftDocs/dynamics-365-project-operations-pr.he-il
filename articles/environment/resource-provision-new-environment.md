---
title: הקצאת סביבה חדשה
description: נושא זה מספק מידע אודות אופן הקצאת סביבת Project Operations חדשה.
author: sigitac
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 9ed502a1312b702e029d8910d62f72b8e0e4df06
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642973"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="40154-103">הקצאת סביבה חדשה</span><span class="sxs-lookup"><span data-stu-id="40154-103">Provision a new environment</span></span>

<span data-ttu-id="40154-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="40154-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="40154-105">נושא זה מספק מידע על הדרך להקצות סביבת Dynamics 365 Project Operations חדשה לתרחישים מבוססי משאבים/ללא מלאי.</span><span class="sxs-lookup"><span data-stu-id="40154-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="40154-106">הפוך הקצאת משאבים אוטומטית של Project Operations לזמינה בפרויקט LCS</span><span class="sxs-lookup"><span data-stu-id="40154-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="40154-107">השתמש בשלבים הבאים כדי להפוך את זרימת הקצאת המשאבים האוטומטית של Project Operations לאוטומטית עבור פרויקט LCS שלך.</span><span class="sxs-lookup"><span data-stu-id="40154-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="40154-108">עבור אל [LCS](https://lcs.dynamics.com/v2) ובחר את האריח **ניהול תכונת תצוגה מקדימה**.</span><span class="sxs-lookup"><span data-stu-id="40154-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="40154-109">ברשימת **תכונות התצוגה המקדימה**, בחר **תכונת Project Operations** ואז בחר **תכונת Preview זמינה** כדי להפוך את Project Operations לזמין.</span><span class="sxs-lookup"><span data-stu-id="40154-109">In the **Preview feature** list, select **Project Operations Feature**, and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="40154-110">שלב זה מבוצע פעם אחת בלבד לכל פרויקט LCS.</span><span class="sxs-lookup"><span data-stu-id="40154-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="40154-111">הקצאת סביבת Project Operations</span><span class="sxs-lookup"><span data-stu-id="40154-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="40154-112">פתח פריסה חדשה של Dynamics 365 Finance [סביבת הדגמה](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) או [סביבת ארגז חול/ ייצור](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure).</span><span class="sxs-lookup"><span data-stu-id="40154-112">Open a new Dynamics 365 Finance [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="40154-113">הסבר על אשף **הקצאת הסביבה**.</span><span class="sxs-lookup"><span data-stu-id="40154-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="40154-114">ודא שגירסת היישום שנבחרה היא 10.0.13 ומעלה.</span><span class="sxs-lookup"><span data-stu-id="40154-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="40154-115">להקצאת Project Operations, תחת **הגדרות מתקדמות**, בחר **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="40154-115">To provision Project Operations, under **Advance settings**, select **Common Data Service**.</span></span> 
4. <span data-ttu-id="40154-116">הפוך את **הגדרת Common Data Service** לזמינה על-ידי בחירת **כן** ואז הזן מידע בשדות הנדרשים:</span><span class="sxs-lookup"><span data-stu-id="40154-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="40154-117">שם</span><span class="sxs-lookup"><span data-stu-id="40154-117">Name</span></span>
  - <span data-ttu-id="40154-118">אזור</span><span class="sxs-lookup"><span data-stu-id="40154-118">Region</span></span>
  - <span data-ttu-id="40154-119">שפה</span><span class="sxs-lookup"><span data-stu-id="40154-119">Language</span></span>
  - <span data-ttu-id="40154-120">מטבע</span><span class="sxs-lookup"><span data-stu-id="40154-120">Currency</span></span>
 
5. <span data-ttu-id="40154-121">בשדה **תבנית Common Data Service**, בחר **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="40154-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="40154-122">בחר את סוג הסביבה לפריסה.</span><span class="sxs-lookup"><span data-stu-id="40154-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="40154-123">גירסת ניסיון מבוססת-מנוי תאפשר לך לפרוס סביבת CDS למשך 30 יום.</span><span class="sxs-lookup"><span data-stu-id="40154-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![הגדרות פריסה](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="40154-125">בחר **מסכים** כדי להסכם לתנאי השירות ואז בחר **סיום** כדי לחזור להגדרות הפריסה.</span><span class="sxs-lookup"><span data-stu-id="40154-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![הסכמת פריסה](./media/2DeploymentConsent.png)

7. <span data-ttu-id="40154-127">מלא את שאר השדות הנדרשים באשף ואשר את הפריסה.</span><span class="sxs-lookup"><span data-stu-id="40154-127">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="40154-128">זמן הקצאת הסביבה משתנה בהתאם לסוג הסביבה.</span><span class="sxs-lookup"><span data-stu-id="40154-128">Environment provisioning time varies based on the environment type.</span></span> <span data-ttu-id="40154-129">ההקצאה עשויה להימשך עד שש שעות.</span><span class="sxs-lookup"><span data-stu-id="40154-129">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="40154-130">לאחר השלמת הפריסה בהצלחה, הסביבה תוצג בתור **פרוסה**.</span><span class="sxs-lookup"><span data-stu-id="40154-130">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

8. <span data-ttu-id="40154-131">כדי לאשר שהסביבה נפרסה בהצלחה, בחר **כניסה** והיכנס לסביבה כדי לאשר.</span><span class="sxs-lookup"><span data-stu-id="40154-131">To confirm the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![פרטי סביבת ](./media/3EnvironmentDetails.png)

## <a name="apply-project-operations-finance-demo-data-optional-step"></a><span data-ttu-id="40154-133">החל את נתוני ההדגמה של Project Operations Finance (שלב אופציונלי)</span><span class="sxs-lookup"><span data-stu-id="40154-133">Apply Project Operations Finance demo data (optional step)</span></span>

<span data-ttu-id="40154-134">החל את נתוני ההדגמה של Project Operations Finance בסביבה המתארחת בענן במהדורת שירות 10.0.13 כמתואר [במאמר הזה](resource-apply-finance-demo-data.md).</span><span class="sxs-lookup"><span data-stu-id="40154-134">Apply Project Operations Finance demo data to 10.0.13 service release Cloud Hosted Environment as described in [this article](resource-apply-finance-demo-data.md).</span></span>

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="40154-135">החל עדכונים על סביבת Finance</span><span class="sxs-lookup"><span data-stu-id="40154-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="40154-136">ל- Project Operations נדרשת סביבת Finance עם גירסת יישום **10.0.13 (10.0.569.20009)** ומעלה.</span><span class="sxs-lookup"><span data-stu-id="40154-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="40154-137">ייתכן שתצטרך להחיל עדכוני איכות על סביבת Finance שלך כדי לקבל גירסה זו.</span><span class="sxs-lookup"><span data-stu-id="40154-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="40154-138">ב- LCS, בדף **פרטי הסביבה**, במקטע **עדכונים זמינים**, בחר **הצג עדכון**.</span><span class="sxs-lookup"><span data-stu-id="40154-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![הצג עדכונים](./media/5ViewUpdates.png)

2. <span data-ttu-id="40154-140">בדף **עדכונים בינאריים**, בחר **שמור חבילה.**</span><span class="sxs-lookup"><span data-stu-id="40154-140">On the **Binary updates** page, select **Save package.**</span></span>

![שמור חבילה](./media/6SavePackage.png)

3. <span data-ttu-id="40154-142">לחץ על **בחר הכל** ולאחר מכן בחר **שמור חבילה**.</span><span class="sxs-lookup"><span data-stu-id="40154-142">Click **Select all** and then select **Save package**.</span></span>

![סקור ושמור עדכונים](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="40154-144">הזן שם ותיאור לחבילה ולאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="40154-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="40154-145">בהתאם לחיבור האינטרנט, תהליך זה עשוי להימשך זמן מה.</span><span class="sxs-lookup"><span data-stu-id="40154-145">Depending on the internet connection, this process might take some time.</span></span>

![העלה חבילה לספריית הנכסים](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="40154-147">לאחר שמירת החבילה, בחר **סיום** ושמור חבילה זו בספריית הנכסים בפרויקט LCS שלך.</span><span class="sxs-lookup"><span data-stu-id="40154-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="40154-148">שמירת ואימות החבילה עשויה לארוך כ- 15 דקות.</span><span class="sxs-lookup"><span data-stu-id="40154-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="40154-149">כדי להחיל את העדכון, נווט אל הדף **פרטי הסביבה** ב- LCS ובחר **תחזק** > **החל עדכונים**.</span><span class="sxs-lookup"><span data-stu-id="40154-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![תחזק סביבות](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="40154-151">ברשימת העדכונים, בחר את החבילה שיצרת ובחר **החל**.</span><span class="sxs-lookup"><span data-stu-id="40154-151">In the updates list select the package you created, and select **Apply**.</span></span>

![החל עדכונים](./media/10ApplyUpdates.png)

<span data-ttu-id="40154-153">מתן השירות לסביבה ייקח זמן מה.</span><span class="sxs-lookup"><span data-stu-id="40154-153">Environment servicing will take some time.</span></span> <span data-ttu-id="40154-154">לאחר ההשלמה, הסביבה תחזור למצב פרוס.</span><span class="sxs-lookup"><span data-stu-id="40154-154">After it is complete, the environment will return to a deployed state.</span></span>

![סביבה פרוסה](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="40154-156">יצירת חיבור כתיבה כפולה</span><span class="sxs-lookup"><span data-stu-id="40154-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="40154-157">בפרויקט LCS שלך, עבור אל הדף **פרטי סביבה**.</span><span class="sxs-lookup"><span data-stu-id="40154-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="40154-158">בקטע **פרטי סביבה של Common Data Service**, בחר **קישור ל- CDS עבור יישומים**.</span><span class="sxs-lookup"><span data-stu-id="40154-158">Under **Common Data Service Environment Information**, select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="40154-159">לאחר השלמת הקישור, בחר **קישור ל- CDS עבור יישומים** שוב.</span><span class="sxs-lookup"><span data-stu-id="40154-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="40154-160">תועבר לכתיבה כפולה ב- Finance.</span><span class="sxs-lookup"><span data-stu-id="40154-160">You will be redirected to Dual Write in Finance.</span></span>

![קישור ל- CDS](./media/12LinktoCDS.png)

4. <span data-ttu-id="40154-162">בחר **החל פתרון** כדי לגשת לישויות אשר ימופו בשילוב.</span><span class="sxs-lookup"><span data-stu-id="40154-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![החל פתרונות](./media/13ApplySolutions.png)

5. <span data-ttu-id="40154-164">בחר את שני הפתרונות, **מפת ישויות כתיבה כפולה של Dynamics 365 Finance and Operations** ו- **מפות ישויות כתיבה כפולה של Dynamics 365 Project Operations** ואז בחר **החל**.</span><span class="sxs-lookup"><span data-stu-id="40154-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps**, and then select **Apply**.</span></span>

![אשר פתרונות](./media/14ConfirmSolutions.png)

<span data-ttu-id="40154-166">לאחר החלת הפתרונות, ישויות הכתיבה הכפולה מוחלות על הסביבה.</span><span class="sxs-lookup"><span data-stu-id="40154-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![מחיל פתרונות](./media/15ApplyingSolutions.png)

<span data-ttu-id="40154-168">לאחר החלת הישויות, כל המיפויים הזמינים רשומים בסביבה.</span><span class="sxs-lookup"><span data-stu-id="40154-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![מפות של כתיבה כפולה](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="40154-170">רענן את ישויות הנתונים לאחר העדכון</span><span class="sxs-lookup"><span data-stu-id="40154-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="40154-171">ב- Finance, עבור אל סביבת העבודה **ניהול נתונים**.</span><span class="sxs-lookup"><span data-stu-id="40154-171">In Finance, go to the **Data management** workspace.</span></span>

![סביבת עבודה של ניהול נתונים](./media/16DataManagement.png)

2. <span data-ttu-id="40154-173">בחר את האריח **פרמטרים של מסגרת**.</span><span class="sxs-lookup"><span data-stu-id="40154-173">Select the **Framework parameters** tile.</span></span>

![פרמטרים של מסגרת](./media/17FrameworkParameters.png)

3. <span data-ttu-id="40154-175">בדף **הגדרות ישות**, בחר **רענן את רשימת הישויות**.</span><span class="sxs-lookup"><span data-stu-id="40154-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![רענן את רשימת הישויות](./media/18RefreshEntityList.png)

<span data-ttu-id="40154-177">הרענון יימשך כ- 20 דקות.</span><span class="sxs-lookup"><span data-stu-id="40154-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="40154-178">תקבל התראה כשהוא יסתיים.</span><span class="sxs-lookup"><span data-stu-id="40154-178">You will receive an alert when it is complete.</span></span>

![רענן אישור](./media/19RefreshConfirmation.png)

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="40154-180">הפעל את מפות כתיבה כפולה ב- Project Operations</span><span class="sxs-lookup"><span data-stu-id="40154-180">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="40154-181">בפרויקט LCS שלך, עבור אל הדף **פרטי סביבה**.</span><span class="sxs-lookup"><span data-stu-id="40154-181">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="40154-182">בקטע **פרטי סביבה של Common Data Service**, בחר **קישור ל- CDS עבור יישומים.**</span><span class="sxs-lookup"><span data-stu-id="40154-182">Under **Common Data Service Environment Information**, select **Link to CDS for Apps.**</span></span> <span data-ttu-id="40154-183">לאחר שתבחרו בקישור, תועברו לרשימת הישויות במיפויים.</span><span class="sxs-lookup"><span data-stu-id="40154-183">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="40154-184">התחל את המפות כמתואר בטבלה הבאה.</span><span class="sxs-lookup"><span data-stu-id="40154-184">Start the maps as described in the following table.</span></span> <span data-ttu-id="40154-185">הקפד לעקוב אחר הרצף כמפורט.</span><span class="sxs-lookup"><span data-stu-id="40154-185">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="40154-186">**מפת ישויות**</span><span class="sxs-lookup"><span data-stu-id="40154-186">**Entity Map**</span></span> | <span data-ttu-id="40154-187">**רענן ישות**</span><span class="sxs-lookup"><span data-stu-id="40154-187">**Refresh entity**</span></span> | <span data-ttu-id="40154-188">**סינכרון ראשוני**</span><span class="sxs-lookup"><span data-stu-id="40154-188">**Initial sync**</span></span> | <span data-ttu-id="40154-189">**פריט ראשי לסינכרון ראשוני**</span><span class="sxs-lookup"><span data-stu-id="40154-189">**Master for initial sync**</span></span> | <span data-ttu-id="40154-190">**הפעל דרישות מוקדמות**</span><span class="sxs-lookup"><span data-stu-id="40154-190">**Run prerequisites**</span></span> | <span data-ttu-id="40154-191">**סינכרון ראשוני של דרישות מוקדמות**</span><span class="sxs-lookup"><span data-stu-id="40154-191">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="40154-192">**תפקידי משאבי פרויקט לכל החברות (bookableresourcecategories)**</span><span class="sxs-lookup"><span data-stu-id="40154-192">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="40154-193">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-193">No</span></span> | <span data-ttu-id="40154-194">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="40154-194">Yes</span></span> | <span data-ttu-id="40154-195">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="40154-195">Common Data Service</span></span> | <span data-ttu-id="40154-196">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-196">No</span></span> | <span data-ttu-id="40154-197">לא זמין</span><span class="sxs-lookup"><span data-stu-id="40154-197">N\A</span></span> |
| <span data-ttu-id="40154-198">**ישויות משפטיות (cdm\_companies)**</span><span class="sxs-lookup"><span data-stu-id="40154-198">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="40154-199">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-199">No</span></span> | <span data-ttu-id="40154-200">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="40154-200">Yes</span></span> | <span data-ttu-id="40154-201">יישומי Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="40154-201">Finance and Operations apps</span></span> | <span data-ttu-id="40154-202">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-202">No</span></span> | <span data-ttu-id="40154-203">לא זמין</span><span class="sxs-lookup"><span data-stu-id="40154-203">N\A</span></span> |
| <span data-ttu-id="40154-204">**ספר (msdyn_ledgers)**</span><span class="sxs-lookup"><span data-stu-id="40154-204">**Ledger (msdyn_ledgers)**</span></span> | <span data-ttu-id="40154-205">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-205">No</span></span> | <span data-ttu-id="40154-206">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="40154-206">Yes</span></span> | <span data-ttu-id="40154-207">יישומי Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="40154-207">Finance and Operations apps</span></span> | <span data-ttu-id="40154-208">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="40154-208">Yes</span></span> | <span data-ttu-id="40154-209">כן, יישומי Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="40154-209">Yes, Finance and Operations apps</span></span> |
| <span data-ttu-id="40154-210">**שילוב Project Operations בפועל (msdyn\_actuals)**</span><span class="sxs-lookup"><span data-stu-id="40154-210">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="40154-211">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-211">No</span></span> | <span data-ttu-id="40154-212">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-212">No</span></span> | <span data-ttu-id="40154-213">לא זמין</span><span class="sxs-lookup"><span data-stu-id="40154-213">N\A</span></span> | <span data-ttu-id="40154-214">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="40154-214">Yes</span></span> | <span data-ttu-id="40154-215">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-215">No</span></span> |
| <span data-ttu-id="40154-216">**סעיפי חוזה של פרויקט (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="40154-216">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="40154-217">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-217">No</span></span> | <span data-ttu-id="40154-218">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-218">No</span></span> | <span data-ttu-id="40154-219">לא זמין</span><span class="sxs-lookup"><span data-stu-id="40154-219">N\A</span></span> | <span data-ttu-id="40154-220">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-220">No</span></span> | <span data-ttu-id="40154-221">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-221">No</span></span> |
| <span data-ttu-id="40154-222">**‏‫ישות שילוב ליחסי גומלין של עסקה בפרויקט‬ (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="40154-222">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="40154-223">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-223">No</span></span> | <span data-ttu-id="40154-224">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-224">No</span></span> | <span data-ttu-id="40154-225">לא זמין</span><span class="sxs-lookup"><span data-stu-id="40154-225">N\A</span></span> | <span data-ttu-id="40154-226">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-226">No</span></span> | <span data-ttu-id="40154-227">לא זמין</span><span class="sxs-lookup"><span data-stu-id="40154-227">N\A</span></span> |
| <span data-ttu-id="40154-228">**אבני דרך בסעיף חוזה לשילוב Project Operations (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="40154-228">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="40154-229">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-229">No</span></span> | <span data-ttu-id="40154-230">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-230">No</span></span> | <span data-ttu-id="40154-231">לא זמין</span><span class="sxs-lookup"><span data-stu-id="40154-231">N\A</span></span> | <span data-ttu-id="40154-232">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-232">No</span></span> | <span data-ttu-id="40154-233">לא זמין</span><span class="sxs-lookup"><span data-stu-id="40154-233">N\A</span></span> |
| <span data-ttu-id="40154-234">**ישות שילוב Project Operations להערכת הוצאות (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="40154-234">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="40154-235">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-235">No</span></span> | <span data-ttu-id="40154-236">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-236">No</span></span> | <span data-ttu-id="40154-237">לא זמין</span><span class="sxs-lookup"><span data-stu-id="40154-237">N\A</span></span> | <span data-ttu-id="40154-238">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-238">No</span></span> | <span data-ttu-id="40154-239">לא זמין</span><span class="sxs-lookup"><span data-stu-id="40154-239">N\A</span></span> |
| <span data-ttu-id="40154-240">**ישות ייצוא הוצאות פרויקט בשילוב Project Operations (msdyn\_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="40154-240">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="40154-241">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-241">No</span></span> | <span data-ttu-id="40154-242">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-242">No</span></span> | <span data-ttu-id="40154-243">לא זמין</span><span class="sxs-lookup"><span data-stu-id="40154-243">N\A</span></span> | <span data-ttu-id="40154-244">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-244">No</span></span> | <span data-ttu-id="40154-245">לא זמין</span><span class="sxs-lookup"><span data-stu-id="40154-245">N\A</span></span> |
| <span data-ttu-id="40154-246">**ישות ייצוא הוצאות פרויקט בשילוב Project Operations (msdyn\_expenses)**</span><span class="sxs-lookup"><span data-stu-id="40154-246">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="40154-247">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="40154-247">Yes</span></span> | <span data-ttu-id="40154-248">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-248">No</span></span> | <span data-ttu-id="40154-249">לא זמין</span><span class="sxs-lookup"><span data-stu-id="40154-249">N\A</span></span> | <span data-ttu-id="40154-250">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-250">No</span></span> | <span data-ttu-id="40154-251">לא זמין</span><span class="sxs-lookup"><span data-stu-id="40154-251">N\A</span></span> |
| <span data-ttu-id="40154-252">**ישות שילוב Project Operations להערכת שעות (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="40154-252">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="40154-253">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="40154-253">Yes</span></span> | <span data-ttu-id="40154-254">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-254">No</span></span> | <span data-ttu-id="40154-255">לא זמין</span><span class="sxs-lookup"><span data-stu-id="40154-255">N\A</span></span> | <span data-ttu-id="40154-256">Yes</span><span class="sxs-lookup"><span data-stu-id="40154-256">No</span></span> | <span data-ttu-id="40154-257">לא זמין</span><span class="sxs-lookup"><span data-stu-id="40154-257">N\A</span></span> |


4. <span data-ttu-id="40154-258">כדי לרענן את הישות, בחר את שם המפה ואז בחר **רענן ישויות**.</span><span class="sxs-lookup"><span data-stu-id="40154-258">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![רענן מפה](./media/20RefreshMapping.png)

5. <span data-ttu-id="40154-260">לאחר השלמת הרענון, הפעל את המפה.</span><span class="sxs-lookup"><span data-stu-id="40154-260">After the refresh is complete, run the map.</span></span> <span data-ttu-id="40154-261">לפני הפיכת המפה הבאה לזמינה, ודא שהמפה בטבלה במצב **פועלת**.</span><span class="sxs-lookup"><span data-stu-id="40154-261">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="40154-262">הפעלת מפות עם מספר גדול יותר של תנאים מוקדמים עשויה להימשך זמן מה.</span><span class="sxs-lookup"><span data-stu-id="40154-262">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="40154-263">להפעלת מפה עם תנאים מוקדמים, החלף את המצב של הלחצן **הצג מפות ישויות קשורות** לפועל.</span><span class="sxs-lookup"><span data-stu-id="40154-263">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="40154-264">אם הטבלה מציינת כי **סינכרון ראשוני של דרישות מוקדמות** הוא במצב **לא**, ודא שהדגל **סינכרון ראשוני** הוא **כבוי** בכל מפות הדרישה המוקדמת לפני שתפעיל אותה.</span><span class="sxs-lookup"><span data-stu-id="40154-264">If the table indicates **Prerequisite initial sync** is **No**, verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![הפעל מפה](./media/21RunMap.png)

6. <span data-ttu-id="40154-266">ודא שכל המפות הקשורות לפרויקט במצב פועל.</span><span class="sxs-lookup"><span data-stu-id="40154-266">Validate all project related maps are in the running state.</span></span>

![כל המפות פועלות](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a><span data-ttu-id="40154-268">החלת נתוני תצורה ב-CDS עבור Project Operations (אופציונלי)</span><span class="sxs-lookup"><span data-stu-id="40154-268">Apply configuration data in CDS for Project Operations (optional)</span></span>

<span data-ttu-id="40154-269">אם החלת נתוני הדגמה על סביבת Finance, ראה [הגדרה והחלה של נתוני תצורה ב-Common Data Service עבור Project Operations](resource-apply-pro-setup-config-data.md) כדי להחיל נתוני הדגמה על סביבת CDS.</span><span class="sxs-lookup"><span data-stu-id="40154-269">If you have applied demo data to the Finance environment, see [Set up and apply configuration data in the Common Data Service for Project Operations](resource-apply-pro-setup-config-data.md) to apply demo data to CDS environment.</span></span>


<span data-ttu-id="40154-270">סביבת Project Operations שלך מוקצית ומוגדרת כעת.</span><span class="sxs-lookup"><span data-stu-id="40154-270">Your Project Operations environment is now provisioned and configured.</span></span> 
