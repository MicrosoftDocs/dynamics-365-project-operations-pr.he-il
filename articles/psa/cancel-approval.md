---
title: ביטול ערכי זמן והוצאה שאושרו בעבר
description: נושא זה מספק מידע אודות אופן הביטול של עסקת זמן והוצאה של פרוייקט שאושרה.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/07/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 0ea816040570cc8f6ddf3c5ec8a74ac092fc68b2
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077483"
---
# <a name="cancel-previously-approved-time-or-expense-entries"></a>ביטול ערכי זמן או הוצאה שאושרו בעבר

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

בגירסה העדכנית ביותר של Dynamics 365 Project Service Automation, מאשרים יכולים לבטל ערכי זמן או הוצאה שאושרו בעבר.

## <a name="cancel-a-previously-approved-time-or-expense-entry"></a>ביטול ערך זמן או הוצאה שאושר בעבר

בצע את השלבים הבאים כדי לבטל ערך זמן או הוצאה שאישרת בעבר.

1. עבור אל **פרוייקטים** \> **העבודה שלי** \> **אישורים**.
2. בדף הרשימה **אישורים** , שנה את התצוגה ל **האישורים הקודמים שלי**. רשימה של ערכי הזמן וההוצאות שאישרת בעבר מוצגת.
3. בחר ערך אחד או יותר, ולאחר מכן בחר **בטל אישור**. תקבל הודעת אזהרה.
4. בחר **אישור** כדי לבטל את האישור.

## <a name="understand-the-impact-of-canceling-a-time-or-expense-entry-approval"></a>הבנת ההשפעה של ביטול אישור של ערך זמן או הוצאה

כאשר אישור מבוטל, יש לכך גם השפעה תפעולית וגם השפעה פיננסית.

### <a name="operational-impact"></a>השפעה תפעולית

מבחינת התפעול, כאשר אישור מבוטל, מצב הרשומה מאופס ל **טיוטה** , והאישור אינו מופיע עוד בתצוגה **האישורים הקודמים שלי**. במקום זאת, האישור המבוטל מופיע בתצוגה **ערכי זמן לאישור** או בתצוגה **ערכי הוצאות לאישור** , בהתאם לשאלה אם זה היה ערך זמן או ערך הוצאה. בנוסף, המצב של ערך הזמן או ערך ההוצאה הקשור משתנה ל **נשלח** , כך שהערך הקשור תואם לאישורים בעלי מצב **טיוטה**.

כמאשר, באפשרותך לערוך חלק משדות האישור בעל מצב **טיוטה**. שדות אלה כוללים את **סוג חיוב** ואת **שעות לחיוב עבור ערכי זמן**. לאחר ביצוע שינויים, באפשרותך לאשר שוב את הרשומה. לחלופין, באפשרותך לדחות את הערך. אם תדחה את האישור של ערך זמן, מצב הערך ישתנה ל **הוחזר**. אם תדחה את האישור של ערך הוצאה, המצב ישתנה ל **נדחה**. מבחינה פונקציונלית, הן הערכים שהוחזרו והן הערכים שנדחו מתנהגים כמו ערך בעל מצב של **טיוטה**. חבר צוות של פרוייקט יכול לבצע שינויים נדרשים בערך ולאחר מכן לשלוח אותו מחדש לאישור, או למחוק את הערך לחלוטין.

### <a name="financial-impact"></a>השפעה פיננסית

פרוייקט מושפע גם מבחינה פיננסית כאשר אישור מבוטל. ראשית, הנתונים בפועל המתאימים עבור עלות ומכירות מתעדכנים באופן הבא:

- מצב ההתאמה מוגדר ל **מותאם**.
- מצב החיוב מוגדר ל **בוטל**.

בשלב הבא, ערכי ביטול נוצרים בטבלה 'נתונים בפועל'. כדי ליצור ערכי ביטול, המערכת מעתיקה את ערכי השדה מהנתונים בפועל המקוריים. הערכים היחידים שאינם מועתקים הם ערכי הכמות. ערכים אלה חוזרים לקדמותם במקום זאת. נתונים בפועל שבוטלו נוצרים הן עבור נתונים בפועל של **עלות** והן עבור נתונים בפועל של **מכירות שלא חויבו**. השדה **מצב התאמה** של הנתונים בפועל שהתבטלו מוגדר ל **לא ניתן להתאמה** ומצב החיוב מוגדר ל **בוטל**.

לאחר ששינויים אלה מתבצעים, הסכום שמתועד כסכום שהושקע בפרוייקט ומצבור ההכנסות בפרוייקט לא ייחשבו עוד לסכומים שנתונים בפועל אלה מייצגים.