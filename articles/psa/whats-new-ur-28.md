---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 28 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 28, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/26/2021
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
ms.openlocfilehash: 2c50d6bdc033836e1259a2fd12b78015280d8093
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5150624"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-28-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 28 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים שהם חדשים או ששונו עבור Project Service Automation V3, מהדורת עדכון 28. לגרסה זו יש מספר Build ‏ V 3.10.46.32 והיא זמינה לכלל ציבור המשתמשים באמצעות עדכון עצמי בינואר 2021.

## <a name="update-release-28"></a>הפצת עדכון 28

### <a name="bug-fixes"></a>תיקוני באגים

**זמן והוצאה**

הבעיות הבאות תוקנו:

- משתמשים יכולים להשתמש ב **עריכה בכמות גדולה** לעדכון רשומות זמן שאושרו והוגשו.

**ניהול פרויקט**

הבעיות הבאות תוקנו:

- במקרים שבהם ה-GUID של המשימה נקרא כמספר, לא ניתן לפתוח משימות לעריכה באמצעות **ערוך את המשימה** ברצועת הכלים בדף **מבנה התפלגות עבודה**.

**Sales**

הבעיות הבאות תוקנו:

- חריג של התייחסות null נוצר כאשר יישום plug-in **GetEstimatesForProject** מופעל.
- **סמן מוכן לחשבונית** ברשת אבני הדרך מעדכנת חלקית בלבד את התכונות, למעט המאפיין **InvoiceStatus** שמתעדכן.



[!INCLUDE[footer-include](../includes/footer-banner.md)]