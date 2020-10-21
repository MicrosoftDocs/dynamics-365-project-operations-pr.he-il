---
title: הוסף מנוי Azure לפרויקט LCS
description: נושא זה מספק מידע על אופן חיבור המנוי שלך ל- Azure אל פרויקט LCS.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 0b5703542ac58adcc710890d9676dd0090a82f25
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948891"
---
# <a name="add-an-azure-subscription-to-lcs-project"></a>הוסף מנוי Azure לפרויקט LCS

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

יש לפרוס סביבות המתארחות בענן באמצעות מנוי קיים ל- Azure. נושא זה מסביר איך לחבר את המנוי הקיים שלך ל- Azure אל פרויקט LCS. 

## <a name="grant-admin-consent"></a>הענק הסכמה של מנהל מערכת

1. בפרויקט LCS שלך, במקטע **סביבות**, בחר **הגדרות Microsoft Azure**.

![הגדרות Microsoft Azure](./media/1MicrosoftAzureSettings.png)

2. בדף **הגדרות פרויקט**, בכרטיסיה **מחברי Azure**, בחר באפשרות **אשר**. כך מתאפשר לפרוס את הסביבות בפרויקט זה.

![מחברי Azure](./media/2AzureConnectors.png)

3. בחר שוב באפשרות **אשר** כדי לספק הסכמה של מנהל מערכת.

![הענק הסכמה של מנהל מערכת](./media/3GrantAdminConsent.png)

4. קבל את בקשת ההרשאות.

![קבל בקשת הרשאות](./media/4AcceptPermissionRequest.png)

ההרשאה הושלמה כעת. 

![ההרשאה נקבעה בהצלחה](./media/5AuthorizationComplete.png)

## <a name="provide-dynamics-deployment-services-access-to-your-azure-subscription"></a><a name="provide"></a>ספק גישה אל Dynamics Deployment Services למנוי שלך ב- Azure

1. עבור אל [חיוב Microsoft Azure](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) ובחר את המנוי שלך. כדי שתהיה אפשרות לפרוס סביבות, ל- Dynamics Deployment Services צריכה להיות גישה למנוי זה.

![פרטי מנוי Azure](./media/6AzureSubscription.png)

2. בחר באפשרות **בקרת גישה (IAM)** בחלונית הניווט ולאחר מכן בחר באפשרות **הוסף הקצאת תפקיד**.
3. במחוון שבצד ימין, בחר באפשרות **תפקיד תורם** וברשימה הנפתחת, אתר ובחר את האפשרות **Dynamics Deployment Services**. 
4. בחר **שמור**.

![גישה למנוי](./media/7SubscriptionAccess.png)

### <a name="add-a-subscription-connector-to-an-lcs-project"></a>הוסף מחבר מנוי לפרויקט LCS

1. בפרויקט LCS שלך, בדף **הגדרות Microsoft Azure**, בחר באפשרות **הוסף** כדי להוסיף מחבר חדש.
2. הזן את מזהה המנוי שלך ב- Azure. אתה יכול למצוא את מזהה המנוי שלך [בפורטל Azure](https://ms.portal.azure.com/), בקטע  **הגדרות**  בפינה השמאלית התחתונה של המסך.
3. בשדה **קבע את התצורה של Azure Resource Manager**, בחר באפשרות **כן**.
4. ודא שתחום דייר AAD של מנוי Azure תואם למנוי Azure המוגדר כבעלים של התחום שבו אתה משתמש, ובחר באפשרות **הבא**.
5. במסך **הגדרת Microsoft Azure**, בחר באפשרות **הבא** כדי לאשר. אם נתקלת בשגיאה במסך זה, חזור למקטע [ספק גישה אל Dynamics Deployment Services למנוי שלך ב- Azure](#provide) בנושא זה כדי לוודא שהשלמת את כל השלבים.
6. הורד את Azure Management Certificate לתיקיה מקומית במחשב שלך ולאחר מכן העלה אותו אל Azure Management Portal על-ידי מעבר אל **הגדרות** > **אישורי ניהול**. אישור זה יאפשר ל- LCS לתקשר עם Azure בשמך. אתה יכול לדלג על שלב זה אם למשתמש שלך יש גישה למנוי.
7. בחר באפשרות  **הבא**.
8. בחר את אזור Azure לפריסה ובחר מרכז נתונים הקרוב למקום בו אתה מתכנן להשתמש במערכת זו.
9.  בחר באפשרות  **התחבר**.

חיברת בהצלחה את המנוי שלך ל- Azure. כעת תוכל לפרוס סביבות המתארחות בענן של Dynamics 365 Finance.


