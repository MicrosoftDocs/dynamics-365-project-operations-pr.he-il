---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 17 V3
description: מאמר זה מפרט את התכונות והתיקונים הזמינים בעדכון Project Service Automation מהדורה 17, גרסה 3.
author: ruhercul
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
ms.reviewer: johnmichalak
ms.openlocfilehash: c8486ef689f0d8ab014c2248fc6e5d0fddc937e7
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8915691"
---
# <a name="project-service-automation-update-release-17-v3"></a>מהדורה 17, V3 של Project Service Automation

[!include [banner](../includes/psa-now-project-operations.md)]

אנו שמחים להכריז על העדכון האחרון של אפליקציית Project Service Automation של Dynamics 365. מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.  מהדורה זו תואמת את Dynamics 365 9.x. כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון. למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](/power-platform/admin/install-remove-preferred-solution).

מאמר זה מפרט את התכונות והתיקונים החדשים או ששונו עבור PSA בגרסה 3, מהדורת עדכון 17. מספר גירסת build של גרסה זו הוא V3.10.6.34 ובדרך כלל היא זמינה באמצעות עדכון עצמי החל ממרץ 2020.


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
- תוקן: כאשר מחלקת העסקה היא **זמן**, **UnitGroup** אינו ניתן לעריכה לכל הישויות כולל, **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail**, ו **ContractLineDetails**. למרות זאת, **Unit** אינו ניתן לעריכה רק עבור **JournalLine** ו **InvoiceLineDetails**.




[!INCLUDE[footer-include](../includes/footer-banner.md)]
