---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 14 V3
description: נושא זה מספק מידע על מה חדש בעדכון המהדורה 14 V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/29/2020
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 1d0aeb4684ae04d8774a31a51664ceb84307b10d
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949381"
---
# <a name="project-service-automation-update-release-14-v3"></a>מהדורה 14, V3 של Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור יישום Dynamics 365 Project Service Automation‏ (PSA). מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 14, עדכון V3 של PSA. מספר ה-Build של גרסה זו הוא V3.10.4.21 והיא זמינה בלוח הזמנים הבא:

- **זמינות כללית (עדכון עצמי):** ינואר 2020
- **עדכון אוטומטי:** פברואר 2020

## <a name="update-release-14"></a>הפצת עדכון 14

### <a name="enhancements"></a>שיפורים

- Sales

     - ערכי שדה מותאמים אישית מ- **פרטי שורת הצעת מחיר** מועתקים אל **פרטי סעיף חוזה בפרויקט** כאשר הצעת מחיר מתעדכנת ל **נסגרה כזכייה**.
     - פרויקטים שאושרו יכולים להיות **נסגר כהפסד**.

- ניהול משאבים

     - בעת הארכת הזמנות, המשתמשים יתבקשו דרך תיבת דו-שיח לאישור לסכם את תוצאות ההזמנה ולספק קישור לשמירה על הזמנות.


### <a name="bug-fixes"></a>תיקוני באגים

- זמן והוצאה

     - תוקן: שופרה חווית המשתמש כאשר המשתמש לא בחר ערכים לתיקון.

- ניהול משאבים

     - תוקן: הזמנת משאב פעמים רבות גורמת לשם המשאב הניתן לספירה להופיע פעמים רבות.

- Sales

     - תוקן: מחיר המכירה הכולל לא מחושב עד שהמשתמש מכניס מחיר עלות להערכות ההוצאות על פרויקט.
     - תוקן: סגירת הצעת מחיר בתור **זכייה** נכשלה אם חוזה הפרויקט המשויך אינו במצב **טיוטה**.



[!INCLUDE[footer-include](../includes/footer-banner.md)]