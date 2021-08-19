---
title: סנכרון הערכות פרויקטים ישירות מ- Project Service Automation ל- Finance and Operations
description: נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון הערכת שעות בפרויקט והערכת הוצאות בפרויקט ישירות מ- Microsoft Dynamics 365 Project Service Automation אל Dynamics 365 Finance.
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
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 6696449d80e0915a0c878dbe75cfdf6e268b98ad9f6453bcfc4b424db68021e4
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/06/2021
ms.locfileid: "6988202"
---
# <a name="synchronize-project-estimates-directly-from-project-service-automation-to-finance-and-operations"></a>סנכרון הערכות פרויקטים ישירות מ- Project Service Automation ל- Finance and Operations

[!include[banner](../includes/banner.md)]

נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון הערכת שעות בפרויקט והערכת הוצאות בפרויקט ישירות מ- Dynamics 365 Project Service Automation אל Dynamics 365 Finance.

> [!NOTE]
> - שילוב משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונעילת פונקציונליות זמינים בגירסה 8.0.
> - שילוב נתונים בפועל זמין בגירסה 8.0.1 ואילך.

## <a name="data-flow-for-project-service-automation-to-finance"></a>זרימת נתונים עבור Project Service Automation ל- Finance

פתרון השילוב Project Service Automation ל- Finance משתמש בתכונת שילוב הנתונים לסנכרון נתונים במופעים של Project Service Automation ו- Finance. תבניות השילוב שזמינות עם תכונת שילוב הנתונים מאפשרות זרימת נתונים על הערכת שעות בפרויקט והערכת הוצאות בפרויקט מ- Project Service Automation ל- Finance.

האיור הבא מראה כיצד הנתונים מסונכרנים בין Project Service Automation ו- Finance.

