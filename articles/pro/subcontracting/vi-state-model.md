---
title: מעברי מצב בחשבונית ספק
description: מאמר זה מסביר את מעברי המצב בחשבונית ספק ב- Microsoft Dynamics 365 Project Operations‏.
author: rumant
ms.date: 03/30/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 58b07322fb6480fdeb07eb867a7aabc0eff7b955
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8934321"
---
# <a name="state-transitions-on-a-vendor-invoice"></a>מעברי מצב בחשבונית ספק

[!include [banner](../../includes/dataverse-preview.md)]

_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_

מאמר זה מסביר את מעברי המצב בחשבונית ספק ב- Microsoft Dynamics 365 Project Operations‏. נעשה שימוש במצבים הבאים: **טיוטה**, **בבדיקה**, **מאושר**, **בהמתנה** ו **מבוטל**.

האיור הבא מציג את מעברי המצב.

![מודל מעבר של מצב חוזה משנה.](../media/VI_State_Model.jpg)

הטבלה הבאה מסבירה מה כל מצב מייצג במחזור החיים של חשבונית ספק ב- Project Operations.

| מדינה בארה"ב | Description | מעברים מותרים |
| --- | --- | --- |
| טיוטה | המצב הוא המצב ההתחלתי של חשבונית ספק. הסעיפים והתמחור כפופים לשינויים. לא ניתן לערוך ולמחוק חשבונית ספק במצב זה. | בתהליך |
| בבדיקה | מצב זה מייצג את מצב העיבוד של חשבונית ספק. לפחות שורה אחת של חשבונית ספק נמצאת במצב אימות **בביצוע**. | מאושר, בהמתנה |
| אושר | מצב זה מייצג את השלב בחשבונית ספק שבו האפליקציה יצרה עלויות בפועל עבור כל שורת חשבונית ספק. כל העלויות בפועל הקשורות שהותאמה לשורות חשבונית ספק בוטלו והוחלפו בעלויות בפועל מאותן שורות חשבונית ספק. לא ניתן לערוך או למחוק חשבונית ספק במצב זה. אפשר להשתמש בלחצן **ביטול** כדל לבטל חשבונית ספק שאושרה. פעולת הביטול מבטלת את ההשפעה של פעולת האישור. | בוטלה |
| בהמתנה | <p>מצב זה מייצג שלב בחשבונית ספק שבו חשבונית ספק לא יכולה לנוע בגלל בעיה בחשבונית או במצב הספק. לא ניתן לאשר, לבטל, לערוך או למחוק חשבונית ספק במצב זה.</p><p>אפשר להשתמש בפעולת פתיחה מחדש כדי להעביר את חשבונית הפסק למצב **טיוטה** או **בבדיקה**. אם שורה אחת לפחות בחשבונית ספק נמצאת במצב אימת **בביצוע** או **הושלם**, חשבונית הספק תיפתח מחדש במצב **בבדיקה**. אם כל השורות בחשבונית הספק נמצאות במצב **לא התחיל**, חשבונית הספק תיפתח במצב **טיוטה**.</p> | טיוטה, בבדיקה |
| בוטלה | מצב זה מייצג את השלב של חוזה המשנה שבו לא נדרשת עוד אספקה בפועל של חומרים ו/או עבודה על-ידי משאבים בקבלנות משנה. לא ניתן להשתמש בחוזה משנה במצב זה כדי להעריך ולאייש דרישות פרויקט למשאבים וחומרים, וגם לא ניתן להפנות אליו בנושא זמן, הוצאות ושימוש בחומר בפרויקט. לא ניתן לערוך או למחוק חוזה משנה במצב זה. | ללא |

[!INCLUDE[footer-include](../../includes/footer-banner.md)]