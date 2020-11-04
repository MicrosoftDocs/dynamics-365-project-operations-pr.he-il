---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 20 V3
description: סעיף זה מפרט את התכונות החדשות והתיקונים במהדורה 20, עדכון V3 של Project Service Automation
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 06/12/2020
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
ms.openlocfilehash: 12edae76dbc6de63d3e2d36058c4092f80ede77d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077257"
---
# <a name="project-service-automation-update-release-20-v3"></a>מהדורה 20, V3 של Project Service Automation

אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 20, עדכון V3 של Project Service Automation. גירסה זו כוללת מספר build של V3.10.31.37 ובדרך כלל היא זמינה דרך עדכון עצמי ביוני 2020.

## <a name="update-release-20"></a>הפצת עדכון 20

### <a name="bug-fixes"></a>תיקוני באגים

**ניהול פרויקט**

הבעיות הבאות תוקנו:

- ייבוא חברי צוות הפרויקט בשיטת הקצאה הדורשת שעות גורם להודעת שגיאה לא ברורה כאשר השעות שצוינו הן אפס.
- משתמשים מקבלים שגיאה לא נכונה כאשר מספר התווים המרבי הוזן לשדה **תיאור** של משימת פרויקט.
- הדף **הורדת תוספת Microsoft Dynamics 365 Project Service Automation** מפנה לדף ההורדה באנגלית כאשר השפה של המשתמש מוגדרת ליפנית.
- כאשר מתרחשת שגיאת שרת, תווית הסנכרון בכרטיסיה **לוח זמנים** בטופס **פרויקטים** לפעמים נשארת.
- עדכוני משימות מיותרים נשלחים לשרת עם שינוי המשימה.

**Sales**

הבעיות הבאות תוקנו:

- בטופס **חוזה** , לחיצה כפולה על **צור חשבונית** יוצרת שתי חשבוניות עבור רשומה יחידה.
- ב- Internet Explorer 11, המשתמשים אינם יכולים ליצור ערכי הוצאות.
- ביטול עלות והיפוך של פעולות מכירה שלא חויבו אינן קשורות.
- הלחצן **רענן פעולות** בטופס **פרויקט** לא מרענן **שעות משימה בפועל**.
- יישום plug-in **PreValidateProjectTeamMemberCreate** יכול ליצור משאבים כפולים שניתנים להזמנה כאשר התכונה **msdyn_isgenericresourceprojectscoped** מוגדרת **False**.
- **חישוב מחדש** מנקה עלויות שניתנות לחיוב של פרטי שורה בהצעות מחיר ופרטי סעיף חוזה.
- בתרחישים ספציפיים, יישום plug-in **PostEstimateLineUpdate** מציג שגיאת חריגה null.
- משך שלב זמן ב- **תרשים ניתוח רווחיות** אינו תואם את המשך של עלויות בפרטי שורה בהצעת המחיר במחיר קבוע של הצעת המחיר.
- ערכי יחידות וקבוצת יחידות אינם חוזרים לברירת המחדל כראוי עבור קטגוריות הוצאות בטפסים **פרטי סעיף חוזה** ו- **פרטי סעיף בהצעת מחיר**.
- רשימות **מחיר עלות יחידה ארגונית** מאפשרות חפיפה בתאריך.
- משתמשים אינם רשאים לשנות את **OrgUnit** כאשר סוג ההזמנה אינו מבוסס עבודה מכיוון שהוא יוביל לשגיאת חריגה null.
- כאשר מנסים לנווט מהטופס **פרטי סעיף הצעת מחיר** , חזרה אל הכרטיסיה **הצעת מחיר** , הטופס מרענן ומציג את הכרטיסיה **סיכום**.