[![זרימת נתונים לשילוב Project Service Automation עם Finance.](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)

## <a name="project-hour-estimates"></a>הערכת שעות בפרויקט

### <a name="template-and-tasks"></a>תבנית ומשימות

כדי לגשת לתבניות הזמינות, במרכז הניהול של Microsoft Power Apps, בחר **פרויקטים** ולאחר מכן, בפינה העליונה, בחר **פרויקט חדש** כדי לבחור תבניות ציבוריות.

התבנית והמשימות הבסיסיות הבאות משמשות לסנכרון הערכת שעות בפרויקט מ- Project Service Automation אל Finance:

- **שם התבנית בשילוב נתונים:** הערכת שעות בפרויקט (PSA ל- Fin and Ops)
- **שם המשימות בפרויקט:**

    - יחסי גומלין של עסקה
    - הערכות הוצאות

### <a name="entity-set"></a>קבוצת ישויות

| Project Service Automation | כספים                                       |
|----------------------------|-----------------------------------------------|
| משימות פרויקט              | ישות שילוב להערכת שעות בפרויקט |

### <a name="entity-flow"></a>זרימת ישות

הערכות של שעות בפרויקט מנוהלים ב- Project Service Automation והן מסונכרנות ל- Finance כתחזיות לשעות בפרויקט.

### <a name="prerequisites"></a>דרישות מוקדמות

לפני שתוכל לסנכרן הערכת שעות בפרויקט, עליך לסנכרן פרויקטים, משימות פרויקט וקטגוריות של עסקאות הוצאות בפרויקט.

### <a name="power-query"></a>Power Query

בתבנית הערכת שעות בפרויקט, עליך להשתמש ב- Microsoft Power Query for Excel כדי להשלים את המשימות הבאות:

- הגדר את מזהה מודל תחזית ברירת המחדל שישמש כאשר השילוב יוצר תחזיות חדשות לשעות.
- סנן רשומות שספציפיות למשאבים במשימה אשר יכשלו בשילוב בתוך תחזיות השעות.
- סנן כל שורה ריקה בקטגוריית עסקה. אי השלמת המשימה עשויה להוביל לתחזית שעות שגויה.

#### <a name="set-the-default-forecast-model-id"></a>הגדר את מזהה מודל התחזית בברירת מחדל

כדי לעדכן את מזהה מודל התחזית בברירת מחדל בתבנית, לחץ על החץ **מפה** כדי לפתוח את המיפוי. לאחר מכן, בחר בקישור **שאילתות וסינון מתקדמים**.

- אם אתה משתמש בתבנית ברירת מחדל להערכת השעות בפרויקט (PSA ל- Fin and Ops), בחר באפשרות **תנאי שהוכנס** ברשימה **שלבים שהוחלו**. בערך **פונקציה**, החלף את **O\_forecast** בשם של מזהה מודל התחזית שבו יש להשתמש בשילוב. לתבנית ברירת המחדל יש מזהה מודל תחזית מנתוני ההדגמה.
- אם אתה יוצר תבנית חדשה, עליך להוסיף עמודה זו. ב- Power Query, בחר **הוסף עמודה מותנית** והזן שם לעמודה החדשה, כגון **ModelID**. הזן את התנאי עבור העמודה, שבה, אם משימה בפרויקט אינה Null, \<enter the forecast model ID\>; אחרת Null.

#### <a name="filter-out-resource-specific-records"></a>סנן רשומות שספציפיות למשאבים

לתבנית הערכת שעות בפרויקט (PSA ל- Fin and Ops) יש מסנן ברירת מחדל שמסיר כל רשומה שספציפית למשאבים. אם אתה יוצר תבנית משלך, עליך להוסיף מסנן זה. בחר בקישור **שאילתות וסינון מתקדמים** כדי לסנן את העמודה **msdyn\_islinetask** כך שרק הרשומות שהן **False** יהיו כלולות.

#### <a name="filter-out-empty-transaction-category-rows"></a>סנן כל שורה ריקה בקטגוריית עסקה

עליך להוסיף מסנן כדי להסיר שורות שיש בהן קטגוריות של עסקאות ריקות. משימה זו נדרשת, בין אם אתה משתמש בתבנית ברירת המחדל או יוצר תבנית משלך. מסנן זה מסיר שורות סיכום מ- Project Service Automation העלולות לגרום לתחזיות השעות ב- Finance להיות שגויות. בחר בקישור **שאילתות וסינון מתקדמים** כדי לסנן רשומות שהן Null בעמודה **msdyn\_transactioncategory\_value**.

### <a name="template-mapping-in-data-integration"></a>מיפוי תבנית בשילוב נתונים

האיור הבא מציג דוגמה למיפוי משימת התבנית בשילוב נתונים. המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.

[![מיפוי משימת תבנית בשילוב נתונים.](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)

## <a name="project-expense-estimates"></a>הערכות הוצאה בפרויקט

### <a name="template-and-tasks"></a>תבנית ומשימות

התבנית והמשימות הבסיסיות הבאות משמשות לסנכרון הערכת הוצאות בפרויקט מ- Project Service Automation אל Finance:

- **שם התבנית בשילוב נתונים:** הערכת הוצאות בפרויקט (PSA ל- Fin and Ops)
- **שם המשימות בפרויקט:**

    - יחסי גומלין של עסקה 
    - הערכות הוצאות

### <a name="entity-set"></a>קבוצת ישויות

| Project Service Automation | כספים                                                  |
|----------------------------|----------------------------------------------------------|
| חיבורי עסקה    | ישות שילוב ליחסי גומלין של עסקה בפרויקט |
| שורות של הערכות             | ישות שילוב להערכת הוצאות בפרויקט         |

### <a name="entity-flow"></a>זרימת ישות

הערכות של הוצאות בפרויקט מנוהלות ב- Project Service Automation והן מסונכרנות ל- Finance כתחזיות להוצאות בפרויקט.

### <a name="prerequisites"></a>דרישות מוקדמות

לפני שתוכל לסנכרן הערכת הוצאות בפרויקט, עליך לסנכרן פרויקטים, משימות פרויקט וקטגוריות של עסקאות הוצאות בפרויקט.

### <a name="power-query"></a>Power Query

בתבנית הערכת הוצאות בפרויקט, עליך להשתמש ב- Power Query כדי להשלים את המשימות הבאות:

- סנן כדי לכלול רק רשומות של שורת הערכת הוצאות.
- הגדר את מזהה מודל תחזית ברירת המחדל שישמש כאשר השילוב יוצר תחזיות חדשות לשעות.
- שנה את סוגי החיובים.
- שנה את סוגי העסקאות.

#### <a name="filter-to-include-only-expense-estimate-lines"></a>סנן כדי לכלול רק שורות של הערכת הוצאות

לתבנית הערכת הוצאות בפרויקט (PSA ל- Fin and Ops) יש מסנן ברירת מחדל הכולל רק שורות הוצאות בשילוב. אם אתה יוצר תבנית משלך, עליך להוסיף מסנן זה. בחר במשימה **‏‫יחסי גומלין של עסקה‬** ולאחר מכן לחץ על החץ **מפה** כדי לפתח את המיפוי. בחר בקישור **שאילתות וסינון מתקדמים**. סנן את העמודה **msdyn\_transactiontype1** כך שתכלול רק את **msdyn\_estimateline**.

#### <a name="set-the-default-forecast-model-id"></a>הגדר את מזהה מודל התחזית בברירת מחדל

כדי לעדכן את מזהה מודל התחזית בברירת מחדל בתבנית, בחר במשימה **הערכת הוצאות** ולאחר מכן לחץ על החץ **מפה** כדי לפתוח את המיפוי. בחר בקישור **שאילתות וסינון מתקדמים**.

- אם אתה משתמש בתבנית ברירת מחדל להערכת הוצאות בפרויקט (PSA ל- Fin and Ops), ב- Power Query, בחר באפשרות הראשונה **תנאי שהוכנס** במקטע **שלבים שהוחלו**. בערך **פונקציה**, החלף את **O\_forecast** בשם של מזהה מודל התחזית שבו יש להשתמש בשילוב. לתבנית ברירת המחדל יש מזהה מודל תחזית מנתוני ההדגמה.
- אם אתה יוצר תבנית חדשה, עליך להוסיף עמודה זו. ב- Power Query, בחר **הוסף עמודה מותנית** והזן שם לעמודה החדשה, כגון **ModelID**. הזן את התנאי עבור העמודה, שבה, אם מזהה שורת הערכה אינו Null, \<enter the forecast model ID\>; אחרת Null.

#### <a name="transform-the-billing-types"></a>שנה את סוגי החיובים

תבנית הערכת הוצאות בפרויקט (PSA ל- Fin and Ops) כוללת עמודה מותנית המשמשת לשינוי סוגי החיובים המתקבלים מ- Project Service Automation במהלך השילוב. אם אתה יוצר תבנית משלך, עליך להוסיף עמודה מותנית זו. בחר בקישור **שאילתות וסינון מתקדמים** ולאחר מכן בחר **הוסף עמודה מותנית**. הזן שם לעמודה החדשה, כגון **BillingType**. לאחר מכן הזן את התנאי הבא:

אם ‎**msdyn\_billingtype** = 192350000, אז **NonChargeable**  
אחרת, אם ‎**msdyn\_billingtype** = 192350001, אז **Chargeable**  
אחרת, אם ‎**msdyn\_billingtype** = 192350002, אז **Complimentary**  
אחרת **NotAvailable**

#### <a name="transform-the-transaction-types"></a>שנה את סוגי העסקאות

תבנית הערכת הוצאות בפרויקט (PSA ל- Fin and Ops) כוללת עמודה מותנית המשמשת לשינוי סוגי העסקאות המתקבלים מ- Project Service Automation במהלך השילוב. אם אתה יוצר תבנית משלך, עליך להוסיף עמודה מותנית זו. בחר בקישור **שאילתות וסינון מתקדמים** ולאחר מכן בחר **הוסף עמודה מותנית**. הזן שם לעמודה החדשה, כגון **TransactionType**. לאחר מכן הזן את התנאי הבא:

אם ‎**msdyn\_transactiontypecode** = 192350000, אחרת **Cost**  
אחרת, אם ‎**msdyn\_transactiontypecode** = 192350005, אחרת **Sales**  
אחרת **null**

### <a name="template-mapping-in-data-integration"></a>מיפוי תבנית בשילוב נתונים

האיורים הבאים מציגים דוגמאות למיפויי משימות התבנית בשילוב נתונים. המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.

[![מיפוי תבניות של עסקאות אומדן הוצאות.](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)

[![מיפוי תבניות של אומדן הוצאות.](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)


[!INCLUDE[footer-include](../includes/footer-banner.md)]