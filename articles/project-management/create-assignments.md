---
title: יצירת הקצאות משאבים
description: נושא זה מספק מידע על יצירת הקצאות למשאבים בעלי שם ולמשאבים כלליים.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 20eb3880b17fb1f765ad79bd720520b0c8004c0a
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077221"
---
# <a name="create-resource-assignments"></a><span data-ttu-id="9eae9-103">יצירת הקצאות משאבים</span><span class="sxs-lookup"><span data-stu-id="9eae9-103">Create resource assignments</span></span>

<span data-ttu-id="9eae9-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="9eae9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="9eae9-105">הקצאת משאבים היא שיוך ישיר של חבר צוות פרוייקט למשימת צומת עלה.</span><span class="sxs-lookup"><span data-stu-id="9eae9-105">A resource assignment is the direct association of a project team member to a leaf node task.</span></span> <span data-ttu-id="9eae9-106">נושא זה מספק מידע אודות הדרכים השונות להקצאת משאבים למשימות.</span><span class="sxs-lookup"><span data-stu-id="9eae9-106">This topic provides information about the different ways to assign resources.</span></span>

## <a name="create-a-generic-team-member-through-task-assignment"></a><span data-ttu-id="9eae9-107">יצירת חבר צוות כללי באמצעות הקצאת משימות</span><span class="sxs-lookup"><span data-stu-id="9eae9-107">Create a generic team member through task assignment</span></span>


<span data-ttu-id="9eae9-108">כשאתה יוצר חבר צוות כללי באמצעות הקצאת משימות, אתה יוצר מציין מיקום או משאב כללי.</span><span class="sxs-lookup"><span data-stu-id="9eae9-108">When you create a generic team member through task assignment, you create a placeholder or generic resource.</span></span> <span data-ttu-id="9eae9-109">משאב כללי זה מתאר את המאפיינים של המשאב בעל השם, שבסופו של דבר תרצה שיעבוד על המשימות.</span><span class="sxs-lookup"><span data-stu-id="9eae9-109">This generic resource describes the characteristics of the named resource you ultimately want to work on the tasks.</span></span> <span data-ttu-id="9eae9-110">לאחר מכן צור דרישה, או הגש בקשה באמצעות הדרישה, המשמשת לחיפוש ולהזמנה של משאב בעל שם.</span><span class="sxs-lookup"><span data-stu-id="9eae9-110">You then generate a requirement, or submit a request using the requirement, that is used to search for and book the named resource.</span></span>

1. <span data-ttu-id="9eae9-111">ברשת לוח זמנים עבור משימה, בחר בסמל המשאב בתא **משאב**.</span><span class="sxs-lookup"><span data-stu-id="9eae9-111">On the Schedule grid for a task, select the Resource icon in the **Resource** cell.</span></span>
2. <span data-ttu-id="9eae9-112">הקלד שם שישמש כשם המשאב מציין המיקום.</span><span class="sxs-lookup"><span data-stu-id="9eae9-112">Type a name to serve as the placeholder resource’s name.</span></span> <span data-ttu-id="9eae9-113">לדוגמה, מנהל תוכנית.</span><span class="sxs-lookup"><span data-stu-id="9eae9-113">For example, Program Manager.</span></span>
3. <span data-ttu-id="9eae9-114">בחר **צור** ובשדה **יצירה מהירה של חבר צוות פרוייקט** , הגדר את התפקיד עבור המשאב הכללי.</span><span class="sxs-lookup"><span data-stu-id="9eae9-114">Select **Create** , and in the **Quick Create Project Team Member** field, set the role for the generic resource.</span></span>
4. <span data-ttu-id="9eae9-115">הקצה משימות למשאב מציין מיקום זה לפי הצורך, על ידי בחירת המשאב עבור המשימה ב **בורר המשאבים** .</span><span class="sxs-lookup"><span data-stu-id="9eae9-115">Assign tasks as needed to this placeholder resource by selecting the resource on the **Resource Selector** for the task.</span></span> <span data-ttu-id="9eae9-116">המשאבים רשומים תחת **חברי צוות**.</span><span class="sxs-lookup"><span data-stu-id="9eae9-116">The resources listed under **Team Members**.</span></span>
5. <span data-ttu-id="9eae9-117">כאשר תסיים להקצות את המשאב הכללי, בחר את המשאב הכללי בכרטיסיה **צוות** ואז בחר **צור דרישה** כדי ליצור דרישת משאב עבור המשאב הכללי.</span><span class="sxs-lookup"><span data-stu-id="9eae9-117">When you’re finished assigning the generic resource, on the **Team** tab, select the generic resource, and then select **Generate Requirement** to create a resource requirement for the generic resource.</span></span>
6. <span data-ttu-id="9eae9-118">בחר **הזמן** עבור המשאב הכללי, ולאחר מכן השתמש בלוח הזמנים כדי למצוא ולהזמין משאב אמיתי.</span><span class="sxs-lookup"><span data-stu-id="9eae9-118">Select **Book** for the generic resource and then use the Schedule board to find and book a real resource.</span></span> <span data-ttu-id="9eae9-119">באפשרותך גם לשלוח את הדרישה למימוש על-ידי מנהל משאבים.</span><span class="sxs-lookup"><span data-stu-id="9eae9-119">You can also submit the requirement for fulfillment by a resource manager.</span></span>
7. <span data-ttu-id="9eae9-120">כאשר המשאב הכללי ממומש במלואו (מילוי דרישת משאבים חלקי לא יביא להקצאת משאבים) עם משאב בשם, המשאב הכללי יוסר מהצוות.</span><span class="sxs-lookup"><span data-stu-id="9eae9-120">When the generic resource is fully fulfilled (partial resource requirement fulfillment will not result in a resource assignment) with a named resource, the generic resource is removed from the team.</span></span> <span data-ttu-id="9eae9-121">ההקצאות של המשימות עבור המשאב הכללי מוקצות למשאב בעל השם שמילא את דרישת המשאב הכללי.</span><span class="sxs-lookup"><span data-stu-id="9eae9-121">The task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>

