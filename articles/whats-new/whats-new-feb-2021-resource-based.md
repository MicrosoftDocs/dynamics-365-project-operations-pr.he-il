---
title: מה חדש, פברואר 2021 - Project Operations לתרחישים מבוססי משאבים/ללא מלאי
description: נושא זה מספק מידע על עדכוני האיכות הזמינים במהדורת פברואר 2021 של Project Operations לתרחישים מבוססי משאבים/לא מלאי.
author: sigitac
manager: tfehr
ms.date: 02/08/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 2ba44ea471f7d72d1e816ec74de304d3fdcf1f68
ms.sourcegitcommit: 625b5244aaadff5a24a79d9addff91f87c6b015a
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/09/2021
ms.locfileid: "5141315"
---
# <a name="whats-new-february-2021---project-operations-for-resourcenon-stocked-based-scenarios"></a>מה חדש, פברואר 2021 - Project Operations לתרחישים מבוססי משאבים/ללא מלאי

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

נושא זה חל על הרכיבים והגירסאות הבאים של Dynamics 365 Project Operations:

- Project Operations בסביבת Dataverse 4.7.0.95
- ניהול פרויקטים וחשבונאות בסביבת Dynamics 365 Finance גרסה 10.0.16 

## <a name="quality-updates"></a>עדכוני איכות

### <a name="project-operations-on-dataverse"></a>Project Operations ב- Dataverse

| **אזור תכונות** | **מספר אסמכתא** | **עדכון איכות** |
| --- | --- | --- |
| **חיוב ותמחור** | 2053736 | כעת ניתן לגשת לפרטי שורת החשבונית על ידי מעבר אל **חשבונית מס** > **מידע קשור**. |
| **חיוב ותמחור** | 2122613 | הפעולות **הפעלה** ו **השבתה** הוסרו מהישויות הקשורות של **מחירון**. |
| **חיוב ותמחור** | 2128606 | נפתרה בעיה עם **ullReferenceException** ביישום plug-in **GetEstimatesForProject**. |
| **פריסה וקביעת תצורה** | 2139346 | נפתרה בעיה בייבוא לא מנוהל של פתרון **Dynamics365ProjectOperationsDualWrite**. |
| **פריסה וקביעת תצורה** | 2140569 | אין להתקין את פתרון הפרוייקט בסביבות של Dataverse Teams. |
| **פריסה וקביעת תצורה** | 2086991 | התאמה לשפות אחרות מוגבלת של משאבי רשת. |
| **ניהול הזדמנויות** | 2136794 | מופיעה הודעת השגיאה הנכונה כאשר התהליכים **אשר חשבונית** או **סמן חשבונית כ'שולמה'** נכשלים. |
| **ניהול הזדמנויות** | 2139330 | החלפה של מנהל הפרוייקט בפרוייקט לא יכולה לאפס את החברה המחזיקה לערך ברירת המחדל. |
| **ניהול הזדמנויות** | 2146376 | סכום המס המתוקן בפועל שאינו חייב בתשלום נוצר מאישור החשבונית. |
| **‏‫תכנון פרוייקטים ומעקב אחריהם** | 2099879 | פריסת הסביבה של Dataverse חייבת ליצור קטגוריית ברירת מחדל של עסקאות עם מזהה סטטי ולא ליצור באופן אקראי אחת לכל סביבה. |
| **‏‫תכנון פרוייקטים ומעקב אחריהם** | 2128577 | תוקנו הרשאות המשתמשים ב- Project Service לעדכון קטגוריית העסקה בהקצאת משאבים. |
| **‏‫תכנון פרוייקטים ומעקב אחריהם** | 2164035 | תוקנו בעיות בפונקציה **העתק פרוייקט**. |
| **ערך זמן** | 2129161 | הופעלו מגבלות מחמירות יותר כדי להבטיח שמשתמשים אינם יכולים לשנות ולעדכן רשומת זמן שהוגשה או אושרה. |
| **ערך זמן** | 2103572 | אישור זמן לערכי זמן שאינם פרוייקטים לא יכול לחפש תפקיד של מאשר פרוייקט. |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>ניהול פרויקטים וחשבונאות ב-Dynamics 365 Finance 

למידע נוסף על ניהול פרוייקטים וחשבונאות ב- Dynamics 365 Finance, ראה [מה חדש בינואר 2021 - Project Operations לתרחישים מבוססי משאבים/לא מלאי](whats-new-jan-2021-resource-based.md).


## <a name="regulatory-updates"></a>עדכוני רגולציה

למידע על עדכונים רגולטוריים עבור יישומי Finance and Operations, ראה [עדכוני רגולציה](https://docs.microsoft.com/dynamics365/finance/localizations/regulatory-updates). דרך נוספת ללמוד על עדכונים רגולטוריים היא להיכנס אל Lifecycle Services‏ (LCS) ולהציג את עדכוני הרגולציה המתוכננים באמצעות כלי חיפוש הבעיות. חיפוש בעיות מאפשר לך לחפש לפי מדינה, סוג תכונה והפצה.