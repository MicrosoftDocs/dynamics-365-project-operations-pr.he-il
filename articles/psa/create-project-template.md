---
title: ליצור תבנית פרוייקט
description: כיצד ליצור תבנית פרוייקט ב- Project Service
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: 700d1bb1fd7299b49b6c6f8e4d84d14bc1d52c1a
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077321"
---
# <a name="create-a-project-template-project-service"></a>יצירת תבנית פרוייקט (Project Service)

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

תבניות פרוייקטים חוסכות לך זמן אם החברה שלך באופן קבוע משתתפת במכרזים עבור סוגים דומים של פרוייקטים. הן מספקות קבוצת תפקידים רגילה ושעות משוערות‬ עבור סוג של פרוייקט. מנהלי פרוייקטים ומנהלי תיקי לקוחות יכולים ליצור פרוייקטים בהתבסס על תבנית פרוייקט, או הם יכולים להעתיק את התבנית וליצור אחת משלהם.  
  
## <a name="components-of-project-template"></a>רכיבים של תבנית פרוייקט
 תבנית פרוייקט כוללת שלושה מרכיבים:  
  
- **מבנה התפלגות עבודה** : מבנה התפלגות עבודה בתבנית הפרוייקט מכיל אותה קבוצת רכיבים כמו בפרוייקט. באפשרותך ליצור היררכיית משימות, לשייך תפקידים למשימה, להגדיר תכונות של לוח זמנים, להגדיר יחסי תלות ולהציג את כל הנתונים ב- Gantt. מבנה התפלגות העבודה בתבניות פרוייקט תומך גם במצבי משימה עבור כל משימה. אין כל הבדל בין תבנית פרוייקט ופרוייקט בעת יצירת לוח זמנים לעבודה.  
  
- **הערכות פרוייקט** : הערכות פרוייקט בתבניות פועלות באותו האופן כמו בפרוייקטים, מלבד העובדה שמחירונים המשמשים להגדרת ברירת המחדל של העלות ומחירי המכירה הם תמיד העלות ומחירוני המכירות שהוגדרו כברירת מחדל בפרמטרים של [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. שאר הפונקציונליות היא כמו בפרוייקט.  
  
- **יצירת צוות פרוייקט** : בעת יצירת צוות פרוייקט עבור תבנית פרוייקט, אין אפשרות להזמין משאב בעל שם בתבנית. באפשרותך להשתמש באפשרות **צור צוות פרוייקט** במבנה התפלגות העבודה כדי ליצור קבוצת משאבים כלליים. באפשרותך גם לציין את הכישורים והמומחיות הנדרשים עבור משאבים כלליים. לא ניתן להחליף משאב כללי במשאב הניתן להזמנה בתבניות פרוייקט.  
  
## <a name="create-a-project-from-a-template"></a>יצירת פרוייקט מתבנית  
 ניתן ליצור פרוייקט מתבנית בדרכים הבאות:  
  
-   בעת יצירת פרוייקט מהצעת המחיר, באפשרותך לבחור תבנית פרוייקט בטופס יצירה מהירה של פרוייקט.  
  
-   בעת יצירת פרוייקט על-ידי לחיצה על **פרוייקט חדש** , יוצג טופס הפרוייקט לפני שמירת הרשומה. מכאן, באפשרותך ללחוץ על השדה **בחר תבנית** כדי לבחור מתוך רשימת תבניות פרוייקט מוגדרות מראש בארגון שלך.  
  
-   לחץ על **צור פרוייקט מתבנית** בדף **תבנית פרוייקט** כדי ליצור פרוייקט מהתבנית.  
  
## <a name="copying-components-of-a-template-to-a-project"></a>העתקת רכיבי תבנית לפרוייקט  
 בעת העתקת רכיבי תבנית לפרוייקט, ישנם כמה דברים שעליך לדעת.  
  
 **העתקת מבנה התפלגות עבודה** : כאשר מעתיקים את מבנה התפלגות העבודה מתבנית פרוייקט, אם הפרוייקט כולל לוח תאריכים של פרוייקט השונה מזה של התבנית, שעות העבודה מלוח התאריכים של הפרוייקט יחולו על לוח הזמנים של משימות. פעולה זו מתאימה את לוח הזמנים ללוח התאריכים של פרוייקט גיבוי. באופן דומה, המשימה הראשונה במבנה התפלגות העבודה מקבלת את תאריך ההתחלה של הפרוייקט, כך ששאר לוח הזמנים של הירארכיית המשימות מתעדכן בהתאם למשך הזמן וליחסי התלות שצוינו במבנה התפלגות עבודה של התבנית.  
  
 **העתקת הערכות פרוייקט** : בעת העתקה בשורות הערכה עבור פרוייקט, מחירונים מתעדכנים על בסיס יחידת הבעלות של הפרוייקט עבור מחירון העלות והלקוח עבור מחירון המכירות. עלות יחידה ומחירי מכירה נקבעים מתוך מחירונים אלה בפרוייקטים המשויכים ליישות מכירות.  
  
 **העתקת צוות הפרוייקט** : בעת העתקה של צוות הפרוייקט מהתבנית לפרוייקט, המשאבים הכלליים מועתקים, יחד עם הכישורים והמיומנויות שהוגדרו בתבנית. גם אופן הטיפול בהקצאות המשאבים הכלליים זהה לזה שבתבנית הפרוייקט.  
  
### <a name="see-also"></a>למידע נוסף  
 [מדריך למנהל פרוייקט](../psa/project-manager-guide.md)