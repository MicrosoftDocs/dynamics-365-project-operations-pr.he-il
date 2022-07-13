---
title: פרטי כותרת עבור חשבוניות ספק
description: מאמר זה מסביר את הפונקציונליות המופיעה בכותרת חשבונית הספק ב- Microsoft Dynamics 365 Project Operations.
author: rumant
ms.date: 03/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 95f84f2d2a357abbd8d507705412a0434b44f658
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8929859"
---
# <a name="header-details-for-vendor-invoices"></a>פרטי כותרת עבור חשבוניות ספק

[!include [banner](../../includes/dataverse-preview.md)]

_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_

מאמר זה מסביר את הפונקציונליות המופיעה בכותרת חשבונית הספק ב- Microsoft Dynamics 365 Project Operations.

כאשר מנהלי פרוייקטים מתכננים ומבצעים פרוייקטים, הם יכולים להעסיק קבלני משנה ולרכוש מוצרים מספקים. בעת ביצוע פרוייקט, העלויות נוצרות משירותים, חומרים וקטגוריות הוצאות שנרכשו בחוזי משנה מול ספקים. הספקים מחייבים עלויות אלה לפרוייקטים על-ידי יצירה של חשבוניות ספק.

הטבלה הבאה מספקת מידע על השדות בכותרות של חשבוניות ספק ב- Project Operations

| שדה | Description | השפעה פונקציונלית |
| --- | --- | --- |
| Name | שם חשבונית הספק. | בכל הרשימות הנפתחות של חשבונית ספק, שם חשבונית הספק מופיע בעמודה הראשונה כדי לעזור לך לזהות את חשבונית הספק. כברירת מחדל, כאשר נוצרת חשבונית ספק מחוזה משנה, השדה **שם** של חשבונית הספק מוגדר לערך המורכב משם חוזה המשנה בתוספת התאריך הנוכחי. |
| Description | תיאור קצר של השירותים והמוצרים המופיעים בחשבונית הספק. | ללא |
| יצרן | שם החברה שמנפיקה חשבונית עבור המוצרים והשירותים. חברה זו צריכה להיות רשומת חשבון עם יחסי גומלין מסוג **ספק** או **יצרן**. | <p>בהתבסס על הספק שנבחר, ערכי ברירת המחדל מוזנים אוטומטית בשדות הבאים:</p><ul><li>מטבע</li><li>מחירונים</li><li>תנאי תשלום</li><li>כתובת תשלום</li></ul> |
| חוזה משנה | הפניה לחוזה המשנה עבור חשבונית הספק. | <p>בהתבסס על חוזה המשנה שנבחר, ערכי ברירת המחדל מוזנים אוטומטית בשדות הבאים:</p><ul><li>מטבע</li><li>מחירונים</li><li>תנאי תשלום</li><li>כתובת תשלום</li></ul><p>חוזה המשנה שנבחר בכותרת של חשבונית הספק מוזן כברירת מחדל בשורות חשבונית הספק ולא ניתן לשנותו שם.</p> |
| תאריך חשבונית | התאריך עבור העלויות בפועל שייווצרו עם אישור חשבונית הספק. | תאריך החשבונית משמש גם לבחירת מחירון הרכישה הנכון מתוך המחירונים הקשורים לספק הקשור או מפרמטרי הפרוייקט. |
| סיבת המצב‬ | מצב חשבונית הספק. | <p>המצב קובע היכן נמצאת חשבונית הספק בתהליך העסקי ואם ניתן לערוך אותה. להלן כמה מהערכים הזמינים:</p><ul><li>**טיוטה**: ניתן לערוך את חשבונית הספק.</li><li>**אושר** - חשבונית הספק אומתה ואושרה. לא ניתן לערוך או למחוק חשבונית ספק במצב זה.</li><li>**מתבצע** - חשבונית הספק נמצאת בבדיקה. ניתן לערוך אך לא למחוק חשבוניות במצב זה.</li><li>**בוטל** - חשבונית הספק בוטלה. לא ניתן לערוך או למחוק חשבונית ספק במצב זה.</li></ul> |
| מטבע | המטבע שבו הספק מנפיק חשבונית עבור המוצאים והשירותים בחשבונית הספק. | בחשבונית ספק עם הפניה לחוזה משנה, המטבע של חוזה המשנה מוזן כברירת מחדל כמטבע של חשבונית הספק. בחשבונית ספק ללא הפניה לחוזה משנה, ערך ברירת המחדל מוזן מרשומת חשבון הספק וניתן לשנותו. לאחר שמירת חשבונית ספק, לא ניתן עוד לערוך את המטבע. |
| יחידת החוזה | חטיבת החברה האחראית על קבלת השירותים ו/או המוצרים מהספק. | ללא |
| תנאי תשלום | תנאי התשלום בחשבוניות הספק המונפקות. ערך ברירת המחדל מוזן אוטומטית מרשומת חשבון הספק. | תנאי תשלום מחוזה משנה מועתקים לכל חשבוניות הספק הקשורות לחוזה המשנה. ניתן לעדכן את תנאי התשלום אם יש לחשבונית הספק מצב של **טיוטה**. |
| כתובת תשלום | כתובת הספק שאליה יש לשלוח תשלומים. ערך ברירת המחדל מוזן אוטומטית מרשומת חשבון הספק. | כתובת התשלום מחוזה משנה מועתקת ככתובת התשלום לכל חשבוניות הספק שנוצרות עבור אותו חוזה משנה. ניתן לעדכן את כתובת התשלום אם יש לחשבונית הספק מצב של **טיוטה**. |
| סכום ביניים | אם בחשבונית הספק אין שורות, הזן את סכום הביניים של החשבונית לפני מיסים. אם חשבונית הספק כוללת שורות, שדה זה יהיה לקריאה בלבד. במקרה זה, הסכום המוצג הוא סכום הביניים מכל השורות בחשבונית הספק. | ללא |
| סה''כ מס | אם בחשבונית הספק אין שורות, הזן את סכום המס הכולל בחוזה המשנה. אם חשבונית הספק כוללת שורות, שדה זה יהיה לקריאה בלבד. במקרה זה, הסכום המוצג הוא סכום המס מכל השורות בחשבונית הספק. | ללא |
| סכום כולל | שדה מחושב זה מציג את הסכום הכולל של חשבונית הספק לאחר הוספת מיסים. | ללא |

> [!NOTE]
> לא ניתן לשנות את השדות הבאים בחשבנית ספק לאחר שמירת חשבונית הספק: **ספק**, **חוזה משנה**, **מטבע**, **יחידת החוזה** ו **תנאי תשלום**. אם נדרשים שינויים כלשהם בשדות אלה בחשבונית ספק, עליך למחוק את חשבונית הספק וליצור חשבונית ספק חדשה.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]