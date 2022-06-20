---
title: מבט כולל על Project Service Automation
description: מאמר זה מספק מידע על Dynamics 365 Project Service Automation לפתרון השילוב של Dynamics 365 Finance.
author: ruhercul
ms.date: 07/25/2019
ms.topic: overview
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: johnmichalak
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: ruhercul
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 96fdb31b7b1d4f33cb565cf902039f72a3f90fd7
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8929583"
---
# <a name="project-service-automation-overview"></a>מבט כולל על Project Service Automation

[!include[banner](../includes/banner.md)]


פתרון השילוב של Project Service Automation to Finance משתמש בתכונת שילוב הנתונים כדי לסנכרן נתונים בין מופעים של Dynamics 365 Finance ו- Dynamics 365 Project Service Automation באמצעות Common Data Service. תבניות השילוב שזמינות עם תכונת שילוב הנתונים מאפשרות זרימה של פרויקטים, חוזי פרויקט, סעיפי חוזה של פרויקט, אבני דרך בסעיפי חוזה של פרויקט, משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות מ- Project Service Automation ל- Finance.

> [!NOTE]
> - אם אתה משתמש בגירסה 7.3.0, עליך להתקין את KB 4074835. לאחר מכן תוכל לשלב פרויקטים במחיר קבוע.
> - אם אתה משתמש בגירסה 7.3.0 ואתה מעביר עסקאות עמלה מ- Project Service Automation, עליך להתקין את KB 4345320 כדי לכלול את העמלות בחשבונית הפרויקט.
> - אם אתה משתמש בגירסה 8.0, תוכל להשתמש בשילוב משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונעילת פונקציונליות.
> - אם אתה משתמש בגרסה 8.0.1 ואילך, תוכל לסנכרן את הנתונים בפועל.

לפני שתוכל לשלב את Project Service Automation Finance, עליך להגדיר את פרמטרי השילוב של Project Service Automation. לקבלת מידע נוסף, ראה [פרמטרי שילוב של Project Service Automation](PSA-parameters.md).

פתרון שילוב זה מאפשר סנכרון ישיר בתרחישים הבאים:

- אחזקת חוזי פרויקט ב- Project Service Automation וסנכרון שלהם ישירות מ- Project Service Automation ל- Finance.
- יצירת פרויקטים ב- Project Service Automation וסנכרון שלהם ישירות מ- Project Service Automation ל- Finance.
- אחזקת סעיפי חוזים בפרויקט ב- Project Service Automation וסנכרון שלהם ישירות מ- Project Service Automation ל- Finance.
- אחזקת אבני דרך בסעיפי חוזים בפרויקט ב- Project Service Automation וסנכרון שלהם ישירות מ- Project Service Automation ל- Finance.
- אחזקת משימות פרויקט ב- Project Service Automation וסנכרון שלהן ישירות מ- Project Service Automation ל- Finance.
- אחזקת קטגוריות של עסקאות הוצאות ב- Finance וסנכרון שלהן ישירות מ- Finance ל- Project Service Automation.
- יצירת הערכות של שעות בפרויקטים ב- Project Service Automation וסנכרון שלהם ישירות מ- Project Service Automation ל- Finance.
- יצירת הערכות של הוצאות בפרוייקטים ב- Project Service Automation וסנכרון שלהם ישירות מ- Project Service Automation ל- Finance.
- יצירת שעות בפרויקט, הוצאות ונתונים בפועל של עמלות ב- Project Service Automation, ויצירת עסקאות פרויקט ביומן שילוב של Project Service Automation כך שניתן יהיה לרשום אותם ב- Finance.

## <a name="data-synchronization"></a>‏‏סינכרון נתונים

האיור הבא מראה כיצד נתונים מסונכרנים כחלק מהשילוב בין Project Service Automation ו- Finance.

> [!NOTE]
> לא כל התבניות זמינות כרגע. התבניות ישוחררו עם השלמתן.

[![שילוב Project Service Automation עם Finance.](./media/PSA-integration.png)](./media/PSA-integration.png)

## <a name="system-requirements-for-finance"></a>דרישות מערכת עבור Finance

כדי להשתמש בפתרון השילוב של Project Service Automation ל- Finance, עליך להתקין את Enterprise edition 7.3 עם עדכון 12 ואילך של הפלטפורמה.

## <a name="system-requirements-for-project-service-automation"></a>דרישות מערכת עבור Project Service Automation

כדי להשתמש בפתרון השילוב Project Service Automation ל- Finance, עליך להתקין את הרכיבים הבאים:

- Dynamics 365 Project Service Automation גירסה 9.0.0.0 ואילך
- פתרון Prospect to Cash עבור Dynamics 365 Sales, גירסה 1.14.0.0 (v14) ואילך
- פתרון Project Service Automation ל- Finance solution עבור Dynamics 365 Project Service Automation גירסה 1.0.0.0 ואילך

## <a name="install-the-project-service-automation-to-finance-integration-solution-in-your-project-service-automation-instance"></a>התקן את פתרון השילוב Project Service Automation ל- Finance במופע Project Service Automation

הןרד את פתרון השילוב Project Service Automation ל- Finance מ[מרכז ההורדות של Microsoft](https://www.microsoft.com/download/details.aspx?id=57016), ופעל לפי ההנחיות הכלולות בפתרון.


[!INCLUDE[footer-include](../includes/footer-banner.md)]