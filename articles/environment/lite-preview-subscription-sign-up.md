---
title: הרשמה למנוי Preview‏ - לייט
description: נושא זה מספק מידע על אופן ההרשמה ל-Project Operations ועל אופן פריסתו בגרסת לייט - מהעסקה ועד להוצאת חשבונית פרופורמה.
author: sigitac
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 44edf2613ea4b26dadbd9edc47c784c488c577de
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290045"
---
# <a name="sign-up-for-a-preview-subscription---lite"></a>הרשמה למנוי Preview‏ - לייט 

נושא זה מסביר כיצד להירשם כמנוי להצעת השותף המקדימה ולפרוס את Dynamics 365 Project Operations בפריסה קלה - משלב העסקה ועד לחשבונית פרופורמה.

> [!NOTE]
> תהליך זה ישתנה במהדורות הקרובות של Project Operations.

## <a name="prerequisites"></a>דרישות מוקדמות

- תקבל הודעת דואר המזמינה אותך להשתתף ב-Preview. ניתן לבקש Preview ב[אתר Project Operations](https://dynamics.microsoft.com/en-us/project-operations/overview/).
- המשתמש שמבצע את הפריסה של ה-Preview חייב להיות בעל זכויות מנהל מערכת כלליות של דייר Azure.
- עיין בכל התנאים וההגבלות.

## <a name="subscribe"></a>הירשם כמנוי

כשתקבל [אישור לבקשת ‎,Preview](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u), תקבל שתי הצעות מ-Microsoft בדואר. הצעות אלה מאפשרות לך לפרוס את Project Operations Preview:

- Dynamics 365 Project Operations (CRM)‎ - גירסת ניסיון
- Office 365 Project Operations - גירסת ניסיון של Preview

> [!IMPORTANT]
> רק אדם אחד בארגון, מנהל הדיירים, צריך לבצע את המשימה הזו. אם אינך המנוי למהדורה זו, המתן עד שהארגון שלך יירשם ותקבל את אישורי המשתמש שלך.

### <a name="dynamics-365-project-operations-crm---preview-trial"></a>Dynamics 365 Project Operations (CRM)‎ - גירסת ניסיון 

לפני שתתחיל, ודא שאתה מחובר לדפדפן עם חשבון העבודה שלך בדייר שבו אתה רוצה את התצוגה המקדימה של Project Operations.

1. ניתן לממש את קוד המבצע הראשון, **Dynamics 365 Project Operations (CRM)‎ - גרסת ניסיון של Preview** על ידי הדבקה בכתובת האתר בדפדפן.

![ממש הצעה](./media/16RedeemFirstOfferNew.png)

2. אשר את ההזמנה.
![אשר את ההזמנה](./media/17ConfirmOrderNew.png)

תראה שהצעת האישור מומשה בהצלחה.

![אישור](./media/18OrderConfirmationNew.png)

### <a name="office-365-project-operations---preview-trial"></a>Office 365 Project Operations - גירסת ניסיון של Preview

חזור על אותם שלבים כמו בקוד המבצע הראשון. הקפד להוסיף את קוד המבצע השני באמצעות אותו חשבון משתמש שבו השתמשת עם קוד המבצע הראשון.

## <a name="assign-licenses"></a>הקצאת רשיונות

> [!IMPORTANT]
> תזדקק לגישה מנהלתית לפורטל Microsoft 365 של הארגון שלך כדי להשלים את השלבים הבאים.


1. עבור אל [מרכז הניהול של Microsoft 365](https://portal.office.com/) כדי להקצות את הרישיונות למשתמשים שלך.

![דף הבית של מרכז הניהול](./media/14AdminPortal.png)

2. בדף **משתמשים פעילים** בחר את המשתמשים שאליהם ברצונך להקצות רישיון.

![הקצאת רשיונות](./media/15AssignLicenses.png)

3. ודא שהרישיונות **Dynamics 365 Project Operations (CRM) Preview** ו- **Office 365 Project Operations - Preview** נבחרו. 
4. בחר **שמור שינויים**.

## <a name="create-a-new-cds-environment"></a>צור סביבת CDS חדשה

1. הקצה סביבת פריסת CDS חדשה של Project Operations על ידי מעקב אחר ההוראות בנושא זה, [מודל פריסת CDS](lite-deployment.md). כאשר אתה בוחר את סוג הסביבה, הקפד להשתמש באפשרות **גירסת ניסיון (מבוסס מנוי)**.
![סביבה חדשה](./media/19CreateEnvironment.png)

2. בחר את ההגדרה **הפעל יישומי Dynamics 365** והשאר את **פרוס יישומים אלה באופן אוטומטי** ריק.  
3. בחר **שמור** כדי ליצור סביבה חדשה.

![הוסף מסד נתונים](./media/20CreateEnvironment1.png)

4. לאחר יצירת הסביבה, התקן את הפתרון **Microsoft Dynamics 365 Project Operations**. 

![התקנת פתרון](./media/21InstallSolution.png)

## <a name="install-a-cds-configuration-and-setup-demo-data"></a>התקן את התצורה של CSD ואת נתוני הגדרת ההדגמה

התקן את תצורת ה-CDS והגדר נתוני הדגמה על ידי מעקב אחר ההוראות בנושא, [החל הגדרת ההדגמה ואת נתוני התצורה](lite-apply-demo-setup-config-data.md).


[!INCLUDE[footer-include](../includes/footer-banner.md)]