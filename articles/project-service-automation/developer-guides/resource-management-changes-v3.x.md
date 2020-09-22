---
title: שינויים בניהול משאבים (Project Service Automation 3.x)
description: נושא זה מספק מידע על השינויים בתחום ניהול המשאבים.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 03/18/2019
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 25fafd22-fe94-4865-8d4d-3e6582c999d5
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
ms.openlocfilehash: e00ce5a9604e25764567a3f9d38ec85aec4245d4
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751823"
---
# <a name="resource-management-changes-project-service-automation-3x"></a>שינויים בניהול משאבים (Project Service Automation 3.x)

הסעיפים של נושא זה מספקים מידע על השינויים שבוצעו בתחום ניהול המשאבים של Dynamics 365 Project Service Automation גירסה ‎3.x.

## <a name="project-estimates"></a>הערכות פרוייקט

במקום להתבסס על הישות **msdyn\_projecttask** (**משימת פרוייקט‬**), הערכות הפרוייקט מבוססות על הישות **msdyn\_resourceassignment** (**הקצאת משאבים‬**). הקצאות המשאבים הפכו ל"מקור אמת" לתזמון ולתמחור של משימות.

## <a name="line-tasks"></a>משימות שורה

ב- PSA 3.x, משימות שורה הן מיושנות (לא בשימוש). ההקצאות מצביעות כעת על המשימה כולה, במקום על משימות השורה.

הדוגמה הבאה מראה כיצד משימה ששמה "משימת בדיקה" מוקצית לחברי הצוות A ו- B בגירסאות קודמות של PSA וב-PSA 3.x.

- **לפני PSA 3.x:**

    - משימת בדיקה

        - משימת בדיקה - משימת שורה 1

            - הקצאה ל- A

        - משימת בדיקה - משימת שורה 2

            - הקצאה ל- B

- **PSA 3.x:**

    - משימת בדיקה

        - הקצאה ל- A
        - הקצאה ל- B

## <a name="unassigned-assignment"></a>הקצאה לא מוקצית

ב- PSA 3.x, הקצאה לא מוקצית היא הקצאה המוקצית לחבר צוות **NULL** ולמשאב **NULL**. הקצאות לא מוקצות יכולות להתרחש במספר תרחישים:

- אם נוצרה משימה, אך היא עדיין לא הוקצתה לאף חבר צוות, נוצרת תמיד הקצאה לא מוקצית. 
- אם הוסרו כל מקבלי ההקצאות במשימה, הקצאה לא מוקצית נוצרת מחדש עבור אותה משימה.

## <a name="scheduling-fields-on-the-project-task-entity"></a>תזמון שדות בישות 'משימת פרוייקט'

השדות בישות **msdyn\_projecttask** הוצאו משימוש או הועברו לישות **msdyn\_resourceassignment**, או שכעת מתבצעת אליהם הפניה מהישות **msdyn\_projectteam** (**חבר צוות פרוייקט**).

| שדה לא בשימוש ב- msdyn\_projecttask (משימת פרוייקט) | שדה חדש ב- msdyn\_resourceassignment (הקצאת משאבים) | הערה |
|---|---|---|
| msdyn\_assignedresources | ללא | |
| msdyn\_assignedteammembers | ללא | |
| msdyn\_numberofresources | ללא | |
| msdyn\_scheduledhours | ללא | |
| msdyn\_effortcontour | msdyn\_plannedwork | התבנית של מבנה הנתונים JavaScript Object Notation ‏(JSON) המאוחסן בשדה שונתה. |

## <a name="schedule-contour"></a>מתאר לוח זמנים

מתאר לוח הזמנים מאוחסן בשדה **עבודה מתוכננת‬** (**msdyn\_plannedwork**) של כל ישות **הקצאת משאבים** (**msdyn\_resourceassignment**).

### <a name="structure"></a>מבנה

המבנה החדש של מתאר לוח הזמנים מורכב מפרוסות זמן גמישות המוגדרות עבור כל יום בלוח הזמנים. כל פרוסת זמן כוללת את המאפיינים הבאים:

