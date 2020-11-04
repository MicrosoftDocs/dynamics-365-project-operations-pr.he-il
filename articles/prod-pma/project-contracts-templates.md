---
title: סנכרון חוזי פרויקטים ופרויקטים ישירות מ- Project Service Automation ל- Finance and Operations
description: נושא זה מתאר את התבנית ואת המשימות הבסיסיות המשמשות לסנכרון חוזי פרויקטים ופרויקטים ישירות מ- Microsoft Dynamics 365 Project Service Automation אל Dynamics 365 Finance.
author: Yowelle
manager: AnnBe
ms.date: 09/09/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2017-12-13
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 9e4f11ec0bb88ed0971a3d082e7ca7823fcf8453
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077442"
---
# <a name="synchronize-project-contracts-and-projects-directly-from-project-service-automation-to-finance-and-operations"></a>סנכרון חוזי פרויקטים ופרויקטים ישירות מ- Project Service Automation ל- Finance and Operations

[!include[banner](../includes/banner.md)]

נושא זה מתאר את התבנית ואת המשימות הבסיסיות המשמשות לסנכרון חוזי פרויקטים ופרויקטים ישירות מ- Dynamics 365 Project Service Automation אל Dynamics 365 Finance.

> [!NOTE] 
> אם אתה משתמש ב- Enterprise edition 7.3.0, עליך להתקין את KB 4074835.

## <a name="data-flow-for-project-service-automation-to-finance"></a>זרימת נתונים עבור Project Service Automation ל- Finance

> [!NOTE]
> לפני שתוכל להשתמש בפתרון השילוב Project Service Automation ל- Finance, עליך להכיר את תכונת השילוב של נתוני Dynamics 365.

פתרון השילוב Project Service Automation ל- Finance משתמש בתכונת שילוב הנתונים לסנכרון נתונים במופעים של Project Service Automation ו- Finance. תבנית השילוב שזמינה עם תכונת שילוב הנתונים מאפשרת זרימת נתונים על חוזי פרויקט, פרויקטים, סעיפי חוזה של פרויקט ואבני דרך בסעיפי חוזה של פרויקט מ- Project Service Automation ל- Finance.

האיור הבא מראה כיצד הנתונים מסונכרנים בין Project Service Automation ו- Finance.

[![זרימת נתונים לשילוב Project Service Automation עם Finance](./media/ProjectsAndContractsFlow_upd.JPG)](./media/ProjectsAndContractsFlow.JPG)

## <a name="templates-and-tasks"></a>תבניות ומשימות

כדי לגשת לתבניות הזמינות, במרכז הניהול של Microsoft Power Apps, בחר **פרויקטים** ולאחר מכן, בפינה העליונה, בחר **פרויקט חדש** כדי לבחור תבניות ציבוריות.

התבניות והמשימות הבסיסיות הבאות משמשות לסנכרון חוזי פרויקטים ופרויקטים מ- Project Service Automation אל Finance:

### <a name="integrating-with-dynamics-365-project-service-automation-v2x"></a>שילוב עם Dynamics 365 Project Service Automation v2.x
- **שם התבנית בשילוב נתונים:** פרויקטים וחוזים (PSA ל- Fin and Ops)
- **שם המשימות בפרויקט:**

    - חוזי פרויקטים - PSA ל- Fin and Ops
    - פרויקטים - PSA ל- Fin and Ops
    - סעיפי חוזה בפרויקט - PSA ל- Fin and Ops
    - אבני דרך בסעיפי חוזה בפרויקט - PSA ל- Fin and Ops
  
### <a name="integrating-with-dynamics-365-project-service-automation-v3x"></a>שילוב עם Dynamics 365 Project Service Automation v3.x
יש שינוי בסכימה ב- Project Service Automation שמשפיע על תבנית אבן הדרך בסעיף החוזה בפרויקט ונדרש שימוש בגירסה v2 של התבנית כדי לשלב את Project Service Automation v3.x עם Dynamics 365.

- **שם התבנית בשילוב נתונים:** פרויקטים וחוזים (PSA 3.x ל- Fin and Ops)‏ - v2
- **שם המשימות בפרויקט:**

    - חוזי פרויקטים - PSA ל- Fin and Ops
    - פרויקטים - PSA ל- Fin and Ops
    - סעיפי חוזה בפרויקט - PSA ל- Fin and Ops
    - אבני דרך בסעיפי חוזה בפרויקט - PSA ל- Fin and Ops

עליך לסנכרן תיקי לקוחות לפני שתוכל לסנכרן חוזי פרויקטים ופרויקטים.

## <a name="entity-set"></a>קבוצת ישויות

