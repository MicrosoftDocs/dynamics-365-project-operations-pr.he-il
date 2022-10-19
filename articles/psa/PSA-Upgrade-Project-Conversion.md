---
title: תהליך המרה של תזמון פרוייקטים ב- Project Service Automation לתזמון ב- Project Operations
description: מאמר זה מספק סקירה כללית של השינויים בתכונות עבור Microsoft Dynamics 365 Project Service Automation Project Service Automation ל- Dynamics 365 Project Operations.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 10/07/2022
ms.topic: article
ms.author: ruhercul
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
ms.openlocfilehash: 84a40fcc9a8561c4ade0be175b08f701f3196508
ms.sourcegitcommit: 28004d38800782540fa5642d41f8fe0f6e2d9fa5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/08/2022
ms.locfileid: "9642569"
---
# <a name="project-service-automation-to-project-operations-project-scheduling-conversion-process"></a>תהליך המרה של תזמון פרוייקטים ב- Project Service Automation לתזמון ב- Project Operations

לאחר שפרויקט שודרג בהצלחה מ- Microsoft Dynamics 365 Project Service Automation 3.X ל- Dynamics 365 Project Operations Lite, לא ניתן לערוך משימות פרויקט במבנה התפלגות העבודה  (WBS) של רשת המשימות. לקוחות יוכלו לסקור את מבני ה- WBS ברשת המעקב שבה נוספו שדות חדשים כדי לספק את כל הפרטים הקשורים למשימה. עבור פרויקטים שבהם נדרשות עריכות ל- WBS, אתה יכול להמיר באופן סלקטיבי פרויקטים כשירים לפרויקט החדש עבור חוויית תזמון ב- Projects for the Web.

## <a name="project-conversion-process"></a>תהליך המרת פרויקט

כדי להמיר פרויקט, בצע את השלבים הבאים.

1. פתח את העמוד הראשי של הפרויקט ובחר **המר** בחלונית הפעולה.
1. בתיבת הודעת האישור שמופיעה, בחר **אישור** כדי להתחיל את המרת הפרויקט. הפעולות הבאות מתרחשות:

    1. שורת הודעות שמופיעה בעמוד הראשי של הפרויקט מציינת, "לוח הזמנים של הפרויקט עובר המרה. לא ניתן לבצע שינויים בפרויקט עד להשלמת ההמרה."
    1. אתה מנותב לרשימת הפרויקטים.

    לאחר השלמת המרת הפרויקט, מתרחשות הפעולות הבאות:

    1. מנהל הפרויקט שהוקצה מקבל הודעה בצד שמאל של האפליקציה.
    1. סרגל ההודעות שמציין שההמרה מתבצעת מוסר.
    1. הכרטיסיה **לוח זמנים** מציגה את חוויית התזמון החדשה עם Project for the Web. כל משתמש עם הרישיונות ותפקידי האבטחה המתאימים יכול לערוך את ה- WBS.
    1. השדה **מנוע תזמון** מעודכן ל- **Project for the Web**.
    1. הלחצן **המר** הלחצן מחלונית הפעולה.

> [!IMPORTANT]
> המרה בצובר של פרויקטים אסורה. כל ניסיון לעדכן נפח גדול של פרויקטים בו-זמנית יווסת. מגבלה זו עוזרת להבטיח ביצועים גבוהים עבור כל הלקוחות.

## <a name="manual-tasks-vs-automatic-tasks"></a>משימות ידניות לעומת משימות אוטומטיות

כאשר סביבה משודרגת מ- Project Service Automation ל- Project Operations, כל המשימות ב- WBS נחשבות למשימות שתוזמנו אוטומטית. הרעיון של משימות מתוזמנות באופן ידני אינו זמין ב- Project for the Web. עם זאת, אתה יכול להגדיר את אופן הפעולה המועדף לתזמון עבור הפרויקטים שלך על ידי שימוש בהגדרה [מצב תזמון](/project-management/scheduling-modes.md) בעת יצירת פרויקטים חדשים.

## <a name="restricted-operations-for-pre-conversion-projects"></a>פעולות מוגבלות עבור פרויקטים של טרום המרה

מקטע זה מתאר את ההבדלים הפונקציונליים שניתן לצפות להם כאשר פרויקטים לא הומרו.

### <a name="copy-project"></a>העתק פרוייקט

הפעולה **העתק** נתמכת רק בפרויקטים שהומרו. לא ניתן להעתיק פרויקטים משודרגים לפני ההמרה.

### <a name="move-project"></a>העבר פרוייקט

שינוי בתאריך ההתחלה של פרויקט לא יעביר באופן פרופורציונלי את תחילת המשימות אלא אם הפרויקט הומר.

## <a name="frequently-asked-questions"></a>‏‫שאלות נפוצות‬

### <a name="what-are-the-differences-between-converted-projects-and-new-projects-that-are-created-after-the-upgrade-has-been-completed"></a>מה ההבדלים בין פרויקטים שהומרו לפרויקטים חדשים שנוצרים לאחר השלמת השדרוג?

עבור פרויקטים שהומרו לאחר שדרוג הסביבה, יוגדר דגל המורה ללוח הזמנים לכבד רק את לוח השנה של הפרויקט. אופן פעולה זה תואם לאופן הפעולה באוטומציה ב- Project Service Automation. עם זאת, הדגל לא יוגדר עבור פרויקטים חדשים שנוצרו לאחר השדרוג. לכן, לוח הזמנים יכבד את שעות העבודה של משאבים כאשר הם מוקצים למשימה.

### <a name="what-should-i-do-if-my-project-fails-to-be-converted"></a>מה עלי לעשות אם המרת הפרויקט שלי נכשל?

אם המרת הפרויקט שלך נכשל, הצעד הראשון הוא לסקור את יומני השגיאות כדי לזהות בעיות נפוצות הקשורות ל- WBS שלך. אם היומנים אינם מציינים שגיאה ספציפית שתוכל לנקוט בפעולה לגביה, צור קשר עם שירות הלקוחות כדי לאפשר בידקה נוספת של האירוע שלך.

### <a name="how-are-business-closures-handled-in-project-for-the-web"></a>כיצד מטופלים במועדי סגירות עסקים ב- Project for the Web?

Project for the Web אינו מכבד מועדי סגירת עסקים שהארגון מגדיר ברמת הארגון. עם זאת, הוא יכבד סוגים אחרים של ימי חופש המוגדרים בתבנית שעת עבודה נתונה.

### <a name="what-are-the-limitations-of-project-for-the-web"></a>מהן המגבלות של התכונה Project for the Web?

עיין ב[יצירת מבנה התפלגות עבודה: מגבלות הפרויקט](/project-management/create-wbs#project-limitations.md).

### <a name="can-i-expect-changes-to-my-cost-and-sales-estimates"></a>האם אוכל לצפות לשינויים בהערכות של העלויות והמכירות שלי?

במקרים נדירים שבהם קווי המתאר של הקצאת משאבים מחושבים מחדש, או כשהם הם נופלים על גבול תאריך שונה מזה שבפרויקט המקור, ייתכן שתראה הבדלים בהערכות של המכירות והעלות. כחלק מתהליך השדרוג, אנחנו מצפים מלקוחות לבדוק קבוצת מדגם מייצג של פרויקטים, על מנת שיוכלו להבין כל שינוי פוטנציאלי בלוח הזמנים.
