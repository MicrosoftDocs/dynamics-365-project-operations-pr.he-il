---
title: הזמנות מכירה בפרויקטים עבור פרויקטים של זמן וחומר
description: נושא זה מסביר כיצד ליצור הזמנות מכירה מבוססות פרויקטים עבור פרויקטים של זמן וחומר.
author: Yowelle
manager: AnnBe
ms.date: 04/05/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2019-04-05
ms.dyn365.ops.version: AX 10.0.2
ms.openlocfilehash: 3653a6869dab323be88f1fd0f9fd0f2cb35c456f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077293"
---
# <a name="project-sales-orders-for-time-and-material-projects"></a>הזמנות מכירה בפרויקטים עבור פרויקטים של זמן וחומר

[!include[banner](../includes/banner.md)]

נושא זה מתאר כיצד ליצור הזמנת מכירות לפרויקט. ניתן ליצור הזמנות מכירה רק עבור פרויקטיים מסוג **זמן וחומר**.

אם לפרויקט זמן וחומר יש כמה מקורות מימון בחוזה הפרויקט, עליך להפוך את הפרמטר **אפשר הזמנות מכירה עבור פרויקטים עם כמה מקורות מימון** לזמין בדף **ניהול פרויקטים ופרמטרים חשבונאיים**. 

> [!NOTE]
> - תמיכה בהזמנות מכירה של פרויקטים עם כמה מקורות מימון זמינה החל ממהדורת יישום 10.0.2 ואילך.
> - הפרמטר להפעלת תמיכה בהזמנות מכירה של פרויקט עם כמה מקורות מימון יוסר בגל ההפצה של אפריל 2020, שלאחריו הפונקציונליות תמיד תהיה מופעלת.

ניתן ליצור הזמנות מכירה מבוססות פרויקט בשתי דרכים:

- מעבר אל הפרויקט עצמו. בחלונית הפעולות, בחר **ניהול > משימות פריט > הזמנת מכירות**. פרטי הפרויקט יוגדרו כברירת מחדל להזמנת המכירות מהפרויקט. אם בחוזה הפרויקט יש יותר ממקור מימון אחד, יהיה עליך לבחור במקור המימון כדי להגדיר את הלקוח להזמנת המכירות. אם יש רק מקור מימון אחד לפרויקט, הלקוח יוגדר אוטומטית.
- עבור אל דף הרשימה **כל הזמנות המכירה** וצור הזמנת מכירות חדשה. עליך לבחור את הפרויקט להזמנת המכירות. לאחר בחירת הפרויקט, הלקוח יוגדר ממקור המימון או שתצטרך לבחור את מקור המימון אם לחוזה הפרויקט יש כמה מקורות מימון.
