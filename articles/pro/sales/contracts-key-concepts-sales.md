---
title: מושגים מרכזיים של חוזי פרויקט
description: נושא זו מספק מידע אודות המושגים המרכזיים של חוזי פרוייקט.
author: rumant
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 66d6b72b19a90ecc9161cd16ce9d4dd22798803b
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077214"
---
# <a name="key-concepts-of-project-contracts"></a>מושגים מרכזיים של חוזי פרויקט

_**חל על** : פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_

נושא זה מאיר את מושגי מפתח שכדאי להיות מודעים אליהם לפני שמתחילים להשתמש בחוזי פרויקט ב-Dynamics 365 Project Operations:

## <a name="contracting-unit"></a>יחידת החוזה

יחידת החוזה מייצגת את החטיבה או את הפרקטיקה שמסירת הפרויקט נמצאת בבעלותה. ניתן להגדיר עלויות משאבים לכל יחידת חוזה. כאשר מציינים את עלות המשאב עבור משאב, אפשר גם להגדיר שיעורי עלות שונים עבור משאבים. יחידה קבלנית זו שואלת משאבים אלה מחטיבה או מפרקטיקות אחרות בארגון. שיעורי העלות עבור משאבים אלה מכונים מחירי העברה, שאילת משאבים או מחירי חליפין. כאשר מגדירים את שיעורי העלות להשאלת המשאבים מחטיבות אחרות, אפשר גם לבחור להגדיר שיעורי עלות אלה במטבע של החטיבה המלווה.

## <a name="cost-currency"></a>מטבע עלות

מטבע העלות הוא המטבע שבו מדווחים על עלויות במסך. מטבע זה נגזר מהמטבע המצורף לשדה **יחידת החוזה** בחוזה ובפרויקט. ניתן לרשום עלויות בכל מטבע כנגד פרויקט. עם זאת, יש המרת מטבע מהמטבע שבו נרשמו העלויות למטבע העלות של הפרויקט כאשר מוצג על המסך.

מכיוון ששערי החליפין בפלטפורמת (CDS) Common Data Service אינם יכולים להיות תקפים לתאריך מסוים, סיכומי העלות שמוצגים על המסך עשויים להשתנות לאורך זמן אם תעדכן את שערי החליפין של המטבע. עם זאת, העלויות כפי שהן רשומות במסד הנתונים נותרות ללא שינוי מכיוון שהסכומים מאוחסנים במטבע שבו הן נגרמו.

## <a name="sales-currency"></a>מטבע מכירות

מטבע מכירות ב- Project Operations הוא המטבע שבו נרשמים ומוצגים סכומי המכירות בפועל והמשוערים. מטבע המכירה הוא גם המטבע שבו מוגשת חשבונית ללקוח עבור העסקה. בהצעת מחיר לפרויקט, מטבע המכירות הוא ברירת המחדל מרשומת תיק הלקוח או הלקוח וניתן לשנותו בעת יצירת החוזה. כאשר נוצר חוזה על ידי סגירת הצעת מחיר כזכייה, כברירת מחדל, המטבע של החוזה מוגדר למטבע שבהצעת המחיר.

כאשר יוצרים חוזה פרויקט מאפס, השדה **מטבע המכירות** לא ניתן לעריכה. מחירוני מוצרים ופרויקטים נקבעים כברירת מחדל על סמך מטבע החוזה.

בניגוד לעלויות, ניתן לרשום ערכי מכירות רק במטבע המכירות.

## <a name="billing-method"></a>שיטת חיוב

בדרך כלל, לפרויקטים יש שני סוגי מודלים של חוזה, אחד בתשלום קבוע ושני מבוסס-צריכה. מודלים אלה מיוצגים ב-Project Operations כשיטות חיוב עם שני ערכים אפשריים:

- זמן וחומרים: זהו מודל חוזה מבוסס-צריכה בו כל עלות שנגרמת מגובה בהכנסה תואמת. ככל שמעריכים או צוברים יותר עלויות, המכירות המשוערות והמכירות בפועל התואמות יגדלו אף הן. ציין מגבלות 'אין לחרוג' בסעיפי חוזה עם שיטת חיוב זו, שיקבעו את תקרת ההכנסות בפועל. ההכנסה המשוערת לא מושפעת ממגבלות 'אין לחרוג'.
- מחיר קבוע: מודל חוזה בתשלום קבוע המציין כי ערכי המכירה יהיו בלתי תלויים בעלויות שייגרמו. ערך המכירות הוא קבוע ואינו משתנה כאשר מעריכים או צוברים עלויות נוספות.

