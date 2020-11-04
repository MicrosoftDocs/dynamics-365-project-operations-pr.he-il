---
title: החזר מע"מ
description: נושא זה מסביר כיצד ניתן לקבל החזרים בגין עסקאות הכוללות מס ערך מוסף (מע"מ).
author: saraschi2
manager: AnnBe
ms.date: 02/26/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvPerDiems
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: d1be96521cdb486dd5a702cded615d3e1015b364
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077350"
---
# <a name="vat-recovery"></a>החזר מע"מ 

[!include [banner](../includes/banner.md)]

כדי לקבל החזרים כספיים בגין עסקאות זכאיות למס ערך מוסף (מע"מ), על החברה או הארגון לזהות, לאסוף, לאמת ולהגיש מידע מדויק. תהליך זה כולל מספר משימות, ובהתאם לגודל החברה, עשוי לכלול מספר עובדים או תפקידים.

כדי לקבל החזרי מע"מ באמצעות ניהול הוצאות, יש להשלים את ה‏‫דרישות המוקדמות הבאות:

- יש ליצור קודי מס עבור מדינות/אזורים בעלי הקצאות לקטגוריות של הוצאות.
- יש ליצור קבוצת מע"מ עבור כל קוד מס.
- יש ליצור קוד מע"מ לפריט עבור כל קבוצת מע"מ.

לאחר השלמת ‏‫הדרישות המוקדמות, על העובדים לבצע את השלבים הבאים כדי לבקש החזר עבור עסקאות מע"מ.

1. בדוח הוצאות, הזן פרטי מס של עסקאות בכרטיס אשראי כדי לזהות זכאויות להחזרי מע"מ.
2. יש לוודא שכל פרטי המס מלאים ולאחר מכן לרשום את דוח ההוצאות.
3. בצע עיבוד של הוצאות זכאיות להחזר מע"מ בין מדינות.
4. שלח את הנתונים על החזרי מע"מ לספק החיצוני כדי להגיש בקשות להחזרי מע"מ בין מדינות.
5. בצע עיבוד של הוצאות עבור החזר מע"מ מקומי.

הסעיפים הבאים כוללים דוגמאות המראות כיצד עובדי Contoso מבצעים כל שלב.

## <a name="on-an-expense-report-enter-tax-information-about-credit-card-transactions-to-identify-eligible-vat-refunds"></a>בדוח הוצאות, הזן פרטי מס של עסקאות בכרטיס אשראי כדי לזהות זכאויות להחזרי מע"מ

הגר, נציגת מכירות מחברת Contoso הממוקמת בארצות הברית, חזרה לאחרונה מנסיעת מכירות לבריטניה. במהלך הנסיעה היו להגר מספר הוצאות על ארוחות, והיא שילמה באמצעות כרטיס האשראי האישי שלה. כעת הגר צריכה להכין דוח הוצאות כדי להסדיר את עניין ההוצאות.

הגר מזינה את הפרטים בדוח ההוצאות: היא בוחרת ב **בריטניה** בשדה **מדינה/אזור** שבדף **ערוך דוח הוצאות**. לאחר מכן, מתבצע סינון של רשימת קבוצות המע"מ כך שרק הקבוצות הנוגעות לבריטניה מוצגות. הגר בוחרת את קבוצת המע"מ **בריטניה 001** ולאחר מכן בוחרת בפריט **ארוחות** מבין קבוצות המע"מ לפריטים. לאחר מכן, הגר מוסיפה עסקה של לינה. מאחר שיש רק קבוצת מע"מ אחת ורק קבוצת מע"מ אחת לפריט עבור לינה בבריטניה, אפשרות זו מוזנת אוטומטית בדוח ההוצאות של הגר.

לפי המדיניות של Contoso, עבור כל הוצאה חייבת להיות קבלה תואמת. לכן, כשהגר שומרת את דוח ההוצאות, היא מקבלת הודעה לפיה עליה לצרף קבלה עבור כל עסקה שהיא רשמה בדוח ההוצאות. הגר מוודאת שהיא צירפה לדוח ההוצאות צילום דיגיטלי של הקבלות על כל העסקאות ולאחר מכן מגישה את הדוח לקבלת אישור. לאחר מכן היא שולחת את העתקי הקבלות המודפסים אל הצוות המטפל בכך במערך האחורי. צוות זה ישלח את הנתונים על החזרי מע"מ לספק החיצוני אשר מגיש בקשות להחזרי מע"מ בין מדינות מטעם Contoso.

## <a name="make-sure-that-all-tax-information-is-complete-and-then-post-the-expense-report"></a>יש לוודא שכל פרטי המס מלאים ולאחר מכן לרשום את דוח ההוצאות

אפרת, מתאמת חשבונות זכאים ב- Contoso, צריכה להזין את פרטי המיסוי שחסרים בדוח ההוצאות לפני שהיא תוכל לשלוח את הדוח. היא פותחת את דף **פרטי דוח הוצאות** ורואה את דוח ההוצאות של הגר שעבר אישור. לאחר מכן, אפרת פותחת את דוח ההוצאות כדי לראות את פרטי העסקאות. היא רואה שהגר לא הזינה קבוצת מע"מ לפריט עבור אחת מהעסקאות. מכיוון שמידע זה חסר, אפרת לא יכולה לרשום את דוח ההוצאות. לכן, אפרת בודקת בדף **תצורות מס** בניהול הוצאות, ומוצאת את קבוצת המע"מ לפריט המתאימה למדינה/אזור ולסוג העסקה. כעת אפרת יכולה לרשום את דוח ההוצאות בספר החשבונות הראשי.

במהלך הרישום של דוח ההוצאות, נוצר פריט עבודה של החזר מע"מ. פריט עבודה זה מוקצה לחבר בצוות העיבוד במערך האחורי. אפרת מקבלת הודעה המאשרת שהרישום התבצע בהצלחה. בהודעה זו גם מצוין מספר עסקאות המע"מ שזוהו לצורך החזר.

## <a name="process-expenses-that-are-eligible-for-international-vat-recovery"></a>עיבוד של הוצאות זכאיות להחזר מע"מ בין מדינות

ארנון, חבר בצוות העיבוד במערך האחורי ב- Contoso, אחראי לאשר שכל המידע הנדרש לביצוע החזרי מע"מ נכלל בדוחות ההוצאות. הוא פותח את דף **החזר מס על הוצאות** ובוחר את דוח ההוצאות שהגר הגישה. ארנון מוודא שכל הקבלות הנדרשות צורפו ושהוזנו הפרטים הנכונים של קבוצת מע"מ וקודי מע"מ לפריט.

כאשר ארנון מקבל מהגר את העתקי הקבלות המודפסים, הוא מאמת את קבלות הנייר מול הקבלות הדיגיטליות ולאחר מכן משנה את הסטטוס של דוח ההוצאות ל **מוכן להחזר**.

## <a name="send-vat-recovery-data-to-the-third-party-vendor-to-file-international-recovery-returns"></a>שלח את הנתונים על החזרי מע"מ לספק החיצוני כדי להגיש בקשות להחזרי מע"מ בין מדינות

כאשר ארנון מוכן לשליחת נתוני דוח ההוצאות לספק החיצוני שיגיש את הבקשות להחזרי מע"מ, הוא פותח את דף **החזרי מס על הוצאות**. הוא מסנן את הדף כך שיוצגו רק דוחות ההוצאות המסומנים כ **מוכן להחזר**. לאחר מכן, ארנון בוחר **קובץ** &gt; **ייצא ל- Excel**. פרטי המע"מ מדוחות ההוצאות מיוצאים לגליון עבודה של Microsoft Excel. ארנון שולח את גליון העבודה לספק החיצוני וכולל הודעה המציינת כי הקבלות המודפסות נשלחו באמצעות שליח.

## <a name="process-expenses-for-domestic-vat-recovery"></a>עיבוד הוצאות עבור החזר מע"מ מקומי

ארנון חייב לוודא שהעסקאות המפורטות בדוח ההוצאות זכאיות להחזר מע"מ, ושהקבלות הדיגיטליות צורפו לדוחות. כדי להתחיל לטפל בהוצאות הזכאיות להחזר מקומי, ארנון פותח את הדף **החזר מס על הוצאות** ובוחר את דוח ההוצאות שיש לבדוק ולאמת. הוא מוודא כי הקבלות רשומות על שם החברה ולא על שם העובד. לצורך החזר מע"מ, הקבלות חייבות להיות על שם החברה. לאחר מכן, ארנון מאשר שהקודים הנכונים של מס מכירה וקבוצת מס מכירה מופיעים.

כאשר ארנון מקבל את הקבלות המודפסות, הוא משנה את הסטטוס של דוח ההוצאות ל **מוכן להחזר**. לאחר מכן הוא יכול להגיש את הבקשה להחזר לרשות המס המתאימה. במקרה זה, רשות המסים המתאימה בארה"ב היא מס הכנסה (IRS).