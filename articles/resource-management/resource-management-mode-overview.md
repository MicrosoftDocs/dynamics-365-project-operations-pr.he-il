---
title: מבט כולל על מצבי ניהול משאבים
description: מאמר זה מספק מידע על פונקציולניות ניהול המשאבים ב- Dynamics 365 Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: overview
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: dd50d12686a6ad17f6a95ccf0c2f1447cc470bf7
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8928433"
---
# <a name="resource-management-modes-overview"></a>מבט כולל על מצבי ניהול משאבים

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_


Dynamics 365 Project Operations תומך בשני מצבים על מנת שתוכל לבצע את זרימת ההזמנות הכוללת. מצב הניהול מוגדר כפרמטר פרויקט וניתן לשנותו אם הצרכים העסקיים שלך משתנים.    

## <a name="central-mode"></a>מצב מרכזי
לארגונים שמרכזים את הקצאת המשאבים לפרויקטים, המצב המרכזי מספק דרך להבטיח שמנהלי הפרויקטים יוכלו להגדיר דרישות משאבים ברמת הפרויקט. מילוי דרישות המשאבים מוקצה למנהל משאבים. מנהלי פרויקטים יכולים לקבל או לדחות משאבים המוצעים על-ידי מנהל המשאבים.

![מצב מרכזי.](./media/resource-management-central.png)

כדי לנהל משאבים במצב המרכזי, ראה:

- [הקצאת משאבים כלליים הניתנים להזמנה למשימה ויצירת דרישות משאבים](/dynamics365/project-service/assign-generic-bookable-resource)
- [הזמנת משאבים בעלי שם מדרישות משאב](/dynamics365/project-service/book-named-resource)
- [שליחת בקשת משאב](/dynamics365/project-service/submit-resource-request)
- [מימוש בקשה למשאב](/dynamics365/project-service/resource-management-fulfill-requests)
- [קבלה או דחייה של משאב פרויקט מוצע מבקשת משאב](/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a>מצב היברידי
לארגונים שנדרשת להם גמישות בהקצאת משאבים, המצב ההיברידי מאפשר גם למנהלי פרויקטים וגם למנהלי משאבים להזמין משאבים.

![מצב היברידי.](./media/resource-management-hybrid.png)

בנוסף לתהליך המצב המרכזי הנתמך, עיין במאמרים הבאים כדי לנהל את כל זרימות ההזמנות הנתמכות האחרות במצב היברידי:

הזמן משאב ישירות לפרויקט:
- [הזמנת משאבים בעלי שם הניתנים להזמנה לצוות פרויקט והקצאת משימות](/dynamics365/project-service/assign-named-bookable-resource)

הזמן משאב מדרישות משאב:
- [הקצאת משאבים כלליים הניתנים להזמנה למשימה ויצירת דרישות משאבים](/dynamics365/project-service/assign-generic-bookable-resource)
- [הזמנת משאבים בעלי שם מדרישות משאב](/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]