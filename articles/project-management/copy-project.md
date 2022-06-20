---
title: העתקת פרויקט
description: מאמר זה מספק מידע על העתקת פרויקטים ב- Dynamics 365 Project Operations.
author: ruhercul
ms.date: 03/07/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: b358f9e45278d886f3e6e8e8cd747fc0ea30212b
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8925765"
---
# <a name="copy-a-project"></a>העתקת פרויקט

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

עם Dynamics 365 Project Operations אפשר לבנות במהירות פרויקטים חדשים על ידי בחירה באפשרות **העתק פרויקט** בטופס **פרויקטים** . להעתקת פרויקט, פתח את הפרויקט שברצונך להעתיק ואז בחר **העתק פרויקט**. הפעולה תעתיק את הפרטים הבאים:

- מאפייני פרויקט 
- מבנה התפלגות העבודה
- חברי צוות בפרוייקט
- הערכות פרוייקט
- הערכות הוצאה בפרויקט
- הערכות חומרים בפרוייקט
- רשימות פעולות לביצוע של פרויקט
- המיכלים של של פרוייקט

## <a name="project-properties"></a>מאפייני פרויקט

כאשר הפרויקט מועתק, הערכים בשדות הבאים מועתקים.

| שדה | Project Operations לחומרים שאינם במלאי | ו- Project Operations Lite | Project for the Web |
|-------|------------------------------------------|-------------------------|---------------------|
| Name | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| Description | :heavy_check_mark: | :heavy_check_mark: | |
| לקוח | :heavy_check_mark: | :heavy_check_mark: | |
| תבנית לוח שנה | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| מטבע | :heavy_check_mark: | :heavy_check_mark: | |
| יחידת החוזה | :heavy_check_mark: | :heavy_check_mark: | |
| החברה המהווה בעלים | :heavy_check_mark: | | |
| מנהל פרויקט | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| סטטוס | :heavy_check_mark: | :heavy_check_mark: | |
| מצב פרוייקט כולל | :heavy_check_mark: | :heavy_check_mark: | |
| הערות  | :heavy_check_mark: | :heavy_check_mark: | |
| הערכות | :heavy_check_mark: | :heavy_check_mark: | |
| <p>תאריך התחלה משוער</p><p><strong>הערה:</strong> שדה זה מציין את התאריך שבו הפרוייקט נוצר מהעותק. | :heavy_check_mark: | :heavy_check_mark: | |
| <p>תאריך סיום משוער</p><p><strong>הערה:</strong> התאריך בשדה זה מותאם לפי לתאריך ההתחלה של הפרויקט החדש שנוצר מהעותק.</p> | :heavy_check_mark: | :heavy_check_mark: | |
| מאמץ (בשעות) | :heavy_check_mark: | :heavy_check_mark: | |
| עלות עבודה משוערת | :heavy_check_mark: | :heavy_check_mark: | |
| עלות הוצאות משוערת | :heavy_check_mark: | :heavy_check_mark: | |
| עלות חומרים משוערת | | :heavy_check_mark: | |

> [!NOTE]
> העתקת פרוייקט יכולה להיות פעולה ארוכת טווח. מועתקים גם רשומות הפרוייקט, המאפיינים הרלוונטיים שלו וישויות קשורות רבות. בגלל אופי הפעולה הארוכה, לאחר תחילת ההעתקה, דף פרוייקט היעד נעול לעריכה עד להשלמת פעולת ההעתקה.

## <a name="work-breakdown-structure"></a>מבנה התפלגות העבודה

כאשר הפרויקט מועתק, כל מבנה התפלגות העבודה של המשאב שנטען מועתק. משאבים בעלי שם מוחלפים במשאבים כלליים. אם למשאבים בעלי שם אין את אותן שעות עבודה כמו להמשאב הגנרי, לוח הזמנים יחושב מחדש ומשך המשימות עשוי להשתנות.

## <a name="project-team-members"></a>חברי צוות בפרויקט

כאשר צוות פרויקט מועתק מפרויקט המקור, המשאבים הכלליים מועתקים. הקצאות של המשאבים הכלליים נשארות כפי השהיו בפרוייקט המקור. משאבים בעלי שם יומרו לחברי צוות כלליים.

> [!NOTE]
> חברי צוות ומשימות אינן מועתקות ב- Project for the Web.

## <a name="estimates"></a>הערכות

כאשר מועתק הפרוייקט, מועתקים שורות המשאבים, ההוצאות והערכות החומר מפרוייקט המקור. 

למידע על אופן הגישה הפרוגרמטית אל 'העתק פוריקט', ראה [פיתוח תבניות פרוייקט באמצעות 'העתקת פוריקט'](dev-copy-project.md).

## <a name="quotes-and-contracts"></a>הצעות מחיר וחוזים

הצעות מחיר וחוזים אינם מקושרים לפרויקט היעד.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
