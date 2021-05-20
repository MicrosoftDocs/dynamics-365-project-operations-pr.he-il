---
title: שילוב נתוני התקנה ותצורה של Project Operations
description: נושא זה מספק מידע על הגדרה וקביעת התצורה של מפות כתיבה כפולה של Project Operations.
author: sigitac
manager: Annbe
ms.date: 4/23/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d5fe81dca30039f99d5d7b9bb459214e540db945
ms.sourcegitcommit: bc51629df94c164325cf2afee387d0e7cda66da7
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2021
ms.locfileid: "5938991"
---
# <a name="project-operations-setup-and-configuration-data-integration"></a>שילוב נתוני התקנה ותצורה של Project Operations

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

נושא זה מספק מידע על שילוב כתיבה כפולה של Project Operations לישויות הגדרה ותצורה.

## <a name="project-contracts-contract-lines-and-projects"></a>חוזי פרוייקט, סעיפי חוזה ופרוייקטים

חוזי פרויקטים, סעיפי חוזה ופרויקטים נוצרים ב- Dataverse ומסונכרנים עם יישומי Finance and Operations לביצוע חשבונאות נוספות. ניתן ליצור ולמחוק את הרשומות בישויות אלה רק ב- Dataverse. עם זאת, ניתן להוסיף לרשומות אלה תכונות חשבונאות כגון ברירות מחדל של קבוצת מע"מ ומדדים פיננסים ביישומי Finance and Operations.

  ![מושגי שילוב של חוזה של פרוייקט](./media/1ProjectContract.jpg)

מעקב אחר לידים, הזדמנויות והצעות מחיר של מכירות מתבצע ב- Dataverse ואין סנכרון עם ישומי Finance and Operations מכיוון שאין פעילות חשבונאית במורד הזרם המשוייכת לפעילות זו.

הפונקציונליות של חוזה הפרויקט ב- Dataverse יוצרת רשומת חוזה פרויקט בישומי Finance and Operations באמצעות מפת הטבלה **כותרות חוזי פרויקטים (salesorders)**. שמירת חוזה פרויקט ב- Dataverse מניע גם יצירת רשומת ישות לקוח של של חוזה פרויקט. רשומה זו מסונכרנת עם ישומי Finance and Operations באמצעות מפת הטבלה **מקור מימון הפרויקט (msdyn\_projectcontractssplitbillingrules)**. מפה זו מסנכרנת גם תוספות, עדכונים ומחיקות של לקוח חוזה הפרויקט. אחוזי חיוב מפוצלים בין לקוחות חוזה הפרויקט נשלטים רק ב- Dataverse ולא מסונכרנים עם יישומי Finance and Operations.

לאחר יצירת חוזה פרויקט ב- Dataverse, רואה חשבון הפרויקט יכול לעדכן את תכונות החשבונאות של חוזה פרויקט זה בישומי Finance and Operations על ידי מעבר אל **ניהול פרויקטים וחשבונאות** > **חוזי פרויקט** > **הגדרה** > **הצג חשבונאות ברירת מחדל**. רואה החשבון יכול לסקור את התכונות התפעוליות של חוזה הפרויקט, כגון תאריך מסירה מבוקש וסכום החוזה על ידי בחירת מזהה חוזה הפרויקט ביישומי Finance and Operations הפותחים את רשומת חוזה הפרויקט הקשור ב - Dataverse.

ישות הפרויקט מסונכרנת עם יישומי Finance and Operations באמצעות מפת הטבלה **פרויקטים גרסה 2 (msdyn\_projects)**. רואה חשבון הפרויקט יכול:

  - לסקור פרויקטים בישומי Finance and Operations על ידי מעבר אל **ניהול פרויקטים וחשבונאות** > **כל הפרויקטים**. 
  - לעדכן תכונות חשבונאיות עבור הפרויקט בישומי Finance and Operations על ידי מעבר אל **ניהול פרויקטים וחשבונאות** > **כל הפרויקטים** > **הגדרה** > **הצג חשבונאות ברירת מחדל**.  
  - לבדוק את התכונות התפעוליות של הפרויקט, כגון תאריכי התחלה וסיום משוערים, על ידי בחירה במזהה הפרויקט בישומי Finance and Operations, פעולה שפותחת את רשומת הפרויקט הקשור ב- Dataverse.

פרויקט משויך לחוזה פרויקט באמצעות הישות **שורת חוזה פרויקט**.

