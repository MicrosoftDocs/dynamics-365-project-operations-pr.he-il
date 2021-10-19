---
title: הקצאת סביבה חדשה
description: נושא זה מספק מידע אודות אופן הקצאת סביבת Project Operations חדשה.
author: sigitac
ms.date: 09/13/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7f63b144b6fe3eb848d0c303b64237516a97cb56
ms.sourcegitcommit: 083e3d219cd5126eecb74debb1b70b361680b1f6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/18/2021
ms.locfileid: "7501417"
---
# <a name="provision-a-new-environment"></a>הקצאת סביבה חדשה

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

נושא זה מספק מידע על הדרך להקצות סביבת Dynamics 365 Project Operations חדשה לתרחישים מבוססי משאבים/ללא מלאי.

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a>הפוך הקצאת משאבים אוטומטית של Project Operations לזמינה בפרויקט LCS

השתמש בשלבים הבאים כדי להפוך את זרימת הקצאת המשאבים האוטומטית של Project Operations לאוטומטית עבור פרויקט LCS שלך.

1. עבור אל [LCS](https://lcs.dynamics.com/v2) ובחר את האריח **ניהול תכונת תצוגה מקדימה**.
2. ברשימת **תכונות התצוגה המקדימה**, בחר **תכונת Project Operations** ואז בחר **תכונת Preview זמינה** כדי להפוך את Project Operations לזמין.

   > [!NOTE]
   > שלב זה מבוצע פעם אחת בלבד לכל פרויקט LCS.

## <a name="provision-a-project-operations-environment"></a>הקצאת סביבת Project Operations

1. פתח פריסה חדשה של Dynamics 365 Finance [סביבת הדגמה](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) או [סביבת ארגז חול/ ייצור](/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure). 
2. הסבר על אשף **הקצאת הסביבה**. 

   > [!IMPORTANT]
   > ודא שגירסת היישום שנבחרה היא 10.0.13 ומעלה.

3. להקצאת Project Operations, תחת **הגדרות מתקדמות**, בחר **Common Data Service**. 
4. הפוך את **הגדרת Common Data Service** לזמינה על-ידי בחירת **כן** ואז הזן מידע בשדות הנדרשים:

  - שם
  - אזור
  - שפה
  - מטבע
 
5. בשדה **תבנית Common Data Service**, בחר **Project Operations** 
6. בחר את סוג הסביבה לפריסה. גירסת ניסיון מבוססת-מנוי תאפשר לך לפרוס סביבת CDS למשך 30 יום. 

     ![הגדרות פריסה.](./media/1DeploymentSettings.png)

    > [!IMPORTANT]
    > בחר **מסכים** כדי להסכם לתנאי השירות ואז בחר **סיום** כדי לחזור להגדרות הפריסה.
    >
    >![הסכמת פריסה.](./media/2DeploymentConsent.png)

7. אופציונלי - החל נתוני הדגמה על הסביבה. עבור אל **הגדרות מתקדמות**, בחר **התאם אישית את תצורת מסד הנתונים של SQL**, והגדר **ציין ערכת נתונים למסד נתונים של יישומים** שיהיה **הדגמה**.
8. מלא את שאר השדות הנדרשים באשף ואשר את הפריסה. הזמן להקצאה של הסביבה משתנה בהתאם לסוג הסביבה. ההקצאה עשויה להימשך עד שש שעות.

   לאחר השלמת הפריסה בהצלחה, הסביבה תוצג בתור **פרוסה**.

9. כדי לאשר שהסביבה נפרסה בהצלחה, בחר **התחברות** והיכנס לסביבה כדי לאשר.

    ![פרטי סביבה.](./media/3EnvironmentDetails.png)

## <a name="apply-updates-to-the-finance-environment"></a>החל עדכונים על סביבת Finance

ל- Project Operations נדרשת סביבת Finance עם גירסת יישום **10.0.13 (10.0.569.20009)** ומעלה.

ייתכן שתצטרך להחיל עדכוני איכות על סביבת Finance שלך כדי לקבל גירסה זו.

1. ב- LCS, בדף **פרטי הסביבה**, במקטע **עדכונים זמינים**, בחר **הצג עדכון**.

    ![הצג עדכונים.](./media/5ViewUpdates.png)

2. בדף **עדכונים בינאריים**, בחר **שמור חבילה.**

    ![שמור חבילה.](./media/6SavePackage.png)

3. לחץ על **בחר הכל** ולאחר מכן בחר **שמור חבילה**.

    ![סקור ושמור עדכונים.](./media/7ReviewAndSaveUpdates.png)

4. הזן שם ותיאור לחבילה ולאחר מכן בחר **שמור**. בהתאם לחיבור האינטרנט, תהליך זה עשוי להימשך זמן מה.

    ![העלה חבילה לספריית הנכסים.](./media/8UploadPackageToAssetsLibrary.png)

5. לאחר שמירת החבילה, בחר **סיום** ושמור חבילה זו בספריית הנכסים בפרויקט LCS שלך.

   שמירת ואימות החבילה עשויה לארוך כ- 15 דקות.

6. כדי להחיל את העדכון, נווט אל הדף **פרטי הסביבה** ב- LCS ובחר **תחזק** > **החל עדכונים**.

    ![תחזק סביבות.](./media/9MaintainEnvironment.png)

7. ברשימת העדכונים, בחר את החבילה שיצרת ובחר **החל**.

    ![החל עדכונים.](./media/10ApplyUpdates.png)

   מתן השירות לסביבה ייקח זמן מה. לאחר ההשלמה, הסביבה תחזור למצב פרוס.

    ![סביבה פרוסה.](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a>יצירת חיבור כתיבה כפולה 

1. בפרויקט LCS שלך, עבור אל הדף **פרטי סביבה**.
2. בקטע **פרטי סביבה של Common Data Service**, בחר **קישור ל- CDS עבור יישומים**.
3. לאחר השלמת הקישור, בחר **קישור ל- CDS עבור יישומים** שוב. תועבר לכתיבה כפולה ב- Finance.

    ![קישור ל- CDS.](./media/12LinktoCDS.png)

4. בחר **החל פתרון** כדי לגשת לישויות אשר ימופו בשילוב.

    ![החל פתרונות.](./media/13ApplySolutions.png)

5. בחר את שני הפתרונות, **מפת ישויות כתיבה כפולה של Dynamics 365 Finance and Operations** ו- **מפות ישויות כתיבה כפולה של Dynamics 365 Project Operations** ואז בחר **החל**.

    ![אשר פתרונות.](./media/14ConfirmSolutions.png)

    לאחר החלת הפתרונות, ישויות הכתיבה הכפולה מוחלות על הסביבה.

    ![מחיל פתרונות.](./media/15ApplyingSolutions.png)

    לאחר החלת הישויות, כל המיפויים הזמינים רשומים בסביבה.

    ![מפות של כתיבה כפולה.](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a>רענן את ישויות הנתונים לאחר העדכון

1. ב- Finance, עבור אל סביבת העבודה **ניהול נתונים**.

    ![סביבת עבודה של ניהול נתונים.](./media/16DataManagement.png)

2. בחר את האריח **פרמטרים של מסגרת**.

    ![פרמטרים של מסגרת.](./media/17FrameworkParameters.png)

3. בדף **הגדרות ישות**, בחר **רענן את רשימת הישויות**.

    ![רענן את רשימת הישויות.](./media/18RefreshEntityList.png)

הרענון יימשך כ- 20 דקות. תקבל התראה כשהוא יסתיים.

  ![רענן אישור.](./media/19RefreshConfirmation.png)

## <a name="update-security-settings-on-project-operations-on-dataverse"></a>עדכן את הגדרות האבטחה של Project Operations ב- Dataverse

1. עבור אל Project Operations בסביבת Dataverse שלך. 
2. עבור אל **הגדרות** > **אבטחה** > **תפקידי אבטחה**. 
3. בדף **תפקידי אבטחה**, ברשימת התפקידים, בחר **משתמש באפליקציה עם כתיבה כפולה** ובחר את הכרטיסיה **ישויות מותאמות אישית**.  
4. ודא שלתפקיד יש הרשאות **קריאה** ו **צירוף אל** עבור הישויות הבאות:
      
      - **סוג שער החליפין של מטבע**
      - **תרשים של תיקי לקוחות**
      - **לוח שנה כספי**
      - **ספר חשבונות**
      - **חברה**
      - **סוג שער החליפין של מטבע**
      - **הוצאה**

5. לאחר עדכון תפקיד האבטחה, עבור אל **הגדרות** > **אבטחה** > **Teams‎**, ובחר את צוות ברירת המחדל בתצוגה **בעל עסק מקומי**.
6. בחר **נהל תפקידים** וודא כי הרשאת האבטחה **משתמש באפליקציה עם כתיבה כפולה** מוחלת על צוות זה.

## <a name="run-project-operations-dual-write-maps"></a>הפעל את מפות כתיבה כפולה ב- Project Operations

1. בפרויקט LCS שלך, עבור אל הדף **פרטי סביבה**.
2. בקטע **פרטי סביבה של Common Data Service**, בחר **קישור ל- CDS עבור יישומים.** לאחר שתבחרו בקישור, תועברו לרשימת הישויות במיפויים.
3. הפעל את המפות. לקבלת מידע נוסף, ראה [גירסאות מפה של כתיבה כפולה של Project Operations](resource-dual-write-maps.md#project-operations-dual-write-maps)
4. ודא שכל המפות הקשורות לפרויקט במצב פועל.

    ![כל המפות פועלות.](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a>החלת נתוני תצורה ב-CDS עבור Project Operations (אופציונלי)

אם החלת נתוני הדגמה על סביבת Finance, ראה [הגדרה והחלה של נתוני תצורה ב-Common Data Service עבור Project Operations](resource-apply-pro-setup-config-data.md) כדי להחיל נתוני הדגמה על סביבת CDS.


סביבת Project Operations שלך מוקצית ומוגדרת כעת. 


[!INCLUDE[footer-include](../includes/footer-banner.md)]
