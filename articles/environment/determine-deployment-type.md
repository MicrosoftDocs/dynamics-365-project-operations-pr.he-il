---
title: קביעת סוג הפריסה
description: מאמר זה מספק מידע שיעזור לך לקבוע את סוג הפריסה הנכון של Project Operations עבור החברה שלך.
author: stsporen
ms.date: 03/15/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 592c1bfdaf5ea6bdbf6c67bc5b82dd5cf979b367
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912195"
---
# <a name="determine-your-deployment-type"></a>קביעת סוג הפריסה

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

> [!IMPORTANT]
> לאחר רכישת הרישיון, התחל כאן כדי לקבוע את מודל הפריסה הטוב ביותר של Dynamics 365 Project Operations באמצעות [זרימת התקנה מודרכת](https://aka.ms/provisionprojectoperations).
> לאחר שתסיים את זרימת ההתקנה המודרכת, תועבר לפורטל הניהול הנכון להשלמת ההתקנה. עיין בפרטי הפריסה להשלמת ההתקנה.


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a>לקוחות קיימים של Dynamics באמצעות Dynamics 365 Project Service Automation
Project Operations כולל את היכולות שנשלחו עם Project Service Automation. נתיב שדרוג ישוחרר ללקוחות אלה בגל הפצה 1 של 2021.

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a>לקוחות קיימים של Dynamics 365 Finance המשתמשים בניהול פרויקטים וחשבונאות 

לקוחות קיימים של Finance המשתמשים בפונקציונליות ניהול פרויקטים וחשבונאות יכולים להמשיך להשתמש בה כפי שהיא. ראה את [Project Operations לתרחישי מלאי/הזמנת ייצור](#pma).


## <a name="deployment-regions"></a>אזורי פריסה
כדי לקבוע אילו אזורים תומכים בפריסה של Project Operations, ראה [זמינות גיאוגרפית עבור Dynamics 365 ו- Power Platform](https://dynamics.microsoft.com/en-us/geographic-availability/). בחר באפשרות **צפה בדוח**, והרחב את **Dynamics 365 > יישומי תפעול > Dynamics 365 Project Operations** לצפייה באזורים הנתמכים.

## <a name="deployment-types"></a>סוגי פריסה
Project Operations תומך במספר אפשרויות פריסה כדי להתאים לדרישות שלך. בין אם אתה לקוח חדש או קיים של Dynamics 365, ‏Project Operations יכול לתמוך בצרכים שלך.

[שאלון פריסה](https://aka.ms/provisionprojectoperations) שלנו יעזור לך לקבוע את הפריסה הנכונה. התוצאות ינחו אותך לעבר אחד מסוגי הפריסה הבאים:

- [פריסה קלה – עסקה לחשבונית פרופורמה](#lite)
- [Project Operations לתרחישים של משאבים/ללא מלאי](#integrated)
- [Project Operations לתרחישי מלאי/הזמנת ייצור](#pma)

Project Operations תומכות בתרחישים של מלאי/הזמנת ייצור ותרחישים ללא מלאי / מבוססי משאבים באותה סביבה באמצעות תצורות ברמת הישות המשפטית. לדוגמה, חברת Contoso יכולה להשתמש ביכולות הזמנת מלאי/הייצורבמתקן הייצור בארה"ב (היישות המשפטית = Contoso Manufacturing United States). Contoso יכולה להשתמש ביכולות שאינן במלאי/מבוססות משאבים במתקן השירות שלהם Contoso Robotics Arms בבריטניה (ישות משפטית = Contoso Robotics בריטניה).

### <a name="lite-deployment---deal-to-proforma-invoicing"></a><a  name="lite"></a>פריסה קלה – עסקה לחשבונית פרופורמה

הפריסת הלייט כוללת את היכולות הבאות:

- תהליך מכירה לפרויקטים המרחיב את חווית היישום של Dynamics 365 Sales
- תכנון פרויקטים באמצעות Microsoft Project באינטרנט
- תמחור רב-ממדי
- ניהול משאבים מאוחד
- מעקב אחר זמנים
- הוצאה בסיסית
- חשבוניות פרופורמה לבדיקה ולעריכה על-ידי מנהל הפרויקט 

#### <a name="deployment-steps"></a>שלבי הפריסה
קבע את מודל הפריסה הטוב ביותר של Project Operations באמצעות [שאלון הפריסה](https://aka.ms/provisionprojectoperations).

לפריסה זו, ראה [הירשם למנוי Preview](lite-preview-subscription-sign-up.md) ו[להקצאת סביבה חדשה](lite-deployment.md). 


### <a name="project-operations-for-resourcenon-stocked-scenarios"></a><a name="integrated"></a>Project Operations לתרחישים של משאבים/ללא מלאי
Project Operations עבור תרחישי משאבים/ללא מלאי כולל את היכולות הבאות:
 
- תהליך מכירה לפרויקטים המרחיב את חווית היישום של Dynamics 365 Sales
- תכנון פרויקטים באמצעות Microsoft Project באינטרנט
- תמחור רב-ממדי
- ניהול משאבים מאוחד
- מעקב אחר זמנים
- הוצאה בסיסית
- הוצאה מלאה
- קבלת OCR
- הפקת חשבוניות פרופורמה וחשבונית המוצגות ללקוח 
- הכרה בהכנסות מפרויקטים

#### <a name="deployment-steps"></a>שלבי הפריסה
קבע את מודל הפריסה הטוב ביותר של Project Operations באמצעות [שאלון הפריסה](https://aka.ms/provisionprojectoperations).

לפריסה זו, ראה [הירשם למנוי Preview](resource-sign-up-preview-subscription.md) ו[להקצאת סביבה חדשה](resource-provision-new-environment.md). 


### <a name="project-operations-for-stockedproduction-order-scenarios"></a><a name="pma"></a>Project Operations לתרחישי מלאי/הזמנת ייצור

- תכנון פרוייקטים באמצעות WBS
- ניהול משאבים
- מעקב אחר זמנים
- הוצאה מלאה
- קבלת OCR
- הפקת חשבונית מלאה
- זיהוי הכנסה
- הזמנות ייצור
- ‏‫תמיכה בחומרים במלאי‬ בעזרת מלאי

#### <a name="deployment-steps"></a>שלבי הפריסה
קבע את מודל הפריסה הטוב ביותר של Project Operations באמצעות [שאלון הפריסה](https://aka.ms/provisionprojectoperations).

לפריסה זו, ראה [הירשם למנוי Preview](/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=%2fdynamics365%2ffinance%2ftoc.json) ו[להקצאת סביבה חדשה](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=%2fdynamics365%2ffinance%2ftoc.json). 



[!INCLUDE[footer-include](../includes/footer-banner.md)]