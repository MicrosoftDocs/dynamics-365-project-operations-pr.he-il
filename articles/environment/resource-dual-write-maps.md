---
title: גרסאות מפה של כתיבה כפולה ב-Project Operations
description: נושא זה מספק את רשימת המפות הכתיבה הכפולה הנדרשת עבור Dynamics 365 Project Operations.
author: sigitac
manager: Annbe
ms.date: 04/22/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: fa0342985f2c860cd3cb3f686f0dcaa59d8cfd41
ms.sourcegitcommit: bc51629df94c164325cf2afee387d0e7cda66da7
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2021
ms.locfileid: "5938989"
---
# <a name="project-operations-dual-write-map-versions"></a>גרסאות מפה של כתיבה כפולה ב-Project Operations

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

לשימוש ב- Dynamics 365 Project Operations עבור תרחישים מבוססי משאבים/ללא מלאי, נדרשת קבוצה של מפות כתיבה כפולה שפועלים בסביבה. 

## <a name="prerequisite-maps-dual-write-orchestration-solution"></a>מפות דרושות מראש: פתרון התיאום של הכתיבה הכפולה

המפות הבאות נדרשות מראש לפתרון Project Operations. הקפד להפעיל את המפות המפורטות בטבלה הבאה ואת כל מפת טבלה קשורה בסביבתך.

| מפת טבלאות | סינכרון ראשוני |
| --- | --- |
| ספר (msdyn_ledgers) | דרוש סנכרון ראשוני עבור מפת הטבלה והדרישות המוקדמות. פריט ראשי לסינכרון ראשוני הוא יישומי Finance and Operations. |
| ישויות משפטיות (cdm_companies) | לא נדרש. המערכת מאכלסת ישות זו באופן אוטומטי כאשר מקושרים סביבות באמצעות כתיבה כפולה. |
| לקוחות גרסה 3 (תיקי לקוח) | לא נדרש להקצאה. |
| ספקים גרסה 2 (msdyn_vendors) | לא נדרש להקצאה. |

1. מרשימת המפות, בחר את המפה 'ספר חשבונות' **(‏‎‏‏msdyn‏‏\_ledgers)** עם כל הדרישות המוקדמות ובחר את תיבת הסימון **סנכרון ראשוני**. בשדה **פריט ראשי לסנכרון ראשוני**, בחר **ביישומי Finance and Operations** הן עבור מפת ספר החשבונות הראשי והן עבור כל המפות שנדרשות מראש. בחר **הפעל**.

![סנכרון מפת ספר חשבונאות](media/DW6.png)

1. בצע את אותם השלבים עבור כל מפות הטבלה שנותרו, המפורטות בטבלה לעיל. אל תבחר את תיבת הסימון **סנכרון ראשוני** בעת הפעלת מפות אלה.

## <a name="project-operations-dual-write-maps"></a>מפות כתיבה כפולה של Project Operations

המפות הבאות נדרשות מראש לפתרון Project Operations.

