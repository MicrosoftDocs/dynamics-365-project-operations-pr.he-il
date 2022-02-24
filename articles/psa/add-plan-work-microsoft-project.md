---
title: שימוש בתוספת של ‏‫Project Service לתכנון העבודה ב- Microsoft Project | MicrosoftDocs
description: נושא זה מספק מידע אודות אופן ההוספה, קביעת התצורה והשימוש בתוספת Microsoft project עבור Microsoft project Service.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 04/06/2019
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
ms.openlocfilehash: 9556feac5481e20bde1c9624c0eccc05385eaa94
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5145989"
---
# <a name="use-the-project-service-automation-add-in-to-plan-your-work-in-microsoft-project"></a>השתמש בתוספת של ‏‫Project Service Automation‬ כדי לתכנן את העבודה שלך ב- Microsoft Project

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] מאפשר לך לבצע תכנון פרוייקט, כולל הערכות, בקלות רבה יותר. באפשרותך להגדיר את העבודה כך שעלויות, מאמץ וערך מכירות יהיו ברורים בעת הגשת ההצעה הסופית.  

 כעת באפשרותך להתקין את [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] ולבצע את עבודת התכנון בסביבה המוכרת של [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]. השתמש ביכולות החזקות של תכנון וניהול ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולאחר מכן עדכן את תוכנית הפרוייקט שלך ב- Project Service Automation.  

> [!IMPORTANT]
> - כדי להשתמש בתכונת ניהול המסמכים של SharePoint לצורך אחסון קובצי [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] עבור פרוייקטים של [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], מנהל המערכת של [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] יצטרך להפעיל את ניהול המסמכים. 
> - The [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] תואם רק ל- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition.  

## <a name="download-and-install-the-add-in"></a>הורדה והתקנה של התוספת  
 הכן את פרטי הכניסה שלך ל- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. תזדקק למידע זה כדי להתחבר מתוך [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

1.  דרך 'מרכז ההורדות', באפשרותך להוריד את התוספת עבור הגירסה הנתמכת של Project Service, גירסה [V2.X](https://go.microsoft.com/fwlink/?linkid=828268) או גירסה [V3.4+‎](https://www.microsoft.com/download/details.aspx?id=57956).  

2.  לחץ על קישור ההורדה.  

3.  כאשר ההורדה תושלם, לחץ על **כן** כדי להתקין את התוספת.  

## <a name="configure-the-add-in"></a>קביעת תצורה של התוספת  

1. פתח את [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולחץ על הכרטיסיה **Project Service**.  

2. לחץ על **התחבר**.  

3. הזן את פרטי הכניסה שלך ולאחר מכן לחץ על **כניסה**.  

   כעת תוכל להתחיל להשתמש בתוספת.  

## <a name="read-from-a-template"></a>קריאה מתוך תבנית  
 קרא מתוך תבנית שיצרת ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] והעתקת לתוך [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] כדי להתחיל את תכנון הפרוייקט שלך. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [יצירת תבנית לפרוייקט (Project Service Automation)](../psa/create-project-template.md)  

1.  מתוך הכרטיסיה **Project Service**, לחץ על **קריאה** > **תבנית פרוייקט של Project Service Automation**.  

2.  בחר תבנית פרוייקט מהרשימה ולאחר מכן לחץ על **פתח**.  

    > [!NOTE]
    >  כברירת מחדל, משימות המועתקות מתוך התבנית לפרוייקט מוגדרות בתור מתוזמנות באופן ידני.  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a>הקצאת תפקידי [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] למשאבי פרוייקט  

1.  פתח פרוייקט ולחץ על רצועת הכלים **משימה**.  

2.  לחץ על התפריט **תרשים גנט** ולאחר מכן בחר **גיליון משאבים**.  

3.  בגיליון המשאבים, לחץ על התפריט הנפתח **תפקיד של משאב Project Service** ובחר תפקיד של Project Service Automation.  

## <a name="staff-your-project-with-resources"></a>איוש הפרוייקט שלך במשאבים  

1.  מתוך הכרטיסיה Project Service, בחר שורה ולחץ על **חיפוש משאבים**.  

2.  במסך **‏‫הזמן משאב‬**, בחר את המשאב שברצונך להשתמש בו עבור הפרוייקט.  

3.  לחץ על **הזמן** ולאחר מכן לחץ על **אישור**.  

## <a name="publish-your-project"></a>פרסום הפרוייקט שלך  
לאחר השלמת תכנון הפרוייקט שלך, השלב הבא הוא לייבא ולפרסם את הפרוייקט ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

הפרוייקט יובא לתוך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. תהליכי תמחור והפקת צוות מוחלים. פתח את הפרוייקט ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] כדי לראות שהצוות, הערכות הפרוייקט ומבנה התפלגות העבודה נוצרו. הטבלה הבאה מראה היכן למצוא את התוצאות:


|                                                                                          |                                                                                                                                   |
|------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **תרשים גנט**   | מייבא לתוך המסך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **מבנה התפלגות עבודה**. |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **גליון משאבים** |   מייבא לתוך המסך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **חברי צוות הפרוייקט**.   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **שימוש בנתוני שימוש**    |    מייבא לתוך המסך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **‏‫הערכות פרוייקט‬**.     |

**כדי לייבא ולפרסם את הפרוייקט שלך**  
1. מתוך הכרטיסיה **Project Service**, לחץ על **פרסום** > **פרוייקט חדש של Project Service Automation**.  

2. בתיבת הדו שיח **פרסם בפרוייקט חדש ב- Project Service**, הזן את **שם הפרוייקט** ובחר את **הלקוח**.  

3. אם תרצה, תוכל לבחור את האפשרות **‏‫קשר את תוכנית הפרוייקט ל- Project Service Automation‬** כדי לקשר את קובץ תוכנית הפרוייקט אל Project Service Automation‬.  

4. לחץ על **פרסם**.  

   קישור קובץ הפרוייקט אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] הופך את קובץ הפרוייקט לקובץ ראשי ומגדיר את מבנה התפלגות העבודה ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] לקריאה בלבד.  כדי לבצע שינויים בתוכנית הפרוייקט, עליך ליצור אותם ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולפרסם כעדכונים ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

