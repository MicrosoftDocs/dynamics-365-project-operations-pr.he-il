---
title: סנכרון נתונים בפועל של פרויקט ישירות מ- Project Service Automation ליומן שילוב הפרויקט עבור רישום ב- Finance and Operations
description: נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון נתונים בפועל של פרויקט ישירות מ- Microsoft Dynamics 365 Project Service Automation אל Finance and Operations.
author: Yowelle
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 11ccbd64c37341b2969e10e9a737f1aa4b4a61f9
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289685"
---
# <a name="synchronize-project-actuals-directly-from-project-service-automation-to-the-project-integration-journal-for-posting-in-finance-and-operations"></a>סנכרון נתונים בפועל של פרויקט ישירות מ- Project Service Automation ליומן שילוב הפרויקט עבור רישום ב- Finance and Operations

[!include[banner](../includes/banner.md)]

נושא זה מתאר את התבניות ואת המשימות הבסיסיות המשמשות לסנכרון נתונים בפועל של פרויקט ישירות מ- Dynamics 365 Project Service Automation אל Dynamics 365 Finance.

התבנית מסנכרנת עסקאות מ- Project Service Automation לטבלת אחסון זמני ב- Finance. לאחר השלמת הסנכרון, **עליך** לייבא נתונים מטבלת האחסון הזמני אל יומן השילוב.

> [!NOTE]
> - שילוב נתונים בפועל של פרויקט יהיה זמין החל מגירסה 8.0.1 ואילך.
> - אם אתה משתמש ב- Enterprise Edition 7.3.0 לאחר התקנת KB 4132657 ו- KB 4132660, תוכל להשתמש בתבניות לשילוב משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונתונים בפועל, וכן להגדיר תצורה של נעילת פונקציונליות. אם עליך לאפס את ההפצות החשבונאיות, מומלץ להתקין גם את KB 4131710.
> - אם אתה משתמש בגירסה 7.3.0 ואתה מעביר עסקאות עמלה מ- Project Service Automation, עליך להתקין את KB 4345320 כדי לכלול את העמלות בחשבונית הפרויקט.
> - אם אתה מזין סכומי מס מכירות בעסקאות הוצאה או שעות ב- Project Service Automation, עליך להתקין את עדכון 7 של Project Service Automation. אחרת, הנתונים בפועל של המס לא יקושרו לנתונים בפועל של ההוצאות או השעות המשויכות והם לא יסונכרנו אל Finance. לקבלת מידע נוסף, פנה לתמיכה.

## <a name="data-flow-for-project-service-automation-to-finance"></a>זרימת נתונים עבור Project Service Automation ל- Finance

פתרון השילוב Project Service Automation ל- Finance משתמש בתכונת שילוב הנתונים לסנכרון נתונים במופעים של Project Service Automation ו- Finance. תבניות השילוב שזמינות עם תכונת שילוב הנתונים מאפשרות זרימת נתונים על נתונים בפועל של פרויקט מ- Project Service Automation ל- Finance.

האיור הבא מראה כיצד הנתונים מסונכרנים בין Project Service Automation ו- Finance.

[![זרימת נתונים לשילוב Project Service Automation עם Finance and Operations](./media/ProjectActualsFlow.jpg)](./media/ProjectActualsFlow.jpg)

## <a name="project-actuals-from-project-service-automation"></a>נתונים בפועל של פרויקט מ- Project Service Automation

### <a name="template-and-tasks"></a>תבנית ומשימות

כדי לגשת לתבניות הזמינות, במרכז הניהול של Microsoft Power Apps, בחר **פרויקטים** ולאחר מכן, בפינה העליונה, בחר **פרויקט חדש** כדי לבחור תבניות ציבוריות.

התבנית והמשימות הבסיסיות הבאות משמשות לסנכרון נתונים בפועל של פרויקט מ- Project Service Automation אל Finance:

- **שם התבנית בשילוב נתונים:** נתונים בפועל של פרויקט (PSA ל- Fin and Ops)
- **שם המשימות בפרויקט:**

    - נתונים בפועל
    - TransactionConnections

