---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 24 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 24, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 10/02/2020
ms.topic: article
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
ms.openlocfilehash: 6c8348e65307f63a251f97bf1ea17578e7026da8
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077260"
---
# <a name="project-service-automation-update-release-24-v3"></a>מהדורה 24, V3 של Project Service Automation

אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 24, עדכון V3 של Project Service Automation. מספר ה- Build של גירסה זו הוא V 3.10.42.43 והיא זמינה דרך עדכון עצמי החל מאוקטובר 2020.

## <a name="update-release-24"></a>הפצת עדכון 24

### <a name="bug-fixes"></a>תיקוני באגים

**Sales**

הבעיות הבאות תוקנו:

- בעיה בעת הגדרת מחירון ברירת המחדל של מוצרים.
- הביצועים של זכייה בהצעת מחיר הם איטיים בגלל מחירון מוטבע ועותק של רשומות מחיר-תפקיד‬.
- **חוזה פרויקט/מרכז המכירות** > **פריט שורת מוצרים/כמות שורות הזמנה** מעוגל אוטומטית למספר השלם הקרוב ביותר.
- הרם להרשאות מערכת בעת קריאת מחירונים.
- העתק את שדות כתובת הלקוח **address1_freighttermscode** ו- **address1_shippingmethodcode** להצעת מחיר/הזמנה. 


**זמן והוצאה**

הבעיות הבאות תוקנו:

- **רשת ערכי הזמן** לא תומכת בהתנהגות זמן של **תאריך בלבד** .
- **ערך זמן** אינו מתרענן אוטומטית. נדרש רענון ידני.
- לא ניתן לייבא את רשומות ערכי הזמן ממשימה כשיש הפסקה (0 שעות) בהקצאות המשאב.
- בעת יצירת ערך זמן, הגדר את ההתחלה שתהיה דומה ל- **msdyn_date**.
- הפעל מחדש עריכה בכמות גדולה לערכי זמן.

**ניהול משאבים**

הבעיות הבאות תוקנו:

- ניסיון לעדכן את סטטוס ההזמנה בין הימים ללא דרישה יגרום לחריגה של ref-null.
- שגיאה בטעינת **תצוגת יישוב**.


**ניהול פרויקט**

הבעיות הבאות תוקנו:

- ב **לוח הזמנים של הפרויקט** , בעת שינוי מ **ידני** ל **אוטומטי** , שמירה אוטומטית לא מסתיימת.
- עלויות ההוצאות לא צריכות לחשב את השונות ב **רשת מעקב אחר פרויקטים**.
- התנהגות לא עקבית של עמודות **הערכת תג** במהלך עומס לעומת שינוי בסוג **יחידות זמן עבודה**.
- העלות בפועל בפרויקט עשויה שלא לשקף את הסכומים הכוללים **נתונים בפועל**.
- **תאריך סיום משוער** בכרטיסיה **סיכום** אינו תואם את **לוח הזמנים של WBS**.
- **עדכן שעות בפועל** ב-outdent לא עובד כראוי.
- מנהל פרויקט מחוץ ל- **BU** הבסיסי לא יכול ליצור פרויקט.
- שינויים במשימה או בקטגוריה של **אומדני הוצאות** אינם נשמרים.
- **העתק החוזה** מעתיק את לוחות הזמנים של החשבונית ואת סטטוס הריצה.
- הלחצן **רענן את הנתונים בפועל** מחשב באופן שגוי משימות סיכום.
- תוספת של Microsoft Project: תקן שגיאת התייחסות null אם לחבר צוות כלשהו יש יחידת משאבים ריקה.
