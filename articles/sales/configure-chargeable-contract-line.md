---
title: קביעת תצורה של רכיבים הניתנים לחיוב של סעיף חוזה מבוסס פרויקט
description: נושא זה מספק מידע אודות רכיבים כלולים, רכיבים הניתנים לחיוב ורכיבים שאינם ניתנים לחיוב בסעיפי חוזה.
author: rumant
manager: Annbe
ms.date: 10/12/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: af97904b0171618cb15d060da9bc87fcf6bbabeb
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077245"
---
# <a name="configure-chargeable-components-of-a-project-based-contract-line"></a>קביעת תצורה של רכיבים הניתנים לחיוב של סעיף חוזה מבוסס פרויקט

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

בסעיף חוזה מבוסס פרויקט יש מושג של רכיבים כלולים, רכיבים הניתנים לחיוב ורכיבים שאינם ניתנים לחיוב.

הרכיבים הכלולים כפופים לשיטת החיוב, לפיצולי לקוחות, למגבלות 'אין לחרוג' ולהגדרות תדירות החשבונית המוגדרות בשורת החוזה מבוססת הפרויקט.

ניתן לסמן תת קבוצה של הרכיבים הכלולים כניתנים לחיוב באמצעות עדכון השדה **סוג החיוב**.

ניתן להגדיר רכיבים הניתנים לחיוב בתפקידים ובקטגוריות של עסקאות.

עבור סעיף חוזה פרויקט, יכולת החיוב המוגדרת לתפקיד חלה רק על סיווג העסקאות **זמן**. אם **כלול זמן** מוגדר כ **לא** בסעיף חוזה של פרויקט, הכרטיסיה **תפקידים הניתנים לחיוב** לא תהיה זמינה.

יכולת חיוב המוגדרת בקטגוריות של עסקאות עבור סעיף חוזה פרויקט חלה רק על סיווג העסקאות **הוצאה**. אם **כלול הוצאות** מוגדר כ **לא** בסעיף חוזה של פרויקט, הכרטיסיה **קטגוריות הניתנות לחיוב** לא תהיה זמינה.

### <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a>עדכן תפקיד כניתן לחיוב או כלא ניתן לחיוב

תפקיד יכול להיות ניתן לחיוב או לא ניתן לחיוב בסעיף חוזה מבוסס פרויקט ספציפי.

עדכן את סוג החיוב עבור תפקיד בכרטיסיה **תפקידים הניתנים לחיוב** של סעיף חוזה מבוסס פרויקט, ברשת המשנה **קטגוריות הניתנות לחיוב** , בשדה **סוג החיוב**.

### <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a>עדכן קטגוריית עסקאות כניתנת לחיוב או כלא ניתנת לחיוב

קטגוריה של עסקאות יכולה להיות ניתנת לחיוב או לא ניתנת לחייב בסעיף חוזה ספציפי המבוסס פרויקט.

עדכן את סוג החיוב עבור עסקה בכרטיסיה **קטגוריות הניתנות לחיוב** של סעיף חוזה מבוסס פרויקט, ברשת המשנה **קטגוריות הניתנות לחיוב** , בשדה **סוג החיוב**.

### <a name="resolve-chargeability"></a>פתרון של יכולת חיוב

אומדן או נתונים בפועל שנוצרו עבור זמן ייחשבו כניתנים לחיוב רק אם זמן כלול בסעיף החוזה, ואם התפקיד מוגדרים כניתן לחיוב בסעיף החוזה.

אומדן או נתונים בפועל שנוצרו עבור הוצאה ייחשבו כניתנים לחיוב רק אם הוצאה כלולה בסעיף החוזה, ואם הקטגוריות העסקה מוגדרת כניתנת לחיוב בסעיף החוזה.

| כולל זמן | כולל הוצאה | תפקיד | קטגוריה | משימה |
| --- | --- | --- | --- | --- |
| ‏‏כן | ‏‏כן | ניתן לחיוב | ניתן לחיוב | חיוב לפי נתוני זמן בפועל: ניתן לחיוב </br>סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב |
| ‏‏כן | ‏‏כן | לא ניתן לחיוב | ניתן לחיוב | חיוב לפי נתוני זמן בפועל: לא ניתן לחיוב </br>סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב |
| ‏‏כן | ‏‏כן | לא ניתן לחיוב | לא ניתן לחיוב | חיוב לפי נתוני זמן בפועל: לא ניתן לחיוב </br>סוג חיוב עבור נתונים של הוצאה בפועל: לא ניתן לחיוב |
| Yes | ‏‏כן | לא ניתן להגדיר | ניתן לחיוב | חיוב לפי נתוני זמן בפועל: לא זמין </br>סוג חיוב עבור נתוני הוצאה בפועל: ניתן לחיוב |
| Yes | ‏‏כן | לא ניתן להגדיר | לא ניתן לחיוב | חיוב לפי נתוני זמן בפועל: לא זמין </br>סוג חיוב עבור נתונים של הוצאה בפועל: לא ניתן לחיוב |
| ‏‏כן | Yes | ניתן לחיוב | לא ניתן להגדיר | חיוב לפי נתוני זמן בפועל: ניתן לחיוב </br>סוג חיוב עבור נתונים של הוצאה בפועל: לא זמין |
| ‏‏כן | Yes | לא ניתן לחיוב | לא ניתן להגדיר | חיוב לפי נתוני זמן בפועל: לא ניתן לחיוב </br> סוג חיוב עבור נתונים של הוצאה בפועל: לא זמין |