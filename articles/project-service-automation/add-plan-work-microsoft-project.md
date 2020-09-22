---
title: שימוש בתוספת של ‏‫Project Service לתכנון העבודה ב- Microsoft Project | MicrosoftDocs
description: נושא זה מספק מידע אודות אופן ההוספה, קביעת התצורה והשימוש בתוספת Microsoft project עבור Microsoft project Service.
author: ruhercul
manager: kfend
ms.service: Dynamics 365 Project Service Automation
ms.custom:
- dyn365-projectservice
ms.date: 04/06/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: efd589e0-8233-4abf-bf7e-5c1e83c4daea
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 0ad503ff0c27f1543d15b60714c2be46b8487d18
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751769"
---
# <a name="use-the-project-service-automation-add-in-to-plan-your-work-in-microsoft-project"></a><span data-ttu-id="0aa0c-103">השתמש בתוספת של ‏‫Project Service Automation‬ כדי לתכנן את העבודה שלך ב- Microsoft Project</span><span class="sxs-lookup"><span data-stu-id="0aa0c-103">Use the Project Service Automation Add-in to plan your work in Microsoft Project</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] <span data-ttu-id="0aa0c-104">מאפשר לך לבצע תכנון פרוייקט, כולל הערכות, בקלות רבה יותר.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-104">makes it easier for you to do your project planning, including estimates.</span></span> <span data-ttu-id="0aa0c-105">באפשרותך להגדיר את העבודה כך שעלויות, מאמץ וערך מכירות יהיו ברורים בעת הגשת ההצעה הסופית.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-105">You can define the work so that costs, effort, and sales value are clear as the final proposal is submitted.</span></span>  

 <span data-ttu-id="0aa0c-106">כעת באפשרותך להתקין את [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] ולבצע את עבודת התכנון בסביבה המוכרת של [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="0aa0c-106">Now you can install the [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] and do your planning work in the familiar environment of [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span> <span data-ttu-id="0aa0c-107">השתמש ביכולות החזקות של תכנון וניהול ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולאחר מכן עדכן את תוכנית הפרוייקט שלך ב- Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-107">Use the robust planning and management capabilities of [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and then update your project plan in Project Service Automation.</span></span>  

> [!IMPORTANT]
> - <span data-ttu-id="0aa0c-108">כדי להשתמש בתכונת ניהול המסמכים של SharePoint לצורך אחסון קובצי [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] עבור פרוייקטים של [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], מנהל המערכת של [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] יצטרך להפעיל את ניהול המסמכים.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-108">To use SharePoint document management to store your [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] files for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] projects, your [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] admin will need to turn on document management.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="0aa0c-109">[הפעלת ניהול מסמכים של SharePoint עבור ישויות ספציפיות](../admin/enable-sharepoint-document-management-specific-entities.md)</span><span class="sxs-lookup"><span data-stu-id="0aa0c-109">[Enable SharePoint document management for specific entities](../admin/enable-sharepoint-document-management-specific-entities.md)</span></span>  
> - <span data-ttu-id="0aa0c-110">The [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] תואם רק ל- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-110">The [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] is only compatible with [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.</span></span>  

## <a name="download-and-install-the-add-in"></a><span data-ttu-id="0aa0c-111">הורדה והתקנה של התוספת</span><span class="sxs-lookup"><span data-stu-id="0aa0c-111">Download and install the add-in</span></span>  
 <span data-ttu-id="0aa0c-112">הכן את פרטי הכניסה שלך ל- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0aa0c-112">Have your [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] sign-in information ready.</span></span> <span data-ttu-id="0aa0c-113">תזדקק למידע זה כדי להתחבר מתוך [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0aa0c-113">You will need this information to connect from [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

1.  <span data-ttu-id="0aa0c-114">דרך 'מרכז ההורדות', באפשרותך להוריד את התוספת עבור הגירסה הנתמכת של Project Service, גירסה [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) או גירסה [V3.4+‎](https://www.microsoft.com/download/details.aspx?id=57956).</span><span class="sxs-lookup"><span data-stu-id="0aa0c-114">From the Download Center, download the add-in for your supported version of Project Service, either [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) or [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956).</span></span>  

2.  <span data-ttu-id="0aa0c-115">לחץ על קישור ההורדה.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-115">Click the download link.</span></span>  

3.  <span data-ttu-id="0aa0c-116">כאשר ההורדה תושלם, לחץ על **כן** כדי להתקין את התוספת.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-116">When the download is complete, click **Yes** to install the add-in.</span></span>  

## <a name="configure-the-add-in"></a><span data-ttu-id="0aa0c-117">קביעת תצורה של התוספת</span><span class="sxs-lookup"><span data-stu-id="0aa0c-117">Configure the add-in</span></span>  

1. <span data-ttu-id="0aa0c-118">פתח את [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולחץ על הכרטיסיה **Project Service**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-118">Open [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and click the **Project Service** tab.</span></span>  

2. <span data-ttu-id="0aa0c-119">לחץ על **התחבר**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-119">Click **Connect**.</span></span>  

3. <span data-ttu-id="0aa0c-120">הזן את פרטי הכניסה שלך ולאחר מכן לחץ על **כניסה**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-120">Enter your sign-in information and then click **Sign in**.</span></span>  

   <span data-ttu-id="0aa0c-121">כעת תוכל להתחיל להשתמש בתוספת.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-121">Now you can start using the add-in.</span></span>  

## <a name="read-from-a-template"></a><span data-ttu-id="0aa0c-122">קריאה מתוך תבנית</span><span class="sxs-lookup"><span data-stu-id="0aa0c-122">Read from a template</span></span>  
 <span data-ttu-id="0aa0c-123">קרא מתוך תבנית שיצרת ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] והעתקת לתוך [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] כדי להתחיל את תכנון הפרוייקט שלך.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-123">Read from a template that you created in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] and copied into [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] to start your project planning.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="0aa0c-124">[יצירת תבנית לפרוייקט (Project Service Automation)](../project-service/create-project-template.md)</span><span class="sxs-lookup"><span data-stu-id="0aa0c-124">[Create a project template (Project Service Automation)](../project-service/create-project-template.md)</span></span>  

1.  <span data-ttu-id="0aa0c-125">מתוך הכרטיסיה **Project Service**, לחץ על **קריאה** > **תבנית פרוייקט של Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-125">From the **Project Service** tab, click **Read** > **Project Service Automation Project Template**.</span></span>  

2.  <span data-ttu-id="0aa0c-126">בחר תבנית פרוייקט מהרשימה ולאחר מכן לחץ על **פתח**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-126">Choose a project template from the list and then click **Open**.</span></span>  

    > [!NOTE]
    >  <span data-ttu-id="0aa0c-127">כברירת מחדל, משימות המועתקות מתוך התבנית לפרוייקט מוגדרות בתור מתוזמנות באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-127">By default, the tasks that are copied from the template into Project are set as manually scheduled.</span></span>  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a><span data-ttu-id="0aa0c-128">הקצאת תפקידי [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] למשאבי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="0aa0c-128">Assign [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] roles to project resources</span></span>  

1.  <span data-ttu-id="0aa0c-129">פתח פרוייקט ולחץ על רצועת הכלים **משימה**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-129">Open a project and click the **Task** ribbon.</span></span>  

2.  <span data-ttu-id="0aa0c-130">לחץ על התפריט **תרשים גנט** ולאחר מכן בחר **גיליון משאבים**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-130">Click the **Gantt Chart** menu and then choose **Resource Sheet**.</span></span>  

3.  <span data-ttu-id="0aa0c-131">בגיליון המשאבים, לחץ על התפריט הנפתח **תפקיד של משאב Project Service** ובחר תפקיד של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-131">On the Resource Sheet, click the **Project Service Resource Role** drop-down menu and choose a Project Service Automation role.</span></span>  

## <a name="staff-your-project-with-resources"></a><span data-ttu-id="0aa0c-132">איוש הפרוייקט שלך במשאבים</span><span class="sxs-lookup"><span data-stu-id="0aa0c-132">Staff your project with resources</span></span>  

1.  <span data-ttu-id="0aa0c-133">מתוך הכרטיסיה Project Service, בחר שורה ולחץ על **חיפוש משאבים**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-133">From the Project Service tab, select a row and click **Find Resources**.</span></span>  

2.  <span data-ttu-id="0aa0c-134">במסך **‏‫הזמן משאב‬**, בחר את המשאב שברצונך להשתמש בו עבור הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-134">On the **Book Resource** screen, select the resource that you want to use for the project.</span></span>  

3.  <span data-ttu-id="0aa0c-135">לחץ על **הזמן** ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-135">Click **Book** and then click **OK**.</span></span>  

## <a name="publish-your-project"></a><span data-ttu-id="0aa0c-136">פרסום הפרוייקט שלך</span><span class="sxs-lookup"><span data-stu-id="0aa0c-136">Publish your project</span></span>  
<span data-ttu-id="0aa0c-137">לאחר השלמת תכנון הפרוייקט שלך, השלב הבא הוא לייבא ולפרסם את הפרוייקט ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0aa0c-137">When your project planning is complete, the next step is to import and publish the project in to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

<span data-ttu-id="0aa0c-138">הפרוייקט יובא לתוך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0aa0c-138">The project will import into [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> <span data-ttu-id="0aa0c-139">תהליכי תמחור והפקת צוות מוחלים.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-139">The pricing and team generation process are applied.</span></span> <span data-ttu-id="0aa0c-140">פתח את הפרוייקט ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] כדי לראות שהצוות, הערכות הפרוייקט ומבנה התפלגות העבודה נוצרו.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-140">Open the project in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to see that the team, project estimates, and work breakdown structure has been generated.</span></span> <span data-ttu-id="0aa0c-141">הטבלה הבאה מראה היכן למצוא את התוצאות:</span><span class="sxs-lookup"><span data-stu-id="0aa0c-141">The following table shows where to find the results:</span></span>


|                                                                                          |                                                                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="0aa0c-142">**תרשים גנט**</span><span class="sxs-lookup"><span data-stu-id="0aa0c-142">**Gantt Chart**</span></span>   | <span data-ttu-id="0aa0c-143">מייבא לתוך המסך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **מבנה התפלגות עבודה**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-143">Imports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Work Breakdown Structure** screen.</span></span> |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="0aa0c-144">**גליון משאבים**</span><span class="sxs-lookup"><span data-stu-id="0aa0c-144">**Resource Sheet**</span></span> |   <span data-ttu-id="0aa0c-145">מייבא לתוך המסך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **חברי צוות הפרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-145">Imports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Project Team Members** screen.</span></span>   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="0aa0c-146">**שימוש בנתוני שימוש**</span><span class="sxs-lookup"><span data-stu-id="0aa0c-146">**Use Usage**</span></span>    |    <span data-ttu-id="0aa0c-147">מייבא לתוך המסך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **‏‫הערכות פרוייקט‬**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-147">Omports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Project Estimates** screen.</span></span>     |

<span data-ttu-id="0aa0c-148">**כדי לייבא ולפרסם את הפרוייקט שלך**</span><span class="sxs-lookup"><span data-stu-id="0aa0c-148">**To import and publish your project**</span></span>  
1. <span data-ttu-id="0aa0c-149">מתוך הכרטיסיה **Project Service**, לחץ על **פרסום** > **פרוייקט חדש של Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-149">From the **Project Service** tab, click **Publish** > **New Project Service Automation Project**.</span></span>  

2. <span data-ttu-id="0aa0c-150">בתיבת הדו שיח **פרסם בפרוייקט חדש ב- Project Service**, הזן את **שם הפרוייקט** ובחר את **הלקוח**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-150">On **Publish to a new project in Project Service** dialog box, enter the **Project Name** and select the **Customer**.</span></span>  

3. <span data-ttu-id="0aa0c-151">אם תרצה, תוכל לבחור את האפשרות **‏‫קשר את תוכנית הפרוייקט ל- Project Service Automation‬** כדי לקשר את קובץ תוכנית הפרוייקט אל Project Service Automation‬.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-151">Optionally check the **Link project plan to Project Service Automation** to link the plan Project file to Project Service Automation.</span></span>  

4. <span data-ttu-id="0aa0c-152">לחץ על **פרסם**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-152">Click **Publish**.</span></span>  

   <span data-ttu-id="0aa0c-153">קישור קובץ הפרוייקט אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] הופך את קובץ הפרוייקט לקובץ ראשי ומגדיר את מבנה התפלגות העבודה ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-153">Linking the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes the Project file the master and sets the work breakdown structure in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to read-only.</span></span>  <span data-ttu-id="0aa0c-154">כדי לבצע שינויים בתוכנית הפרוייקט, עליך ליצור אותם ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולפרסם כעדכונים ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0aa0c-154">In order to make changes to the project plan, you need to make them in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and publish them as updates to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

## <a name="edit-a-project-thats-been-imported"></a><span data-ttu-id="0aa0c-155">עריכת פרוייקט מיובא</span><span class="sxs-lookup"><span data-stu-id="0aa0c-155">Edit a project that’s been imported</span></span>  
 <span data-ttu-id="0aa0c-156">כדי לבצע שינויים בתוכנית פרוייקט שיובאה לתוך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], עומדות בפניך שתי אפשרויות:</span><span class="sxs-lookup"><span data-stu-id="0aa0c-156">To make changes to a project plan that's been imported into [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you have two options:</span></span>  

- <span data-ttu-id="0aa0c-157">לפתוח את הקובץ הראשי ולערוך אותו ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="0aa0c-157">Open the master file and edit it in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

- <span data-ttu-id="0aa0c-158">לבטל את קישור הקובץ ולערוך אותו ישירות ב- Project Service.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-158">Unlink the file and edit it directly in Project Service.</span></span> <span data-ttu-id="0aa0c-159">כברירת מחדל, פרוייקט שהועלה מתוך [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] נעול וניתן לערוך אותו רק ב- Project.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-159">By default, a project that’s been uploaded from [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] is locked and can only be edited in Project.</span></span> <span data-ttu-id="0aa0c-160">כדי לערוך את הקובץ ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], יש לבטל את קישור הקובץ.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-160">To edit the file in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], the file has to be unlinked.</span></span>  

