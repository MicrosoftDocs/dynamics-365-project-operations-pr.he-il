---
title: תכנון העבודה ב- Microsoft Project עם התוספת Project Service
description: נושא זה מספק מידע על השימוש בתוספת Microsoft project עבור Microsoft Project Service.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 01/07/2021
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
ms.openlocfilehash: 87387ff870a7ef3ed0689f4ae38daad8cf220b46
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5145944"
---
# <a name="plan-your-work-in-microsoft-project-with-the-project-service-add-in"></a>תכנון העבודה ב- Microsoft Project עם התוספת Project Service

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3x](../includes/cc-applies-to-psa-app-3x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] מאפשר לך לבצע תכנון פרוייקט, כולל הערכות, בקלות רבה יותר. באפשרותך להגדיר את העבודה כך שעלויות, מאמץ וערך מכירות יהיו ברורים בעת הגשת ההצעה הסופית.  

באפשרותך להתקין את [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] ולבצע את עבודת התכנון בסביבה המוכרת של [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]. השתמש ביכולות החזקות של תכנון וניהול ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולאחר מכן עדכן את תוכנית הפרוייקט שלך ב- Project Service Automation.  

> [!IMPORTANT]
> - כדי להשתמש בתכונת ניהול המסמכים של SharePoint לצורך אחסון קובצי [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] עבור פרוייקטים של [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], מנהל המערכת של [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] יצטרך להפעיל את ניהול המסמכים. 
> - The [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] תואם רק ל- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.  

## <a name="download-and-install-the-add-in"></a>הורדה והתקנה של התוספת  
 הכן את פרטי הכניסה שלך ל- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. תזדקק למידע זה כדי להתחבר מתוך [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

1.  דרך 'מרכז ההורדות', באפשרותך להוריד את התוספת עבור הגירסה הנתמכת של Project Service, גירסה [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) או גירסה [V3.4+‎](https://www.microsoft.com/download/details.aspx?id=57956).  

2.  בחר את קישור ההורדה.  

3.  כאשר ההורדה תושלם, בחר **כן** כדי להתקין את התוספת.  

## <a name="configure-the-add-in"></a>קביעת תצורה של התוספת  

1. פתח את [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ובחר את הכרטיסיה **Project Service**.  

2. בחר **התחבר**.  

3. הזן את פרטי הכניסה שלך ולאחר מכן בחר **כניסה**.  

   כעת תוכל להתחיל להשתמש בתוספת.  

## <a name="read-from-a-template"></a>קריאה מתוך תבנית  
 קרא מתוך תבנית שיצרת ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] והעתקת לתוך [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] כדי להתחיל את תכנון הפרוייקט שלך. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [יצירת תבנית לפרוייקט (Project Service Automation)](../psa/create-project-template.md)  

1.  מתוך הכרטיסיה **Project Service**, בחר **קריאה** > **תבנית פרוייקט של Project Service Automation**.  

2.  בחר תבנית פרוייקט מהרשימה ולאחר מכן בחר **פתח**.  

    > [!NOTE]
    >  כברירת מחדל, משימות המועתקות מתוך התבנית לפרוייקט מוגדרות בתור מתוזמנות באופן ידני.  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a>הקצאת תפקידי [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] למשאבי פרוייקט  

1.  פתח פרוייקט ובחר את רצועת הכלים **משימה**.  

2. בחר את התפריט **תרשים גנט** ולאחר מכן בחר **גיליון משאבים**.  

3. בגיליון המשאבים, בחר את התפריט הנפתח **תפקיד של משאב Project Service** ובחר תפקיד של Project Service Automation.  

## <a name="staff-your-project-with-resources"></a>איוש הפרוייקט שלך במשאבים  

1.  מתוך הכרטיסיה Project Service, בחר שורה ובחר **חיפוש משאבים**.  

2.  במסך **‏‫הזמן משאב‬**, בחר את המשאב שברצונך להשתמש בו עבור הפרוייקט.  

3.  בחר באפשרות **הזמנה**, ולאחר מכן בחר באפשרות **אישור**.  

## <a name="publish-your-project"></a>פרסום הפרוייקט שלך  
לאחר השלמת תכנון הפרוייקט שלך, השלב הבא הוא לייבא ולפרסם את הפרוייקט ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

הפרוייקט יובא לתוך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. תהליכי תמחור והפקת צוות מוחלים. פתח את הפרוייקט ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] כדי לראות שהצוות, הערכות הפרוייקט ומבנה התפלגות העבודה נוצרו. הטבלה הבאה מראה היכן למצוא את התוצאות.


|              Microsoft Project                                                           |                      Project Service Automation                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **תרשים גנט**   | מייבא לתוך המסך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **מבנה התפלגות עבודה**. |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **גליון משאבים** |   מייבא לתוך המסך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **חברי צוות הפרוייקט**.   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **שימוש בנתוני שימוש**    |    מייבא לתוך המסך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **‏‫הערכות פרוייקט‬**.     |

**כדי לייבא ולפרסם את הפרוייקט שלך**  
1. בכרטיסיה **Project Service**, עבור אל **פרסום** > **פרוייקט חדש של Project Service Automation**.  

2. בתיבת הדו שיח **פרסם בפרוייקט חדש ב- Project Service**, הזן את **שם הפרוייקט** ובחר את **הלקוח**.  

3. אם תרצה, תוכל לבחור את האפשרות **‏‫קשר את תוכנית הפרוייקט ל- Project Service Automation‬** כדי לקשר את קובץ תוכנית הפרוייקט אל Project Service Automation‬.  

4. בחר **פרסם**.  

   קישור קובץ הפרוייקט אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] הופך את קובץ הפרוייקט לקובץ ראשי ומגדיר את מבנה התפלגות העבודה ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] לקריאה בלבד.  כדי לבצע שינויים בתוכנית הפרוייקט, עליך ליצור אותם ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולפרסם כעדכונים ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

