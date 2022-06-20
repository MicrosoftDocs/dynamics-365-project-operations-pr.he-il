---
title: מה חדש בספטמבר 2021 - Project Operations לתרחישים מבוססי משאב/לא במלאי
description: מאמר זה מספק מידע אודות עדכוני האיכות הזמינים במהדורת ספטמבר 2021 של Project Operations עבור תרחישים מבוססי-משאב/ללא במלאי.
author: sigitac
ms.date: 09/12/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: c7f764b3e8ee3775167ee57b4f034e383899aea3
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8923373"
---
# <a name="whats-new-september-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>מה חדש בספטמבר 2021 - Project Operations לתרחישים מבוססי משאב/לא במלאי

*חל על: ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי*

מאמר זה חל על הרכיבים והגירסאות הבאים של Dynamics 365 Project Operations:

   - Project Operations בגירסה של סביבת Microsoft Dataverse 4.14.0.99.
   - ניהול פרויקטים וחשבונאות בסביבת Dynamics 365 Finance גירסה 10.0.20.

## <a name="project-operations-dual-write-maps-updates"></a>עדכוני מפות כתיבה כפולה של Project Operations

במהדורה זו אין עדכונים עבור מפות כתיבה כפולה של Project Operations. לקבלת רשימה עדכנית וגרסאות של מפות כתיבה כפולה של Project Operations, ראה [גירסאות של מפות כתיבה כפולה ב- Project Operations](../environment/resource-dual-write-maps.md).

הפעל תמיד את הגרסה האחרונה של המפה בסביבה שלך והפעל את כל מפות הטבלות הקשורות תוך כדי עדכון הפתרון שלך ב- Dataverse Project Operations גרסת Finance. ייתכן שתכונות ויכולות מסוימות לא יפעלו כראוי אם הגירסה האחרונה של המפה אינה מופעלת. אתה יכול לראות את הגירסה הפעילה של המפה בדף **כתיבה כפולה** בעמודה **גירסה**. כדי להפעיל גירסה חדשה של המפה, בחר באפשרות  **גירסאות של מפת טבלאות**, בחר בגירסה העדכנית ביותר ושמור את הגירסה שנבחרה. אם התאמת אישית מפת טבלה שהגיעה מוכנה לשימוש עם המוצר, יהיה עליך להחיל מחדש את השינויים. מידע נוסף ראה [ניהול מחזור החיים של פתרונות](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

אם אתה נתקל בבעיה בהפעלת המפה, בצע את ההוראות בסעיף [בעיה של עמודות טבלה חסרות במפות](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) במדריך לפתרון בעיות של כתיבה כפולה.

## <a name="quality-updates"></a>עדכוני איכות

### <a name="project-operations-on-dataverse"></a>Project Operations ב- Dataverse

| **אזור תכונות** | **מספר אסמכתא** | **עדכון איכות** |
| --- | --- | --- |
| זמן והוצאה | 1811407 | תפקיד האבטחה 'מאשר פרוייקט' הותאם עבור אישורי ערך הוצאה. |
| זמן והוצאה | 1811438 | תפקיד האבטחה 'מאשר פרוייקט' הותאם עבור ביטול אישור של ערך זמן. |
| זמן והוצאה | 2370126 | הסמלים **משימת פרוייקט** ו **תפקיד** עודכנו בישות **ערך זמן**. |
| זמן והוצאה | 2379879 | הפונקציה **העתק שבוע** בערך הזמן תוקנה בעת שימוש ב- Dynamics 365 עבור טלפון. |
| חיוב ותמחור | 2371906 | הסכום הכולל של חשבונית הפרופורמה לא יכול להיות סכום מתכוונן ב- Project Operations עבור פריסות מבוססות-משאבים. |
| חיוב ותמחור | 2385802 | תוקנה השגיאה המתרחשת עם שעות בפועל שליליות כאשר מתבצע רענון של סכומי הפרוייקט. |
| חיוב ותמחור | 2389675 | אופן הפעולה של אישור חשבונית פרופורמה שופר. ישות משימות הפועלות זמן רב מוכרחה לקחת בחשבון את הפעילות הנדרשת לכתיבת תוצאות אישור עבור חשבונאות. |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>ניהול וחשבונאות של פרוייקטים ב- Dynamics 365 Finance

| אזור תכונות | מספר אסמכתא | עדכון איכות |
| --- | --- | --- |
| נסיעות והוצאה | [4618082](https://fix.lcs.dynamics.com/Issue/Details?kb=4618082&amp;bugId=583101&amp;dbType=3&amp;qc=9c85ac8ca1e5e9cd07fac9e9aa2cb0914724e28b86ad3339dacf7741f554c605) | הסכומים בעסקאות ספק ומס מכירות שפורסמו מהוצאה שנוצרה מעסקת כרטיס אשראי שגויים. |
| נסיעות והוצאה | [4620366](https://fix.lcs.dynamics.com/Issue/Details?kb=4620366&amp;bugId=579485&amp;dbType=3&amp;qc=e864789bd95505ea624c537d585bf113c2de60b97c88439d44693dbd85aa8e92) | שורות יישוב התביעות השגויות נוצרות כאשר יומן התשלומים נוצר. |
| נסיעות והוצאה | [4618082](https://fix.lcs.dynamics.com/Issue/Details?kb=4618082&amp;bugId=583101&amp;dbType=3&amp;qc=9c85ac8ca1e5e9cd07fac9e9aa2cb0914724e28b86ad3339dacf7741f554c605) | הסכומים בעסקאות מס מכירות שפורסמו מהוצאה שנוצרה מעסקת כרטיס אשראי שגויים. |
| נסיעות והוצאה | [4621765](https://fix.lcs.dynamics.com/Issue/Details?kb=4621765&amp;bugId=587306&amp;dbType=3&amp;qc=6fbfad0123d4e95eaf8d5a5a2f6c354577c991b7905c852ab02d1f94e728a876) | מחיקת שורת הוצאות עשויה להימשך זמן רב. |
| חשבונאות פרויקט | [4623737](https://fix.lcs.dynamics.com/Issue/Details?kb=4623737&amp;bugId=598109&amp;dbType=3&amp;qc=4101fc5865201e21815299f2ff11ae46d5d5370510868df86c25ee09a8ca1a0c) | לאחר החלת KB 4619395, שינוי רצף המספרים לערך **רציף** אינו נתמך וכאשר אתה מפרסם אומדן, מתרחשת השגיאה הבאה, "המערכת אינה תומכת בהגדרת 'רציף' של רצף המספרים Proj_X." |
| חשבונאות פרויקט | [4623332](https://fix.lcs.dynamics.com/Issue/Details?kb=4623332&amp;bugId=586034&amp;dbType=3&amp;qc=2f64bb1977c4a9c9dd2ce9de7e72230b86eca14b6295c5bbfb614ea97ad81caf) | פרסום חשבונית ספק עלול להיכשל עם הודעת השגיאה הבאה, "העסקאות בשובר אינן מתאזנות לפי 17/5/2021. (מטבע חשבונאות: 0.00 - מטבע דיווח: 0.01)." |