### <a name="edit-in-pn_microsoft_project"></a><span data-ttu-id="0aa0c-161">לערוך ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span><span class="sxs-lookup"><span data-stu-id="0aa0c-161">Edit in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span></span>  

1. <span data-ttu-id="0aa0c-162">מתוך התפריט הראשי, לחץ על **Project Service** > **פרוייקטים**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-162">From the main menu, click **Project Service** > **Projects**.</span></span>  

2. <span data-ttu-id="0aa0c-163">מתוך רשימת הפרוייקטים, פתח את הפרוייקט שיצרת ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="0aa0c-163">From the list of projects, open the one you created in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

3. <span data-ttu-id="0aa0c-164">לחץ על **פתח ב- MS Project** מרצועת הכלים.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-164">Click **Open in MS Project** from the ribbon.</span></span> <span data-ttu-id="0aa0c-165">פעולה זו תפתח את הקובץ הראשי המקושר ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="0aa0c-165">This will open the linked master file in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a><span data-ttu-id="0aa0c-166">ביטול קישור הקובץ ועריכתו ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service</span><span class="sxs-lookup"><span data-stu-id="0aa0c-166">Unlink a file and edit in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service</span></span>  

1. <span data-ttu-id="0aa0c-167">מתוך התפריט הראשי, לחץ על **Project Service** > **פרוייקטים**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-167">From the main menu, click **Project Service** > **Projects**.</span></span>  