סעיפי חוזה הפרויקט ב- Dataverse יוצרות כלל חיוב חוזה פרויקט בישומי Finance and Operations באמצעות מפת הטבלה **שורות חוזי פרויקטים (salesorderdetails)**. שיטת החיוב מגדירה את סוג כלל החיוב בחוזה הפרויקט בישומי Finance and Operations:

  - סעיפי חוזה פרויקט בשיטת חיוב של זמן וחומר יוצרים כלל חיוב של זמן וסוג חומר.
  - סעיפי חוזה בשיטת חיוב של מחיר קבוע יוצרים כלל אבן דרך לחיוב.

רואה חשבון הפרויקט יכול לסקור את סעיפי הפרויקט ביישומי Finance and Operations על ידי מעבר אל **ניהול פרויקטים וחשבונאות** > **חוזי פרויקט** > **הגדרה** > **הצג חשבונאות ברירת מחדל** וסקירת הפרטים בכרטיסיה **סעיפי חוזה**. רואה החשבון יכול גם להגדיר מימדים פיננסיים כברירת מחדל עבור סעיפי החוזה בשיטת החיוב מחיר קבוע בכרטיסייה זו.

## <a name="billing-milestones"></a>אבני דרך לחיוב

סעיפי חוזה פרויקט שמשתמשים בשיטת החיוב במחיר קבוע מחושבים באמצעות אבני דרך לחיוב. אבני דרך לחיוב מסונכרנות עם עסקאות לחשבון של פרויקטים בישומי Finance and Operations באמצעות מפת הטבלה **אבני דרך בשילוב סעיפי חוזה לשילוב של Project Operations (‏msdyn\_contractlinescheduleofvalues)**.

  ![אבני דרך לחיוב](./media/2Milestones.jpg)

רואה החשבון יכול לבדוק עסקאות לחשבון ולהתאים את תכונות החשבונאות עבור עסקאות אלה על ידי מעבר אל **ניהול פרויקטים וחשבונאות** > **חוזי פרויקט** > **שמירה** > **עסקאות לחשבון** או **ניהול פרויקטים וחשבונאות** > **כל הפרויקטים** > **שמירה** > **עסקאות לחשבון**.

כשיוצרים אבן דרך לחיוב עבור סעיף חוזה פרויקט מסוים, המערכת יוצרת באופן אוטומטי פרויקט הערכת הכנסה במחיר קבוע עבור הפרויקט המשויך לסעיף חוזה זה. ניתן לסקור פרויקטים של הערכת הכנסות במחיר קבוע על ידי מעבר אל **ניהול פרויקטים וחשבונאות** > **פרויקטים של הערכת הכנסות במחיר קבוע**.

### <a name="project-tasks"></a>משימות פרויקט

משימות הפרויקט מסונכרנות עם ישומי Finance and Operations דרך מפת הטבלה **משימות פרויקט (msdyn\_projecttasks)** למטרות הפניה בלבד. פעולות יצירה, עדכון ומחיקה אינן נתמכות דרך יישומי Finance and Operations.

  ![שילוב משימות פרויקט](./media/3Tasks.jpg)

## <a name="project-resources"></a>משאבי פרוייקט

הישות **תפקידי משאבים בפרויקט** מסונכרנת עם ישומי Finance and Operations באמצעות מפת הטבלה **תפקידי משאבי פרוייקט לכל החברות (bookableresourcecategories)** למטרות הפניה בלבד. מכיוון שתפקידי משאבים ב- Dataverse אינם ספציפיים לחברה, המערכת יוצרת באופן אוטומטי רשומות תפקידי משאבים ספציפיים לחברה בהתאמה בישומי Finance and Operations עבור כל הישויות המשפטיות הנכללות בטווח שילוב של כתיבה כפולה.

![שילוב תפקידי משאבים](./media/5Resources.jpg)

משאבי הפרויקט ב- Project Operations נשמרים ב- Dataverse ואינם מסונכרנים עם ישומי Finance and Operations.

### <a name="transaction-categories"></a>קטגוריות עסקה

קטגוריות של העסקאות נשמרות ב- Dataverse ומסונכרנות עם ישומי Finance and Operations באמצעות מפת הטבלה **קטגוריות של עסקאות פרוייקט (msdyn\_transactioncategories)**. לאחר סינכרון רשומת קטגוריית העסקה, המערכת יוצרת באופן אוטומטי ארבע רשומות קטגוריה משותפות. כל רשומה תואמת לסוג עסקה בישומי Finance and Operations וקושר אותם לרשומת קטגוריית העסקה.

![שילוב קטגוריות של עסקאות](./media/4TransactionCategories.jpg)

שימוש בקטגוריות עסקאות לאומדנים ולמעשים מחייבים את רואה החשבון של הפרויקט או את המערכת מנהל מערכת ליצור קטגוריות פרויקט תואמות בכל ישות משפטית. לקבלת מידע נוסף, ראה [קביעת תצורה של קטגוריות של מוצרים](../project-accounting/configure-project-categories.md).