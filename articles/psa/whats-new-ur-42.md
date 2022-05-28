---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 42 V3
description: נושא זה מפרט את התכונות והתיקונים הזמינים ב- Microsoft Dynamics 365 Project Service Automation מהדורת עדכון 42, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/05/2022
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
ms.openlocfilehash: 32cb7a4c5fc29d5c0dcec37dd395ae69037435a2
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8589197"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-42-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 42 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור האפליקציה Microsoft Dynamics 365 Project Service Automation. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. הוא תואם ל- Dynamics 365 9.x. לעדכון למהדורה זו, בקר בדף הפתרונות המקוון של מרכז הניהול עבור Dynamics 365 והתקן את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 42, עדכון V3 של Project Service Automation. גירסה זו כוללת מספר build של V3.10.73.61 ובדרך כלל היא זמינה דרך עדכון עצמי באפריל 2022.

## <a name="update-release-42"></a>הפצת עדכון 42

### <a name="bug-fixes"></a>תיקוני באגים

הבעיות הבאות תוקנו.

**זמן והוצאה**

- בעת דחיית גיליון זמנים, המשתמש שדחה אותו מזוהה באופן שגוי כ **מערכת**.
- בעת ייבוא ערכי זמן, חסר הערך **קטגוריית משאב**.
- מאשרי הפרוייקט יכולים לאשר פרוייקטים שהוגשו כאשר ההרשאות שלהם אינן מוגדרות באופן ספציפי ל **יכול לאשר**.

**מכירות**

- בעת רישום נתונים בפועל במשימות שאינן ברמת בסיס, העלויות בפועל מצטברות באופן שגוי.