2. <span data-ttu-id="0aa0c-168">מתוך רשימת הפרוייקטים, פתח את הפרוייקט שיצרת ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="0aa0c-168">From the list of projects, open the one you created in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

3. <span data-ttu-id="0aa0c-169">לחץ על **‏‫בטל את הקישור ל- MS Project‬** מרצועת הכלים.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-169">Click **Unlink from MS Project** from the ribbon.</span></span>  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a><span data-ttu-id="0aa0c-170">העלאת קובץ פרוייקט ל- SharePoint או לקבוצות Office</span><span class="sxs-lookup"><span data-stu-id="0aa0c-170">Upload a Project file to SharePoint or Office Groups</span></span>  
 <span data-ttu-id="0aa0c-171">באפשרותך להעלות את קובץ Project שלך אל SharePoint ולמצוא אותו תחת 'מסמכים משויכים' עבור פרוייקט [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] שלך.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-171">You can upload your Project file to SharePoint and find it under the Associated Documents for your [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  <span data-ttu-id="0aa0c-172">מנהל המערכת שלך צריך להגדיר את ניהול המסמכים של SharePoint ולהפעיל אותו עבור הישות 'פרוייקט'.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-172">You need to have your administrator configure SharePoint document management and turn it on for the Project entity.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="0aa0c-173">[הגדרת שילוב של SharePoint](../admin/set-up-sharepoint-integration.md)</span><span class="sxs-lookup"><span data-stu-id="0aa0c-173">[Set up SharePoint integration](../admin/set-up-sharepoint-integration.md)</span></span>  

 <span data-ttu-id="0aa0c-174">באפשרותך גם להעלות את קובץ הפרוייקט שלך ל- [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] אם מוגדרות אצלך Office Groups.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-174">You can also upload your Project file to [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] if you have Office Groups set up.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="0aa0c-175">[שיתוף פעולה עם עמיתים באמצעות קבוצות Office 365 ](../basics/collaborate-with-colleagues-using-office-365-groups.md)</span><span class="sxs-lookup"><span data-stu-id="0aa0c-175">[Collaborate with your colleagues using Office 365 Groups](../basics/collaborate-with-colleagues-using-office-365-groups.md)</span></span>  

