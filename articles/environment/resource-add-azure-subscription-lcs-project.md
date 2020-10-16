---
title: הוסף מנוי Azure לפרויקט LCS
description: נושא זה מספק מידע על אופן חיבור המנוי שלך ל- Azure אל פרויקט LCS.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 0b5703542ac58adcc710890d9676dd0090a82f25
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948891"
---
# <a name="add-an-azure-subscription-to-lcs-project"></a><span data-ttu-id="a037f-103">הוסף מנוי Azure לפרויקט LCS</span><span class="sxs-lookup"><span data-stu-id="a037f-103">Add an Azure subscription to LCS project</span></span>

<span data-ttu-id="a037f-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="a037f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="a037f-105">יש לפרוס סביבות המתארחות בענן באמצעות מנוי קיים ל- Azure.</span><span class="sxs-lookup"><span data-stu-id="a037f-105">Cloud-hosted environments must be deployed using an existing Azure subscription.</span></span> <span data-ttu-id="a037f-106">נושא זה מסביר איך לחבר את המנוי הקיים שלך ל- Azure אל פרויקט LCS.</span><span class="sxs-lookup"><span data-stu-id="a037f-106">This topic explains how to connect your existing Azure subscription to an LCS project.</span></span> 

## <a name="grant-admin-consent"></a><span data-ttu-id="a037f-107">הענק הסכמה של מנהל מערכת</span><span class="sxs-lookup"><span data-stu-id="a037f-107">Grant admin consent</span></span>

1. <span data-ttu-id="a037f-108">בפרויקט LCS שלך, במקטע **סביבות**, בחר **הגדרות Microsoft Azure**.</span><span class="sxs-lookup"><span data-stu-id="a037f-108">In your LCS project, in the **Environments** section, select **Microsoft Azure settings**.</span></span>

![הגדרות Microsoft Azure](./media/1MicrosoftAzureSettings.png)

2. <span data-ttu-id="a037f-110">בדף **הגדרות פרויקט**, בכרטיסיה **מחברי Azure**, בחר באפשרות **אשר**.</span><span class="sxs-lookup"><span data-stu-id="a037f-110">On the **Project settings** page, on the **Azure connectors** tab, select **Authorize**.</span></span> <span data-ttu-id="a037f-111">כך מתאפשר לפרוס את הסביבות בפרויקט זה.</span><span class="sxs-lookup"><span data-stu-id="a037f-111">This allows environments to be deployed to this project.</span></span>

![מחברי Azure](./media/2AzureConnectors.png)

3. <span data-ttu-id="a037f-113">בחר שוב באפשרות **אשר** כדי לספק הסכמה של מנהל מערכת.</span><span class="sxs-lookup"><span data-stu-id="a037f-113">Select **Authorize** again to provide admin consent.</span></span>

![הענק הסכמה של מנהל מערכת](./media/3GrantAdminConsent.png)

4. <span data-ttu-id="a037f-115">קבל את בקשת ההרשאות.</span><span class="sxs-lookup"><span data-stu-id="a037f-115">Accept the permissions request.</span></span>

![קבל בקשת הרשאות](./media/4AcceptPermissionRequest.png)

<span data-ttu-id="a037f-117">ההרשאה הושלמה כעת.</span><span class="sxs-lookup"><span data-stu-id="a037f-117">The authorization is now complete.</span></span> 

![ההרשאה נקבעה בהצלחה](./media/5AuthorizationComplete.png)

## <a name="provide-dynamics-deployment-services-access-to-your-azure-subscription"></a><a name="provide"></a><span data-ttu-id="a037f-119">ספק גישה אל Dynamics Deployment Services למנוי שלך ב- Azure</span><span class="sxs-lookup"><span data-stu-id="a037f-119">Provide Dynamics Deployment Services access to your Azure subscription</span></span>

1. <span data-ttu-id="a037f-120">עבור אל [חיוב Microsoft Azure](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) ובחר את המנוי שלך.</span><span class="sxs-lookup"><span data-stu-id="a037f-120">Go to [Microsoft Azure billing](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) and select your subscription.</span></span> <span data-ttu-id="a037f-121">כדי שתהיה אפשרות לפרוס סביבות, ל- Dynamics Deployment Services צריכה להיות גישה למנוי זה.</span><span class="sxs-lookup"><span data-stu-id="a037f-121">Dynamics Deployment Services needs to access this subscription to be able to deploy environments.</span></span>

![פרטי מנוי Azure](./media/6AzureSubscription.png)

2. <span data-ttu-id="a037f-123">בחר באפשרות **בקרת גישה (IAM)** בחלונית הניווט ולאחר מכן בחר באפשרות **הוסף הקצאת תפקיד**.</span><span class="sxs-lookup"><span data-stu-id="a037f-123">Select **Access control (IAM)** in the navigation pane, and then select **Add role assignment**.</span></span>
3. <span data-ttu-id="a037f-124">במחוון שבצד ימין, בחר באפשרות **תפקיד תורם** וברשימה הנפתחת, אתר ובחר את האפשרות **Dynamics Deployment Services**.</span><span class="sxs-lookup"><span data-stu-id="a037f-124">In the slider on the right side, select **Contributor role**, and in the list provided, find and select **Dynamics Deployment Services**.</span></span> 
4. <span data-ttu-id="a037f-125">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="a037f-125">Select **Save**.</span></span>

