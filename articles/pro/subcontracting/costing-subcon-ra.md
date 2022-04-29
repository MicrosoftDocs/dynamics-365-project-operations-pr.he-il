---
title: הערכת עלויות של הקצאות משאבים בקבלנות משנה
description: נושא זה מסביר כיצד Dynamics 365 Project Operations‏ Microsoft מחשבת הערכת עלות של הקצאות משאבים בקבלנות משנה.
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: tonyafehr
ms.author: rumant
ms.openlocfilehash: 09a2a86ea0e97376939d5bff6df9177747818ebb
ms.sourcegitcommit: 04dc8d952e6da3ab3eb2a20131c6f7cee6040876
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 12/10/2021
ms.locfileid: "7903438"
---
# <a name="cost-estimation-of-subcontracted-resource-assignments"></a>הערכת עלויות של הקצאות משאבים בקבלנות משנה

[!include [banner](../../includes/dataverse-preview.md)]

_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_

תמחיר הקצאות משימות של חברי צוות פרויקט בקבלנות משנה מתבצעת באמצעות המחירון **רכישה** המצורף לחוזה המשנה ברשומת חבר הצוות הקשור. זה שונה מהאופן שבו מתבצע תמחיר הקצאות משאבי עובדים כאשר תמחיר הקצאות משימות של משאבי עובדים מתבצעת באמצעות המחירון **עלות** המצורף ליחידה הקבלנית של הפרויקט. 

התמחיר עבור חברי צוות פרויקט כלליים בקבלנות משנה מתבצעת באמצעות הגדרת מחיר מבוסס תפקיד במחירון 'רכישה' המצורף לחוזה המשנה. ניתן גם להגדיר מחירי רכישה ספציפית עבור כל משאב. מחירים ספציפיים למשאבים אלה יקבלו עדיפות בעת חישוב תמחיר של הקצאת משימות של חברי צוות פרויקט בעלי שם שהם קבלני משנה. 

עדיפות השימוש במחיר רכישה ספציפי לתפקיד לעומת ספציפי למשאב מונעת על ידי הגדרת עדיפות ממד התמחור ב **פרמטרים > ממדי תמחור מבוססי כמות**.

פונקציונליות זו של הפקת מחירים דינמית על סמך הגדרת ממד עבור מחירי רכישה של קבלני משנה דומה לאופן שבו נגזרים תעריפי עלויות וחשבונות עבור עובדים במשרה מלאה. 

## <a name="creating-task-assignments-for-getting-cost-estimates-of-subcontractor-resources"></a>יצירת הקצאות משימות לקבלת הערכות של עלויות של משאבי קבלן משנה

ניתן ליצור הקצאות משימות עבור קבלני משנה בשתי דרכים: 
- באמצאות הכרטיסיה **משימות**.
- באמצאות הכרטיסיה **צוות**.

### <a name="creating-resources-assignments-using-the-tasks-tab"></a>יצירת הקצאות משאבים באמצעות הכרטיסייה 'משימות'
באמצעות שימוש ברשימה **משאבים** בכרטיסיה **משימות** עבור משימה ספציפית, אפשר ליצור הקצאת משימה עבור משאב בעל שם או משאב כללי. אם תבחר משאב בעל שם מתוך הרשימה הנפתחת **משאבים שהוקצו** במשימה, והמשאב הזה הוא קבלן משנה, המשאב בעל השם מוקצה למשימה ונוצרת רשומת חבר צוות פרויקט תואמת שבה סוג העובד בה מוגדר **קבלן משנה** וה **תוקף** מוגדר כ **לא חוקי**. כשלב הבא, יהיה עליך לפתוח את רשומת חבר צוות הפרויקט ולבחור חוזה משנה וסעיף חוזה משנה. פעולה זו תעדכן את הקצאת המשימה כך שתהיה לה הפניה לחוזה המשנה ולסעיף בחוזה המשנה וכן תעדכן את מצב חבר הצוות ל **בתוקף**.

אם תבחר ליצור חבר צוות כללי מהרשימה הנפתחת **משאבים שהוקצו** במשימה, תיבת הדו-שיח **יצירת חבר צוות כללי** תאפשר לך לבחור חוזה משנה וסעיף בחוזה המשנה. כאשר המשאב כללי מוקצה למשימה ורשומת חבר צוות הפרויקט המתאימה נוצרת, תבחין שרשומת חבר צוות הפרויקט נוצרת עם סוג עובד שמוגדר כ **קבלן משנה** ו **תוקף** מוגדר כ **תקף**.

### <a name="creating-project-team-members-using-the-team-tab"></a>יצירת חברי צוות פרויקט באמצעות הכרטיסייה 'צוות'
באמצעות הכרטיסייה 'צוות' בפרויקט, אפשר ליצור חבר צוות כללי או בעל שם. בעת יצירת חבר הצוות, ניתן לבחור בחוזה המשנה ובסעיף חוזה המשנה. לאחר יצירת חבר הצוות, תצטרך להקצות את חבר הצוות למשימה באמצעות הרשימה הנפתחת **משאבים שהוקצו** במשימה. 

## <a name="updating-estimates"></a>עדכון אומדנים
לאחר שהקצית את חברי צוות הפרויקט למשימות, תצטרך לנווט אל הכרטיסיה **הערכות** בפרויקט ולבחור באפשרות **עדכן מחירים** כדי להבטיח ששיעורי העלויות של הקצאות משאבי קבלני משנה יעודכנו בהתבסס על מחירון הרכישה המצורף לחוזה המשנה. הערכות לא נוצרות עבור משימות שלא הוקצו ב- Dynamics 365 Project Operations Microsoft. כתוצאה מכך, תצטרך ליצור הקצאות משימות לתמחור ולביצוע תמחיר של משימות שונות בפרויקט שלך. 

> [הערה!] חברי צוות הפרויקט ש **סוג העובד** שלהם מוגדר כ **קבלן משנה**, אך אין להם הפניה של חוזה משנה מסומנים כ **לא חוקי** ברשת **חברי צוות הפרויקט**. אם ישנם חברי צוות פרויקט עם סטטוס זה, פתח את רשומת חבר צוות הפרויקט באופן ידני ועדכן ידנית את השדות 'חוזה משנה' ו'סעיף חוזה המשנה' כך שאומדן העלות הפיננסית משקף במדויק את עלות קבלן המשנה בכרטיסיה **הערכות**. 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]