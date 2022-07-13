---
title: השפעת נתונים בפועל עבור פרוייקט פנימי
description: מאמר זה מספק מידע על ההשפעה על טבלת הנתונים בפועל באירועים שונים עבור פרויקט פנימי ב- Microsoft Dynamics 365 Project Operations.
author: rumant
ms.date: 02/22/2022
ms.topic: overview
ms.prod: ''
audience: Application User
ms.reviewer: johnmichalak
ms.search.scope: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: de05714c079fe121ef68e28b1acb82c24bce095e
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8921349"
---
# <a name="actuals-impact-for-an-internal-project"></a>השפעת נתונים בפועל עבור פרוייקט פנימי

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

הטבלה הבאה מפרטת את הנתונים בפועל של סוגים שונים של עסקאות שנוצרות באירועים שונים בהתקשרות של פרויקט פנימי.

| אירוע | נתון בפועל של עלות | דוגמה |
|---|---|---|
| זמן נוצר. | לא ישים | <p>בוב קוזאק, מהיחידה הארגונית של Fabrikam בארה"ב ששיעור העלות שלו הוא 100 דולר ארה"ב (100 דולר ארה"ב) לשעה, עובד על פרויקט שנקרא "התקנת זרועות באדאטום". פרויקט זה ממופה לשיטת חיוב מחיר קבוע בסעיף החוזה. להלן ערך זמן לדוגמה של בוב קוזאק:</p><p>בוב קוזאק - 8 שעות</p> |
| הזמן נשלח. | לא ישים | נוצרת שורת יומן עלות עבור ערך הזמן. תעריף העלות המוגדר כברירת המחדל מוזן בפקודת היומן. |
| ערך הזמן מאוחזר לפני שהוא מאושר. | לא ישים | |
| הזמן מאושר. | נוצר נתון עלות בפועל. | <p>נתון בפועל חדשים שנוצר:</p><ul><li>**נתון עלות בפועל:** בוב קוזאק, 8 שעות, USD 800</li></ul> |
| אישור הזמן מבוטל. | <p>מצב ההתאמה של הנתון בפועל המקורי של העלות מתעדכן ל **מותאם**.</p><p>נוצרת ביטול של הנתון בפעול של עלות עם מצב התאמה של **לא ניתן להתאמה**.</p> | <p>נתון בפועל קיים שמתעדכן:</p><ul><li>**נתון עלות בפועל:** בוב קוזאק, 8 שעות, USD 800 *מותאם*</li></ul><p>נתון בפועל חדש שנוצר כדי לבטל את ההשפעה הכספית הקודמת:</p><ul><li>**נתון עלות בפועל:** בוב קוזאק, (8 שעות), (USD 800) *לא ניתן להתאמה*</li></ul> |
| ערך הזמן מאוחזר אחרי שהוא מאושר. | <p>מצב ההתאמה של הנתון בפועל המקורי של העלות מתעדכן ל **מותאם**.</p><p>נוצרת ביטול של הנתון בפעול של עלות עם מצב התאמה של **לא ניתן להתאמה**.</p> | <p>נתון בפועל קיים שמתעדכן:</p><ul><li>**נתון עלות בפועל:** בוב קוזאק, 8 שעות, USD 800 *מותאם*</li></ul><p>נתון בפועל חדש שנוצר כדי לבטל את ההשפעה הכספית הקודמת:</p><ul><li>**נתון עלות בפועל:** בוב קוזאק, (8 שעות), (USD 800) *לא ניתן להתאמה*</li></ul> |

[!INCLUDE[footer-include](../includes/footer-banner.md)]