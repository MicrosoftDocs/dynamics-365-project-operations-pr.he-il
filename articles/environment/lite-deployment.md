---
title: פריסה של Project Operations בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה
description: נושא זה מספק מידע על אופן ההתקנה של פריסת Project Operations בגרסת לייט - מהעסקה ועד להוצאת חשבונית פרופורמה.
author: stsporen
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: e938876d459b3f6dfedd90e57e3042cda96bffb7
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077172"
---
# <a name="deploy-project-operations-lite-deployment--deal-to-proforma-invoicing"></a>פריסה של Project Operations בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה

_**חל על** : פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_

Project Operations תומך במספר מודלים של פריסה. כדי לקבוע את מודל הפריסה הטוב ביותר, ראה [סוגי פריסה](determine-deployment-type.md).


> [!IMPORTANT]
> פריסה זו, פריסת לייט - מהעסקה ועד להוצאת חשבונית פרופורמה, מביאה לפריסת **Common Data Service בלבד של Project Operations**.

- [התקן את Project Operations לסביבת CDS חדשה](#new)
- [התקן בסביבת CDS קיימת](#existing)



## <a name="install-project-operations-to-a-new-cds-environment"></a><a name="new"></a>התקן את Project Operations בסביבת CDS חדשה

1. בתור [מנהל מערכת כללי או מנהל מערכת של Power Platform](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) עם רישיון Project Operations, צור סביבת CDS חדשה ב[מרכז ניהול של Power Platform](https://admin.powerplatform.com). ודא ש **מסד הנתונים של CDS** ו- **‏האפליקציות של Dynamics 365** זמינים. למידע נוסף, ראה [צור ונהל סביבות במרכז הניהול של Power Platform](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
2. בחר **Microsoft Dynamics 365 Project Operations** מרשימת הפריסה של אפליקציות של Dynamics 365.


## <a name="install-project-operations-to-an-existing-cds-environment"></a><a name="existing"></a>התקן את Project Operations בסביבת CDS חדשה

1. בתור [מנהל המערכת הכללי או מנהל המערכת של Power Platform](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) עם רישיון של Project Operations, אתר את הסביבה ב[מרכז ניהול של Power Platform](https://admin.powerplatform.com) שבה ברצונך להתקין את Project Operations.
2. התקן את **Microsoft Dynamics 365 Project Operations** מרשימת הפריסה של אפליקציות של Dynamics 365. לקבלת מידע נוסף, עיין ב[ניהול האפליקצות של Dynamics 365](https://docs.microsoft.com/power-platform/admin/manage-apps).


