---
title: מבט כולל על מעקב אחר פרוייקט
description: נושא זו מספק מידע כיצד ניתן לעקוב אחר התקדמות הפרוייקט וצריכת העלות.
author: ruhercul
manager: AnnBe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: c998addbbdbbea8fe69c95f65e58a24146f394c8
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/01/2020
ms.locfileid: "3907364"
---
# <a name="project-tracking-overview"></a>מבט כולל על מעקב אחר פרוייקט

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

הצורך לעקוב אחר ההתקדמות מול לוח זמנים משתנה לפי ענף. תעשיות מסוימות עוקבות ברמה מפורטת, ואילו תעשיות אחרות עוקבות ברמה גבוהה יותר. נושא זה מראה כיצד ליצור לוח זמנים שיעמוד בדרישות הארגון שלך.

## <a name="effort-tracking-view"></a>תצוגה של מעקב אחר המאמץ

התצוגה **מעקב אחר מאמץ** עוקבת אחר התקדמות המשימות בלוח הזמנים על-ידי השוואת שעות המאמץ בפועל שהושקעו במשימה לשעות המאמץ המתוכננות של המשימה. Dynamics 365 Project Operations משתמש בנוסחאות הבאות כדי לחשב את מדדי המעקב:

- **אחוזי התקדמות**: מאמץ בפועל שנעשה עד היום ÷ הערכה בעת סיום (EAC) 
- **הערכה לסיום (ETC)**: מאמץ מתוכנן – מאמץ בפועל שהושקע עד היום 
- **EAC**: מאמץ שנותר + מאמץ בפועל שהושקע עד היום 
- **סטיית מאמץ חזוי**: מאמץ מתוכנן – EAC

Project Operations מציג תחזית לסטיית המאמץ במשימה. אם ה- EAC הוא יותר מהמאמץ המתוכנן, המשימה מתוכננת להימשך זמן רב יותר ממה שתוכנן במקור והיא בפיגור אל מול לוח הזמנים. אם ה- EAC הוא פחות מהמאמץ המתוכנן, המשימה מתוכננת להימשך זמן קצר יותר ממה שתוכנן במקור והיא מקדימה את לוח הזמנים.

## <a name="reprojecting-effort"></a>חיזוי מחדש למאמץ

מנהלי פרויקטים משנים לעיתים קרובות את ההערכות המקוריות במשימה. חיזויים מחדש של פרויקט הם תפיסות של מנהל הפרויקט להערכות, בהינתן המצב הנוכחי של הפרויקט. עם זאת, איננו ממליצים למנהלי פרויקטים לשנות את המספרים הבסיסיים. זאת מכיוון שבסיס הפרויקט מייצג את מקור האמת המבוסס של הערכת העלות ולוח הזמנים של הפרויקט, וכל בעלי העניין של הפרויקט הסכימו עליו.

קיימות שתי דרכים שבהן מנהל פרויקט יכול לבצע חיזוי מחדש של מאמץ במשימות:

- עקוף את ה- ETC שבברירת מחדל בעזרת הערכה חדשה של המאמץ בפועל שנותר במשימה. 
- עקוף את אחוז ההתקדמות שבברירת מחדל בעזרת הערכה חדשה של ההתקדמות האמיתית במשימה.

כל גישה גורמת לחישוב מחדש של ה- ETC, ה- ‏EAC, אחוז ההתקדמות במשימה ושל סטיית המאמץ החזוי במשימה. ה- EAC, ה- ‏ETC ואחוז ההתקדמות בפעילויות הערסל מחושבים גם כן, ומפיקים חיזוי חדש לסטיית המאמץ.

## <a name="reprojection-of-effort-on-summary-tasks"></a>חיזוי מחדש של מאמץ בפעילויות ערסל

ניתן ליצור חיזוי מחדש למאמץ בפעילויות ערבול או במשימות של גורמים מכילים. בין אם המשתמש מבצע חיזוי מחדש באמצעות המאמץ שנותר או אחוז ההתקדמות בפעילויות ערסל, קבוצת החישובים הבאה מתחילה:

