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
ms.openlocfilehash: 31986efed81892cc5722cb8f5e292cde14d8843d
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5144594"
---
# <a name="add-new-custom-entity-forms-project-service-automation-2x"></a><span data-ttu-id="80990-103">הוספת טפסי ישות מותאמים אישית חדשים (Project Service Automation 2.x)</span><span class="sxs-lookup"><span data-stu-id="80990-103">Add new custom entity forms (Project Service Automation 2.x)</span></span>

[!include [banner](../../includes/psa-now-project-operations.md)]

## <a name="type-field"></a><span data-ttu-id="80990-104">שדה 'סוג'</span><span class="sxs-lookup"><span data-stu-id="80990-104">Type field</span></span> 

<span data-ttu-id="80990-105">Dynamics 365 Project Service Automation מתבסס על השדה **סוג** (**msdyn\_ordertype**) של הישויות 'הזדמנות', 'הצעת מחיר', 'הזמנה' ו'חשבונית' כדי להבחין בין גירסאות **מבוססות-עבודה** של ישויות אלה לבין גירסאות **מבוססות-פריט** ו **מבוססות-שירות**.</span><span class="sxs-lookup"><span data-stu-id="80990-105">Dynamics 365 Project Service Automation relies on the **Type** (**msdyn\_ordertype**) field of the Opportunity, Quote, Order, and Invoice entities to distinguish **work-based** versions of these entities from **item-based** and **service-based** versions.</span></span> <span data-ttu-id="80990-106">גירסאות מבוססות-עבודה של ישויות אלה מטופלות על-ידי PSA.</span><span class="sxs-lookup"><span data-stu-id="80990-106">Work-based versions of these entities are handled by PSA.</span></span> <span data-ttu-id="80990-107">לוגיקה עסקית רבה בצד הלקוח ובצד השרת של הפתרון תלויה בשדה **סוג**.</span><span class="sxs-lookup"><span data-stu-id="80990-107">Lots of business logic on the client side and server side of the solution depends on the **Type** field.</span></span> <span data-ttu-id="80990-108">לכן, חשוב שהשדה יאותחל עם ערך נכון בעת יצירת הישויות.</span><span class="sxs-lookup"><span data-stu-id="80990-108">Therefore, it's important that the field be initialized with a correct value when the entities are created.</span></span> <span data-ttu-id="80990-109">ערך שגוי עלול לגרום לאופן פעולה שגוי, וייתכן שלוגיקה עסקית מסוימת לא תפעל כהלכה.</span><span class="sxs-lookup"><span data-stu-id="80990-109">An incorrect value can cause incorrect behaviors, and some business logic might not run correctly.</span></span>

## <a name="automatic-form-switching"></a><span data-ttu-id="80990-110">החלפת טופס אוטומטית</span><span class="sxs-lookup"><span data-stu-id="80990-110">Automatic form switching</span></span>

<span data-ttu-id="80990-111">כדי למנוע השחתת נתונים אפשרית ואופן פעולה לא צפוי שנגרמים על-ידי אתחול ועריכה שגויים של רשומות ישות המכירות, PSA כולל כעת לוגיקה עבור החלפת טפסים אוטומטית בטפסים מוכנים לשימוש.</span><span class="sxs-lookup"><span data-stu-id="80990-111">To avoid potential data corruption and unexpected behaviors that are caused by incorrect initialization and editing of the sales entity records, PSA now includes logic for automatic form switching in out-of-box forms.</span></span> <span data-ttu-id="80990-112">לוגיקה זו מעבירה משתמשים אל הטופס הנכון לעבודה עם הגירסה מבוססת העבודה או כל סוג אחר של ישות 'הזדמנות', 'הצעת מחיר', 'הזמנה' או 'חשבונית'.</span><span class="sxs-lookup"><span data-stu-id="80990-112">This logic takes users to the correct form for working with the work-based version or any other type of Opportunity, Quote, Order, or Invoice entity.</span></span> <span data-ttu-id="80990-113">כאשר משתמש פותח גירסה מבוססת-עבודה של הישות 'הזדמנות', 'הצעת מחיר', 'הזמנה' או 'חשבונית', הטופס עובר אל **פרטי פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="80990-113">When a user opens the work-based version of an Opportunity, Quote, Order, or Invoice entity, the form is switched to **Project Information**.</span></span>

