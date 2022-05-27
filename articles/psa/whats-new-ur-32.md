---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 32 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 32, עדכון V3 של Project Service Automation.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/01/2021
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
ms.openlocfilehash: 3ad87eceb90a48997aadf00803b8d14c5108eb83
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8580089"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-32-v3"></a>מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 32 V3

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור האפליקציה Microsoft Dynamics 365 Project Service Automation. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. הוא תואם ל- Dynamics 365 9.x. לעדכון למהדורה זו, בקר בדף הפתרונות המקוון של מרכז הניהול עבור Dynamics 365 והתקן את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 32, עדכון V3 של Project Service Automation. גירסה זו כוללת מספר build של V3.10.53.108 והיא זמינה לרוב באמצעות עדכון עצמי ביוני 2021.

## <a name="update-release-32"></a>הפצת עדכון 32

### <a name="bug-fixes"></a>תיקוני באגים

#### <a name="general"></a>כללי

- כאשר שדרוג גדול נכשל, יש לחסום רק את נקודות הכניסה העיקריות לאפליקציה, כדי להבטיח שהישויות המשותפות עדיין יהיו נגישות.

#### <a name="time-and-expense"></a>זמן והוצאה

הבעיות הבאות תוקנו:

- הפרמטר **TimeEntriesImportFromResourceAssignment** אינו מקיים את זמני ההתחלה והסיום של נתח המתאר בהקצאת המשאבים.
- כשתבחר **נקודת כניסה** ברשת **ערכי זמן**, ייתכן שלא תהיה לך אפשרות לבחור טפסים אחרים.
- בזמן שאתה מייבא מטלות לערכי זמן, שאילתת קוד הלקוח עשויה ליצור כתובת URL ארוכה שנכשלה בשאילתה.
- ברשת **ערכי זמן**, לאחר שנמחק ערך מהתא, המיקוד לא נשאר ברשת.
- הלחצן **דחה** הוסר מהתצוגה **אישורים בעיבוד** עבור האישורים המודרניים.
- היציבות והביצועים של אישור ערכי זמן בכמויות מושפעים ממנעולים ואי טיפול נכון בהתאמות האישיות שקשורות לישות **ערך זמן**.

#### <a name="project-planning"></a>תכנון פרוייקטים

- חריגה של ערך null נוצרת כאשר אתה מעדכן פרוייקט שיש לו ערך null בשדה **‏‫יחידת החוזה‬**.
- האפשרות **רענן את סך כל הפרוייקטים** מחשבת באופן שגוי את העלות הנותרת ואת המכירות הנותרות בפרוייקט.
- חישובי תמחור מיותרים משפיעים על הביצועים שקשורים לעדכונים בקווי המתאר של הקצאת משאבים.

#### <a name="resource-management"></a>ניהול משאבים

הבעיה הבאה תוקנה:

- כאשר קיבולת לוח השנה של משאב שניתן להזמין היא יותר מ- 1, Project Service Automation מזהה באופן שגוי את הקיבולת כ- 0 (אפס). כך נוצרת לולאה אינסופית בתצוגת לוח הזמנים.

#### <a name="sales"></a>מכירות

הבעיות הבאות תוקנו:

- כאשר נוצרת שורת יומן המכילה סוג עסקה מותאם אישית, מתרחש החריג הבא של התייחסות null: *Microsoft.Dynamics.ProjectService.Plugins.JournalLinePlugins.ValidateUnitScheduleAndUnitWithTransactionType (TransactionTypetransactionType, TransactionTypeCode transTypeCodeFromPlugin)*.
- אין להוסיף תפקידים וקטגוריות שהושבתו לפני העתקה של הצעת מחיר לתפקידים וקטגוריות שניתנים לחיוב של הצעת מחיר שהועתקה לאחרונה.
- תאריך המסמך ותאריך החשבונאות אינם מתואמים עם תאריך ההתחלה המסופק בפירוט שורת חשבונית שנוצר ישירות בטיוטת חשבונית.
- חריגות של ערכי Null נוצרות בתרחישים שקשורים להשבתת תפקידים וקטגוריות לפני העתקת הצעת מחיר.
- הפעולה **עדכן מחירים** בדף **פרוייקטים** לא מעדכנת אומדני הוצאות והערכות חומרים.
