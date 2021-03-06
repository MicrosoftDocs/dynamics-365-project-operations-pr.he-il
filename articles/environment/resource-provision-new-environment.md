---
title: הקצאת סביבה חדשה
description: נושא זה מספק מידע אודות אופן הקצאת סביבת Project Operations חדשה.
author: sigitac
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 45700371c50e3b5a840df45fc24fa8a5b4584b61
ms.sourcegitcommit: 87b7a8d793c19c50f3765b8d788cde24a6a0ca24
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/02/2020
ms.locfileid: "3949363"
---
# <a name="provision-a-new-environment"></a>הקצאת סביבה חדשה

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

נושא זה מספק מידע אודות אופן הקצאת סביבת Dynamics 365 Project Operations חדשה לתרחישים מבוססי משאבים/ללא מלאי.

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a>הפוך הקצאת משאבים אוטומטית של Project Operations לזמינה בפרויקט LCS

השתמש בשלבים הבאים כדי להפוך את זרימת הקצאת המשאבים האוטומטית של Project Operations לאוטומטית עבור פרויקט LCS שלך.

1. עבור אל [LCS](https://lcs.dynamics.com/v2) ובחר את האריח **ניהול תכונת תצוגה מקדימה**.
2. ברשימת **תכונות התצוגה המקדימה**, בחר **Project Operations** ואז בחר **תכונת תצוגה מקדימה זמינה** כדי להפוך את Project Operations לזמין.

> [!NOTE]
> שלב זה מבוצע פעם אחת בלבד לכל פרויקט LCS.

## <a name="provision-a-project-operations-environment"></a>הקצאת סביבת Project Operations

1. פתח פריסת [סביבת הדגמה](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) או [ארגז חול (Sandbox)‬/ סביבת ייצור](https://docs.microsoft.com/edynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) חדשה של Dynamics 365 Finance. 
2. הסבר על אשף **הקצאת הסביבה**. 

> [!IMPORTANT]
> ודא שגירסת היישום שנבחרה היא 10.0.13 ומעלה.

3. להקצאת Project Operations, תחת **הגדרות מתקדמות**, בחר **Common Data Service**. 
4. הפוך את **הגדרת Common Data Service** לזמינה על-ידי בחירת **כן** ואז הזן מידע בשדות הנדרשים:

  - שם
  - אזור
  - שפה
  - מטבע
 
5. בתוך השדה **תבנית Common Data Service**, בחר **Project Operations** 

6. בחר את סוג הסביבה לפריסה. גירסת ניסיון מבוססת-מנוי תאפשר לך לפרוס סביבת CDS למשך 30 יום. 

![הגדרות פריסה](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> בחר **מסכים** כדי להסכם לתנאי השירות ואז בחר **סיום** כדי לחזור להגדרות הפריסה.

![הסכמת פריסה](./media/2DeploymentConsent.png)

7. מלא את שאר השדות הנדרשים באשף ואשר את הפריסה. זמן הקצאת הסביבה משתנה בהתאם לסוג הסביבה. ההקצאה עשויה להימשך עד שש שעות.

  לאחר השלמת הפריסה בהצלחה, הסביבה תוצג בתור **פרוסה**.

8. כדי לאשר שהסביבה נפרסה בהצלחה, בחר **כניסה** והיכנס לסביבה כדי לאשר.

![פרטי סביבת ](./media/3EnvironmentDetails.png)

## <a name="apply-project-operations-finance-demo-data-optional-step"></a>החל את נתוני ההדגמה של Project Operations Finance (שלב אופציונלי)

החל את נתוני ההדגמה של Project Operations Finance בסביבה המתארחת בענן במהדורת שירות 10.0.13 כמתואר [במאמר הזה](resource-apply-finance-demo-data.md).

## <a name="apply-updates-to-the-finance-environment"></a>החל עדכונים על סביבת Finance

ל- Project Operations נדרשת סביבת Finance עם גירסת יישום **10.0.13 (10.0.569.20009)** ומעלה.

ייתכן שתצטרך להחיל עדכוני איכות על סביבת Finance שלך כדי לקבל גירסה זו.

1. ב- LCS, בדף **פרטי הסביבה**, במקטע **עדכונים זמינים**, בחר **הצג עדכון**.

![הצג עדכונים](./media/5ViewUpdates.png)

2. בדף **עדכונים בינאריים**, בחר **שמור חבילה.**

![שמור חבילה](./media/6SavePackage.png)

3. לחץ על **בחר הכל** ולאחר מכן בחר **שמור חבילה**.

![סקור ושמור עדכונים](./media/7ReviewAndSaveUpdates.png)

4. הזן שם ותיאור לחבילה ולאחר מכן בחר **שמור**. בהתאם לחיבור האינטרנט, תהליך זה עשוי להימשך זמן מה.

![העלה חבילה לספריית הנכסים](./media/8UploadPackageToAssetsLibrary.png)

5. לאחר שמירת החבילה, בחר **סיום** ושמור חבילה זו בספריית הנכסים בפרויקט LCS שלך.

שמירת ואימות החבילה עשויה לארוך כ- 15 דקות.

6. כדי להחיל את העדכון, נווט אל הדף **פרטי הסביבה** ב- LCS ובחר **תחזק** > **החל עדכונים**.

![תחזק סביבות](./media/9MaintainEnvironment.png)

7. ברשימת העדכונים, בחר את החבילה שיצרת ובחר **החל**.

![החל עדכונים](./media/10ApplyUpdates.png)

מתן השירות לסביבה ייקח זמן מה. לאחר ההשלמה, הסביבה תחזור למצב פרוס.

![סביבה פרוסה](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a>יצירת חיבור כתיבה כפולה 

1. בפרויקט LCS שלך, עבור אל הדף **פרטי סביבה**.
2. בקטע **פרטי סביבה של Common Data Service**, בחר **קישור ל- CDS עבור יישומים**.
3. לאחר השלמת הקישור, בחר **קישור ל- CDS עבור יישומים** שוב. תועבר לכתיבה כפולה ב- Finance.

![קישור ל- CDS](./media/12LinktoCDS.png)

4. בחר **החל פתרון** כדי לגשת לישויות אשר ימופו בשילוב.

![החל פתרונות](./media/13ApplySolutions.png)

5. בחר בשני הפתרונות **מפת ישות כתיבה כפולה ב- Dynamics 365 Finance and Operations** ו**מפות ישות כתיבה כפולה ב- Dynamics 365 Project Operations** ולאחר מכן בחר **החל**.

![אשר פתרונות](./media/14ConfirmSolutions.png)

לאחר החלת הפתרונות, ישויות הכתיבה הכפולה מוחלות על הסביבה.

![מחיל פתרונות](./media/15ApplyingSolutions.png)

לאחר החלת הישויות, כל המיפויים הזמינים רשומים בסביבה.

![מפות של כתיבה כפולה](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a>רענן את ישויות הנתונים לאחר העדכון

1. ב- Finance, עבור אל סביבת העבודה **ניהול נתונים**.

![סביבת עבודה של ניהול נתונים](./media/16DataManagement.png)

2. בחר את האריח **פרמטרים של מסגרת**.

![פרמטרים של מסגרת](./media/17FrameworkParameters.png)

3. בדף **הגדרות ישות**, בחר **רענן את רשימת הישויות**.

![רענן את רשימת הישויות](./media/18RefreshEntityList.png)

הרענון יימשך כ- 20 דקות. תקבל התראה כשהוא יסתיים.

![רענן אישור](./media/19RefreshConfirmation.png)

## <a name="run-project-operations-dual-write-maps"></a>הפעל את מפות כתיבה כפולה ב- Project Operations

1. בפרויקט LCS שלך, עבור אל הדף **פרטי סביבה**.
2. בקטע **פרטי סביבה של Common Data Service**, בחר **קישור ל- CDS עבור יישומים.** לאחר שתבחרו בקישור, תועברו לרשימת הישויות במיפויים.
3. התחל את המפות כמתואר בטבלה הבאה. הקפד לעקוב אחר הרצף כמפורט.

| **מפת ישויות** | **רענן ישות** | **סינכרון ראשוני** | **פריט ראשי לסינכרון ראשוני** | **הפעל דרישות מוקדמות** | **סינכרון ראשוני של דרישות מוקדמות** |
| --- | --- | --- | --- | --- | --- |
| **תפקידי משאבי פרויקט לכל החברות (bookableresourcecategories)** | Yes | ‏‏כן | Common Data Service | Yes | לא זמין |
| **ישויות משפטיות (cdm\_companies)** | Yes | ‏‏כן | יישומי Finance and Operations | Yes | לא זמין |
| **שילוב Project Operations בפועל (msdyn\_actuals)** | Yes | Yes | לא זמין | ‏‏כן | Yes |
| **סעיפי חוזה של פרויקט (salesorderdetails)** | Yes | Yes | לא זמין | Yes | Yes |
| **‏‫ישות שילוב ליחסי גומלין של עסקה בפרויקט‬ (msdyn\_transactionconnections)** | Yes | Yes | לא זמין | Yes | לא זמין |
| **אבני דרך בסעיף חוזה לשילוב Project Operations (msdyn\_contractlinesscheduleofvalues)** | Yes | Yes | לא זמין | Yes | לא זמין |
| **ישות שילוב Project Operations להערכת הוצאות (msdyn\_estimateslines)** | Yes | Yes | לא זמין | Yes | לא זמין |
| **ישות שילוב Project Operations להערכת שעות (msdyn\_resourceassignments)** | Yes | Yes | לא זמין | Yes | לא זמין |
| **ישות ייצוא הוצאות פרויקט בשילוב Project Operations (msdyn\_expenses)** | ‏‏כן | Yes | לא זמין | Yes | לא זמין |
| **ישות שילוב Project Operations להערכת שעות (msdyn\_resourceassignments)** | ‏‏כן | Yes | לא זמין | Yes | לא זמין |

4. כדי לרענן את הישות, בחר את שם המפה ואז בחר **רענן ישויות**. 
5. המשך בהפעלת המפה לאחר השלמת הרענון.

![רענן מפה](./media/20RefreshMapping.png)

לפני הפיכת המפה הבאה לזמינה, ודא שהמפה בטבלה במצב **פועלת**. הפעלת מפות עם מספר גדול יותר של תנאים מוקדמים עשויה להימשך זמן מה.

להפעלת מפה עם תנאים מוקדמים, החלף את המצב של הלחצן **הצג מפות ישויות קשורות** לפועל. אם הטבלה מציינת כי **סינכרון ראשוני של דרישות מוקדמות** הוא במצב **לא**, ודא שהדגל **סינכרון ראשוני** הוא **כבוי** בכל מפות הדרישה המוקדמת לפני שתפעיל אותה.

![הפעל מפה](./media/21RunMap.png)

6. ודא שכל המפות הקשורות לפרויקט במצב פועל.

![כל המפות פועלות](./media/22AllMapsRunning.png)

סביבת Project Operations שלך מוקצית ומוגדרת כעת.
