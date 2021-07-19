---
title: פריסה ידנית של אפליקציית Dataverse ‏Project Operations עם תמיכה בכתיבה כפולה
description: נושא זה מסביר כיצד לפרוס ידנית את האפליקציה Dataverse של Project Operations כך שהיא תתמוך בכתיבה כפולה.
author: stsporen
ms.date: 06/18/2021
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 2ad147da542fc9e7a2705da7a834d1a6512907e5
ms.sourcegitcommit: 205a94ab4168de25b102f31d00a691c8205ba63e
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/18/2021
ms.locfileid: "6274009"
---
# <a name="manually-deploy-the-project-operations-dataverse-app-with-dual-write-support"></a><span data-ttu-id="17a7d-103">פריסה ידנית של אפליקציית Dataverse ‏Project Operations עם תמיכה בכתיבה כפולה</span><span class="sxs-lookup"><span data-stu-id="17a7d-103">Manually deploy the Project Operations Dataverse app with dual-write support</span></span>

<span data-ttu-id="17a7d-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="17a7d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="17a7d-105">נושא זה מסביר כיצד לפרוס ידנית את Microsoft Dynamics 365 Project Operations ב- Microsoft Dataverse כך שהיא תתמוך בכתיבה כפולה.</span><span class="sxs-lookup"><span data-stu-id="17a7d-105">This topic explains how to manually deploy Microsoft Dynamics 365 Project Operations in Microsoft Dataverse so that it supports dual-write.</span></span> <span data-ttu-id="17a7d-106">Project Operations מזהה את תצורת הסביבה ומוסיף תמיכה בכתיבה כפולה אם מתקיימים התנאים המוקדמים.</span><span class="sxs-lookup"><span data-stu-id="17a7d-106">Project Operations detects the environment's configuration and adds additional support for dual-write if the prerequisites are met.</span></span>

<span data-ttu-id="17a7d-107">במהלך פריסה דרך Microsoft Dynamics Lifecycle Services (LCS), אם בצעת את ההנחיות בנושא זה, תוכל לדלג על הפריסה של שילוב Microsoft Power Platform (נקראה קודם סביבת Common Data Service).</span><span class="sxs-lookup"><span data-stu-id="17a7d-107">During deployment through Microsoft Dynamics Lifecycle Services (LCS), if you've followed the instructions in this topic, you can skip the deployment of the Microsoft Power Platform integration (previously known as the Common Data Service environment).</span></span>

<span data-ttu-id="17a7d-108">לתהליך הפרידה של Project Operations ב- Dataverse לצורך תמיכה בכתיבה כפולה יש ארבעה שלבים עיקריים:</span><span class="sxs-lookup"><span data-stu-id="17a7d-108">The process of deploying Project Operations in Dataverse so that it supports dual-write has four main steps:</span></span>

