---
title: שילוב Microsoft Project Client
description: תכנון לוח הזמנים של פרוייקט ואחזקתו יכולים להיות מורכבים, כך שמנהלי הפרויקטים צריכים להשתמש בכלים שעוזרים להם לנהל משימה זו. שילוב עם Microsoft Project Client מספק תמיכה לפתיחת מבנה התפלגות עבודה וניהולו.
author: KimANelson
manager: AnnBe
ms.date: 12/11/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjWbsTemplate
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: c6478e05-50ee-4993-87f4-6ce9cb78f076
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2017-12-04
ms.dyn365.ops.version: 7.2999999999999998
ms.openlocfilehash: e35e1e54bad659d1329c333479830b680a17cbb0
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751866"
---
# <a name="microsoft-project-client-integration"></a>שילוב Microsoft Project Client

[!include [banner](../includes/banner.md)]

תכנון לוח הזמנים של פרוייקט ואחזקתו יכולים להיות מורכבים, כך שמנהלי הפרויקטים צריכים להשתמש בכלים שעוזרים להם לנהל משימה זו. שילוב עם Microsoft Project Client מספק תמיכה לפתיחת מבנה התפלגות עבודה וניהולו. מנהל הפרויקט יכול לפרסם כל שינוי בחזרה אל מבנה התפלגות עבודת הפרוייקט ב- Dynamics 365 Finance.

> [!NOTE]
> אם אתה משתמש בעדכון יולי (גירסה 10.0.4), עליך להתקין את KB 4054797 ואת 4055884.

## <a name="configure-the-microsoft-project-client-add-in"></a>הגדרת התוספת Microsoft Project Client
כדי להפעיל את השילוב עם Microsoft Project Client, נדרשת התקנת תוספת Microsoft Dynamics 365 ביישום Microsoft Project בלקוח של המשתמש. זה נעשה על-ידי פתיחת **סביבת העבודה לניהול פרוייקטים**.

•   לחץ על **הגדר תצורת תוספת בלקוח פרוייקט** מהמקטע **קישורים** > **הגדרה** בסביבת העבודה.

•   לחץ **פתח**, וכשתתבקש, לחץ על **הפעל**.

## <a name="open-and-edit-an-existing-draft-work-breakdown-structure-in-microsoft-project-client"></a>פתיחת טיוטה קיימת של מבנה התפלגות עבודה ב- Microsoft Project Client ועריכתה
אם לפרוייקט ב- Dynamics 365 Finance כבר נוצר מבנה התפלגות עבודה, ניתן לפתוח את מבנה התפלגות העבודה ביישום Microsoft Project Client אם מבנה התפלגות העבודה נמצא במצב טיוטה. כדי לפתוח את הדף **פרוייקט**, לחץ על הקישור **פתח ב- Microsoft Project** מהכרטיסיה **תכנון**. בנוסף, ניתן לפתוח דך זה מתוך יישום Microsoft Project Client על-ידי לחיצה על **פתח** בכרטיסיה **Microsoft Dynamics 365**. בחר **ישות משפטית** ו**פרוייקט** מהרשימה.

> [!NOTE]
> אם אתה משתמש ב- Internet Explorer כדפדפן שלך, עליך ללחוץ על **שמור** כדי לפתוח ידנית מהמיקום שאליו הקובץ הורד. לחלופין, לחץ על **שמור ופתח** כדי לפתוח את הקובץ ב- Microsoft Project Client. אל תשנה את השם של הקובץ בעת השמירה.

לפני ביצוע פעולות עריכה בקובץ בעת שימוש ב- Microsoft Project Client, עליך להוציא אותו. לחץ על **הוצא קובץ** בכרטיסיה **Microsoft Dynamics 365**. פעולה זו תמנע ממשתמשים אחרים לערוך את מבנה התפלגות העבודה מתוך Finance במקביל. כדי לפרסם את מבנה התפלגות העבודה לאחר השלמת העריכה, לחץ על **הכנס קובץ** בכרטיסיה **Microsoft Dynamics 365**.

אם צוות פרוייקט כבר נוסף לפרוייקט ב- Finance, רשימת המשאבים תאוכלס עם חברי הצוות. אם טרם התווסף צוות פרוייקט לפרוייקט, באפשרותך לבחור משאבים ולבנות את הצוות בתוך Microsoft Project Client על ידי לחיצה על לחצן **משאבים‏‎** בכרטיסיה **Microsoft Dynamics 365**. 

הנתונים הבאים יסונכרנו בחזרה ל- Finance כחלק מתהליך הכנסת הקובץ:

•   שם משימה

•   תאריך התחלה

•   תאריך סיום

•   ‏‏פעילויות קדם

•   שמות משאבים

•   קטגוריה

•   קטגוריית משאבים

•   שעות עבודה

•   הערות

•   עדיפות

> [!NOTE]
> אם תוסיף עמודות אחרות לקובץ Microsoft Project Client שלך, הן לא יישמרו בקובץ ולא יוצגו עם פתיחת הקובץ שוב.

## <a name="create-the-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a>יצירת מבנה התפלגות העבודה עבור פרוייקט קיים באמצעות Microsoft Project Client
כדי ליצור מבנה התפלגות עבודה חדש באמצעות Microsoft Project Client, בצע את השלבים הבאים:


1.  פתח את Microsoft Project Client.

2.  בכרטיסיה **Microsoft Dynamics 365**, לחץ על **פתח**.

3.  בחר את **הישות המשפטית** עבור הפרוייקט.

4.  בחר את ה**פרוייקט**.

5.  לחץ על **הוצא קובץ** בכרטיסיה **Microsoft Dynamics 365**.

6.  כשתהיה מוכן לפרסם ב- Finance, לחץ על **הכנס קובץ** בכרטיסיה **Microsoft Dynamics 365**.

## <a name="replace-the-existing-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a>החלפת את מבנה התפלגות העבודה הקיים עבור פרוייקט קיים באמצעות Microsoft Project Client
כדי ליצור מבנה התפלגות עבודה חדש באמצעות Microsoft Project Client ולהחליף מבנה התפלגות עבודה קיים לפרוייקט קיים, בצע את השלבים הבאים:

1.  פתח את Microsoft Project Client.

2.  צור את לוח הזמנים ב- Microsoft Project Client.

3.  בכרטיסיה **Microsoft Dynamics 365**, לחץ על **שמור שינויים** > **החלף פרוייקט קיים**.

4.  בחר את **הישות המשפטית** עבור הפרוייקט.

5.  בחר את ה**פרוייקט**.

6.  לחץ על **אישור**.

## <a name="create-a-new-project-from-within-microsoft-project-client"></a>יצירת פרוייקט חדש מתוך Microsoft Project Client


1.  פתח את Microsoft Project Client.

2.  צור את לוח הזמנים ב- Microsoft Project Client.

3.  בכרטיסיה **Microsoft Dynamics 365**, לחץ על **שמור שינויים** > **שמור לפרוייקט חדש**.

4.  בחר את **הישות המשפטית** עבור הפרוייקט.

5.  בעת הצורך, הזן את **מזהה הפרוייקט**.

6.  הזן את **שם הפרוייקט**.

7.  בחר את **סוג הפרוייקט**, **קבוצת הפרוייקטים** ואת **מזהה חוזה הפרוייקט**. לחלופין, תוכל ליצור חוזה פרוייקט חדש על ידי לחיצה על **חדש**.

8.  בחר את **לוח השנה** שבו יש להשתמש להקצאת משאבים.

11. לחץ על **אישור**.
