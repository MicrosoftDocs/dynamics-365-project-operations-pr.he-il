---
title: מבט כולל על תהליך הוצאת חשבוניות
description: נושא זה מספק סקירה כללית על הפקת חשבוניות ב- Project Operations עבור תרחישים מבוססי משאבים/ללא מלאי.
author: sigitac
manager: Annbe
ms.date: 01/29/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: fbc1519b6cbcf231cfa89df8b7843d11a8904e49
ms.sourcegitcommit: b4298ca4729643c1040ef35dde8c67f829461ce7
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 01/29/2021
ms.locfileid: "5089247"
---
# <a name="invoicing-process-overview"></a>מבט כולל על תהליך הוצאת חשבוניות

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

Project Operations לתרחישים מבוססי משאבים/ללא מלאי מציע יכולות מקיפות המותאמות לצרכים של מנהל הפרוייקט ושל פקיד החשבונות/רואה החשבון של הפרוייקט. בתהליך הפקת החשבונית מנהל הפרוייקט מנהל את צבר החיובים בפרוייקט ומנהל החשבונות/החשב של הפרוייקט יוצר מסמך חשבוניות תואם ומדויק שמיועד ללקוח.

![תרשים זרימה של הפקת חשבונית](./media/invoicing-flow.png)

סעיף חוזה הפרוייקט מגדיר את שיטת החיוב עבור עסקאות פרוייקט משויכות. כאשר מנהל הפרוייקט מאשר עסקאות זמן והוצאות, המערכת רושמת את העסקאות בישות **פרוייקטים אמיתיים** ושולחת את המידע אל המודול **ניהול פרוייקטים וחשבונאות** ב- Dynamics 365 Finance. חשב הפרוייקט סוקר ומפרסם את הרשומות באמצעות [יומן השילוב של Project Operations](../project-accounting/project-operations-integration-journal.md). יומן זה כולל פרטים חשבונאיים חשובים עבור הנתונים בפועל של הפרוייקט, כגון חיוב, קבוצת מס מכירה, קבוצת מס מכירות של פריטי חיוב וממדים פיננסיים.

מנהל הפרוייקט יכול לבדוק עסקאות מכירה שלא בוצעו באמצעות שיטת החיוב בזמן ובחומר ב- [מצבור חיובי זמן וחומר](../proforma-invoicing/manage-billing-backlog.md#time-and-material-billing-backlog) וחיוב במחיר קבוע ב- [אבני דרך של מחיר קבוע](../proforma-invoicing/manage-billing-backlog.md#fixed-price-milestones). תצוגות אלו מאפשרות לך לסנן ולבחור עסקאות שצריכות להיכלל במחזור החיוב הבא ואז לסמן אותן **מוכנות לחשבונית**.

אתה יכול [ליצור ידנית חשבונית פרופורמה](../proforma-invoicing/create-manual-proforma-invoice.md) או להשתמש ב- [תהליך תקופתי](../proforma-invoicing/configure-automated-invoice-creation.md). מנהל הפרוייקט יכול [להתאים טיוטת חשבונית פרופורמה](../proforma-invoicing/manage-proforma-invoice.md) לפי הצורך ואז לאשר זאת.

חשבונית הפרופורמה שאושרה נשלחת למודול **ניהול פרוייקטים וחשבונאות** ב- Finance. רואה החשבון של הפרוייקט מעצב ומעדכן את הצעת חשבונית הפרוייקט, ואז מפרסם ומדפיס את המסמך. חשבוניות פרוייקט שפורסמו נרשמות בספר החשבונות הכללי, וכן בספרי המשנה של הלקוח ושל הפרוייקט.