| Project Service Automation       | כספים                                                |
|----------------------------------|--------------------------------------------------------|
| הזמנות                           | ישות שילוב לחוזה פרויקט                |
| פרויקטים                         | ישות שילוב לפרויקט                         |
| שורות הזמנה                      | ישות שילוב לסעיף חוזה בפרויקט           |
| אבני דרך של סעיף חוזה פרויקט | ישות שילוב לאבן דרך של סעיף חוזה בפרויקט |

## <a name="entity-flow"></a>זרימת ישות

חוזי פרויקטים מנוהלים ב- Project Service Automation והם מסונכרנים ל- Finance כחוזי פרויקט. כחלק מתבנית השילוב, תוכל להגדיר את מקור השילוב ב- Finance עבור חוזה הפרויקט.

פרויקט זמן וחומר ופרויקטי מחיר קבוע מנוהלים ב- Project Service Automation והם מסונכרנים ל- Finance כפרויקטים. כחלק משילוב התבנית, תוכל להגדיר את מקור השילוב ב- Finance עבור חוזה הפרויקט.

סעיפי חוזה בפרויקט מנוהלים ב- Project Service Automation והם מסונכרנים ל- Finance ככללי חיוב בחוזה פרויקט. אם שיטת החיוב שונה מסוג הפרויקט המוגדר כברירת מחדל, הסנכרון מעדכן את סוג הפרויקט עבור פרויקט בסעיף חוזה וקבוצת פרויקטים.

אבני דרך של סעיפי חוזה בפרויקט מנוהלים ב- Project Service Automation והם מסונכרנים ל- Finance כאבני דרך בכללי חיוב בחוזה פרויקט.

## <a name="project-service-automation-to-finance-integration-solution"></a>פרויקט שילוב Project Service Automation ל-Finance

השדה **מזהה חוזה פרויקט** זמין בדף **חוזי פרויקט**. שדה זה הפך למפתח טבעי וייחודי כדי לתמוך בשילוב.

כשנוצר חוזה פרויקט חדש, אם לא היה קיים כבר ערך של **מזהה חוזה פרויקט** , הוא ייווצר באופן אוטומטי באמצעות רצף מספרים. הערך מורכב מ- **ORD** ואחריו רצף מספרים הגדלים בהפרש קבוע ולאחר מכן סיומת של שישה תווים. הנה דוגמה: **ORD-01022-Z4M9Q0**.

השדה **מספר פרויקט** זמין בדף **פרויקטים**. שדה זה הפך למפתח טבעי וייחודי כדי לתמוך בשילוב.

כשנוצר פרויקט חדש, אם לא היה קיים כבר ערך של **מספר פרויקט** , הוא ייווצר באופן אוטומטי באמצעות רצף מספרים. הערך מורכב מ- **PRJ** ואחריו רצף מספרים הגדלים בהפרש קבוע ולאחר מכן סיומת של שישה תווים. הנה דוגמה: **PRJ-01049-CCNID0**.

בעת החלת פתרון שילוב Project Service Automation ל- Finance, קובץ Script לשדרוג קובע את השדה **מזהה חוזה פרויקט** עבור חוזי פרויקטים קיימים ואת השדה **מספר פרויקט** עבור פרויקטים קיימים ב- Project Service Automation.

## <a name="prerequisites-and-mapping-setup"></a>דרישות מוקדמות והגדרת מיפוי

