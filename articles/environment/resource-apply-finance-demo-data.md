---
title: החלת נתוני ההדגמה בסביבת Finance המתארחת בענן
description: נושא זה מסביר כיצד להחיל נתוני הדגמה מ- Project Operations בסביבת Dynamics 365 Finance המתארחת בענן.
author: sigitac
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: e4ccc7eb02fabdc0476fe454f33bff637ab8b835
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8588967"
---
# <a name="apply-demo-data-to-a-finance-cloud-hosted-environment"></a>החלת נתוני ההדגמה בסביבת Finance המתארחת בענן

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

> [!IMPORTANT]
> נושא זה ישים רק בגירסת Microsoft Dynamics 365 Finance‏ 10.0.13 וניתן לביצוע בסביבה המתארחת בענן בלבד. השלם את השלבים בנושא זה **לפני** שאתה מחיל עדכוני איכות על הסביבה.

1. בפרויקט LCS שלך, פתח את הדף **פרטי סביבה**. שים לב שהוא כולל את הפרטים הדרושים להתחברות לסביבה באמצעות פרוטוקול שולחן עבודה מרוחק (RDP).

![פרטי סביבה.](./media/1EnvironmentDetails.png)

הקבוצה הראשונה של האישורים המודגשים הם אישורי החשבון המקומי והם מכילים היפר-קישור לחיבור אל שולחן העבודה המרוחק. האישורים כוללים את שם המשתמש והסיסמה של מנהל הסביבה. הקבוצה השנייה של האישורים משמשת להתחברות אל SQL Server בסביבה זו.

2. התחבר מרחוק לסביבה באמצעות ההיפר-קישור **בחשבונות מקומיים** והשתמש **באישורי חשבון מקומי** כדי לבצע אימות.
3. עבור אל **Internet Information Services** > **מאגרי יישומים** > **AOSService** והפסק את השירות. אתה מפסיק את השירות בשלב זה כדי שתוכל להמשיך להחליף את מסד הנתונים של SQL.

![הפסק את AOS.](./media/2StopAOS.png)

4. עבור אל **שירותים** והפסק את שני הפריטים הבאים:

- Microsoft Dynamics 365 Unified Operations: שירות ניהול אצווה
- Microsoft Dynamics 365 Unified Operations: מסגרת לייצוא וייבוא נתונים

![הפסק שירותים.](./media/3StopServices.png)

5. פתח את Microsoft SQL Server Management Studio. היכנס באמצעות אישורי שרת SQL והשתמש במשתמש ובסיסמה axdbadmin מהדף **פרטי הסביבות** ב- LCS.

![SQL Server Management Studio.](./media/4SSMS.png)

6. בסייר האובייקטים, **מסדי נתונים** ואתר את **AXDB**. אתה תחליף את מסד הנתונים במסד נתונים חדש שנמצא [במרכז ההורדות](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip). 
7. העתק את קובץ ה- zip ל- VM שאתה מחובר אליו מרחוק וחלץ את תוכן ה- zip.
8. ב- SQL Server Management Studio, לחץ באמצעות לחצן העכבר הימני על **AxDB** ואז בחר **משימות** > **שחזר** > **מסד נתונים**.

![שחזר את מסד הנתונים.](./media/5RestoreDatabase.png)

9. בחר **מכשיר מקור** ונווט אל הקובץ שחולץ מה- zip שהעתקת.

![מכשירי מקור.](./media/6SourceDevice.png)

10. בחר **אפשרויות** ואז בחר **החלף את מסד הנתונים הקיים** ו **סגור חיבורים קיימים למסד הנתונים המהווה יעד**. 
11. בחר **OK**.

![שחזר הגדרות.](./media/7RestoreSetting.png)

תקבל אישור כי שחזור AXDB הצליח. לאחר שתקבל אישור זה, תוכל לסגור את SQL Services Management Studio.

12. חזור אל **Internet Information Services** > **מאגרי יישומים** > **AOSService** והתחל את AOSService.
13. עבור אל **שירותים** והתחל את שני השירותים שהפסקת קודם לכן.

14. אתר את הכלי AdminUserProvisioning ב- VM זה. חפש תחת K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.
15. הפעל את קובץ ה- ‎.ext באמצעות כתובת המשתמש שלך בשדה **כתובת דוא"ל**. 
16. בחר **שלח**.

![הקצאת משאבים של משתמש מנהל מערכת.](./media/8AdminUserProvisioning.png)

לוקח מספר דקות להשלים את התהליך. אתה אמור לקבל הודעת אישור שמשתמש מנהל המערכת עודכן בהצלחה.

17. לבסוף, הפעל את שורת הפקודה כמנהל מערכת ובצע iisreset

![איפוס IIS.](./media/9IISReset.png)

18. סגור את הפעלת שולחן העבודה המרוחק והשתמש בדף **פרטי הסביבה** של LCS כדי להתחבר לסביבה ולאשר שהיא פועלת כצפוי.

![.Finance and Operations](./media/10FinanceAndOperations.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]