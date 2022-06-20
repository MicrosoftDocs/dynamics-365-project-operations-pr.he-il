---
title: יצירת תבנית שעות עבודה
description: מאמר זה מתאר את אופן יצירת תבנית שעות עבודה ב- Project Service
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: 8f3ac17a29e79f86f7c3ce127edb4b02ca63ea04
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8916059"
---
# <a name="create-a-work-hours-template-project-service"></a>יצירת תבנית שעות עבודה (Project Service)

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-3x.md)]

כדי ליצור ולנהל פרויקט, עליך להחיל תבנית לוח שנה על הפרויקט. תבנית לוח השנה מגדירה את התכונות הבאות של הפרויקט:

- שעות עבודה, כולל שעת התחלה וסיום
- ימי עבודה
- חריגים ביומן כגון ימים שאינם ימי עבודה

תבנית לוח השנה המוחלת על פרויקט היא העתק של תבנית לוח השנה המוגדרת בהגדרות הארגון שלך.

> [!NOTE]
> אם תשנה את תבנית לוח השנה, שינויים אלה אינם מופצים לשעות העבודה של הפרויקט. כדי לשנות את שעות העבודה של הפרויקט, יש להחיל תבנית חדשה.

כדי ליצור תבנית לוח שנה לארגון שלך, ישנן שתי דרישות עיקריות:

- הגדר את שעות העבודה הרצויות של התבנית באמצעות משאב חדש או קיים שניתן להזמנה.
- צור תבנית לוח שנה חדשה ושייך את התבנית למשאב שניתן להזמינה.

**הגדרת שעות העבודרה של התבנית**

1. עבור אל **משאבים** \> **משאבים**.
2. צור משאב חדש להפניה בתבנית לוח השנה, או בחר משאב קיים.
3. בחר את הכרטיסיה **שעות עבודה** של המשאב והשלם את ההוראות בהסבר: [הגדרת שעות עבודה עבור משאב](/dynamics365/field-service/set-work-hours-resource) כדי להגדיר את כללי לוח השנה.

**צור תבנית לוח שנה חדשה**

1. עבור אל **הגדרות** \> **תבנית לוח שנה**.
2. בחר **חדש** והזן שם, תיאור תבנית משאב.


> [!NOTE]
> כאשר משאב כולל בהפניה בתבנית לוח שנה, עותק של לוח השנה של המשאב משויך לתבנית לוח השנה. אם ישונו שעות העבודה של תבנית לוח השנה שהועתקה, שינויים אלה אינם מופצים לשעות העבודה של תבנית לוח השנה.


### <a name="see-also"></a>למידע נוסף  
 [הגדרת משאבים](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
