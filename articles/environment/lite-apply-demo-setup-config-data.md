---
title: החלת נתוני ההדגמה והתצורה - לייט
description: מאמר זה מספק מידע על אופן החלת נתוני הדגמה להגדרה לתצורה של Project Operations.
author: sigitac
ms.date: 01/27/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 9a3a99c326b7ebbdfa859c3298b35e910af0eb2a
ms.sourcegitcommit: 16c9eded66d60d4c654872ff5a0267cccae9ef0e
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/07/2022
ms.locfileid: "9409991"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a>החל את נתוני ההדגמה והתצורה עבור Project Operations - לייט 

_**פריסת לייט - מהעסקה ועד להוצאת חשבונית פרופורמה_



## <a name="prerequisites"></a>‏‫דרישות מוקדמות‬

לפני תחילת קביעת התצורה, נדרשת לך סביבת Dataverse שמוקצה ל- Dynamics 365 Project Operations.


## <a name="instructions"></a>הוראות

1. הורד את [חבילת נתוני האב](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData-%20CE%20only.zip). 
2. עבור לתיקיה *ProjOpsSampleSetupData - CE only CMT* והפעל את קובץ ההפעלה, *DataMigrationUtility*.
3. בעמוד 1 של אשף הגדרת התצורה (CMT‏) של Common Data Service, בחר **ייבא נתונים** ואז בחר **המשך**.

    ![‏‫העברת תצורה.](./media/1ConfigurationMigration.png)

4. בעמוד 2 של אשף CMT, בחר **Microsoft 365** כ **סוג הפריסה**.
5. בחר את תיבות הסימון **הצג רשימה של ארגונים זמינים** ו **הצג מתקדם**.
6. בחר את האזור של הדייר שלך, הזן את האישורים שלך ואז בחר **כניסה**.

   ![כניסת תצורה.](./media/2ConfigurationSignin.png)

7. בעמוד 3, מרשימת הארגונים בדייר, בחר לאיזה ארגון ברצונך לייבא את נתוני ההדגמה ואז בחר **כניסה**.
8. בעמוד 4, בחר את קובץ ה-zip, *SampleSetupAndConfigData* מהתיקייה שפתחת, *ProjOpsSampleSetupData - CE only CMT*.

   ![קובץ Zip.](./media/3ZipFile.png)

   ![בחר קובץ.](./media/4SelectAFile.png)

9. לאחר בחירת קובץ ה-zip בחר **ייבא נתונים**.

   ![ייבוא נתונים.](./media/5ImportData.png)

10. הייבוא יפעל בין שתיים לעשר דקות, תלוי במהירות הרשת שלך. לאחר השלמת הייבוא, צא מאשף ה-CMT. 
11. בדוק אם ישנם נתונים בארגון שלך ב-18 הישויות הבאות:

    -   מטבע
    -   חשבון
    -   יחידה ארגונית
    -   איש קשר
    -   יחידה
    -   קבוצת יחידות
    -   מחירון
    -   מחירון פרמטרים של פרוייקט 
    -   תדירות הגשת חשבונית
    -   קטגוריית משאבים הניתנים להזמנה
    -   קטגוריית עסקה
    -   קטגוריית הוצאות
    -   מחיר תפקיד
    -   מחיר קטגוריית עסקה
    -   מאפיין
    -   משאב הניתן להזמנה
    -   קטגוריות משאבים הניתנים להזמנה
    -   מאפיין של משאב הניתן להזמנה

    ![השלם את הייבוא.](./media/6CompleteImport.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
