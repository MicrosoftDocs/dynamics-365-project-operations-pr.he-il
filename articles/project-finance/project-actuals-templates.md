---
title: סנכרון נתונים בפועל של פרוייקט ישירות מ- Project Service Automation ליומן שילוב הפרוייקט עבור רישום ב- Finance and Operations
description: נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון נתונים בפועל של פרוייקט ישירות מ- Microsoft Dynamics 365 Project Service Automation אל Finance and Operations.
author: KimANelson
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: 02ae4986-8e7b-4abe-97d3-cff0904d84de
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 7e5aff102226e5eac2ba3de17407eaa4461cd1ac
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751832"
---
# <a name="synchronize-project-actuals-directly-from-project-service-automation-to-the-project-integration-journal-for-posting-in-finance-and-operations"></a>סנכרון נתונים בפועל של פרוייקט ישירות מ- Project Service Automation ליומן שילוב הפרוייקט עבור רישום ב- Finance and Operations

[!include[banner](../includes/banner.md)]

נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון נתונים בפועל של פרוייקט ישירות מ- Dynamics 365 Project Service Automation אל Dynamics 365 Finance.

התבנית מסנכרנת עסקאות מ- Project Service Automation לטבלת אחסון זמני ב- Finance. לאחר השלמת הסנכרון, **עליך** לייבא נתונים מטבלת האחסון הזמני אל יומן השילוב.

> [!NOTE]
> - שילוב נתונים בפועל של פרוייקט יהיה זמין החל מגירסה 8.0.1 ואילך.
> - אם אתה משתמש ב- Enterprise Edition 7.3.0 לאחר התקנת KB 4132657 ו- KB 4132660, תוכל להשתמש בתבניות לשילוב משימות פרוייקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונתונים בפועל, וכן להגדיר תצורה של נעילת פונקציונליות. אם עליך לאפס את ההפצות החשבונאיות, מומלץ להתקין גם את KB 4131710.
> - אם אתה משתמש בגירסה 7.3.0 ואתה מעביר עסקאות עמלה מ- Project Service Automation, עליך להתקין את KB 4345320 כדי לכלול את העמלות בחשבונית הפרויקט.
> - אם אתה מזין סכומי מס מכירות בעסקאות הוצאה או שעות ב- Project Service Automation, עליך להתקין את עדכון 7 של Project Service Automation. אחרת, הנתונים בפועל של המס לא יקושרו לנתונים בפועל של ההוצאות או השעות המשויכות והם לא יסונכרנו אל Finance. לקבלת מידע נוסף, פנה לתמיכה.

## <a name="data-flow-for-project-service-automation-to-finance"></a>זרימת נתונים עבור Project Service Automation ל- Finance

פתרון השילוב Project Service Automation ל- Finance משתמש בתכונת שילוב הנתונים לסנכרון נתונים במופעים של Project Service Automation ו- Finance. תבניות השילוב שזמינות עם תכונת שילוב הנתונים מאפשרות זרימת נתונים על נתונים בפועל של פרוייקט מ- Project Service Automation ל- Finance.

האיור הבא מראה כיצד הנתונים מסונכרנים בין Project Service Automation ו- Finance.

[![זרימת נתונים לשילוב Project Service Automation עם Finance and Operations](./media/ProjectActualsFlow.jpg)](./media/ProjectActualsFlow.jpg)

## <a name="project-actuals-from-project-service-automation"></a>נתונים בפועל של פרוייקט מ- Project Service Automation

### <a name="template-and-tasks"></a>תבנית ומשימות

כדי לגשת לתבניות הזמינות, במרכז הניהול של Microsoft Power Apps, בחר **פרוייקטים** ולאחר מכן, בפינה העליונה, בחר **פרוייקט חדש** כדי לבחור תבניות ציבוריות.

התבנית והמשימות הבסיסיות הבאות משמשות לסנכרון נתונים בפועל של פרוייקט מ- Project Service Automation אל Finance:

- **שם התבנית בשילוב נתונים:** נתונים בפועל של פרוייקט (PSA ל- Fin and Ops)
- **שם המשימות בפרוייקט:**

    - נתונים בפועל
    - TransactionConnections

