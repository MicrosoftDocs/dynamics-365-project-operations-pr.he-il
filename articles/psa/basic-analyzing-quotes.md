---
title: ניתוח של הצעות מחיר לפרוייקט
description: נושא זו מספק מידע אודות הניתוח של הצעות מחיר לפרוייקט.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 0d9cefafcce33297146cae81d9ba7e68ab79aeb6
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077424"
---
# <a name="analysis-of-project-quotes"></a>ניתוח של הצעות מחיר לפרוייקט

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Dynamics 365 Project Service Automation מנתח הצעות מחיר לפרוייקט כדי להעריך רווחיות. הוא מנתח גם באיזו מידה הצעת המחיר מותאמת לציפיות הלקוח לגבי תאריך המסירה או תאריך ההשלמה, ולגבי התקציב.

## <a name="profitability-analysis"></a>ניתוח רווחיות

Project Service Automation מנתח רווחיות באמצעות שולי הרווח הגולמי ושולי הרווי הגולמי המותאמים.

- שולי הרווח הגולמי מחושבים באמצעות הנוסחה הבאה:

  `
    (Sum of estimated chargeable sales value – Sum of estimated chargeable costs) x 100
  `
- שולי הרווח הגולמי המותאמים מחושבים באמצעות הנוסחה הבאה:

  `
    (Sum of estimated chargeable sales value – Sum of all estimated costs) x 100
  `

אם קיים הבדל בין הערכים עבור שולי הרווח הגולמי ושולי הרווח הגולמי המותאמים של שוליים רחבים, רוב העבודה בהצעת המחיר מסווגת כלא לחיוב.

## <a name="analysis-of-customer-expectations"></a>ניתוח של ציפיות הלקוח

באפשרותך לנתח הצעות מחיר וליצור תרשימים עבור ציפיות של לקוחות לגבי לוח הזמנים והתקציב אם תזין ערכים עבור השדות הבאים:

- השדה **תאריך מסירה מבוקש** בכותרת הצעת המחיר.
- השדה **תקציב הלקוח** עבור כל שורת הצעת מחיר (עבור שורות מבוססות-פרוייקט ושורות מבוססות-מוצר).

ניתוח של ציפיות הלקוח לגבי לוח הזמנים מתבצע על-ידי השוואת תאריך הסיום המאוחר ביתר של הפרט בשורת הצעת המחיר לתאריך המסירה המבוקש בכל שורות הצעת המחיר בהצעת המחיר.

ניתוח של ציפיות הלקוח לגבי התקציב מתבצע על-ידי השוואת הסכום של תקציב הלקוח הכולל לסכום המופיע בהצעת המחיר בכל שורות הצעת המחיר.