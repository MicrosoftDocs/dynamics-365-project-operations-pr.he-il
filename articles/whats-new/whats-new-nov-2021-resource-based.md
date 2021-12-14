---
title: מה חדש נובמבר 2021 - Project Operations לתרחישים מבוססי משאבים/ללא מלאי
description: נושא זה מספק מידע אודות עדכוני האיכות הזמינים במהדורת נובמבר 2021 של Project Operations עבור תרחישים מבוססי-משאב/לא במלאי.
author: sigitac
ms.date: 11/09/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 20f277bc9b6f571c0144eaaa867bb97c0cf30ddb
ms.sourcegitcommit: 04ebe764afa22742b3fbf8f12af31e8eea93682e
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 11/23/2021
ms.locfileid: "7827327"
---
# <a name="whats-new-november-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>מה חדש נובמבר 2021 - Project Operations לתרחישים מבוססי משאבים/ללא מלאי

*חל על: ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי*

נושא זה חל על הרכיבים והגירסאות הבאים של Microsoft Dynamics 365 Project Operations:

- Project Operations בגרסה של סביבת Dataverse 4.26.0.145‏, 4.26.0.148 או 4.26.0.150
- ניהול פרויקטים וחשבונאות בסביבת Dynamics 365 Finance גירסה 10.0.22

## <a name="features-included-in-this-release"></a>התכונות הזמינות בגירסה זו

התכונות הבאות כלולות בהפצה זו:

- ממשקי תיכנות יישומים לתזמון פרויקטים (API) תומכים כעת ביכולת ליצור ולמחוק מיכלים של פרויקטים.

## <a name="project-operations-dual-write-maps-updates"></a>עדכוני מפות כתיבה כפולה של Project Operations

במהדורה זו אין עדכונים עבור מפות כתיבה כפולה של Project Operations. לקבלת רשימה עדכנית וגרסאות של מפות כתיבה כפולה של Project Operations, ראה [גירסאות של מפות כתיבה כפולה ב- Project Operations](/dynamics365/project-operations/environment/resource-dual-write-maps).

