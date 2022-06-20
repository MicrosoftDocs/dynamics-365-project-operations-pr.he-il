---
title: עדכון תכונות של יישום plug-in עם ממדי תמחור חדשים
description: מאמר זה מספק מידע על אופן עדכון תכונות של יישום plug-in עבור ממדי תמחור.
author: rumant
ms.date: 11/18/2020
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 2ae502fea533d9f199ef5ee1cc85b623f08cbd84
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8920015"
---
# <a name="update-plug-in-attributes-with-new-pricing-dimensions"></a>עדכון תכונות של יישום plug-in עם ממדי תמחור חדשים

מאמר זה מספק מידע על אופן עדכון תכונות של יישום plug-in עבור ממדי תמחור.

> [!NOTE]
> מאמר זה חל רק על תכונות הצעת המחיר והחוזה ב- Dynamics 365 Project Operations.

## <a name="prerequisites"></a>דרישות מוקדמות
לפני השלמת השלבים במאמר זה, עליך להשלים את ההליכים במאמרים הבאים:

  - [יצירת שדות וישויות מותאמים אישית](create-custom-fields-entities-pricing-dimensions.md) 
  - [הוספת שדות מותאמים אישית לישויות הגדרת מחיר וישויות של עסקאות ](add-custom-fields-price-setup-transactional-entities.md)
  - [הגדרת שדות מותאמים אישית כממדי תמחור](set-up-custom-fields-pricing-dimensions.md). 
  
אם לא השלמת הליכים אלה, השלם אותם ולאחר מכן חזור מאמר זה.

## <a name="register-a-plug-in"></a>רשום יישום plug-in
כאשר נוצר פרט של שורת הצעת מחיר בדף **שורת הצעת מחיר** עבור שורת הצעת מחיר של פרויקט, המערכת יוצרת שתי שורות אומדן. שורה אחת מיועדת לצד העלות של האומדן והשורה השנייה מיועדת למכירות. אותה פעולה מתבצעת עבור סעיפי חוזה של פרויקט.

בעת ביצוע שינוי בכמות או בשדה שבצד העלות, השינוי מופץ גם לצד המכירות. זה אפשרי מכיוון שיישומי plug-in של PreOperation ב- Quotelinedetail ובישויות פרטי חוזה מחוברים עם מאפיינים ספציפיים מצד העלות לצד המכירות של העסקה. אם אתה צריך ששינויים בערכי ממד התמחור בצד המכירות ייערכו גם בצד העלות, יש לרשום מחדש את יישומי ה-plug-in הבאים לאחר ביצוע שינויים בממד התמחור.

אלה יישומי ה-plug-in לעדכון ורישום מחדש:

- PreOperationContractLineDetailUpdate - **מעדכן את msdyn_orderlinetransaction**
- PreOperationQuoteLineDetailUpdate - **מעדכן את msdyn_quotelinetransaction**

השלם את השלבים הבאים לעדכון ורישום מחדש של יישומי plug-in.

1. פתח את **PluginRegistrationTool** והתחבר לסביבת Project Operations שלך ב- Dataverse.
2. בחר **חפש** והקלד את האותיות הראשונות של יישום plug-in שיעודכן.
3. לאחר מציאת יישום ה- Plug-in, בחר אותו ולאחר מכן בחר **בחר בטופס הראשי**.
4. בחר את השלב **Update msdyn_orderlinetransaction**, לחץ באמצעות לחצן העכבר הימני ולאחר מכן בחר **עדכן**.
5. בחלון **עדכון**, לחץ על שלוש הנקודות (**...**) בתכונות הסינון.
6. חלון מאפייני הסינון נפתח עם רשימה של כל התכונות בישות וממדי התמחור. בחר את תיבות הסימון עבור מאפייני ממד התמחור.
7. בחר **אישור** כדי לסגור את הדף ולאחר מכן בחר **עדכן שלב**.
8. חזור על שלבים 2 עד 7 עבור יישום ה-plug-in השני, **PreOperationQuoteLineDetail**. עבור יישום plug-in זה, עליך לעדכן את השלב **Update of msdyn_quotelinetransaction**.
9. סגור את **PluginRegistrationTool**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]