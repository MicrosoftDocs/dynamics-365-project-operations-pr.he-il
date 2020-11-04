---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 17 V3
description: נושא זה מפרט את התכונות החדשות והתיקונים במהדורה 17, עדכון V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 03/06/2020
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 7ba685568692dafe117de42a71bb14d391cd7cc4
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077264"
---
# <a name="project-service-automation-update-release-17-v3"></a>מהדורה 17, V3 של Project Service Automation

אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.  מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 17, עדכון V3 של PSA. מספר גירסת build של גרסה זו הוא V3.10.6.34 ובדרך כלל היא זמינה באמצעות עדכון עצמי החל ממרץ 2020.


## <a name="update-release-17"></a>הפצת עדכון 17

### <a name="bug-fixes"></a>תיקוני באגים

**כללי**

- תוקן: עדכן את Project Service Automation כדי לאכוף רישיונות של חברי צוות (Project Resource Hub יכלול מטא-נתונים 3.x על תוכנית השירות של חברי הצוות).
 
**זמן והוצאה**

- תוקן: לא ניתן לשנות הערכת הוצאה ממחיר שאינו אפס לאפס (0). ניסיון לשינוי לא יבוצע.

**ניהול פרויקט**

- תוקן: נוספה בדיקת ערכי null לשם המשרה של חבר הצוות.
- תוקן: נמחק שדה **msdyn_userresid** בישות **‎msdyn_resourceassignment**.
- תוקן: שדרוג מ- 2.x ל- 3.x כעת מטפל בפעולות מתאר ריקות בהקצאת משימות.

**Sales**

- תוקן: **Invoice.PreValidateInvoiceUpdate** כעת מטפל כראוי בתרחיש של הקצאת בעלי תיעוד מחדש.
- תוקן: כאשר מחלקת העסקה היא **זמן** , **UnitGroup** אינו ניתן לעריכה לכל הישויות כולל, **QuoteLineDetails** , **JournalLine** , **InvoiceLineDetail** , ו **ContractLineDetails**. למרות זאת, **Unit** אינו ניתן לעריכה רק עבור **JournalLine** ו **InvoiceLineDetails**.

