---
title: אפשרויות קבלנות משנה לחברי צוות הפרויקט
description: נושא זה מסביר את אפשרויות קבלנות המשנה עבור חברי צוות הפרויקט ב- Dynamics 365 Project Operations‏ Microsoft.
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: tonyafehr
ms.author: rumant
ms.openlocfilehash: 4db283db728b50ccf76eafabfd643313620bbce2
ms.sourcegitcommit: 04dc8d952e6da3ab3eb2a20131c6f7cee6040876
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 12/10/2021
ms.locfileid: "7903445"
---
# <a name="subcontracting-options-for-project-team-members"></a>אפשרויות קבלנות משנה לחברי צוות הפרויקט

[!include [banner](../../includes/dataverse-preview.md)]

_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_

ב- Dynamics 365 Project Operations‏ Microsoft, תוכל להעריך את אפשרויות קבלנות המשנה הזמינות עבור חבר אחד או יותר בצוות הפרויקט. אפשרויות קבלנות המשנה הזמינות מאפשרות לך:

- ליצור חוזה משנה חדש ו/או ליצור שורות חדשות בחוזה משנה קיים עבור חברי צוות הפרויקט שנבחרו. 
- לשריין כנגד חוזה משנה וסעיף חוזה משנה קיימים. 

ניתן לבחור מבין אפשרויות קבלנות המשנה הזמינות עבור חברי צוות פרויקט כלליים או לבחור מבין חברי צוות פרויקט שאוישו במשאב בעל שם שהוא קבלן משנה. 

אין אפשרויות קבלנות משנה זמינות עבור המקרים הבאים:

- חברי צוות פרויקט אשר אוישו בעובד. 
- חברי צוות פרוייקט שכבר משוייכים לחוזה משנה ולסעיף בחוזה משנה. 

## <a name="subcontracting-an-unstaffed-project-team-member"></a>קבלנות משנה לחבר צוות הפרויקט שלא אויש

כדי לסקור ולבחור מבין אפשרויות קבלנות המשנה הזמינות עבור חבר צוות פרויקט כללי או לא מאויש, בצע את השלבים הבאים:

1. בחר רשומה אחת או יותר של חבר צוות פרויקט שבהן המשאב הוא משאב כללי.
2. ודא שאף אחת מהרשומות של חברי צוות הפרויקט שנבחרו אינה נמצאת כבר בקבלנות משנה. 
3. בחר **אפשרויות קבלנות משנה** ברשת המשנה של חברי צוות הפרויקט. נפתחת תיבת הדו-שיח **אפשרויות קבלונת משנה**. 
4. אם בחרת רק רשומת חבר צוות פרויקט אחד בשלב 1, האפשרויות הבאות יהיו זמינות:
    - יצירת סעיפים חדשים של חוזה משנה. 
    - האפשרות היחידה הזמינה לשריון כנגד חוזה משנה קיים אם בחרת במספר רשומות של חברי צוות פרויקט בשלב 1, היא יצירת סעיפים חדשים של חוזה משנה.
5. האפשרות לשריין כנגד סעיף קיים בחוזה משנה מאפשרת לבחור חוזה משנה סעיף חוזה משנה שכנגדו ברצונך לשריין. בעת בחירת סעיף חוזה משנה לשריון קיבולת, עליך לוודא שסעיף חוזה המשנה שנבחר הוא לזמן ושהתפקיד הנדרש בחבר צוות הפרויקט תואם לתפקיד שנרכש בסעיף חוזה המשנה.
6. כשבוחרים ליצור סעיפי חוזה משנה חדשים עבור חברי צוות הפרויקט, המערכת מאפשרת לבחור את חוזה המשנה הרצוי ליצירת סעיפים אלו. חוזה המשנה שבחרת ליצור בו סעיפים חדשים צריך להיות במצב **טיוטה**. עם אפשרות זו ליצירת סעיפי חוזה משנה חדשים עבור חברי צוות הפרויקט שנבחרו, המערכת תיצור סעיף חוזה משנה אחת עבור זמן עבור כל חבר צוות פרויקט. התפקיד, השעות והתאריכים יועתקו מחבר צוות הפרויקט לכל סעיף חוזה משנה שיווצר. 
7. כאשר חבר צוות כללי משויך לחוזה משנה ולסעיף חוזה משנה, השדה **סוג עובד** בשורת חבר הצוות כללי יעודכן ל **קבלן משנה** והערך של **תוקף חוזה משנה** יוגדר ל **חוקי**.

