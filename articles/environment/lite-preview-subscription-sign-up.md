---
title: רישום למנוי Preview‏ - Lite
description: מאמר זה מספק מידע על אופן ההרשמה והפריסה של Project Operations lite - מהעסקה ועד הפקת חשבונית פרופורמה.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 6953956c0b3401a6c64ee597f966ba4a4c0d07b5
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8921257"
---
# <a name="sign-up-for-a-preview-subscription---lite"></a>רישום למנוי Preview‏ - Lite 

מאמר זה מסביר כיצד להירשם להצעת הניסיון ולפרוס את הפריסה של Dynamics 365 Project Operations lite - מהעסקה ועד הפקת חשבונית פרופורמה.

> [!NOTE]
> תהליך זה ישתנה במהדורות הקרובות של Project Operations.

## <a name="prerequisites"></a>דרישות מוקדמות
- המשתמש שמבצע את הפריסה של ה-Preview חייב להיות בעל זכויות מנהל מערכת כלליות של דייר Azure. ניתן ליצור דייר במהלך מימוש ההצעה הראשונה.

> [!IMPORTANT]
> רק אדם אחד בארגון, מנהל הדיירים, צריך לבצע את המשימה הזו. אם אינך המנוי למהדורה זו, המתן עד שהארגון שלך יירשם ותקבל את אישורי המשתמש שלך.
> 
> גירסאות ניסיון הן לשימוש חד פעמי בדייר. אפשר להריץ גירסת ניסיון רק פעם אחת. אנו ממליצים ליצור דייר חדש לצורך גירסת הניסיון.

### <a name="dynamics-365-project-operations-trial"></a>גירסת ניסיון של Dynamics 365 Project Operations 

לפני שתתחיל, ודא שאתה מחובר לדפדפן עם חשבון העבודה שלך בדייר שבו אתה רוצה את התצוגה המקדימה של Project Operations.

1. עבור אל [גירסת הניסיון של Project Operations](https://aka.ms/try-po) כדי לממש את קוד ההצעה הראשון, **Dynamics 365 Project Operations**.
2. אשר את ההזמנה.

  תראה שהצעת האישור מומשה בהצלחה.

## <a name="assign-licenses"></a>הקצאת רשיונות

> [!IMPORTANT]
> תזדקק תגישה ניהולית לפורטל Microsoft 365 של הארגון שלך כדי להשלים את השלבים הבאים.


1. עבור אל [מרכז הניהול של Microsoft 365](https://portal.office.com/) כדי להקצות את הרישיונות למשתמשים שלך.
2. בדף **משתמשים פעילים** בחר את המשתמשים שאליהם ברצונך להקצות רישיון.
3. ודא שהרישיון **Dynamics 365 Project Operations** נבחר. 
4. בחר **שמור שינויים**.

## <a name="create-a-new-dataverse-environment"></a>יצירת סביבת Dataverse חדשה

1. הקצאת סביבת פריסה של Dataverse ‏Project Operations על ידי ביצוע ההוראות במאמר [מודל הפריסה של Dataverse](lite-deployment.md). כאשר אתה בוחר את סוג הסביבה, הקפד להשתמש באפשרות **גירסת ניסיון (מבוסס מנוי)**.

  ![סביבה חדשה.](./media/19CreateEnvironment.png)

2. בחר את ההגדרה **הפעל יישומי Dynamics 365** והשאר את **פרוס יישומים אלה באופן אוטומטי** ריק.  
3. בחר **שמור** כדי ליצור סביבה חדשה.

  ![הוסף מסד נתונים.](./media/20CreateEnvironment1.png)

4. לאחר יצירת הסביבה, התקן את הפתרון **Microsoft Dynamics 365 Project Operations**. 

![התקן פתרון.](./media/21InstallSolution.png)

## <a name="install-a-cds-configuration-and-setup-demo-data"></a>התקן את התצורה של CSD ואת נתוני הגדרת ההדגמה

התקן את תצורת ה- CDS והגדר נתוני הדגמה על ידי ביצוע ההוראות במאמר [החל נתוני הגדרה ותצורה של הדגמה](lite-apply-demo-setup-config-data.md).


[!INCLUDE[footer-include](../includes/footer-banner.md)]
