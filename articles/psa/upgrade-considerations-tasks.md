---
title: שיקולים לשדרוג עבור מבנה התפלגות העבודה
description: נושא זה מספק מידע לגבי שדרוג מבנה התפלגות העבודה מ- Project Service Automation 2.x ל- ‎3.x.
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
author: ruhercul
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
ms.openlocfilehash: 169dc24f0d1ae151ea5927123fb738221de88250
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077390"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a>שיקולים לשדרוג עבור מבנה התפלגות העבודה
נושא זה מספק מידע לגבי שדרוג מבנה התפלגות העבודה מ- Project Service Automation 2.x ל- ‎3.x. נושא זה מגדיר את המצב התקין של פרויקטים ב- Project Service Automation ‏(PSA) הנדרש לשדרוג מוצלח. הוא כולל גם מידע על תנאי החסימה הנפוצים שיגרמו לשדרוג להיכשל. לקבלת מידע נוסף על הגדרת משימות פרויקט והפונקציות שלהן במסגרת לוח זמנים של פרויקט, ראה [לוחות זמנים של פרויקטים](project-creating.md).

## <a name="key-entities"></a>ישויות עיקריות
עבור מבנה התפלגות עבודה מדויק שכבר נטענו בו משאבים, הישויות הבאות נדרשות:

- [פרויקט](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project)
- [צוות פרויקט](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam)
- [משימת פרויקט](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask)
- [הקצאות משאבים](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment)
- [‏‫יחס תלות במשימת פרויקט](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency)
- [משאבים הניתנים להזמנה](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/bookableresource)

כדי להגדיר מבנה התפלגות עבודה שנטען במשאבים, עליך להשלים את השלבים הבאים:

1. צור פרויקט חדש. לקבלת מידע נוסף על יצירת פרויקט חדש, ראה [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).
2. צור משימה אחת או יותר. לקבלת מידע נוסף על יצירת משימות, ראה [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).
3. הגדר את יחסי התלות בין המשימות. למידע נוסף ראה [תלות במשימת פרויקט](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).
4. הקצה חברי צוות פרויקט לפרויקט. לקבלת מידע נוסף, ראה [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).
5. הקצה חברי צוות פרויקט למשימות. לקבלת מידע נוסף, ראה [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).

## <a name="project-team-relationships"></a>קשרי גומלין בצוות הפרויקט

כדי להבטיח שדרוג מוצלח, יש לשמור כראוי על קשרי הגומלין הבאים:
- כל חברי צוות הפרויקט צריכים להיות משויכים למשאב הניתן להזמנה.
- כל חברי צוות הפרויקט צריכים להיות משויכים לאותו הפרויקט. 

## <a name="project-task-relationships"></a>קשרי גומלין במשימות הפרויקט
כדי להבטיח שדרוג מוצלח, יש לשמור כראוי על קשרי הגומלין הבאים:

- כל המשימות הקשורות חייבות להיות משויכות לאותו הפרויקט.
- כל משימת שורה צריכה משימת אב.
- כל משימה צריכה פרויקט אב.

### <a name="valid-conditions"></a>תנאים חוקיים

- כל משכי הזמן של המשימות חייבים להיות גדולים משעה אחת או שווים לה (>=) וקטנים מ- 1,800,000 דקות (1,250 ימים).*
- תאריך ההתחלה של כל המשימות חייב להתקיים ב- 01/01/2000 או לאחר מכן.*
- תאריך ההתחלה של כל המשימות חייב להתקיים 17 שנה לכל היותר מהתאריך הנוכחי.*
- תאריך ההתחלה של כל המשימות חייב להתקיים לפני תאריך הסיום או בתאריך הסיום.
- כל סוגי העסקאות בסיווגים ('הוצאה', 'חומר', 'מס' ו'זמן') חייבים להכיל ערכים של **יחידת ברירת מחדל** ו **קבוצת יחידות**.
- יש להימנע מתבניות תאריך הכוללות אותיות.

### <a name="potential-mitigation-steps"></a>שלבים פוטנציאליים לצמצום סיכונים
- השתמש בחיפוש מתקדם כדי לזהות משימות פרויקט שאינן מכילות מזהה פרויקט.
- השתמש בחיפוש מתקדם כדי לזהות משימות פרויקט שבהן משך הזמן המתוזמן גדול מ- 1,800,000.
- לפני ביצוע שינויים בנתונים, עליך לבדוק התאמות אישיות הקשורות לישות שעלולות לפגוע במצב הנתונים. יש להתייחס להתאמות אישיות אלה לפני שתמשיך בעדכונים הקשורים לנתונים.
- עבור המשימות שזוהו שהתייתמו, שקול למחוק משימות אלה אם אין בהן צורך יותר או אם יש לשייך אותן לפרויקט ההורה הנכון.
- עבור משימות שבהן משך הזמן הוא מעל 1,250 יום, שקול להוסיף משימות מרובות כדי לייצג את משך הזמן הכולל, אם הדבר אפשרי.

> [!NOTE]
> לפריטים שצוינו בכוכבית (\*) יש מגבלות הקשורות לכך שניהול קשרי לקוחות (CRM) תומך רק ב- 7,320 הרחבות מופע חוזר. יש להישאר מתחת למגבלה זו.

## <a name="resource-assignment-relationships"></a>קשרי גומלין של הקצאת משאבים
כדי להבטיח שדרוג מוצלח, יש לשמור כראוי על קשרי הגומלין הבאים:

- כל הקצאות המשאבים במבנה התפלגות העבודה חייבות להיות קשורות לאותו הפרויקט.
- כל הקצאות המשאבים במבנה התפלגות העבודה חייבות להיות משויכות לחברי צוות הפרויקט באותו הפרויקט.

### <a name="potential-mitigation-steps"></a>שלבים פוטנציאליים לצמצום סיכונים
- זהה את כל המשימות שאינן תואמות לתנאים המתוארים לעיל.  
- יש למחוק את כל מטלות המשאבים שאינן תקפות עוד.

## <a name="project-task-dependency-relationships"></a>קשרי גומלין של יחסי תלות של משימות הפרויקט
כדי להבטיח שדרוג מוצלח, יש לשמור כראוי על קשרי הגומלין הבאים:

- כל יחסי התלות של משימות הפרויקט חייבים להיות קשורים לאותו הפרויקט.
- לא ניתן להפנות לאותם יחסי תלות של משימות יותר מפעם אחת.