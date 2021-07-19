---
title: מבט כולל על מצבי ניהול משאבים
description: נושא זה מספק מידע על ניהול משאבים ב- Dynamics 365 Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.custom: intro-internal
ms.openlocfilehash: 41265534661e51565bf31105ef69cec9b3b181c3
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 07/07/2021
ms.locfileid: "6367892"
---
# <a name="resource-management-modes-overview"></a>מבט כולל על מצבי ניהול משאבים

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_


Dynamics 365 Project Operations תומך בשני מצבים על מנת שתוכל לבצע את זרימת ההזמנות הכוללת. מצב הניהול מוגדר כפרמטר פרויקט וניתן לשנותו אם הצרכים העסקיים שלך משתנים.    

## <a name="central-mode"></a>מצב מרכזי
לארגונים שמרכזים את הקצאת המשאבים לפרויקטים, המצב המרכזי מספק דרך להבטיח שמנהלי הפרויקטים יוכלו להגדיר דרישות משאבים ברמת הפרויקט. מילוי דרישות המשאבים מוקצה למנהל משאבים. מנהלי פרויקטים יכולים לקבל או לדחות משאבים המוצעים על-ידי מנהל המשאבים.

![מצב מרכזי](./media/resource-management-central.png)

כדי לנהל משאבים במצב המרכזי, ראה:

- [הקצאת משאבים כלליים הניתנים להזמנה למשימה ויצירת דרישות משאבים](/dynamics365/project-service/assign-generic-bookable-resource)
- [הזמנת משאבים בעלי שם מדרישות משאב](/dynamics365/project-service/book-named-resource)
- [שליחת בקשת משאב](/dynamics365/project-service/submit-resource-request)
- [מימוש בקשה למשאב](/dynamics365/project-service/resource-management-fulfill-requests)
- [קבלה או דחייה של משאב פרויקט מוצע מבקשת משאב](/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a>מצב היברידי
לארגונים שנדרשת להם גמישות בהקצאת משאבים, המצב ההיברידי מאפשר גם למנהלי פרויקטים וגם למנהלי משאבים להזמין משאבים.

![מצב היברידי](./media/resource-management-hybrid.png)

בנוסף לתהליך המצב המרכזי הנתמך, עיין בנושאים הבאים לניהול כל זרימות ההזמנות הנתמכות הנוספות במצב היברידי:

הזמן משאב ישירות לפרויקט:
- [הזמנת משאבים בעלי שם הניתנים להזמנה לצוות פרויקט והקצאת משימות](/dynamics365/project-service/assign-named-bookable-resource)

הזמן משאב מדרישות משאב:
- [הקצאת משאבים כלליים הניתנים להזמנה למשימה ויצירת דרישות משאבים](/dynamics365/project-service/assign-generic-bookable-resource)
- [הזמנת משאבים בעלי שם מדרישות משאב](/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]