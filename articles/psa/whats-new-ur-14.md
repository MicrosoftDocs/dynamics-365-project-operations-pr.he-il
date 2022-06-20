---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 14 V3
description: מאמר זה מספק מידע על הדברים החדשים והדברים שהשתנו ב- Project Service Automation מהדורת עדכון 14, גרסה 3.
author: ruhercul
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
ms.reviewer: johnmichalak
ms.openlocfilehash: e8e5132f970e3ec5742842175c118faf98a7b079
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8926547"
---
# <a name="project-service-automation-update-release-14-v3"></a>מהדורה 14, V3 של Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון עבור יישום Dynamics 365 Project Service Automation‏ (PSA). מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות. מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

מאמר זה מפרט את התכונות והתיקונים החדשים או ששונו עבור PSA בגרסה 3, מהדורת עדכון 14. מספר ה-Build של גרסה זו הוא V3.10.4.21 והיא זמינה בלוח הזמנים הבא:

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
