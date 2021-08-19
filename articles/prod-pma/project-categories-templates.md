---
title: סנכרון קטגוריות של הוצאות בפרויקט בין Finance and Operations ו- Project Service Automation
description: נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון קטגוריות של הוצאות בפרויקט בין Microsoft Dynamics 365 Finance ו- Dynamics 365 Project Service Automation.
author: Yowelle
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: 52c79f8b641d4b2df3b30964331633f2487402f8f8d229b540f9544c0f848557
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/06/2021
ms.locfileid: "7001117"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a>סנכרון קטגוריות של הוצאות בפרויקט בין Finance and Operations ו- Project Service Automation

[!include[banner](../includes/banner.md)]

נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון קטגוריות של הוצאות בפרויקט בין Dynamics 365 Finance ו- Dynamics 365 Project Service Automation.

> [!NOTE]
> - שילוב משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונעילת פונקציונליות זמינים בגירסה 8.0.
> - שילוב נתונים בפועל זמין בגירסה 8.0.1 ואילך.
> - אם אתה משתמש ב- Enterprise Edition 7.3.0, לאחר התקנת KB 4132657 ו- KB 4132660, תוכל להשתמש בתבניות לשילוב משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונתונים בפועל, וכן להגדיר תצורה של נעילת פונקציונליות. אם עליך לאפס את ההפצות החשבונאיות, מומלץ להתקין גם את KB 4131710.

## <a name="data-flow-for-project-service-automation-and-finance"></a>זרימת נתונים עבור Project Service Automation ו- Finance

פתרון השילוב Project Service Automation ו- Finance משתמש בתכונת שילוב הנתונים לסנכרון נתונים במופעים של Project Service Automation ו- Finance. תבניות השילוב שזמינות עם תכונת שילוב הנתונים מאפשרות זרימת נתונים על קטגוריות של עסקאות הוצאה בפרויקט ובין Finance ו- Project Service Automation.

אם הקטגוריות של הוצאות בפרויקט נשלטות ב- Finance, זרימת השילוב תהיה ראשונה מ- Finance אל Project Service Automation. מזהי השילוב של קטגוריות הוצאות בפרויקט מתעדכנים לאחר מכן באמצעות סנכרון מ- Project Service Automation ל- Finance.

אם הקטגוריות של הוצאות בפרויקט נשלטות ב- Project Service Automation, זרימת השילוב תהיה ראשונה מ- Project Service Automation אל Finance. יש להגדיר את קטגוריות הפרויקט כבר ב- Finance לפני הסינכרון מ- Project Service Automation. לאחר מכן סנכרן מ- Finance בחזרה ל- Project Service Automation, ואז מ- Project Service Automation ל- Finance שוב. באופן זה, אתה עוזר להבטיח שהקטגוריות יהיו מקושרות ושלא ייווצרו כפילויות.

> [!NOTE]
> בדרך כלל, קטגוריות של הוצאות בפרויקט נשלטות ב- Finance. עם זאת, אם הן לא נשלטות משם, או אם הקטגוריות של ההוצאות כבר נוצרו ב- Project Service Automation, עליך תחילה לסנכרן באמצעות תבנית קטגוריות של עסקאות הוצאות בפרויקט (PSA ל- Fin and Ops). לאחר מכן סנכרן באמצעות תבנית הקטגוריות של עסקאות הוצאות בפרויקט (Fin and Ops ל- PSA). לאחר מכן עליך להפעיל את הסנכרון מ- Project Service Automation ל- Finance פעם נוספת.
>
> אם אתה מסנכרן תחילה מ- Project Service Automation, יש לעמוד בדרישות הבאות ב- Finance לפני הפעלת הסנכרון:
>
> - הקטגוריה המשותפת שתואמת לקטגוריית הפרויקט שמוגדרת ב- Project Service Automation חייבת להתקיים, והיא חייבת להיות מופעלת גם עבור **פרויקט** וגם עבור **הוצאה**.
> - עבור כל ישות משפטית ב- Finance שבה יש לשלב, קטגוריות הפרויקט הבאות חייבות להתקיים:
>
>     - **קטגוריית פרויקט** קיימת. 
>     - האפשרות **השתמש בהוצאה** זמינה.
>     - האפשרות **פעיל ביומן** זמינה.
>     - **סוג עסקה** נקבעה בתור **הוצאה**.