1. <span data-ttu-id="17a7d-109">[צור סביבה חדשה ב- Dataverse התומכת בכתיבה כפולה](#create).</span><span class="sxs-lookup"><span data-stu-id="17a7d-109">[Create a new environment in Dataverse that supports dual-write](#create).</span></span>
2. <span data-ttu-id="17a7d-110">[הוסף תנאים מוקדמים לכתיבה כפולה לסביבה](#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="17a7d-110">[Add dual-write prerequisites to the environment](#prerequisites).</span></span>
3. <span data-ttu-id="17a7d-111">[הוסף את אפליקציית Project Operations Dataverse](#dataverse).</span><span class="sxs-lookup"><span data-stu-id="17a7d-111">[Add the Project Operations Dataverse app](#dataverse).</span></span>
4. <span data-ttu-id="17a7d-112">[קשר אל הסביבות שלך](#link).</span><span class="sxs-lookup"><span data-stu-id="17a7d-112">[Link your environments](#link).</span></span>

## <a name="create-a-new-environment-in-dataverse-that-supports-dual-write"></a><a name="create"></a><span data-ttu-id="17a7d-113">צור סביבה חדשה ב- Dataverse התומכת בכתיבה כפולה</span><span class="sxs-lookup"><span data-stu-id="17a7d-113">Create a new environment in Dataverse that supports dual-write</span></span>

<span data-ttu-id="17a7d-114">להשלמת הליך זה, עליך להתחבר כמנהל מערכת.</span><span class="sxs-lookup"><span data-stu-id="17a7d-114">To complete this procedure, you must sign in as an administrator.</span></span>

1. <span data-ttu-id="17a7d-115">פתח את [מרכז הניהול של Power Platform](https://admin.powerplatform.com) והיכנס כמנהל מערכת.</span><span class="sxs-lookup"><span data-stu-id="17a7d-115">Open the [Power Platform admin center](https://admin.powerplatform.com), and sign in as an administrator.</span></span>
2. <span data-ttu-id="17a7d-116">צור סביבה חדשה ותן לה שם.</span><span class="sxs-lookup"><span data-stu-id="17a7d-116">Create a new environment, and name it.</span></span>
3. <span data-ttu-id="17a7d-117">בחר את סוג הסביבה.</span><span class="sxs-lookup"><span data-stu-id="17a7d-117">Select the environment type.</span></span> <span data-ttu-id="17a7d-118">אם נרשמת לגירסת הניסיון, בחר **גירסת ניסיון (מבוסס מנוי)**.</span><span class="sxs-lookup"><span data-stu-id="17a7d-118">If you signed up for the trial offer, select **Trial (subscription-based)**.</span></span>
4. <span data-ttu-id="17a7d-119">אשר את אזור הפריסה.</span><span class="sxs-lookup"><span data-stu-id="17a7d-119">Confirm the deployment region.</span></span>
5. <span data-ttu-id="17a7d-120">הפעל את האפשרות **צור מסד נתונים עבור סביבה זו**.</span><span class="sxs-lookup"><span data-stu-id="17a7d-120">Enable the **Create a database for this environment** option.</span></span> 
6. <span data-ttu-id="17a7d-121">אשר את השפה ולאחר מכן אשר שהמטבע תואם למטבע של יישומי Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="17a7d-121">Confirm the language, and then confirm that the currency matches the currency for your Finance and Operations apps.</span></span>
7. <span data-ttu-id="17a7d-122">הפעל את האפשרות **יישומי Dynamics 365**, ואשר שהשדה **פרוס יישומים אלה באופן אוטומטי** מוגדר **אף אחד**.</span><span class="sxs-lookup"><span data-stu-id="17a7d-122">Enable the **Dynamics 365 apps** option, and confirm that the **Automatically deploy these apps** field is set to **None**.</span></span>
8. <span data-ttu-id="17a7d-123">הוסף קבוצת אבטחה אם נדרשת קבוצת אבטחה.</span><span class="sxs-lookup"><span data-stu-id="17a7d-123">Add a security group, if a security group is required.</span></span>
9. <span data-ttu-id="17a7d-124">בחר **שמור** כדי ליצור סביבה חדשה.</span><span class="sxs-lookup"><span data-stu-id="17a7d-124">Select **Save** to create the environment.</span></span>
10. <span data-ttu-id="17a7d-125">המתן עד להשלמת הפריסה כך שהסביבה מגיעה למצב **מוכן**.</span><span class="sxs-lookup"><span data-stu-id="17a7d-125">Wait until the deployment is completed and the environment reaches the **Ready** state.</span></span>

## <a name="add-dual-write-prerequisites-to-the-environment"></a><a name="prerequisites"></a><span data-ttu-id="17a7d-126">הוסף תנאים מוקדמים לכתיבה כפולה לסביבה</span><span class="sxs-lookup"><span data-stu-id="17a7d-126">Add dual-write prerequisites to the environment</span></span>

<span data-ttu-id="17a7d-127">תמיכה בכתיבה כפולה כוללת שדות נוספים שמתווספים לישויות מפתח, כמו הישות **חברה**.</span><span class="sxs-lookup"><span data-stu-id="17a7d-127">Dual-write support includes additional fields that are added to key entities, such as the **Company** entity.</span></span> <span data-ttu-id="17a7d-128">אם אתה מוסיף תמיכה בכתיבה כפולה לסביבה קיימת, ייתכן שיהיה עליך לעדכן את הנתונים כדי לאפשר את התמיכה.</span><span class="sxs-lookup"><span data-stu-id="17a7d-128">If you're adding dual-write support to an existing environment, you might have to update the data to enable the support.</span></span> <span data-ttu-id="17a7d-129">למידע על אופן האתחול של הנתונים, ראה [נתוני חברת Bootstrap](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data).</span><span class="sxs-lookup"><span data-stu-id="17a7d-129">For information about how to bootstrap the data, see [Bootstrap company data](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data).</span></span> <span data-ttu-id="17a7d-130">למידע נוסף על כתיבה כפולה, ראה [דרישות מערכת לכתיבה כפולה](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req).</span><span class="sxs-lookup"><span data-stu-id="17a7d-130">For more information about dual-write, see [Dual-write system requirements](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req).</span></span>

<span data-ttu-id="17a7d-131">השלם הליך זה כדי להוסיף את התנאים המוקדמים לכתיבה כפולה לסביבה שלך.</span><span class="sxs-lookup"><span data-stu-id="17a7d-131">Complete this procedure to add the dual-write prerequisites to your environment.</span></span>

1. <span data-ttu-id="17a7d-132">פתח את הסביבה שיצרת זה עתה, ועבור אל **משאב** \> **יישומי Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="17a7d-132">Open the environment that you just created, and then go to **Resource** \> **Dynamics 365 apps**.</span></span>
2. <span data-ttu-id="17a7d-133">בחר **פתרון ליבה של כתיבה כפולה** ברשימת האפליקציות והתקן אותו.</span><span class="sxs-lookup"><span data-stu-id="17a7d-133">Select **Dual-write core solution** in the app list, and install it.</span></span>
3. <span data-ttu-id="17a7d-134">המתן עד לסיום ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="17a7d-134">Wait until the installation is completed.</span></span> <span data-ttu-id="17a7d-135">בחר **פתרון התיאום של הכתיבה הכפולה** ברשימת האפליקציות והתקן אותו.</span><span class="sxs-lookup"><span data-stu-id="17a7d-135">Then select **Dual-write application orchestration solution** in the app list, and install it.</span></span>

## <a name="add-the-project-operations-dataverse-app"></a><a name="dataverse"></a><span data-ttu-id="17a7d-136">הוסף את אפליקציית Dataverse של Project Operations</span><span class="sxs-lookup"><span data-stu-id="17a7d-136">Add the Project Operations Dataverse app</span></span>

<span data-ttu-id="17a7d-137">ניתן להשלים הליך זה רק אם השלמת את השלבים הקודמים לפני שהתקנת את Project Operations.</span><span class="sxs-lookup"><span data-stu-id="17a7d-137">You can complete this procedure only if you completed the previous procedures before you installed Project Operations.</span></span> <span data-ttu-id="17a7d-138">במהלך ההתקנה, המערכת מנתחת את תצורת הסביבה ומוסיפה תמיכה בכתיבה כפולה אם היא נדרשת.</span><span class="sxs-lookup"><span data-stu-id="17a7d-138">During installation, the system analyzes the environment configuration and adds support for dual-write if it's required.</span></span>

1. <span data-ttu-id="17a7d-139">פתח את הסביבה שיצרת, ועבור אל **משאב** \> **יישומי Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="17a7d-139">Open the environment that you created earlier, and then go to **Resource** \> **Dynamics 365 apps**.</span></span>
2. <span data-ttu-id="17a7d-140">בחר **Microsoft Dynamics 365 Project Operations** ברשימת האפליקציות והתקן אותה.</span><span class="sxs-lookup"><span data-stu-id="17a7d-140">Select **Microsoft Dynamics 365 Project Operations** in the app list, and install it.</span></span>

## <a name="link-your-environments"></a><a name="link"></a><span data-ttu-id="17a7d-141">קשר אל הסביבות שלך</span><span class="sxs-lookup"><span data-stu-id="17a7d-141">Link your environments</span></span>

<span data-ttu-id="17a7d-142">לאחר הפריסה של סביבת Dataverse, אתה יכול להגדיר את הקישור לאפליקציות Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="17a7d-142">After the Dataverse environment is deployed, you can set up the link in your Finance and Operations apps.</span></span> <span data-ttu-id="17a7d-143">בצע את השלבים במקטע [השתמש באשף הכתיבה הכפולה לקישור הסביבות שלך](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment).</span><span class="sxs-lookup"><span data-stu-id="17a7d-143">Follow the steps in [Use the dual-write wizard to link your environments](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment).</span></span>
