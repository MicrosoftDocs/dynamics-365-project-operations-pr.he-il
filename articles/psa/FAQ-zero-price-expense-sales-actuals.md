---
title: מדוע ברירת המחדל למחיר היא אפס עבור הוצאות המכירות בפועל?
description: שלוש הבדיקות הבאות יסייעו לך להבין מדוע ברירת המחדל למחיר היא 0 עבור הוצאות מכירות בפועל.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 5840bda4f74c720bfcdc7f4e84c8f22e0c6163ec
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077328"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-sales-actuals"></a>מדוע ברירת המחדל למחיר היא אפס עבור הוצאות המכירות בפועל?

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

שאלות נפוצות אלה דנות בנושא ההוצאות בפועל כאשר מחלקת התנועות מוגדרת כ'הוצאה' וסוג התנועה הוא '‏‫מכירות שלא חויבו‬'. שלוש הבדיקות הבאות יסייעו לך להבין מדוע ברירת המחדל למחיר (‏‫תעריף חיוב‬) היא 0 עבור הוצאות מכירות בפועל.

## <a name="check-1-identify-the-sales-price-list-for-project"></a>בדיקה 1: זיהוי מחירון מכירות עבור פרוייקט

חפש את הפרוייקט משדה הפרוייקט של השעות בפועל ועבור אל דף הפרוייקט. לאחר מכן עבור אל הכרטיסיה 'מכירות'. ברשת 'סעיפי חוזה של פרוייקט', לחץ על הקישור בשדה חוזה הפרוייקט. ייפתח דף חוזה הפרוייקט. בדף חוזה הפרוייקט, עבור אל הכרטיסיה 'מחירוני פרוייקט'. בדוק אם קיים לפחות מחירון אחד המצורף כאן.

אם לא מצורף מחירון ברשת 'מחירוני פרוייקט' של חוזה הפרוייקט, בצע את הפעולות הבאות:

- צרף מחירון לרשת 'מחירוני פרוייקט'. במחירונים שמותר לצרף כאן שדה ההקשר צריך להיות מוגדר בתור 'מכירות' ושדה המטבע במחירון אמור להתאים לשדה המטבע בחוזה הפרוייקט. לאחר שביצעת את כל התיקונים הנדרשים, צור מחדש ערך הוצאות, אשר אותו, ווודא שהנתונים בפועל של המכירות שלא חויבו מציגים מחיר חוקי.
- אם יש לך מחירון אחד או יותר שמצורפים לרשת 'מחירוני פרוייקט' של חוזה הפרוייקט, עבור לבדיקה 2.

## <a name="check-2-are-any-of-the-price-lists-identified-above-valid-for-the-specific-date-of-the-expense-actual"></a>בדיקה 2: האם מחירון כלשהו מבין המחירונים שזוהו לעיל תקפים עבור התאריך המסוים של הוצאות בפועל?

כדי ש- Project Service ישקול מחירון עבור מחיר ברירת מחדל, מחירון זה צריך להיות ישים עבור התאריך בהוצאות המכירות בפועל. בדוק את הפרטים הבאים כדי לראות אם המחירונים שתוארו לעיל ישימים:

- התחל על-ידי בדיקה אם תאריכי ההתחלה והסיום בכרטיסיה 'כללי' עבור המחירונים המצורפים אינם ריקים. אם תאריכי ההתחלה והסיום עבור המחירונים שתוארו לעיל ריקים, גילית את הבעיה. 
- רשום לעצמך את שדה תאריך ההתחלה בהוצאות המכירות בפועל שלך ובדוק אם מחירון כלשהו מבין המחירונים שזוהו ישים עבור תאריך זה. לדוגמה, תאריך ההוצאה בפועל אמור להימצא בטווח תאריך התחלה ותאריך הסיום במחירון. 
    - אם לא קיים מחירון המכסה תאריך זה בהוצאות מכירות בפועל, גילית את הבעיה. שנה את תאריכי ההתחלה והסיום של המחירון כדי להבטיח שהמחירון מכסה את תאריך ההוצאה בפועל. 
    - אם קיים יותר ממחירון אחד המכסה את תאריך הוצאות המכירות בפועל, גילית את הבעיה. באפשרותך לתקן זאת על-ידי עריכת תאריכי ההתחלה והסיום של המחירונים כך שיהיה מחירון אחד בלבד שמכסה את תאריך ההוצאה בפועל. 
    - אם ישנו מחירון אחד בלבד שמכסה את תאריך ההוצאה בפועל, עבור לבדיקה 3.
לאחר שביצעת את כל התיקונים הנדרשים, צור מחדש ערך הוצאות, אשר אותו, ווודא שהנתונים בפועל של המכירות שלא חויבו מציגים מחיר חוקי.

## <a name="check-3-is-there-a-valid-price-for-the-expense-category-in-the-applicable-project-price-list"></a>בדיקה 3: האם יש מחיר חוקי עבור קטגוריית ההוצאות במחירון הפרוייקט הישים? 

אם השלמת בהצלחה בדיקה 1 ובדיקה 2, כעת צריך להיות לך מחירון אחד בלבד של פרוייקט שישים עבור התאריך של הוצאות המכירות בפועל. פתח את מחירון פרוייקט זה ועבור אל הכרטיסיה 'מחירי קטגוריה'. ודא שקיימת שורה ברשת עבור קטגוריית ההוצאות הספציפית בהוצאה בפועל.
 
- אם אין שורה, גילית את הבעיה. צור שורה ברשת 'מחיר קטגוריה' עבור הקטגוריה בהוצאות בפועל שלך. לאחר שביצעת זאת, צור מחדש ערך הוצאות, אשר אותו, ווודא שהנתונים בפועל של המכירות שלא חויבו מציגים מחיר חוקי. 
- אם יש שורה עבור קטגוריית הוצאות ברשת 'מחירי קטגוריה', בדוק אם יש לה מחיר חוקי.

כדי להבין מה הוא מחיר חוקי, השתמש באחת מהשיטות הבאות:

- אם השדה 'שיטת תמחור' בשורת מחיר 'קטגוריה' מוגדר בתור 'לפי עלות', שיעור היחידה בהוצאות המכירות בפועל שלך הופך כברירת מחדל לערך בהוצאה.
- אם השדה 'שיטת תמחור' בשורת המחיר 'קטגוריה' מוגדר בתור 'אחוזי ייקור', בדוק אם שדה האחוז מוגדר לערך חוקי. שיעור היחידה בהוצאות המכירות בפועל שלך מוגדר כברירת מחדל על-ידי החלת אחוז ייקור זה על המחיר בערך ההוצאה.
- אם השדה 'שיטת תמחור' בשורת המחיר 'קטגוריה' מוגדר בתור '‏‫מחיר ליחידה‬', בדוק אם שדה המחיר מוגדר לערך חוקי. שיעור היחידה בהוצאות המכירות בפועל שלך יוגדר כברירת מחדל כסכום המטבע שצוין בשדה המחיר.

אם הגדרת המחיר עבור קטגוריית ההוצאות אינה חוקית, גילית את הבעיה. הפתרון הוא לעדכן את שורת מחיר הקטגוריה במחיר חוקי עבור קטגוריית ההוצאות בהתאם לכללים לעיל. לאחר שביצעת זאת, צור מחדש ערך הוצאות, אשר אותו, ואז בדוק שהנתונים בפועל של המכירות שלא חויבו מציגים מחיר חוקי.

אם עדיין אינך רואה מחיר חוקי בהוצאות המכירות בפועל שלך לאחר ביצוע שלוש הבדיקות לעיל, צור כרטיס תמיכה.