האיור הבא מראה כיצד הנתונים מסונכרנים בין Project Service Automation ו- Finance.

[![זרימת נתונים לשילוב Project Service Automation עם Finance.](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a>סנכרון קטגוריית הוצאה בפרויקט מ- Finance אל Project Service Automation

### <a name="template-and-task"></a>תבנית ומשימה

כדי לגשת לתבנית, במרכז הניהול של Microsoft Power Apps, בחר **פרויקטים** ולאחר מכן, בפינה העליונה, בחר **פרויקט חדש** כדי לבחור תבניות ציבוריות.

התבנית והמשימה הבסיסית הבאות משמשות לסנכרון קטגוריות של הוצאות בפרויקט מ- Finance אל Project Service Automation:

- **שם התבנית בשילוב נתונים:** קטגוריות של עסקאות הוצאות בפרויקט (Fin and Ops ל- PSA)
- **שם המשימה בפרויקט:** סנכרון קטגוריות ל- PSA

### <a name="entity-set"></a>קבוצת ישויות

| כספים                           | Project Service Automation |
|-----------------------------------|----------------------------|
| ישות שילוב לקטגוריות | קטגוריות עסקה     |

### <a name="entity-flow"></a>זרימת ישות

קטגוריות של הוצאות בפרויקט מנוהלות ב- Finance והן מסונכרנות ל- Project Service Automation כקטגוריות של עסקאות.

### <a name="power-query"></a>Power Query

בעת סנכרון ל- Project Service Automation, עליך להשתמש ב- Microsoft Power Query for Excel כדי לקבוע את סוג החיוב בקטגוריית העסקה. התבנית קטגוריות של עסקאות הוצאות בפרויקט (Fin and Ops ל- PSA) מספק עמודה ומיפוי בברירת מחדל. אם אתה יוצר תבנית משלך, עליך להוסיף עמודה מותנית ב- Power Query. פעל בהתאם לשלבים אלה.

1. לחץ על החץ כדי לפתוח את המיפוי של משימת הקטגוריות של הוצאות בפרויקט בתבנית קטגוריות עסקאות של הוצאות הפרויקט (Fin and Ops ל- PSA).
2. לחץ על הקישור **שאילתות וסינון מתקדמים** כדי לפתוח את Power Query.
2. בחר **הוסף עמודה מותנית**.
3. הזן שם לעמודה החדשה, כגון **BillingType**.
4. הזן את התנאי הבא: **אם CATEGORYID לא שווה ל- Null אז 19235001, אחרת Null**.
5. לחץ על **אישור** בעמודה.
6. הקפד למפות את העמודה החדשה הזו בדף המיפוי.

האיור הבא מציג דוגמה למיפוי משימת התבנית בשילוב נתונים. המיפוי מציג את פרטי השדה שיסונכרנו מ- Finance ל- Project Service Automation.

[![קטגוריית הוצאה בפרוייקט למיפוי תבנית של Project Service Automation.](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a>סנכרון קטגוריית הוצאה בפרויקט מ- Project Service Automation אל Finance

### <a name="template-and-task"></a>תבנית ומשימה

התבנית והמשימה הבסיסית הבאות משמשות לסנכרון קטגוריות של הוצאות בפרויקט מ- Project Service Automation אל Finance:

- **שם התבנית בשילוב נתונים:** קטגוריות של עסקאות הוצאות בפרויקט (PSA ל- Fin and Ops)
- **שם המשימה בפרויקט:** סנכרון קטגוריות ל- Fin and Ops

### <a name="entity-set"></a>קבוצת ישויות

| Project Service Automation | כספים                           |
|----------------------------|-----------------------------------|
| קטגוריות עסקה     | ישות שילוב לקטגוריות |

### <a name="entity-flow"></a>זרימת ישות

קטגוריות של הוצאות בפרויקט מנוהלות ב- Finance והן מסונכרנות ל- Project Service Automation כקטגוריות של עסקאות. הסנכרון בחזרה אל Finance מעדכן את קטגוריית הפרויקט ב- Finance עם מזהה השילוב מ- Project Service Automation.

### <a name="template-mapping-in-data-integration"></a>מיפוי תבנית בשילוב נתונים

האיור הבא מציג דוגמה למיפוי משימת התבנית בשילוב נתונים.

> [!NOTE]
> המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.

[![Project Service Automation למיפוי תבנית Finance.](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)


[!INCLUDE[footer-include](../includes/footer-banner.md)]