---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 28 V3
description: מאמר זה מפרט את התכונות והתיקונים הזמינים בעדכון Project Service Automation מהדורה 28, גרסה 3.
author: ruhercul
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
ms.reviewer: johnmichalak
ms.openlocfilehash: 56a87bce55c560e541e20709b10d38b9512ffcee
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8930595"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-28-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 28 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

מאמר זה מפרט את התכונות והתיקונים שהם חדשים או השתנו עבור Project Service Automation גרסה 3, עדכון מהדורה 28 מספר Build של גרסה זו הוא V3.10.46.32 והיא זמינה לכלל המשתמשים באמצעות עדכון עצמי בינואר 2021.

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