### <a name="upload-a-file-for-sharepoint"></a><span data-ttu-id="0aa0c-176">העלאת קובץ עבור SharePoint</span><span class="sxs-lookup"><span data-stu-id="0aa0c-176">Upload a file for SharePoint</span></span>  

1. <span data-ttu-id="0aa0c-177">מתוך התפריט הראשי, לחץ על **Project Service** > **העלאה**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-177">From the main menu, click **Project Service** > **Upload**.</span></span>  

2. <span data-ttu-id="0aa0c-178">בחר **אל מסמכי פרוייקט של Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-178">Select **To Project Service Automation Project Documents**.</span></span>  

3. <span data-ttu-id="0aa0c-179">בדו-שיח **אפשר פתיחה ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**, בחר **כן** או **לא**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-179">On the **Enable Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** dialog, select **Yes** or **No**.</span></span>  

   - <span data-ttu-id="0aa0c-180">אם תלחץ על **כן**, תוכל לבחור בלחצן **פתח ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** ב- Project Service Automation, להפעיל את [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולטעון את קובץ הפרוייקט מתוך ספריית המסמכים של SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-180">If you click **Yes**, you'll be able select the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button in Project Service Automation, launch [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], and load the Project file from the SharePoint document library.</span></span>  

   - <span data-ttu-id="0aa0c-181">אם תלחץ על **לא**, הקישור ללחצן **פתח ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** לא יעבוד.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-181">If you click **No**, the link for the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button won't work.</span></span>  

4. <span data-ttu-id="0aa0c-182">ניתן למצוא את קובץ [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] תחת **מסמכים** עבור פרוייקט [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ספציפי.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-182">The [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] file can be found in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] under **Documents** for the specific [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  

### <a name="upload-a-file-for-office-groups"></a><span data-ttu-id="0aa0c-183">העלאת קובץ ל- Office Groups</span><span class="sxs-lookup"><span data-stu-id="0aa0c-183">Upload a file for Office Groups</span></span>  

1. <span data-ttu-id="0aa0c-184">מתוך התפריט הראשי, לחץ על **Project Service** > **העלאה**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-184">From the main menu, click **Project Service** > **Upload**.</span></span>  

2. <span data-ttu-id="0aa0c-185">בחר **אל מסמכי פרוייקט של Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-185">Select **To Project Service Automation Project Documents**.</span></span>  

3. <span data-ttu-id="0aa0c-186">בדו-שיח **אפשר פתיחה ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**, בחר **כן** או **לא**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-186">On the **Enable Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** dialog, select **Yes** or **No**.</span></span>  

   - <span data-ttu-id="0aa0c-187">אם תלחץ על **כן**, תוכל לבחור בלחצן **פתח ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** ב- Project Service Automation, להפעיל את [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולטעון את קובץ הפרוייקט מתוך ספריית המסמכים של SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-187">If you click **Yes**, you'll be able to select the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button in Project Service Automation, launch [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], and load the Project file from the SharePoint document library.</span></span>  

   - <span data-ttu-id="0aa0c-188">אם תלחץ על **לא**, הקישור ללחצן **פתח ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** לא יעבוד.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-188">If you click **No**, the link for the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button won't work.</span></span>  

4. <span data-ttu-id="0aa0c-189">ניתן למצוא את קובץ [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] תחת **מסמכים** עבור פרוייקט [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ספציפי.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-189">The [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] file can be found in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] under **Documents** for the specific [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  

## <a name="publish--your-project-as-a-template"></a><span data-ttu-id="0aa0c-190">פרסום הפרוייקט שלך כתבנית</span><span class="sxs-lookup"><span data-stu-id="0aa0c-190">Publish  your project as a template</span></span>  
 <span data-ttu-id="0aa0c-191">באפשרותך לשמור את הפרוייקט שלך ולעשות בו שימוש חוזר על-ידי שמירתו כתבנית פרוייקט ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0aa0c-191">You can save your project and reuse it by saving it as a project template in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  <span data-ttu-id="0aa0c-192">תבניות פרוייקט הן תוכניות פרוייקט הניתנות לשימוש חוזר ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0aa0c-192">Project templates are reusable project plans in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="0aa0c-193">[יצירת תבנית לפרוייקט (Project Service Automation)](../project-service/create-project-template.md)</span><span class="sxs-lookup"><span data-stu-id="0aa0c-193">[Create a project template (Project Service Automation)](../project-service/create-project-template.md)</span></span>  

1. <span data-ttu-id="0aa0c-194">מתוך הכרטיסיה **Project Service**, לחץ על **פרסום** > **תבנית פרוייקט חדשה של Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-194">From the **Project Service** tab, click **Publish** > **New Project Service Automation Project Template**.</span></span>  

2. <span data-ttu-id="0aa0c-195">בתיבת הדו שיח **פרסם בפרוייקט חדש בתבנית Project Service**, הזן את **שם תבנית הפרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-195">On the **Publish to a new project in Project Service template** dialog box, enter the **Project template name**.</span></span>  

3. <span data-ttu-id="0aa0c-196">אם תרצה, תוכל לבחור את האפשרות **קשר את תוכנית הפרוייקט ל- Project Service Automation** כדי לקשר את קובץ הפרוייקט אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0aa0c-196">Optionally, check the **Link project plan to Project Service Automation** to link the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

4. <span data-ttu-id="0aa0c-197">לחץ על **פרסם**.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-197">Click **Publish**.</span></span>  

<span data-ttu-id="0aa0c-198">קישור קובץ הפרוייקט אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] הופך את קובץ הפרוייקט לקובץ ראשי ומגדיר את מבנה התפלגות העבודה בתבנית [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="0aa0c-198">Linking the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes the Project file the master and sets the work breakdown structure in the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] template to read-only.</span></span>  <span data-ttu-id="0aa0c-199">כדי לבצע שינויים בתוכנית הפרוייקט, עליך ליצור אותם ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולפרסם כעדכונים ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0aa0c-199">In order to make changes to the project plan, you need to make them in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and publish them as updates to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>

### <a name="see-also"></a><span data-ttu-id="0aa0c-200">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="0aa0c-200">See Also</span></span>  
 [<span data-ttu-id="0aa0c-201">מדריך למנהל פרוייקט</span><span class="sxs-lookup"><span data-stu-id="0aa0c-201">Project Manager Guide</span></span>](../project-service/project-manager-guide.md)