### <a name="entity-set"></a>קבוצת ישויות

| Project Service Automation | כספים                                   |
|----------------------------|----------------------------------------------------------|
| נתונים בפועל                    | ישות שילוב לנתונים בפועל של פרוייקט                   |
| חיבורי עסקה    | ישות שילוב ליחסי גומלין של עסקה בפרוייקט |

### <a name="entity-flow"></a>זרימת ישות

נתונים בפועל של פרוייקט מנוהלים ב- Project Service Automation והם מסונכרנים ליומן שילוב הפרוייקט ב- Finance. החשבונאות תוחל על סמך הממדים הכספיים בברירת המחדל והגדרת הרישום.

### <a name="prerequisites"></a>דרישות מוקדמות

לפני שיתרחש סנכרון של נתונים בפועל, עליך להגדיר את התצורה של פרמטרי השילוב של Project Service Automation ולסנכרן פרוייקטים, משימות פרוייקט וקטגוריות עסקאות של הוצאות בפרוייקט.

### <a name="power-query"></a>Power Query

בתבנית נתונים בפועל של פרוייקט, עליך להשתמש ב- Microsoft Power Query for Excel כדי להשלים את המשימות הבאות:

- שנה את סוג העסקה ב- Project Service Automation לסוג העסקה הנכון ב- Finance. שינוי זה כבר הוגדר בתבנית נתונים בפועל של פרוייקט (PSA ל- Fin and Ops).
- שנה את סוג החיוב ב- Project Service Automation לסוג החיוב הנכון ב- Finance. שינוי זה כבר הוגדר בתבנית נתונים בפועל של פרוייקט (PSA ל- Fin and Ops). לאחר מכן, סוג החיוב ימופה אל מאפיין השורה, בהתאם לתצורה בדף **פרמטרי שילוב של Project Service Automation**.
- יש לסנכרן סינון ליחידות ארגוניות ספציפיות של משאב באמצעות תבנית זו.
- אם נתונים בפועל של שעות בין-חברתיות או הוצאות בין-חברתיות יסונכרנו ל- Finance, עליך לשנות את היחידה הארגונית של החוזה לישות המשפטית הנכונה ב- Finance. בתבנית נתונים בפועל של פרוייקט (PSA ל- Fin and Ops), עמודה מותנית מוגדרת בהתאם לנתוני ההדגמה. עליך לעדכן את העמודה המותנית שהוכנסה לאחרונה לישויות המשפטיות הנכונות. אחרת, עלולה להתרחש שגיאת שילוב או ייבוא של עסקאות בפועל שגויות אל Finance.
- אם לא יסונכרנו הנתונים בפועל של שעות בין-חברתיות והוצאות בין-חברתיות ל- Finance, עליך למחוק את העמודה המותנית האחרונה שהוכנסה מהתבנית. אחרת, עלולה להתרחש שגיאת שילוב או ייבוא של עסקאות בפועל שגויות אל Finance.

#### <a name="contract-organizational-unit"></a>יחידה ארגונית של חוזה
כדי לעדכן את העמודה המותנית שהוכנסה בתבנית, לחץ על החץ **מפה** כדי לפתוח את המיפוי. בחר בקישור **שאילתות וסינון מתקדמים** כדי לפתוח את Power Query.

- אם אתה משתמש בתבנית ברירת מחדל לנתונים בפועל של פרוייקט (PSA ל- Fin and Ops), ב- Power Query, בחר באפשרות האחרונה **תנאי שהוכנס** במקטע **שלבים שהוחלו**. בערך **פונקציה**, החלף את **USSI** בשם של הישות המשפטית שתהיה בשימוש בשילוב. הוסף תנאים נוספים לערך **פונקציה** כנדרש ועדכן את התנאי **else** מ- **USMF** לישות המשפטית הנכונה.
- אם אתה יוצר תבנית חדשה, עליך להוסיף את העמודה כדי לתמוך בשעות והוצאות בין-חברתיות. בחר **הוסף עמודה מותנית** והזן שם לעמודה, כגון **LegalEntity**. הזן תנאי לעמודה שבו, אם **msdyn\_contractorganizationalunitid.msdyn\_name** הוא \<יחידה ארגונית\>, אז \<הזן את הישות המשפטית\>; אחרת Null.