הפעל תמיד את הגרסה האחרונה של המפה בסביבה שלך, והפעל את כל מפות הטבלות הקשורות תוך כדי עדכון הפתרון שלך ב- Dataverse Project Operations גרסת Finance. ייתכן שחלק מהתכונות והיכולות לא יפעלו כהלכה אם הגרסה האחרונה של המפה לא מופעלת. אפשר לראות את הגרסה הפעילה של המפה בעמודה **גרסה** בדף **כתיבה כפולה**. כדי להפעיל גירסה חדשה של המפה, בחר באפשרות **גירסאות של מפת טבלאות**, בחר בגירסה העדכנית ביותר ושמור את הגירסה שנבחרה. אם התאמת אישית מפת טבלה שכלולה במוצר, החל מחדש את השינויים. מידע נוסף ראה [ניהול מחזור החיים של פתרונות](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

אם אתה נתקל בבעיה בזמן הפעלת המפה, בצע את ההוראות בסעיף [בעיה של עמודות טבלה חסרות במפות](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) במדריך לפתרון בעיות של כתיבה כפולה.

## <a name="quality-updates"></a>עדכוני איכות

### <a name="project-operations-in-dataverse"></a>Project Operations ב- Dataverse

| אזור תכונות | מספר אסמכתא | עדכון איכות |
| --- | --- | --- |
| חיוב ותמחור | 2240080 | אין לשכפל את השדה **תנאי תשלום** בחשבונית הפרופורמה. |
| חיוב ותמחור | 2358236 | תיקון חשבונית חייב לאפשר תיקונים עם שורות במחיר אפס. |
| ניהול משאבים | 2410072 | מאפשר הגדרה של משאב‬ שהוקצה למשימה בתור מנהל פרוייקט. |
| חיוב ותמחור | 2430234 | תקן בעיית חישוב ביצועי עלות. |
| זמן והוצאה | 2436978 | אפשר להזין זמן בפורמט hh:mm. |
| חיוב ותמחור | 2448623 | אפשר לעדכן מחירונים לאחר שיוך ליחידה ארגונית. |
| זמן והוצאה | 2460396 | אפשר למחוק ערך זמן על ידי ניקוי התא. |
| חיוב ותמחור | 2467386 | אפשר למחוק פרויקט שיש לו משימה, גם כאשר המשימה משויכת להצעת מחיר שהושגה. |
| זמן והוצאה | 2461744 | התצוגה **‏‫האישורים שלי שנכשלו‬** מכילה רק אישורי פרויקטים בשלב **נשלח**. |
| זמן והוצאה | 2464082 | הסר את הקישור מאישורי הפרוייקט לסט האישורים כאשר מצב היעד מותאם. |
| זמן והוצאה | 2468108 | משימת לוח הזמנים לא אמורה להגדיר מצב **מעבד** עבור ערכת האישורים. |
| זמן והוצאה | 2471503 | מחק ערכות אישורים בנות שבעה ימים. |
| חיוב ותמחור | 2480687 | אין להסיר את ההפניה לשורת הצעת מחיר כאשר נוצרת אבן דרך של שורת הצעת מחיר. |

### <a name="project-management-and-accounting-in-finance"></a>ניהול וחשבונאות של פרוייקטים ב- Finance

| אזור תכונות | מספר אסמכתא | עדכון איכות |
| --- | --- | --- |
| ניהול פרוייקטים וחשבונאות | [584732](https://fix.lcs.dynamics.com/Issue/Details/?bugId=584732) | סכומים של ספקים שנשמרו בעסקאות הוצאות בפרוייקט אינם מוצגים ברשימת העסקאות. |
| ניהול פרוייקטים וחשבונאות | [593068](https://fix.lcs.dynamics.com/Issue/Details/?bugId=593068) | חשבונית הספק הבין-ארגונית מנותקת כאשר שילוב חשבונית הספק מופעל. |
| ניהול פרוייקטים וחשבונאות | [593382](https://fix.lcs.dynamics.com/Issue/Details/?bugId=593382) | תנאי התשלום בחשבוניות הפרויקט אינם פועלים כצפוי. |
| ניהול פרוייקטים וחשבונאות | [596263](https://fix.lcs.dynamics.com/Issue/Details/?bugId=596263) | כאשר שמירת הספק משתחררת, לרישום השובר יש שורות נוספות שאינן נכונות. |
| ניהול פרוייקטים וחשבונאות | [598758](https://fix.lcs.dynamics.com/Issue/Details/?bugId=598758) | כאשר יומן השילוב של Project Operations מתפרסם, הוא נכשל בגלל מאפיינים חסרים עבור תיק לקוח שלא נרשם אליו. |
| ניהול פרוייקטים וחשבונאות | [602650](https://fix.lcs.dynamics.com/Issue/Details/?bugId=602650) | הכרטיסיה **פּרוייקט** אינה ניתנת לעריכה בחשבונית ספק ממתינה כאשר קטגוריית הרכש מוקצית לפריט. |
| ניהול פרוייקטים וחשבונאות | [605121](https://fix.lcs.dynamics.com/Issue/Details/?bugId=605121) | חלונית הניווט חסרה אם אינך מחובר ל- Project Operations Dataverse. |
| ניהול פרוייקטים וחשבונאות | [602728](https://fix.lcs.dynamics.com/Issue/Details/?bugId=602728) | כאשר אתה רושם הכנסה מחשבונית פרויקט במקרה של שמירה שהוחלה, יש בעיה מכיוון שהעסקאות בשובר אינן מתאזנות. |
| ניהול פרוייקטים וחשבונאות | [603624](https://fix.lcs.dynamics.com/Issue/Details/?bugId=603624) | יצירת אומדן לאחר פרסום הצעת חשבונית חוסמת שורות תיקון מיבוא. |
| ניהול פרוייקטים וחשבונאות | [606083](https://fix.lcs.dynamics.com/Issue/Details/?bugId=606083) | שינוי של רשומת אבן דרך עם חשבונית מלאה לא אמור להיות אפשרי. |
| נסיעות והוצאה | [575305](https://fix.lcs.dynamics.com/Issue/Details/?bugId=575305) | כל דוחות ההוצאות גלויים כאשר אתה מחפש קטגוריה באפליקציה למכשירים ניידים של Expense. |
| נסיעות והוצאה | [583101](https://fix.lcs.dynamics.com/Issue/Details/?bugId=583101) | סכומים שגויים בעסקאות ספק ומס מכירות מפורסמים מהוצאה שנוצרה מעסקת כרטיס אשראי. |
| נסיעות והוצאה | [583760](https://fix.lcs.dynamics.com/Issue/Details/?bugId=583760) | אזהרה לא רלוונטית מופיעה כאשר אתה מרענן את הדף **דוח הוצאות**. |
| נסיעות והוצאה | [598656](https://fix.lcs.dynamics.com/Issue/Details/?bugId=598656) | נעשה שימוש במאשר ביניים שגוי כאשר אתה מוחק מאשר ביניים ולאחר מכן שולח מחדש דוח הוצאות דרך זרימת העבודה. |
| נסיעות והוצאה | [612742](https://fix.lcs.dynamics.com/Issue/Details/?bugId=612742) | מתרחשת שגיאת פרסום הקשורה להגדרת קילומטראז'. |