---
title: שינוי בתכונות מ- Project Service Automation ל- Project Operations
description: נושא זה מספק סקירה כללית של השינויים בתכונות מ- Project Service Automation ל- Dynamics 365 Project Operations.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/03/2022
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
ms.openlocfilehash: 7e41b381d6da267f58174305f33fc229c66cd7b7
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8595407"
---
# <a name="feature-changes-from-project-service-automation-to-project-operations"></a>שינוי בתכונות מ- Project Service Automation ל- Project Operations

השדרוג מ- Dynamics 365 Project Service Automation ל- Lite Dynamics 365 Project Operations יסופק בשלושה שלבים. נושא זה מספק מידע על השינויים העיקריים שניתן לצפות להם עם סיום השדרוג.

| אספקת השדרוג | שלב 1 <br>(ינואר 2022) | שלב 2 <br>(גל אפריל 2022) | שלב 3  |
|------------------|------------------------|---------------------------|---------------------------|
| אין תלות במבנה התפלגות העבודה (WBS) עבור פרויקטים. | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| ה-WBS כלול במסגרת המגבלות של Project Operations שנתמכות כרגע. | &nbsp; | :heavy_check_mark: | :heavy_check_mark: |
| ה- WBS מחוץ למגבלות של Project Operations שנתמכות כרגע, כולל תמיכה ב- Project Desktop Client. | &nbsp; | &nbsp; | :heavy_check_mark: |

## <a name="project-management"></a>ניהול פרוייקט