## <a name="edit-a-project-thats-been-imported"></a>עריכת פרוייקט מיובא  
 כדי לבצע שינויים בתוכנית פרוייקט שיובאה לתוך [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], עומדות בפניך שתי אפשרויות:  

- לפתוח את הקובץ הראשי ולערוך אותו ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

- לבטל את קישור הקובץ ולערוך אותו ישירות ב- Project Service. כברירת מחדל, פרוייקט שהועלה מתוך [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] נעול וניתן לערוך אותו רק ב- Project. כדי לערוך את הקובץ ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], יש לבטל את קישור הקובץ.  

### <a name="edit-in-pn_microsoft_project"></a>לערוך ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]  

1. מתוך התפריט הראשי, לחץ על **Project Service** > **פרוייקטים**.  

2. מתוך רשימת הפרוייקטים, פתח את הפרוייקט שיצרת ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. לחץ על **פתח ב- MS Project** מרצועת הכלים. פעולה זו תפתח את הקובץ הראשי המקושר ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a>ביטול קישור הקובץ ועריכתו ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service  

1. מתוך התפריט הראשי, לחץ על **Project Service** > **פרוייקטים**.  

2. מתוך רשימת הפרוייקטים, פתח את הפרוייקט שיצרת ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)].  

3. לחץ על **‏‫בטל את הקישור ל- MS Project‬** מרצועת הכלים.  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a>העלאת קובץ פרוייקט ל- SharePoint או לקבוצות Office  
 באפשרותך להעלות את קובץ Project שלך אל SharePoint ולמצוא אותו תחת 'מסמכים משויכים' עבור פרוייקט [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] שלך.  מנהל המערכת שלך צריך להגדיר את ניהול המסמכים של SharePoint ולהפעיל אותו עבור הישות 'פרוייקט'. 

 באפשרותך גם להעלות את קובץ הפרוייקט שלך ל- [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] אם מוגדרות אצלך Office Groups.

### <a name="upload-a-file-for-sharepoint"></a>העלאת קובץ עבור SharePoint  

1. מתוך התפריט הראשי, לחץ על **Project Service** > **העלאה**.  

2. בחר **אל מסמכי פרוייקט של Project Service Automation**.  

