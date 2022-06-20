---
title: מה חדש במאי 2022 - Project Operations לתרחישים מבוססי משאבים/ללא מלאי
description: מאמר זה מספק מידע אודות עדכוני האיכות הזמינים במהדורת מאי 2022 של Microsoft Dynamics 365 Project Operations עבור תרחישים מבוססי-משאב/לא במלאי.
author: sigitac
ms.date: 05/02/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: beb75fc4b721d52cddbdaf2d20194218cefced5e
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8921395"
---
# <a name="whats-new-may-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>מה חדש במאי 2022 - Project Operations לתרחישים מבוססי משאבים/ללא מלאי

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

מאמר זה חל על הרכיבים והגירסאות הבאים של Microsoft Dynamics 365 Project Operations:

- Project Operations בגירסת סביבת Dataverse 4.42.0.70
- ניהול פרויקטים וחשבונאות בסביבת Dynamics 365 Finance גירסה 10.0.26

## <a name="project-operations-dual-write-maps-updates"></a>עדכוני מפות כתיבה כפולה של Project Operations

במהדורה זו אין עדכונים עבור מפות כתיבה כפולה של Project Operations. לקבלת רשימה עדכנית וגרסאות של מפות כתיבה כפולה של Project Operations, ראה [גירסאות של מפות כתיבה כפולה ב- Project Operations](../environment/resource-dual-write-maps.md).

הפעל תמיד את הגרסה האחרונה של המפה בסביבה שלך, והפעל את כל מפות הטבלות הקשורות תוך כדי עדכון הפתרון שלך ב- Dataverse Project Operations גרסת Finance. ייתכן שחלק מהתכונות והיכולות לא יפעלו כהלכה אם הגרסה האחרונה של המפה לא מופעלת. אפשר לראות את הגרסה הפעילה של המפה בעמודה **גרסה** בדף **כתיבה כפולה**. כדי להפעיל גירסה חדשה של המפה, בחר באפשרות **גירסאות של מפת טבלאות**, בחר בגירסה העדכנית ביותר ושמור את הגירסה שנבחרה. אם התאמת אישית מפת טבלה שכלולה במוצר, החל מחדש את השינויים. מידע נוסף ראה [ניהול מחזור החיים של פתרונות](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

אם אתה נתקל בבעיה בזמן הפעלת המפה, בצע את ההוראות בסעיף [בעיה של עמודות טבלה חסרות במפות](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) במדריך לפתרון בעיות של כתיבה כפולה.

## <a name="quality-updates"></a>עדכוני איכות
### <a name="project-operations-on-dataverse"></a>Project Operations ב- Dataverse

| אזור תכונות | מספר אסמכתא | עדכון איכות |
| --- | --- | --- |
| ניהול משאבים | 2634019 | הודעות שגיאה משופרות עבור אימותים עסקיים בעת הוספת חברי צוות כלליים כמשאבים. |
| ‏‫תכנון פרויקטים ומעקב אחריהם | 2648515 | עדכונים מוגבלים של **ownerid**, **מצב** ו **סטטוס** בישויות תזמון. |
| חיוב ותמחור | 2653167 | המפריד העשרוני של רשת **הערכות** חייב לעקוב אחר הגדרות התבנית ב **אפשרויות אישיות**. |
| חיוב ותמחור| 2662251 | הערכים בשדות **יחידה מתוקנת** ו **קבוצת יחידות** חוזרות לברירת המחדל בעת יצירת רשומות בהערכות של חומרים. |
| חיוב ותמחור| 2571408 | נתוני בפועל של מכירות שלא חויבו מוטבעות במזהה חשבונית פרופורמה בעת יצירה של טיוטת חשבונית. |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>ניהול וחשבונאות של פרוייקטים ב- Dynamics 365 Finance

למידע על תיקוני הבאגים הכלולים בעדכון זה, היכנס אל Microsoft Dynamics Lifecycle Services‏ (LCS), והצג את [מאמר KB ](https://fix.lcs.dynamics.com/Issue/Details?bugId=662864).