## <a name="edit-a-project-thats-been-imported"></a>עריכת פרוייקט מיובא  
 כדי לבצע שינויים בתוכנית פרוייקט שיובאה לתוך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], עומדות בפניך שתי אפשרויות:  

- לפתוח את הקובץ הראשי ולערוך אותו ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

- לבטל את קישור הקובץ ולערוך אותו ישירות ב- Project Service. כברירת מחדל, פרוייקט שהועלה מתוך [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] נעול וניתן לערוך אותו רק ב- Project. כדי לערוך את הקובץ ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], יש לבטל את קישור הקובץ.  

### <a name="edit-in-pn_microsoft_project"></a>ערוך ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]  

1. בתפריט הראשי, עבור אל **Project Service** > **פרוייקטים**.  

2. מתוך רשימת הפרוייקטים, פתח את הפרוייקט שיצרת ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. בחר **פתח ב- MS Project** מרצועת הכלים. פעולה זו תפתח את הקובץ הראשי המקושר ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a>ביטול קישור הקובץ ועריכתו ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service  

1. בתפריט הראשי, עבור אל **Project Service** > **פרוייקטים**.  

2. מתוך רשימת הפרוייקטים, פתח את הפרוייקט שיצרת ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. בחר **‏‫בטל את הקישור ל- MS Project‬** מרצועת הכלים.  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a>העלאת קובץ פרוייקט ל- SharePoint או לקבוצות Office  
 באפשרותך להעלות את קובץ Project שלך אל SharePoint ולמצוא אותו תחת 'מסמכים משויכים' עבור פרוייקט [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] שלך.  מנהל המערכת שלך צריך להגדיר את ניהול המסמכים של SharePoint ולהפעיל אותו עבור הישות 'פרוייקט'. 

 באפשרותך גם להעלות את קובץ הפרוייקט שלך ל- [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] אם מוגדרות אצלך Office Groups.

### <a name="upload-a-file-for-sharepoint"></a>העלאת קובץ עבור SharePoint  

1. בתפריט הראשי, עבור אל **Project Service** > **העלה**.  

2. בחר **אל מסמכי פרוייקט של Project Service Automation**.  