3. בדו-שיח **אפשר פתיחה ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**, בחר **כן** או **לא**.  

   - אם תלחץ על **כן**, תוכל לבחור בלחצן **פתח ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** ב- Project Service Automation, להפעיל את [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולטעון את קובץ הפרוייקט מתוך ספריית המסמכים של SharePoint.  

   - אם תלחץ על **לא**, הקישור ללחצן **פתח ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** לא יעבוד.  

4. ניתן למצוא את קובץ [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] תחת **מסמכים** עבור פרוייקט [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ספציפי.  

### <a name="upload-a-file-for-office-groups"></a>העלאת קובץ ל- Office Groups  

1. מתוך התפריט הראשי, לחץ על **Project Service** > **העלאה**.  

2. בחר **אל מסמכי פרוייקט של Project Service Automation**.  

3. בדו-שיח **אפשר פתיחה ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]**, בחר **כן** או **לא**.  

   - אם תלחץ על **כן**, תוכל לבחור בלחצן **פתח ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** ב- Project Service Automation, להפעיל את [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולטעון את קובץ הפרוייקט מתוך ספריית המסמכים של SharePoint.  

   - אם תלחץ על **לא**, הקישור ללחצן **פתח ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** לא יעבוד.  

4. ניתן למצוא את קובץ [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] תחת **מסמכים** עבור פרוייקט [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ספציפי.  

## <a name="publish--your-project-as-a-template"></a>פרסום הפרוייקט שלך כתבנית  
 באפשרותך לשמור את הפרוייקט שלך ולעשות בו שימוש חוזר על-ידי שמירתו כתבנית פרוייקט ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  תבניות פרוייקט הן תוכניות פרוייקט הניתנות לשימוש חוזר ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [יצירת תבנית לפרוייקט (Project Service Automation)](../psa/create-project-template.md)  

1. מתוך הכרטיסיה **Project Service**, לחץ על **פרסום** > **תבנית פרוייקט חדשה של Project Service Automation**.  

2. בתיבת הדו שיח **פרסם בפרוייקט חדש בתבנית Project Service**, הזן את **שם תבנית הפרוייקט**.  

3. אם תרצה, תוכל לבחור את האפשרות **קשר את תוכנית הפרוייקט ל- Project Service Automation** כדי לקשר את קובץ הפרוייקט אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

4. לחץ על **פרסם**.  

קישור קובץ הפרוייקט אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] הופך את קובץ הפרוייקט לקובץ ראשי ומגדיר את מבנה התפלגות העבודה בתבנית [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] לקריאה בלבד.  כדי לבצע שינויים בתוכנית הפרוייקט, עליך ליצור אותם ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולפרסם כעדכונים ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].

## <a name="read-a-resource-loaded-schedule"></a>קרא לוח זמנים שטעון משאבים

בעת קריאת פרויקט מ- Project Service Automation, לוח השנה של המשאב אינו מסונכרן עם לקוח שולחן העבודה. אם יש הבדלים במשך המשימות, המאמץ או הסיום, זה כנראה בגלל שהמשאבים ולקוח שולחן העבודה אינם באותו לוח שנה של תבנית שעות עבודה על הפרויקט.


## <a name="data-synchronization"></a>‏סנכרון נתונים

הטבלה הבאה מתארת כיצד הנתונים מסונכרנים בין Project Service Automation לבין התוספת לשולחן העבודה של Microsoft Project.

| **ישות** | **שדה** | **Microsoft Project ל- Project Service Automation** | **Project Service Automation ל- Microsoft Project** |
| --- | --- | --- | --- |
| משימת פרויקט | תאריך יעד | ● | - |
| משימת פרויקט | מאמץ מוערך | ● | - |
| משימת פרויקט | מזהה לקוח MS Project | ● | - |
| משימת פרויקט | משימת אב | ● | - |
| משימת פרויקט | פרויקט | ● | - |
| משימת פרויקט | משימת פרוייקט | ● | - |
| משימת פרויקט | שם משימת פרוייקט | ● | - |
| משימת פרויקט | יחידת הקצאת משאבים (הוצא משימוש בגירסה 3.0) | ● | - |
| משימת פרויקט | משך מתוזמן | ● | - |
| משימת פרויקט | תאריך התחלה | ● | - |
| משימת פרויקט | מזהה WBS | ● | - |

| **ישות** | **שדה** | **Microsoft Project ל- Project Service Automation** | **Project Service Automation ל- Microsoft Project** |
| --- | --- | --- | --- |
| חבר צוות | מזהה לקוח MS Project | ● | - |
| חבר צוות | שם עמדה | ● | - |
| חבר צוות | פרויקט | ● | ● |
| חבר צוות | צוות פרוייקט | ● | ● |
| חבר צוות | יחידת הקצאת משאבים | - | ● |
| חבר צוות | תפקיד | - | ● |
| חבר צוות | שעות עבודה | לא מסונכרן | לא מסונכרן |

| **ישות** | **שדה** | **Microsoft Project ל- Project Service Automation** | **Project Service Automation ל- Microsoft Project** |
| --- | --- | --- | --- |
| הקצאת משאבים | מתאריך | ● | - |
| הקצאת משאבים | שעות | ● | - |
| הקצאת משאבים | מזהה לקוח MS Project | ● | - |
| הקצאת משאבים | עבודה מתוכננת | ● | - |
| הקצאת משאבים | פרויקט | ● | - |
| הקצאת משאבים | צוות פרוייקט | ● | - |
| הקצאת משאבים | הקצאת משאבים | ● | - |
| הקצאת משאבים | משימה | ● | - |
| הקצאת משאבים | עד היום | ● | - |

| **ישות** | **שדה** | **Microsoft Project ל- Project Service Automation** | **Project Service Automation ל- Microsoft Project** |
| --- | --- | --- | --- |
| ‏‫יחסי תלות במשימת פרוייקט | ‏‫יחס תלות במשימת פרוייקט | ● | - |
| ‏‫יחסי תלות במשימת פרוייקט | סוג קישור | ● | - |
| ‏‫יחסי תלות במשימת פרוייקט | משימת ‏‏פעילות קדם | ● | - |
| ‏‫יחסי תלות במשימת פרוייקט | פרויקט | ● | - |
| ‏‫יחסי תלות במשימת פרוייקט | משימת ‏‏פעילות עוקבת | ● | - |

### <a name="see-also"></a>למידע נוסף  
 [מדריך למנהל פרויקט](../psa/project-manager-guide.md)