## <a name="project-price-lists"></a>מחירוני פרוייקט

מחירוני פרויקטים משמשים למחירי ברירת מחדל, לא לתעריפי עלות, עבור זמן, הוצאות ורכיבים אחרים הקשורים לפרויקט. יכולים להיות מחירונים מרובים. לכל מחירון יש תאריכים תקפים משלו עובר כל חוזה פרויקט. ב-Project Operations אין תמיכה בחפיפה של התאריכים התקפים של מחירוני פרויקטים.

כאשר נוצר חוזה פרויקט על ידי זכייה בהצעת מחיר לפרויקט, מחירוני הפרויקט מועתקים יחד עם שם החוזה והתאריך. העתקת מידע זה מהווה תמחור מותאם אישית לרכיבי הפרויקט בחוזה פרויקט זה.

## <a name="product-price-lists"></a>מחירוני מוצרים

מחירוני מוצרים הם מחירונים המשמשים להגדרת מחירי ברירת מחדל, לא שיעורי עלות, עבור סעיפי חוזה מבוססי מוצר. לכל חוזה יש רק מחירון מוצרים אחד.

## <a name="transaction-classes"></a>סיווגי עסקאות

Project Operations תומך בארבעה סוגים של סיווגי עסקאות:

- זמן
- הוצאה
- חומרים
- תשלום

ניתן להעריך ולצבור ערכי עלות ומכירות בסיווגי העסקאות זמן, הוצאה וחומר. עמלה היא סיווג עסקה של הכנסה בלבד.

## <a name="work-entities-and-billing-entities"></a>ישויות עבודה וישויות חיוב

ישויות המייצגות עבודה הן פרויקטים ומשימות. ישויות המייצגות הבטים של חיוב הן סעיפי חוזה. באפשרותך לקשר בין ישויות עבודה שונות לאפשרויות חיוב על-ידי קשירתן לסעיפי חוזה.

## <a name="multi-customer-deals"></a>עסקאות מרובות לקוחות

עסקאות מרובות לקוחות הן עסקאות שבהן יש יותר מלקוח אחד שיש להנפיק לו חשבונית עבור העסקה. דוגמאות נפוצות כוללות את:

- ארגוני OEM ושותפיהן: שותפים ומפיצים מוכרים מוצר עם כמה שירותים בעלי ערך מוסף, שבדרך כלל כרוך בעסקה מסוימת עם לקוח. חברת ה-OEM מציעה לממון חלק מהפרויקט. 

- פרויקטים במגזר הציבורי: מחלקות מרובות של מוסדות ממשלתיים מקומיים מסכימות לממן פרויקט ומוגש להן חשבונית על פי חלוקה שסוכמה לפני כן. למשל, מחלקת החינוך ומוסדות השלטון המקומי מסכימים לממן את הבנייה של בריכת שחייה.

## <a name="invoice-schedules"></a>לוחות זמנים של חשבוניות

לוחות הזמנים של חשבוניות הם ספציפיים לכל סעיף חוזה ונדרשים כדי שההפקה האוטומטית של חשבוניות תעבוד. לוחות זמנים של חשבוניות נוצרים על סמך תאריכי התחלה וסיום מסוימים ועל סמך תדירות החשבונית. לוחות הזמנים משמשים בשלב החוזה, כאשר מוגדר תהליך הפקת החשבוניות האוטומטי. כאשר נוצר חוזה פרויקט מהצעת מחיר, לוח הזמנים של החשבונית מועתק לחוזה הפרויקט מהצעת המחיר.

## <a name="changes-from-the-dynamics-365-sales-contract"></a>שינויים מחוזה של Dynamics 365 Sales

חוזים של Project Operations בנויים על חוזים של Dynamics 365 Sales. עם זאת, ישנם כמה הבדלים חשובים בפונקציונליות שעליך להיות מודע להם:

- בחוזי Project Operations שני סוגים סעיפים שונים, אחד לפרויקטים ואחד למוצרים.
- לחוזים של Project Operations יש רכיבי ממשק משתמש וטופס משלהם, כללים עסקיים, לוגיקה עסקית ביישומי plug-in וקבצי Script בצד הלקוח משלהן, שמייחדים אותן חוזים של מכירות.

מסיבות אלה, אין להשתמש בחוזה מכירה ובחוזה פרוייקט באופן חליפי.