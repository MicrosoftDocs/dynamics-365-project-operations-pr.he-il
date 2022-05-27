---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 26 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 26, עדכון V3 של Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/12/2021
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
ms.openlocfilehash: cebfcd6425f11b74ce6331a093d8d3db3da356a0
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8577283"
---
# <a name="project-service-automation-update-release-26-v3"></a>מהדורה 26, V3 של Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 26, עדכון V3 של Project Service Automation. לגרסה זו יש מספר build של V3.10.44.59 והיא זמינה בדרך כלל באמצעות עדכון עצמי בדצמבר 2020.

## <a name="update-release-26"></a>הפצת עדכון 26

### <a name="bug-fixes"></a>תיקוני באגים

**זמן והוצאה**

הבעיות הבאות תוקנו:

- משתמשים יכולים לשנות את המשימה ברישום זמן שאושר/נשלח.
- שגיאת "הפניה לאובייקט לא מוגדר" בעת שמירת ערך זמן.
- ייבוא ערך זמן מהקצאות משאבים יוצר ערכי זמן עם ערכי DateTime שגויים.
- כאשר גם Project Service Automation וגם Field Service מותקנים, הלחצן **חדש** מופיע פעמיים בסרגל הפקודות עבור ערכי זמן ביישום Field Service.
- עדכונים של התאים **אפשר יחידה** ו **קבוצת יחידות** פועלים כעת ברשת **אומדני הוצאות**.
- הטופס **עדכן עריכה של ערך זמן** כולל **ציר זמן**.
- אישור זמן לערכי זמן שאינם שייכים לפרויקט חוסם את המערכת בעת חיפוש תפקיד מאשר פרויקט.

**ניהול משאבים**

הבעיות הבאות תוקנו:

- נוסף אימות ביישום plug-in **PostProjectCreate** כדי לבדוק דרישה עיקרית לפני יצירת יישום מסוג זה.
- טופס יצירה מהירה **חבר בצוות הפרויקט** יוצר חריגה להפניה null אם שדות מוסרים מהטופס.
- יצירת דרישות למשך 12 שעות מעל לשנה נכשלת.
- שופרה הודעת שגיאה על חריגה עם הפניה null במהלך יצירת דרישת משאב.

**ניהול פרויקט**

הבעיות הבאות תוקנו:

- אימות משופר לטיפול בחריגות עם הפניה null שנוצרו ביישום plug-in **PreProjectUpdate**.
- פרויקטים שפורסמו על ידי התוספת השולחנית של Microsoft Project מוחקים מטלות שלא הוקצו.
- נוסף אימות חדש כאשר הפניה לפרויקט של משימה אינה חוקית עקב חריגה עם הפניה null ביישום plug-in **PreValidateProjectTaskUpdate**.
- רשת חברי הצוות אינה מציגה משימות נפרדות ברשומת חבר הצוות.
- נוספו הודעות אימות והודעות שגיאה חדשות עקב חריגה של הפניה null ביישום plug-in **PreProjectTaskDelete**.

**Sales**

הבעיות הבאות תוקנו:

- בעת בחירת שורה מבוססת פרויקט בהצעת מחיר או חוזה, הלחצן **הצעה** אמור להיות גלוי רק כשבוחרים שורה מבוססת מוצר המשויכת למוצר קיים.
- פיצול הראשה **Create_Product** מהרשאה **Create_ProjectContract**.
- מחיקת שורה בחשבונית גורמת לכשל בהפניה null ב- **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
