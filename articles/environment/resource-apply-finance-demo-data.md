---
title: החלת נתוני ההדגמה בסביבת Finance המתארחת בענן
description: נושא זה מסביר כיצד להחיל נתוני הדגמה מ- Project Operations בסביבת Dynamics 365 Finance המתארחת בענן.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a7239301dc8b775dc4a53a1cf6c0bcba3956125a
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289865"
---
# <a name="apply-demo-data-to-a-finance-cloud-hosted-environment"></a><span data-ttu-id="f84e1-103">החלת נתוני ההדגמה בסביבת Finance המתארחת בענן</span><span class="sxs-lookup"><span data-stu-id="f84e1-103">Apply demo data to a Finance Cloud-hosted environment</span></span>

<span data-ttu-id="f84e1-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="f84e1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f84e1-105">נושא זה חל רק על Microsoft Dynamics 365 Finance בגירסה 10.0.13 בלבד וניתן לבצע אותו רק בסביבה המתארחת בענן.</span><span class="sxs-lookup"><span data-stu-id="f84e1-105">This topic is only applicable only Microsoft Dynamics 365 Finance version 10.0.13 and can be performed only on a Cloud-hosted environment.</span></span> <span data-ttu-id="f84e1-106">השלם את השלבים בנושא זה **לפני** שאתה מחיל עדכוני איכות על הסביבה.</span><span class="sxs-lookup"><span data-stu-id="f84e1-106">Complete the steps in this topic **BEFORE** you apply quality updates to the environment.</span></span>

1. <span data-ttu-id="f84e1-107">בפרויקט LCS שלך, פתח את הדף **פרטי סביבה**.</span><span class="sxs-lookup"><span data-stu-id="f84e1-107">In your LCS project, open the **Environment details** page.</span></span> <span data-ttu-id="f84e1-108">שים לב שהוא כולל את הפרטים הדרושים להתחברות לסביבה באמצעות פרוטוקול שולחן עבודה מרוחק (RDP).</span><span class="sxs-lookup"><span data-stu-id="f84e1-108">Notice that it includes the details needed to connect to the environment by using Remote Desktop Protocol (RDP).</span></span>

![פרטי סביבת ](./media/1EnvironmentDetails.png)

<span data-ttu-id="f84e1-110">הקבוצה הראשונה של האישורים המודגשים הם אישורי החשבון המקומי והם מכילים היפר-קישור לחיבור אל שולחן העבודה המרוחק.</span><span class="sxs-lookup"><span data-stu-id="f84e1-110">The first set of highlighted credentials are the local account credentials and contain a hyperlink to the remote desktop connection.</span></span> <span data-ttu-id="f84e1-111">האישורים כוללים את שם המשתמש והסיסמה של מנהל הסביבה.</span><span class="sxs-lookup"><span data-stu-id="f84e1-111">The credentials include the environment admin username and password.</span></span> <span data-ttu-id="f84e1-112">הקבוצה השנייה של האישורים משמשת להתחברות אל SQL Server בסביבה זו.</span><span class="sxs-lookup"><span data-stu-id="f84e1-112">The second set of credentials are used to log in to SQL Server in this environment.</span></span>

2. <span data-ttu-id="f84e1-113">התחבר מרחוק לסביבה באמצעות ההיפר-קישור **בחשבונות מקומיים** והשתמש **באישורי חשבון מקומי** כדי לבצע אימות.</span><span class="sxs-lookup"><span data-stu-id="f84e1-113">Remote to the environment by the hyperlink in **Local Accounts**, and use the **Local Account credentials** to authenticate.</span></span>
3. <span data-ttu-id="f84e1-114">עבור אל **Internet Information Services** > **מאגרי יישומים** > **AOSService** והפסק את השירות.</span><span class="sxs-lookup"><span data-stu-id="f84e1-114">Go to **Internet Information Services** > **Application Pools** > **AOSService** and stop the service.</span></span> <span data-ttu-id="f84e1-115">אתה מפסיק את השירות בשלב זה כדי שתוכל להמשיך להחליף את מסד הנתונים של SQL.</span><span class="sxs-lookup"><span data-stu-id="f84e1-115">You are stopping the service at this point so that you can continue to replace the SQL database.</span></span>

