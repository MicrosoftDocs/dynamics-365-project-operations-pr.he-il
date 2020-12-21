---
title: פיתוח תבניות פרוייקט בעזרת 'העתק פרוייקט'
description: נושא זה מספק מידע על אופן יצירת תבניות פרוייקט באמצעות הפעולה המותאמת אישית העתק פרויקט.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 22976730ef3c8c22ea028b27a6eb5f14fb88993e
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642409"
---
# <a name="develop-project-templates-with-copy-project"></a>פיתוח תבניות פרוייקט בעזרת 'העתק פרוייקט'

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Dynamics 365 Project Operations תומך ביכולת להעתיק פרויקט ולהחזיר כל משימה למשאבים הגנריים המייצגים את התפקיד. לקוחות יכולים להשתמש בפונקציונליות זו לבניית תבניות פרוייקט בסיסיות.

כשבוחרים **העתק פרויקט**, מצב פרויקט היעד מתעדכן. השתמש ב **סיבת המצב** כדי לקבוע מתי הושלמה פעולת ההעתקה. בחירה ב **העתק פרויקט** מעדכן גם את תאריך ההתחלה של הפרויקט לתאריך ההתחלה הנוכחי אם לא מזוהה תאריך יעד בישות פרויקט היעד.

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


- **{"clearTeamsAndAssignments":true}**: התנהגות ברירת המחדל עבור Project באינטרנט ותסיר את כל ההקצאות וחברי הצוות..
- **{"removeNamedResources":true}** אופן הפעולה המהווה ברירת המחדל ב-Project Operations שיחזיר את ההקצאות למשאבים כלליים.

לקבלת מידע נוסף על פעולות ברירת מחדל נוספיות, ראה [שימוש בפולות Web API](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)

## <a name="specify-fields-to-copy"></a>ציון שדות להעתקה 
כאשר נקראת הפעולה, **העתק פרויקט** יבדק את תצוגת הפרויקט **העתק עמודות פרוייקט** כדי לקבוע אילו שדות יש להעתיק בעת העתקת הפרויקט.
