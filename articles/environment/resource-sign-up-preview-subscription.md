---
title: הירשם למנוי Preview של Project Operations עבור תרחישים מבוססי משאבים/ללא מלאי
description: נושא זה מספק מידע אודות אופן ההרשמה ל- Project Operations ופריסה שלו עבור תרחישים מבוססי משאבים/ללא מלאי.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4d35a8bf9e8a841b45808b26ae2587c5b7d99d72
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948892"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a>הירשם למנוי Preview של Project Operations עבור תרחישים מבוססי משאבים/ללא מלאי

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

נושא מסביר כיצד להירשם כמנוי להצעת Preview/שותף וכיצד לפרוס את סביבת Project Operations לתרחישים מבוססי משאבים/ללא מלאי.

## <a name="prerequisites"></a>דרישות מוקדמות

- תקבל הודעת דואר המזמינה אותך להשתתף ב-Preview. ניתן לבקש Preview ב[אתר Project Operations](https://dynamics.microsoft.com/en-us/project-operations/overview/).
- המשתמש שמבצע את הפריסה של ה-Preview חייב להיות בעל זכויות מנהל מערכת כלליות של דייר Azure.
- פריסת סביבת Finance מחייבת מנוי תקף ל- Azure שיחויב לכל סביבה. באפשרותך להשתמש במנוי הקיים של הארגונים שלך או להשתמש [בגירסת ניסיון של Azure](https://azure.microsoft.com/en-us/free/) כדי להתחיל בעבודה. סביבת ה- CDS תינתן בחינם לתקופה מוגבלת של 30 יום.

## <a name="subscribe"></a>הירשם כמנוי

כש[בקשת ‎Preview](https://forms.office.com/FormsPro/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbR56j8lZs0FdAvwT75_WNFyxUMkRDV1NYQU5TNjE2VjhKOVBUNVg2R0s1NC4u) שלך תקבל אישור, תקבל שתי הצעות מ-Microsoft בדואר. הצעות אלה מאפשרות לך לפרוס את Project Operations Preview:

- Dynamics 365 Project Operations - גירסת הניסיון של Preview
- גירסת הניסיון של Preview עבור Dynamics 365 for Finance and Operations.

> [!IMPORTANT]
> רק אדם אחד בארגון, מנהל הדיירים, צריך לבצע את המשימה הזו. אם אינך המנוי למהדורה זו, המתן עד שהארגון שלך יירשם ותקבל את אישורי המשתמש שלך.

### <a name="dynamics-365-project-operations--preview-trial"></a>Dynamics 365 Project Operations - גרסת הניסיון של Preview

1. ממש את ההצעה הראשונה, **גירסת הניסיון של Dynamics 365 Project Operations**, באמצעות כתובת ה-URL המופיעה בהודעת ברוכים הבאים שנשלחה אליך.

![הצעה ראשונה](./media/1FirstOffer.png)

2. ודא שאתה מחובר כמשתמש המשתייך לארגון שיירשם כמנוי לשירות.
3. המשך במימוש ההצעה. 
4. בחר **כן, הוסף לתיק הלקוח שלי**.

![ממש הצעה](./media/2RedeemFirstOffer.png)

![אשר את ההצעה](./media/3ConfirmFirstOffer.png)

![ההצעה מומשה](./media/4OfferSuccessfulyRedeemed.png)

### <a name="dynamics-365-finance-preview-trial"></a>גירסת הניסיון של Preview עבור Dynamics 365 Finance

חזור על אותם שלבים עם ההצעה השנייה מהודעת ברוכים הבאים שנשלחה אליך.

## <a name="assign-licenses"></a>הקצאת רשיונות

> [!IMPORTANT]
> תזדקק לגישה מנהלתית לפורטל Office 365 של הארגון שלך כדי להשלים את השלבים הבאים.

1. עבור אל [מרכז הניהול של Microsoft 365](https://portal.office.com/) כדי להקצות רישיונות למשתמשים שלך.

![פורטל הניהול של Office](./media/5OfficeAdminPortal.png)

2. בדף **משתמשים פעילים** בחר את המשתמשים שאליהם ברצונך להקצות רישיון.

![הקצאת רשיונות](./media/6AssignLicenses.png)

3. ודא כי הרישיון ל- Project Operations נבחר ובחר **שמור שינויים**. 

> [!NOTE]
> אין צורך להקצות למשתמש את הצעת גירסת הניסיון ל- Finance.

## <a name="start-a-new-project-in-lcs"></a>התחלת פרויקט חדש ב-LCS

צור פרויקט LCS חדש כמתואר בנושא [התחלת פרויקט חדש ב- LCS](create-lcs-project.md)

## <a name="add-an-azure-subscription-to-an-lcs-project"></a>הוסף מנוי Azure לפרויקט LCS

להשלמת משימה זו, בצע את השלבים בנושא [הוסף מנוי Azure לפרויקט LCS](resource-add-azure-subscription-lcs-project.md).

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a>פרוס את סביבת ההדגמה של Finance עם Project Operations לתרחישים מבוססי משאבים/ללא מלאי‬

פעל לפי ההנחיות בנושא [הקצאת סביבה חדשה](resource-provision-new-environment.md) להשלמת הפריסה. השתמש בסוג הפריסה [סביבת הדגמה](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) עבור ה- Preview.

## <a name="install-cds-setup-and-configuration-data"></a>התקן הגדרת CDS ונתוני תצורה

התקן הגדרת CDS ונתוני תצורה כמתואר בנושא [הגדר והחל נתוני תצורה ב- Common Data Service](resource-apply-pro-setup-config-data.md).

