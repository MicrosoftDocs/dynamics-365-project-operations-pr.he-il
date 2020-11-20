---
title: שימוש בתוספת של ‏‫Project Service לתכנון העבודה ב- Microsoft Project | MicrosoftDocs
description: נושא זה מספק מידע אודות אופן ההוספה, קביעת התצורה והשימוש בתוספת Microsoft project עבור Microsoft project Service.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 04/06/2019
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
ms.openlocfilehash: 6bc74442866caccc02e53afc913a55aab81f9629
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4129679"
---
# <a name="use-the-project-service-automation-add-in-to-plan-your-work-in-microsoft-project"></a><span data-ttu-id="0b885-103">השתמש בתוספת של ‏‫Project Service Automation‬ כדי לתכנן את העבודה שלך ב- Microsoft Project</span><span class="sxs-lookup"><span data-stu-id="0b885-103">Use the Project Service Automation Add-in to plan your work in Microsoft Project</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] <span data-ttu-id="0b885-104">מאפשר לך לבצע תכנון פרוייקט, כולל הערכות, בקלות רבה יותר.</span><span class="sxs-lookup"><span data-stu-id="0b885-104">makes it easier for you to do your project planning, including estimates.</span></span> <span data-ttu-id="0b885-105">באפשרותך להגדיר את העבודה כך שעלויות, מאמץ וערך מכירות יהיו ברורים בעת הגשת ההצעה הסופית.</span><span class="sxs-lookup"><span data-stu-id="0b885-105">You can define the work so that costs, effort, and sales value are clear as the final proposal is submitted.</span></span>  

 <span data-ttu-id="0b885-106">כעת באפשרותך להתקין את [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] ולבצע את עבודת התכנון בסביבה המוכרת של [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="0b885-106">Now you can install the [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] and do your planning work in the familiar environment of [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span> <span data-ttu-id="0b885-107">השתמש ביכולות החזקות של תכנון וניהול ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולאחר מכן עדכן את תוכנית הפרוייקט שלך ב- Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="0b885-107">Use the robust planning and management capabilities of [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and then update your project plan in Project Service Automation.</span></span>  

> [!IMPORTANT]
> - <span data-ttu-id="0b885-108">כדי להשתמש בתכונת ניהול המסמכים של SharePoint לצורך אחסון קובצי [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] עבור פרוייקטים של [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], מנהל המערכת של [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] יצטרך להפעיל את ניהול המסמכים.</span><span class="sxs-lookup"><span data-stu-id="0b885-108">To use SharePoint document management to store your [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] files for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] projects, your [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] admin will need to turn on document management.</span></span> 
> - <span data-ttu-id="0b885-109">The [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] תואם רק ל- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.</span><span class="sxs-lookup"><span data-stu-id="0b885-109">The [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] is only compatible with [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.</span></span>  

## <a name="download-and-install-the-add-in"></a><span data-ttu-id="0b885-110">הורדה והתקנה של התוספת</span><span class="sxs-lookup"><span data-stu-id="0b885-110">Download and install the add-in</span></span>  
 <span data-ttu-id="0b885-111">הכן את פרטי הכניסה שלך ל- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0b885-111">Have your [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] sign-in information ready.</span></span> <span data-ttu-id="0b885-112">תזדקק למידע זה כדי להתחבר מתוך [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0b885-112">You will need this information to connect from [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

1.  <span data-ttu-id="0b885-113">דרך 'מרכז ההורדות', באפשרותך להוריד את התוספת עבור הגירסה הנתמכת של Project Service, גירסה [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) או גירסה [V3.4+‎](https://www.microsoft.com/download/details.aspx?id=57956).</span><span class="sxs-lookup"><span data-stu-id="0b885-113">From the Download Center, download the add-in for your supported version of Project Service, either [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) or [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956).</span></span>  

2.  <span data-ttu-id="0b885-114">לחץ על קישור ההורדה.</span><span class="sxs-lookup"><span data-stu-id="0b885-114">Click the download link.</span></span>  

3.  <span data-ttu-id="0b885-115">כאשר ההורדה תושלם, לחץ על **כן** כדי להתקין את התוספת.</span><span class="sxs-lookup"><span data-stu-id="0b885-115">When the download is complete, click **Yes** to install the add-in.</span></span>  

## <a name="configure-the-add-in"></a><span data-ttu-id="0b885-116">קביעת תצורה של התוספת</span><span class="sxs-lookup"><span data-stu-id="0b885-116">Configure the add-in</span></span>  

1. <span data-ttu-id="0b885-117">פתח את [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולחץ על הכרטיסיה **Project Service**.</span><span class="sxs-lookup"><span data-stu-id="0b885-117">Open [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and click the **Project Service** tab.</span></span>  

2. <span data-ttu-id="0b885-118">לחץ על **התחבר**.</span><span class="sxs-lookup"><span data-stu-id="0b885-118">Click **Connect**.</span></span>  

3. <span data-ttu-id="0b885-119">הזן את פרטי הכניסה שלך ולאחר מכן לחץ על **כניסה**.</span><span class="sxs-lookup"><span data-stu-id="0b885-119">Enter your sign-in information and then click **Sign in**.</span></span>  

   <span data-ttu-id="0b885-120">כעת תוכל להתחיל להשתמש בתוספת.</span><span class="sxs-lookup"><span data-stu-id="0b885-120">Now you can start using the add-in.</span></span>  

## <a name="read-from-a-template"></a><span data-ttu-id="0b885-121">קריאה מתוך תבנית</span><span class="sxs-lookup"><span data-stu-id="0b885-121">Read from a template</span></span>  
 <span data-ttu-id="0b885-122">קרא מתוך תבנית שיצרת ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] והעתקת לתוך [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] כדי להתחיל את תכנון הפרוייקט שלך.</span><span class="sxs-lookup"><span data-stu-id="0b885-122">Read from a template that you created in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] and copied into [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] to start your project planning.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="0b885-123">[יצירת תבנית לפרוייקט (Project Service Automation)](../psa/create-project-template.md)</span><span class="sxs-lookup"><span data-stu-id="0b885-123">[Create a project template (Project Service Automation)](../psa/create-project-template.md)</span></span>  

1.  <span data-ttu-id="0b885-124">מתוך הכרטיסיה **Project Service**, לחץ על **קריאה** > **תבנית פרוייקט של Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="0b885-124">From the **Project Service** tab, click **Read** > **Project Service Automation Project Template**.</span></span>  

2.  <span data-ttu-id="0b885-125">בחר תבנית פרוייקט מהרשימה ולאחר מכן לחץ על **פתח**.</span><span class="sxs-lookup"><span data-stu-id="0b885-125">Choose a project template from the list and then click **Open**.</span></span>  

    > [!NOTE]
    >  <span data-ttu-id="0b885-126">כברירת מחדל, משימות המועתקות מתוך התבנית לפרוייקט מוגדרות בתור מתוזמנות באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="0b885-126">By default, the tasks that are copied from the template into Project are set as manually scheduled.</span></span>  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a><span data-ttu-id="0b885-127">הקצאת תפקידי [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] למשאבי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="0b885-127">Assign [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] roles to project resources</span></span>  

1.  <span data-ttu-id="0b885-128">פתח פרוייקט ולחץ על רצועת הכלים **משימה**.</span><span class="sxs-lookup"><span data-stu-id="0b885-128">Open a project and click the **Task** ribbon.</span></span>  

2.  <span data-ttu-id="0b885-129">לחץ על התפריט **תרשים גנט** ולאחר מכן בחר **גיליון משאבים**.</span><span class="sxs-lookup"><span data-stu-id="0b885-129">Click the **Gantt Chart** menu and then choose **Resource Sheet**.</span></span>  

3.  <span data-ttu-id="0b885-130">בגיליון המשאבים, לחץ על התפריט הנפתח **תפקיד של משאב Project Service** ובחר תפקיד של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="0b885-130">On the Resource Sheet, click the **Project Service Resource Role** drop-down menu and choose a Project Service Automation role.</span></span>  

## <a name="staff-your-project-with-resources"></a><span data-ttu-id="0b885-131">איוש הפרוייקט שלך במשאבים</span><span class="sxs-lookup"><span data-stu-id="0b885-131">Staff your project with resources</span></span>  

1.  <span data-ttu-id="0b885-132">מתוך הכרטיסיה Project Service, בחר שורה ולחץ על **חיפוש משאבים**.</span><span class="sxs-lookup"><span data-stu-id="0b885-132">From the Project Service tab, select a row and click **Find Resources**.</span></span>  

2.  <span data-ttu-id="0b885-133">במסך **‏‫הזמן משאב‬**, בחר את המשאב שברצונך להשתמש בו עבור הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0b885-133">On the **Book Resource** screen, select the resource that you want to use for the project.</span></span>  

3.  <span data-ttu-id="0b885-134">לחץ על **הזמן** ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="0b885-134">Click **Book** and then click **OK**.</span></span>  

## <a name="publish-your-project"></a><span data-ttu-id="0b885-135">פרסום הפרוייקט שלך</span><span class="sxs-lookup"><span data-stu-id="0b885-135">Publish your project</span></span>  
<span data-ttu-id="0b885-136">לאחר השלמת תכנון הפרוייקט שלך, השלב הבא הוא לייבא ולפרסם את הפרוייקט ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0b885-136">When your project planning is complete, the next step is to import and publish the project in to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

<span data-ttu-id="0b885-137">הפרוייקט יובא לתוך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0b885-137">The project will import into [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> <span data-ttu-id="0b885-138">תהליכי תמחור והפקת צוות מוחלים.</span><span class="sxs-lookup"><span data-stu-id="0b885-138">The pricing and team generation process are applied.</span></span> <span data-ttu-id="0b885-139">פתח את הפרוייקט ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] כדי לראות שהצוות, הערכות הפרוייקט ומבנה התפלגות העבודה נוצרו.</span><span class="sxs-lookup"><span data-stu-id="0b885-139">Open the project in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to see that the team, project estimates, and work breakdown structure has been generated.</span></span> <span data-ttu-id="0b885-140">הטבלה הבאה מראה היכן למצוא את התוצאות:</span><span class="sxs-lookup"><span data-stu-id="0b885-140">The following table shows where to find the results:</span></span>


|                                                                                          |                                                                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="0b885-141">**תרשים גנט**</span><span class="sxs-lookup"><span data-stu-id="0b885-141">**Gantt Chart**</span></span>   | <span data-ttu-id="0b885-142">מייבא לתוך המסך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **מבנה התפלגות עבודה**.</span><span class="sxs-lookup"><span data-stu-id="0b885-142">Imports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Work Breakdown Structure** screen.</span></span> |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="0b885-143">**גליון משאבים**</span><span class="sxs-lookup"><span data-stu-id="0b885-143">**Resource Sheet**</span></span> |   <span data-ttu-id="0b885-144">מייבא לתוך המסך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **חברי צוות הפרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="0b885-144">Imports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Project Team Members** screen.</span></span>   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] <span data-ttu-id="0b885-145">**שימוש בנתוני שימוש**</span><span class="sxs-lookup"><span data-stu-id="0b885-145">**Use Usage**</span></span>    |    <span data-ttu-id="0b885-146">מייבא לתוך המסך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **‏‫הערכות פרוייקט‬**.</span><span class="sxs-lookup"><span data-stu-id="0b885-146">Omports into the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **Project Estimates** screen.</span></span>     |

<span data-ttu-id="0b885-147">**כדי לייבא ולפרסם את הפרוייקט שלך**</span><span class="sxs-lookup"><span data-stu-id="0b885-147">**To import and publish your project**</span></span>  
1. <span data-ttu-id="0b885-148">מתוך הכרטיסיה **Project Service**, לחץ על **פרסום** > **פרוייקט חדש של Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="0b885-148">From the **Project Service** tab, click **Publish** > **New Project Service Automation Project**.</span></span>  

2. <span data-ttu-id="0b885-149">בתיבת הדו שיח **פרסם בפרוייקט חדש ב- Project Service**, הזן את **שם הפרוייקט** ובחר את **הלקוח**.</span><span class="sxs-lookup"><span data-stu-id="0b885-149">On **Publish to a new project in Project Service** dialog box, enter the **Project Name** and select the **Customer**.</span></span>  

3. <span data-ttu-id="0b885-150">אם תרצה, תוכל לבחור את האפשרות **‏‫קשר את תוכנית הפרוייקט ל- Project Service Automation‬** כדי לקשר את קובץ תוכנית הפרוייקט אל Project Service Automation‬.</span><span class="sxs-lookup"><span data-stu-id="0b885-150">Optionally check the **Link project plan to Project Service Automation** to link the plan Project file to Project Service Automation.</span></span>  

4. <span data-ttu-id="0b885-151">לחץ על **פרסם**.</span><span class="sxs-lookup"><span data-stu-id="0b885-151">Click **Publish**.</span></span>  

   <span data-ttu-id="0b885-152">קישור קובץ הפרוייקט אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] הופך את קובץ הפרוייקט לקובץ ראשי ומגדיר את מבנה התפלגות העבודה ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="0b885-152">Linking the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes the Project file the master and sets the work breakdown structure in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to read-only.</span></span>  <span data-ttu-id="0b885-153">כדי לבצע שינויים בתוכנית הפרוייקט, עליך ליצור אותם ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולפרסם כעדכונים ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0b885-153">In order to make changes to the project plan, you need to make them in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and publish them as updates to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

## <a name="edit-a-project-thats-been-imported"></a><span data-ttu-id="0b885-154">עריכת פרוייקט מיובא</span><span class="sxs-lookup"><span data-stu-id="0b885-154">Edit a project that’s been imported</span></span>  
 <span data-ttu-id="0b885-155">כדי לבצע שינויים בתוכנית פרוייקט שיובאה לתוך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], עומדות בפניך שתי אפשרויות:</span><span class="sxs-lookup"><span data-stu-id="0b885-155">To make changes to a project plan that's been imported into [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you have two options:</span></span>  

- <span data-ttu-id="0b885-156">לפתוח את הקובץ הראשי ולערוך אותו ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="0b885-156">Open the master file and edit it in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

- <span data-ttu-id="0b885-157">לבטל את קישור הקובץ ולערוך אותו ישירות ב- Project Service.</span><span class="sxs-lookup"><span data-stu-id="0b885-157">Unlink the file and edit it directly in Project Service.</span></span> <span data-ttu-id="0b885-158">כברירת מחדל, פרוייקט שהועלה מתוך [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] נעול וניתן לערוך אותו רק ב- Project.</span><span class="sxs-lookup"><span data-stu-id="0b885-158">By default, a project that’s been uploaded from [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] is locked and can only be edited in Project.</span></span> <span data-ttu-id="0b885-159">כדי לערוך את הקובץ ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], יש לבטל את קישור הקובץ.</span><span class="sxs-lookup"><span data-stu-id="0b885-159">To edit the file in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], the file has to be unlinked.</span></span>  