### <a name="entity-set"></a>קבוצת ישויות

| Project Service Automation | כספים                                   |
|----------------------------|----------------------------------------------------------|
| נתונים בפועל                    | ישות שילוב לנתונים בפועל של פרויקט                   |
| חיבורי עסקה    | ישות שילוב ליחסי גומלין של עסקה בפרויקט |

### <a name="entity-flow"></a>זרימת ישות

נתונים בפועל של פרויקט מנוהלים ב- Project Service Automation והם מסונכרנים ליומן שילוב הפרויקט ב- Finance. החשבונאות תוחל על סמך הממדים הכספיים בברירת המחדל והגדרת הרישום.

### <a name="prerequisites"></a>דרישות מוקדמות

לפני שיתרחש סנכרון של נתונים בפועל, עליך להגדיר את התצורה של פרמטרי השילוב של Project Service Automation ולסנכרן פרויקטים, משימות פרויקט וקטגוריות עסקאות של הוצאות בפרויקט.

### <a name="power-query"></a>Power Query

בתבנית נתונים בפועל של פרויקט, עליך להשתמש ב- Microsoft Power Query for Excel כדי להשלים את המשימות הבאות:

- שנה את סוג העסקה ב- Project Service Automation לסוג העסקה הנכון ב- Finance. שינוי זה כבר הוגדר בתבנית נתונים בפועל של פרויקט (PSA ל- Fin and Ops).
- שנה את סוג החיוב ב- Project Service Automation לסוג החיוב הנכון ב- Finance. שינוי זה כבר הוגדר בתבנית נתונים בפועל של פרויקט (PSA ל- Fin and Ops). לאחר מכן, סוג החיוב ימופה אל מאפיין השורה, בהתאם לתצורה בדף **פרמטרי שילוב של Project Service Automation**.
- יש לסנכרן סינון ליחידות ארגוניות ספציפיות של משאב באמצעות תבנית זו.
- אם נתונים בפועל של שעות בין-חברתיות או הוצאות בין-חברתיות יסונכרנו ל- Finance, עליך לשנות את היחידה הארגונית של החוזה לישות המשפטית הנכונה ב- Finance. בתבנית נתונים בפועל של פרויקט (PSA ל- Fin and Ops), עמודה מותנית מוגדרת בהתאם לנתוני ההדגמה. עליך לעדכן את העמודה המותנית שהוכנסה לאחרונה לישויות המשפטיות הנכונות. אחרת, עלולה להתרחש שגיאת שילוב או ייבוא של עסקאות בפועל שגויות אל Finance.
- אם לא יסונכרנו הנתונים בפועל של שעות בין-חברתיות והוצאות בין-חברתיות ל- Finance, עליך למחוק את העמודה המותנית האחרונה שהוכנסה מהתבנית. אחרת, עלולה להתרחש שגיאת שילוב או ייבוא של עסקאות בפועל שגויות אל Finance.

#### <a name="contract-organizational-unit"></a>יחידה ארגונית של חוזה
כדי לעדכן את העמודה המותנית שהוכנסה בתבנית, לחץ על החץ **מפה** כדי לפתוח את המיפוי. בחר בקישור **שאילתות וסינון מתקדמים** כדי לפתוח את Power Query.

- אם אתה משתמש בתבנית ברירת מחדל לנתונים בפועל של פרויקט (PSA ל- Fin and Ops), ב- Power Query, בחר באפשרות האחרונה **תנאי שהוכנס** במקטע **שלבים שהוחלו**. בערך **פונקציה**, החלף את **USSI** בשם של הישות המשפטית שתהיה בשימוש בשילוב. הוסף תנאים נוספים לערך **פונקציה** כנדרש ועדכן את התנאי **else** מ- **USMF** לישות המשפטית הנכונה.
- אם אתה יוצר תבנית חדשה, עליך להוסיף את העמודה כדי לתמוך בשעות והוצאות בין-חברתיות. בחר **הוסף עמודה מותנית** והזן שם לעמודה, כגון **LegalEntity**. הזן תנאי עבור העמודה, שבו, אם **msdyn\_contractorganizationalunitid.msdyn\_name** הוא \<organizational unit\>, אז \<enter the legal entity\>; אחרת Null.

