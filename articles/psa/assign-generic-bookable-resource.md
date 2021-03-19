---
title: הקצאת משאבים כלליים הניתנים להזמנה למשימה וצוות פרוייקט
description: נושא זה מספק מידע אודות הזמנת משאבים כלליים למשימות ולצוותי פרוייקט.
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 12/11/2018
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
ms.openlocfilehash: 5b4c47513b96310745fd2cdb296988a57df0e966
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5291395"
---
# <a name="assign-generic-bookable-resources-to-a-task-and-generate-resource-requirements"></a><span data-ttu-id="8177f-103">הקצאת משאבים כלליים הניתנים להזמנה למשימה ויצירת דרישות משאבים</span><span class="sxs-lookup"><span data-stu-id="8177f-103">Assign generic bookable resources to a task and generate resource requirements</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="8177f-104">בנוסף להזמנה והקצאה של משאבים בעלי שם או משאבים ממשיים לפרוייקט שלך, באפשרותך להקצות משאבים כלליים למשימות פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="8177f-104">In addition to booking and assigning named or real resources to your project, you can assign generic resources to project tasks.</span></span> <span data-ttu-id="8177f-105">משאבים אלה יכולים לשמש כמצייני מיקום עבור משאבים בעלי שם עד שתהיה מוכן לאייש את הפרוייקט עם משאבים בעלי שם.</span><span class="sxs-lookup"><span data-stu-id="8177f-105">These resources can serve as placeholders for named resources until you are ready to staff your project with named resources.</span></span> 

1. <span data-ttu-id="8177f-106">ב- Project Service Automation‏ (PSA), פתח את הדף **פרוייקט** ובכרטיסיה **לוח זמנים**, הזן את שם המשרה של המשאב הכללי בתא **משאב** של לוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="8177f-106">In Project Service Automation (PSA), open the **Project** page and on the **Schedule** tab, enter the position name of the generic resource in the **Resource** cell of the schedule.</span></span> <span data-ttu-id="8177f-107">לחלופין, לחץ על סמל **משאב** בתא כדי לפתוח את בורר המשאבים ולאחר מכן, הזן את שם המשאב הכללי שברצונך ליצור.</span><span class="sxs-lookup"><span data-stu-id="8177f-107">Or, click the **Resource** icon in the cell to open the resource picker and then enter the name of the generic resource that you want to create.</span></span>

![יצירה והקצאה של חבר צוות כללי](media/RM-how-to-9.png)

<span data-ttu-id="8177f-109">פעולה זו תפתח את החלונית **יצירה מהירה: חבר צוות פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="8177f-109">This will open the **Quick Create: Project Team Member** panel.</span></span> 

2. <span data-ttu-id="8177f-110">הזן את התפקיד והיחידה הארגונית של חבר הצוות של המשאב הכללי ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="8177f-110">Enter the role and organization unit of the generic resource team member and then click **Save**.</span></span>

![יצירה מהירה של חבר צוות כללי](media/RM-how-to-10.png)

3. <span data-ttu-id="8177f-112">לאחר שיצרת את חבר הצוות של המשאב הכללי החדש, הוא מוקצה למשימה.</span><span class="sxs-lookup"><span data-stu-id="8177f-112">After you have created the new generic resource team member, it is assigned to the task.</span></span> <span data-ttu-id="8177f-113">באפשרותך להמשיך להקצות משאב כללי זה למשימות אחרות בלוח הזמנים של המשימה.</span><span class="sxs-lookup"><span data-stu-id="8177f-113">You can continue to assign that generic resource to other tasks in the task schedule.</span></span>

![הקצאת חבר צוות כללי קיים למשימות](media/RM-how-to-11.png)

4. <span data-ttu-id="8177f-115">לאחר שהקצית את המשאב הכללי, באפשרותך ליצור דרישת משאב ולממש אותה על-ידי הזמנה ישירה או שליחת בקשת משאב למנהל משאבים.</span><span class="sxs-lookup"><span data-stu-id="8177f-115">After you have assigned the generic resource, you can generate a resource requirement and fulfill it by directly booking or submitting a resource request to a resource manager.</span></span>

![יצירת דרישה עבור חבר צוות כללי](media/RM-how-to-12.png)

<span data-ttu-id="8177f-117">ברשת חבר הצוות, בנוסף ליכולת להשתמש בבורר המשאבים כפי שמוזכר לעיל, באפשרותך להוסיף משאבים כלליים באופן ישיר.</span><span class="sxs-lookup"><span data-stu-id="8177f-117">On the team member grid, in addition to being able to use the resource picker as mentioned above, you can add generic resources directly.</span></span> <span data-ttu-id="8177f-118">המשאבים מתווספים עם דרישת משאב המבוססת על תאריכי ההתחלה/סיום ושיטת ההקצאה המצוינים בחלונית **יצירה מהירה: חבר צוות פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="8177f-118">The resources are added with a resource requirement that is based on the start/end dates and allocation method specified in the **Quick Create: Project Team Member** panel.</span></span>

<span data-ttu-id="8177f-119">באפשרותך לראות הבדל אם אתה מוסיף את חבר הצוות הכללי באופן ישיר ולאחר מכן מקצה למשאב הכללי משימות נוספות שחורגות מהשעות הנדרשות לכיסוי שיש לו.</span><span class="sxs-lookup"><span data-stu-id="8177f-119">You can see a difference if you add the generic team member directly and then assign more tasks to the generic resource than they have required hours to cover.</span></span> <span data-ttu-id="8177f-120">לחץ על **צור דרישה** כדי ליצור מחדש את הדרישה לאיזון השעות הנדרשות מול ההקצאות.</span><span class="sxs-lookup"><span data-stu-id="8177f-120">Click **Generate Requirement** to regenerate the requirement to balance the required hours against assignments.</span></span>

<span data-ttu-id="8177f-121">באפשרותך גם ללחוץ על הקישור **דרישת משאב** ברשת הצוות כדי לפתוח את הדרישה ולהוסיף כישורים, משאבים מועדפים וכדומה.</span><span class="sxs-lookup"><span data-stu-id="8177f-121">You can also click the **Resource requirement** link in the team grid to open the requirement and add skills, preferred resources, etc.</span></span>

![דרישת משאב](media/RM-how-to-13.png)



[!INCLUDE[footer-include](../includes/footer-banner.md)]