---
title: מבט כולל על זיהוי הכנסה
description: נושא זו מספק מידע על זיהוי הכנסות ב-Project Operations.
author: sigitac
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.custom: intro-internal
ms.openlocfilehash: 3d2fcf434a5086595e40f50afc2366eb806168085ae9212b5d25e3e9bd02e2c6
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/06/2021
ms.locfileid: "6988652"
---
# <a name="revenue-recognition-overview"></a>מבט כולל על זיהוי הכנסה

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

ב- Dynamics 365 Project Operations, עקרונות של זיהוי הכנסות משתנים בהתאם לשיטת החיוב שנבחרה עבור פרויקט או חלק מהפרויקט. נושא זו מספק מידע על זיהוי הכנסות ב-Project Operations.

## <a name="transactions-accounted-using-time-and-material-billing-method"></a>עסקאות מחויבות לפי שיטת חיוב עבור זמן וחומר

- יש קשר בין עלויות לזיהוי הכנסות. עלות העסקה והמכירות שלא בוצעו נרשמות באמצעות [יומן לשילוב Project Operations](../project-accounting/project-operations-integration-journal.md).
- עלות הפרויקט ופרופיל ההכנסות קובעים אם עסקאות מכירה שלא בוצעו נרשמות בספר החשבונות הכללי. אם נבחרה **צבירת הכנסות**, המערכת משתמשת בנתונים **ערך מכירות WIP** ו- **שווי מכירות שהצטברו** במהלך הפרסום. להלן דוגמה לשיטה זו.  

  | סוג עסקה | חיוב/אשראי | סכום |
  | --- | --- | --- |
  | ערך מכירה של WIP | חיוב | 100 |
  | ערך מכירה של הכנסה נצברת | אשראי | 100 |

- ההכנסה מזוהה בעת הפקת החשבונית. המערכת משתמשת בחשבון **הכנסות מחשבוניות** במהלך הפרסום. להלן דוגמה לשיטה זו.  

  | סוג עסקה | חיוב/אשראי | סכום |
  | --- | --- | --- |
  | יתרת לקוחות | חיוב | 120 |
  | מס מכירות לתשלום | אשראי | 20 |
  | הכנסה שחויבה | אשראי | 100 |

- אם הצטברו הכנסות בעת רישום מכירות שלא בוצעו, המערכת תהפוך את ההכנסות שנצברו בחשבונית.

  | סוג עסקה | חיוב/אשראי | סכום |
  | --- | --- | --- |
  | ערך מכירה של WIP | אשראי | 100 |
  | ערך מכירה של הכנסה נצברת | חיוב | 100 |

## <a name="transactions-accounted-using-the-fixed-price-billing-method"></a>עסקאות מחויבות לפי שיטת חיוב של מחיר קבוע

- אין קשר בין עלויות לזיהוי הכנסות. עלות העסקה מפורסמת באמצעות [יומן לשילוב Project Operations](../project-accounting/project-operations-integration-journal.md). לא נוצרות עסקאות מכירה שלא חויבו.
- הכנסה יכולה להיות מזוהה במהלך הפקת החשבונית אם לעלות הפרויקט ולפרופיל ההכנסות יש **עקרון המשמש לחישובי השלמת הפרויקט** שמוגדר **ללא WIP**. השתמש בשיטה זו בפרויקטים פשוטים לטווח קצר.
- ניתן לזהות הכנסות באמצעות אומדני הכנסות עם מחירים קבועים, כאשר השיטה **חוזה שהושלם** או **זיהוי אחוזים מהכנסות שהושלמו**.

## <a name="additional-resources"></a>משאבים נוספים
[מאמר על קביעת תצורה של חשבונאות לפרויקטים הניתנים לחיוב](../project-accounting/configure-accounting-billable-projects.md)

[פרוייקטים של הערכת הכנסה במחיר קבוע](rev-rec-percentage-completion-method.md)

[ניהול הערכות הכנסה](rev-rec-completed-contract-method.md)

[עלות להשלמת שיטות](cost-complete-methods.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]