---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 37 V3
description: נושא זה מפרט את התכונות והתיקונים הזמינים ב- Microsoft Dynamics 365 Project Service Automation מהדורת עדכון 37, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 11/01/2021
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
ms.openlocfilehash: 7bd00ccbb09fb43f7d7c3e0fef888a4e9dfcc752
ms.sourcegitcommit: f888e9c6e0290608abb915aa599ae9629b0efd3e
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 11/01/2021
ms.locfileid: "7727606"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-37-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 37 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור האפליקציה Microsoft Dynamics 365 Project Service Automation. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. הוא תואם ל- Dynamics 365 9.x. לעדכון למהדורה זו, בקר בדף הפתרונות המקוון של מרכז הניהול עבור Dynamics 365 והתקן את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 37, עדכון V3 של Project Service Automation. לגרסה זו יש מספר build של V3.10.58.120 והיא זמינה בדרך כלל באמצעות עדכון עצמי בנובמבר 2021.

## <a name="update-release-37"></a>הפצת עדכון 37

### <a name="bug-fixes"></a>תיקוני באגים

הבעיות הבאות תוקנו.

**זמן והוצאה**
- משתמשים אינם יכולים למחוק ערך זמן על ידי ניקוי התא.
- התצוגה **‏‫האישורים שלי שנכשלו‬** מכילה רק אישורי פרויקטים עם המצב **נשלח**.

**ניהול פרוייקט**
- משתמשים מקבלים שגיאת חריגת הפניה אפסית בעת פתיחת פרויקט בתוסף שולחן העבודה של Microsoft, אם שם המיקום של חבר צוות הפרויקט ריק.
- אין לחצן **שמירה** בדף **משימת פרויקט** כדי שמשתמשים לא יוכלו לשמור שינויים ברשומות המשימות.
- משתמשים לא יכולים למחוק פרויקט שיש לו משימה הקשורה להצעת מחיר במצב **זכייה**.

**מכירות**
- השדה **מטבע** בדף **פרוייקט** מתעדכן כך שיתאים למטבע של התבנית שהוחלה.
- העלות מחושבת בצורה שגויה במשימות שיש להן מספר מטבעות.
