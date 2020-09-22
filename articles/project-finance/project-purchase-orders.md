---
title: הזמנות רכש לפרוייקט
description: מאמר זה מתאר את השיטות השונות שבהן תוכל להשתמש כדי ליצור הזמנות רכש לפרוייקט. השיטה שבה תשתמש תלויה במטרה של הזמנת הרכש ומתי יבוצעו הצריכה והחיוב של הפריטים שנרכשו לפרוייקט.
author: KimANelson
manager: AnnBe
ms.date: 09/14/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 83972
ms.assetid: 247e4d72-610b-4fa5-9873-601ed0f4b2d6
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: a4975b9f9e20906fb1259e36a07d8ef3db4f4fee
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751793"
---
# <a name="purchase-orders-for-a-project"></a>הזמנות רכש לפרוייקט

[!include [banner](../includes/banner.md)]

מאמר זה מתאר את השיטות השונות שבהן תוכל להשתמש כדי ליצור הזמנות רכש לפרוייקט. השיטה שבה תשתמש תלויה במטרה של הזמנת הרכש ומתי יבוצעו הצריכה והחיוב של הפריטים שנרכשו לפרוייקט.

### <a name="methods-for-creating-a-purchase-order"></a>שיטות ליצירת הזמנת רכש

באפשרותך להשתמש באחת מהשיטות הבאות כדי ליצור הזמנת רכש בניהול פרוייקטים וחשבונאות. מטרת הזמנת הרכש קובעת מתי נצרכת הזמנת הרכש, ולפיכך מתי מחויבים פריטים בפרוייקט.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>שיטה</th>
<th>מטרה</th>
<th>צריכת פריטים</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>צור הזמנת רכש באופן ישיר מפרוייקט.</td>
<td>השתמש בשיטה זו כדי לרכוש פריטים מספק חיצוני לצריכה בפרוייקט. ניתן ליצור את הזמנת הרכש בשתי דרכים:
<ul>
<li>מהפרוייקט עצמו. במקרה כזה, הפרוייקט כבר מוגדר להזמנת הרכש.</li>
<li>על ידי ניווט להזמנת הרכש של הפרוייקט. עליך לבחור גם את הספק וגם את הפרוייקט שעבורו תיווצר הזמנת הרכש.</li>
</ul></td>
<td>פריטים נצרכים כאשר חשבונית הספק מתעדכנת.</td>
</tr>
<tr class="even">
<td>צור הזמנת רכש מהזמנת מכירות.</td>
<td>השתמש בשיטה זו כדי לרכוש פריטים בעת יצירת הזמנת מכירות מפרוייקט.</td>
<td>פריטים נצרכים כאשר מופקת חשבונית עבור הזמנת המכירות ללקוח.</td>
</tr>
<tr class="odd">
<td>צור הזמנת רכש מפריט נדרש.</td>
<td>השתמש בשיטה זו כדי לרכוש פריטים בעת יצירת פריט נדרש מפרוייקט.</td>
<td>פריטים נצרכים בעת עדכון תעודת משלוח לפריט נדרש.</td>
</tr>
</tbody>
</table>

> [!NOTE] 
> בעת עדכון חשבונית הספק או תעודת המשלוח, תתבקש לעדכן את תעודת המשלוח בפריט הנדרש.

לקבלת מידע נוסף, ראה [קבלת פריטים בהזמנת רכש מפריט נדרש](tasks/receive-items-purchase-order-item-requirement.md).

