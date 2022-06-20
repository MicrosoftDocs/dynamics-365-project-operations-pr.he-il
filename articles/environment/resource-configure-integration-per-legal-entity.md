---
title: קביעת תצורה של שילוב Project Operations עבור כל ישות משפטית
description: מאמר זה מספק מידע על הגדרת שילוב לפי ישות משפטית ב- Project Operations.
author: sigitac
ms.date: 10/21/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 3f33e641ee0932655282618c99a26e2603660059
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8914679"
---
# <a name="configure-project-operations-integration-per-legal-entity"></a>קביעת תצורה של שילוב Project Operations עבור כל ישות משפטית 

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

מאמר זה מנחה אותך בשלבים הדרושים להגדרה Dynamics 365 Project Operations לכל ישות משפטית.

## <a name="enable-feature-keys-in-dynamics-365-finance"></a>הפעלת מפתחות של תכונות ב- Dynamics 365 Finance

בצע את השלבים הבאים כדי להפעיל תכונות נדרשות.

1. ב- Dynamics 365 Finance, עבור אל סביבת העבודה **ניהול תכונות**.
2. ב **רשימת תכונות**, מצא והפעל את התכונות הבאות:
  
    - **הפעל מספר סעיפי חוזה לפרויקט**
    - **הפעלת Project Operations ב- Dynamics 365 Customer Engagement**

> [!NOTE]
> אם אתה לא רואה את **מקשי התכונות** ברשימה, ודא שגרסת Finance שלך עומדת בדרישת הגרסה המינימלית (גרסת היישום 10.0.13 עם כל עדכוני האיכות שהוחלו ומעלה). בחר **בדוק עדכונים** כדי לרענן את רשימת התכונות.

## <a name="define-the-project-operations-deployment-scenario-for-a-legal-entity"></a>הגדר את תרחיש הפריסה ב- Project Operations עבור ישות משפטית

ניתן להפעיל את Project Operations ב- Dynamics 365 Customer Engagement ברמת ישות משפטית. ניתן להחזיק בישות משפטית אחת באמצעות Project Operations ב- Dynamics 365 Customer Engagement עבור תרחישים על בסיס משאבים/שאינם במלאי. באותה סביבה, יכולה להיות לך ישות משפטית אחרת המשתמשת ב- Project Operations לתרחישים בהזמנת מלאי/ייצור.

1. ב- Dynamics 365 Finance, עבור אל **ניהול וחשבונאות של פרוייקטים** > **הגדרה** > **ניהול פרוייקטים כלליים ופרמטרים חשבונאיים**.
2. ברשימת הישויות המשפטיות הזמינות, בחר ישויות שבהן מופעלים סעיפי חוזה מרובים ותכונות של Project Operations ב- Dynamics 365 Customer Engagement. השאר את הישויות המשפטיות שישתמשו ב- Project Operations עבור תרחישים במלאי/הזמנת ייצור.

> [!NOTE]
> ניתן לבחור ישות משפטית רק אם אין לה פרויקטים קיימים.

## <a name="configure-project-management-and-accounting-parameters"></a>הגדרה של ניהול פרויקטים ופרמטרים של חשבונאות

כל ישות משפטית המשתמשת ב-Project Operations ב-Dynamics 365 Customer Engagement זקוקה לקבוצה של פרמטרי ברירת מחדל. פרמטרים אלה מוגדרים בכרטיסיה **Project Operations** בדף **ניהול פרויקטים ופרמטרים חשבונאיים**. הפרמטרים הם:

  - **ברירות מחדל של סוג חיוב**:‏ Project Operations משתמש בקבוצה קבועה של ברירות מחדל מסוג חיוב שיש למפות למאפייני השורות של Finance. צור רשומה עבור כל סוג חיוב: **לא מוגדר**, **בתשלום**, **ללא חיוב**, **משלים** ו **לא זמין**.
  - **ברירות מחדל של קטגוריית הפרויקט**: בחר בקטגוריות הפרויקט המוגדרות כברירת מחדל לשימוש עבור כל סוג עסקה. ברירות מחדל אלה ישמשו ב- **כתב העת לשילוב Project Operations** ובהערכות שבהן לא מוגדרת קטגוריית עסקאות עבור הפרויקט בפועל.
  - **תחזיות**: בחר במודל התחזית שישמש לאומדני זמן והוצאות.


[!INCLUDE[footer-include](../includes/footer-banner.md)]