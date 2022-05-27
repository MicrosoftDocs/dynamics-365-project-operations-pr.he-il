---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 35 V3
description: נושא זה מפרט את התכונות והתיקונים הזמינים ב- Microsoft Dynamics 365 Project Service Automation מהדורת עדכון 35, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 09/03/2021
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
ms.openlocfilehash: e210777f1e4d149b700721ac7fb9bd129b1166fe
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8574029"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-35-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 35 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור האפליקציה Microsoft Dynamics 365 Project Service Automation. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. הוא תואם ל- Dynamics 365 9.x. לעדכון למהדורה זו, בקר בדף הפתרונות המקוון של מרכז הניהול עבור Dynamics 365 והתקן את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 35, עדכון V3 של Project Service Automation. גירסה זו כוללת מספר build של V3.10.56.110 והיא זמינה בדרך כלל באמצעות עדכון עצמי בספטמבר 2021.

## <a name="update-release-35"></a>הפצת עדכון 35

### <a name="bug-fixes"></a>תיקוני באגים

הבעיות הבאות תוקנו.

**זמן והוצאה**

- מאשר הפרוייקט מקבל שגיאת הרשאת קריאה כאשר הוא מאשר רשומות הוצאות עם תפקיד **מאשר פרוייקט**.
- מאשר הפרוייקט מקבל שגיאת הרשאת כתיבה ב- **msdyn_projectapproval** כאשר הוא מבטל רשומת זמן מאושרת עם תפקיד **מאשר פרוייקט**.
- כאשר אתה בוחר **העתק שבוע** בהזנת זמן ב- Dynamics 365 לטלפונים - מודול היישום 'מרכז משאבי פרוייקט', השגיאה הבאה מופיעה: "...\OfficeProductivity_RibbonRules.js.map: שגיאת HTTP: קוד מצב 404, net::ERR_HTTP_RESPONSE_CODE_FAILURE."
- המדיניות **נסה שוב** מאשרת אוטומטית הזנות שנדחו קודם לכן.
- רשת המשנה **קבוצות אישורים** מציגה פעולות רצועת כלים שאינן ישימות.
- סמלים חסרים עבור **משימת פרוייקט** ו **תפקיד משאב** בישות **ערך זמן**.
- בעת ייבוא הקצאות משאבים, לערכי זמן מיובאים אין את משך הזמן המתאים להקצאות שנוצרו באמצעות משימות במצב ידני.
- **מחק** חסר בדף **חיפוש מתקדם עבור רשומות ערך זמן**.
- **שמור** חסר בדף **מידע על ערך זמן**. בעיה זו מונעת את שמירת השינויים בעת סגירת הדף.

**תכנון פרוייקטים**

- הרשתות **הקצאת משאבים** ו **התאמת משאבים** אינן ממיינות תכונות מקובצות בסדר אלפביתי.
- לא ניתן ליצור משימות אם אופן הפעולה של התאריך מותאם אישית ל **תאריך בלבד**.

**ניהול משאבים**

- אם הן Dynamics 365 Field Service והן Project Service Automation מותקנים, בעיות יצירת שכבת יתר מופיעות כאשר **תצוגה משויכת של דרישת משאב** משויכת לדף ראשי.
- לחיצה כפולה על **שמור** בתיבת הדו-שיח **יצירה מהירה של חבר צוות** מונעת את יצירת דרישת המשאב.

**מכירות**

- מוחזרת חריגה אם אתה מוחק משימה המשויכת להצעת מחיר בעלת מצב **זכייה**.
