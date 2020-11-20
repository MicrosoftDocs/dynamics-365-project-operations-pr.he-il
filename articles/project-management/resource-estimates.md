---
title: הערכות משאבים
description: נושא זה מספק מידע על אופן החישוב של הערכות משאבים ב-Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 454b8931db53739a7bc19364911109802a1ed087
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127362"
---
# <a name="resource-estimates"></a>הערכות משאבים

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

הערכות המשאבים מגיעות ממאמץ שמחולק ליחידות זמן עבודה המוגדר במבנה התפלגות העבודה יחד עם ממדי תמחור ישימים. בדרך כלל, החישוב הוא **תעריף לשעה לכל תפקיד x שעות.** המאמץ שמחולק ליחידות זמן עבודה של כל משאב נשמר ברשומת הקצאת המשאבים. התמחור נשמר במחירון שהוגדר מראש. המרת יחידות מיושמת על סמך המחירון הרלוונטי.

![הערכות משאבים](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a>ברירות מחדל של מחיר עלות ושל מטבע עלות

מחירי העלות מוגדרים כברירת מחדל מהיחידה הארגונית.

## <a name="default-bill-rate-and-sales-currency"></a>ברירות מחדל של תעריף חיוב ושל מטבע מכירות

מחירי מכירה מוחלים פעם אחת בכל עסקה. ההירארכיה לברירת המחדל של מחירון המכירה היא כדלקמן:

1. הארגון
2. לקוח
3. הצעת מחיר / חוזה
