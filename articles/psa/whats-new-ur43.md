---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 43 V3
description: נושא זה מפרט את התכונות והתיקונים הזמינים ב- Microsoft Dynamics 365 Project Service Automation מהדורת עדכון 43, V3.
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
ms.openlocfilehash: fcf18a24b3bc354a16a415368063133743e79696
ms.sourcegitcommit: 7e419a5f73f80fa887084e3b212c90586fc397dd
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/05/2022
ms.locfileid: "8710005"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-43-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 43 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור האפליקציה Microsoft Dynamics 365 Project Service Automation. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. היא תואמת עם Dynamics 365 9.x. לעדכון למהדורה זו, בקר בדף הפתרונות המקוון של מרכז הניהול עבור Dynamics 365 והתקן את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 43, עדכון V3 של Project Service Automation. גירסה זו כוללת מספר build של V3.10.74.200 ובדרך כלל היא זמינה דרך עדכון עצמי במאי 2022.

## <a name="update-release-43"></a>הפצת עדכון 43

### <a name="bug-fixes"></a>תיקוני באגים

הבעיות הבאות תוקנו.


**זמן והוצאה**

- בעת ייבוא ערכי זמן מהזמנות או הקצאות משאבים, ההפניה למשאב הקשור הניתן להזמנה אינה נשמרת.
- כאשר רשת ערכי הזמן מורחבת למסך מלא, הניווט ברשת באמצעות מקש tab אינו פועל.
- בעת הגשת ערך זמן שנוצר על-ידי משתמש אחר, השדה **נשלח על-ידי** מאוכלס באופן שגוי עם המשתמש שיצר את גיליון הזמנים.