![גישה למנוי](./media/7SubscriptionAccess.png)

### <a name="add-a-subscription-connector-to-an-lcs-project"></a><span data-ttu-id="a037f-127">הוסף מחבר מנוי לפרויקט LCS</span><span class="sxs-lookup"><span data-stu-id="a037f-127">Add a subscription connector to an LCS project</span></span>

1. <span data-ttu-id="a037f-128">בפרויקט LCS שלך, בדף **הגדרות Microsoft Azure**, בחר באפשרות **הוסף** כדי להוסיף מחבר חדש.</span><span class="sxs-lookup"><span data-stu-id="a037f-128">In your LCS project, on the **Microsoft Azure settings** page, select **Add** to add a new connector.</span></span>
2. <span data-ttu-id="a037f-129">הזן את מזהה המנוי שלך ב- Azure.</span><span class="sxs-lookup"><span data-stu-id="a037f-129">Enter your Azure subscription ID.</span></span> <span data-ttu-id="a037f-130">אתה יכול למצוא את מזהה המנוי שלך [בפורטל Azure](https://ms.portal.azure.com/), בקטע  **הגדרות**  בפינה השמאלית התחתונה של המסך.</span><span class="sxs-lookup"><span data-stu-id="a037f-130">You can find your Azure subscription ID in the [Azure portal](https://ms.portal.azure.com/), under  **Settings**  in the lower left of the screen.</span></span>
3. <span data-ttu-id="a037f-131">בשדה **קבע את התצורה של Azure Resource Manager**, בחר באפשרות **כן**.</span><span class="sxs-lookup"><span data-stu-id="a037f-131">In the **Configure to use Azure Resource Manager** field, select **Yes**.</span></span>
4. <span data-ttu-id="a037f-132">ודא שתחום דייר AAD של מנוי Azure תואם למנוי Azure המוגדר כבעלים של התחום שבו אתה משתמש, ובחר באפשרות **הבא**.</span><span class="sxs-lookup"><span data-stu-id="a037f-132">Make sure Azure's Subscription AAD Tenant Domain matches the domain-owning Azure subscription that you are using, and select **Next**.</span></span>
5. <span data-ttu-id="a037f-133">במסך **הגדרת Microsoft Azure**, בחר באפשרות **הבא** כדי לאשר.</span><span class="sxs-lookup"><span data-stu-id="a037f-133">On the **Microsoft Azure Setup** screen, select **Next** to confirm.</span></span> <span data-ttu-id="a037f-134">אם נתקלת בשגיאה במסך זה, חזור למקטע [ספק גישה אל Dynamics Deployment Services למנוי שלך ב- Azure](#provide) בנושא זה כדי לוודא שהשלמת את כל השלבים.</span><span class="sxs-lookup"><span data-stu-id="a037f-134">If you receive an error on this screen, return to the section [Provide Dynamics Deployment Services access to Azure subscription](#provide) in this topic and make sure you have completed all of the steps.</span></span>
6. <span data-ttu-id="a037f-135">הורד את Azure Management Certificate לתיקיה מקומית במחשב שלך ולאחר מכן העלה אותו אל Azure Management Portal על-ידי מעבר אל **הגדרות** > **אישורי ניהול**.</span><span class="sxs-lookup"><span data-stu-id="a037f-135">Download the Azure Management Certificate to a local folder on your computer, and then upload it to Azure Management Portal by going to **Settings** > **Management Certificates**.</span></span> <span data-ttu-id="a037f-136">אישור זה יאפשר ל- LCS לתקשר עם Azure בשמך.</span><span class="sxs-lookup"><span data-stu-id="a037f-136">This certificate will enable LCS to communicate with Azure on your behalf.</span></span> <span data-ttu-id="a037f-137">אתה יכול לדלג על שלב זה אם למשתמש שלך יש גישה למנוי.</span><span class="sxs-lookup"><span data-stu-id="a037f-137">You can skip this step if your user has access to the subscription.</span></span>
7. <span data-ttu-id="a037f-138">בחר באפשרות  **הבא**.</span><span class="sxs-lookup"><span data-stu-id="a037f-138">Select  **Next**.</span></span>
8. <span data-ttu-id="a037f-139">בחר את אזור Azure לפריסה ובחר מרכז נתונים הקרוב למקום בו אתה מתכנן להשתמש במערכת זו.</span><span class="sxs-lookup"><span data-stu-id="a037f-139">Select the Azure region to deploy in and select a data center that is close to where you plan to use this system.</span></span>
9.  <span data-ttu-id="a037f-140">בחר באפשרות  **התחבר**.</span><span class="sxs-lookup"><span data-stu-id="a037f-140">Select  **Connect**.</span></span>

<span data-ttu-id="a037f-141">חיברת בהצלחה את המנוי שלך ל- Azure.</span><span class="sxs-lookup"><span data-stu-id="a037f-141">You have successfully connected your Azure subscription.</span></span> <span data-ttu-id="a037f-142">כעת תוכל לפרוס סביבות המתארחות בענן של Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="a037f-142">You can now deploy Dynamics 365 Finance cloud-hosted environments.</span></span>


