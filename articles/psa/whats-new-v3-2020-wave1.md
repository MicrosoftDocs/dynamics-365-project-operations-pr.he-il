---
title: מה חדש או השתנה בגירסה ‎3.x wave 1 2020 של Project Service Automation
description: נושא זה מספק מידע על מה חדש ומה שהשתנה בגירסה 3, גל 1 2020 של Project Service Automation.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 05/15/2020
ms.topic: article
author: stsporen
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 16b51995f863d9ee54172625dacbf081c51c8556
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077254"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3-wave-1-2020"></a>מה חדש או השתנה בגירסה ‎3 גל 1 2020 של Project Service Automation
הנושא מדגיש את השיקולים המרכזיים לשדרוג בעת המעבר למהדורה האחרונה של Project Service Automation‏ (PSA) גירסה ‎ 3.xגל 1 2020.

## <a name="time-entry"></a>ערך זמן
החוויה של הכנסת ערך הזמן הורחבה כדי לספק יכולות להארכת ערכי הזמן לתרחישים רבים יותר של לקוחות. זה כולל את היכולת להוסיף סוגי ערכים, מה שמניע כעת התנהגות ספציפית על סמך שם סכימת השדה **הגדרות ערך זמן** , שמוצג בתור **מקור זמן**. פתרון חדש, שנקרא 'זמן, הוצאה, סטטוס ואישורים' (TESA) נוסף לתמיכה בפונקציונליות זו.

### <a name="upgrade-consideration"></a>שיקולים לגבי שדרוג
כדי לתמוך בפונקציונליות זו, התפקידים בתוך PSA עודכנו כך שהם כוללים הרשאות חדשות. הרשאות אלה מעניקות גישה לקריאה לישות החדשה, **הגדרות ערך זמן**.

משתמשים הזקוקים ליכולת רישום זמן צריכים לקבל את תפקיד המשתמש **משתמש עם ערך זמן** בנוסף לתפקידים הקיימים. תפקיד זה כולל את הפונקציונליות החדשה ומבטיח שערך הזמן ימשיך לעבוד.

בנוסף, אם ברשותך מודולי אפליקציה מותאמים אישית הכוללים את כל הטפסים עבור ישות הזנת הזמן, תידרש להסיר את **טופס ליצירה מהירה של זמן TESA** מהמודול.

### <a name="currently-extended-time-entry-changes"></a>שינויים נוכחיים בערכי זמן מורחבים
כדי למזער את ההשפעה על המשתמשים הנוכחיים בערכי זמן, שינוי תפקיד זה הוא הדרישה המרכזית היחידה הנחוצה כדי להמשיך ולהשתמש בערכי זמן. אם יצרת תצוגות מותאמות אישית או חוויות נפרדות של ערכי זמן, עליך להגדיר את השדות של **הגדרת ערך זמן** לערך ה-PSA הנכון.