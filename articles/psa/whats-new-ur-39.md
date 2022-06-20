---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 39 V3
description: מאמר זה מפרט את התכונות והתיקונים הזמינים בעדכון Microsoft Dynamics 365 Project Service Automation מהדורה 39, גרסה 3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/20/2022
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
ms.openlocfilehash: d5b5938762d98acaead9e26c47bce07e0059faf6
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922453"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-39-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 39 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור האפליקציה Microsoft Dynamics 365 Project Service Automation. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. הוא תואם ל- Dynamics 365 9.x. לעדכון למהדורה זו, בקר בדף הפתרונות המקוון של מרכז הניהול עבור Dynamics 365 והתקן את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

מאמר זה מפרט את התכונות והתיקונים החדשים או ששונו בעדכון Project Service Automation מהדורה 39, גרסה 3. מספר ה-build של גירסה זו הוא V3.10.60.170 והיא זמינה דרך עדכון עצמי החל מינואר 2022.

## <a name="update-release-39"></a>הפצת עדכון 39

### <a name="bug-fixes"></a>תיקוני באגים

הבעיות הבאות תוקנו.

**כללי**

- מספר שיפורים בוצעו במפת האתר עבור תרגום לערבית.

**ניהול פרויקט**

- מתרחשת שגיאה בעת שינוי מנהל הפרוייקט בפרוייקט למשתמש שהוא כבר חבר צוות בפרוייקט.

**מכירות**

- הבעלים של **מחירון חוזה הפרוייקט** שגוי כאשר המחירון נוצר באופן אוטומטי. 
- תוקף התאריך של מחירון אינו מתקיים כאשר המחירון מוחל על פרמטר הפרוייקט.
- ייתכן שליחידת החוזה אין ערך ברירת מחדל נכון בעת עריכת שתי הצעות מחיר נפרדות.