| **מפת ישות** | **הגירסה האחרונה** | **סינכרון ראשוני** |
| --- | --- | --- |
| ‏‫ישות שילוב לקשרי עסקת פרויקט‬ (msdyn\_transactionconnections) | 1.0.0.0 | לא נדרש להקצאה. |
| כותרות על חוזי פרויקט (הזמנות מכירה) | 1.0.0.1 | לא נדרש להקצאה. |
| סעיפי חוזה של פרויקט (salesorderdetails) | 1.0.0.0 | לא נדרש להקצאה. |
| מקור מימון הפרויקט (msdyn_projectcontractsplitbillingrules) | 1.0.0.1 | לא נדרש להקצאה. |
| טבלת שילוב Project Operations להערכת הוצאות (msdyn\_estimateslines) | 1.0.0.0 | לא נדרש להקצאה. |
| הצעות לחשבוניות פרוייקט גרסה 2 (חשבוניות) | 1.0.0.2 | לא נדרש להקצאה. |
| נתוני שילוב בפועל של Project Operations ‏(msdyn_actuals) | 1.0.0.14 | לא נדרש להקצאה. |
| אבני דרך של סעיף חוזה לשילוב Project Operations‏ (msdyn_contractlinesscheduleofvalues) | 1.0.0.4 | לא נדרש להקצאה. |
| ישות שילוב של Project Operations להערכת הוצאות (msdyn_estimateslines) | 1.0.0.2 | לא נדרש להקצאה. |
| ישות שילוב של Project Operations להערכת שעות (msdyn_resourceassignments) | 1.0.0.5 | לא נדרש להקצאה. |
| ישות ייצוא של Project Operations לשילוב קטגוריות של הוצאות פרויקט (msdyn_expensecategories) | 1.0.0.2 | לא נדרש להקצאה. |
| ישות ייצוא של שילוב הוצאות פרויקט של Project Operations ‏(msdyn_expenses) | 1.0.0.2 | לא נדרש להקצאה. |
| ישות יצוא חשבוניות ספק של פרויקט שילוב של Project Operations (msdyn_projectvendorinvoices‎)‎ | 1.0.0.0 | לא נדרש להקצאה. |
| ישות יצוא שורות חשבוניות ספק של פרויקט שילוב של Project Operations (msdyn_projectvendorinvoices‎)‎ | 1.0.0.0 | לא נדרש להקצאה. |
| תפקידי משאבי פרויקט לכל החברות (bookableresourcecategories) | 1.0.0.1 | מחייב סנכרון ראשוני של מפת הטבלה כדי לסנכרן את תפקידי המשאבים של מנהל הפרויקט וחבר הצוות, שמאוכלסים בסביבת Dataverse Dynamics 365 במהלך ההקצאה. Dataverse הוא המקור הראשי לסנכרון הראשוני. |
| משימות פרויקט (msdyn_projecttasks) | 1.0.0.4 | לא נדרש להקצאה. |
| קטגוריות עסקאות פרויקט (msdyn_transactioncategories) | 1.0.0.0 | לא נדרש להקצאה. |
| פרויקטים גרסה 2 (msdyn_projects) | 1.0.0.1 | לא נדרש להקצאה. |

השלם את השלבים הבאים להפעלת המפות המפורטות.

1. הפעל את תפקידי משאבי הפרויקט עבור מפת הטבלה **כל החברות (bookableresourcecategories)** מכיוון שמפה זו דורשת סנכרון ראשוני. בתוך השזה **פריט ראשי לסנכרון ראשוני**, בחר **Common Data Service**. 

 ![סנכרון מפת טבלת תפקידי משאבים](media/6ResourceInitialSync.jpg)

 המתן עד שהמפה במצב **מופעל** לפני שתעבור לשלב הבא.

2. בחר את כל המפות הנדרשות שנותרו. אפשר לסנן אותם ברשימת המפות לכתיבה כפולה באמצעות מילת המפתח **פרויקט** בחיפוש בפינה השמאלית העליונה. ניתן לבצע בחירה של כל המפות ואז להפעיל. למידע נוסף ראה [ניהל מפות טבלה מרובות](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/multiple-entity-maps). הקפד להפוך לזמין ולהפעיל גם מפות ישויות קשורות.

### <a name="project-operations-dual-write-map-versions"></a>גרסאות מפה של כתיבה כפולה ב-Project Operations

הפעל תמיד את הגרסה האחרונה של המפה בסביבתך. ייתכן שתכונות ויכולות מסוימות לא יפעלו כראוי אם מתקיים אחד מהתנאים הבאים:

- מפה אינה מופעלת.
- הגרסה האחרונה של המפה אינה מופעלת. 
- מפות טבלה קשורות אינן מופעלות.

אפשר לראות את הגרסה הפעילה של המפה בעמודה **גרסה** בדף **כתיבה כפולה**. אפשר להפעיל גרסה חדשה של המפה על ידי בחירה באפשרות **גרסאות של מפת טבלאות**, בחירה בגדסה העדכנית ביותר ואז שמירה של הגרסה שנבחרה. אם התאמת אישית מפת טבלה שהגיעה מוכנה לשימוש עם המוצר, יהיה עליך להחיל מחדש את השינויים. מידע נוסף ראה [ניהול מחזור החיים של פתרונות](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).