![הפסק את AOS](./media/2StopAOS.png)

4. <span data-ttu-id="f84e1-117">עבור אל **שירותים** והפסק את שני הפריטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="f84e1-117">Go to **Services** and stop the following two items:</span></span>

- <span data-ttu-id="f84e1-118">Microsoft Dynamics 365 Unified Operations: שירות ניהול אצווה</span><span class="sxs-lookup"><span data-stu-id="f84e1-118">Microsoft Dynamics 365 Unified Operations: Batch Management Service</span></span>
- <span data-ttu-id="f84e1-119">Microsoft Dynamics 365 Unified Operations: מסגרת לייצוא וייבוא נתונים</span><span class="sxs-lookup"><span data-stu-id="f84e1-119">Microsoft Dynamics 365 Unified Operations: Data Import Export Framework</span></span>

![הפסק שירותים](./media/3StopServices.png)

5. <span data-ttu-id="f84e1-121">פתח את Microsoft SQL Server Management Studio.</span><span class="sxs-lookup"><span data-stu-id="f84e1-121">Open Microsoft SQL Server Management Studio.</span></span> <span data-ttu-id="f84e1-122">היכנס באמצעות אישורי שרת SQL והשתמש במשתמש ובסיסמה axdbadmin מהדף **פרטי הסביבות** ב- LCS.</span><span class="sxs-lookup"><span data-stu-id="f84e1-122">Log in with SQL server credentials and use the axdbadmin user and password from the LCS **Environments details** page.</span></span>

![SQL Server Management Studio](./media/4SSMS.png)

6. <span data-ttu-id="f84e1-124">בסייר האובייקטים, **מסדי נתונים** ואתר את **AXDB**.</span><span class="sxs-lookup"><span data-stu-id="f84e1-124">In Object Explorer, **Databases** and locate **AXDB**.</span></span> <span data-ttu-id="f84e1-125">אתה תחליף את מסד הנתונים במסד נתונים חדש שנמצא [במרכז ההורדות](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip).</span><span class="sxs-lookup"><span data-stu-id="f84e1-125">You will replace database with a new database that is located in the [Download Center](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip).</span></span> 
7. <span data-ttu-id="f84e1-126">העתק את קובץ ה- zip ל- VM שאתה מחובר אליו מרחוק וחלץ את תוכן ה- zip.</span><span class="sxs-lookup"><span data-stu-id="f84e1-126">Copy the zip file to the VM you are remoted into and extract zip contents.</span></span>
8. <span data-ttu-id="f84e1-127">ב- SQL Server Management Studio, לחץ באמצעות לחצן העכבר הימני על **AxDB** ואז בחר **משימות** > **שחזר** > **מסד נתונים**.</span><span class="sxs-lookup"><span data-stu-id="f84e1-127">In SQL Server Management Studio, right-click **AxDB**, and then select **Tasks** > **Restore** > **Database**.</span></span>

![שחזר את מסד הנתונים](./media/5RestoreDatabase.png)

9. <span data-ttu-id="f84e1-129">בחר **מכשיר מקור** ונווט אל הקובץ שחולץ מה- zip שהעתקת.</span><span class="sxs-lookup"><span data-stu-id="f84e1-129">Select **Source Device** and navigate to the file extracted from zip you copied.</span></span>

![מכשירי מקור](./media/6SourceDevice.png)

