---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 25 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 25, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 10/26/2020
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
ms.openlocfilehash: 30822ec64b31e110202a587dd941bdff60116712
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280444"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-25-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 25 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים שהם חדשים או ששונו עבור Project Service Automation V3, מהדורת עדכון 25. לגרסה זו יש מספר Build ‏ V 3.10.43.76 והיא זמינה לכלל ציבור המשתמשים באמצעות עדכון עצמי באוקטובר 2020.

## <a name="update-release-25"></a>הפצת עדכון 25

### <a name="bug-fixes"></a>תיקוני באגים

**זמן והוצאה**

הבעיה הבאה תוקנה:

- תרשים ערכי זמן המציג נתונים נוספים בהתבסס על מרווח גדול מדי של אחזור.

**ניהול משאבים**

הבעיה הבאה תוקנה:

- נוסף קוד Package Deployer כדי לדלג על יצוא התיקון Universal Resource Scheduling אם כבר קיים תיקון בגרסה גבוהה יותר.

**ניהול פרויקט**

הבעיות הבאות תוקנו:

- תוקנו פערים בעיגול ובשער החליפין שגרמו לעלות מתוכננת שגויה ברשת המעקב אחר הפרויקט.
- תומך ביכולת להציג שני רשתות תגובה או יותר בטופס **פרויקט**.
- ניתן אימות לטיפול ביכולת להקצות משימה מעבר לתאריך הסיום של היומן, מה שמביא להקצאת משאבים כושלת.
- טיפול משופר בשגיאות לטיפול בחריגת הפניות Null שנוצרות מהבאים:

    - תוסף **PreValidateProjectTeamMemberCreate**
    - **PreValidateProjectTaskCreate** כאשר נוצרת משימת פרויקט ללא פרויקט משויך
    - תוסף **PreProjectTeamMemberCreate**
    - תוסף **PostProjectTeamMemberCreate**
    - תוסף **PreValidateProjectTaskDelete**

**Sales**

הבעיות הבאות תוקנו:

- טיפול משופר בשגיאות כדי לטפל בחריגות הפניה Null שנוצרות מ **העתקת פרויקט: ניהול הערכות HelperResource**.
- **לא מוכן להפקת חשבונית** ב **מצבור פרטי עבודה של חיוב זמן ומומרים** אינו מנקה את מצב החיוב.
- תוקן שגיאה בתויות לחצני ה **מחירים** בכרטיסיה **מחיר תפקיד** ו **פריטי קטלוג**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]