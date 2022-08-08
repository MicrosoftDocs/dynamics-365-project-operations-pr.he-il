---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 45 V3
description: מאמר זה מפרט את התכונות והתיקונים הזמינים בעדכון Microsoft Dynamics 365 Project Service Automation מהדורה 45, גירסה V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 07/14/2022
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
ms.openlocfilehash: 98f7c973917d7d6334e6e0aeb15214c538b33143
ms.sourcegitcommit: 36fda4f45ddeb0f81d30bd1e22852727df644754
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 07/16/2022
ms.locfileid: "9169157"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-45-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 45 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור האפליקציה Microsoft Dynamics 365 Project Service Automation. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. הוא תואם ל- Dynamics 365 9.x. לעדכון למהדורה זו, בקר בדף הפתרונות המקוון של מרכז הניהול עבור Dynamics 365 והתקן את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

מאמר זה מפרט את התכונות והתיקונים החדשים או ששונו בעדכון Project Service Automation מהדורה 45, גירסה V3. גרסה זו כוללת מספר build של V3.10.76.168 והיא זמינה בדרך כלל באמצעות עדכון עצמי ביולי 2022.

## <a name="update-release-45"></a>הפצת עדכון 45

### <a name="bug-fixes"></a>תיקוני באגים

הבעיות הבאות תוקנו.

**מכירות**

- משתמשים לא יכולים ליצור חשבוניות בהצלחה לאחר שהם מנסים ליצור חשבונית ללא מכירות שלא חויבו, אם הם גם צופים באותו מופע של הדף ולא מרעננים אותו.

**זמן והוצאה**

- כאשר אישורים מודרניים מופעלים ואישור פרויקט מאוחזר מאושר, שלב הרשומה מתעדכן באופן שגוי ל **בקשה לאחזור אושרה**.
- כאשר אישורים מודרניים מופעלים וזרימות ענן אינן פעילות, תהליך האישור לא מוצלח, והמשתמשים השולחים או מאשרים לא מקבלים הודעה.