3. בדו-שיח **אפשר פתיחה ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** בחר **כן** או **לא**.  

   - אם תבחר **כן** תוכל לבחור **פתח ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** ב- Project Service Automation ולהפעיל אל [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולטעון את קובץ הפרוייקט מתוך ספריית המסמכים של SharePoint.  

   - אם תבחר **לא**, הקישור עבור **פתח ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** לא יעבוד.  

4. ניתן למצוא את קובץ [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] תחת **מסמכים** עבור פרוייקט [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ספציפי.  

### <a name="upload-a-file-for-office-groups"></a>העלאת קובץ ל- Office Groups  

1. בתפריט הראשי, עבור אל **Project Service** > **העלה**.  

2. בחר **אל מסמכי פרוייקט של Project Service Automation**.  

3. בדו-שיח **אפשר פתיחה ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** בחר **כן** או **לא**.  

   - אם תבחר **כן** תוכל לבחור **פתח ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** ב- Project Service Automation ולהפעיל אל [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולטעון את קובץ הפרוייקט מתוך ספריית המסמכים של SharePoint.  

   - אם תבחר **לא**, הקישור עבור **פתח ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** לא יעבוד.  

4. ניתן למצוא את קובץ [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] תחת **מסמכים** עבור פרוייקט [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ספציפי.  

## <a name="publish--your-project-as-a-template"></a>פרסום הפרוייקט שלך כתבנית  
 באפשרותך לשמור את הפרוייקט שלך ולעשות בו שימוש חוזר על-ידי שמירתו כתבנית פרוייקט ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. תבניות פרוייקט הן תוכניות פרוייקט הניתנות לשימוש חוזר ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. למידע נוסף ראה [צור תבנית פרוייקט (Project Service Automation)](../psa/create-project-template.md). 

1. בכרטיסיה **Project Service**, עבור אל **פרסום** > **תבנית פרוייקט חדשה של Project Service Automation**.  

2. בתיבת הדו שיח **פרסם בפרוייקט חדש בתבנית Project Service**, הזן את **שם תבנית הפרוייקט**.  

3. אם תרצה, בחר את האפשרות **קשר את תוכנית הפרוייקט ל- Project Service Automation** כדי לקשר את קובץ הפרוייקט אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

4. בחר **פרסם**.  

קישור קובץ הפרוייקט אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] הופך את קובץ הפרוייקט לקובץ ראשי ומגדיר את מבנה התפלגות העבודה בתבנית [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] לקריאה בלבד.  כדי לבצע שינויים בתוכנית הפרוייקט, עליך ליצור אותם ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולפרסם כעדכונים ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].

## <a name="read-a-resource-loaded-schedule"></a>קרא לוח זמנים שטעון משאבים

בעת קריאת פרויקט מ- Project Service Automation, לוח השנה של המשאב אינו מסונכרן עם לקוח שולחן העבודה. אם יש הבדלים במשך המשימות, המאמץ או הסיום, זה כנראה בגלל שהמשאבים ולקוח שולחן העבודה אינם באותו לוח שנה של תבנית שעות עבודה על הפרויקט.


## <a name="data-synchronization"></a>‏‏סינכרון נתונים
הטבלאות בסעיף זה מספקות מידע על סנכרון נתוני ישויות בין Project Service Automation לבין התוספת השולחנית של Microsoft Project.

### <a name="project-task-entity-table"></a>טבלת ישויות משימות פרוייקט
הטבלה הבאה מתארת כיצד נתוני ישויות של משימות פרוייקט מסונכרנים בין Project Service Automation לבין התוספת לשולחן העבודה של Microsoft Project.

| **ישות** | **שדה** | **Microsoft Project ל- Project Service Automation** | **Project Service Automation ל- Microsoft Project** |
| --- | --- | --- | --- |
| משימת פרוייקט | תאריך יעד | Synchronized | ללא סנכרון |
| משימת פרוייקט | מאמץ מוערך | Synchronized | ללא סנכרון |
| משימת פרוייקט | מזהה לקוח MS Project | Synchronized | ללא סנכרון |
| משימת פרוייקט | משימת אב | Synchronized | ללא סנכרון |
| משימת פרוייקט | פרויקט | Synchronized | ללא סנכרון |
| משימת פרוייקט | משימת פרוייקט | Synchronized | ללא סנכרון |
| משימת פרוייקט | שם משימת פרוייקט | Synchronized | ללא סנכרון |
| משימת פרוייקט | יחידת הקצאת משאבים (הוצא משימוש בגירסה 3.0) | Synchronized | ללא סנכרון |
| משימת פרוייקט | משך מתוזמן | Synchronized | ללא סנכרון |
| משימת פרוייקט | תאריך התחלה | Synchronized | ללא סנכרון |
| משימת פרוייקט | מזהה WBS | Synchronized | ללא סנכרון |

### <a name="team-member-entity-table"></a>טבלת ישויות של חברי הצוות
הטבלה הבאה מתארת כיצד הנתונים של ישויות חברי הצוות מסונכרנים בין Project Service Automation לבין

| **ישות** | **שדה** | **Microsoft Project ל- Project Service Automation** | **Project Service Automation ל- Microsoft Project** |
| --- | --- | --- | --- |
| חבר צוות | מזהה לקוח MS Project | Synchronized | ללא סנכרון |
| חבר צוות | שם עמדה | Synchronized | ללא סנכרון |
| חבר צוות | פרוייקט | Synchronized | Synchronized |
| חבר צוות | צוות פרוייקט | Synchronized | Synchronized |
| חבר צוות | יחידת הקצאת משאבים | ללא סנכרון | Synchronized |
| חבר צוות | תפקיד | ללא סנכרון | Synchronized |
| חבר צוות | שעות עבודה | ללא סנכרון | ללא סנכרון |

### <a name="resource-assignment-entity-table"></a>טבלת ישויות הקצאות משאבים
הטבלה הבאה מתארת כיצד הנתונים של ישויות הקצאות משאבים מסונכרנים בין Project Service Automation לבין

| **ישות** | **שדה** | **Microsoft Project ל- Project Service Automation** | **Project Service Automation ל- Microsoft Project** |
| --- | --- | --- | --- |
| הקצאת משאבים | מתאריך | Synchronized | ללא סנכרון |
| הקצאת משאבים | שעות | Synchronized | ללא סנכרון |
| הקצאת משאבים | מזהה לקוח MS Project | Synchronized | ללא סנכרון |
| הקצאת משאבים | עבודה מתוכננת | Synchronized | ללא סנכרון |
| הקצאת משאבים | פרויקט | Synchronized | ללא סנכרון |
| הקצאת משאבים | צוות פרוייקט | Synchronized | ללא סנכרון |
| הקצאת משאבים | הקצאת משאבים | Synchronized | ללא סנכרון |
| הקצאת משאבים | משימה | Synchronized | ללא סנכרון |
| הקצאת משאבים | עד היום | Synchronized | ללא סנכרון |

### <a name="project-task-dependencies-entity-table"></a>טבלת ישויות תלות של משימות פרוייקט
הטבלה הבאה מתארת כיצד הנתונים של ישויות תלות של משימות פרוייקט מסונכרנים בין Project Service Automation לבין

| **ישות** | **שדה** | **Microsoft Project ל- Project Service Automation** | **Project Service Automation ל- Microsoft Project** |
| --- | --- | --- | --- |
| ‏‫יחסי תלות במשימת פרוייקט | ‏‫יחס תלות במשימת פרוייקט | Synchronized | ללא סנכרון |
| ‏‫יחסי תלות במשימת פרוייקט | סוג קישור | Synchronized | ללא סנכרון |
| ‏‫יחסי תלות במשימת פרוייקט | משימת ‏‏פעילות קדם | Synchronized | ללא סנכרון |
| ‏‫יחסי תלות במשימת פרוייקט | פרויקט | Synchronized | ללא סנכרון |
| ‏‫יחסי תלות במשימת פרוייקט | משימת ‏‏פעילות עוקבת | Synchronized | ללא סנכרון |

### <a name="additional-resources"></a>משאבים נוספים
 [מדריך למנהל פרויקט](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]