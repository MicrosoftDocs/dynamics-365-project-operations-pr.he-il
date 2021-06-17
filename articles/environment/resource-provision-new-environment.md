---
title: הקצאת סביבה חדשה
description: נושא זה מספק מידע אודות אופן הקצאת סביבת Project Operations חדשה.
author: sigitac
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d0712d9d5dfc6c35ccd07142ff5948f50e6a254c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995487"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="96930-103">הקצאת סביבה חדשה</span><span class="sxs-lookup"><span data-stu-id="96930-103">Provision a new environment</span></span>

<span data-ttu-id="96930-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="96930-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="96930-105">נושא זה מספק מידע על הדרך להקצות סביבת Dynamics 365 Project Operations חדשה לתרחישים מבוססי משאבים/ללא מלאי.</span><span class="sxs-lookup"><span data-stu-id="96930-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="96930-106">הפוך הקצאת משאבים אוטומטית של Project Operations לזמינה בפרויקט LCS</span><span class="sxs-lookup"><span data-stu-id="96930-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="96930-107">השתמש בשלבים הבאים כדי להפוך את זרימת הקצאת המשאבים האוטומטית של Project Operations לאוטומטית עבור פרויקט LCS שלך.</span><span class="sxs-lookup"><span data-stu-id="96930-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="96930-108">עבור אל [LCS](https://lcs.dynamics.com/v2) ובחר את האריח **ניהול תכונת תצוגה מקדימה**.</span><span class="sxs-lookup"><span data-stu-id="96930-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="96930-109">ברשימת **תכונות התצוגה המקדימה**, בחר **תכונת Project Operations** ואז בחר **תכונת Preview זמינה** כדי להפוך את Project Operations לזמין.</span><span class="sxs-lookup"><span data-stu-id="96930-109">In the **Preview feature** list, select **Project Operations Feature**, and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="96930-110">שלב זה מבוצע פעם אחת בלבד לכל פרויקט LCS.</span><span class="sxs-lookup"><span data-stu-id="96930-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="96930-111">הקצאת סביבת Project Operations</span><span class="sxs-lookup"><span data-stu-id="96930-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="96930-112">פתח פריסה חדשה של Dynamics 365 Finance [סביבת הדגמה](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) או [סביבת ארגז חול/ ייצור](/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure).</span><span class="sxs-lookup"><span data-stu-id="96930-112">Open a new Dynamics 365 Finance [demo environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="96930-113">הסבר על אשף **הקצאת הסביבה**.</span><span class="sxs-lookup"><span data-stu-id="96930-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="96930-114">ודא שגירסת היישום שנבחרה היא 10.0.13 ומעלה.</span><span class="sxs-lookup"><span data-stu-id="96930-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="96930-115">להקצאת Project Operations, תחת **הגדרות מתקדמות**, בחר **Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="96930-115">To provision Project Operations, under **Advance settings**, select **Common Data Service**.</span></span> 
4. <span data-ttu-id="96930-116">הפוך את **הגדרת Common Data Service** לזמינה על-ידי בחירת **כן** ואז הזן מידע בשדות הנדרשים:</span><span class="sxs-lookup"><span data-stu-id="96930-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="96930-117">שם</span><span class="sxs-lookup"><span data-stu-id="96930-117">Name</span></span>
  - <span data-ttu-id="96930-118">אזור</span><span class="sxs-lookup"><span data-stu-id="96930-118">Region</span></span>
  - <span data-ttu-id="96930-119">שפה</span><span class="sxs-lookup"><span data-stu-id="96930-119">Language</span></span>
  - <span data-ttu-id="96930-120">מטבע</span><span class="sxs-lookup"><span data-stu-id="96930-120">Currency</span></span>
 
5. <span data-ttu-id="96930-121">בשדה **תבנית Common Data Service**, בחר **Project Operations**</span><span class="sxs-lookup"><span data-stu-id="96930-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="96930-122">בחר את סוג הסביבה לפריסה.</span><span class="sxs-lookup"><span data-stu-id="96930-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="96930-123">גירסת ניסיון מבוססת-מנוי תאפשר לך לפרוס סביבת CDS למשך 30 יום.</span><span class="sxs-lookup"><span data-stu-id="96930-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![הגדרות פריסה](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="96930-125">בחר **מסכים** כדי להסכם לתנאי השירות ואז בחר **סיום** כדי לחזור להגדרות הפריסה.</span><span class="sxs-lookup"><span data-stu-id="96930-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![הסכמת פריסה](./media/2DeploymentConsent.png)

7. <span data-ttu-id="96930-127">אופציונלי - החל נתוני הדגמה על הסביבה.</span><span class="sxs-lookup"><span data-stu-id="96930-127">Optional - Apply demo data to the environment.</span></span> <span data-ttu-id="96930-128">עבור אל **הגדרות מתקדמות**, בחר **התאם אישית את תצורת מסד הנתונים של SQL**, והגדר **ציין ערכת נתונים למסד נתונים של יישומים** שיהיה **הדגמה**.</span><span class="sxs-lookup"><span data-stu-id="96930-128">Go to **Advanced settings**, select **Customize SQL Database Configuration**, and set **Specify a dataset for Application database** to **Demo**.</span></span>

8. <span data-ttu-id="96930-129">מלא את שאר השדות הנדרשים באשף ואשר את הפריסה.</span><span class="sxs-lookup"><span data-stu-id="96930-129">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="96930-130">הזמן להקצאה של הסביבה משתנה בהתאם לסוג הסביבה.</span><span class="sxs-lookup"><span data-stu-id="96930-130">The time to provision the environment varies based on the environment type.</span></span> <span data-ttu-id="96930-131">ההקצאה עשויה להימשך עד שש שעות.</span><span class="sxs-lookup"><span data-stu-id="96930-131">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="96930-132">לאחר השלמת הפריסה בהצלחה, הסביבה תוצג בתור **פרוסה**.</span><span class="sxs-lookup"><span data-stu-id="96930-132">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

9. <span data-ttu-id="96930-133">כדי לאשר שהסביבה נפרסה בהצלחה, בחר **התחברות** והיכנס לסביבה כדי לאשר.</span><span class="sxs-lookup"><span data-stu-id="96930-133">To confirm that the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![פרטי סביבת ](./media/3EnvironmentDetails.png)

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="96930-135">החל עדכונים על סביבת Finance</span><span class="sxs-lookup"><span data-stu-id="96930-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="96930-136">ל- Project Operations נדרשת סביבת Finance עם גירסת יישום **10.0.13 (10.0.569.20009)** ומעלה.</span><span class="sxs-lookup"><span data-stu-id="96930-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="96930-137">ייתכן שתצטרך להחיל עדכוני איכות על סביבת Finance שלך כדי לקבל גירסה זו.</span><span class="sxs-lookup"><span data-stu-id="96930-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="96930-138">ב- LCS, בדף **פרטי הסביבה**, במקטע **עדכונים זמינים**, בחר **הצג עדכון**.</span><span class="sxs-lookup"><span data-stu-id="96930-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![הצג עדכונים](./media/5ViewUpdates.png)

2. <span data-ttu-id="96930-140">בדף **עדכונים בינאריים**, בחר **שמור חבילה.**</span><span class="sxs-lookup"><span data-stu-id="96930-140">On the **Binary updates** page, select **Save package.**</span></span>

![שמור חבילה](./media/6SavePackage.png)

3. <span data-ttu-id="96930-142">לחץ על **בחר הכל** ולאחר מכן בחר **שמור חבילה**.</span><span class="sxs-lookup"><span data-stu-id="96930-142">Click **Select all** and then select **Save package**.</span></span>

![סקור ושמור עדכונים](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="96930-144">הזן שם ותיאור לחבילה ולאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="96930-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="96930-145">בהתאם לחיבור האינטרנט, תהליך זה עשוי להימשך זמן מה.</span><span class="sxs-lookup"><span data-stu-id="96930-145">Depending on the internet connection, this process might take some time.</span></span>

![העלה חבילה לספריית הנכסים](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="96930-147">לאחר שמירת החבילה, בחר **סיום** ושמור חבילה זו בספריית הנכסים בפרויקט LCS שלך.</span><span class="sxs-lookup"><span data-stu-id="96930-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="96930-148">שמירת ואימות החבילה עשויה לארוך כ- 15 דקות.</span><span class="sxs-lookup"><span data-stu-id="96930-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="96930-149">כדי להחיל את העדכון, נווט אל הדף **פרטי הסביבה** ב- LCS ובחר **תחזק** > **החל עדכונים**.</span><span class="sxs-lookup"><span data-stu-id="96930-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![תחזק סביבות](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="96930-151">ברשימת העדכונים, בחר את החבילה שיצרת ובחר **החל**.</span><span class="sxs-lookup"><span data-stu-id="96930-151">In the updates list select the package you created, and select **Apply**.</span></span>

![החל עדכונים](./media/10ApplyUpdates.png)

<span data-ttu-id="96930-153">מתן השירות לסביבה ייקח זמן מה.</span><span class="sxs-lookup"><span data-stu-id="96930-153">Environment servicing will take some time.</span></span> <span data-ttu-id="96930-154">לאחר ההשלמה, הסביבה תחזור למצב פרוס.</span><span class="sxs-lookup"><span data-stu-id="96930-154">After it is complete, the environment will return to a deployed state.</span></span>

![סביבה פרוסה](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="96930-156">יצירת חיבור כתיבה כפולה</span><span class="sxs-lookup"><span data-stu-id="96930-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="96930-157">בפרויקט LCS שלך, עבור אל הדף **פרטי סביבה**.</span><span class="sxs-lookup"><span data-stu-id="96930-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="96930-158">בקטע **פרטי סביבה של Common Data Service**, בחר **קישור ל- CDS עבור יישומים**.</span><span class="sxs-lookup"><span data-stu-id="96930-158">Under **Common Data Service Environment Information**, select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="96930-159">לאחר השלמת הקישור, בחר **קישור ל- CDS עבור יישומים** שוב.</span><span class="sxs-lookup"><span data-stu-id="96930-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="96930-160">תועבר לכתיבה כפולה ב- Finance.</span><span class="sxs-lookup"><span data-stu-id="96930-160">You will be redirected to Dual Write in Finance.</span></span>

![קישור ל- CDS](./media/12LinktoCDS.png)

4. <span data-ttu-id="96930-162">בחר **החל פתרון** כדי לגשת לישויות אשר ימופו בשילוב.</span><span class="sxs-lookup"><span data-stu-id="96930-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![החל פתרונות](./media/13ApplySolutions.png)

5. <span data-ttu-id="96930-164">בחר את שני הפתרונות, **מפת ישויות כתיבה כפולה של Dynamics 365 Finance and Operations** ו- **מפות ישויות כתיבה כפולה של Dynamics 365 Project Operations** ואז בחר **החל**.</span><span class="sxs-lookup"><span data-stu-id="96930-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps**, and then select **Apply**.</span></span>

![אשר פתרונות](./media/14ConfirmSolutions.png)

<span data-ttu-id="96930-166">לאחר החלת הפתרונות, ישויות הכתיבה הכפולה מוחלות על הסביבה.</span><span class="sxs-lookup"><span data-stu-id="96930-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![מחיל פתרונות](./media/15ApplyingSolutions.png)

<span data-ttu-id="96930-168">לאחר החלת הישויות, כל המיפויים הזמינים רשומים בסביבה.</span><span class="sxs-lookup"><span data-stu-id="96930-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![מפות של כתיבה כפולה](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="96930-170">רענן את ישויות הנתונים לאחר העדכון</span><span class="sxs-lookup"><span data-stu-id="96930-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="96930-171">ב- Finance, עבור אל סביבת העבודה **ניהול נתונים**.</span><span class="sxs-lookup"><span data-stu-id="96930-171">In Finance, go to the **Data management** workspace.</span></span>

![סביבת עבודה של ניהול נתונים](./media/16DataManagement.png)

2. <span data-ttu-id="96930-173">בחר את האריח **פרמטרים של מסגרת**.</span><span class="sxs-lookup"><span data-stu-id="96930-173">Select the **Framework parameters** tile.</span></span>

![פרמטרים של מסגרת](./media/17FrameworkParameters.png)

3. <span data-ttu-id="96930-175">בדף **הגדרות ישות**, בחר **רענן את רשימת הישויות**.</span><span class="sxs-lookup"><span data-stu-id="96930-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![רענן את רשימת הישויות](./media/18RefreshEntityList.png)

<span data-ttu-id="96930-177">הרענון יימשך כ- 20 דקות.</span><span class="sxs-lookup"><span data-stu-id="96930-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="96930-178">תקבל התראה כשהוא יסתיים.</span><span class="sxs-lookup"><span data-stu-id="96930-178">You will receive an alert when it is complete.</span></span>

![רענן אישור](./media/19RefreshConfirmation.png)

## <a name="update-security-settings-on-project-operations-on-dataverse"></a><span data-ttu-id="96930-180">עדכן את הגדרות האבטחה של Project Operations ב- Dataverse</span><span class="sxs-lookup"><span data-stu-id="96930-180">Update security settings on Project Operations on Dataverse</span></span>

1. <span data-ttu-id="96930-181">עבור אל Project Operations בסביבת Dataverse שלך.</span><span class="sxs-lookup"><span data-stu-id="96930-181">Go to Project Operations on your Dataverse environment.</span></span> 
2. <span data-ttu-id="96930-182">עבור אל **הגדרות** > **אבטחה** > **תפקידי אבטחה**.</span><span class="sxs-lookup"><span data-stu-id="96930-182">Go to **Settings** > **Security** > **Security roles**.</span></span> 
3. <span data-ttu-id="96930-183">בדף **תפקידי אבטחה**, ברשימת התפקידים, בחר **משתמש באפליקציה עם כתיבה כפולה** ובחר את הכרטיסיה **ישויות מותאמות אישית**.</span><span class="sxs-lookup"><span data-stu-id="96930-183">On the **Security roles** page, in the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span>  
4. <span data-ttu-id="96930-184">ודא שיש לתפקיד הרשאות **קריאה** ו **צירוף** עבור:</span><span class="sxs-lookup"><span data-stu-id="96930-184">Verify that the role has **Read** and **Append To** permissions for the:</span></span>
      
      - <span data-ttu-id="96930-185">**סוג שער החליפין של מטבע**</span><span class="sxs-lookup"><span data-stu-id="96930-185">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="96930-186">**תרשים של תיקי לקוחות**</span><span class="sxs-lookup"><span data-stu-id="96930-186">**Chart Of Accounts**</span></span>
      - <span data-ttu-id="96930-187">**לוח שנה כספי**</span><span class="sxs-lookup"><span data-stu-id="96930-187">**Fiscal Calendar**</span></span>
      - <span data-ttu-id="96930-188">**ספר חשבונות**</span><span class="sxs-lookup"><span data-stu-id="96930-188">**Ledger**</span></span>

5. <span data-ttu-id="96930-189">לאחר עדכון תפקיד האבטחה, עבור אל **הגדרות** > **אבטחה** > **Teams‎**, ובחר את צוות ברירת המחדל בתצוגה **בעל עסק מקומי**.</span><span class="sxs-lookup"><span data-stu-id="96930-189">After the security role is updated, go to **Settings** > **Security** > **Teams**, and select the default team in the **Local Business Owner** team view.</span></span>
6. <span data-ttu-id="96930-190">בחר **נהל תפקידים** וודא כי הרשאת האבטחה **משתמש באפליקציה עם כתיבה כפולה** מוחלת על צוות זה.</span><span class="sxs-lookup"><span data-stu-id="96930-190">Select **Manage Roles** and verify that the **dual-write app user** security privilege is applied to this team.</span></span>

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="96930-191">הפעל את מפות כתיבה כפולה ב- Project Operations</span><span class="sxs-lookup"><span data-stu-id="96930-191">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="96930-192">בפרויקט LCS שלך, עבור אל הדף **פרטי סביבה**.</span><span class="sxs-lookup"><span data-stu-id="96930-192">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="96930-193">בקטע **פרטי סביבה של Common Data Service**, בחר **קישור ל- CDS עבור יישומים.**</span><span class="sxs-lookup"><span data-stu-id="96930-193">Under **Common Data Service Environment Information**, select **Link to CDS for Apps.**</span></span> <span data-ttu-id="96930-194">לאחר שתבחרו בקישור, תועברו לרשימת הישויות במיפויים.</span><span class="sxs-lookup"><span data-stu-id="96930-194">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="96930-195">התחל את המפות כמתואר בטבלה הבאה.</span><span class="sxs-lookup"><span data-stu-id="96930-195">Start the maps as described in the following table.</span></span> <span data-ttu-id="96930-196">הקפד לעקוב אחר הרצף כמפורט.</span><span class="sxs-lookup"><span data-stu-id="96930-196">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="96930-197">**מפת ישויות**</span><span class="sxs-lookup"><span data-stu-id="96930-197">**Entity Map**</span></span> | <span data-ttu-id="96930-198">**רענן ישות**</span><span class="sxs-lookup"><span data-stu-id="96930-198">**Refresh entity**</span></span> | <span data-ttu-id="96930-199">**סינכרון ראשוני**</span><span class="sxs-lookup"><span data-stu-id="96930-199">**Initial sync**</span></span> | <span data-ttu-id="96930-200">**פריט ראשי לסינכרון ראשוני**</span><span class="sxs-lookup"><span data-stu-id="96930-200">**Master for initial sync**</span></span> | <span data-ttu-id="96930-201">**הפעל דרישות מוקדמות**</span><span class="sxs-lookup"><span data-stu-id="96930-201">**Run prerequisites**</span></span> | <span data-ttu-id="96930-202">**סינכרון ראשוני של דרישות מוקדמות**</span><span class="sxs-lookup"><span data-stu-id="96930-202">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="96930-203">**תפקידי משאבי פרויקט לכל החברות (bookableresourcecategories)**</span><span class="sxs-lookup"><span data-stu-id="96930-203">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="96930-204">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-204">No</span></span> | <span data-ttu-id="96930-205">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="96930-205">Yes</span></span> | <span data-ttu-id="96930-206">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="96930-206">Common Data Service</span></span> | <span data-ttu-id="96930-207">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-207">No</span></span> | <span data-ttu-id="96930-208">לא זמין</span><span class="sxs-lookup"><span data-stu-id="96930-208">N\A</span></span> |
| <span data-ttu-id="96930-209">**ישויות משפטיות (cdm\_companies)**</span><span class="sxs-lookup"><span data-stu-id="96930-209">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="96930-210">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-210">No</span></span> | <span data-ttu-id="96930-211">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="96930-211">Yes</span></span> | <span data-ttu-id="96930-212">יישומי Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="96930-212">Finance and Operations apps</span></span> | <span data-ttu-id="96930-213">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-213">No</span></span> | <span data-ttu-id="96930-214">לא זמין</span><span class="sxs-lookup"><span data-stu-id="96930-214">N\A</span></span> |
| <span data-ttu-id="96930-215">**ספר (msdyn_ledgers)**</span><span class="sxs-lookup"><span data-stu-id="96930-215">**Ledger (msdyn_ledgers)**</span></span> | <span data-ttu-id="96930-216">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-216">No</span></span> | <span data-ttu-id="96930-217">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="96930-217">Yes</span></span> | <span data-ttu-id="96930-218">יישומי Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="96930-218">Finance and Operations apps</span></span> | <span data-ttu-id="96930-219">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="96930-219">Yes</span></span> | <span data-ttu-id="96930-220">כן, יישומי Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="96930-220">Yes, Finance and Operations apps</span></span> |
| <span data-ttu-id="96930-221">**שילוב Project Operations בפועל (msdyn\_actuals)**</span><span class="sxs-lookup"><span data-stu-id="96930-221">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="96930-222">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-222">No</span></span> | <span data-ttu-id="96930-223">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-223">No</span></span> | <span data-ttu-id="96930-224">לא זמין</span><span class="sxs-lookup"><span data-stu-id="96930-224">N\A</span></span> | <span data-ttu-id="96930-225">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="96930-225">Yes</span></span> | <span data-ttu-id="96930-226">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-226">No</span></span> |
| <span data-ttu-id="96930-227">**סעיפי חוזה של פרויקט (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="96930-227">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="96930-228">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-228">No</span></span> | <span data-ttu-id="96930-229">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-229">No</span></span> | <span data-ttu-id="96930-230">לא זמין</span><span class="sxs-lookup"><span data-stu-id="96930-230">N\A</span></span> | <span data-ttu-id="96930-231">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-231">No</span></span> | <span data-ttu-id="96930-232">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-232">No</span></span> |
| <span data-ttu-id="96930-233">**‏‫ישות שילוב ליחסי גומלין של עסקה בפרויקט‬ (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="96930-233">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="96930-234">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-234">No</span></span> | <span data-ttu-id="96930-235">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-235">No</span></span> | <span data-ttu-id="96930-236">לא זמין</span><span class="sxs-lookup"><span data-stu-id="96930-236">N\A</span></span> | <span data-ttu-id="96930-237">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-237">No</span></span> | <span data-ttu-id="96930-238">לא זמין</span><span class="sxs-lookup"><span data-stu-id="96930-238">N\A</span></span> |
| <span data-ttu-id="96930-239">**אבני דרך בסעיף חוזה לשילוב Project Operations (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="96930-239">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="96930-240">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-240">No</span></span> | <span data-ttu-id="96930-241">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-241">No</span></span> | <span data-ttu-id="96930-242">לא זמין</span><span class="sxs-lookup"><span data-stu-id="96930-242">N\A</span></span> | <span data-ttu-id="96930-243">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-243">No</span></span> | <span data-ttu-id="96930-244">לא זמין</span><span class="sxs-lookup"><span data-stu-id="96930-244">N\A</span></span> |
| <span data-ttu-id="96930-245">**ישות שילוב Project Operations להערכת הוצאות (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="96930-245">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="96930-246">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-246">No</span></span> | <span data-ttu-id="96930-247">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-247">No</span></span> | <span data-ttu-id="96930-248">לא זמין</span><span class="sxs-lookup"><span data-stu-id="96930-248">N\A</span></span> | <span data-ttu-id="96930-249">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-249">No</span></span> | <span data-ttu-id="96930-250">לא זמין</span><span class="sxs-lookup"><span data-stu-id="96930-250">N\A</span></span> |
| <span data-ttu-id="96930-251">**ישות ייצוא הוצאות פרויקט בשילוב Project Operations (msdyn\_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="96930-251">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="96930-252">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-252">No</span></span> | <span data-ttu-id="96930-253">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-253">No</span></span> | <span data-ttu-id="96930-254">לא זמין</span><span class="sxs-lookup"><span data-stu-id="96930-254">N\A</span></span> | <span data-ttu-id="96930-255">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-255">No</span></span> | <span data-ttu-id="96930-256">לא זמין</span><span class="sxs-lookup"><span data-stu-id="96930-256">N\A</span></span> |
| <span data-ttu-id="96930-257">**ישות ייצוא הוצאות פרויקט בשילוב Project Operations (msdyn\_expenses)**</span><span class="sxs-lookup"><span data-stu-id="96930-257">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="96930-258">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="96930-258">Yes</span></span> | <span data-ttu-id="96930-259">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-259">No</span></span> | <span data-ttu-id="96930-260">לא זמין</span><span class="sxs-lookup"><span data-stu-id="96930-260">N\A</span></span> | <span data-ttu-id="96930-261">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-261">No</span></span> | <span data-ttu-id="96930-262">לא זמין</span><span class="sxs-lookup"><span data-stu-id="96930-262">N\A</span></span> |
| <span data-ttu-id="96930-263">**ישות שילוב Project Operations להערכת שעות (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="96930-263">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="96930-264">‏‏כן</span><span class="sxs-lookup"><span data-stu-id="96930-264">Yes</span></span> | <span data-ttu-id="96930-265">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-265">No</span></span> | <span data-ttu-id="96930-266">לא זמין</span><span class="sxs-lookup"><span data-stu-id="96930-266">N\A</span></span> | <span data-ttu-id="96930-267">Yes</span><span class="sxs-lookup"><span data-stu-id="96930-267">No</span></span> | <span data-ttu-id="96930-268">לא זמין</span><span class="sxs-lookup"><span data-stu-id="96930-268">N\A</span></span> |


4. <span data-ttu-id="96930-269">כדי לרענן את הישות, בחר את שם המפה ואז בחר **רענן ישויות**.</span><span class="sxs-lookup"><span data-stu-id="96930-269">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![רענן מפה](./media/20RefreshMapping.png)

5. <span data-ttu-id="96930-271">לאחר השלמת הרענון, הפעל את המפה.</span><span class="sxs-lookup"><span data-stu-id="96930-271">After the refresh is complete, run the map.</span></span> <span data-ttu-id="96930-272">לפני הפיכת המפה הבאה לזמינה, ודא שהמפה בטבלה במצב **פועלת**.</span><span class="sxs-lookup"><span data-stu-id="96930-272">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="96930-273">הפעלת מפות עם מספר גדול יותר של תנאים מוקדמים עשויה להימשך זמן מה.</span><span class="sxs-lookup"><span data-stu-id="96930-273">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="96930-274">להפעלת מפה עם תנאים מוקדמים, החלף את המצב של הלחצן **הצג מפות ישויות קשורות** לפועל.</span><span class="sxs-lookup"><span data-stu-id="96930-274">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="96930-275">אם הטבלה מציינת כי **סינכרון ראשוני של דרישות מוקדמות** הוא במצב **לא**, ודא שהדגל **סינכרון ראשוני** הוא **כבוי** בכל מפות הדרישה המוקדמת לפני שתפעיל אותה.</span><span class="sxs-lookup"><span data-stu-id="96930-275">If the table indicates **Prerequisite initial sync** is **No**, verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![הפעל מפה](./media/21RunMap.png)

6. <span data-ttu-id="96930-277">ודא שכל המפות הקשורות לפרויקט במצב פועל.</span><span class="sxs-lookup"><span data-stu-id="96930-277">Validate all project related maps are in the running state.</span></span>

![כל המפות פועלות](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a><span data-ttu-id="96930-279">החלת נתוני תצורה ב-CDS עבור Project Operations (אופציונלי)</span><span class="sxs-lookup"><span data-stu-id="96930-279">Apply configuration data in CDS for Project Operations (optional)</span></span>

<span data-ttu-id="96930-280">אם החלת נתוני הדגמה על סביבת Finance, ראה [הגדרה והחלה של נתוני תצורה ב-Common Data Service עבור Project Operations](resource-apply-pro-setup-config-data.md) כדי להחיל נתוני הדגמה על סביבת CDS.</span><span class="sxs-lookup"><span data-stu-id="96930-280">If you have applied demo data to the Finance environment, see [Set up and apply configuration data in the Common Data Service for Project Operations](resource-apply-pro-setup-config-data.md) to apply demo data to CDS environment.</span></span>


<span data-ttu-id="96930-281">סביבת Project Operations שלך מוקצית ומוגדרת כעת.</span><span class="sxs-lookup"><span data-stu-id="96930-281">Your Project Operations environment is now provisioned and configured.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]