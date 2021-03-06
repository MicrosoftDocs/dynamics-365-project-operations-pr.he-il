---
title: החל את נתוני ההדגמה של Project Operations בסביבת Finance המתארחת בענן
description: נושא זה מסביר כיצד להחיל נתוני הדגמה מ- Project Operations בסביבת Dynamics 365 Finance המתארחת בענן.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 1a94862d5a024eb1630f33c0c96699e8b4b49bf2
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948895"
---
# <a name="apply-project-operations-demo-data-to-a-finance-cloud-hosted-environment"></a>החל את נתוני ההדגמה של Project Operations בסביבת Finance המתארחת בענן

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

>[חשוב] נושא זה חל רק על Microsoft Dynamics 365 Finance בגירסה 10.0.13 בלבד וניתן לבצע אותו רק בסביבה המתארחת בענן. השלם את השלבים בנושא זה **לפני** שאתה מחיל עדכוני איכות על הסביבה.

1. בפרויקט LCS שלך, פתח את הדף **פרטי סביבה**. שים לב שהוא כולל את הפרטים הדרושים להתחברות לסביבה באמצעות פרוטוקול שולחן עבודה מרוחק (RDP).

![פרטי סביבת ](./media/1EnvironmentDetails.png)

הקבוצה הראשונה של האישורים המודגשים הם אישורי החשבון המקומי והם מכילים היפר-קישור לחיבור אל שולחן העבודה המרוחק. האישורים כוללים את שם המשתמש והסיסמה של מנהל הסביבה. הקבוצה השנייה של האישורים משמשת להתחברות אל SQL Server בסביבה זו.

2. התחבר מרחוק לסביבה באמצעות ההיפר-קישור **בחשבונות מקומיים** והשתמש **באישורי חשבון מקומי** כדי לבצע אימות.
3. עבור אל **Internet Information Services** > **מאגרי יישומים** > **AOSService** והפסק את השירות. אתה מפסיק את השירות בשלב זה כדי שתוכל להמשיך להחליף את מסד הנתונים של SQL.

![הפסק את AOS](./media/2StopAOS.png)

4. עבור אל **שירותים** והפסק את שני הפריטים הבאים:

- Microsoft Dynamics 365 Unified Operations: שירות ניהול אצווה
- Microsoft Dynamics 365 Unified Operations: מסגרת ייצוא ייבוא נתונים

![הפסק שירותים](./media/3StopServices.png)

5. פתח את Microsoft SQL Server Management Studio. היכנס באמצעות אישורי שרת SQL והשתמש במשתמש ובסיסמה axdbadmin מהדף **פרטי הסביבות** ב- LCS.

![SQL Server Management Studio](./media/4SSMS.png)

6. בסייר האובייקטים, **מסדי נתונים** ואתר את **AXDB**. אתה תחליף את מסד הנתונים במסד נתונים חדש שנמצא [במרכז ההורדות](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip). 
7. העתק את קובץ ה- zip ל- VM שאתה מחובר אליו מרחוק וחלץ את תוכן ה- zip.
8. ב- SQL Server Management Studio, לחץ באמצעות לחצן העכבר הימני על **AxDB** ואז בחר **משימות** > **שחזר** > **מסד נתונים**.

![שחזר את מסד הנתונים](./media/5RestoreDatabase.png)

9. בחר **מכשיר מקור** ונווט אל הקובץ שחולץ מה- zip שהעתקת.

![מכשירי מקור](./media/6SourceDevice.png)

10. בחר **אפשרויות** ואז בחר **החלף את מסד הנתונים הקיים** ו**סגור חיבורים קיימים למסד הנתונים המהווה יעד**. 
11. בחר **אישור**.

![שחזר הגדרות](./media/7RestoreSetting.png)

תקבל אישור כי שחזור AXDB הצליח. לאחר שתקבל אישור זה, תוכל לסגור את SQL Services Management Studio.

12. חזור אל **Internet Information Services** > **מאגרי יישומים** > **AOSService** והתחל את AOSService.
13. עבור אל **שירותים** והתחל את שני השירותים שהפסקת קודם לכן.

14. אתר את הכלי AdminUserProvisioning ב- VM זה. חפש תחת K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.
15. הפעל את קובץ ה- ‎.ext באמצעות כתובת המשתמש שלך בשדה **כתובת דוא"ל**. 
16. בחר **שלח**.

![הקצאת משאבים של משתמש מנהל מערכת](./media/8AdminUserProvisioning.png)

לוקח מספר דקות להשלים את התהליך. אתה אמור לקבל הודעת אישור שמשתמש מנהל המערכת עודכן בהצלחה.

17. לבסוף, הפעל את שורת הפקודה כמנהל מערכת ובצע iisreset

![איפוס IIS](./media/9IISReset.png)

18. סגור את הפעלת שולחן העבודה המרוחק והשתמש בדף **פרטי הסביבה** של LCS כדי להתחבר לסביבה ולאשר שהיא פועלת כצפוי.

![Finance and Operations](./media/10FinanceAndOperations.png)
