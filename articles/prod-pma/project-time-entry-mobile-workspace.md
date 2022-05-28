---
title: סביבת עבודה ניידת של הזנת זמן בפרויקט
description: נושא זה מספק מידע על סביבת עבודה ניידת של הזנת זמן בפרויקט. סביבת עבודה זו מאפשרת למשתמשים להזין שעות לפרויקט ולשמור אותם באמצעות המכשיר הנייד שלהם.
author: Yowelle
ms.date: 12/01/2017
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: johnmichalak
ms.custom: 272101
ms.assetid: 4505f021-b9bb-4b87-be24-6bf0bd88ee60
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: Version 1611
ms.search.validFrom: 2016-11-30
ms.openlocfilehash: 64a80d931332a4d6edfcd175d7168a7815ddca38
ms.sourcegitcommit: 2c2a5a11d446adec2f21030ab77a053d7e2da28e
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/04/2022
ms.locfileid: "8683953"
---
# <a name="project-time-entry-mobile-workspace"></a>סביבת עבודה ניידת של הזנת זמן בפרויקט

[!include [banner](../includes/banner.md)]

נושא זה מספק מידע על סביבת עבודה ניידת של **הזנת זמן בפרויקט**. סביבת עבודה זו מאפשרת למשתמשים להזין שעות לפרויקט ולשמור אותם באמצעות המכשיר הנייד שלהם.

סביבת עבודה ניידת זו מיועדת לשימוש עם יישום Dynamics 365 Unified Ops למכשירים ניידים. 

## <a name="overview"></a>מבט כולל
משאבי פרויקט, כחלק מעבודתם היומיומית, נמצאים לעיתים קרובות באתר או בנסיעות. סביבת העבודה הניידת של **הזנת זמן בפרויקט** מאפשרת למשתמשים להזין את השעות הניתנות לחיוב ושאינן ניתנות לחיוב כנגד פרויקט במכשיר הנייד שלהם. לכן, משאבי הפרויקט יכולים לתעד ערכי זמן בכל עת ובכל מקום. הם יכולים גם להציג ערכי זמן שכבר תועדו. 

באופן ספציפי, בסביבת העבודה הניידת של **הזנת זמן בפרויקט**, משתמשים יכולים לבצע את המשימות הבאות:

-   עבור כל תאריך שנבחר, הזנת מספר השעות שהוקדשו למשימה ספציפית.
-   חיפוש לפי שם פרויקט או לקוח כדי למצוא את הפרויקט שעבורו יש להזין שעות.
-   ציון הקטגוריה והפעילות עבור השעות שהוקדשו.
-   תיעוד השעות כניתנות לחיוב או כלא ניתנות לחיוב עבור הפרויקט.
-   אפשרות להזנת הערה חיצונית או פנימית.

## <a name="prerequisites"></a>דרישות מוקדמות
הדרישות המוקדמות משתנות, בהתאם לגירסה של Microsoft Dynamics 365 שנפרסה עבור הארגון שלך.

### <a name="prerequisites-if-you-use-dynamics-365-finance"></a>תנאים מוקדמים לשימוש ב- Dynamics 365 Finance
אם Finance נפרס עבור הארגון שלך, מנהל המערכת חייב לפרסם את סביבת העבודה הניידת של **הזנת זמן בפרויקט**. ‏‫לקבלת הנחיות, ראה [פרסום סביבת עבודה ניידת](/dynamics365/fin-ops-core/dev-itpro/mobile-apps/publish-mobile-workspace).

### <a name="prerequisites-if-you-use-version-1611-with-platform-update-3-or-later"></a>דרישות מקדימות אם אתה משתמש בגירסה 1611 עם עדכון 3 ואילך לפלטפורמה
אם גירסה 1611 עם עדכון 3 ואילך לפלטפורמה נפרסה עבור הארגון שלך, מנהל המערכת חייב להשלים את הדרישות המוקדמות הבאות. 

<table>
<thead>
<tr class="header">
<th>דרישה מוקדמת</th>
<th>תפקיד</th>
<th>תיאור</th>
</tr>
</thead>
<tbody>
<tr class="odd">