### <a name="template-mapping-in-data-integration"></a>מיפוי תבנית בשילוב נתונים

האיורים הבאים מציגים דוגמה למיפוי משימת התבנית בשילוב נתונים. המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.

[![מיפוי תבניות - ‏‫נתונים בפועל](./media/ActualsMapping.jpg)](./media/ActualsMapping.jpg)

[![מיפוי תבניות - חיבורי עסקאות](./media/TransactionConnections.jpg)](./media/TransactionConnections.jpg)

## <a name="import-from-staging-table-after-integration-from-project-service-automation"></a>ייבוא מטבלת אחסון זמני לאחר שילוב מ- Project Service Automation

יש להפעיל את התהליך התקופתי לייבוא מטבלת אחסון זמני לאחר סנכרון של נתונים בפועל מ- Project Service Automation אל Finance. תהליך זה ייבא את עסקאות הפרויקט מטבלת האחסון הזמני אל יומן שילוב Project Service Automation, שבו החשבונאות חלה וניתן לרשום את העסקאות שיובאו. מומלץ להפעיל תהליך זה במצב אצווה; באפשרותך להגדיר אותו כך שיפעל כאצווה חוזרת.

## <a name="update-actuals-from-finance"></a>עדכון נתונים בפועל מ- Finance

### <a name="template-and-tasks"></a>תבנית ומשימות

התבנית והמשימות הבסיסיות הבאות משמשות לסנכרון מספר השובר ומסי המכירות עבור עסקאות פרויקט שנרשמו מ- Finance ל- Project Service Automation:

- **שם התבנית בשילוב נתונים:** עדכון נתונים בפועל של פרויקט (Fin Ops ל- PSA)
- **שם המשימות בפרויקט:**

    - נתונים בפועל 
    - TransactionConnections

### <a name="entity-set"></a>קבוצת ישויות

| כספים                                                  | Project Service Automation |
|----------------------------------------------------------|----------------------------|
| ישות שילוב לנתונים בפועל של פרויקט                   | נתונים בפועל                    |
| ישות שילוב ליחסי גומלין של עסקה בפרויקט | חיבורי עסקה    |

### <a name="entity-flow"></a>זרימת ישות

נתונים בפועל של פרויקט מנוהלים ב- Project Service Automation והם מסונכרנים ליומן שילוב הפרויקט ב- Finance. לאחר רישום נתונים בפועל ב- Finance, הם מעודכנים ב- Project Service Automation עם מספר השובר מ- Finance. אם מסי המכירות התווספו ב- Finance, נוצרים נתונים בפועל חדשים למסים ב- Project Service Automation.

### <a name="power-query"></a>Power Query

בתבנית עדכון נתונים בפועל של פרויקט, עליך להשתמש ב- Power Query כדי להשלים את המשימות הבאות:

- שנה את סוג העסקה ב- Finance לסוג העסקה הנכון ב- Project Service Automation. שינוי זה כבר הוגדר בתבנית עדכון נתונים בפועל של פרויקט (Fin Ops ל- PSA).
- שנה את סוג החיוב ב- Finance לסוג החיוב הנכון ב- Project Service Automation. שינוי זה כבר הוגדר בתבנית עדכון נתונים בפועל של פרויקט (Fin Ops ל- PSA).

### <a name="template-mapping-in-data-integration"></a>מיפוי תבנית בשילוב נתונים

האיורים הבאים מציגים דוגמאות למיפויי משימות התבנית בשילוב נתונים. המיפוי מציג את פרטי השדה שיסונכרנו מ- Finance ל- Project Service Automation.

[![מיפוי תבניות - ‏‫עדכון נתונים בפועל](./media/ActualsUpdateMapping.jpg)](./media/ActualsUpdateMapping.jpg)

[![מיפוי תבניות - ‏‫עדכון עסקאות](./media/TransactionConnectionsUpdate.jpg)](./media/TransactionConnectionsUpdate.jpg)


[!INCLUDE[footer-include](../includes/footer-banner.md)]