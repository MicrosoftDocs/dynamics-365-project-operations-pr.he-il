---
title: הגדרה והחלה של נתוני  תצורה ב-Common Data Service
description: נושא זה מספק מידע על הגדרה והחלה של נתוני התצורה ב- Project Operations.
author: sigitac
ms.date: 05/10/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 2ea00df6112fb69b61f1889463424fdfee79aec9
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001292"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service"></a>הגדרה והחלה של נתוני  תצורה ב-Common Data Service 

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a>דרישות מוקדמות

לפני שתתחיל להגדיר נתונים ב- Common Data Service (CDS), יש לעמוד בתנאים המוקדמים הבאים:

1.  הקצאת סביבת CDS וסביבת Dynamics 365 Finance ל-Project Operations.
2.  מידע על הישות המשפטית מ-Dynamics 365 Finance משותף בסביבת CDS. פירוש הדבר שישות **חברה** ב- CDS כוללת את רשומות החברה הבאות:
  - THPM
  - USPM
  - GBPM

## <a name="install-setup-and-configuration-data"></a>הגדרת התקנה ונתוני תצורה

1. הורד, בטל חסימה ובטל דחיסה של [החבילה 'הגדרה ונתוני תצורה'](https://download.microsoft.com/download/e/2/d/e2da6c98-d5dd-450c-aabe-fd6bf2ba374b/ProjOpsSampleSetupData-%20Integrated%20Latest.zip).
2. נווט אל התיקיה שדחיסתה בוטלה והפעל את קובץ ההפעלה *DataMigrationUtility*.
3. בעמוד 1 של אשף הגדרת התצורה (CMT‏) של Common Data Service, בחר **ייבא נתונים** ואז בחר **המשך**.

![‏‫העברת תצורה](./media/1ConfigurationMigration.png)

4. בעמוד 2 של אשף ב-CMT בחר ב **Microsoft 365** כ **סוג הפריסה**.
5. בחר את תיבות הסימון **הצג רשימה של ארגונים זמינים** ו **הצג מתקדם**.
6. בחר את האזור של הדייר שלך, הזן את האישורים שלך ובחר **כניסה**.

![כניסת תצורה](./media/2ConfigurationSignin.png)

7. בעמוד 3, מרשימת הארגונים בדייר, בחר את הארגון שאליו אתה רוצה לייבא את נתוני ההדגמה ובחר **כניסה**.
8. בעמוד 4, בחר את קובץ ה- zip *SampleSetupAndConfigData* מהתיקיה שפורקה.

![בחירת קובץ Zip](./media/3ZipFile.png)

![בחר קובץ](./media/4SelectAFile.png)

9. לאחר בחירת קובץ ה-zip בחר **ייבא נתונים**.

![יבא נתונים](./media/5ImportData.png)

10. הייבוא יפעל בין שתיים לעשר דקות, תלוי במהירות הרשת שלך. לאחר השלמת הייבוא, צא מאשף ה- CMT. 
11. בדוק אם ישנם נתונים בארגון שלך ב-26 הישויות הבאות:

  - מטבע
  - תרשים של תיקי לקוחות
  - לוח שנה כספי
  - סוגי שער חליפין
  - יום התשלום
  - לוח זמנים לתשלום
  - תנאי תשלום
  - יחידה ארגונית
  - איש קשר
  - קבוצת מיסים
  - קבוצת לקוחות
  - קבוצת ספקים
  - יחידה
  - קבוצת יחידות
  - מחירון
  - מחירון פרמטרים של פרוייקט
  - תדירות חשבונית
  - קטגוריית משאבים הניתנים להזמנה
  - קטגוריית עסקה
  - קטגוריית הוצאות
  - מחיר תפקיד
  - מחיר קטגוריית עסקה
  - מאפיין
  - משאב הניתן להזמנה
  - קטגוריות משאבים הניתנים להזמנה
  - מאפיין של משאב הניתן להזמנה

![השלם את הייבוא](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a>עדכן את התצורות של Project Operations

1. נווט אל סביבת CE. אתה יכול למצוא אותה על-ידי פתיחת [מרכז הניהול של Power Platform](https://admin.powerplatform.microsoft.com/environments), בחירת הסביבה ואז בחירת האפשרות **פתח סביבה**. 

![פתח את הסביבה](./media/7OpenEnvironment.png)

2. כדי ליצור משאב הניתן להזמנה למשתמש שלך, עבור אל **פרויקטים** > **משאבים** ולאחר מכן בחר **חדש**.

![משאבים הניתנים להזמנה](./media/8BookableResources.png)

3. בכרטיסיה **כללי**, בחר את המשתמש שהוא מנהל המערכת שלך. ודא שאזור הזמן תואם את זה שאתה נמצא בו. 

![משאב חדש הניתן להזמנה](./media/9NewBookableResource.png)

4. בכרטיסיה **תזמון**, בשדה **חברה**, בחר את החברה **USPM** ולאחר מכן בחר **שמור**. 

![כרטיסיית תזמון](./media/10SchedulingTab.png)

5. בחר בכרטיסיה **שעות עבודה**.  

![שעות עבודה](./media/11WorkHours.png)

6. לחץ פעמיים על ערך כלשהו בלוח השנה ובחר **ערוך** > **כל האירועים בסדרה**. 

![לוח שנה של עבודה](./media/12WorkCalendar.png)

7. שנה את שעות העבודה לשמונה (8) שעות עבודה ביום, סמן סופי שבוע כימים שאינם ימי עבודה וכן וודא שאזור הזמן תואם לשלך. 
8. בחר **שמור וסגור**.

![עדכן לוח שנה](./media/13UpdateCalendar.png)

9. עבור אל **הגדרות** > **תבניות לוח שנה** ובחר **חדש**.
 
 ![תבניות לוח שנה](./media/14CalendarTemplates.png)
 
 10. הזן שם, בחר את משאב התבנית שיצרת ולאחר מכן בחר **שמור**. 
 
 ![שמור תבנית לוח שנה](./media/15SaveCalendarTemplate.png)
 
 11. עבור אל **פרמטרים** ולחץ פעמיים על הרשומה. 
 
 ![פרמטרי פרויקט](./media/16ProjectParameters.png)
 
12. עדכן את השדות הבאים:

 - **חברת ברירת מחדל**: USPM
 - **יחידה ארגונית המוגדרת כברירת מחדל**: Contoso רובוטיקה גלובלית
 - **תדירות חשבונית**: היום השביעי והאחרון
 - **תבנית שעות עבודה**: שנה לתבנית שיצרת.

13. בחר **שמור**. 

![עדכן פרמטרי פרויקט](./media/17UpdatedProjectParameters.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
