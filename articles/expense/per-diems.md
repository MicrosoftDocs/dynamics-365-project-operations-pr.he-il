---
title: אש"ל
description: נושא זה מספק מידע אודות כללי האש"ל המשמשים בניהול הוצאות.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 7d1c4ac7781cb711e2cc0d09606d422b4dd554f3
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908190"
---
# <a name="per-diems"></a>אש"ל

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_


דמי אש"ל הם קצבה המשולמת לעובד הנוסע למטרות עבודה. בניהול הוצאות, ניתן ליצור כללי אש"ל עבור מצבי נסיעה שונים. תעריפי אש"ל יכולים להתבסס על תקופת השנה, על יעד הנסיעה או על שניהם. כשיוצרים כלל לדמי אש"ל, אפשר לקבוע שאחוז תעריף האש"ל ההנאה ינוכה אם עובד מקבל ארוחות או שירותים בחינם. ניתן גם להגדיר מספר שעות מינימלי ומקסימאלי להחלת דמי אש"ל על נסיעה של עובד.

## <a name="configuration"></a>תצורה 

1. כדי להוסיף מיקומים לאש"ל, עבור אל **הגדרות** > **חישובים וקודים** > **מיקומי אש"ל**.
2. עבור כל אחד מהמיקומים שנוספו לעיל, בחרו תעריף אש"ל ומטבע, שתקף בין תאריך התחלה וסיום ספציפיים עבור מלון, ארוחות והוצאות אחרות. תעריפי האש"ל והמטבעות מוגדרים תחת **הגדרות** > **חישובים וקודים** > **דמי אש"ל**.
3. בדף **מיקומים לאש"ל**, הגדר את הרמות של תעריף אש"ל. רמות תעריף האש"ל מאפשרות לך להגדיר את אחוז הפיצול של הקצבה היומית עבור מלון, ארוחות והוצאות אחרות. 
4. כדי לציין את הפחתת האחוזים לארוחות בוקר, צהריים או ערב, יש עדכן את השדות בדף **פרמטרים לניהול הוצאות** בכרטיסיה **אש"ל**. 
    
## <a name="submit-expenses-using-per-diem"></a>הגשת הוצאות באמצעות אש"ל
כדי להגיש הוצאות באמצעות אש"ל , השתמש בקטגוריית ההוצאות **אש"ל** בעת יצירת דוח הוצאות. הזן את הערכים **אש"ל מהתאריך**, **אש"ל עד לתאריך**, ואת **מיקום האש"ל**. הסכום יחושב בהתבסס על תעריפי האש"ל עבור המיקום הנבחר והפחתת הארוחות תחושב על סמך רמות תעריפי האש"ל.
