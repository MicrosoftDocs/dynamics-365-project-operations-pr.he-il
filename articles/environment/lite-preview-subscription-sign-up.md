---
title: רישום למנוי Preview‏ - Lite
description: מאמר זה מספק מידע על אופן ההרשמה והפריסה של Project Operations lite - מהעסקה ועד הפקת חשבונית פרופורמה.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 29bf31cd1bc9c1c5ac757de989154b4c7acc53fe
ms.sourcegitcommit: 16c9eded66d60d4c654872ff5a0267cccae9ef0e
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/07/2022
ms.locfileid: "9410012"
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

## <a name="set-up-demo-data"></a>הגדר נתונים הדגמה

הגדר נתוני הדגמה על ידי ביצוע ההוראות במאמר [החל נתוני הגדרה ותצורה של הדגמה](lite-apply-demo-setup-config-data.md).


[!INCLUDE[footer-include](../includes/footer-banner.md)]