### <a name="edit-in-pn_microsoft_project"></a><span data-ttu-id="0b885-160">לערוך ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span><span class="sxs-lookup"><span data-stu-id="0b885-160">Edit in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]</span></span>  

1. <span data-ttu-id="0b885-161">מתוך התפריט הראשי, לחץ על **Project Service** > **פרוייקטים**.</span><span class="sxs-lookup"><span data-stu-id="0b885-161">From the main menu, click **Project Service** > **Projects**.</span></span>  

2. <span data-ttu-id="0b885-162">מתוך רשימת הפרוייקטים, פתח את הפרוייקט שיצרת ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="0b885-162">From the list of projects, open the one you created in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

3. <span data-ttu-id="0b885-163">לחץ על **פתח ב- MS Project** מרצועת הכלים.</span><span class="sxs-lookup"><span data-stu-id="0b885-163">Click **Open in MS Project** from the ribbon.</span></span> <span data-ttu-id="0b885-164">פעולה זו תפתח את הקובץ הראשי המקושר ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="0b885-164">This will open the linked master file in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a><span data-ttu-id="0b885-165">ביטול קישור הקובץ ועריכתו ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service</span><span class="sxs-lookup"><span data-stu-id="0b885-165">Unlink a file and edit in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service</span></span>  

1. <span data-ttu-id="0b885-166">מתוך התפריט הראשי, לחץ על **Project Service** > **פרוייקטים**.</span><span class="sxs-lookup"><span data-stu-id="0b885-166">From the main menu, click **Project Service** > **Projects**.</span></span>  

