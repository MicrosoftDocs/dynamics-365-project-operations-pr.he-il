---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 31 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 31, עדכון V3 של Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/26/2021
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
ms.openlocfilehash: 2e5fce003c25f9c5911e5a01fb4ec3e19c06c078e00b054472699a522b9cd070
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/06/2021
ms.locfileid: "7002152"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-31-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 31 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 31, עדכון V3 של Project Service Automation. גירסה זו כוללת מספר build של V3.10.52.77 ובדרך כלל היא זמינה דרך עדכון עצמי במאי 2021.

## <a name="update-release-31"></a>הפצת עדכון 31

### <a name="bug-fixes"></a>תיקוני באגים

**זמן והוצאה**

הבעיות הבאות תוקנו:

- לחצני פקודה לערכי זמן בדף **משאבים הניתנים להזמנה** היו מבלבלים.
- נוצר חריג הפניה null ב **Project.SetTrackingFields** באישור ערך זמן.

**ניהול משאבים**

הבעיות הבאות תוקנו:

- **צור חבר צוות** אינו מציג כראוי את הגדרת המטא נתונים של הגדרת ההזמנה עבור **מצב ברירת המחדל 'מוקצה'**.
- בעת השדרוג מ- PSA 1.X ל- X‏.3, תהליך השדרוג נכשל ב-**UpgradeResourceRequirements**.


**מכירות**

הבעיות הבאות תוקנו:

- הכנסות בפועל ממירות את הסכומים למטבע הפרויקט ברשת המעקב.
- ברירת המחדל של המטבע אינה ברורה בעת יצירת שורות יומן, שורות הצעות מחיר וסעיפי חוזה בתרחישים שבהם מטבע הבסיס של הארגון שונה ממטבע הפרויקט.
- **ממתין לאימות יומן התיקון** שאילתה אינה מסננת לפי פרויקט.
- המכירות הנותרות מחושבות באופן שגוי בפרויקט.
- הצעות מחיר המבוססות על איש קשר נכשלות כאשר הן נוצרות ללא מחירון.
- לא מופיע מחוון התקדמות לעיבוד בעת הבחירה באפשרות **אשר חשבונית**.
- לא מופיע מחוון התקדמות בעת הבחירה באפשרות **צור חשבונית**.
- סגירת הצעת מחיר כאבודה אינה מבטלת את ההזמנות.







