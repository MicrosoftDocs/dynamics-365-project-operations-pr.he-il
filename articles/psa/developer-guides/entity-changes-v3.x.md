---
title: שינויי ישות, פקד וממשק משתמש (Project Service Automation 3.x)
description: נושא זה מתאר שינויי פתרון עבור Microsoft Dynamics Project Service Automation 3.x.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 03/15/2019
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
ms.openlocfilehash: 48062eda1f524dd3ca0d5feccf11fd5577521275
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148734"
---
# <a name="entity-control-and-user-interface-changes-project-service-automation-3x"></a>שינויי ישות, פקד וממשק משתמש (Project Service Automation 3.x)

[!include [banner](../../includes/psa-now-project-operations.md)]


עם הפצת Microsoft Dynamics Project Service Automation (PSA) 3.x, שינויים רבים בוצעו בישויות, בפקדים, בתצוגות ובממשק המשתמש. נושא זה מספק מידע לגבי שינויים חשובים אלה.

## <a name="parent-child-relationships-for-sales-document-sales-document-line-sales-document-line-detail-entities"></a>קשרי אב-צאצא עבור ישויות מסמך מכירות, שורת מסמך של מכירות, פרט שורת מסמך של מכירות
בגירסאות של Dynamics 365 Project Service Automation (PSA) שקדמו לגירסה 3.0, חלק מקשרי הגומלין בין ישויות מסמכי המכירות, שורות מסמכי המכירות ופרט שורת מסמך של מכירות יושמו באמצעות שדות מחרוזת ששמרו ייצוג מחרוזת של GUID של הישות הקשורה. זה נבע ממגבלות פלטפורמה שדרשו קוד מותאם אישית משמעותי בצד השרת ובצד הלקוח של הפתרון, כדי לגרום לקשרי גומלין אלה לפעול בדומה לקשרי גומלין של ישות Dynamics CRM טיפוסית וכדי לגרום לשדות מחרוזת לפעול כמו שדות בדיקת מידע.

PSA 3.0 עודכן כדי למנף את קשרי הגומלין החדשים של הישות בין ישות מסמך מכירות לישות שורת מסמך מכירות.

מכיוון שניתן להשתמש כעת בשדות בדיקת מידע כדי לציין הפניות לישויות, השדות ששמרו את ערך המחרוזת של ה- GUID של הישות הקשורה בגירסאות קודמות אינם דרושים עוד ולכן הוצאו משימוש. גם הקוד המותאם אישית של צד הלקוח וצד השרת אשר מטפל בקשרי הגומלין שהוגדרו על-ידי שדות מחרוזת מדור קודם הוצא משימוש.

### <a name="entity-schema-changes"></a>שינויי סכימת ישות
הטבלה הבאה מספקת רשימה של אחד לאחד של שדות המחרוזת שהוצאו משימוש ושל שדות בדיקת המידע החדשים עבור הישויות. 

 ישות |   שדה שהוצא משימוש (מחרוזת) | שדה חדש (בדיקת מידע)
--- | --- | ---
פרט חשבונית (שורה בחשבונית) |  msdyn_contractline |    msdyn_contractlineid
msdyn_actual (נתון בפועל) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_contractlineinvoiceschedule (לוח זמנים של חשבונית של סעיף חוזה עבור פרוייקט) |    msdyn_contractline |    msdyn_contractlineid
msdyn_contractlinescheduleofvalue (אבן דרך של סעיף חוזה בפרוייקט) |   msdyn_contractline |    msdyn_contractlineid
msdyn_fact (עובדה) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_invoicelinetransaction (פרט שורה בחשבונית) | msdyn_invoiceline <br> msdyn_salescontractline | msdyn_invoicelineid <br> msdyn_salescontractlineid
msdyn_journalline (שורת יומן) |  msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_orderlineresourcecategory (קטגוריית משאב של סעיף חוזה בפרוייקט) | msdyn_salescontractline |   msdyn_contractlineid
msdyn_orderlinetransaction (פרט סעיף חוזה בפרוייקט) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_orderlinetransactioncategory (קטגוריית עסקה של סעיף חוזה בפרוייקט) |   msdyn_contractline |    msdyn_contractlineid
msdyn_orderlinetransactionclassification (סיווג עסקת סעיף חוזה בפרוייקט) |   msdyn_contractline |    msdyn_contractlineid
msdyn_quotelineinvoiceschedule (לוח זמנים של חשבונית בשורת הצעת מחיר) |  msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelineresourcecategory (קטגוריית משאב של שורת הצעת מחיר) |    msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinescheduleofvalue (אבן דרך של שורת הצעת מחיר) | msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransaction (פרט של שורת הצעת מחיר) |    msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransactioncategory (קטגוריית עסקה בשורת הצעת מחיר) |  msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransactionclassification (סיווג עסקה בשורת הצעת מחיר) |  msdyn_quoteline |   msdyn_quotelineid
SalesOrderDetail (שורת הזמנה) | msdyn_quotelineid | msdyn_quoteline 

### <a name="deprecated-custom-views-and-controls"></a>תצוגות ופקדים מותאמים אישית שהוצאו משימוש
התצוגות והפקדים המותאמים אישית הבאים, והפריטים החזותיים הקשורים אליהם, הוצאו משימוש.

- תצוגת יכולת חיוב.
- פקדי רשת מותאמים אישית להצגת פרטים של שורת הצעת מחיר בדף **פרטי פרוייקט** עבור שורת הצעת המחיר.
- פקדי רשת מותאמים אישית להצגת פרטי סעיף חוזה בפרוייקט בדף **פרטי פרוייקט** עבור שורת הזמנת המכירות.

> [!NOTE]
> לקבלת הרשימה המלאה של משאבים שהוצאו משימוש, ראה [משאבי אינטרנט שהוצאו משימוש ב- Project Service Automation v3.x](../developer-guides/web-resources-deprecated-v3.x.md)

## <a name="unified-client-interface-app-module"></a>מודול יישום של ממשק לקוח מאוחד
עם הצהעה של מודולי יישום של ממשק לקוח מאוחד (UCI), ערכי מפת האתר של PSA הוסרו מהמערכת.  
פונקציונליות הקשורה להחלפת טופס עבור 'הזדמנות', 'הצעת מחיר', 'הזמנה', 'חשבונית' הוצאה משימוש משום שאינה דרושה עוד מאחר שמודול היישום של UCI כולל רק גירסאות PSA של הטפסים.  

משאבי האינטרנט הבאים הוצאו משימוש:

- msdyn_\SalesDocument\SalesDocumentFormLoader.js
- msdyn_\SalesDocument\PSSalesDocumentCustomFormIds.js

> [!NOTE]
> לקבלת הרשימה המלאה של משאבים שהוצאו משימוש, ראה [משאבי אינטרנט שהוצאו משימוש ב- Project Service Automation v3.x](../developer-guides/web-resources-deprecated-v3.x.md).




[!INCLUDE[footer-include](../../includes/footer-banner.md)]