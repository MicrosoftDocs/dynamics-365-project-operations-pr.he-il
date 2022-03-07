---
title: יצירת תבנית שעות עבודה
description: נושא זה מתאר כיצד ליצור תבנית שעות עבודה ב- Project Service.
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
ms.openlocfilehash: 90525cf1e7cd487a03b064466ad1b13f8afb7819443fc4bacf9c7d3eee86f0b6
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/06/2021
ms.locfileid: "6987392"
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
3. בחר את הכרטיסיה **שעות עבודה** של המשאב והשלם את ההוראות בהסבר: [הגדרת שעות עבודה עבור משאב](/dynamics365/field-service/set-work-hours-resource.md) כדי להגדיר את כללי לוח השנה.

**צור תבנית לוח שנה חדשה**

1. עבור אל **הגדרות** \> **תבנית לוח שנה**.
2. בחר **חדש** והזן שם, תיאור תבנית משאב.


> [!NOTE]
> כאשר משאב כולל בהפניה בתבנית לוח שנה, עותק של לוח השנה של המשאב משויך לתבנית לוח השנה. אם ישונו שעות העבודה של תבנית לוח השנה שהועתקה, שינויים אלה אינם מופצים לשעות העבודה של תבנית לוח השנה.


### <a name="see-also"></a>למידע נוסף  
 [הגדרת משאבים](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
