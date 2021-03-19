---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 19 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 19, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 05/05/2020
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
ms.openlocfilehash: b9baeca9e79e233c25a6310e426d755b9162bbad
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280714"
---
# <a name="project-service-automation-update-release-19-v3"></a>מהדורה 19, V3 של Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 19, עדכון V3 של PSA. גירסה זו כוללת מספר build של V3.10.30.41 ובדרך כלל היא זמינה דרך עדכון עצמי במאי 2020.

## <a name="update-release-19"></a>הפצת עדכון 19

### <a name="bug-fixes"></a>תיקוני באגים

**זמן והוצאה**

הבעיות הבאות תוקנו: 

- שגיאות שנגזרות מייבוא של ערכי זמן שלא הוצגו כראוי.
- רשת הזנת זמן אינה תומכת בהתנהגות שדה **תאריך בלבד**.
- משאבי פרויקט אינם יכולים ליצור הוצאה בפרויקט.

**ניהול פרויקט**

הבעיות הבאות תוקנו: 

-  משימת נכד גורמת לאומדן מאמץ שגוי במהלך חישוב ההשלמה (EAC).

**Sales**

הבעיות הבאות תוקנו: 

- הפעולה **חישוב מחדש** לא עובדת עם פרטי סעיף חוזה הוצאות או פרטי שורה בהצעות מחיר.
- **עדכן מחירים** חסר לאומדני הוצאות.
-  לקוחות אינם יכולים לבחור סיבות מותאמות אישית למצב חוזה מהדף **חוזה של פרויקט**.
- לקוחות חווים ביצועים פחות טובים בעת יצירת מחירון מותאם אישית מהצעת מחיר.
- לקוחות חווים חוסר עקביות עם ברירת מחדל של **יחידה** בדפים **פרטי סעיף בהצעת מחיר** ו- **פרטי סעיף בחוזה**.
- הוספת פריטים בקטגוריית עסקאות שלא ניתן לחייב לסעיף חוזה הניתן לחיוב לא תכבד את סוג החיוב **ללא חיוב** של קטגוריית העסקה.
- לקוחות אינם יכולים להשתמש בתפקידים ובקטגוריה בחוזים שנוצרו בעבר.
- לקוחות חווים ביצועים גרועים ואחזור מיותר ב- PreValidateProjectTeamMemberUpdate.cs
- יש להוסיף תפקידים שהוגדרו ככאלו שאינם חייבים בתשלום ברשימה **קטגוריות משאבים** לכרטיסיה **תפקידים שניתנים לחיוב** כ- **לא לחיוב** בסעיף החוזה של פרויקט.
- לקוחות עשויים לחוות ביצועים גרועים בעת יצירת פרויקט מכיוון ש- **GetBookableResourceIdFromUser** מאחזר את כל העמודות של משאבים שניתנים להזמנה במקום רק את המזהה הראשי.
- בישות **TransactionType** חסר יישום plug-in לעדכון אימות מראש כדי למנוע ממשתמשים להזין **יחידות** ו- **UnitGroups** שאינן חוקיות לסוגי הטרנזקציות.
- השלב **הסר** אינו פועל לייבוא ערך זמן.


[!INCLUDE[footer-include](../includes/footer-banner.md)]