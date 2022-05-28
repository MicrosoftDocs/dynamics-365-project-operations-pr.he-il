---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 40 V3
description: נושא זה מפרט את התכונות והתיקונים הזמינים ב- Microsoft Dynamics 365 Project Service Automation מהדורת עדכון 40, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/31/2022
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
ms.openlocfilehash: 25f375ce648eb7d233f6433739832caee351830d
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8588645"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-40-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 40 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור האפליקציה Microsoft Dynamics 365 Project Service Automation. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. הוא תואם ל- Dynamics 365 9.x. לעדכון למהדורה זו, בקר בדף הפתרונות המקוון של מרכז הניהול עבור Dynamics 365 והתקן את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 40, עדכון V3 של Project Service Automation. לגרסה זו יש מספר build של V3.10.61.61 והיא זמינה בדרך כלל באמצעות עדכון עצמי בפברואר 2022.

## <a name="update-release-40"></a>הפצת עדכון 40

### <a name="features"></a>תכונות
שלב 1 של השדרוג מ- Project Service Automation ל-Project Operations ‏- Lite יופץ בפברואר 2022 לכל הלקוחות. כדי לבדוק זכאות, ראה [שדרוג מ- Project Service Automation ל- Project Operations](upgrade-project-operations-non-stocked.md). אם היישום אינו מופיע במופע שלך במרכז הניהול של Power Platform, פנה לתמיכה ובקש הפעלה של הטיסה עבור הסביבות שלך. על הבקשה לכלול רשימת מזהי סביבות שבהן יש צורך להפעיל את הטיסה.

### <a name="bug-fixes"></a>תיקוני באגים

הבעיות הבאות תוקנו.

**זמן והוצאה**
- חסרה רשומת הערה כאשר נדחית או מבוטלת רשומת זמן. 

**מכירות**

- בעת עדכון הערכות עלות או מכירות באמצעות יישומי plug-in מוכנים לשימוש, אתה מקבל הרשאה שגויה לשלוח פריטי תוכן מנה של JSON שאינם תקפים מחוץ לממשק המשתמש.
- בעת עדכון של שורות הצעת מחיר באמצעות התצוגה המהירה, אתה רשאי להפעיל הצעות מחיר.
