---
title: דף הבית 'דיווח'
description: נושא זה מספק מידע אודות דיווח ב- Dynamics 365 Project Service Automation.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: 6c35729e51b7439a74446641af3feace5c7751ac
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998097"
---
# <a name="reporting-home-page"></a><span data-ttu-id="3d910-103">דף הבית של דיווח</span><span class="sxs-lookup"><span data-stu-id="3d910-103">Reporting home page</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="3d910-104">Microsoft Dynamics 365 Project Service Automation מאפשר לארגונים מבוססי פרויקטים לנהל ביעילות את הפעולות של העסק שלהם.</span><span class="sxs-lookup"><span data-stu-id="3d910-104">Microsoft Dynamics 365 Project Service Automation lets project-based organizations efficiently manage the operations of their business.</span></span> <span data-ttu-id="3d910-105">בכל פרויקט, חברי הצוות צריכים לנהל את ההזדמנות, את הצעת המחיר ולתכנן את העבודה, לאייש את הפרויקטים במשאבים, לנהל את העבודה לפי התוכנית, לחייב עבור העבודה ולאחר מכן לבצע את העבודה להשלמת הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="3d910-105">On any project, team members must manage the opportunity, quote and plan the work, resource the projects, manage the work according to the plan, bill for the work, and then do the work to complete the project.</span></span> <span data-ttu-id="3d910-106">היכולת לדווח על פעולות חשובה לקביעת תקינות הארגון ולצורך נקיטת פעולה מתקנת, במידה וזו נדרשת.</span><span class="sxs-lookup"><span data-stu-id="3d910-106">The ability to report on operations is key to determining the health of the organization and taking any corrective action that's required.</span></span> <span data-ttu-id="3d910-107">PSA משתמש בשיטות ובטכנולוגיות דיווח של Microsoft Dynamics 365 עבור כל הדיווח שלו.</span><span class="sxs-lookup"><span data-stu-id="3d910-107">PSA uses Microsoft Dynamics 365 reporting methods and technologies for all its reporting.</span></span> <span data-ttu-id="3d910-108">למידע נוסף על אפשרויות הדיווח, ראה [מדריך לכתיבת דוחות עבור Dynamics 365 Customer Engagement (on-premises), גרסה 9](/dynamics365/customerengagement/on-premises/analytics/reporting-analytics-with-dynamics-365).</span><span class="sxs-lookup"><span data-stu-id="3d910-108">For more information about the options for reporting, see the [Report writing guide for Dynamics 365 Customer Engagement (on-premises), version 9](/dynamics365/customerengagement/on-premises/analytics/reporting-analytics-with-dynamics-365).</span></span>

## <a name="report-wizard"></a><span data-ttu-id="3d910-109">אשף הדוחות</span><span class="sxs-lookup"><span data-stu-id="3d910-109">Report Wizard</span></span>

<span data-ttu-id="3d910-110">אשף הדוחות מאפשר למשתמשים שאינם מפתחים ליצור דוחות פשוטים.</span><span class="sxs-lookup"><span data-stu-id="3d910-110">The Report Wizard lets non-developers create simple reports.</span></span> <span data-ttu-id="3d910-111">מכיוון שהאפליקציה בנויה על פלטפורמה קיימת, החוויה זהה לחוויה המתועדת בנושא [‬‏‫יצירה או עריכה של דוח באמצעות אשף הדוחות‬‏‫](/dynamics365/customerengagement/on-premises/basics/create-edit-copy-report-wizard).</span><span class="sxs-lookup"><span data-stu-id="3d910-111">Because the app is built on an existing platform, the experience is the same as the experience that is documented in [Create or edit a report using the Report Wizard](/dynamics365/customerengagement/on-premises/basics/create-edit-copy-report-wizard).</span></span> <span data-ttu-id="3d910-112">עם זאת, עליך להשתמש בישויות שהנן ספציפיות ל- Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="3d910-112">However, you will use the Project Service Automation-specific entities.</span></span>

## <a name="custom-sql-server-reporting-services-reports"></a><span data-ttu-id="3d910-113">דוחות מותאמים אישית של SQL Server Reporting Services</span><span class="sxs-lookup"><span data-stu-id="3d910-113">Custom SQL Server Reporting Services reports</span></span>

