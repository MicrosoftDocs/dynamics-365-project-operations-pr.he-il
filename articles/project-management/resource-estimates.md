---
title: הערכות משאבים
description: נושא זה מספק מידע על אופן החישוב של הערכות משאבים ב-Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 2ebde2b3c5bcfb5faa02ee476065ac34b1953432
ms.sourcegitcommit: f255b2cbf290973ce62fe2c1c121bd1df15a7392
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/01/2020
ms.locfileid: "3928570"
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
