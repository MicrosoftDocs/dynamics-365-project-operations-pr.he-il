---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 29 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 29, עדכון V3 של Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/22/2021
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
ms.openlocfilehash: 56cf47d207c7ee518d5d4b53866c3d6ddf1d1fb3
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8587219"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-29-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 29 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 29, עדכון V3 של Project Service Automation. לגרסה זו יש מספר build של V3.10.47.7 והיא זמינה בדרך כלל באמצעות עדכון עצמי בפברואר 2021.

## <a name="update-release-29"></a>הפצת עדכון 29

### <a name="bug-fixes"></a>תיקוני באגים

**זמן והוצאה**

הבעיות הבאות תוקנו:

- משתמשים לא יכולים לראות את שעות העבודה המחוברות לימי עבודה שאינם ברשת ערכי הזמן.
- ניתן לערוך רשומות הוצאות מאושרות ברשת.

**ניהול פרויקט**

הבעיות הבאות תוקנו:

- לוגיקה של אימות חסר כדי להבטיח שעות עבודה של הקצאת משאבים לא יכולה להיות שלילית.
- הפעולה המותאמת אישית, **AssignResourcesForTask**, מעדכנת את כל השדות במקום רק שדות שהשתנו.
- בעת העתקת פרויקט בסביבה עם תוספים או תהליכי עבודה הרשומים באירוע **CreateProject**, התכונה **msdyn_bulkgenerationstatus** לא מעודכנת אם הפעולה **CopyWBSToProject** נכשלה.
- כשאתה מרחיב את לוח השנה של הפרויקט, ימי העבודה אינם ממוינים בסדר עולה וגורמים לכמה עדכונים של משימות הפרויקט להיכשל.
- שינוי מנהל הפרויקט בפרויקט קיים מפעיל את ברירת המחדל של הלוגיקה של היחידה הארגונית.

**מכירות**

הבעיות הבאות תוקנו:

- הכרטיסיה **ביצועי חוזה** בדף **חוזה** נכשלת באופן שקט במהלך האתחול כאשר לא קיימים סעיפי חוזה.
