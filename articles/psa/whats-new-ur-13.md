---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 13 V3
description: נושא זה מספק מידע על מה חדש בעדכון המהדורה 13, V3 של Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: eb935d5bf3d2deb95db420f20a8102dae1864515
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8596157"
---
# <a name="project-service-automation-update-release-13-v3"></a>מהדורה 13, V3 של Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור יישום Dynamics 365 Project Service Automation‏ (PSA). מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 13, עדכון V3 של Project Service Automation. מספר ה-Build של גרסה זו הוא V3.10.3.18 והיא זמינה בלוח הזמנים הבא:

- **זמינות כללית (עדכון עצמי):** נובמבר 2019
- **עדכון עצמי:** דצמבר 2019


## <a name="update-release-13"></a>הפצת עדכון 13 

### <a name="bug-fixes"></a>תיקוני באגים

- זמן והוצאה

     - קבוע: פונקציונליות חיפוש בדף **אישור הוצאה** אינו פועל בעת חיפוש לפי מטרת ההוצאה.

- ניהול משאבים

     - קבוע: המספרים בהתאמה עודכנו כמיושרים לימין.
     - קבוע: לא ניתן להקצות משאבים עם שם למשימות דרך הכרטיסיה **לוח זמנים**.

- ניהול פרויקט

     - קבוע: חריגה מערך Null בעת הקצאת חבר צוות כאשר בערך **TransactionType‎** חסרים נתוני התקנה עבור **יחידה** ו- **DefaultGroup**.

- Sales

     - קבוע: רשומות מסוג עסקאות כפולות מחזירות שגיאה בעת יצירת רשומות של מחיר תפקיד.
     - תוקן: לחצנים נוספים עבור **הזדמנות חדשה**, **הצעת מחיר**, **שורת הזמנה**, ו **הוסף מוצר** גלויים בפקודות עבור הזדמנויות, הצעות מחיר, הזמנת מוצרים ורשת המשנה של שורות מבוססות פרויקט.




[!INCLUDE[footer-include](../includes/footer-banner.md)]
