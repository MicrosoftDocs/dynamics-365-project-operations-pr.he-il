---
title: הזמנות רכש לפרויקט
description: מאמר זה מתאר את השיטות השונות שבהן תוכל להשתמש כדי ליצור הזמנות רכש לפרויקט. השיטה שבה תשתמש תלויה במטרה של הזמנת הרכש ומתי יבוצעו הצריכה והחיוב של הפריטים שנרכשו לפרויקט.
author: Yowelle
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
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: bd891aec5bcab66c5801a5d9ca8abbbf632d662d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077296"
---
# <a name="purchase-orders-for-a-project"></a>הזמנות רכש לפרויקט

[!include [banner](../includes/banner.md)]

מאמר זה מתאר את השיטות השונות שבהן תוכל להשתמש כדי ליצור הזמנות רכש לפרויקט. השיטה שבה תשתמש תלויה במטרה של הזמנת הרכש ומתי יבוצעו הצריכה והחיוב של הפריטים שנרכשו לפרויקט.

### <a name="methods-for-creating-a-purchase-order"></a>שיטות ליצירת הזמנת רכש

באפשרותך להשתמש באחת מהשיטות הבאות כדי ליצור הזמנת רכש בניהול פרויקטים וחשבונאות. מטרת הזמנת הרכש קובעת מתי נצרכת הזמנת הרכש, ולפיכך מתי מחויבים פריטים בפרויקט.

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
<td>צור הזמנת רכש באופן ישיר מפרויקט.</td>
<td>השתמש בשיטה זו כדי לרכוש פריטים מספק חיצוני לצריכה בפרויקט. ניתן ליצור את הזמנת הרכש בשתי דרכים:
<ul>
<li>מהפרויקט עצמו. במקרה כזה, הפרויקט כבר מוגדר להזמנת הרכש.</li>
<li>על ידי ניווט להזמנת הרכש של הפרויקט. עליך לבחור גם את הספק וגם את הפרויקט שעבורו תיווצר הזמנת הרכש.</li>
</ul></td>
<td>פריטים נצרכים כאשר חשבונית הספק מתעדכנת.</td>
</tr>
<tr class="even">
<td>צור הזמנת רכש מהזמנת מכירות.</td>
<td>השתמש בשיטה זו כדי לרכוש פריטים בעת יצירת הזמנת מכירות מפרויקט.</td>
<td>פריטים נצרכים כאשר מופקת חשבונית עבור הזמנת המכירות ללקוח.</td>
</tr>
<tr class="odd">
<td>צור הזמנת רכש מפריט נדרש.</td>
<td>השתמש בשיטה זו כדי לרכוש פריטים בעת יצירת פריט נדרש מפרויקט.</td>
<td>פריטים נצרכים בעת עדכון תעודת משלוח לפריט נדרש.</td>
</tr>
</tbody>
</table>

> [!NOTE] 
> בעת עדכון חשבונית הספק או תעודת המשלוח, תתבקש לעדכן את תעודת המשלוח בפריט הנדרש.

לקבלת מידע נוסף, ראה [קבלת פריטים בהזמנת רכש מפריט נדרש](tasks/receive-items-purchase-order-item-requirement.md).
