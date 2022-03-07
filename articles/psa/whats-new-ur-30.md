---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 30 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 30, עדכון V3 של Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/01/2021
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
ms.openlocfilehash: 3b6b7dba9c2a22587d27006b9972c950fbb454f2
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6010427"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-30-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 30 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution.md).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 30, עדכון V3 של Project Service Automation. גירסה זו כוללת מספר build של V3.10.51.61 ובדרך כלל היא זמינה דרך עדכון עצמי באפריל 2021.

## <a name="update-release-30"></a>הפצת עדכון 30

### <a name="bug-fixes"></a>תיקוני באגים

**זמן והוצאה**

הבעיות הבאות תוקנו:

- שגיאה מתרחשת כאשר אתה יוצר ושומר ערך זמן בדף **יצירה מהירה** אם השדה **תפקיד** מוסר.
- מסנן ערכי הזמן מחיל את אופרטור המסנן השגוי.
- גיליונות זמנים שהועתקו אינם מוצגים אוטומטית בעת בחירה באפשרות **העתק שבוע** בפקד הזנת הזמן.

**ניהול משאבים**

הבעיות הבאות תוקנו:

- בעת הארכת הזמנה, מצב ההזמנה המוקצה להזמנה הבטוחה שגוי. הארכת הזמנה מכבדת את מצב ההזמנה המוגדר בתור **מחויב‬** במטה-נתונים של הגדרת ההזמנה.
- כאשר לא מצוין מצב הזמנה תקף, הודעת השגיאה אינה מותאמת נכון לשפה המקומית.

**ניהול פרויקט**

הבעיות הבאות תוקנו:

- לא ניתן ליצור פרויקטים במטבע אחד ולכלול משימות קשורות במטבע אחר.

**מכירות**

הבעיות הבאות תוקנו:

- בעת העתקת מחירון, המחירים אינם מעודכנים.
- סגירת הצעת מחיר כזכייה נכשלת כאשר לפרט העלות יש ערך עבור מקור.
- בישות **משימת פרויקט**, השם **עלות מוערכת** משתנה לשם **עלות מתוכננת (בסיס)**.
- חריגה עם הפניה ל- null נוצרת בעת יצירה או מחיקה של חשבוניות.
