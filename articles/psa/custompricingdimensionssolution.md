---
title: יצירת פתרונות מותאמים אישית עבור ממדי תמחור
description: נושא זה מסביר כיצד ליצור פתרון מותאם אישית בעת יצירת ממדי תמחור מותאמים אישית.
author: Rumant
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: ae7f22b9cb092e956d0f1eaf1f1997c8e97392f4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012317"
---
# <a name="create-custom-solutions-for-pricing-dimensions"></a>יצירת פתרונות מותאמים אישית עבור ממדי תמחור

[!include [banner](../includes/psa-now-project-operations.md)]

> [!IMPORTANT]
> כל השינויים בממדי התמחור המותאמים אישית צריכים להיות בפתרון נפרד. שיטת עבודה מומלצת וחשובה זו מספקת גמישות בעתיד כדי לעדכן או להסיר שינויים בהתאם לצורך, היא תסייע לך להשתמש מחדש בעבודתך ומאפשרת להפנות את השינויים הללו אל מופע אחר בקלות רבה יותר. לאחר ביצוע כל השינויים הדרושים, ייצא פתרון זה כ **פתרון מנוהל** ויבא אותו אל מופעים אחרים כדי להשתמש שוב בהגדרת התמחור.

1. בחר **הגדרות** > **פתרונות**, ולאחר מכן בחר **חדש**. 
2. תן שם לפתרון, **\<your organization name> ממדי תמחור**, הזן את המידע הדרוש שנותר ובחר **שמור**.

> ![יצירת פתרון מותאם אישית עבור ממדי תמחור](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a>הוסף את כל הישויות הנדרשות ואת הרכיבים הקשורים לפתרון ממד התמחור
יהיה עליך להוסיף את הישויות הבאות של Project Service לפתרון התמחור שלך. השלם את השלבים שבהליך זה כדי לבצע שינויים חשובים בסכימה בפתרון התמחור כך שהישויות יהיו מודעות לממדי התמחור החדשים.

1. בחר **הגדרות** > **פתרונות** ולחץ פעמיים על **\<your organization name> ממדי תמחור**. 
2. בסייר הפתרונות, בחלונית הניווט הימנית בחר **הוסף קיים**  > **ישויות**.
3. בתיבת הדו-שיח **רכיבי פתרון**, בחר את הישויות הבאות:

- בפועל
- משאב הניתן להזמנה
- שורת הערכה
- משימת פרויקט
- פרט בשורת חשבונית
- שורת יומן
- פרט סעיף חוזה של פרויקט
- חבר צוות פרוייקט
- פרטים בשורת הצעת מחיר
- ייקור מחיר תפקיד
- מחיר תפקיד 
- ערך זמן 

> ![הוספת ישויות קיימות לפתרון ממדי התמחור](media/Existing-entities-to-PD-solution.png)

> ![בחירת רכיבי פתרון](media/Dimension-Components.png)

> [!NOTE]
> הקפד לכלול את כל הטפסים והתצוגות עבור כל אחת מהישויות שנבחרו.

4. כאשר תתבקש לכלול ישויות תלויות עבור הישויות שנבחרו, בחר **לא**.

> ![אל תכלול את כל הרכיבים הקשורים](media/Do-not-include-required.png)




[!INCLUDE[footer-include](../includes/footer-banner.md)]