<span data-ttu-id="3d910-114">אם העסק שלך דורש דוח מסוים שלא ניתן ליצור באמצעות אשף הדוחות, תוכל ליצור דוח מותאם אישית.</span><span class="sxs-lookup"><span data-stu-id="3d910-114">If your business requires a specific report that can't be created by using the Report Wizard, you can create a custom report.</span></span> <span data-ttu-id="3d910-115">עליך להתקין את Microsoft Visual Studio, יחד עם Microsoft SQL Server Data Tools ו- Report Authoring Extensions המתאימים.</span><span class="sxs-lookup"><span data-stu-id="3d910-115">You must have Microsoft Visual Studio installed, together with the appropriate Microsoft SQL Server Data Tools and Report Authoring Extensions.</span></span> <span data-ttu-id="3d910-116">לקבלת מידע נוסף על כלים וגירסאות, ראה [סביבת כתיבת דוחות באמצעות SQL Server Data Tools](/dynamics365/customerengagement/on-premises/analytics/report-writing-environment-using-sql-server-data-tools).</span><span class="sxs-lookup"><span data-stu-id="3d910-116">For more information about tools and versions, see [Report writing environment using SQL Server Data Tools](/dynamics365/customerengagement/on-premises/analytics/report-writing-environment-using-sql-server-data-tools).</span></span> <span data-ttu-id="3d910-117">לקבלת מידע אודות אופן יצירת דוח מותאם אישית, ראה [יצירת דוח חדש באמצעות SQL Server Data Tools](/dynamics365/customerengagement/on-premises/analytics/create-a-new-report-using-sql-server-data-tools).</span><span class="sxs-lookup"><span data-stu-id="3d910-117">For information about how to create a custom report, see [Create a new report using SQL Server Data Tools](/dynamics365/customerengagement/on-premises/analytics/create-a-new-report-using-sql-server-data-tools).</span></span>

## <a name="power-bi-insights-apps"></a><span data-ttu-id="3d910-118">אפליקציות Power BI להשגת תובנות</span><span class="sxs-lookup"><span data-stu-id="3d910-118">Power BI insights apps</span></span>

<span data-ttu-id="3d910-119">ביחד, Microsoft Power BI ו- Dynamics 365 מספקים לך דרך רבת עוצמה לעבוד עם הנתונים שלך, בצורה של אפליקציות להשגת תובנות.</span><span class="sxs-lookup"><span data-stu-id="3d910-119">Together, Microsoft Power BI and Dynamics 365 give you a powerful way to work with your data, in the form of insights apps.</span></span> <span data-ttu-id="3d910-120">לקבלת מידע על הזמינות של אפליקציות להשגת תובנות, ראה [דף אפליקציות Power BI להשגת תובנות](https://powerbi.microsoft.com/power-bi-insights-apps/).</span><span class="sxs-lookup"><span data-stu-id="3d910-120">For information about the availability of insights apps, see the [Power BI insights apps page](https://powerbi.microsoft.com/power-bi-insights-apps/).</span></span>


## <a name="additional-resources"></a><span data-ttu-id="3d910-121">משאבים נוספים</span><span class="sxs-lookup"><span data-stu-id="3d910-121">Additional resources</span></span>
<span data-ttu-id="3d910-122">לקבלת מידע אודות דיווח ב- PSA, עיין בנושאים הבאים:</span><span class="sxs-lookup"><span data-stu-id="3d910-122">For more information about reporting in PSA, see the following topics:</span></span>

- [<span data-ttu-id="3d910-123">עבודה עם מודל הנתונים של Project Service</span><span class="sxs-lookup"><span data-stu-id="3d910-123">Working with the Project Service data model</span></span>](reports-working-project-service-data-model.md)
- [<span data-ttu-id="3d910-124">לוחות מחוונים</span><span class="sxs-lookup"><span data-stu-id="3d910-124">Dashboards</span></span>](reports-dashboards.md)



[!INCLUDE[footer-include](../includes/footer-banner.md)]