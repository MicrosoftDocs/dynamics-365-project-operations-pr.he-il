---
title: פריסת Project Operations - לייט
description: נושא זה מספק מידע על אופן ההתקנה של פריסת Project Operations בגרסת לייט - מהעסקה ועד להוצאת חשבונית פרופורמה.
author: stsporen
ms.date: 02/28/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: e33506504665f2e7ef7ad48469082f9f64a2a44b
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8580733"
---
# <a name="deploy-project-operations---lite"></a>פריסת Project Operations - לייט

_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_



Project Operations תומך במספר מודלים של פריסה. כדי לקבוע את מודל הפריסה הטוב ביותר, ראה [סוגי פריסה](determine-deployment-type.md).


> [!IMPORTANT]
> פריסה זו, פריסת לייט - מהעסקה ועד להוצאת חשבונית פרופורמה, מביאה לפריסת **Dataverse בלבד של Project Operations**.

- [התקן את Project Operations לסביבת Dataverse חדשה](#new)
- [התקן בסביבת Dataverse קיימת](#existing)



## <a name="install-project-operations-to-a-new-dataverse-environment"></a><a name="new"></a>התקן את Project Operations בסביבת Dataverse חדשה

1. בתור [מנהל מערכת כללי או מנהל מערכת של Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) עם רישיון Project Operations, צור סביבת Dataverse חדשה [במרכז ניהול של PowerPlatform](https://admin.powerplatform.com). תוודא שהאפשרויות **צור מסד נתונים עבור סביבה זו** ו **Dynamics 365 Apps** זמינות. למידע נוסף, ראה [צור ונהל סביבות במרכז הניהול של Power Platform](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
2. בחר **Microsoft Dynamics 365 Project Operations** מרשימת הפריסה של יישומי Dynamics 365.


## <a name="install-project-operations-to-an-existing-dataverse-environment"></a><a name="existing"></a>התקן את Project Operations בסביבת Dataverse חדשה
1. ודא שהסביבה לא הוגדרה באמצעות [כתיבה כפולה](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-overview) מכיוון שאז ההתקנה תתקין את יכולות [Project Operations עבור תרחישים מבוססי משאבים/לא מלאי](project-operations-integrated-deployment-overview.md).
2. בתור [מנהל המערכת הכללי או מנהל המערכת של Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) עם רישיון של Project Operations, אתר את הסביבה ב[מרכז ניהול של Power Platform](https://admin.powerplatform.com) שבה ברצונך להתקין את Project Operations.
3. התקן את **Microsoft Dynamics 365 Project Operations** מרשימת הפריסה של יישומי Dynamics 365. לקבלת מידע נוסף, עיין ב[ניהול האפליקצות של Dynamics 365](/power-platform/admin/manage-apps).




[!INCLUDE[footer-include](../includes/footer-banner.md)]
