---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 34 V3
description: מאמר זה מפרט את התכונות והתיקונים הזמינים בעדכון Project Service Automation מהדורה 34, גרסה 3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 08/05/2021
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
ms.openlocfilehash: e47a5442f285952c165a2d30e337a362a6b065dd
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8928663"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-34-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 34 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור האפליקציה Microsoft Dynamics 365 Project Service Automation. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. הוא תואם ל- Dynamics 365 9.x. לעדכון למהדורה זו, בקר בדף הפתרונות המקוון של מרכז הניהול עבור Dynamics 365 והתקן את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

מאמר זה מפרט את התכונות והתיקונים החדשים או ששונו בעדכון Project Service Automation גרסה 3, מהדורה 34. גרסה זו כוללת מספר build של V3.10.55.38 והיא זמינה בדרך כלל באמצעות עדכון עצמי ביולי 2021.

## <a name="update-release-34"></a>הפצת עדכון 34

### <a name="bug-fixes"></a>תיקוני באגים
הבעיות הבאות תוקנו.

**כללי**

- עדכונים מונעי אתרים אינם מפעילים את זרימת העבודה החדשה והמודרנית לאישור.
- התכונות **סטטוס יעד** ו- **סוג פעולה** חסרות בעמוד הראשי של **ערכת אישור**.

**זמן והוצאה**

- לא ניתן לאשר בקשה לאחזור באמצעות זרימת האישור המודרנית.
- העתקת רשומות של שבוע אינה פועלת בעת העתקת ערכים שאינם קשורים למשתמש המחובר.

**תכנון פרוייקטים**

- קווי המתאר של הקצאת משאבים נפגמים בעת ייבוא מתוסף שולחן העבודה של Microsoft Project.

**ניהול משאבים**

- כאשר אתה מפרסם פרוייקט מהתוסף של לקוח שולחן העבודה של Microsoft Project, תאריך הסיום של הדרישות הקיימות משתנה.
- הדיוק העשרוני עולה על שני מקומות עשרוניים בתיבת הדו -שיח לאישור הארכת הזמנות.

**מכירות**

- כאשר אתה מוסיף שורה מבוססת מוצר עם מוצר קיים לחוזה פרוייקט, מוצגת החריגה **מפתח לא נמצא במילון**.
- לא ניתן להכשיר הפניות כאשר סוג הזמנה ממופה מהפניה להזדמנות.
