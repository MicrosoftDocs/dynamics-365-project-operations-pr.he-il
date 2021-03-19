---
title: החלת נתוני ההדגמה והתצורה - לייט
description: נושא זה מספק מידע על אופן החלת הגדרת ההדגמה ונתוני התצורה עבור Project Operations.
author: sigitac
manager: Annbe
ms.date: 01/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 694dbc74591de74895095a9da6e590069711fc83
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290135"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a>החל את נתוני ההדגמה והתצורה עבור Project Operations - לייט 

_**פריסת לייט - מהעסקה ועד להוצאת חשבונית פרופורמה_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a>דרישות מוקדמות

לפני שתתחיל בקביעת התצורה, צריך להיות לך סביבת Common Data Service ‏(CDS) שמוקצה עבור Dynamics 365 Project Operations.


## <a name="instructions"></a>הוראות

1. הורד את [חבילת נתוני האב](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip). 
2. נווט לתיקיה *ProjOpsDemoDataSetupAndMaster - Integrated CMT* והפעל את קובץ ההפעלה, *DataMigrationUtility*.
3. בעמוד 1 של אשף הגדרת התצורה (CMT‏) של Common Data Service, בחר **ייבא נתונים** ואז בחר **המשך**.

    ![‏‫העברת תצורה](./media/1ConfigurationMigration.png)

4. בעמוד 2 של אשף ב-CMT בחר ב **Microsoft 365** כ **סוג הפריסה**.
5. בחר את תיבות הסימון **הצג רשימה של ארגונים זמינים** ו **הצג מתקדם**.
6. בחר את האזור של הדייר שלך, הזן את האישורים שלך ואז בחר **כניסה**.

   ![כניסת תצורה](./media/2ConfigurationSignin.png)

7. בעמוד 3, מרשימת הארגונים בדייר, בחר לאיזה ארגון ברצונך לייבא את נתוני ההדגמה ואז בחר **כניסה**.
8. בעמוד 4 בחר את קובץ ה-zip, *MasterAndSetupData* מהתיקייה שפורקה, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.

   ![קובץ Zip](./media/3ZipFile.png)

   ![בחר קובץ](./media/4SelectAFile.png)

9. לאחר בחירת קובץ ה-zip בחר **ייבא נתונים**.

   ![יבא נתונים](./media/5ImportData.png)

10. הייבוא יפעל בין שתיים לעשר דקות, תלוי במהירות הרשת שלך. לאחר השלמת הייבוא, צא מאשף ה-CMT. 
11. בדוק אם ישנם נתונים בארגון שלך ב-20 הישויות הבאות:

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

    ![השלם את הייבוא](./media/6CompleteImport.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]