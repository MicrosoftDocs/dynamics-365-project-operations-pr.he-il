---
title: קביעת התצורה של חשבונאות לפרוייקטים פנימיים
description: נושא זה מספק מידע על אופן הגדרת נוהלי חשבונאות עבור פרויקטים פנימיים ב-Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 504e7481cb2aee6310cb4ace2d0791d1c7fe360d
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077242"
---
# <a name="configure-accounting-for-internal-projects"></a>קביעת התצורה של חשבונאות לפרוייקטים פנימיים

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

פרויקטים פנימיים מאפשרים לחברות לעקוב אחר עלויות הקשורות לפעילויות שלא מחייבים עבורן את הלקוח. דוגמאות לפרויקטים פנימיים כוללים:

- פיתוח מוצר, כמו אפליקציה למכשירים ניידים, ומעקב אחר העלויות הכרוכות בפיתוח.
- ניהול זמן והוצאות טרום-מכירה. ניתן להמיר פרויקט טרום-מכירה פנימי זה מאוחר יותר לפרויקט לחיוב אם הצעת המחיר זוכה.

כל פרויקט שאינו משויך לחוזה ב-Dynamics 365 Project Operations מטופל כפרויקט פנימי. פרופילי העלות וההכנסות של פרויקט אינם משמשים לקביעת עקרונות החשבונאות עבור הפרויקט. עלות פרויקט פנימית נרשמת תמיד על פי עקרונות רווח והפסד. חשבונות ספר ראשי עבור רישומים מוגדרים בדף **הגדרת רישום בספר ראשי**.

- עסקאות זמן מתבצעות באמצעות חיוב חשבון **עלות** וזיכוי חשבון **הקצאת שכר**.
- עסקאות של הוצאה נרשמות באמצעות חיוב חשבון **עלות** וזיכוי **חשבון קיזוז להוצאות**.

לאחר רישום עסקאות בפרויקט, אם הפרויקט משויך לחוזה פרוייקט, המערכת מבטלת את כל העסקאות שנצברו ויוצרת עסקאות חדשות לחיוב. העסקאות לחיוב מתבצעות לפי כללי החשבונאות המוגדרים בפרופיל העלות וההכנסות של הפרויקט, בהתאמה.