2. <span data-ttu-id="0b885-167">מתוך רשימת הפרוייקטים, פתח את הפרוייקט שיצרת ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span><span class="sxs-lookup"><span data-stu-id="0b885-167">From the list of projects, open the one you created in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].</span></span>  

3. <span data-ttu-id="0b885-168">לחץ על **‏‫בטל את הקישור ל- MS Project‬** מרצועת הכלים.</span><span class="sxs-lookup"><span data-stu-id="0b885-168">Click **Unlink from MS Project** from the ribbon.</span></span>  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a><span data-ttu-id="0b885-169">העלאת קובץ פרוייקט ל- SharePoint או לקבוצות Office</span><span class="sxs-lookup"><span data-stu-id="0b885-169">Upload a Project file to SharePoint or Office Groups</span></span>  
 <span data-ttu-id="0b885-170">באפשרותך להעלות את קובץ Project שלך אל SharePoint ולמצוא אותו תחת 'מסמכים משויכים' עבור פרוייקט [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] שלך.</span><span class="sxs-lookup"><span data-stu-id="0b885-170">You can upload your Project file to SharePoint and find it under the Associated Documents for your [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  <span data-ttu-id="0b885-171">מנהל המערכת שלך צריך להגדיר את ניהול המסמכים של SharePoint ולהפעיל אותו עבור הישות 'פרוייקט'.</span><span class="sxs-lookup"><span data-stu-id="0b885-171">You need to have your administrator configure SharePoint document management and turn it on for the Project entity.</span></span> 

 <span data-ttu-id="0b885-172">באפשרותך גם להעלות את קובץ הפרוייקט שלך ל- [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] אם מוגדרות אצלך Office Groups.</span><span class="sxs-lookup"><span data-stu-id="0b885-172">You can also upload your Project file to [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] if you have Office Groups set up.</span></span>

### <a name="upload-a-file-for-sharepoint"></a><span data-ttu-id="0b885-173">העלאת קובץ עבור SharePoint</span><span class="sxs-lookup"><span data-stu-id="0b885-173">Upload a file for SharePoint</span></span>  

1. <span data-ttu-id="0b885-174">מתוך התפריט הראשי, לחץ על **Project Service** > **העלאה**.</span><span class="sxs-lookup"><span data-stu-id="0b885-174">From the main menu, click **Project Service** > **Upload**.</span></span>  

2. <span data-ttu-id="0b885-175">בחר **אל מסמכי פרוייקט של Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="0b885-175">Select **To Project Service Automation Project Documents**.</span></span>  

3. <span data-ttu-id="0b885-176">בדו-שיח **אפשר פתיחה ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**, בחר **כן** או **לא**.</span><span class="sxs-lookup"><span data-stu-id="0b885-176">On the **Enable Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** dialog, select **Yes** or **No**.</span></span>  

   - <span data-ttu-id="0b885-177">אם תלחץ על **כן**, תוכל לבחור בלחצן **פתח ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** ב- Project Service Automation, להפעיל את [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולטעון את קובץ הפרוייקט מתוך ספריית המסמכים של SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0b885-177">If you click **Yes**, you'll be able select the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button in Project Service Automation, launch [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], and load the Project file from the SharePoint document library.</span></span>  

   - <span data-ttu-id="0b885-178">אם תלחץ על **לא**, הקישור ללחצן **פתח ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** לא יעבוד.</span><span class="sxs-lookup"><span data-stu-id="0b885-178">If you click **No**, the link for the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button won't work.</span></span>  

4. <span data-ttu-id="0b885-179">ניתן למצוא את קובץ [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] תחת **מסמכים** עבור פרוייקט [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ספציפי.</span><span class="sxs-lookup"><span data-stu-id="0b885-179">The [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] file can be found in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] under **Documents** for the specific [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  

### <a name="upload-a-file-for-office-groups"></a><span data-ttu-id="0b885-180">העלאת קובץ ל- Office Groups</span><span class="sxs-lookup"><span data-stu-id="0b885-180">Upload a file for Office Groups</span></span>  

1. <span data-ttu-id="0b885-181">מתוך התפריט הראשי, לחץ על **Project Service** > **העלאה**.</span><span class="sxs-lookup"><span data-stu-id="0b885-181">From the main menu, click **Project Service** > **Upload**.</span></span>  

2. <span data-ttu-id="0b885-182">בחר **אל מסמכי פרוייקט של Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="0b885-182">Select **To Project Service Automation Project Documents**.</span></span>  

3. <span data-ttu-id="0b885-183">בדו-שיח **אפשר פתיחה ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**, בחר **כן** או **לא**.</span><span class="sxs-lookup"><span data-stu-id="0b885-183">On the **Enable Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** dialog, select **Yes** or **No**.</span></span>  

   - <span data-ttu-id="0b885-184">אם תלחץ על **כן**, תוכל לבחור בלחצן **פתח ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** ב- Project Service Automation, להפעיל את [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולטעון את קובץ הפרוייקט מתוך ספריית המסמכים של SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0b885-184">If you click **Yes**, you'll be able to select the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button in Project Service Automation, launch [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)], and load the Project file from the SharePoint document library.</span></span>  

   - <span data-ttu-id="0b885-185">אם תלחץ על **לא**, הקישור ללחצן **פתח ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** לא יעבוד.</span><span class="sxs-lookup"><span data-stu-id="0b885-185">If you click **No**, the link for the **Open in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** button won't work.</span></span>  

4. <span data-ttu-id="0b885-186">ניתן למצוא את קובץ [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] תחת **מסמכים** עבור פרוייקט [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ספציפי.</span><span class="sxs-lookup"><span data-stu-id="0b885-186">The [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] file can be found in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] under **Documents** for the specific [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] project.</span></span>  

## <a name="publish--your-project-as-a-template"></a><span data-ttu-id="0b885-187">פרסום הפרוייקט שלך כתבנית</span><span class="sxs-lookup"><span data-stu-id="0b885-187">Publish  your project as a template</span></span>  
 <span data-ttu-id="0b885-188">באפשרותך לשמור את הפרוייקט שלך ולעשות בו שימוש חוזר על-ידי שמירתו כתבנית פרוייקט ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0b885-188">You can save your project and reuse it by saving it as a project template in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  <span data-ttu-id="0b885-189">תבניות פרוייקט הן תוכניות פרוייקט הניתנות לשימוש חוזר ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0b885-189">Project templates are reusable project plans in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="0b885-190">[יצירת תבנית לפרוייקט (Project Service Automation)](../psa/create-project-template.md)</span><span class="sxs-lookup"><span data-stu-id="0b885-190">[Create a project template (Project Service Automation)](../psa/create-project-template.md)</span></span>  

1. <span data-ttu-id="0b885-191">מתוך הכרטיסיה **Project Service**, לחץ על **פרסום** > **תבנית פרוייקט חדשה של Project Service Automation**.</span><span class="sxs-lookup"><span data-stu-id="0b885-191">From the **Project Service** tab, click **Publish** > **New Project Service Automation Project Template**.</span></span>  

2. <span data-ttu-id="0b885-192">בתיבת הדו שיח **פרסם בפרוייקט חדש בתבנית Project Service**, הזן את **שם תבנית הפרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="0b885-192">On the **Publish to a new project in Project Service template** dialog box, enter the **Project template name**.</span></span>  

3. <span data-ttu-id="0b885-193">אם תרצה, תוכל לבחור את האפשרות **קשר את תוכנית הפרוייקט ל- Project Service Automation** כדי לקשר את קובץ הפרוייקט אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0b885-193">Optionally, check the **Link project plan to Project Service Automation** to link the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>  

4. <span data-ttu-id="0b885-194">לחץ על **פרסם**.</span><span class="sxs-lookup"><span data-stu-id="0b885-194">Click **Publish**.</span></span>  

<span data-ttu-id="0b885-195">קישור קובץ הפרוייקט אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] הופך את קובץ הפרוייקט לקובץ ראשי ומגדיר את מבנה התפלגות העבודה בתבנית [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="0b885-195">Linking the Project file to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] makes the Project file the master and sets the work breakdown structure in the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] template to read-only.</span></span>  <span data-ttu-id="0b885-196">כדי לבצע שינויים בתוכנית הפרוייקט, עליך ליצור אותם ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולפרסם כעדכונים ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span><span class="sxs-lookup"><span data-stu-id="0b885-196">In order to make changes to the project plan, you need to make them in [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] and publish them as updates to [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span>

### <a name="see-also"></a><span data-ttu-id="0b885-197">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="0b885-197">See Also</span></span>  
 [<span data-ttu-id="0b885-198">מדריך למנהל פרוייקט</span><span class="sxs-lookup"><span data-stu-id="0b885-198">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