## <a name="assign-a-named-resource-from-the-list-of-all-bookable-resources"></a><span data-ttu-id="9eae9-122">הקצאת משאב בעל שם מתוך רשימת כל המשאבים הניתנים להזמנה</span><span class="sxs-lookup"><span data-stu-id="9eae9-122">Assign a named resource from the list of all bookable resources</span></span>

<span data-ttu-id="9eae9-123">באפשרותך להשתמש בתיבת החיפוש **בורר המשאבים** כדי לחפש את כל המשאבים הניתנים להזמנה ולהקצות אותם לכל משימת צומת עלה.</span><span class="sxs-lookup"><span data-stu-id="9eae9-123">You can use the search box in the **Resource Picker** to search all active bookable resources and assign them to any leaf node task.</span></span> <span data-ttu-id="9eae9-124">משאבים שהוקצו בדרך זו יתווספו לצוות ללא הזמנות.</span><span class="sxs-lookup"><span data-stu-id="9eae9-124">Resources assigned this way are added to the team without any bookings.</span></span> <span data-ttu-id="9eae9-125">הדבר דומה להוספת חבר צוות ובחירה באפשרות **ללא** כשיטת ההקצאה.</span><span class="sxs-lookup"><span data-stu-id="9eae9-125">This is similar to adding a team member and selecting **None** as the allocation method.</span></span> <span data-ttu-id="9eae9-126">המשאב מוצג בכרטיסיות **צוות** , **הקצאת משאבים** ו **התאמה** כמשאב עם הקצאות בלבד ועם גירעון של הזמנות.</span><span class="sxs-lookup"><span data-stu-id="9eae9-126">The resource is displayed on the **Team** , **Resource Assignment** , and **Reconciliation** tabs as resources with only assignments and a booking deficit.</span></span> <span data-ttu-id="9eae9-127">הזמן אותם אם ברצונך להשתמש בזמינות שלהם.</span><span class="sxs-lookup"><span data-stu-id="9eae9-127">Book them if you want to use their availability.</span></span>

1. <span data-ttu-id="9eae9-128">מרשת המשימות, הלוח או ציר הזמן, נווט אל התא **הוקצה ל:**.</span><span class="sxs-lookup"><span data-stu-id="9eae9-128">From the task grid, board, or timeline, navigate to the **Assigned To** cell.</span></span>
2. <span data-ttu-id="9eae9-129">בתיבת החיפוש התחל להקליד שם.</span><span class="sxs-lookup"><span data-stu-id="9eae9-129">In the search box, start typing a name.</span></span> <span data-ttu-id="9eae9-130">תוצאות החיפוש עבור השם מוצגות ב **בורר המשאבים** תחת **משאבים אחרים**.</span><span class="sxs-lookup"><span data-stu-id="9eae9-130">The search results for the name are displayed in the **Resource Selector** under **Other Resources**.</span></span>
3. <span data-ttu-id="9eae9-131">בחר את המשאב שברצונך להקצות למשימה או בחר את שם המשאב תחת **משאבי צוות אחרים**.</span><span class="sxs-lookup"><span data-stu-id="9eae9-131">Select the resource that you want to assign to the task or select the name of the resource under **Other Team Resources**.</span></span>