- **התחלה** - תחילת שעות העבודה באותו יום, לפי לוח השנה של הפרוייקט.
- **סיום** - סיום שעות העבודה באותו יום, לפי לוח השנה של הפרוייקט.
- **שעות** - מספר השעות המוקצות ביום.

**דוגמה**

דוגמה זו משתמשת בלוח שנה של פרוייקט שבו יום העבודה מתקיים בין השעות 09:00 ל- 17:00 באזור הזמן UTC-8.

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

### <a name="auto-scheduling-and-manual-scheduling"></a>תזמון אוטומטי ותזמון ידני

אם משימה מתוזמנת באופן אוטומטי, השעות נטענות מראש וייתכן שמשך המשימה יתקצר.

**דוגמה**

המשימה הבאה מתוזמנת באופן אוטומטי במשך 18 שעות על-פני שלושה ימים (3 בדצמבר 2018 עד 5 בדצמבר 2018).

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

אם משימה מתוזמנת באופן ידני, השעות מתחלקות באופן שווה בין כל התאריכים.

**דוגמה**

המשימה הבאה מתוזמנת באופן ידני במשך 18 שעות על-פני שלושה ימים (3 בדצמבר 2018 עד 5 בדצמבר 2018).

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":6},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":6},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":6}]
```

### <a name="assignment-unit"></a>יחידת הקצאה

יחידת ההקצאה הוצאה משימוש ב- PSA 3.x. שעות המאמץ הדרושות למשימה מחולקות כעת באופן שווה, לכל יום, בין כל המשאבים שהוקצו.

**דוגמה**

בדוגמה זו, המשימה מוקצית לשני משאבים ומתוזמנת באופן אוטומטי עבור 36 שעות על-פני שלושה ימים (3 בדצמבר 2018 עד 5 בדצמבר 2018).

- הקצאה 1:

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

- הקצאה 2:

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

## <a name="pricing-dimensions"></a>ממדי תמחור

ב- PSA 3.x, שדות ממד תמחור ספציפיים למשאבים (כגון **תפקיד** ו**יחידה ארגונית**) הוסרו מהישות **msdyn‎\_projecttask‎**. כעת ניתן לאחזר שדות אלה מחבר צוות הפרוייקט המתאים (**msdyn\_projectteam**) של הקצאת המשאב (**msdyn\_resourceassignment**) כאשר הערכות הפרוייקט נוצרות. שדה חדש, **msdyn\_organizationalunit**, נוסף לישות **msdyn\_projectteam**.

| שדה לא בשימוש ב- msdyn\_projecttask (משימת פרוייקט) | שדה מ- msdyn\_projectteam (חבר צוות פרוייקט) המשמש במקום זאת |
|---|---|
| msdyn\_resourcecategory | msdyn\_resourcecategory |
| msdyn\_organizationalunit | msdyn\_organizationalunit |

## <a name="contours"></a>מתארים

שדות המתאר של התמחור וההערכה הוצאו משימוש בישות **msdyn\_projecttask**. הם הועברו לישות **msdyn\_resourceassignment**.

| שדה לא בשימוש ב- msdyn\_projecttask (משימת פרוייקט) | שדה חדש ב- msdyn\_resourceassignment (הקצאת משאבים) |
|---|---|
| msdyn\_costestimatecontour | msdyn\_plannedcostcontour |
| msdyn\_salesestimatecontour | msdyn\_plannedsalescontour |

השדות הבאים נוספו לישות **msdyn\_resourceassignment**:

* msdyn\_plannedcost
* msdyn\_plannedsales

השדות הבאים עבור עלות ומכירות 'מתוכננות', 'בפועל' ו'נותרו' לא השתנו בישות **msdyn\_projecttask**:

* msdyn\_plannedcost
* msdyn\_plannedsales
* msdyn\_actualcost
* msdyn\_actualsales
* msdyn\_remainingcost
* msdyn\_remainingsales