<span data-ttu-id="80990-114">הלוגיקה של החלפת הטופס האוטומטית מסתמכת על המיפוי בין הערך **formId** לשדה **msdyn\_ordertype**.</span><span class="sxs-lookup"><span data-stu-id="80990-114">The automatic form switching logic relies on the mapping between the **formId** value and the **msdyn\_ordertype** field.</span></span> <span data-ttu-id="80990-115">כל הטפסים המוכנים לשימוש נוספו למיפוי זה.</span><span class="sxs-lookup"><span data-stu-id="80990-115">All out-of-box forms have been added to that mapping.</span></span> <span data-ttu-id="80990-116">עם זאת, יש להוסיף באופן ידני טפסים מותאמים אישית כדי לציין באיזו גירסה של הישות הם נועדו לטפל.</span><span class="sxs-lookup"><span data-stu-id="80990-116">However, custom forms must be manually added to indicate which version of the entity they are intended to handle.</span></span> <span data-ttu-id="80990-117">זה מבוסס על השדה **msdyn\_ordertype**.</span><span class="sxs-lookup"><span data-stu-id="80990-117">This is based on the **msdyn\_ordertype** field.</span></span> <span data-ttu-id="80990-118">אם החלפת הטופס חסרה במיפוי, הלוגיקה תעבור לטופס המוכן לשימוש, בהתבסס על הערך שנשמר בשדה **msdyn\_ordertype** של הישות.</span><span class="sxs-lookup"><span data-stu-id="80990-118">If the form switching is missing from the mapping, logic will switch to the out-of-box form, based on the value that is saved in the **msdyn\_ordertype** field of the entity.</span></span>

## <a name="add-custom-forms-and-turn-on-the-form-switching-logic"></a><span data-ttu-id="80990-119">הוספת טפסים מותאמים אישית והפעלת לוגיקת החלפת הטופס</span><span class="sxs-lookup"><span data-stu-id="80990-119">Add custom forms and turn on the form switching logic</span></span>

<span data-ttu-id="80990-120">הדוגמה הבאה מציגה כיצד להוסיף טופס מותאם אישית, **פרטי הפרוייקט שלי**, כך שיפעל עם הזדמנויות מבוססות-עבודה.</span><span class="sxs-lookup"><span data-stu-id="80990-120">The following example shows how to add a custom form, **My Project Information**, so that it works with work-based opportunities.</span></span> <span data-ttu-id="80990-121">אותו תהליך משמש להוספת טפסים מותאמים אישית כך שיפעלו עם הצעות מחיר, הזמנות וחשבוניות.</span><span class="sxs-lookup"><span data-stu-id="80990-121">The same process is used to add custom forms so that they work with quotes, orders, and invoices.</span></span>

<span data-ttu-id="80990-122">בצע את השלבים הבאים כדי ליצור גירסה מותאמת אישית של הטופס **פרטי פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="80990-122">Follow these steps to create a custom version of the **Project Information** form.</span></span>

