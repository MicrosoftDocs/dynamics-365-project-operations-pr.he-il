---
title: פריסת Project Operations - לייט
description: נושא זה מספק מידע על אופן ההתקנה של פריסת Project Operations בגרסת לייט - מהעסקה ועד להוצאת חשבונית פרופורמה.
author: stsporen
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 0633585fcef91d9218d6140764addb7cf96ab31d
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/30/2020
ms.locfileid: "4175667"
---
# <a name="deploy-project-operations---lite"></a><span data-ttu-id="dd0d2-103">פריסת Project Operations - לייט</span><span class="sxs-lookup"><span data-stu-id="dd0d2-103">Deploy Project Operations - lite</span></span>

<span data-ttu-id="dd0d2-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="dd0d2-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="dd0d2-105">Project Operations תומך במספר מודלים של פריסה.</span><span class="sxs-lookup"><span data-stu-id="dd0d2-105">Project Operations supports multiple deployment models.</span></span> <span data-ttu-id="dd0d2-106">כדי לקבוע את מודל הפריסה הטוב ביותר, ראה [סוגי פריסה](determine-deployment-type.md).</span><span class="sxs-lookup"><span data-stu-id="dd0d2-106">To determine the best deployment model, see [Deployment types](determine-deployment-type.md).</span></span>


> [!IMPORTANT]
> <span data-ttu-id="dd0d2-107">פריסה זו, פריסת לייט - מהעסקה ועד להוצאת חשבונית פרופורמה, מביאה לפריסת **Common Data Service בלבד של Project Operations**.</span><span class="sxs-lookup"><span data-stu-id="dd0d2-107">This deployment, Lite deployment – deal to proforma invoicing, results in a **Common Data Service-only deployment of Project Operations**.</span></span>

- [<span data-ttu-id="dd0d2-108">התקן את Project Operations לסביבת CDS חדשה</span><span class="sxs-lookup"><span data-stu-id="dd0d2-108">Install Project Operations into a new CDS environment</span></span>](#new)
- [<span data-ttu-id="dd0d2-109">התקן בסביבת CDS קיימת</span><span class="sxs-lookup"><span data-stu-id="dd0d2-109">Install into an existing CDS environment</span></span>](#existing)



## <a name="install-project-operations-to-a-new-cds-environment"></a><a name="new"></a><span data-ttu-id="dd0d2-110">התקן את Project Operations בסביבת CDS חדשה</span><span class="sxs-lookup"><span data-stu-id="dd0d2-110">Install Project Operations to a new CDS environment</span></span>

1. <span data-ttu-id="dd0d2-111">בתור [מנהל מערכת כללי או מנהל מערכת של Power Platform](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) עם רישיון Project Operations, צור סביבת CDS חדשה ב[מרכז ניהול של Power Platform](https://admin.powerplatform.com).</span><span class="sxs-lookup"><span data-stu-id="dd0d2-111">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, create a new CDS environment in the [PowerPlatform admin center](https://admin.powerplatform.com).</span></span> <span data-ttu-id="dd0d2-112">ודא ש **מסד הנתונים של CDS** ו-**‏האפליקציות של Dynamics 365** זמינים.</span><span class="sxs-lookup"><span data-stu-id="dd0d2-112">Make sure that **CDS database** and **Dynamics 365 Apps** are enabled.</span></span> <span data-ttu-id="dd0d2-113">למידע נוסף, ראה [צור ונהל סביבות במרכז הניהול של Power Platform](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span><span class="sxs-lookup"><span data-stu-id="dd0d2-113">For more information, see [Create and manage environments in the Power Platform admin center](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span></span>
2. <span data-ttu-id="dd0d2-114">בחר **Microsoft Dynamics 365 Project Operations** מרשימת הפריסה של אפליקציות של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="dd0d2-114">Select **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span>


## <a name="install-project-operations-to-an-existing-cds-environment"></a><a name="existing"></a><span data-ttu-id="dd0d2-115">התקן את Project Operations בסביבת CDS חדשה</span><span class="sxs-lookup"><span data-stu-id="dd0d2-115">Install Project Operations to an existing CDS environment</span></span>

1. <span data-ttu-id="dd0d2-116">בתור [מנהל המערכת הכללי או מנהל המערכת של Power Platform](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) עם רישיון של Project Operations, אתר את הסביבה ב[מרכז ניהול של Power Platform](https://admin.powerplatform.com) שבה ברצונך להתקין את Project Operations.</span><span class="sxs-lookup"><span data-stu-id="dd0d2-116">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, locate the environment in the [PowerPlatform admin center](https://admin.powerplatform.com) where you want to install Project Operations.</span></span>
2. <span data-ttu-id="dd0d2-117">התקן את **Microsoft Dynamics 365 Project Operations** מרשימת הפריסה של אפליקציות של Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="dd0d2-117">Install **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span> <span data-ttu-id="dd0d2-118">לקבלת מידע נוסף, עיין ב[ניהול האפליקצות של Dynamics 365](https://docs.microsoft.com/power-platform/admin/manage-apps).</span><span class="sxs-lookup"><span data-stu-id="dd0d2-118">For more information, see [Manage Dynamics 365 apps](https://docs.microsoft.com/power-platform/admin/manage-apps).</span></span>


