---
title: ייבוא הערכות עובר פרוייקט לשורת הצעת מחיר מבוססת פרויקט
description: נושא זה מספק מידע על ייבוא הערכות מפרויקט לשורת הצעת מחיר.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 75511f0d7ef1d2d1b3bf5cc598a8f51d0c553939
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908183"
---
# <a name="import-estimates-for-a-project-to-a-project-based-quote-line"></a>ייבוא הערכות עובר פרוייקט לשורת הצעת מחיר מבוססת פרויקט

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_


אם פרויקט נוצר בשלב טרום המכירה, ניתן לבחור לייבא את ההערכה הכספית מהפרויקט לשורת הצעת המחיר מבוססת הפרויקט.

1. וודא כי פרטי הפרויקט קיימים בשורת הצעת המחיר מבוססת הפרויקט, בשדה **פרויקט**.
2. בכרטיסיה **פרטים בשורת הצעת מחיר**, בחר **ייבא מהערכת הפרוייקט**.
3. לאחר פתיחת דף הדו-שיח, בחר באחת מהאפשרויות הסיכום הבאות.

  - **מחלקת עסקה**
  - **קטגוריה**
  - **תפקיד** 
  - **משימת פרוייקט**

על סמך בחירתך, ההערכה מהפרויקט עבור כל סווגי העסקאות הכלולות בשורת הצעת מחיר זו מועתקת. כדי לבדוק אילו סיווגי עסקאות כלולות, בחר בכרטיסיה **כללי** בשורת הצעת המחיר מבוססת הפרויקט, ובדוק את הערכים עבור **כלול זמן**, **כלול הוצאות**, ו**כלול עמלות**.

כאשר אתה מייבא הערכות, המערכת תגדיר תמחור ברירת המחדל בהתבסס על מחירוני הפרויקט המצורפים להצעת המחיר וסוג החיוב שהוגדר בשורת הצעת המחיר מבוססת הפרויקט. אם תפקיד או קטגוריה מוגדרים בשורת הצעת המחיר מבוססת הפרויקט כבלתי ניתנים לחיוב, שורת ההערכה המיובאת תוגדר כבלתי ניתנת לחיוב ולא תגיע לערך הצעת המחיר שבשורת הצעת המחיר.

כאשר קיימים פרטים בשורת הצעת מחיר, השדות **ערך הצעת המחיר** ו**המס המשוער** בשורת הצעת המחיר מסוכמים ואינם ניתנים לעריכה.

כאשר נבחרות אפשרויות סיכום מרובות, הסיכום מנסה לסכם לפי כל האפשרויות שנבחרו. המשמעות היא שהסכום של שורות הצעת מחיר מיובאות יהיה גבוה יותר מאשר אם הייתה נבחרת אפשרות סיכום אחת בלבד.

לדוגמא, אם בפרויקט קיימות שורות ההערכה הבאות להוצאות.

| משימה | קטגוריה | תאריך | כמות | מחיר יחידה | סכום |
| --- | --- | --- | --- | --- | --- |
| משימה א' | טיסות | 1/10/2020 | 4 | 400 | 1600 |
| משימה ב' | בתי מלון | 1/10/2020 | 4 | 200 | 800 |
| משימה ג' | בתי מלון | 1/11/2020 | 2 | 200 | 400 |

כאשר המשתמש בוחר לסכם לפי סיווגי עסקאות, המידע הבא ייובא.

| משימה | קטגוריה | תאריך | כמות | מחיר יחידה | סכום |
| --- | --- | --- | --- | --- | --- |
| | | 1/10/2020 | 3.34 | 840 | 2800 |

כאשר המשתמש בוחר לסכם לפי סיווגי עסקאות וקטגוריה, המידע הבא ייובא.

| משימה | קטגוריה | תאריך | כמות | מחיר יחידה | סכום |
| --- | --- | --- | --- | --- | --- |
| משימה א' | טיסות | 1/10/2020 | 4 | 400 | 1600 |
| | בתי מלון | 1/10/2020 | 6 | 200 | 1200 |

כאשר המשתמש בוחר לסכם לפי סיווגי עסקאות, קטגוריה ומשימת צומת עלה, המידע הבא ייובא. שימו לב שתוצאה זו זהה למה שהיה בפרויקט.

| משימה | קטגוריה | תאריך | כמות | מחיר יחידה | סכום |
| --- | --- | --- | --- | --- | --- |
| משימה א' | טיסות | 1/10/2020 | 4 | 400 | 1600 |
| משימה ב' | בתי מלון | 1/10/2020 | 4 | 200 | 800 |
| משימה ג' | בתי מלון | 1/11/2020 | 2 | 200 | 400 |