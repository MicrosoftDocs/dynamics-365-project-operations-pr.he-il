---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 15 V3
description: נושא זה מספק מידע על מה חדש בעדכון המהדורה 15, V3 של Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/27/2020
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
ms.openlocfilehash: 26b9ee0a6ff1ad81d6c77a6a7091733667c493ff
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8585149"
---
# <a name="project-service-automation-update-release-15-v3"></a>מהדורה 15, V3 של Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור יישום Dynamics 365 Project Service Automation‏ (PSA). מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 15, עדכון V3 של PSA. מספר ה-build של גירסה זו הוא V3.10.5.28 והיא זמינה דרך עדכון עצמי החל מינואר 2020.

## <a name="update-release-15"></a>הפצת עדכון 15 

### <a name="enhancements"></a>שיפורים

- ניהול פרויקט

### <a name="bug-fixes"></a>תיקוני באגים

- זמן והוצאה

  - תוקן: נוסף טיפול בשגיאות בעומס בתצוגת ההתאמה.
  - תוקן: מרכז משאבי הפרויקט: שינוי שם **כמות** כדי להפחית את העמימות.
  - תוקן: התאמת התצוגה **העתקת עמודות של ערכי זמן** כדי לכלול את הסוג.
  - תוקן: עריכת משך הזנת זמן בתצוגת הרשת באמצעות מספרים עשרוניים מביאה לשגיאה לא ידועה עבור מספרים מסוימים.

- ניהול פרויקט

  - תוקן: התפריט הנפתח עבור **השתמש בתצוגת מעקב** כעת מתרחב על סמך רוחב האפשרויות.
  - תוקן: בעת ניהול פרויקטים באזור הזמן +13, חישובי משימות יכולים להציג תוצאות לא מדויקות.
  - תוקן: **זמן סיום של חבר צוות** תוקן בעת שימוש בלוח השנה הפתוח 24 שעות ביממה.
  - תוקן: הפעלה מחדש של **BPF** בטופס הראשי **msdyn_project**.
  - תוקן: חישוב המשימות כבר לא מתעלם מיום אחד.
  - תוקן: באנר התראות חדש נוסף לטופס הפרויקט כאשר אזור הזמן של המשתמש שונה מזה של הפרויקט.

- Sales

  - תוקן: ניתן להשתמש בחיפוש קטגוריות לאומדן הוצאות לצורך סינון כפילויות.
  - תוקן: הקוד ב- **PluginDomain.ExecuteInTryCatchBlock (..)** כבר לא מסתיר את מקור החריגה.
  - תוקן: כבר לא מקבלים הודעת שגיאה בזמן **חיפוש פרויקט** בטופס **שורת הצעת מחיר** כשיש יותר מ- 1000 פרויקטים.
  - תוקן: רשת **הערכות** לאומדני עבודה ואומדני הוצאות מציגה כעת את סמל המטבע הנכון.
  - תוקן: לאחר שארגון מעדכן את PSA מעדכון מהדורה 14 לעדכון מהדורה 15, הכרטיסיה **לוח זמנים** כבר לא מופיעה ריקה בטופס **פרויקט**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
