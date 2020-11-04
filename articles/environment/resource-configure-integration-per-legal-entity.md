---
title: קביעת תצורה של שילוב Project Operations עבור כל ישות משפטית
description: נושא זה מספק מידע על הגדרת שילוב לפי ישות משפטית ב- Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/21/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: c0e02ef2d17bf49209369f7adad681d9a5981e2a
ms.sourcegitcommit: 91ad491e94a421f256a378b0f4b26ed48c67bc93
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/22/2020
ms.locfileid: "4096753"
---
# <a name="configure-project-operations-integration-per-legal-entity"></a>קביעת תצורה של שילוב Project Operations עבור כל ישות משפטית 

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

נושא זה מתאר את השלבים הנדרשים להגדרת תצורת Dynamics 365 Project Operations לכל ישות משפטית.

## <a name="enable-feature-keys-in-dynamics-365-finance"></a>הפעלת מפתחות של ישויות ב- Dynamics 365 Finance

בצע את השלבים הבאים כדי להפעיל תכונות נדרשות.

1. ב- Dynamics 365 Finance, עבור אל סביבת העבודה **ניהול ישויות**.
2. ב **רשימת תכונות** , מצא והפעל את התכונות הבאות:
  
    - **הפעל מספר סעיפי חוזה לפרויקט**
    - **הפעל את Project Operations ב- Dynamics 365 Customer Engagement**

> [!NOTE]
> אם אתה לא רואה את **מקשי התכונות** ברשימה, ודא שגרסת Finance שלך עומדת בדרישת הגרסה המינימלית (גרסת היישום 10.0.13 עם כל עדכוני האיכות שהוחלו ומעלה). בחר **בדוק עדכונים** כדי לרענן את רשימת התכונות.

## <a name="define-the-project-operations-deployment-scenario-for-a-legal-entity"></a>הגדר את תרחיש הפריסה ב- Project Operations עבור ישות משפטית

באפשרותך להפעיל את Project Operations ב- Dynamics 365 Customer Engagement ברמת הישות המשפטית. יכולה להיות לך ישות משפטית אחת באמצעות Project Operations ב- Dynamics 365 Customer Engagement לתרחישים מבוססי משאבים/ללא מלאי. באותה סביבה, יכולה להיות לך ישות משפטית אחרת המשתמשת ב- Project Operations לתרחישים בהזמנת מלאי/ייצור.

1. ב- Dynamics 365 Finance עבור אל **ניהול פרויקטים וחשבונאות** > **הגדרה** > **ניהול פרויקטים ופרמטרים חשבונאיים**.
2. ברשימת הישויות המשפטיות הזמינות, בחר ישויות שבהן יש מספר סעיפי חוזה והתכונות של Project Operations ב- Dynamics 365 Customer Engagement פועלות. השאר את הישויות המשפטיות שישתמשו ב- Project Operations עבור תרחישים במלאי/הזמנת ייצור.

> [!NOTE]
> ניתן לבחור ישות משפטית רק אם אין לה פרויקטים קיימים.

## <a name="configure-project-management-and-accounting-parameters"></a>הגדרה של ניהול פרויקטים ופרמטרים של חשבונאות

כל ישות משפטית שמשתמשת ב- Project Operations ב- Dynamics 365 Customer Engagement צריכה קבוצה של פרמטרים המוגדרים כברירת מחדל. פרמטרים אלה מוגדרים בכרטיסיה **Project Operations** בדף **ניהול פרויקטים ופרמטרים חשבונאיים**. הפרמטרים הם:

  - **ברירות מחדל של סוג חיוב** :‏ Project Operations משתמש בקבוצה קבועה של ברירות מחדל מסוג חיוב שיש למפות למאפייני השורות של Finance. צור רשומה עבור כל סוג חיוב: **לא מוגדר** , **בתשלום** , **ללא חיוב** , **משלים** ו **לא זמין**.
  - **ברירות מחדל של קטגוריית הפרויקט** : בחר בקטגוריות הפרויקט המוגדרות כברירת מחדל לשימוש עבור כל סוג עסקה. ברירות מחדל אלה ישמשו ב- **כתב העת לשילוב Project Operations** ובהערכות שבהן לא מוגדרת קטגוריית עסקאות עבור הפרויקט בפועל.
  - **תחזיות** : בחר במודל התחזית שישמש לאומדני זמן והוצאות.