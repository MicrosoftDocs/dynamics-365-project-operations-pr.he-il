---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 41 V3
description: נושא זה מפרט את התכונות והתיקונים הזמינים ב- Microsoft Dynamics 365 Project Service Automation מהדורת עדכון 41, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 03/07/2022
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
ms.openlocfilehash: 649d8bca36fda0a09dc7230ee4d742cadb32f3b3
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8580917"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-41-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 41 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור האפליקציה Microsoft Dynamics 365 Project Service Automation. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. הוא תואם ל- Dynamics 365 9.x. לעדכון למהדורה זו, בקר בדף הפתרונות המקוון של מרכז הניהול עבור Dynamics 365 והתקן את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 41, עדכון V3 של Project Service Automation. מספר גירסת build של גירסה זו הוא V3.10.62.162 ובדרך כלל היא זמינה באמצעות עדכון עצמי החל ממרץ 2022.

## <a name="update-release-41"></a>הפצת עדכון 41

### <a name="bug-fixes"></a>תיקוני באגים

הבעיות הבאות תוקנו.

**ניהול פרויקט**
- כאשר אתה מנסה ליצור פרוייקט מתבנית המבוססת על פרוייקט שנוצר מהתוספת של שולחן העבודה, מוצגת השגיאה הבאה, "אימות השדה 'עבודה מתוכננת' של הקצאת משאבים: תאריך הסיום של כל פרוסת זמן של הקצאת משאבים לא יכול להיות מוקדם יותר מאשר תאריך ההתחלה".

**זמן והוצאה**
- כאשר אתה מנסה למחוק רשומת זמן, תוצג הודעת השגיאה הבאה: "אירעה שגיאה בלתי צפויה מקוד ISV".

**מכירות**
- כאשר אתה יוצר חשבונית עבור אבן דרך במחיר קבוע, השדות **תיאור** ו **תיאור חיצוני** אינם מאוכלסים. 
