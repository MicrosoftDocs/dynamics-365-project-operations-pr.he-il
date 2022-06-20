---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 42 V3
description: מאמר זה מפרט את התכונות והתיקונים הזמינים בעדכון Microsoft Dynamics 365 Project Service Automation מהדורה 42, גרסה 3.
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
ms.openlocfilehash: e9911531e4acbd78db416f554c8d85c4f1fee1cf
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912716"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-42-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 42 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור האפליקציה Microsoft Dynamics 365 Project Service Automation. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. הוא תואם ל- Dynamics 365 9.x. לעדכון למהדורה זו, בקר בדף הפתרונות המקוון של מרכז הניהול עבור Dynamics 365 והתקן את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

מאמר זה מפרט את התכונות והתיקונים החדשים או ששונו בעדכון Project Service Automation מהדורה 42, גרסה 3. גירסה זו כוללת מספר build של V3.10.73.61 ובדרך כלל היא זמינה דרך עדכון עצמי באפריל 2022.

## <a name="update-release-42"></a>הפצת עדכון 42

### <a name="bug-fixes"></a>תיקוני באגים

הבעיות הבאות תוקנו.

**זמן והוצאה**

- בעת דחיית גיליון זמנים, המשתמש שדחה אותו מזוהה באופן שגוי כ **מערכת**.
- בעת ייבוא ערכי זמן, חסר הערך **קטגוריית משאב**.
- מאשרי הפרוייקט יכולים לאשר פרוייקטים שהוגשו כאשר ההרשאות שלהם אינן מוגדרות באופן ספציפי ל **יכול לאשר**.

**מכירות**

- בעת רישום נתונים בפועל במשימות שאינן ברמת בסיס, העלויות בפועל מצטברות באופן שגוי.
