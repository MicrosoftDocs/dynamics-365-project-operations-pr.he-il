---
title: יצירת מקדמה אד-הוק על חוזה
description: נושא זה מספק מידע על יצירת מקדמה במזומן על חוזה לפי הצורך.
author: rumant
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 790a0281f72eff5f241d11da025b5b4af643a567
ms.sourcegitcommit: 250270409412ba4cad95fbd4c345a80d3d2b3e53
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 11/21/2020
ms.locfileid: "4595981"
---
# <a name="creating-an-ad-hoc-advance-on-a-contract"></a>יצירת מקדמה אד-הוק על חוזה

_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_

Microsoft Dynamics 365 Project Operations ‏תומך בתרחישים של חשבוניות הכוללים תשלומים מקדמים ומקדמות. תהליך השימוש ב **מקדמות במזומן** ב-**Project Operations** דומה לחוזי **ריטיינר**. 

בצע את השלבים הבאים כדי להגיש ללקוח חשבונית על מקדמה במזומן.

1. עבור אל הדף **חוזה פרויקט** ולאחר מכן בחר את הכרטיסיה **מקדמות במזומן וריטיינרים**.
2. ברשת-המשנה המפרטת את כל המקדמות במזומן ותשלומי המקדמה שנרשמו בעבר, בחר **+ ריטיינר חדש לחוזה פרוייקט**. 

    הטופס **יצירה מהירה** נפתח לרישום של תשלום מקדמה או מקדמה במזומן.
    
3. הטבלה שלהלן מפרטת את השדות לרישום מקדמה במזומן ואת השיקולים שיש לקחת בחשבון בעת יצירת מקדמות חדשות:

    | שדה | תיאור | השפעה במורד הזרם |
    | --- | --- | --- |
    | **לקוח חוזה הפרויקט** | שדה זה מציין לאיזה לקוח בחוזה יוגש חשבונית בגין מקדמה במזומן זו. | אם יש לך מספר לקוחות בחוזה וברצונך לחייב כל אחד מהם עבור ריטיינר או סכום של מקדמה במזומן ספציפי, צור מקדמה במזומן עבור כל לקוח בנפרד. |
    | **תיאור** | תיאור המטרה או העיתוי של המקדמה במזומן בכדי לסייע בזיהוי מקדמה במזומן זו. | תיאור זה מוצג בשורת החשבונית בגין מקדמה במזומן זו. |
    | **סכום** | סכום תשלום המקדמה או המקדמה במזומן. | סכום זה מוצג בשורת החשבונית בגין מקדמה במזומן זו. |
    | **תאריך חשבונית** | המועד בו מוגש חשבונית הלקוח עבור מקדמה במזומן זו. | זהו התאריך לתהליך יצירת החשבונית האוטומטית ליצירת שורת חשבונית עבור מקדמה במזומן זו. |
    | **מצב חשבונית** | זוהי הגדרת אפשרות המציינת אם מקדמה במזומן זו מתווספת לטיוטת חשבונית עבור לקוח זה. הערכים האפשריים הם:</br>- **לא מוכן להגיש חשבונית**</br>- **מוכן להגיש חשבונית** | כאשר מקדמה במזומן או תשלום מקדמה מסומנים כ **מוכן להגשת חשבונית**, הוא מתווסף כשעת שורה בחשבונית טיוטה. ניתן להשתמש רק במקדמה במזומן שחויבה במלואה להתאמה מול עלויות הפרויקט לתקופת החשבונית הבאה. |

4. בחר **שמור וסגור** בתיבת הדו-שיח יצירה מהירה כדי לרשום את המקדמה במזומן או את תשלום המקדמה.