<td>הטמעת KB 4018050.</td>
<td>מנהל מערכת</td>
<td>KB 4018050 הוא עדכון X++‎ או תיקון חם למטה-נתונים שמכיל את סביבת העבודה הניידת של <strong>הזנת זמן בפרויקט</strong>. כדי להטמיע את KB 4018050, מנהל המערכת חייב לבצע את השלבים הבאים.
<ol>
<li><a href="/dynamics365/fin-ops-core/dev-itpro/migration-upgrade/download-hotfix-lcs">הורדת התיקון החם למטה-נתונים מ- Microsoft Dynamics Lifecycle Services (LCS)‎</a>.</li>
<li><a href="/dynamics365/fin-ops-core/dev-itpro/migration-upgrade/install-metadata-hotfix-package">התקנת התיקון החם של המטה-נתונים</a>.</li>
<li><a href="/dynamics365/fin-ops-core/dev-itpro/deployment/create-apply-deployable-package">יצירת חבילה ניתנת לפריסה</a> המכילה את המודל <strong>ApplicationSuite</strong> ואת המודל <strong>ProjectMobile</strong> ולאחר מכן להעלות את החבילה הניתנת לפריסה ל- LCS.</li>
<li><a href="/dynamics365/fin-ops-core/dev-itpro/deployment/apply-deployable-package-system">החלת החבילה הניתנת לפריסה</a>.</li>

</ol></td>
</tr>
<tr class="even">
<td>פרסום סביבת העבודה הניידת של <strong>הזנת זמן בפרויקט</strong>.</td>
<td>מנהל מערכת</td>
<td>ראה <a href="/dynamics365/fin-ops-core/dev-itpro/mobile-apps/publish-mobile-workspace">פרסום סביבת עבודה ניידת</a>.</td>
</tr>
</tbody>
</table>

## <a name="download-and-install-the-mobile-app"></a>הורדת היישום למכשירים ניידים והתקנתו

הורד והתקן את האפלקייה למכשירים ניידים פיננסים ותפעול:

-   [לטלפונים של Android](https://go.microsoft.com/fwlink/?linkid=850662)
-   [לטלפוני iPhone](https://go.microsoft.com/fwlink/?linkid=850663)

## <a name="sign-in-to-the-mobile-app"></a>היכנס ליישום למכשירים ניידים
1.  הפעל את היישום במכשיר הנייד שלך.
2.  הזן את כתובת ה- URL של Dynamics 365.
3.  בפעם הראשונה שתיכנס, תתבקש להזין את שם המשתמש והסיסמה שלך. הזן את האישורים שלך.
4.  לאחר הכניסה, סביבות העבודה הזמינות עבור החברה שלך מוצגות. שים לב, אם מנהל המערכת מפרסם סביבת עבודה חדשה מאוחר יותר, יהיה עליך לרענן את רשימת סביבות העבודה הניידות.

[![משיכה לצורך ריענון.](./media/pull-to-refresh-list-of-workspaces-183x300.png)](./media/pull-to-refresh-list-of-workspaces.png)

## <a name="enter-time-by-using-the-project-time-entry-mobile-workspace"></a>הזנת שעות באמצעות סביבת העבודה הניידת של הזנת זמן בפרויקט
1.  במכשיר הנייד, בחר את סביבת העבודה **הזנת זמן בפרויקט**.
2.  בחר **הזנת זמן**. מוצגים תאריכי לוח השנה לשבוע הנוכחי.
3.  לתאריך שנבחר, בחר **פעולות** &gt; **ערך חדש**.
4.  הזן את מספר השעות שיש לתעד.
5.  בחר את הפרויקט עבור הזנת ערכי הזמן. רשימה המציגה את הפרויקטים שנטענים אל היישום לשימוש לא מקוון. כברירת מחדל, 50 פריטים נטענים, אך מפתח יכול לשנות את המספר הזה. למידע נוסף, ראה [פלטפורמה למכשירים ניידים](/dynamics365/fin-ops-core/dev-itpro/mobile-apps/mobile-app-home-page).
6.  אם הפרויקט שלך לא ברשימה, בחר **חפש**. חפש לפי שם או עבור לחיפוש לפי שם פרויקט או לקוח.
7.  בחר קטגוריה. רשימה המציגה את הקטגוריות שנטענות אל היישום לשימוש לא מקוון. כברירת מחדל, 50 פריטים נטענים, אך מפתח יכול לשנות את המספר הזה. למידע נוסף, ראה [פלטפורמה למכשירים ניידים](/dynamics365/fin-ops-core/dev-itpro/mobile-apps/mobile-app-home-page).
8.  אם הקטגוריה לא ברשימה, בחר **חפש**. חפש לפי קטגוריה או עבור לחיפוש לפי שם קטגוריה.
9.  בחר פעילות. רשימה המציגה את הפעילויות שנטענות אל היישום לשימוש לא מקוון. כברירת מחדל, 50 פריטים נטענים, אך מפתח יכול לשנות את המספר הזה. למידע נוסף, ראה [פלטפורמה למכשירים ניידים](/dynamics365/fin-ops-core/dev-itpro/mobile-apps/mobile-app-home-page).
10. אם הפעילות לא ברשימה, בחר **חפש**. חפש לפי מספר פעילות או עבור לחיפוש לפי מטרה.

11. בחר את מאפיין השורה.
12. אופציונלי‬: הזן הערות חיצוניות ופנימיות.
13. בחר **סיום**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]