- מתבצע חישוב ל- EAC,‏‏ ל- ETC ולאחוז ההתקדמות במשימה.
- ה- EAC החדש מופץ לפעילויות הצאצא ביחס זהה לזה שהיה ב- EAC המקורי בפעילות.
- ה- EAC החדש מחושב בכל אחת מהפעילויות הבודדות עד לפעילויות של צומת העלה. 
- החישוב מחדש של ETC ואחוז התקדמות בפעילויות הצאצא המושפעות עד לצמתי העלה מתבסס על ערך ה- EAC. התוצאה היא חיזוי חדש עבור סטיית המאמץ של הפעילות. 
- מתבצע חישוב מחדש להערכות ה- EAC של פעילויות הערסל ועד לצומת הבסיס.

### <a name="cost-tracking-view"></a>תצוגת מעקב עלות 

התצוגה **מעקב עלות** משווה בין העלות בפועל שהושקעה לעלות המתוכננת במשימה. 

> [!NOTE]
> תצוגה זו מציגה רק עלויות עבודה ואינה כוללת עלויות מהערכת ההוצאות. Project Operations משתמש בנוסחאות הבאות כדי לחשב את מדדי המעקב:

- **אחוז העלות הנצרכת**: עלות בפועל שהושקעה עד היום ÷ אומדן עלות בעת השלמת המשימה
- **עלות לסיום (CTC)**: עלות מתוכננת – עלות בפועל שהושקעה עד היום
- **EAC**: עלות נותרת + סכום עלות בפועל עד היום
- **סטיית עלות חזויה**: עלות מתוכננת – EAC

תחזית לסטיית העלות מוצגת במשימה. אם ה- EAC הוא יותר מהעלות המתוכננת, המשימה מתוכננת לעלות יותר ממה שתוכנן במקור. לכן היא חורגת מהתקציב. אם ה- EAC הוא פחות מהעלות המתוכננת, המשימה מתוכננת לעלות פחות ממה שתוכנן במקור. לכן היא מתחת לתקציב.

## <a name="project-managers-reprojection-of-cost"></a>חיזוי עלות מחדש של מנהל הפרויקט

כאשר מבצעים חיזוי מחדש למאמץ, ה- CTC,‏ EAC, אחוז העלות שנצרכה וסטיית העלות החזויה מחושבים מחדש בתצוגה **מעקב עלות**.

## <a name="project-status-summary"></a>סיכום מצב פרוייקט

מעקב אחר נתונים בתצוגה **מעקב מאמץ** ובתצוגה **מעקב עלות** מראה את ההתקדמות ואת צריכת העלות בצומת הבסיס של הפרוייקט, פעילויות ערסל ורמות של משימות צומת עלה. המקטע **מצב** בדף **ישות פרוייקט** מציג סיכום של מצב רמת הפרוייקט.

## <a name="status-summary-fields"></a>שדות סיכום מצב

השדה **מצב פרוייקט כולל‬** הוא שדה שניתן לערוך אותו ושמציג את המצב הכולל של הפרוייקט. הוא משתמש בקידוד צבעים, כגון ירוק, צהוב ואדום, כדי לציין סיכון שמתגבר. השדה **הערות** מאפשר למנהל הפרוייקט להזין הערות ספציפיות לגבי המצב. לא ניתן לערוך את השדה **‏‫המצב עודכן בתאריך** והערך הוא חותמת זמן שמציינת מתי המצב עודכן לאחרונה.

השדה **‏‫ביצועי לוח זמנים‬** והשדה **‏‫ביצועי עלות‬** נקבעים מתאריך המעקב. כאשר לוח הזמנים וסטיית העלות עבור צומת הבסיס בתצוגה **מעקב מאמץ** חיוביים, תוכל להגדיר שדות אלו בתור **הקדמה‬**. כאשר לוח הזמנים וסטיית העלות עבור צומת הבסיס שליליים, תוכל להגדיר אותם בתור **עיכוב**.