10. <span data-ttu-id="f84e1-131">בחר **אפשרויות** ואז בחר **החלף את מסד הנתונים הקיים** ו **סגור חיבורים קיימים למסד הנתונים המהווה יעד**.</span><span class="sxs-lookup"><span data-stu-id="f84e1-131">Select **Options**, and then select **Overwrite the existing database** and **Close existing connections to destination database**.</span></span> 
11. <span data-ttu-id="f84e1-132">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="f84e1-132">Select **OK**.</span></span>

![שחזר הגדרות](./media/7RestoreSetting.png)

<span data-ttu-id="f84e1-134">תקבל אישור כי שחזור AXDB הצליח.</span><span class="sxs-lookup"><span data-stu-id="f84e1-134">You will receive confirmation that the AXDB restore was successful.</span></span> <span data-ttu-id="f84e1-135">לאחר שתקבל אישור זה, תוכל לסגור את SQL Services Management Studio.</span><span class="sxs-lookup"><span data-stu-id="f84e1-135">After you receive this confirmation, you can close SQL Services Management Studio.</span></span>

12. <span data-ttu-id="f84e1-136">חזור אל **Internet Information Services** > **מאגרי יישומים** > **AOSService** והתחל את AOSService.</span><span class="sxs-lookup"><span data-stu-id="f84e1-136">Go back to **Internet Information Services** > **Application Pools** > **AOSService** and start the AOSService.</span></span>
13. <span data-ttu-id="f84e1-137">עבור אל **שירותים** והתחל את שני השירותים שהפסקת קודם לכן.</span><span class="sxs-lookup"><span data-stu-id="f84e1-137">Go to **Services** and start the two services you stopped earlier.</span></span>

14. <span data-ttu-id="f84e1-138">אתר את הכלי AdminUserProvisioning ב- VM זה.</span><span class="sxs-lookup"><span data-stu-id="f84e1-138">Locate the AdminUserProvisioning tool on this VM.</span></span> <span data-ttu-id="f84e1-139">חפש תחת K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.</span><span class="sxs-lookup"><span data-stu-id="f84e1-139">Look under, K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.</span></span>
15. <span data-ttu-id="f84e1-140">הפעל את קובץ ה- ‎.ext באמצעות כתובת המשתמש שלך בשדה **כתובת דוא"ל**.</span><span class="sxs-lookup"><span data-stu-id="f84e1-140">Run the .ext file using your user address in the **Email Address** field.</span></span> 
16. <span data-ttu-id="f84e1-141">בחר **שלח**.</span><span class="sxs-lookup"><span data-stu-id="f84e1-141">Select **Submit**.</span></span>

![הקצאת משאבים של משתמש מנהל מערכת](./media/8AdminUserProvisioning.png)

<span data-ttu-id="f84e1-143">לוקח מספר דקות להשלים את התהליך.</span><span class="sxs-lookup"><span data-stu-id="f84e1-143">This takes a couple of minutes to complete.</span></span> <span data-ttu-id="f84e1-144">אתה אמור לקבל הודעת אישור שמשתמש מנהל המערכת עודכן בהצלחה.</span><span class="sxs-lookup"><span data-stu-id="f84e1-144">You should receive a confirmation message that the Admin user was successfully updated.</span></span>

17. <span data-ttu-id="f84e1-145">לבסוף, הפעל את שורת הפקודה כמנהל מערכת ובצע iisreset</span><span class="sxs-lookup"><span data-stu-id="f84e1-145">Lastly, run Command Prompt as Administrator and perform iisreset</span></span>

![איפוס IIS](./media/9IISReset.png)

18. <span data-ttu-id="f84e1-147">סגור את הפעלת שולחן העבודה המרוחק והשתמש בדף **פרטי הסביבה** של LCS כדי להתחבר לסביבה ולאשר שהיא פועלת כצפוי.</span><span class="sxs-lookup"><span data-stu-id="f84e1-147">Close the remote desktop session and use the LCS **Environment details** page to log in to the environment to confirm it is working as expected.</span></span>

![Finance and Operations](./media/10FinanceAndOperations.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]