- עליך לסנכרן תיקי לקוחות לפני שתוכל לסנכרן חוזי פרויקטים ופרויקטים.
- בקבוצת החיבורים, הוסף את מיפוי שדה מפתח השילוב עבור **msdyn\_organizationalunits** אל **msdyn\_name \[Name\]**. ייתכן שיהיה עליך תחילה להוסיף פרויקט לקבוצת החיבורים. לקבלת מידע נוסף, ראה [שילוב נתונים אל Common Data Service עבור יישומים](https://docs.microsoft.com/powerapps/administrator/data-integrator).
- בקבוצת החיבורים, הוסף את מיפוי שדה מפתח השילוב עבור **msdyn\_projects** אל **msdynce\_projectnumber \[Project Number\]**. ייתכן שיהיה עליך תחילה להוסיף פרויקט לקבוצת החיבורים. לקבלת מידע נוסף, ראה [שילוב נתונים אל Common Data Service עבור יישומים](https://docs.microsoft.com/powerapps/administrator/data-integrator).
- **SourceDataID** עבור חוזי פרויקטים וניתן לעדכן פרויקטים לערך שונה או להסיר מהמיפוי. ערך התבנית המוגדרת כברירת מחדל הוא **Project Service Automation**.
- יש לעדכן את המיפוי **PaymentTerms** כך שהוא ישקף תנאי תשלום חוקיים ב- Finance. בנוסף, תוכל להסיר את המיפוי ממשימת הפרויקט. במפת ערך ברירת המחדל יש ערכי ברירת מחדל לנתוני הדגמה. הטבלה הבאה מציגה את הערכים ב- Project Service Automation.

    | ערך | תיאור   |
    |-------|---------------|
    | 1     | שוטף+30        |
    | 2     | ‏‫שוטף+30, 10 2%‬ |
    | 3     | שוטף+‏45        |
    | 4     | שוטף+‏60        |

## <a name="power-query"></a>Power Query

עליך להשתמש ב- Microsoft Power Query for Excel כדי לסנן נתונים אם מתקיימים התנאים הבאים:

- יש לך הזמנות מכירה ב- Dynamics 365 Sales.
- יש לך יחידות ארגוניות מרובות ב- Project Service Automation והיחידות הארגוניות האלה ימופו לכמה ישויות משפטיות ב- Finance.

אם עליך להשתמש ב- Power Query, פעל לפי ההנחיות הבאות:

- התבנית פרויקטים וחוזים (PSA ל- Fin and Ops) כוללת מסנן ברירת מחדל שכולל רק הזמנות מכירות מסוג **Work item (msdyn\_ordertype = 192350001)‎**. מסנן זה עוזר להבטיח כי לא נוצרים חוזי פרויקט להזמנות מכירה ב- Finance. אם אתה יוצר תבנית משלך, עליך להוסיף מסנן זה.
- עליך ליצור מסנן Power Query שכולל רק את ארגוני החוזה שיש לסנכרן לישות המשפטית של קבוצת חיבורי השילוב. לדוגמה, יש לסנכרן חוזי פרויקטים שיש לך עם היחידה הארגונית של החוזה של Contoso US עם הישות המשפטית USSI, אך יש לסנכרן את חוזי הפרויקט שיש לך עם היחידה הארגונית של החוזה של Contoso Global עם הישות המשפטית USMF. אם לא תוסיף מסנן זה למיפוי המשימות, כל חוזי הפרויקט יסונכרנו עם הישות המשפטית שהוגדרה עבור קבוצת החיבורים, ללא קשר ליחידה הארגונית של החוזה.

## <a name="template-mapping-in-data-integration"></a>מיפוי תבנית בשילוב נתונים

> [!NOTE] 
> השדות **CustomerReference** ,‏ **AddressCity** , **AddressCountryRegionID** ,‏ **AddressDescription** ,‏ **AddressLine1** ,‏ **AddressLine2** ,‏ **AddressState** ו- **AddressZipCode** לא כלולים במיפוי ברירת המחדל עבור חוזי פרויקטים. באפשרותך להוסיף את המיפויים אם סנכרון נתונים אלו נדרש לחוזי פרויקט.
>
> השדות **Description** ,‏ **ParentID** ,‏ **ProjectGroup** ‏, **ProjectManagerPersonnelNumber** ו- **ProjectType** אינם כלולים במיפוי ברירת המחדל עבור פרויקטים. באפשרותך להוסיף את המיפויים אם סנכרון נתונים אלו נדרש לפרויקטים.

האיורים הבאים מציגים דוגמאות למיפויי משימות התבנית בשילוב נתונים. המיפוי מציג את פרטי השדה שיסונכרנו מ- Project Service Automation ל- Finance.

[![מיפוי תבניות חוזה בפרויקט](./media/ProjectContractTemplateMapping.JPG)](./media/ProjectContractTemplateMapping.JPG)

[![מיפוי תבניות בפרויקט](./media/ProjectTemplateMapping.JPG)](./media/ProjectTemplateMapping.JPG)

[![מיפוי תבניות סעיפי חוזה בפרויקט](./media/ProjectContractLinesMapping.JPG)](./media/ProjectContractLinesMapping.JPG)

[![מיפוי תבניות ציוני דרך של סעיפי חוזה בפרויקט](./media/ProjectContractLineMilestonesMapping.JPG)](./media/ProjectContractLineMilestonesMapping.JPG)

#### <a name="project-contract-line-milestone-mapping-in-the-projects-and-contracts-psa-3x-to-dynamics---v2-template"></a>מיפוי אבן דרך לסעיף חוזה של פרויקט בתבנית פרויקטים וחוזים (PSA 3.x ל- Dynamics) ‏- v2:

[![מיפוי ציוני דרך של סעיפי חוזה בפרויקט ותבנית של גרסה שנייה](./media/ProjectContractLineMilestoneMapping_v2.jpg)](./media/ProjectContractLineMilestoneMapping_v2.jpg)