### <a name="template-mapping-in-data-integration"></a>מיפוי תבנית בשילוב נתונים

האיורים הבאים מציגים דוגמה למיפוי משימת התבנית בשילוב נתונים. המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.

[![מיפוי תבנית](./media/ActualsMapping.jpg)](./media/ActualsMapping.jpg)

[![מיפוי תבנית](./media/TransactionConnections.jpg)](./media/TransactionConnections.jpg)

## <a name="import-from-staging-table-after-integration-from-project-service-automation"></a>ייבוא מטבלת אחסון זמני לאחר שילוב מ- Project Service Automation

יש להפעיל את התהליך התקופתי לייבוא מטבלת אחסון זמני לאחר סנכרון של נתונים בפועל מ- Project Service Automation אל Finance. תהליך זה ייבא את עסקאות הפרויקט מטבלת האחסון הזמני אל יומן שילוב Project Service Automation, שבו החשבונאות חלה וניתן לרשום את העסקאות שיובאו. מומלץ להפעיל תהליך זה במצב אצווה; באפשרותך להגדיר אותו כך שיפעל כאצווה חוזרת.

## <a name="update-actuals-from-finance"></a>עדכון נתונים בפועל מ- Finance

### <a name="template-and-tasks"></a>תבנית ומשימות

התבנית והמשימות הבסיסיות הבאות משמשות לסנכרון מספר השובר ומסי המכירות עבור עסקאות פרוייקט שנרשמו מ- Finance ל- Project Service Automation:

- **שם התבנית בשילוב נתונים:** עדכון נתונים בפועל של פרוייקט (Fin Ops ל- PSA)
- **שם המשימות בפרוייקט:**

    - נתונים בפועל 
    - TransactionConnections

### <a name="entity-set"></a>קבוצת ישויות

| כספים                                                  | Project Service Automation |
|----------------------------------------------------------|----------------------------|
| ישות שילוב לנתונים בפועל של פרוייקט                   | נתונים בפועל                    |
| ישות שילוב ליחסי גומלין של עסקה בפרוייקט | חיבורי עסקה    |

### <a name="entity-flow"></a>זרימת ישות

נתונים בפועל של פרוייקט מנוהלים ב- Project Service Automation והם מסונכרנים ליומן שילוב הפרוייקט ב- Finance. לאחר רישום נתונים בפועל ב- Finance, הם מעודכנים ב- Project Service Automation עם מספר השובר מ- Finance. אם מסי המכירות התווספו ב- Finance, נוצרים נתונים בפועל חדשים למסים ב- Project Service Automation.

### <a name="power-query"></a>Power Query

בתבנית עדכון נתונים בפועל של פרוייקט, עליך להשתמש ב- Power Query כדי להשלים את המשימות הבאות:

- שנה את סוג העסקה ב- Finance לסוג העסקה הנכון ב- Project Service Automation. שינוי זה כבר הוגדר בתבנית עדכון נתונים בפועל של פרוייקט (Fin Ops ל- PSA).
- שנה את סוג החיוב ב- Finance לסוג החיוב הנכון ב- Project Service Automation. שינוי זה כבר הוגדר בתבנית עדכון נתונים בפועל של פרוייקט (Fin Ops ל- PSA).

### <a name="template-mapping-in-data-integration"></a>מיפוי תבנית בשילוב נתונים

האיורים הבאים מציגים דוגמאות למיפויי משימות התבנית בשילוב נתונים. המיפוי מציג את פרטי השדה שיסונכרנו מ- Finance ל- Project Service Automation.

[![מיפוי תבנית](./media/ActualsUpdateMapping.jpg)](./media/ActualsUpdateMapping.jpg)

[![מיפוי תבנית](./media/TransactionConnectionsUpdate.jpg)](./media/TransactionConnectionsUpdate.jpg)
