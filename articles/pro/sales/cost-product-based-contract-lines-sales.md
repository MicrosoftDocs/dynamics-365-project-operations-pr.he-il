---
title: סעיפי חוזה מבוססי מוצר של עלות - לייט
description: נושא זה מספק מידע אודות יצירת
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 001b0b54abcdd5fcd1eca7f3271cc78392f68860
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5273694"
---
# <a name="cost-product-based-contract-lines---lite"></a>סעיפי חוזה מבוססי מוצר של עלות - לייט

_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_


סעיפי חוזה שמבוססים על מוצר ב- Dynamics 365 Project Operations כוללים את השדה **מחיר עלות**, המאחסן את מחיר העלות של המוצר לצורך חישובי רווחיות במורד הזרם.

כאשר נוצר סעיף חוזה שמבוסס על מוצר עבור מוצר קטלוג, עלות הסעיף היא ברירת המחדל מהשדה **מחיר רגיל** בקטלוג המוצרים. השדה **עלות סטנדרטית** שבקטלוג המוצרים מוגדר במטבע הבסיס של הארגון. כאשר ברירת המחדל של עלות היחידה נקבעת בסעיף החוזה, היא מומרת למטבע המכירות בחוזה.

## <a name="unit-cost-on-a-product-based-contract-line"></a>עלות יחידה בסעיף חוזה מבוסס מוצר

כאשר סעיף חוזה מבוסס מוצר כולל עלות יחידה, מתאפשרות עלויות מוצר שונות עבור כל מכירה של יחידה. אמנם לא תמיד הכרחי, אך ישנם תרחישים מסוימים שבהם הספק עשוי להוזיל את עלות המוצר עבור הלקוח. לפניך התרחיש הבא:

Fabrikam Robotics מתקין זרועות רובוטיות בקווי הייצור של חברת Adatum. Fabrikam מספקת שירותי התקנה אך הזרועות הרובוטיות הן של Trey Research. אם התקנת הזרועות הרובוטיות בחברת Adatum תפתח קהילה אנכית חדשה עבור הזרועות הרובוטיות של Trey, היא עשויה להעניק ל-Fabrikam הנחה מיוחדת על עסקה זו. במקרה זה, Fabrikam יוצר סעיף חוזה מבוסס מוצרים עבור Robotic Arms. עלות ליחידה מוזנת עבור חוזה זה. העלות שונה מעלות הזרועות הרובוטיות מ- Robotic Arms.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]