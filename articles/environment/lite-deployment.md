---
title: פריסת Project Operations Lite
description: מאמר זה מספק מידע על אופן ההתקנה של Project Operations lite - מהעסקה ועד הפקת חשבונית פרופורמה.
author: stsporen
ms.date: 11/29/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 2c508f56b3018b6a86fea78bcf9ee4136e90f385
ms.sourcegitcommit: 38cb012502cbd640abbc21a0912b195112b27ccb
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 11/30/2022
ms.locfileid: "9810979"
---
# <a name="deploy-project-operations-lite"></a>פריסת Project Operations Lite

_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_



Project Operations תומך במספר מודלים של פריסה. כדי לקבוע את מודל הפריסה הטוב ביותר, ראה [סוגי פריסה](determine-deployment-type.md).


> [!IMPORTANT]
> פריסה זו, פריסת לייט - מהעסקה ועד להוצאת חשבונית פרופורמה, מביאה לפריסת **Dataverse בלבד של Project Operations**.

- [התקן את Project Operations לסביבת Dataverse חדשה](#new)
- [התקן בסביבת Dataverse קיימת](#existing)
- [התקן בסביבת Dataverse קיימת הכוללת רכיבי כתיבה כפולים](#existingdw)



## <a name="install-project-operations-lite-to-a-new-dataverse-environment"></a><a name="new"></a>התקן את Project Operations Lite בסביבת Dataverse חדשה

1. בתור [מנהל מערכת כללי או מנהל מערכת של Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) עם רישיון Project Operations, צור סביבת Dataverse חדשה [במרכז ניהול של PowerPlatform](https://admin.powerplatform.com). תוודא שהאפשרויות **צור מסד נתונים עבור סביבה זו** ו **Dynamics 365 Apps** זמינות. למידע נוסף, ראה [צור ונהל סביבות במרכז הניהול של Power Platform](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
1. בחר **Microsoft Dynamics 365 Project Operations** מרשימת הפריסה של יישומי Dynamics 365.


## <a name="install-project-operations-lite-to-an-existing-dataverse-environment"></a><a name="existing"></a>התקן את Project Operations Lite בסביבת Dataverse קיימת 
1. בתור [מנהל המערכת הכללי או מנהל המערכת של Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) עם רישיון של Project Operations, אתר את הסביבה ב[מרכז ניהול של Power Platform](https://admin.powerplatform.com) שבה ברצונך להתקין את Project Operations.
1. התקן את **Microsoft Dynamics 365 Project Operations** מרשימת הפריסה של יישומי Dynamics 365. לקבלת מידע נוסף, עיין ב[ניהול האפליקצות של Dynamics 365](/power-platform/admin/manage-apps).

## <a name="install-project-operations-lite-to-an-existing-dataverse-environment-where-dual-write-solutions-are-already-present"></a><a name="existingdw"></a>התקן את Project Operations Lite בסביבה Dataverse קיימת שבה כבר קיימים פתרונות כתיבה כפולה

אם ברצונך להמשיך להפעיל את Project Operations במצב פריסת Lite, עליך לבצע את השלבים הבאים:

1. בתור [מנהל המערכת הכללי או מנהל המערכת של Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) עם רישיון של Project Operations, אתר את הסביבה ב[מרכז ניהול של Power Platform](https://admin.powerplatform.com) שבה ברצונך להתקין את Project Operations.
1. התקן את **Microsoft Dynamics 365 Project Operations** מרשימת הפריסה של יישומי Dynamics 365. לקבלת מידע נוסף, עיין ב[ניהול האפליקצות של Dynamics 365](/power-platform/admin/manage-apps).
1. מכיוון שהסביבה שלך כוללת רכיבי כתיבה כפולים המסייעים באינטגרציה עם יישומי פיננסים ותפעול שמותקנים, התקנת Project Operations תתקין גם את היכולות וההרחבות הנדרשות לשילוב נתונים הקשורים לפרויקט עם יישומי פיננסים ותפעול. מכיוון שברצונך להפעיל את Project Operations בפריסת Lite, יש להסיר את רכיבי האינטגרציה הללו מכיוון שהם ייצרו הגבלות ותקורה עבור תרחישי פריסת Lite. הסר ידנית את הפתרונות **Dynamics 365 Project Operations כתיבה כפולה** ו- **Dynamics 365 Project Operations מפות ישויות של כתיבה כפולה** כדי להסיר רכיבים אלו.
1. עבור אל **Project Operations -> הגדרות -> פרמטרים**. פתח את דף הפרטים **פרמטר הפרויקט** והגדר את השדה **אופן הפעולה של שדרוג הפתרון** ל **לייט בלבד**. זה מבטיח שכל השדרוגים הבאים של Project Operations לא יחזירו את רכיבי האינטגרציה לתוך Project Operations.  

[!INCLUDE[footer-include](../includes/footer-banner.md)]
