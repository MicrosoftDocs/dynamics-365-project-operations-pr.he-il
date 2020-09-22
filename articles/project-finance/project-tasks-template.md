---
title: סנכרון משימות פרוייקטים ישירות מ- Project Service Automation ל- Finance and Operations
description: נושא זה מתאר את התבנית ואת המשימה הבסיסית המשמשות לסנכרון משימות פרוייקט ישירות מ- Microsoft Dynamics 365 Project Service Automation אל Dynamics 365 Finance.
author: KimANelson
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: d7f32327-33c4-43ab-b799-786210e93277
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 66a255346727c7ee4fbbf2920d2ef437ded03308
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751870"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a>סנכרון משימות פרוייקטים ישירות מ- Project Service Automation ל- Finance and Operations

[!include[banner](../includes/banner.md)]

נושא זה מתאר את התבנית ואת המשימה הבסיסית המשמשות לסנכרון משימות פרוייקט ישירות מ- Dynamics 365 Project Service Automation אל Dynamics 365 Finance.

> [!NOTE]
> - שילוב משימות פרוייקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונעילת פונקציונליות זמינים בגירסה 8.0.
> - אם אתה משתמש ב- Enterprise Edition 7.3.0, לאחר התקנת KB 4132657 ו- KB 4132660, תוכל להשתמש בתבניות לשילוב משימות פרוייקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונתונים בפועל, וכן להגדיר תצורה של נעילת פונקציונליות. אם עליך לאפס את ההפצות החשבונאיות, מומלץ להתקין גם את KB 4131710.
> - שילוב נתונים בפועל זמין בגירסה 8.0.1 ואילך.

## <a name="data-flow-for-project-service-automation-to-finance"></a>זרימת נתונים עבור Project Service Automation ל- Finance

פתרון השילוב Project Service Automation ל- Finance משתמש בתכונת שילוב הנתונים לסנכרון נתונים במופעים של Project Service Automation ו- Finance. תבנית השילוב שזמינה עם תכונת שילוב הנתונים מאפשרת זרימת נתונים על משימות פרוייקט מ- Project Service Automation ל- Finance.

האיור הבא מראה כיצד הנתונים מסונכרנים בין Project Service Automation ו- Finance.

[![זרימת נתונים לשילוב Project Service Automation עם Finance](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)

## <a name="template-and-task"></a>תבנית ומשימה

כדי לגשת לתבנית, במרכז הניהול של Microsoft Power Apps, בחר **פרוייקטים** ולאחר מכן, בפינה העליונה, בחר **פרוייקט חדש** כדי לבחור תבניות ציבוריות.

התבנית והמשימה הבסיסית הבאות משמשות לסנכרון משימות פרוייקט מ- Project Service Automation אל Finance:

- **שם התבנית בשילוב נתונים:** משימות פרוייקט (PSA ל- Fin and Ops)
- **שם המשימה בפרוייקט:** משימות פרוייקט

עליך לסנכרן חוזי פרוייקטים ופרוייקטים לפני שתוכל לסנכרן משימות פרוייקט.

## <a name="entity-set"></a>קבוצת ישויות

| Project Service Automation | כספים                             |
|----------------------------|-------------------------------------|
| משימות פרוייקט              | ישות שילוב למשימת פרוייקט |

## <a name="entity-flow"></a>זרימת ישות

משימות פרוייקטים מנוהלות ב- Project Service Automation והם מסונכרנים ל- Finance כפעילויות פרוייקט.

## <a name="prerequisites-and-mapping-setup"></a>דרישות מוקדמות והגדרת מיפוי

עליך לסנכרן חוזי פרוייקטים ופרוייקטים לפני שתוכל לסנכרן משימות פרוייקט.

## <a name="power-query"></a>Power Query

עליך להשתמש ב- Microsoft Power Query for Excel כדי לסנן נתונים אם מתקיים התנאי הזה:

- יש לך רשומות ספציפיות למשאבים במשימת הפרוייקט.

אם עליך להשתמש ב- Power Query, פעל לפי ההנחיה זו:

- תבנית משימות הפרוייקט (PSA ל- Fin and Ops) כוללת מסנן ברירת מחדל המסנן רשומות ספציפיות למשאבים ממשימת פרוייקט על ידי הגדרת המסנן ל- **IsLineTask** בתור **False**. אם אתה יוצר תבנית משלך, עליך להוסיף מסנן זה.

## <a name="template-mapping-in-data-integration"></a>מיפוי תבנית בשילוב נתונים

האיור הבא מציג דוגמה למיפויי משימת התבנית בשילוב נתונים. המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.

[![מיפוי תבנית](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)
