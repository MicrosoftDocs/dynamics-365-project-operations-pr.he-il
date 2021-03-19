---
title: מה חדש, מרץ 2021 - Project Operations לתרחישים מבוססי משאבים/ללא מלאי
description: נושא זה מספק מידע על עדכוני האיכות הזמינים במהדורת מרץ 2021 של Project Operations לתרחישים מבוססי משאבים/לא מלאי.
author: sigitac
manager: tfehr
ms.date: 03/03/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 95a9251707de3699322471535aa93070ba4fb2ae
ms.sourcegitcommit: f78087174a8512199a1bcbd7e8610bbc80e64801
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "5500005"
---
# <a name="whats-new-march-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>מה חדש, מרץ 2021 - Project Operations לתרחישים מבוססי משאבים/ללא מלאי

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

נושא זה חל על הרכיבים והגירסאות הבאים של Dynamics 365 Project Operations:

- Project Operations בסביבת Dataverse גרסה 4.8.0.91 
- ניהול פרויקטים וחשבונאות בסביבת Dynamics 365 Finance גרסה 10.0.16 

## <a name="quality-updates"></a>עדכוני איכות

### <a name="project-operations-on-dataverse"></a>Project Operations ב- Dataverse


| **אזור תכונות** | **מספר אסמכתא** | **עדכון איכות** |
| --- | --- | --- |
| חיוב ותמחור | 2133873 | תוקנה התצוגה של סמל מטבע **מחיר מכירות ליחידה** ברשת **אומדני הוצאות**. |
| חיוב ותמחור | 2174616 | כאשר הצעת מחיר זוכה, יש התייחסות למחירון מותאם אישית של חוזה בסעיפי חוזה שמועתקים מהצעת המחיר. |
| ניהול הזדמנויות | 2167475 | סכום מס קבוע בחשבונית התיקון שמקורו ברישום בפועל שלא בוצע. |
| ניהול הזדמנויות | 2176285 | אין להעתיק סכום מס מפרטי חוזה מכירות/שורת הצעת מחיר לפרטי חוזה עלות/הצעת מחיר. |
| ניהול הזדמנויות | 2188079 | אין ליצור כלל חיוב מפוצל עבור חוזים שאינם מבוססים על עבודה. |
| ‏‫תכנון ומעקב | 2125274 | התכונה **מפת פרוייקט בכתיבה כפולה** עבור **מיפוי תאריכי התחלה בפרויקט** עודכנה מ- **msdyn\_taskearlieststart‎** ל- **msdyn\_actualstart‎**. |
| ‏‫תכנון ומעקב | 2138853 | פונקציית העתקת הפרויקט עודכנה כדי להבטיח ששורות אומדן הוצאות שמתייחסות להפניה מועתקות לפרויקט היעד. |
| ‏‫תכנון ומעקב | 2154306 | תוקנו בעיות במחיקת אומדני הוצאות ב- Project Operations לתרחישים מבוססי משאבים. |
| ‏‫תכנון ומעקב | 2173259 | פונקציית העתקת הפרויקט עודכנה כדי להבטיח שהיא לא מציגה הודעת שגיאה על **העתקת WBS** בתרחישים מסוימים. |
| זמן והוצאה | 2148910 | תוקנה בעיה בתצוגה קבועה בדף **ערוך ערך** ברשת **ערכי זמן**. |
| זמן והוצאה | 2159798 | בקרות טובות יותר כדי להבטיח שלא ניתן לערוך רשומות הוצאות שאושרו. |

### <a name="project-management-and-accounting-on-dynamics-365-finance"></a>ניהול פרויקטים וחשבונאות ב- Dynamics 365 Finance

למידע נוסף, ראה [מה חדש, ינואר 2021 - Project Operations לתרחישים המבוססים על משאבים/ללא מלאי](whats-new-jan-2021-resource-based.md).

## <a name="regulatory-updates"></a>עדכוני רגולציה

למידע על עדכונים רגולטוריים עבור יישומי Finance and Operations, ראה [עדכוני רגולציה](https://docs.microsoft.com/dynamics365/finance/localizations/regulatory-updates). דרך נוספת ללמוד על עדכונים רגולטוריים היא להיכנס אל LCS ולהציג את עדכוני הרגולציה המתוכננים באמצעות כלי חיפוש הבעיות. חיפוש בעיות מאפשר לך לחפש לפי מדינה, סוג תכונה והפצה.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
