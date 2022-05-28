---
title: נתונים בפועל
description: נושא זה מספק מידע על אופן העבודה עם נתונים בפועל ב- Microsoft Dynamics 365 Project Operations.
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
ms.openlocfilehash: 3f0cb8c478e2ce6fba589d51d95649f53f62e883
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8581285"
---
# <a name="actuals"></a>נתונים בפועל

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

‏‫נתונים בפועל‬ מייצגים את ההתקדמות הכספית והתקדמות לוח הזמנים שנבדקה ואושרה בפרויקט. הם נוצרים לאחר אישור ערכי זמן, הוצאות ושימוש בחומרים, פקודות יומן וחשבוניות.

> [!IMPORTANT]
> אין לערוך או למחוק נתונים בפועל מהמערכת. אחרת, היושרה הפיננסית ושילוב כלשהו עם מערכות פיננסיות וחשבונאיות אחרות עשויות להיות מושפעות לרעה. Microsoft Dynamics 365 Project Operations מאפשר לך להשתמש בביטול והחלפת נתונים בפועל כדי לערוך נתונים בפועל בנקודות שונות במחזור החיים של הפרויקטים שלך.

## <a name="recording-actuals-based-on-project-events"></a>תיעוד נתונים בפועל בהתבסס על אירועי פרוייקט

Project Operations מתעד את העסקאות הפיננסיות המתרחשות במהלך מחזור חיים של התקשרות בפרויקט כנתונים בפועל. יצירת נתונים בפועל באירועים שונים במחזור החיים משתנה, בהתאם לאם ההתקשרות בפרויקט משתמשת במודל חיוב הזמן והחומרים או במודל החיוב במחיר קבוע, ובין אם זה בשלב טרום המכירה או שמדובר בפרויקט פנימי.

הנושאים הבאים מסבירים את ההשפעה על טבלת הנתונים בפועל באירועים שונים עבור וריאציות שונות:

- [השפעה של נתונים בפועל על על התקשרות של זמן וחומרים](ActualsonTM.md)
- [השפעת הנתונים בפועל בהתקשרות במחיר קבוע](ActualonFP.md)
- [השפעת הנתונים בפועל בשלב טרום המכירה של התקשרות](ActualonPreSales.md)
- [השפעת נתונים בפועל עבור פרוייקט פנימי](ActualonInternal.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
