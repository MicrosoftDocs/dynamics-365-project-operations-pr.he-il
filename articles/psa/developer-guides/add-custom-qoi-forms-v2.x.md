---
title: הוספת טפסי ישות מותאמים אישית חדשים (Project Service Automation 2.x)
description: נושא זה מספק מידע אודות אופן הוספת טפסי ישות מותאמים אישית עבור הזדמנויות, הצעות מחיר, הזמנות או חשבוניות ב- Dynamics 365 Project Service Automation 2.x.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 3/14/2019
ms.topic: article
ms.service: business-applications
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 9c9e31dc6d4d5a8ad5cc568f2d7d673c8703936d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5284854"
---
# <a name="add-new-custom-entity-forms-project-service-automation-2x"></a>הוספת טפסי ישות מותאמים אישית חדשים (Project Service Automation 2.x)

[!include [banner](../../includes/psa-now-project-operations.md)]

## <a name="type-field"></a>שדה 'סוג' 

Dynamics 365 Project Service Automation מתבסס על השדה **סוג** (**msdyn\_ordertype**) של הישויות 'הזדמנות', 'הצעת מחיר', 'הזמנה' ו'חשבונית' כדי להבחין בין גירסאות **מבוססות-עבודה** של ישויות אלה לבין גירסאות **מבוססות-פריט** ו **מבוססות-שירות**. גירסאות מבוססות-עבודה של ישויות אלה מטופלות על-ידי PSA. לוגיקה עסקית רבה בצד הלקוח ובצד השרת של הפתרון תלויה בשדה **סוג**. לכן, חשוב שהשדה יאותחל עם ערך נכון בעת יצירת הישויות. ערך שגוי עלול לגרום לאופן פעולה שגוי, וייתכן שלוגיקה עסקית מסוימת לא תפעל כהלכה.

## <a name="automatic-form-switching"></a>החלפת טופס אוטומטית

כדי למנוע השחתת נתונים אפשרית ואופן פעולה לא צפוי שנגרמים על-ידי אתחול ועריכה שגויים של רשומות ישות המכירות, PSA כולל כעת לוגיקה עבור החלפת טפסים אוטומטית בטפסים מוכנים לשימוש. לוגיקה זו מעבירה משתמשים אל הטופס הנכון לעבודה עם הגירסה מבוססת העבודה או כל סוג אחר של ישות 'הזדמנות', 'הצעת מחיר', 'הזמנה' או 'חשבונית'. כאשר משתמש פותח גירסה מבוססת-עבודה של הישות 'הזדמנות', 'הצעת מחיר', 'הזמנה' או 'חשבונית', הטופס עובר אל **פרטי פרוייקט**.

הלוגיקה של החלפת הטופס האוטומטית מסתמכת על המיפוי בין הערך **formId** לשדה **msdyn\_ordertype**. כל הטפסים המוכנים לשימוש נוספו למיפוי זה. עם זאת, יש להוסיף באופן ידני טפסים מותאמים אישית כדי לציין באיזו גירסה של הישות הם נועדו לטפל. זה מבוסס על השדה **msdyn\_ordertype**. אם החלפת הטופס חסרה במיפוי, הלוגיקה תעבור לטופס המוכן לשימוש, בהתבסס על הערך שנשמר בשדה **msdyn\_ordertype** של הישות.

## <a name="add-custom-forms-and-turn-on-the-form-switching-logic"></a>הוספת טפסים מותאמים אישית והפעלת לוגיקת החלפת הטופס

הדוגמה הבאה מציגה כיצד להוסיף טופס מותאם אישית, **פרטי הפרוייקט שלי**, כך שיפעל עם הזדמנויות מבוססות-עבודה. אותו תהליך משמש להוספת טפסים מותאמים אישית כך שיפעלו עם הצעות מחיר, הזמנות וחשבוניות.

בצע את השלבים הבאים כדי ליצור גירסה מותאמת אישית של הטופס **פרטי פרוייקט**.

1. בישות 'הזדמנות', פתח את הטופס **פרטי פרוייקט** ושמור עותק תחת השם **פרטי הפרוייקט שלי**.
2. פתח את הטופס החדש ולאחר מכן, במאפיינים, ודא שקבצי ה- Script של אתחול הטופס מהטופס **פרטי הפרוייקט** קיימים. 

    > [!IMPORTANT]
    > אל תסיר את קבצי ה- Script. אחרת, ייתכן שנתונים מסוימים יאותחלו באופן שגוי.

3. ודא שהשדה **סוג** (**msdyn\_ordertype**) קיים בטופס. 

    > [!IMPORTANT]
    > אל תסיר את השדה. אחרת, קבצי ה- Script של האתחול ייכשלו.

4. מצא את הערך **formId** של הטופס החדש. באפשרותך לבצע שלב זה בשתי דרכים:

    - יצא את הטופס **פרטי הפרוייקט שלי** כחלק מפתרון לא מנוהל ולאחר מכן חפש את הערך **formId** בקובץ customization.xml של הפתרון המיוצא.
    - פתח את הטופס **פרטי הפרוייקט שלי** בעורך הטפסים וחפש את המזהה הייחודי הכללי (GUID) לצד הפרמטר **fromId** בכתובת ה- URL, כפי שמוצג באיור הבא.

    ![הערך formId של הטופס החדש בכתובת ה- URL](media/how-to-add-custom-forms-in-v2.0.png)

5. צור מיפוי **msdyn\_ordertype** עבור הערך **formId** על-ידי עריכת משאב האינטרנט msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js. הסר את הקוד מהמשאב והחלף אותו בקוד הבא.

    ```javascript
    define(["require", "exports"], function (require, exports) {
        "use strict";
        var SalesDocumentCustomFormIds = (function () {
            function SalesDocumentCustomFormIds() {
            }
            SalesDocumentCustomFormIds.overwriteFormIds = function (mappedFormIds) {
                /*
                ---- Notes ----
                mappedFormIds[SalesEntity][OrderType] => The array of forms IDs that support particular entity and order type
                Add or overwrite customized formId for the particular entity and order type by calling:
                    mappedFormIds[<EntityType>][<msdyn_ordertype>].push("<formId>");
                Allowed msdyn_ordertype values for reference:
                    ServiceBased: 690970002 (Field Service version of the entity)
                    WorkBased: 192350001 (PSA version of the entity)
                    ItemBased: 192350000 (Regular out of the box entity)
                Uncomment and update one of the following lines to register custom PSA form for required entity:
                */      
                //mappedFormIds[1][192350001].push("<formId>"); //Quote
                //mappedFormIds[5][192350001].push("<formId>"); //Quote Line
                //mappedFormIds[2][192350001].push("<formId>"); //Sales Order
                //mappedFormIds[6][192350001].push("<formId>"); //Sales Order Line
                // In this example we have added new form for Opportunity
                mappedFormIds[0][192350001].push("192EE537-DCC4-45D3-B7AF-EA694B9113D2"); //Opportunity
                //mappedFormIds[4][192350001].push("<formId>"); //Opportunity Line
            };
            return SalesDocumentCustomFormIds;
        }());
        exports.default = SalesDocumentCustomFormIds;
    });
    ```

6. שמור ולאחר מכן פרסם את ההתאמות האישיות.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]