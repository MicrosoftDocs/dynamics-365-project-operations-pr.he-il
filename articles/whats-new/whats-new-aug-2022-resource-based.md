---
title: מה חדש באוגוסט 2022 - Project Operations לתרחישים של משאבים/ללא-מלאי
description: מאמר זה מספק מידע אודות עדכוני האיכות הזמינים במהדורת אוגוסט 2022 של Microsoft Dynamics 365 Project Operations עבור תרחישים מבוססי-משאב/לא במלאי.
author: ramagadu
ms.date: 07/19/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: 112dbb98de09ef342c03d122a29cb8025058e47f
ms.sourcegitcommit: 6b6c2bfd04e3e613ed1f38355c7cd47c3a56748d
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/24/2022
ms.locfileid: "9348011"
---
# <a name="whats-new-august-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>מה חדש באוגוסט 2022 - Project Operations לתרחישים של משאבים/ללא-מלאי

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

מאמר זה חל על הרכיבים והגירסאות הבאים של Microsoft Dynamics 365 Project Operations:

- Project Operations בגירסת סביבת Dataverse 4.45.0.53
- ניהול פרויקטים וחשבונאות בסביבת Dynamics 365 Finance גירסה 10.0.28

## <a name="project-operations-dual-write-maps-updates"></a>עדכוני מפות כתיבה כפולה של Project Operations

במהדורה זו אין עדכונים עבור מפות כתיבה כפולה של Project Operations. לקבלת רשימה עדכנית וגרסאות של מפות כתיבה כפולה של Project Operations, ראה [גירסאות של מפות כתיבה כפולה ב- Project Operations](../environment/resource-dual-write-maps.md).

הפעל תמיד את הגרסה האחרונה של המפה בסביבה שלך, והפעל את כל מפות הטבלות הקשורות תוך כדי עדכון הפתרון שלך ב- Dataverse Project Operations גרסת Finance. ייתכן שחלק מהתכונות והיכולות לא יפעלו כהלכה אם הגרסה האחרונה של המפה לא מופעלת. אפשר לראות את הגרסה הפעילה של המפה בעמודה **גרסה** בדף **כתיבה כפולה**. כדי להפעיל גירסה חדשה של המפה, בחר באפשרות **גירסאות של מפת טבלאות**, בחר בגירסה העדכנית ביותר ושמור את הגירסה שנבחרה. אם התאמת אישית מפת טבלה שכלולה במוצר, החל מחדש את השינויים. מידע נוסף ראה [ניהול מחזור החיים של פתרונות](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

אם אתה נתקל בבעיה בזמן הפעלת המפה, בצע את ההוראות בסעיף [בעיה של עמודות טבלה חסרות במפות](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) במדריך לפתרון בעיות של כתיבה כפולה.

## <a name="quality-updates"></a>עדכוני איכות

### <a name="project-operations-on-dataverse"></a>Project Operations ב- Dataverse

| אזור תכונות | מספר אסמכתא | עדכון איכות |
| --- | --- | --- |
|   ניהול הזדמנויות | 2762089 | טיפול בשגיאות במהלך סגירת החוזה יאבד אם השמירה האוטומטית מושבתת בארגון.|

### <a name="project-management-and-accounting-in-finance"></a>ניהול וחשבונאות של פרוייקטים ב- Finance

למידע על תיקוני הבאגים הכלולים בעדכון זה, היכנס אל Microsoft Dynamics Lifecycle Services‏ (LCS), והצג את [מאמר KB ](https://fix.lcs.dynamics.com/Issue/Details?bugId=694438).