השינויים המשמעותיים ביותר בחוויית המשתמש יהיו בתחום תכנון הפרויקט. Project Operations מאמצת חוויה מודרנית חדשה לניהול מבנה התפלגות עבודה (WBS) על ידי מינוף של יכולות התזמון הניתנות על ידי [Project for the Web](https://support.microsoft.com/en-us/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5).

## <a name="differences-in-the-scheduling-experience"></a>הבדלים בחוויית התזמון

הטבלה הבאה מסכמת את ההבדלים בתזמון בין Project Service Automation לבין Project Operations.

|  תזמון     |   Project Operations   |   PSA   |
|-----------------|------------------------|---------|
| תבניות פרויקט – יכולת להגדיר ולהחיל תבניות פרויקט בעת יצירת פרויקט  |  &nbsp;    | :heavy_check_mark: |
| אינטגרציה של מבנה התפלגות עבודה (WBS) עם לקוח שולחן עבודה   |    &nbsp;  | :heavy_check_mark: |
| אילוצים – להתחיל לא מוקדם מ- , לסיים לא יאוחר מ-  | :heavy_check_mark: |   &nbsp;  |
| אבני דרך – משימות ללא משך זמן   | :heavy_check_mark:  |  &nbsp;  |
| משימות מונחות-משאבים יכבדו את זמינות המשאבים שהוקצו   | :heavy_check_mark: |  &nbsp;    |
| עריכה לפי יחידות זמן – עריכת תוכניות ועבודה על בסיס יומיומי   |   &nbsp;  | :heavy_check_mark: |
| תזמון אוטומטי/ידני – שימוש במנוע תזמון הפרויקטים לתזמון משימות באופן אוטומטי או ידני |  &nbsp; | :heavy_check_mark:  |
| עריכת פרויקטים גדולים ישירות בממשק המשתמש: אין הגבלה לגודל התוכניות הניתנות לעריכה  | מגבלה של 500 משימות  | :heavy_check_mark:       |
| אחוז השלמה – סמן התקדמות המשימה   | :heavy_check_mark:  |  &nbsp;  |
| [מצבי לוח זמנים של פרויקט](../project-management/scheduling-modes.md) – הגדרת הפרויקט כיחידות קבועות, מאמץ קבוע או משך זמן קבוע | :heavy_check_mark: | &nbsp; |
| ציר זמן – בנייה והתאמה אישית של תצוגת ציר הזמן כדי להציג את פרטי לוח הזמנים באופן חזותי ולתקשר עם בעלי עניין. | :heavy_check_mark:  | &nbsp; |
| משימות מונחות-מאמצים – תמיעת מנגנון תזמון לתזמון משימה כמונחית-מאמץ  | :heavy_check_mark:  | &nbsp; |
| תיבת הדו-שיח **פרטי משימה** – שמירת פרטי משימה באמצעות תיבת דו-שיח | :heavy_check_mark:  |  &nbsp;  |
| גרירה ושחרור – בחירה מרובה של משימות ושינוי מיקומן ב- WBS | :heavy_check_mark: | &nbsp;  |
| תצוגות מתמשכות גמישות – הגדרת תצוגות מפורטות יותר של תכונות המשימה   | :heavy_check_mark:  | &nbsp; |
| מיון וסינון של ה- WBS  | :heavy_check_mark:  | &nbsp; |
| תצוגת לוחות למסירת פרויקט ללא מפל מים  | :heavy_check_mark:   | &nbsp; |
| תצוגת ציר זמן – תרשים גנט אינטראקטיבי המשמש להמחשה ועריכה של ה- WBS   | :heavy_check_mark:  | &nbsp; |
| קיצורי מקלדת – שימוש בקיצורי מקלדת לפעולות נפוצות, כגון הזחה או הכנסה  | :heavy_check_mark:  |  &nbsp; |
| ביטול רב-שכבתי – ביצוע ניתוח 'מה-אם' כדי להבין באופן מלא את ההשפעה של שינויים על ידי היפוך והחלה מחדש של קבוצת פעולות שלמה | :heavy_check_mark: | &nbsp; |
| גזור/העתק/הדבק – שיתוף פעולה בפיתוח לוח זמנים על ידי העתקה והדבקה של פרטי לוח זמנים בין יישומים  | :heavy_check_mark: | &nbsp; |
| רשימות בדיקה של משימות – הוספה של עד 20 פריטי רשימת תיוג למשימה   | :heavy_check_mark: | &nbsp; |

## <a name="project-planning"></a>תכנון פרוייקטים

לדף ה **פרויקט** ב- Project Operations יש מספר משמעותי של הבדלים בהשוואה לדף ה **פרויקט** ב- Project Service Automation.

הפעולות הבאות הוסרו מהדף **פרויקטים** כחלק משדרוג שלב 1:

  - **פתח ב- MS Project**
  - **יצירת תבנית**
  - **בטל את הקישור ל- MS Project**

הדף **פרויקט** ב- Project Operations כולל את הכרטיסיות החדשות הבאות.

- **הערכות חומרים**
- **הגדרת חיוב משימה**

הכרטיסיה **סטטוס** הוסרה והשדה **סטטוס** נמצא כעת בכרטיסיה **סיכום** עם מצב התזמון של הפרויקט.

   ![עדכונים לדף 'פרויקט'.](media/projectform.png)

שם הכרטיסיה **לוח זמנים** שונה לכרטיסיה **משימה** והכרטיסיה כוללת את החווייה החדשה של תכנון הפרויקט עם Project for the Web.

   ![כרטיסיית משימות פרוייקט חדשה.](media/tasktab.png)

## <a name="scheduling-modes"></a>מצבי תזמון

Project Operations הציג תכונה חדשה, [מצבי תזמון ](../project-management/scheduling-modes.md). כל הפרויקטים הקיימים של Project Service Automation יוגדרו כברירת מחדל ל **משך זמן קבוע** ב- Project Operations. עם זאת, ניתן לנהל את ברירת המחדל עבור פרויקטים חדשים על ידי מעבר אל **הגדרות** > **פרמטרים** > **פרמטר** > **מצב לוח זמנים**.

   ![הגדרות הפרמטר של הפרויקט עבור מצב לוח זמנים.](media/projectparameter.png)

## <a name="project-planning-limits"></a>מגבלות של תכנון פרוייקטים

Project Operations מסתמך על Project for the Web עבור כל פעולות תזמון הפרויקט. Project for the Web מנהל את מבנה התפלגות העבודה תוך שימוש במגבלות בטבלה הבאה.

| **שדה**                                          | **מגבלה**             |
|----------------------------------------------------|-----------------------|
| מקסימום משימות עבור פרויקט                  | 500                   |
| מקסימום משך עבור פרויקט               | 3650 ימים (10 שנים)  |
| מקסימום משאבים עבור פרויקט              | 300                   |
| מקסימום קישורים (יורשים בלבד) עבור פרויקט | 600                   |
| מקסימום שדות בהתאמה אישית עבור פרויקט          | 10                    |
| רמת הירארכיה מקסימלית                            | 10 רמות             |
| מקסימום קישורים (עוקבים + קודמים)            | 20                    |
| משך מקסימלי של משימת עלה                      | 1250 ימים             |
| משך מקסימלי של משימת סיכום                 | 3650 ימים (10 שנים)  |
| מספר מקסימלי של משאבים המוקצים למשימה               | 20 משאבים          |
| טווח תאריכים נתמך עבור משימה                    | 1/1/2000 - 12/31/2149 |
| פריטים ברשימת פעולות לביצוע                                    | 20                    |

## <a name="project-planning-extensibility-and-development"></a>יכולת ההרחבה והפיתוח של תכנון פרויקטים

לאחר השדרוג ל- Project Operations, יש להשתמש בממשקי ה- API של 'שירות תזמון פרויקטים' כדי לבצע פעולות יצירה, עדכון ומחיקה של הישויות הבאות:

|   שם הישות           |   שם לוגי של ישות       |
|-------------------------|-----------------------------|
| פרויקט                 | msdyn_project               |
| משימת הפרוייקט            | msdyn_projecttask           |
| ‏‫יחס תלות במשימת פרוייקט | msdyn_projecttaskdependency |
| הקצאת משאבים     | msdyn_resourceassignment    |
| מיכל של פרוייקט          | msdyn_projectbucket         |
| חבר צוות פרויקט     | msdyn_projectteam           |

אם יש לך כרגע התאמות אישיות הכוללות ישויות אלה, ראה [השתמש בממשקי API של תזמון פרויקטים כדי לבצע פעולות עם ישויות תזמון](../project-management/schedule-api-preview.md) להנחיות יישום.

## <a name="data-model-changes"></a>שינויים במודל הנתונים

כחלק משדרוג שלב 1, ישנם שינויים במודל הנתונים. שינויים אלו הם בעיקר שינויים בשדה לגופים קיימים. בשלב 1, הישויות **msydn_project** ו- **msdyn_projectteam** הן שילוב מחדש של התאמות אישיות. 

> [!IMPORTANT]
> סעיף זה יעודכן עם ישויות נוספות לאחר השלמת שלבי השדרוג העתידיים.

השדות הבאים הוחלפו בשדות חדשים.

|   Entity          |   השם ישן של השדה   |   השם הלוגי החדש    |
|-------------------|----------------------|-----------------------|
| msdyn_project     | msdyn_actualhours    | msdyn_effortcompleted |
| msdyn_project     | msdyn_plannedhours   | msdyn_effort          |
| msdyn_project     | msdyn_remaininghours | msdyn_effortremaining |
| msdyn_project     | msdyn_scheduledend   | msdyn_finish          |
| msdyn_project     | msdyn_wbsduration    | msdyn_duration        |
| msdyn_projectteam | msdyn_assignedhours  | msdyn_effort          |
| msdyn_projectteam | msdyn_from           | msdyn_start           |
| msdyn_projectteam | msdyn_to             | msdyn_finish          |

השדות הבאים נוספו.

|   Entity          |   שם לוגי                               |   Description |
|-------------------|----------------------------------------------|---------------|
| msdyn_project     | msdyn_actualfeesales                         | מציג את הערך הצבור של מכירות תשלום בפועל‬ בפרוייקט. לשימוש ב- Project Service Automation בלבד. |
| msdyn_project     | msdyn_actualmaterialcost                     | מציג את העלות החומרית של ההוצאות בפועל בפרוייקט. לשימוש ב- Project Service Automation בלבד. |
| msdyn_project     | msdyn_actualmaterialsales                    | מציג את הערך הצבור של מכירות חומרים בפועל‬ בפרוייקט. לשימוש ב- Project Service Automation בלבד. |
| msdyn_project     | msdyn_businesscase                           |                |
| msdyn_project     | msdyn_contractlineproject                    | סעיף החוזה שמשויך לפרוייקט זה. |
| msdyn_project     | msdyn_copyprojectcorrelationid               | זהו שדה מערכת פנימי המשמש עבור **העתקת פרויקט** שקשור למזהה מתאם. לשימוש ב- Project Service Automation בלבד. |
| msdyn_project     | msdyn_copyprojectsessionid                   | זהו שדה מערכת פנימי המשמש עבור **העתקת פרויקט** שקשור למזהה הפעלה. לשימוש ב- Project Service Automation בלבד. |
| msdyn_project     | msdyn_globalrevisiontoken                    | אסימון מהדורה כללית של xRM לסנכרון אחרון משירות תזמון הפרויקט. |
| msdyn_project     | msdyn_msprojectdocument                      | מסמך Microsoft Project השייך לפרוייקט. |
| msdyn_project     | msdyn_plannedmaterialcost                    | צבירת העלות החומרית המתוכננת בפרוייקט. לשימוש ב- Project Service Automation בלבד. |
| msdyn_project     | msdyn_plannedmaterialsales                   | צבירת המכירות החומריות המתוכננות בפרוייקט. לשימוש ב- Project Service Automation בלבד. |
| msdyn_project     | msdyn_program                                | התוכנית שפרויקט זה קשור אליה. |
| msdyn_project     | msdyn_quotelineproject                       | שורת הצעת המחיר שמשויכת לפרוייקט זה. |
| msdyn_project     | msdyn_replaylogheader                        | כותרת עבור יומני הפעלה חוזרת. |
| msdyn_project     | msdyn_schedulemode                           | מצב לוח זמנים המהווה ברירת מחדל ומשמש לכל המשימות בפרוייקט.  |
| msdyn_project     | msdyn_taskearlieststart                      | תאריך ההתחלה המוקדם ביותר של כל משימה בפרויקט.  |
| msdyn_project     | msdyn_valuestatement                         |                |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | חבר צוות הפרויקט שממנו הועתק חבר צוות הפרויקט הזה. |
| msdyn_projectteam | msdyn_creategenericteammemberwithrequirement | מציין אם ליצור את דרישת המשאב עבור חבר צוות כללי חדש שנוצר.  |
| msdyn_projectteam | msdyn_deletestatus                           | מצב המחיקה של חבר הצוות שיש לעקוב אם נשלחה בקשת מחיקה אל שירות תזמון הפרויקט, ואם PSS שולח בחזרה תשובה בהצלחה ובמסגרת חלון הזמן הצפוי. |
| msdyn_projectteam | msdyn_effortcompleted                        | עוקב אחר המאמץ שביצע חבר הצוות בהקצאות שלו. |
| msdyn_projectteam | msdyn_effortremaining                        | עוקב אחר המאמץ שמבוצע על ידי חבר הצוות בהקצאות שלו. |
| msdyn_projectteam | msdyn_markedfordeletiontimer                 | תקופת ההמתנה מרגע שחבר הצוות שולח בקשת מחיקה לשירות תזמון הפרויקט ועד למחיקה של חבר הצוות בפועל ב- Microsoft Dataverse.|
| msdyn_projectteam | msdyn_markedfordeletiontimestamp             | חותמת הזמן לתיעוד כאשר בקשת מחיקה של חבר צוות נשלחת אל שירות תזמון הפרויקט. |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | מציג את חבר צוות הפרויקט שממנו הועתק חבר צוות הפרויקט הזה.  |

## <a name="project-templates"></a>תבניות פרויקט

Project Operations אינו מספק תמיכה לתבניות פרויקט. עם זאת, ניתן לשכפל חלק גדול מפונקציונליות הליבה באמצעות [Project Copy API](../project-management/dev-copy-project.md).

## <a name="desktop-add-in-support"></a>תמיכה תוסף שולחן העבודה

תמיכה בתוסף שולחן העבודה של Microsoft Project לא תהיה זמינה בשני השלבים הראשונים של השדרוג. בשלב 3, לקוחות עם פרויקטים גדולים יותר מהמגבלות הנתמכות כיום של Project for the Web יוכלו להשתמש בתוסף שולחן העבודה.

## <a name="editing-resource-assignment-contours"></a>עריכת קווי מתאר של הקצאת משאבים

היכולת לערוך קווי מתאר של הקצאת משאבים תהיה זמינה כאשר שלב 2 של השדרוג יהיה זמין.

## <a name="billing-and-pricing"></a>חיוב ותמחור

התכונות החדשות הבאות נוספו ב- Project Operations. תכונות אלו הן תוספות בטבען ואינן משפיעות על מודל הנתונים של Project Service Automation.

- [רישום השימוש בחומרים בפרוייקטים ובמשימות הפרוייקט](../material/material-usage-log.md)
- [ניהול חוזי משנה](../pro/subcontracting/managing-subcontracts-overview.md)
- [חוזים מבוססי מקדמות וריטיינרים](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [חוזה מצב ואימות של 'אין לחרוג'](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- [חיוב מבוסס משימה](../pro/sales/mapping-projects-tasks-quote-line-sales.md)

## <a name="deprecated-components"></a>רכיבים שהוצאו משימוש

הטבלאות הבאות מתעדות את כל השדות שהוצאו משימוש שהועברו לפתרון הרכיבים שהוצא משימוש לאחר השדרוג. למידע נוסף וקישור לפתרון, ראה [Dynamics 365 Project Service Automation 3x ‏ל-Project Operations ‏‏4x רכיבים שהוצאו משימוש](https://github.com/microsoft/Dynamics365-Project-Operations-PowerApps/tree/main/3x-4x-deprecated-solution).

### <a name="invoicedetail"></a>invoicedetail

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
|invoicedetail.msdyn_contractline    |

### <a name="msdyn_actual"></a>msdyn_actual

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_actual.msdyn_salescontractline                                                          |

### <a name="msdyn_characteristicreqforteammember"></a>msdyn_characteristicreqforteammember

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_characteristicreqforteammember.msdyn_characteristic                                     |
| msdyn_characteristicreqforteammember.msdyn_characteristicreqforteammemberid                   |
| msdyn_characteristicreqforteammember.msdyn_characteristictype                                 |
| msdyn_characteristicreqforteammember.msdyn_name                                               |
| msdyn_characteristicreqforteammember.msdyn_ratingvalue                                        |
| msdyn_characteristicreqforteammember.msdyn_resourcerequirementid                              |

### <a name="msdyn_contractlineinvoiceschedule"></a>msdyn_contractlineinvoiceschedule

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_contractlineinvoiceschedule.msdyn_contractline                                          |
| msdyn_contractlinescheduleofvalue.msdyn_contractline                                          |
 
### <a name="msdyn_dataexport"></a>msdyn_dataexport

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_dataexport.msdyn_dataexportid                                                           |
| msdyn_dataexport.msdyn_datatoken                                                              |
| msdyn_dataexport.msdyn_entityname                                                             |
| msdyn_dataexport.msdyn_exportedrecordcount                                                    |
| msdyn_dataexport.msdyn_exportstatus                                                           |
| msdyn_dataexport.msdyn_linkedentitydata                                                       |
| msdyn_dataexport.msdyn_name                                                                   |
| msdyn_dataexport.msdyn_pagingdata                                                             |

### <a name="msdyn_fact"></a>msdyn_fact

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_fact.msdyn_salescontractline                                                            |

### <a name="msdyn_findworkevent"></a>msdyn_findworkevent

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_findworkevent.msdyn_bookableresource                                                    |
| msdyn_findworkevent.msdyn_findworkeventid                                                     |
| msdyn_findworkevent.msdyn_name                                                                |
| msdyn_findworkevent.msdyn_timestamp                                                           |
| msdyn_findworkevent.msdyn_type                                                                |
| msdyn_findworkevent.msdyn_value                                                               |
| msdyn_findworkevent.msdyn_work                                                                |

### <a name="msdyn_invoicelinetransaction"></a>msdyn_invoicelinetransaction

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_invoicelinetransaction.msdyn_invoiceline                                                |
| msdyn_invoicelinetransaction.msdyn_salescontractline                                          |

### <a name="msdyn_journalline"></a>msdyn_journalline

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_journalline.msdyn_salescontractline                                                     |

### <a name="msdyn_opportunitylineresourcecategory"></a>msdyn_opportunitylineresourcecategory

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylineresourcecategory.msdyn_billingtype                                       |
| msdyn_opportunitylineresourcecategory.msdyn_description                                       |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylineresourcecategoryid                 |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylinetransactionclassification          |
| msdyn_opportunitylineresourcecategory.msdyn_resourcecategory                                  |

### <a name="msdyn_opportunitylinetransaction"></a>msdyn_opportunitylinetransaction

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransaction.msdyn_accountcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_accountingdate                                         |
| msdyn_opportunitylinetransaction.msdyn_accountvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_amount                                                 |
| msdyn_opportunitylinetransaction.msdyn_amount_base                                            |
| msdyn_opportunitylinetransaction.msdyn_amountmethod                                           |
| msdyn_opportunitylinetransaction.msdyn_basisamount                                            |
| msdyn_opportunitylinetransaction.msdyn_basisamount_base                                       |
| msdyn_opportunitylinetransaction.msdyn_basisprice                                             |
| msdyn_opportunitylinetransaction.msdyn_basisprice_base                                        |
| msdyn_opportunitylinetransaction.msdyn_basisquantity                                          |
| msdyn_opportunitylinetransaction.msdyn_billingtype                                            |
| msdyn_opportunitylinetransaction.msdyn_bookableresource                                       |
| msdyn_opportunitylinetransaction.msdyn_contactcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_contactvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_customertype                                           |
| msdyn_opportunitylinetransaction.msdyn_description                                            |
| msdyn_opportunitylinetransaction.msdyn_documentdate                                           |
| msdyn_opportunitylinetransaction.msdyn_enddatetime                                            |
| msdyn_opportunitylinetransaction.msdyn_exchangeratedate                                       |
| msdyn_opportunitylinetransaction.msdyn_opportunityline                                        |
| msdyn_opportunitylinetransaction.msdyn_opportunitylinetransactionid                           |
| msdyn_opportunitylinetransaction.msdyn_percent                                                |
| msdyn_opportunitylinetransaction.msdyn_price                                                  |
| msdyn_opportunitylinetransaction.msdyn_price_base                                             |
| msdyn_opportunitylinetransaction.msdyn_pricelist                                              |
| msdyn_opportunitylinetransaction.msdyn_product                                                |
| msdyn_opportunitylinetransaction.msdyn_project                                                |
| msdyn_opportunitylinetransaction.msdyn_quantity                                               |
| msdyn_opportunitylinetransaction.msdyn_resourcecategory                                       |
| msdyn_opportunitylinetransaction.msdyn_resourceorganizationalunitid                           |
| msdyn_opportunitylinetransaction.msdyn_startdatetime                                          |
| msdyn_opportunitylinetransaction.msdyn_task                                                   |
| msdyn_opportunitylinetransaction.msdyn_transactioncategory                                    |
| msdyn_opportunitylinetransaction.msdyn_transactionclassification                              |
| msdyn_opportunitylinetransaction.msdyn_transactiontypecode                                    |
| msdyn_opportunitylinetransaction.msdyn_unit                                                   |
| msdyn_opportunitylinetransaction.msdyn_unitschedule                                           |
| msdyn_opportunitylinetransaction.msdyn_vendortype                                             |

### <a name="msdyn_opportunitylinetransactioncategory"></a>msdyn_opportunitylinetransactioncategory

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactioncategory.msdyn_billingtype                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_description                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactioncategoryid           |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactionclassification       |
| msdyn_opportunitylinetransactioncategory.msdyn_transactioncategory                            |

### <a name="msdyn_opportunitylinetransactionclassificatio"></a>msdyn_opportunitylinetransactionclassificatio

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactionclassificatio.msdyn_billingtype                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_description                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_include                                   |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunityline                           |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunitylinetransactionclassificatioid |
| msdyn_opportunitylinetransactionclassificatio.msdyn_transactionclassification                 |

### <a name="msdyn_orderlineresourcecategory"></a>msdyn_orderlineresourcecategory

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlineresourcecategory.msdyn_contractline                                            |

### <a name="msdyn_orderlinetransaction"></a>msdyn_orderlinetransaction

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransaction.msdyn_salescontractline                                            |
| msdyn_orderlinetransactioncategory.msdyn_contractline                                         |

### <a name="msdyn_orderlinetransactionclassification"></a>msdyn_orderlinetransactionclassification

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransactionclassification.msdyn_contractline                                   |

### <a name="msdyn_project"></a>msdyn_project

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_project.msdyn_actualdurationminutes                                                     |
| msdyn_project.msdyn_actualhours                                                               |
| msdyn_project.msdyn_istemplate                                                                |
| msdyn_project.msdyn_plannedhours                                                              |
| msdyn_project.msdyn_projecttemplate                                                           |
| msdyn_project.msdyn_remaininghours                                                            |
| msdyn_project.msdyn_scheduleddurationminutes                                                  |
| msdyn_project.msdyn_scheduledend                                                              |
| msdyn_project.msdyn_stagename                                                                 |
| msdyn_project.msdyn_wbsduration                                                               |


### <a name="msdyn_projecttask"></a>msdyn_projecttask

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttask.msdyn_actualdurationminutes                                                 |
| msdyn_projecttask.msdyn_actualeffort                                                          |
| msdyn_projecttask.msdyn_aggregationdirection                                                  |
| msdyn_projecttask.msdyn_assignedresources                                                     |
| msdyn_projecttask.msdyn_assignedteammembers                                                   |
| msdyn_projecttask.msdyn_autoscheduling                                                        |
| msdyn_projecttask.msdyn_costestimatecontour                                                   |
| msdyn_projecttask.msdyn_effortcontour                                                         |
| msdyn_projecttask.msdyn_islinetask                                                            |
| msdyn_projecttask.msdyn_numberofresources                                                     |
| msdyn_projecttask.msdyn_remaininghours                                                        |
| msdyn_projecttask.msdyn_resourceutilization                                                   |
| msdyn_projecttask.msdyn_salesestimatecontour                                                  |
| msdyn_projecttask.msdyn_scheduledhours                                                        |
| msdyn_projecttask.msdyn_wbsid                                                                 |

### <a name="msdyn_projecttaskstatususer"></a>msdyn_projecttaskstatususer

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttaskstatususer.msdyn_bookableresource                                            |
| msdyn_projecttaskstatususer.msdyn_description                                                 |
| msdyn_projecttaskstatususer.msdyn_expectedcompletiondate                                      |
| msdyn_projecttaskstatususer.msdyn_expectedhourstocomplete                                     |
| msdyn_projecttaskstatususer.msdyn_iscompleted                                                 |
| msdyn_projecttaskstatususer.msdyn_name                                                        |
| msdyn_projecttaskstatususer.msdyn_percentcomplete                                             |
| msdyn_projecttaskstatususer.msdyn_projecttaskid                                               |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatusindicator                                  |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatususerid                                     |

### <a name="msdyn_projectteam"></a>msdyn_projectteam

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteam.msdyn_applicantcount                                                        |
| msdyn_projectteam.msdyn_applicantsavailable                                                   |
| msdyn_projectteam.msdyn_assignedhours                                                         |
| msdyn_projectteam.msdyn_description                                                           |
| msdyn_projectteam.msdyn_from                                                                  |
| msdyn_projectteam.msdyn_hoursrequested                                                        |
| msdyn_projectteam.msdyn_membershipstatus                                                      |
| msdyn_projectteam.msdyn_number                                                                |
| msdyn_projectteam.msdyn_to                                                                    |

### <a name="msdyn_projectteammembersignup"></a>msdyn_projectteammembersignup

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteammembersignup.msdyn_bookableresource                                          |
| msdyn_projectteammembersignup.msdyn_membershipstatus                                          |
| msdyn_projectteammembersignup.msdyn_name                                                      |
| msdyn_projectteammembersignup.msdyn_projectteammembersignupid                                 |
| msdyn_projectteammembersignup.msdyn_teammembership                                            |

### <a name="msdyn_projecttransactioncategory"></a>msdyn_projecttransactioncategory

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttransactioncategory.msdyn_billingtype                                            |
| msdyn_projecttransactioncategory.msdyn_name                                                   |
| msdyn_projecttransactioncategory.msdyn_project                                                |
| msdyn_projecttransactioncategory.msdyn_projecttransactioncategoryid                           |
| msdyn_projecttransactioncategory.msdyn_transactioncategory                                    |

### <a name="msdyn_quotelineinvoiceschedule"></a>msdyn_quotelineinvoiceschedule

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_quotelineinvoiceschedule.msdyn_quoteline                                                |
| msdyn_quotelineresourcecategory.msdyn_quoteline                                               |
| msdyn_quotelinescheduleofvalue.msdyn_quoteline                                                |
| msdyn_quotelinetransaction.msdyn_quoteline                                                    |
| msdyn_quotelinetransactioncategory.msdyn_quoteline                                            |
| msdyn_quotelinetransactionclassification.msdyn_quoteline                                      |

### <a name="msdyn_resourceassignment"></a>msdyn_resourceassignment

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_resourceassignment.msdyn_hours                                                          |
| msdyn_resourceassignment.msdyn_fromdate                                                       |
| msdyn_resourceassignment.msdyn_msprojectclientid                                              |
| msdyn_resourceassignment.msdyn_todate                                                         |
| msdyn_resourceassignmentdetail.msdyn_duration                                                 |
| msdyn_resourceassignmentdetail.msdyn_from                                                     |
| msdyn_resourceassignmentdetail.msdyn_name                                                     |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentdetailid                               |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentid                                     |

### <a name="salesorderdetail"></a>salesorderdetail

| שדות                                                    |
|-----------------------------------------------------------------------------------------------|
| salesorderdetail.msdyn_quoteline                                                              |

