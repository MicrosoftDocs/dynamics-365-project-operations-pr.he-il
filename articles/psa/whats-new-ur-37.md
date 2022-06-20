---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 37 V3
description: מאמר זה מפרט את התכונות והתיקונים הזמינים בעדכון Microsoft Dynamics 365 Project Service Automation מהדורה 37, גרסה 3.
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
ms.reviewer: johnmichalak
ms.openlocfilehash: bdbb125b4f41bb9970f5bd8a01cf0bb863c34738
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922499"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-37-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 37 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור האפליקציה Microsoft Dynamics 365 Project Service Automation. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. הוא תואם ל- Dynamics 365 9.x. לעדכון למהדורה זו, בקר בדף הפתרונות המקוון של מרכז הניהול עבור Dynamics 365 והתקן את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

מאמר זה מפרט את התכונות והתיקונים החדשים או ששונו בעדכון Project Service Automation מהדורה 37, גרסה 3. לגרסה זו יש מספר build של V3.10.58.120 והיא זמינה בדרך כלל באמצעות עדכון עצמי בנובמבר 2021.

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
