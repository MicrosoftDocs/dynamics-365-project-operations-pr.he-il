---
title: פיתוח תבניות פרוייקט בעזרת 'העתק פרוייקט'
description: נושא זה מספק מידע על אופן יצירת תבניות פרוייקט באמצעות הפעולה המותאמת אישית העתק פרויקט.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: cb49109e8c199bc4569702ae844a19985534294d
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077248"
---
# <a name="develop-project-templates-with-copy-project"></a>פיתוח תבניות פרוייקט בעזרת 'העתק פרוייקט'

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

Dynamics 365 Project Operations תומך ביכולת להעתיק פרויקט ולהחזיר כל מטלה חזרה למשאבים הכלליים המייצגים את התפקיד. לקוחות יכולים להשתמש בפונקציונליות זו לבניית תבניות פרוייקט בסיסיות.

כשבוחרים **העתק פרויקט** , מצב פרויקט היעד מתעדכן. השתמש ב **סיבת המצב** כדי לקבוע מתי הושלמה פעולת ההעתקה. בחירה ב **העתק פרויקט** מעדכן גם את תאריך ההתחלה של הפרויקט לתאריך ההתחלה הנוכחי אם לא מזוהה תאריך יעד בישות פרויקט היעד.

## <a name="copy-project-custom-action"></a>פעולה מותאמת אישית 'העתק פרויקט' 

### <a name="name"></a>שם 

**msdyn_CopyProjectV2**

### <a name="input-parameters"></a>פרמטרי קלט
ישנם ‏שלושה פרמטרי קלט:

| פרמטר          | סוג   | ערכים                                                   | 
|--------------------|--------|----------------------------------------------------------|
| ProjectCopyOption  | String | **{"removeNamedResources":true}** או **{"clearTeamsAndAssignments":true}** |
| SourceProject      | הפניית ישות | פרויקט מקור |
| יעד             | הפניית ישות | פרויקט יעד |


- **{"clearTeamsAndAssignments":true}** : התנהגות ברירת המחדל עבור Project באינטרנט ותסיר את כל ההקצאות וחברי הצוות..
- **{"removeNamedResources":true}** אופן הפעולה המהווה ברירת המחדל ב-Project Operations שיחזיר את ההקצאות למשאבים כלליים.

לקבלת מידע נוסף על פעולות ברירת מחדל נוספיות, ראה [שימוש בפולות Web API](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)

## <a name="specify-fields-to-copy"></a>ציון שדות להעתקה 
כאשר נקראת הפעולה, **העתק פרויקט** יבדק את תצוגת הפרויקט **העתק עמודות פרוייקט** כדי לקבוע אילו שדות יש להעתיק בעת העתקת הפרויקט.
