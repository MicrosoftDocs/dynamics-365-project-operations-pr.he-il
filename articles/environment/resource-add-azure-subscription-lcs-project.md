---
title: הוסף מנוי Azure לפרויקט LCS
description: מאמר זה מספק מידע על איך לחבר את מנוי Azure שלך לפרויקט LCS.
author: sigitac
ms.date: 04/12/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 64ee8cfa7394a08c3d588c0e8f4a73185d9496cf
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912149"
---
# <a name="add-an-azure-subscription-to-an-lcs-project"></a>הוסף מנוי Azure לפרויקט LCS

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

יש לפרוס סביבות המתארחות בענן באמצעות מנוי קיים ל- Azure. מאמר זה מסביר כיצד לחבר את מנוי Azure הקיים שלך לפרויקט LCS. 

## <a name="grant-admin-consent"></a>הענק הסכמה של מנהל מערכת

1. בפרויקט LCS שלך, במקטע **סביבות**, בחר **הגדרות Microsoft Azure**.

![הגדרות Microsoft Azure.](./media/1MicrosoftAzureSettings.png)

2. בדף **הגדרות פרויקט**, בכרטיסיה **מחברי Azure**, בחר באפשרות **אשר**. כך מתאפשר לפרוס את הסביבות בפרויקט זה.

![מחברי Azure.](./media/2AzureConnectors.png)

3. בחר שוב באפשרות **אשר** כדי לספק הסכמה של מנהל מערכת.

![הענק הסכמה של מנהל מערכת.](./media/3GrantAdminConsent.png)

4. קבל את בקשת ההרשאות.

![קבל בקשת הרשאות.](./media/4AcceptPermissionRequest.png)

ההרשאה הושלמה כעת. 

![ההרשאה נקבעה בהצלחה.](./media/5AuthorizationComplete.png)

## <a name="provide-dynamics-deployment-services-access-to-your-azure-subscription"></a><a name="provide"></a>ספק גישה אל Dynamics Deployment Services למנוי שלך ב- Azure

1. עבור אל [חיוב ב- Microsoft Azure](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) ובחר את המנוי שלך. כדי שתהיה אפשרות לפרוס סביבות, ל- Dynamics Deployment Services צריכה להיות גישה למנוי זה.

![פרטי מנוי Azure.](./media/6AzureSubscription.png)

2. בחר באפשרות **בקרת גישה (IAM)** בחלונית הניווט ולאחר מכן בחר באפשרות **הוסף הקצאת תפקיד**.
3. במחוון שבצד ימין, בחר באפשרות **תפקיד תורם** וברשימה הנפתחת, אתר ובחר את האפשרות **Dynamics Deployment Services**. 
4. בחר **שמור**.

![גישה למנוי.](./media/7SubscriptionAccess.png)

### <a name="add-a-subscription-connector-to-an-lcs-project"></a>הוסף מחבר מנוי לפרויקט LCS

1. בפרויקט LCS שלך, בדף **הגדרות Microsoft Azure**, בחר באפשרות **הוסף** כדי להוסיף מחבר חדש.
2. הזן את מזהה המנוי שלך ב- Azure. אתה יכול למצוא את מזהה המנוי שלך [בפורטל Azure](https://ms.portal.azure.com/), בקטע  **הגדרות**  בפינה השמאלית התחתונה של המסך.
3. בשדה **קבע את התצורה של Azure Resource Manager**, בחר באפשרות **כן**.
4. ודא שתחום דייר AAD של מנוי Azure תואם למנוי Azure המוגדר כבעלים של התחום שבו אתה משתמש, ובחר באפשרות **הבא**.
5. במסך **הגדרת Microsoft Azure**, בחר באפשרות **הבא** כדי לאשר. אם אתה מקבל שגיאה במסך זה, חזור למקטע [מתן גישה לשירותי פריסה של Dynamics אל מינוי Azure](#provide) במאמר זה וודא שהשלמת את כל השלבים.
6. הורד את אישור הניהול של Azure לתיקיה מקומית במחשב שלך. בקש ממנהל המינוי שלך ב- Azure להעלות את האישור לפורטל הניהול של Azure על ידי בחירת המנוי ומעבר אל **הגדרות** > **אישורי ניהול**. אישור זה מאפשר ל- LCS לתקשר עם Azure בשמך. אתה יכול לדלג על שלב זה אם למשתמש שלך יש גישה למנוי.
7. בחר באפשרות  **הבא**.
8. בחר את אזור Azure לפריסה ובחר מרכז נתונים הקרוב למקום בו אתה מתכנן להשתמש במערכת זו.
9.  בחר באפשרות  **התחבר**.

חיברת בהצלחה את המנוי שלך ל- Azure. כעת תוכל לפרוס סביבות המתארחות בענן של Dynamics 365 Finance.




[!INCLUDE[footer-include](../includes/footer-banner.md)]
