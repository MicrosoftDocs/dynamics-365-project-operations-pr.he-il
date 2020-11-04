---
title: ‏‫קביעת לוח זמנים למשאבי פרויקט
description: כיצד לקבוע לוח זמנים למשאבי פרויקט ב- Project Service
author: JohnPBurrows
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
ms.openlocfilehash: db69348aac96cbfaaa865228c9230cbda4b1e784
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077514"
---
# <a name="schedule-resources-for-a-project-project-service"></a>קביעת לוח זמנים למשאבי פרויקט (Project Service)

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

באפשרותך לבדוק זמינות משאבים כדי לקבל תצוגה כוללת על האופן שבו הוזמנו המשאבים שלך, או באפשרותך לסנן את התצוגה לפי כישורים, צוות, מיקום ואפשרויות אחרות.  
  
לוח הזמנים מציג רשימה של משאבים עם הזמינות שלהם. בחר מצב תצוגה כדי להציג את הזמינות שלך לפי **שעות** , **יום** , **שבוע** , או **חודש**.  
  
 קביעת תצורה של לוח הזמנים (Field Service or Project Service Automation) למידע נוסף, ראה [קביעת תצורה ללוח הזמנים (Field Service או Project Service Automation)](https://docs.microsoft.com/dynamics365/field-service/configure-schedule-board).
  
אם אתה משתמש בגרסה ישנה יותר, כדי לצפות בזמינות המשאבים היכנס ל[הצגת זמינות משאבים](../psa/view-resource-availability.md).  

> [!IMPORTANT]
>  כדי להשתמש בפונקציונליות של הזמנת לוח זמנים, קודים גיאוגרפיים‬ ושירותי מיקום, תצטרך להפעיל את המפות.  
> 
> 1. מתוך התפריט הראשי בחר **תזמון משאבים** > **ניהול**.  
> 2. לחץ על **פרמטרים של תזמון**.  
> 3. פתח את הרשומה וגלול למטה למקטע **Resource Scheduling Optimization**.  
> 4. בשדה **התחבר למפות** , בחר **כן**.  
> 5. קבל את התנאים ושמור את הרשומה.  
> 6. מתוך התפריט הראשי בחר **Project Service** > **לוח זמנים**. מכאן, קיימות כמה דרכים לתזמון ידני של דרישת הזמנה. בחר את השיטה המתאימה עבורך.
  
## <a name="find-available-resources"></a>מציאת משאבים זמינים‬

1.  מתוך הרשימה **דרישת ההזמנה** , לחץ לחיצה ימנית על הזמנת משאב מתוכננת ובחר אחת מהאפשרויות הבאות:  
  
- בחר **חיפוש זמינות - משאבים נוכחיים** כדי לאתר משאב זמין מתוך הרשימה בלוח הזמנים.  
- בחר **חיפוש זמינות - כל המשאבים** , כדי לאתר משאבים זמינים ממשאבי המערכת  
   > [!NOTE]
   >  לאחר שתבצע זאת, המסננים יציגו אפשרויות עבור דרישת ההזמנה שנבחרה.  
  
2. כאשר תראה משבצת זמינה, לחץ קליק-ימני על משבצת הזמן בלוח הזמנים ובחר **הזמן כאן**. לחלופין, גרור ושחרר את דרישת ההזמנה למשבצת הזמן.  
  

## <a name="book-a-resource-using-the-daily-view-and-find-whos-under-booked"></a>הזמנת משאב באמצעות תצוגה יומית וזיהוי האנשים שלא הוזמנו
  
1.  בלוח הזמנים, לחץ על **מצב תצוגה** ובחר **ימים**.  
  
    תופיע תצוגת רשת של מספר השעות שבהן משאב מוזמן בכל יום ובאילו ימים הוא פנוי.  
  
2.  לחץ על שם המשאב שברצונך להזמין ולאחר מכן לחץ על **הזמן**.  
  
3.  בתיבת הדו-שיח **הזמנת משאבים (יצירה)** , בחר את הפרויקט שעבורו ברצונך להזמין את המשאב, כמו גם את שיטת הזמנת המשאב ומועדי ההתחלה והסיום.  
  
4.  לאחר שסיימת, בחר **הזמן**.  
  
## <a name="view-to-the-schedule-board"></a>הצגת לוח הזמנים
  
1.  בחר דרישת הזמנה לא מתוזמנת‬ מתוך הרשימה למטה.  
  
2.  גרור את דרישת ההזמנה למשבצת זמן/משאב זמינים בלוח הזמנים.  
  
3.  לאחר שסיימת, בחר **הזמן**.  
  
### <a name="additional-resources"></a>משאבים נוספים  
 [מדריך למנהל משאבים](../psa/resource-manager-guide.md)
