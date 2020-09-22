---
title: שימוש בתוספת של ‏‫Project Service לתכנון העבודה ב- Microsoft Project | MicrosoftDocs
description: נושא זה מספק מידע אודות אופן ההוספה, קביעת התצורה והשימוש בתוספת Microsoft project עבור Microsoft project Service.
author: ruhercul
manager: kfend
ms.service: Dynamics 365 Project Service Automation
ms.custom:
- dyn365-projectservice
ms.date: 04/06/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: efd589e0-8233-4abf-bf7e-5c1e83c4daea
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 0ad503ff0c27f1543d15b60714c2be46b8487d18
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751769"
---
# <a name="use-the-project-service-automation-add-in-to-plan-your-work-in-microsoft-project"></a>השתמש בתוספת של ‏‫Project Service Automation‬ כדי לתכנן את העבודה שלך ב- Microsoft Project

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] מאפשר לך לבצע תכנון פרוייקט, כולל הערכות, בקלות רבה יותר. באפשרותך להגדיר את העבודה כך שעלויות, מאמץ וערך מכירות יהיו ברורים בעת הגשת ההצעה הסופית.  

 כעת באפשרותך להתקין את [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] ולבצע את עבודת התכנון בסביבה המוכרת של [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]. השתמש ביכולות החזקות של תכנון וניהול ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולאחר מכן עדכן את תוכנית הפרוייקט שלך ב- Project Service Automation.  

> [!IMPORTANT]
> - כדי להשתמש בתכונת ניהול המסמכים של SharePoint לצורך אחסון קובצי [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] עבור פרוייקטים של [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], מנהל המערכת של [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] יצטרך להפעיל את ניהול המסמכים. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [הפעלת ניהול מסמכים של SharePoint עבור ישויות ספציפיות](../admin/enable-sharepoint-document-management-specific-entities.md)  
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
 קרא מתוך תבנית שיצרת ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] והעתקת לתוך [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] כדי להתחיל את תכנון הפרוייקט שלך. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [יצירת תבנית לפרוייקט (Project Service Automation)](../project-service/create-project-template.md)  

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
 באפשרותך להעלות את קובץ Project שלך אל SharePoint ולמצוא אותו תחת 'מסמכים משויכים' עבור פרוייקט [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] שלך.  מנהל המערכת שלך צריך להגדיר את ניהול המסמכים של SharePoint ולהפעיל אותו עבור הישות 'פרוייקט'. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [הגדרת שילוב של SharePoint](../admin/set-up-sharepoint-integration.md)  

 באפשרותך גם להעלות את קובץ הפרוייקט שלך ל- [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] אם מוגדרות אצלך Office Groups. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [שיתוף פעולה עם עמיתים באמצעות קבוצות Office 365 ](../basics/collaborate-with-colleagues-using-office-365-groups.md)  

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
 באפשרותך לשמור את הפרוייקט שלך ולעשות בו שימוש חוזר על-ידי שמירתו כתבנית פרוייקט ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  תבניות פרוייקט הן תוכניות פרוייקט הניתנות לשימוש חוזר ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [יצירת תבנית לפרוייקט (Project Service Automation)](../project-service/create-project-template.md)  

1. מתוך הכרטיסיה **Project Service**, לחץ על **פרסום** > **תבנית פרוייקט חדשה של Project Service Automation**.  

2. בתיבת הדו שיח **פרסם בפרוייקט חדש בתבנית Project Service**, הזן את **שם תבנית הפרוייקט**.  

3. אם תרצה, תוכל לבחור את האפשרות **קשר את תוכנית הפרוייקט ל- Project Service Automation** כדי לקשר את קובץ הפרוייקט אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].  

4. לחץ על **פרסם**.  

קישור קובץ הפרוייקט אל [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] הופך את קובץ הפרוייקט לקובץ ראשי ומגדיר את מבנה התפלגות העבודה בתבנית [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] לקריאה בלבד.  כדי לבצע שינויים בתוכנית הפרוייקט, עליך ליצור אותם ב- [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] ולפרסם כעדכונים ב- [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].

### <a name="see-also"></a>למידע נוסף  
 [מדריך למנהל פרוייקט](../project-service/project-manager-guide.md)
