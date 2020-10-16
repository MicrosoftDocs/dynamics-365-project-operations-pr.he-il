---
title: החל את הגדרת ההדגמה ואת נתוני התצורה
description: נושא זה מספק מידע על אופן החלת הגדרת ההדגמה ונתוני התצורה עבור Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 42e02f393e89d20b2a462645f519a3792bee8f2f
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948887"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations-lite-deployment---deal-to-proforma-invoicing"></a>החל את הגדרת ההדגמה ונתונה התצורה עבור פריסת לייט של Project Operations - מהעסקה ועד להוצאת חשבונית פרופורמה

_פריסת לייט - מהעסקה ועד להוצאת חשבונית פרופורמה_

1. הורד את [חבילת נתוני האב](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip). 
2. נווט לתיקיה *ProjOpsDemoDataSetupAndMaster - Integrated CMT* והפעל את קובץ ההפעלה, *DataMigrationUtility*.
3. בעמוד 1 של אשף הגדרת התצורה (CMT‏) של Common Data Service, בחר **ייבא נתונים** ואז בחר **המשך**.

![‏‫העברת תצורה](./media/1ConfigurationMigration.png)

4. בעמוד 2 של אשף ב-CMT בחר ב**Office 365** כ**סוג הפריסה**.
5. בחר את תיבות הסימון **הצג רשימה של ארגונים זמינים** ו**הצג מתקדם**.
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

- מטבע
- יחידה ארגונית
- איש קשר
- קבוצת מיסים
- קבוצת לקוחות
- יחידה
- קבוצת יחידות
- מחירון
- מחירון פרמטרים של פרוייקט
- תדירות חשבונית
- פרטי תדירות של הגשת חשבונית
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
