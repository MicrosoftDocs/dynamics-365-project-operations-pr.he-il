---
title: מבט כולל על מצבי ניהול משאבים
description: נושא זה מספק מידע על ניהול משאבים ב- Dynamics 365 Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 872f4f2878f474e16674932f23fe192c6a8de6eb
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279454"
---
# <a name="resource-management-modes-overview"></a>מבט כולל על מצבי ניהול משאבים

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_


Dynamics 365 Project Operations תומך בשני מצבים על מנת שתוכל לבצע את זרימת ההזמנות הכוללת. מצב הניהול מוגדר כפרמטר פרויקט וניתן לשנותו אם הצרכים העסקיים שלך משתנים.    

## <a name="central-mode"></a>מצב מרכזי
לארגונים שמרכזים את הקצאת המשאבים לפרויקטים, המצב המרכזי מספק דרך להבטיח שמנהלי הפרויקטים יוכלו להגדיר דרישות משאבים ברמת הפרויקט. מילוי דרישות המשאבים מוקצה למנהל משאבים. מנהלי פרויקטים יכולים לקבל או לדחות משאבים המוצעים על-ידי מנהל המשאבים.

![מצב מרכזי](./media/resource-management-central.png)

כדי לנהל משאבים במצב המרכזי, ראה:

- [הקצאת משאבים כלליים הניתנים להזמנה למשימה ויצירת דרישות משאבים](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [הזמנת משאבים בעלי שם מדרישות משאב](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)
- [שליחת בקשת משאב](https://docs.microsoft.com/dynamics365/project-service/submit-resource-request)
- [מימוש בקשה למשאב](https://docs.microsoft.com/dynamics365/project-service/resource-management-fulfill-requests)
- [קבלה או דחייה של משאב פרויקט מוצע מבקשת משאב](https://docs.microsoft.com/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a>מצב היברידי
לארגונים שנדרשת להם גמישות בהקצאת משאבים, המצב ההיברידי מאפשר גם למנהלי פרויקטים וגם למנהלי משאבים להזמין משאבים.

![מצב היברידי](./media/resource-management-hybrid.png)

בנוסף לתהליך המצב המרכזי הנתמך, עיין בנושאים הבאים לניהול כל זרימות ההזמנות הנתמכות הנוספות במצב היברידי:

הזמן משאב ישירות לפרויקט:
- [הזמנת משאבים בעלי שם הניתנים להזמנה לצוות פרויקט והקצאת משימות](https://docs.microsoft.com/dynamics365/project-service/assign-named-bookable-resource)

הזמן משאב מדרישות משאב:
- [הקצאת משאבים כלליים הניתנים להזמנה למשימה ויצירת דרישות משאבים](https://docs.microsoft.com/dynamics365/project-service/assign-generic-bookable-resource)
- [הזמנת משאבים בעלי שם מדרישות משאב](https://docs.microsoft.com/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]