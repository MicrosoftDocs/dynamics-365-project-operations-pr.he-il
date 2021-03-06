---
title: הגדר תהליכי עבודה לניהול הוצאות
description: באפשרותך להגדיר תהליך זרימת עבודה המשמש לבדיקה ולאישור מסמכי נסיעות והוצאות.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: dfc5945f32bb8d4073fc31499979ba279fef66a4
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896552"
---
# <a name="set-up-workflows-for-expense-management"></a>הגדר תהליכי עבודה לניהול הוצאות

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

באפשרותך להגדיר תהליך זרימת עבודה לבדיקה ולאישור מסמכי נסיעות והוצאות. באפשרותך להגדיר זרימות עבודה לדוחות הוצאות, דרישות נסיעות ובקשות למקדמות במזומן.

זרימת עבודה מייצגת תהליך עסקי ומגדירה כיצד מסמך זורם במערכת. זרימת העבודה מציינת גם מי חייב להשלים משימה או לאשר מסמך. ישנם מספר יתרונות לשימוש במערכת זרימת העבודה בארגון שלך:

- **תהליכים עקביים**: באפשרותך להגדיר את תהליך האישור למסמכים ספציפיים, כגון דרישות רכישה ודוחות הוצאות. השימוש במערכת זרימת העבודה מסייע להבטיח עיבוד של מסמכים באופן עקבי ויעיל.
- **נראות התהליך**: ניתן לעקוב אחר מדדי המצב, ההיסטוריה וביצועים של מופע זרימת עבודה ספציפי. זה עוזר לך לקבוע אם יש לבצע שינויים בתהליך העבודה כדי לשפר את היעילות.
- **רשימת עבודה מרכזית**: המשתמשים יכולים להציג רשימת עבודה מרוכזת כדי להציג את משימות זרימת העבודה ואת האישורים שהוקצו להם. 

## <a name="workflow-types"></a>סוגי זרימת עבודה

בטבלה הבאה רשומים סוגי תהליכי העבודה שבאפשרותך ליצור ב**ניהול הוצאות**.


|              <strong>סוג</strong>              |                   <strong>השתמש בסוג זה כדי</strong>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|   <strong>אישור אוטומטי של דוח הוצאות</strong> |            צור זרימות עבודה לדוחות הוצאות.             |
|  <strong>פרסום אוטומטי של דוח הוצאות</strong>   |        צור זרימות עבודה לפרסום אוטומטי של דוחות הוצאות.        |
|       <strong>פריט של סעיף הוצאה</strong>        |     צור זרימות עבודה לאישור עבור פריטי שורה בדוחות הוצאות.      |
| <strong>פרסום אוטומטי של פריט בדוח הוצאות</strong> | צור זרימות עבודה לפרסום אוטומטי עבור פריטי שורה בדוחות הוצאות. |
|       <strong>דרישת נסיעה</strong>       |          צור זרימות עבודה לאישור עבור דרישות נסיעה.           |
|      <strong>בקשה למקדמה במזומן</strong>      |         צור זרימות עבודה לאישור עבור בקשות מקדמה במזומן.          |
|        <strong>החזר מע"מ</strong>        | צור זרימות עבודה לאישור עבור החזרי מס ערך מוסף (מע"מ).  |
