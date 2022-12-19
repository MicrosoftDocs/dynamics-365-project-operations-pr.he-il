---
title: הירשם למנוי Preview של Project Operations עבור תרחישים מבוססי משאבים/ללא מלאי
description: מאמר זה מספק מידע על אופן ההרשמה והפריסה של Project Operations עבור תרחישים מבוססי משאבים/ללא מלאי.
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 3164add153d77a52f85c2aac442dcf90baa24440
ms.sourcegitcommit: 0d11377bf3ac74c80afbd2013775fcc9869f926a
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 12/10/2022
ms.locfileid: "9842016"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a>הירשם למנוי Preview של Project Operations עבור תרחישים מבוססי משאבים/ללא מלאי

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_



מאמר זה כיצד להירשם להצעת הניסיון של סביבת Project Operations ולפרוס אותה עבור תרחישים מבוססי משאבים/ללא מלאי.

## <a name="prerequisites"></a>דרישות מוקדמות
- המשתמש שמבצע את הפריסה של ה-Preview חייב להיות בעל זכויות מנהל מערכת כלליות של דייר Azure. ניתן ליצור דייר במהלך מימוש ההצעה הראשונה. 
- פריסת סביבת Finance מחייבת מנוי תקף ל- Azure שיחויב לכל סביבה. באפשרותך להשתמש במנוי הקיים של הארגונים שלך או להשתמש [בגירסת ניסיון של Azure](https://azure.microsoft.com/free/) כדי להתחיל בעבודה. סביבת ה- CDS תינתן בחינם לתקופה מוגבלת של 30 יום.

> [!IMPORTANT]
> רק אדם אחד בארגון, מנהל הדיירים, צריך לבצע את המשימה הזו. אם אינך המנוי למהדורה זו, המתן עד שהארגון שלך יירשם ותקבל את אישורי המשתמש שלך.
> 
> גירסאות ניסיון הן לשימוש חד פעמי בדייר. אפשר להריץ גירסת ניסיון רק פעם אחת. אנו ממליצים ליצור דייר חדש לצורך גירסת הניסיון.


### <a name="dynamics-365-project-operations-ce---preview-trial"></a>Dynamics 365 Project Operations (CE) - גרסת ניסיון של Preview 

לפני שתתחיל, ודא שאתה מחובר לדפדפן עם חשבון העבודה שלך בדייר שבו אתה רוצה את התצוגה המקדימה של Project Operations.

1. ניתן לממש את קוד ההצעה הראשון, **Dynamics 365 Project Operations** כאן[ גרסת ניסיון של Project Operations](https://aka.ms/try-po).
2. אשר את ההזמנה.

  תראה שהצעת האישור מומשה בהצלחה.

### <a name="dynamics-365-finance-preview-trial"></a>גירסת הניסיון של Preview עבור Dynamics 365 Finance

עבור אל [גירסת ניסיון Preview של Dynamics 365 for Finance](https://aka.ms/trypoche) וחזור על השלבים מהמקטע הקודם עם ההצעה, הירשם לסביבה שמתארחת בענן.  

## <a name="assign-licenses"></a>הקצאת רשיונות

> [!IMPORTANT]
> תזדקק תגישה ניהולית לפורטל Microsoft 365 של הארגון שלך כדי להשלים את השלבים הבאים.

1. עבור אל [מרכז הניהול של Microsoft 365](https://portal.office.com/) כדי להקצות את הרישיונות למשתמשים שלך.

2. בדף **משתמשים פעילים** בחר את המשתמשים שאליהם ברצונך להקצות רישיון.

3. ודא שרישיון **Dynamics 365 Project Operations** נבחר ובחר **שמור שינויים**.

> [!NOTE]
> אין צורך להקצות למשתמש את הצעת גירסת הניסיון ל- Finance.

## <a name="start-a-new-project-in-lcs"></a>התחלת פרויקט חדש ב-LCS

צור פרויקט LCS חדש כמתואר במאמר, [התחל פרויקט חדש ב- LCS](create-lcs-project.md)

## <a name="add-an-azure-subscription-to-an-lcs-project"></a>הוסף מנוי Azure לפרויקט LCS

כדי להשלים משימה זו, בצע את השלבים במאמר, [הוספת מינוי Azure לפרויקט LCS](resource-add-azure-subscription-lcs-project.md).

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a>פרוס את סביבת ההדגמה של Finance עם Project Operations לתרחישים מבוססי משאבים/ללא מלאי‬

עקבו אחר ההנחיות במאמר, [הקצאת סביבה חדשה](resource-provision-new-environment.md) להשלמת הפריסה. השתמש בסוג הפריסה [סביבת הדגמה](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) עבור ה- Preview. 

## <a name="install-cds-setup-and-configuration-data"></a>התקן הגדרת CDS ונתוני תצורה

התקן את נתוני ההגדרה והתצורה של CDS כמתואר במאמר, [הגדר והחל נתוני תצורה ב- Common Data Service](resource-apply-pro-setup-config-data.md).
השלם שלב זה רק לאחר פריסה של סביבת ההדגמה של Finance ולאחר שנתוני ההדגמה יהיו מוכנים.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
