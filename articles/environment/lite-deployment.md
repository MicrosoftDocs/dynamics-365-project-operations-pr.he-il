---
title: פריסת Project Operations - לייט
description: נושא זה מספק מידע על אופן ההתקנה של פריסת Project Operations בגרסת לייט - מהעסקה ועד להוצאת חשבונית פרופורמה.
author: stsporen
ms.date: 10/02/2020
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: cb1f1ad86e19d84d68a40b32b2fdb08dc4777a78
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995532"
---
# <a name="deploy-project-operations---lite"></a><span data-ttu-id="8d030-103">פריסת Project Operations - לייט</span><span class="sxs-lookup"><span data-stu-id="8d030-103">Deploy Project Operations - lite</span></span>

<span data-ttu-id="8d030-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="8d030-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="8d030-105">Project Operations תומך במספר מודלים של פריסה.</span><span class="sxs-lookup"><span data-stu-id="8d030-105">Project Operations supports multiple deployment models.</span></span> <span data-ttu-id="8d030-106">כדי לקבוע את מודל הפריסה הטוב ביותר, ראה [סוגי פריסה](determine-deployment-type.md).</span><span class="sxs-lookup"><span data-stu-id="8d030-106">To determine the best deployment model, see [Deployment types](determine-deployment-type.md).</span></span>


> [!IMPORTANT]
> <span data-ttu-id="8d030-107">פריסה זו, פריסת לייט - מהעסקה ועד להוצאת חשבונית פרופורמה, מביאה לפריסת **Common Data Service בלבד של Project Operations**.</span><span class="sxs-lookup"><span data-stu-id="8d030-107">This deployment, Lite deployment – deal to proforma invoicing, results in a **Common Data Service-only deployment of Project Operations**.</span></span>

- [<span data-ttu-id="8d030-108">התקן את Project Operations לסביבת CDS חדשה</span><span class="sxs-lookup"><span data-stu-id="8d030-108">Install Project Operations into a new CDS environment</span></span>](#new)
- [<span data-ttu-id="8d030-109">התקן בסביבת CDS קיימת</span><span class="sxs-lookup"><span data-stu-id="8d030-109">Install into an existing CDS environment</span></span>](#existing)



## <a name="install-project-operations-to-a-new-cds-environment"></a><a name="new"></a><span data-ttu-id="8d030-110">התקן את Project Operations בסביבת CDS חדשה</span><span class="sxs-lookup"><span data-stu-id="8d030-110">Install Project Operations to a new CDS environment</span></span>

1. <span data-ttu-id="8d030-111">בתור [מנהל מערכת כללי או מנהל מערכת של Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) עם רישיון Project Operations, צור סביבת CDS חדשה ב[מרכז ניהול של Power Platform](https://admin.powerplatform.com).</span><span class="sxs-lookup"><span data-stu-id="8d030-111">As the [Global or Power Platform Administrator](/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, create a new CDS environment in the [PowerPlatform admin center](https://admin.powerplatform.com).</span></span> <span data-ttu-id="8d030-112">ודא ש **מסד הנתונים של CDS** ו-**‏האפליקציות של Dynamics 365** זמינים.</span><span class="sxs-lookup"><span data-stu-id="8d030-112">Make sure that **CDS database** and **Dynamics 365 Apps** are enabled.</span></span> <span data-ttu-id="8d030-113">למידע נוסף, ראה [צור ונהל סביבות במרכז הניהול של Power Platform](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span><span class="sxs-lookup"><span data-stu-id="8d030-113">For more information, see [Create and manage environments in the Power Platform admin center](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span></span>
2. <span data-ttu-id="8d030-114">בחר **Microsoft Dynamics 365 Project Operations** מרשימת הפריסה של יישומי Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="8d030-114">Select **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span>


## <a name="install-project-operations-to-an-existing-cds-environment"></a><a name="existing"></a><span data-ttu-id="8d030-115">התקן את Project Operations בסביבת CDS חדשה</span><span class="sxs-lookup"><span data-stu-id="8d030-115">Install Project Operations to an existing CDS environment</span></span>

1. <span data-ttu-id="8d030-116">בתור [מנהל המערכת הכללי או מנהל המערכת של Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) עם רישיון של Project Operations, אתר את הסביבה ב[מרכז ניהול של Power Platform](https://admin.powerplatform.com) שבה ברצונך להתקין את Project Operations.</span><span class="sxs-lookup"><span data-stu-id="8d030-116">As the [Global or Power Platform Administrator](/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, locate the environment in the [PowerPlatform admin center](https://admin.powerplatform.com) where you want to install Project Operations.</span></span>
2. <span data-ttu-id="8d030-117">התקן את **Microsoft Dynamics 365 Project Operations** מרשימת הפריסה של יישומי Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="8d030-117">Install **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span> <span data-ttu-id="8d030-118">לקבלת מידע נוסף, עיין ב[ניהול האפליקצות של Dynamics 365](/power-platform/admin/manage-apps).</span><span class="sxs-lookup"><span data-stu-id="8d030-118">For more information, see [Manage Dynamics 365 apps](/power-platform/admin/manage-apps).</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]