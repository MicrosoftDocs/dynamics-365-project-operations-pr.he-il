---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 43 V3
description: מאמר זה מפרט את התכונות והתיקונים הזמינים בעדכון Microsoft Dynamics 365 Project Service Automation מהדורה 43, גרסה 3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 05/04/2022
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
ms.openlocfilehash: b12cfda08f1ea1fc441782003130be445a437f7c
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8915321"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-43-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 43 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור האפליקציה Microsoft Dynamics 365 Project Service Automation. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. היא תואמת עם Dynamics 365 9.x. לעדכון למהדורה זו, בקר בדף הפתרונות המקוון של מרכז הניהול עבור Dynamics 365 והתקן את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

מאמר זה מפרט את התכונות והתיקונים החדשים או ששונו בעדכון Project Service Automation מהדורה 43, גרסה 3. גירסה זו כוללת מספר build של V3.10.74.200 ובדרך כלל היא זמינה דרך עדכון עצמי במאי 2022.

## <a name="update-release-43"></a>הפצת עדכון 43

### <a name="bug-fixes"></a>תיקוני באגים

הבעיות הבאות תוקנו.


**זמן והוצאה**

- בעת ייבוא ערכי זמן מהזמנות או הקצאות משאבים, ההפניה למשאב הקשור הניתן להזמנה אינה נשמרת.
- כאשר רשת ערכי הזמן מורחבת למסך מלא, הניווט ברשת באמצעות מקש tab אינו פועל.
- בעת הגשת ערך זמן שנוצר על-ידי משתמש אחר, השדה **נשלח על-ידי** מאוכלס באופן שגוי עם המשתמש שיצר את גיליון הזמנים.
