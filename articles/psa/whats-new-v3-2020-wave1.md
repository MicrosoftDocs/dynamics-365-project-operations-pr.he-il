---
title: מה חדש או השתנה בגירסה ‎3.x wave 1 2020 של Project Service Automation
description: מאמר זה מספק מידע על הדברים החדשים והדברים שהשתנו ב- Project Service Automation גירסה 3, גל הפצה 1 2020.
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
ms.reviewer: johnmichalak
ms.openlocfilehash: c762f2e7931046d32464cfa8486ef8405aa7d836
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8928617"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3-wave-1-2020"></a>מה חדש או השתנה בגירסה ‎3 גל 1 2020 של Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

המאמר מדגיש את שיקולי השדרוג העיקריים בעת מעבר למהדורה האחרונה של Project Service Automation (PSA)‎‏‏‏‎‏‏ גרסה ‎3.x גל 1‏, 2020.

## <a name="time-entry"></a>ערך זמן
החוויה של הכנסת ערך הזמן הורחבה כדי לספק יכולות להארכת ערכי הזמן לתרחישים רבים יותר של לקוחות. זה כולל את היכולת להוסיף סוגי ערכים, מה שמניע כעת התנהגות ספציפית על סמך שם סכימת השדה **הגדרות ערך זמן**, שמוצג בתור **מקור זמן**. פתרון חדש, שנקרא 'זמן, הוצאה, סטטוס ואישורים' (TESA) נוסף לתמיכה בפונקציונליות זו.

### <a name="upgrade-consideration"></a>שיקולים לגבי שדרוג
כדי לתמוך בפונקציונליות זו, התפקידים בתוך PSA עודכנו כך שהם כוללים הרשאות חדשות. הרשאות אלה מעניקות גישה לקריאה לישות החדשה, **הגדרות ערך זמן**.

משתמשים הזקוקים ליכולת רישום זמן צריכים לקבל את תפקיד המשתמש **משתמש עם ערך זמן** בנוסף לתפקידים הקיימים. תפקיד זה כולל את הפונקציונליות החדשה ומבטיח שערך הזמן ימשיך לעבוד.

בנוסף, אם ברשותך מודולי אפליקציה מותאמים אישית הכוללים את כל הטפסים עבור ישות הזנת הזמן, תידרש להסיר את **טופס ליצירה מהירה של זמן TESA** מהמודול.

### <a name="currently-extended-time-entry-changes"></a>שינויים נוכחיים בערכי זמן מורחבים
כדי למזער את ההשפעה על המשתמשים הנוכחיים בערכי זמן, שינוי תפקיד זה הוא הדרישה המרכזית היחידה הנחוצה כדי להמשיך ולהשתמש בערכי זמן. אם יצרת תצוגות מותאמות אישית או חוויות נפרדות של ערכי זמן, עליך להגדיר את השדות של **הגדרת ערך זמן** לערך ה-PSA הנכון.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
