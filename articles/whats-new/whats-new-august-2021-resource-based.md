---
title: מה חדש באוגוסט 2021 - Project Operations לתרחישים של משאבים/ללא-מלאי
description: נושא זה מספק מידע על עדכוני האיכות הזמינים במהדורת אוגוסט 2021 של Project Operations עבור תרחישים של משאבים/ללא מלאי.
author: sigitac
ms.date: 08/11/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: cd5a7e74fc90c6138cd672ff6109b59a8d2ae916
ms.sourcegitcommit: 80aa1e8070f0cb4992ac408fc05bdffe47cee931
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "7323462"
---
# <a name="whats-new-august-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>מה חדש באוגוסט 2021 - Project Operations לתרחישים של משאבים/ללא-מלאי

*חל על: ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי*

נושא זה חל על הרכיבים והגירסאות הבאים של Dynamics 365 Project Operations:

   - Project Operations בגירסה של סביבת Microsoft Dataverse 4.13.0.152.
   - ניהול פרויקטים וחשבונאות בסביבת Dynamics 365 Finance גרסה 10.0.20.

## <a name="features-included-in-this-release"></a>התכונות הזמינות בגירסה זו

התכונות הבאות כלולות בהפצה זו:

- **קבוצות אישורים**: קבוצות אישורים מקבצות בקשות לאישור זמן, הוצאות או שימוש בחומרים לערכות משנה קטנות יותר של פעולות. קיבוץ זה מאפשר לעבד אישורים בסדר ספציפי לפי פרוייקט ומאפשר ניסיון מחדש ויצירת רצף. קיבוץ הבקשות משפר את האמינות ויכולת המעקב של עיבוד אישורים עבור כמויות גדולות של אישורים. למידע נוסף, ראה [קבוצות אישורים](../approvals/approval-sets.md).

## <a name="project-operations-dual-write-maps-updates"></a>עדכוני מפות כתיבה כפולה של Project Operations

במהדורה זו אין עדכונים עבור מפות כתיבה כפולה של Project Operations. 

לקבלת רשימה עדכנית וגרסאות של מפות כתיבה כפולה של Project Operations, ראה [גירסאות של מפות כתיבה כפולה ב- Project Operations](../environment/resource-dual-write-maps.md).

הפעל תמיד את הגרסה האחרונה של המפה בסביבה שלך והפעל את כל מפות הטבלות הקשורות תוך כדי עדכון הפתרון שלך ב- Dataverse Project Operations גרסת Finance. ייתכן שתכונות ויכולות מסוימות לא יפעלו כראוי אם הגירסה האחרונה של המפה אינה מופעלת. אתה יכול לראות את הגירסה הפעילה של המפה בדף **כתיבה כפולה** בעמודה **גירסה**. הפעל גירסה חדשה של המפה על ידי בחירה באפשרות **גירסאות של מפת טבלה**, תוך בחירה בגירסה האחרונה ולאחר מכן שמור את הגירסה שנבחרה. אם התאמת אישית מפת טבלה שהגיעה מוכנה לשימוש עם המוצר, יהיה עליך להחיל מחדש את השינויים. מידע נוסף ראה [ניהול מחזור החיים של פתרונות](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

אם אתה נתקל בבעיה בהתחלת המפה, עקוב אחר ההוראות המופיעות במקטע [בעיה שחסרות עמודות טבלה במפות](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) במדריך לפתרון בעיות כתיבה כפולה.

## <a name="quality-updates"></a>עדכוני איכות

### <a name="project-operations-on-dataverse"></a>Project Operations ב- Dataverse

| **אזור תכונות** | **מספר אסמכתא** | **עדכון איכות** |
| --- | --- | --- |
| חיוב ותמחור | 2295625 | יש להעתיק את שם אבן הדרך מלוח הזמנים לחשבוניות לפרט שורת החשבונית. |
| חיוב ותמחור | 2316323 | לא ניתן לערוך את ההנחה בחשבונית פרופורמה ב- Project Operations עבור תרחישים מבוססי-משאב: |
|   ניהול הזדמנויות | 2338619 | יש להפעיל את הכללים העסקיים **הזדמנות** ו **הצעת מחיר** רק בדפים. |
| ניהול משאבים | 2316523 | שימוש באפשרות **שלח בקשה** מדרישת משאב שמצורף אליה תפקיד לא אמור להציג שגיאה. |
| ניהול משאבים | 2326885 | יצירת דרישת משאב באמצעות פרוייקט לא אמורה להציג שגיאה. |
| זמן והוצאה | 2335584 | זרימות משימה שהוצאו משימוש בערך הזמן. |
| זמן והוצאה | 2336884 | לחצן ערך הזמן **העתק שבוע** מוכרח לפעול עבור יותר מהמשתמש הנוכחי. |


### <a name="project-management-and-accounting-on-dynamics-365-finance"></a>ניהול פרויקטים וחשבונאות ב- Dynamics 365 Finance

| אזור תכונות | מספר אסמכתא | עדכון איכות |
| --- | --- | --- |
| נסיעות והוצאה | [4618082](https://fix.lcs.dynamics.com/Issue/Details?kb=4618082&amp;bugId=583101&amp;dbType=3&amp;qc=9c85ac8ca1e5e9cd07fac9e9aa2cb0914724e28b86ad3339dacf7741f554c605) | סכומי עסקת ספק ועסקת מס מכירות שגויים מתפרסמים כאשר נוצרת הוצאה מעסקת כרטיס אשראי. |
| נסיעות והוצאה | [4620366](https://fix.lcs.dynamics.com/Issue/Details?kb=4620366&amp;bugId=579485&amp;dbType=3&amp;qc=e864789bd95505ea624c537d585bf113c2de60b97c88439d44693dbd85aa8e92) | ההסדר הלא נכון הוא שורות שנוצרו בעת יצירת יומן התשלומים. |
| נסיעות והוצאה | [4618082](https://fix.lcs.dynamics.com/Issue/Details?kb=4618082&amp;bugId=583101&amp;dbType=3&amp;qc=9c85ac8ca1e5e9cd07fac9e9aa2cb0914724e28b86ad3339dacf7741f554c605) | סכומי עסקת מס מכירות שגויים מתפרסמים כאשר נוצרת הוצאה מעסקת כרטיס אשראי. |
| נסיעות והוצאה | [4621765](https://fix.lcs.dynamics.com/Issue/Details?kb=4621765&amp;bugId=587306&amp;dbType=3&amp;qc=6fbfad0123d4e95eaf8d5a5a2f6c354577c991b7905c852ab02d1f94e728a876) | מחיקת שורת הוצאות עשויה להימשך זמן רב. |
| חשבונאות פרויקט | [4623737](https://fix.lcs.dynamics.com/Issue/Details?kb=4623737&amp;bugId=598109&amp;dbType=3&amp;qc=4101fc5865201e21815299f2ff11ae46d5d5370510868df86c25ee09a8ca1a0c) | המערכת אינה תומכת בהגדרת רצף מספרים כאשר אתה מפרסם אומדן לאחר החלת KB 4619395. |
| חשבונאות פרויקט | [4623332](https://fix.lcs.dynamics.com/Issue/Details?kb=4623332&amp;bugId=586034&amp;dbType=3&amp;qc=2f64bb1977c4a9c9dd2ce9de7e72230b86eca14b6295c5bbfb614ea97ad81caf) | פרסום חשבונית ספק עשוי להיכשל עם הודעת השגיאה, "העסקאות בשובר אינן מתאזנות לפי 17/5/2021. (מטבע חשבונאות: 0.00 - מטבע דיווח: 0.01) " |
