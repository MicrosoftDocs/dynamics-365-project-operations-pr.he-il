---
title: עדכון תכונות של יישום Plug-in כדי לכלול ממדי תמחור חדשים
description: נושא זה מספק מידע על עדכון תכונות של יישום Plug-in עבור ממדי תמחור.
author: Rumant
manager: kfend
ms.custom: ''
ms.date: 11/19/2018
ms.topic: article
ms.service: dynamics-365-customerservice
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: f215555dd7b29444e00499c0e731624e51057250
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077391"
---
# <a name="update-plug-in-attributes-to-include-new-pricing-dimensions"></a>עדכון תכונות של יישום Plug-in כדי לכלול ממדי תמחור חדשים

> [!NOTE]
> אם אינך משתמש בתכונות 'יצירת הצעת מחיר' ו'חוזה' של Project Service Automation ‏(PSA), אתה מוזמן לדלג על נושא זה.

נושא זה יוצא מנקודת הנחה שהשלמת את ההליכים בנושאים [יצירת שדות וישויות מותאמים אישית](create-custom-fields-entities.md), [הוספת שדות מותאמים אישית להגדרת מחיר וישויות של עסקאות](field-references.md) ו[הגדרת שדות מותאמים אישית כממדי תמחור](set-up-pricing-dimensions.md). אם לא השלמת הליכים אלה, חזור והשלם אותם ולאחר מכן חזור לנושא זה.

בעת יצירת פרט של שורת הצעת מחיר בדף **שורת הצעת מחיר** של שורת הצעת מחיר של פרויקט, המערכת יוצרת שתי שורות הערכה ברקע – שורה אחת עבור צד העלות של ההערכה ושורה אחת עבור צד המכירות. אותה פעולה מתבצעת עבור סעיפי חוזה של פרויקט.

בעת ביצוע שינוי בכמות או בשדה שבצד העלות, השינוי מופץ לצד המכירות. הדבר אפשרי בזכות יישומי ה- Plug-in הבאים שיש לרשום מחדש לאחר כל שינוי בממדי התמחור.

- PreOperationContractLineDetailUpdate - Updates **msdyn_orderlinetransaction**.
- PreOperationQuoteLineDetailUpdate - Updates **msdyn_quotelinetransaction**.

השלבים הבאים מסבירים לך את תהליך הרישום של יישומי ה- Plug-in.

1. פתח את הכלי **PluginRegistrationTool** והתחבר למופע המקוון שלך.
2. לחץ על **חיפוש** וחפש את יישום ה- Plug-in לעדכון.

 ![צילום מסך של עץ החיפוש](media/PRT-1.png)

3. לאחר מציאת יישום ה- Plug-in, בחר אותו ולאחר מכן לחץ על **בחר בטופס הראשי**.

4. בחר את השלב של יישום ה- plug-in לעדכון, לחץ באמצעות לחצן העכבר הימני ולאחר מכן בחר **עדכן**.

 ![צילום מסך של יישום ה- Plug-in לעדכון](media/PRT-2.png)
 
5. בחלון העדכון, לחץ על שלוש הנקודות ( **...** ) בתכונות הסינון.

 ![צילום מסך של פרטי התצורה של עדכון השלב הנוכחי](media/PRT-3.png)
 
6. בחר את תיבות הסימון של תכונות התמחור.

 ![צילום מסך המציג בחירת תיבות סימון של תכונות תמחור](media/PRT-4.png)

7. לחץ על **אישור** כדי לסגור את הדף ולאחר מכן בחר **עדכן שלב**.

 ![צילום מסך המציג את הלחצן 'עדכן שלב'](media/PRT-5.png)
 
8. חזור על תהליך זה עבור יישום ה- Plug-in השני, **PreOperationQuoteLineDetail - Update of msdyn_quotelinetransaction**.

9. סגור את כלי הרישום של יישומי ה- Plug-in.
