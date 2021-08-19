---
title: סנכרון משימות פרויקטים ישירות מ- Project Service Automation ל- Finance and Operations
description: נושא זה מתאר את התבנית ואת המשימה הבסיסית המשמשות לסנכרון משימות פרויקט ישירות מ- Microsoft Dynamics 365 Project Service Automation אל Dynamics 365 Finance.
author: Yowelle
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 45846d7a6dd7b84fe28f0a78ccc103679236917ea506180c5b383fd2828624eb
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/06/2021
ms.locfileid: "6992792"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a>סנכרון משימות פרויקטים ישירות מ- Project Service Automation ל- Finance and Operations

[!include[banner](../includes/banner.md)]

נושא זה מתאר את התבנית ואת המשימה הבסיסית המשמשות לסנכרון משימות פרויקט ישירות מ- Dynamics 365 Project Service Automation אל Dynamics 365 Finance.

> [!NOTE]
> - שילוב משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונעילת פונקציונליות זמינים בגירסה 8.0.
> - אם אתה משתמש ב- Enterprise Edition 7.3.0, לאחר התקנת KB 4132657 ו- KB 4132660, תוכל להשתמש בתבניות לשילוב משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונתונים בפועל, וכן להגדיר תצורה של נעילת פונקציונליות. אם עליך לאפס את ההפצות החשבונאיות, מומלץ להתקין גם את KB 4131710.
> - שילוב נתונים בפועל זמין בגירסה 8.0.1 ואילך.

## <a name="data-flow-for-project-service-automation-to-finance"></a>זרימת נתונים עבור Project Service Automation ל- Finance

פתרון השילוב Project Service Automation ל- Finance משתמש בתכונת שילוב הנתונים לסנכרון נתונים במופעים של Project Service Automation ו- Finance. תבנית השילוב שזמינה עם תכונת שילוב הנתונים מאפשרת זרימת נתונים על משימות פרויקט מ- Project Service Automation ל- Finance.

האיור הבא מראה כיצד הנתונים מסונכרנים בין Project Service Automation ו- Finance.

[![זרימת נתונים לשילוב Project Service Automation עם Finance.](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)

## <a name="template-and-task"></a>תבנית ומשימה

כדי לגשת לתבנית, במרכז הניהול של Microsoft Power Apps, בחר **פרויקטים** ולאחר מכן, בפינה העליונה, בחר **פרויקט חדש** כדי לבחור תבניות ציבוריות.

התבנית והמשימה הבסיסית הבאות משמשות לסנכרון משימות פרויקט מ- Project Service Automation אל Finance:

- **שם התבנית בשילוב נתונים:** משימות פרויקט (PSA ל- Fin and Ops)
- **שם המשימה בפרויקט:** משימות פרויקט

עליך לסנכרן חוזי פרויקטים ופרויקטים לפני שתוכל לסנכרן משימות פרויקט.

## <a name="entity-set"></a>קבוצת ישויות

| Project Service Automation | כספים                             |
|----------------------------|-------------------------------------|
| משימות פרויקט              | ישות שילוב למשימת פרויקט |

## <a name="entity-flow"></a>זרימת ישות

משימות פרויקטים מנוהלות ב- Project Service Automation והם מסונכרנים ל- Finance כפעילויות פרויקט.

## <a name="prerequisites-and-mapping-setup"></a>דרישות מוקדמות והגדרת מיפוי

עליך לסנכרן חוזי פרויקטים ופרויקטים לפני שתוכל לסנכרן משימות פרויקט.

## <a name="power-query"></a>Power Query

עליך להשתמש ב- Microsoft Power Query for Excel כדי לסנן נתונים אם מתקיים התנאי הזה:

- יש לך רשומות ספציפיות למשאבים במשימת הפרויקט.

אם עליך להשתמש ב- Power Query, פעל לפי ההנחיה זו:

- תבנית משימות הפרויקט (PSA ל- Fin and Ops) כוללת מסנן ברירת מחדל המסנן רשומות ספציפיות למשאבים ממשימת פרויקט על ידי הגדרת המסנן ל- **IsLineTask** בתור **False**. אם אתה יוצר תבנית משלך, עליך להוסיף מסנן זה.

## <a name="template-mapping-in-data-integration"></a>מיפוי תבנית בשילוב נתונים

האיור הבא מציג דוגמה למיפויי משימת התבנית בשילוב נתונים. המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.

[![מיפוי תבנית.](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]