---
title: לוח זמנים להוצאות של חקירת הפרסים הפדרליים
description: נושא זה מספק מידע על לוח הזמנים להוצאות החקירה על פרסים פדרליים.
author: velofog
manager: Ann Beebe
ms.date: 04/2/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: PSNProjSEFAinquiry
audience: Application User
ms.devlang: ''
ms.reviewer: roschlom
ms.search.scope: Operations, Core
ms.tgt_pltfrm: ''
ms.custom: ''
ms.search.region: Global
ms.search.industry: public sector
ms.author: andchoi
ms.search.validFrom: 2020-4-01
ms.dyn365.ops.version: 10.0.11
ms.openlocfilehash: eaf523ab147cbe974fed6e7eab21967404583fe6
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077292"
---
# <a name="schedule-of-expenditures-of-federal-awards-inquiry"></a>לוח זמנים להוצאות של חקירת הפרסים הפדרליים

[!include [banner](../includes/banner.md)]

על פי משרד ניהול התקציב A-133, סוכנויות המקבלות כספים פדרליים כפופות לדרישות ביקורת, המכונות גם ביקורת יחידה. תהליך הביקורת משמש לדיווח על הכנסות והוצאות של מענקים פדרליים על בסיס חוזר. חלק מדוח ביקורת היחידה כולל את לוח הזמנים של ההוצאות של פרסים פדרליים (SEFA).

לוח הזמנים של ההוצאות על חקירת פרסים פדרליים כולל את קטלוג המסמך הפדרלי לסיוע מקומי (CFDA), מספר המענק, שנת המענק, שם הסוכנות הפדרלית המספקת את הכספים ושם ישות המעבר. החקירה היא לתקופה מסוימת. בדרך כלל, תקופה זו זהה לתקופת הדוח הכספי, שהיא שנת כספים.

החקירה כוללת מענקים שמועדי ההעברה שלהם נמצאים בטווח התאריכים שנבחר. העמודה **סוכנות מענקים** של החקירה מציגה את לקוח המענק או, עבור מענק מעבר, את הסוכנות המעניקה. במקרה של מענק מעבר, העמודה **סוכנות מעבר** מציגה את לקוח המענק. אם המענק אינו מענק-מעבר, העמודה **סוכנות מעבר** ריקה.

## <a name="set-up-the-cfda-clusters"></a>הגדרת אשכולות CFDA

יש להגדיר את אשכולות ה- CFDA שיכולים להיות משויכים למספרי CFDA בתזמון ההוצאות של חקירת הפרסים הפדרליים.

1. עבור אל **ניהול פרויקטים וחשבונאות\> הגדרה \> מענקים \> קטלוג אשכולות סיוע מקומי פדרלי**.
2. בחר **חדש** כדי ליצור אשכול CFDA.
3. הזן את שם האשכול.
4. בחר **שמור** כדי לשמור את השינויים.

## <a name="set-up-cfda-numbers"></a>הגדר מספרי CFDA

יש להגדיר את מספרי ה- CFDA שניתן להוסיף למענקים ולכלול בתזמון ההוצאות של חקירת הפרסים הפדרליים.

1. עבור אל **ניהול פרויקטים וחשבונאות \> הגדרה \> מענקים \> קטלוג מספרים של סיוע מקומי פדרלי**.
2. בחר **חדש** כדי ליצור מספר CFDA.
3. בעמודה **מספר** , הזן את המספר ה- CFDA.
4. לחץ על המקש **כרטיסיה**.
5. בעמודה **תיאור** , הזן את כותרת ה- CFDA.
6. לחץ על המקש **כרטיסיה**.
7. אופציונלי: בשדה **אשכול התוכנית** , הוסף את אשכול ה- CFDA המתאים.
8. בחר **שמור** כדי לשמור את השינויים.

## <a name="set-up-grants-to-report-for-the-schedule-of-expenditures-of-federal-awards-inquiry"></a>הגדר מענקים לדיווח עבור לוח הזמנים לחקירה של פרסי הוצאות פדרליים

1. עבור אל **ניהול פרויקטים וחשבונאות \> מענקים \> מענקים** , ובחר מענק קיים.
2. בכרטיסיה **הגדרה** בשדה  **קטלוג סיוע מקומי פדרלי** , הקצה את מספר ה- CFDA. מספר ה- CFDA במענק קובע את אשכול ה- CFDA לדיווח.
3. בכרטיסיה **פרטי התקשרות** , הזן את פרטי המעניק על ידי ביצוע השלבים הבאים:

    1. בשדה **לקוח המענק** , הזן את הלקוח שאחראי למענק. לקבלת מענק קיים, ייתכן שהמידע הזה כבר הוזן.
    2. ציין אם לקוח המענק הוא המממן. אם לקוח המענק הוא המממן, השאר את התיבה **מעבר** ללא סימון. אם לקוח אחר הוא המממן, ולקוח המענק אחראי על הוצאות הכסף ומעקב אחריו, סמן את התיבה **מעבר**.

4. אם סימנת את התיבה **מעבר** בשלב הקודם, בשדה **סוכנות מענק** הזן את הלקוח שסיפק את המענק. הסוכנות המעניקה ולקוח המענק אינם יכולים להיות אותו לקוח.

הנה דוגמה למענק מעבר:

הממשלה הפדרלית מימנה פרויקט תשתית למדינה. הממשלה הפדרלית נתנה את הכסף למדינה. במקרה זה, הממשלה הפדרלית היא הסוכנות המעניקה, והמדינה היא לקוח המענק.

> [!NOTE] 
> כאשר אתה מפעיל לראשונה את התכונה, מספרי CFDA ראשוניים יוזנו באמצעות המספרים הקיימים במענקים.

## <a name="exclude-grants-from-sefa-reporting-based-on-the-grant-type"></a>אל תכלול מענקים מדיווח SEFA בהתבסס על סוג המענק

1. עבור אל  **ניהול פרויקטים וחשבונאות \> הגדרה \> מענקים \> סוגי מענקים**.
2. בכרטיסיה **פרטי ברירת מחדל** סמן את התיבה **לא לכלול בתזמון ההוצאות של פרסים פדרליים**.
3. בחר **שמור** כדי לשמור את השינויים.

## <a name="run-the-schedule-of-expenditures-of-federal-awards-inquiry"></a>הפעל את לוח זמנים להוצאות של חקירת הפרסים הפדרליים

1. עבור אל **ניהול פרויקטים וחשבונאות \> חקירות ודוחות \> חקירת מענקים \> לוח זמנים להוצאות של פרסים פדרליים**.
2. במקטע **פרמטרים** , בצע את הפעולות הבאות:

    1. בשדה **טווח תאריכים** בחר את הקוד עבור טווח התאריכים. לחלופין, בשדות **מתאריך** ו- **עד תאריך** , הגדר את טווח התאריכים.
    2. אופציונלי: כדי לכלול רק עסקאות שחויבו כהכנסות בחקירה, הגדר את האפשרות **כלול רק הכנסות שחויבו** שתהיה **כן**.

## <a name="columns"></a>עמודות

לוח הזמנים להוצאות של חקירת הפרסים הפדרליים כולל את העמודות הבאות:

- שם הקטלוג של אשכול פדרלי לסיוע מקומי
- סוכנות מענק
- סוכנות מעבר
- שם מענק
- מזהה מענק
- מזהה יישום מענק
- קטלוג של אשכולות פדרליים לסיוע מקומי
- קבלות
- הוצאות