## <a name="subcontracting-a-staffed-project-team-member"></a>קבלנות משנה לחבר צוות הפרויקט שאויש

כמו חברי צוות כלליים או לא מאוישים, ניתן גם להציג אפשרויות קבלנות משנה עבור חבר צוות פרויקט מאויש כל עוד חבר הצוות המאויש הוא קבלן משנה. כדי לסקור ולבחור מבין אפשרויות קבלנות המשנה הזמינות עבור חבר צוות פרויקט מאויש או בעל שם, בצע את השלבים הבאים:

1. בחר רשומה אחת או יותר של חבר צוות פרויקט שבהן המשאב הוא קבלן משנה בעל שם.
2. ודא שאף אחת מהרשומות של חברי צוות הפרויקט שנבחרו אינה נמצאת כבר בקבלנות משנה. 
3. בחר **אפשרויות קבלנות משנה** ברשת המשנה של חברי צוות הפרויקט. נפתחת תיבת הדו-שיח **אפשרויות קבלונת משנה**. 
4. אם בחרת רק רשומת חבר צוות פרויקט אחד בשלב 1, האפשרויות הבאות יהיו זמינות:
      - יצירת סעיפים חדשים של חוזה משנה.
      - שריין כנגד חוזה משנה קיים.
  אם בחרת במספר רשומות של חברי צוות פרויקט בשלב 1, האפשרות היחידה הזמינה היא יצירת סעיפים חדשים של חוזה משנה.
5. האפשרות לשריין כנגד סעיף קיים בחוזה משנה מאפשרת לבחור חוזה משנה סעיף חוזה משנה שכנגדו ברצונך לשריין. בעת בחירת סעיף חוזה משנה כדי לשריין קיבולת, עליך לוודא את הדברים הבאים:
      - סעיף חוזה המשנה שנבחר הוא לזמן. 
      - התפקיד הנדרש בחבר צוות הפרויקט תואם את התפקיד שנרכש בסעיף חוזה המשנה. 
      - הספק שאליו משויך קבלן המשנה זהה לספק בחוזה המשנה.
6. כשבוחרים ליצור סעיפי חוזה משנה חדשים עבור חברי צוות הפרויקט, המערכת מאפשרת לבחור את חוזה המשנה הרצוי ליצירת סעיפים אלו. באפשרות זו, עליך לוודא שהספק שאליו שייך קבלן המשנה זהה לספק בחוזה המשנה. 
7. חוזה המשנה שבחרת ליצור בו סעיפים חדשים צריך להיות במצב **טיוטה**. עם אפשרות זו ליצירת סעיפי חוזה משנה חדשים עבור חברי צוות הפרויקט שנבחרו, המערכת תיצור סעיף חוזה משנה אחת עבור זמן עבור כל חבר צוות פרויקט. התפקיד, השעות והתאריכים יועתקו מחבר צוות הפרויקט לכל סעיף חוזה משנה שיווצר.  
8. כאשר חבר צוות בעל שם משויך לחוזה משנה ולסעיף חוזה משנה, השדה **סוג עובד** בשורת חבר הצוות בעל השם יעודכן ל **קבלן משנה** והערך של **תוקף חוזה משנה** יוגדר ל **חוקי**.

## <a name="re-costing-subcontractor-assignments"></a>חישוב מחדש של תמחיר משימות קבלן המשנה

כאשר חבר צוות פרויקט (כללי או בעל שם) מקושר לסעיפי חוזה משנה באמצעות תיבת הדו-שיח **אפשרויות קבלנות משנה**, התמחיר של כל ההקצאות למשימות שיש לחבר הצוות יחושב מחדש על סמך מחירון הרכישה המצורף לחוזה המשנה. בכרטיסיה **הערכות** בדף **פרטי הפרויקט**, בחר את הלחצן **עדכן מחירים** כדי לראות תמחור ו/או תמחיר מעודכנים הנובעים מההחלטה על הוצאת העבודה לקבלן משנה.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]