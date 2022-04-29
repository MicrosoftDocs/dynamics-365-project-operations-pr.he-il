---
title: מעברי מצב בחוזה משנה
description: נושא זה מסביר את מעברי המצב בחוזה משנה ב- Dynamics 365 Project Operations‏ Microsoft כאשר חוזה המשנה נוצר, מבוצע ונסגר.
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: tonyafehr
ms.author: rumant
ms.openlocfilehash: d67f4a3cd834c25462304c2d75c824427fcbd034
ms.sourcegitcommit: 04dc8d952e6da3ab3eb2a20131c6f7cee6040876
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 12/10/2021
ms.locfileid: "7903442"
---
# <a name="state-transitions-on-a-subcontract"></a>מעברי מצב בחוזה משנה 

[!include [banner](../../includes/dataverse-preview.md)]

_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_

נושא זה מסביר את מעברי המצב בחוזה משנה ב- Dynamics 365 Project Operations‏ Microsoft. כל מצב מיוצג כטיוטה, כמאושר, כסגור או כמבוטל. התמונה הבאה מייצגת את מעברי המצב.

![מודל מצב חוזה משנה](../media/SubconStates.png)  

הטבלה הבאה מספקת תיאור של מה כל מצב מייצג במחזור החיים של חוזה משנה ב- Project Operations.

| מדינה בארה"ב | Description | מעברים מותרים |
| --- | --- | --- |
| טיוטה | מצב זה מייצג את המצב הראשוני של חוזה משנה. מתנהל משא ומתן עם הספק. הסעיפים והתמחור כפופים לשינויים. ניתן להשתמש בחוזה משנה במצב זה כדי להעריך ולאייש את דרישות הפרויקט למשאבים וחומרים. ניתן גם להפנות אליו בנושא זמן, הוצאות ושימוש בחומר בפרויקט. ניתן לערוך ולמחוק חוזה משנה במצב זה. | אושר |
| אושר | מצב זה מייצג את השלב שבו נמצא חוזה משנה לאחר השלמת המשא ומתן עם הספק לגבי התמחור והפריטים הנרכשים. עם זאת, אספקת החומרים ו/או העבודה בפועל על ידי משאבים בקבלנות משנה עדיין נמשכת. ניתן להשתמש בחוזה משנה במצב זה כדי להעריך ולאייש את דרישות הפרויקט למשאבים וחומרים. ניתן גם להפנות אליו בנושא זמן, הוצאות ושימוש בחומר בפרויקט. לא ניתן לערוך או למחוק חוזה משנה במצב זה. הלחצן **בטל** מאפשרת ביטול של חוזה משנה שאושר. הלחצן **פתח מחדש** מאפשר לך לפתוח מחדש את חוזה המשנה uלהחזיר אותו למצב **טיוטה**. השתמש בלחצן **סגור** לסגירת חוזה משנה שאושר. | סגירה <br> בוטלה <br> טיוטה |
| סגירה | מצב זה מייצג את השלב של חוזה המשנה שבו הושלמה אספקה בפועל של חומרים ו/או עבודה על ידי משאבים בקבלנות משנה. לא ניתן להשתמש בחוזה משנה במצב זה כדי להעריך ולאייש את דרישות הפרויקט למשאבים וחומרים. נוסף לכך, לא ניתן עוד להפנות אליו בנושא זמן, הוצאות ושימוש בחומר בפרויקט. לא ניתן לערוך או למחוק חוזה משנה במצב זה. | ללא |
| בוטלה | מצב זה מייצג את השלב של חוזה המשנה שבו לא נדרשת עוד אספקה בפועל של חומרים ו/או עבודה על ידי משאבים בקבלנות משנה. לא ניתן להשתמש בחוזה משנה במצב זה כדי להעריך ולאייש דרישות פרויקט למשאבים וחומרים, וגם לא ניתן להפנות אליו בנושא זמן, הוצאות ושימוש בחומר בפרויקט. לא ניתן לערוך או למחוק חוזה משנה במצב זה. | ללא |


[!INCLUDE[footer-include](../../includes/footer-banner.md)]