1. <span data-ttu-id="80990-123">בישות 'הזדמנות', פתח את הטופס **פרטי פרוייקט** ושמור עותק תחת השם **פרטי הפרוייקט שלי**.</span><span class="sxs-lookup"><span data-stu-id="80990-123">In the Opportunity entity, open the **Project Information** form, and save a copy under the name **My Project Information**.</span></span>
2. <span data-ttu-id="80990-124">פתח את הטופס החדש ולאחר מכן, במאפיינים, ודא שקבצי ה- Script של אתחול הטופס מהטופס **פרטי הפרוייקט** קיימים.</span><span class="sxs-lookup"><span data-stu-id="80990-124">Open the new form, and then, in the properties, make sure that the form initialization scripts from the **Project Information** form are present.</span></span> 

    > [!IMPORTANT]
    > <span data-ttu-id="80990-125">אל תסיר את קבצי ה- Script.</span><span class="sxs-lookup"><span data-stu-id="80990-125">Don't remove the scripts.</span></span> <span data-ttu-id="80990-126">אחרת, ייתכן שנתונים מסוימים יאותחלו באופן שגוי.</span><span class="sxs-lookup"><span data-stu-id="80990-126">Otherwise, some data might be initialized incorrectly.</span></span>

3. <span data-ttu-id="80990-127">ודא שהשדה **סוג** (**msdyn\_ordertype**) קיים בטופס.</span><span class="sxs-lookup"><span data-stu-id="80990-127">Verify that the **Type** (**msdyn\_ordertype**) field is present in the form.</span></span> 

    > [!IMPORTANT]
    > <span data-ttu-id="80990-128">אל תסיר את השדה.</span><span class="sxs-lookup"><span data-stu-id="80990-128">Don't remove this field.</span></span> <span data-ttu-id="80990-129">אחרת, קבצי ה- Script של האתחול ייכשלו.</span><span class="sxs-lookup"><span data-stu-id="80990-129">Otherwise, the initialization scripts will fail.</span></span>

4. <span data-ttu-id="80990-130">מצא את הערך **formId** של הטופס החדש.</span><span class="sxs-lookup"><span data-stu-id="80990-130">Find the **formId** value of the new form.</span></span> <span data-ttu-id="80990-131">באפשרותך לבצע שלב זה בשתי דרכים:</span><span class="sxs-lookup"><span data-stu-id="80990-131">You can complete this step in two ways:</span></span>

    - <span data-ttu-id="80990-132">יצא את הטופס **פרטי הפרוייקט שלי** כחלק מפתרון לא מנוהל ולאחר מכן חפש את הערך **formId** בקובץ customization.xml של הפתרון המיוצא.</span><span class="sxs-lookup"><span data-stu-id="80990-132">Export the **My Project Information** form as part of an unmanaged solution, and then look up the **formId** value in the customization.xml file of the exported solution.</span></span>
    - <span data-ttu-id="80990-133">פתח את הטופס **פרטי הפרוייקט שלי** בעורך הטפסים וחפש את המזהה הייחודי הכללי (GUID) לצד הפרמטר **fromId** בכתובת ה- URL, כפי שמוצג באיור הבא.</span><span class="sxs-lookup"><span data-stu-id="80990-133">Open the **My Project Information** form in the form editor, and then look for the globally unique identifier (GUID) next to the **fromId** parameter in the URL, as shown in the following illustration.</span></span>

    ![הערך formId של הטופס החדש בכתובת ה- URL](media/how-to-add-custom-forms-in-v2.0.png)

5. <span data-ttu-id="80990-135">צור מיפוי **msdyn\_ordertype** עבור הערך **formId** על-ידי עריכת משאב האינטרנט msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js.</span><span class="sxs-lookup"><span data-stu-id="80990-135">Create an **msdyn\_ordertype** mapping for the **formId** value by editing the msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js web resource.</span></span> <span data-ttu-id="80990-136">הסר את הקוד מהמשאב והחלף אותו בקוד הבא.</span><span class="sxs-lookup"><span data-stu-id="80990-136">Remove the code from the resource, and replace it with the following code.</span></span>

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

6. <span data-ttu-id="80990-137">שמור ולאחר מכן פרסם את ההתאמות האישיות.</span><span class="sxs-lookup"><span data-stu-id="80990-137">Save and then publish the customizations.</span></span>
