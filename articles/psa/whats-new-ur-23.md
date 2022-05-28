---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 23 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 23, עדכון V3 של Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 08/25/2020
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
ms.openlocfilehash: cc918f1516d4751b3f8e70a93d8fc66058201f22
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8581607"
---
# <a name="project-service-automation-update-release-23-v3"></a>מהדורה 23, V3 של Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 23, עדכון V3 של Project Service Automation. מספר ה- Build של גירסה זו הוא V 3.10.34.30 והיא זמינה דרך עדכון עצמי החל מאוגוסט 2020.

## <a name="update-release-23"></a>הפצת עדכון 23

### <a name="bug-fixes"></a>תיקוני באגים

**זמן והוצאה**

הבעיות הבאות תוקנו:
- טפל במקרי קצה ב **מחיקת חבר צוות פרויקט** כדי לספק חריגה משמעותית.
- ייבוא משימות גורם למסך הסרה ריק.

**ניהול משאבים**

הבעיות הבאות תוקנו:

- **כרטיס משאב רשת ניצול משאבים** מציג נתונים שגויים כאשר ציר הזמן הוא יותר מחמישה ימים.
- כאשר לקוחות יוצרים משאב שניתן להזמין, יישום ה-plug-in אינו מצליח להוסיף את המשאב באופן אוטומטי לקבוצה של Microsoft Office 365.
- תצוגת **יישוב‬** מציגה קווי מתאר ידניים בצורה לא נכונה בתצוגה **שבוע** או **חודש**.

**ניהול פרויקט**

הבעיות הבאות תוקנו:

- מספר מוגזם של ישויות **RetrieveMultiple for usersettings** גורם לביצועים נמוכים של אישורי פרויקט ופעולות אחרות.
- חיפוש המשאבים ברשת של **תכנון משימות** מוגבל להצגה של עד חמישה חברי צוות בלבד מצוות הפרויקט. 
- חיפוש המשאבים ברשת של **תכנון משימות** אינו מסנן משאבים לא פעילים.
- מצב ידני אינו פועל כצפוי במבנה פירוט העבודה של תכנון הפרויקט.
- הרשת **תכנון משימות** מציגה **קטגוריות עסקאות לא פעילות**.
- הרשת **הקצאת משאבים** מעגלת בצורה שגויה כאשר למשימה יש מספר מטלות.
- ערכי העיגול שונים בעלות מתוכננת ובעלות בפועל עבור משימה אחת.

**Sales**

הבעיות הבאות תוקנו:

- **אחזר את כל קטגוריות העסקה** לחיצה כפולה יוצרת מספר שורות.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
