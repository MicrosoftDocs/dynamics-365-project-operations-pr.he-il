---
title: מבט כולל על תהליך הוצאת חשבוניות
description: נושא זה מספק סקירה כללית על הפקת חשבוניות ב- Project Operations עבור תרחישים מבוססי משאבים/ללא מלאי.
author: sigitac
ms.date: 01/29/2021
ms.topic: overview
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 0328d5321909bcc17754da4e19d7652b77a665d5
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8582711"
---
# <a name="invoicing-process-overview"></a>מבט כולל על תהליך הוצאת חשבוניות

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

Project Operations לתרחישים מבוססי משאבים/ללא מלאי מציע יכולות מקיפות המותאמות לצרכים של מנהל הפרוייקט ושל פקיד החשבונות/רואה החשבון של הפרוייקט. בתהליך הפקת החשבונית מנהל הפרוייקט מנהל את צבר החיובים בפרוייקט ומנהל החשבונות/החשב של הפרוייקט יוצר מסמך חשבוניות תואם ומדויק שמיועד ללקוח.

![תרשים זרימה של הפקת חשבונית.](./media/invoicing-flow.png)

סעיף חוזה הפרוייקט מגדיר את שיטת החיוב עבור עסקאות פרוייקט משויכות. כאשר מנהל הפרויקט מאשר עסקאות זמן והוצאות, המערכת מתעדת את העסקאות ביישות **נתונים בפועל של הפרויקט** ושולחת את המידע למודול **ניהול פרויקטים וחשבונאות** ב- Dynamics 365 Finance. חשב הפרוייקט סוקר ומפרסם את הרשומות באמצעות [יומן השילוב של Project Operations](../project-accounting/project-operations-integration-journal.md). יומן זה כולל פרטים חשבונאיים חשובים עבור הנתונים בפועל של הפרוייקט, כגון חיוב, קבוצת מס מכירה, קבוצת מס מכירות של פריטי חיוב וממדים פיננסיים.

מנהל הפרוייקט יכול לבדוק עסקאות מכירה שלא בוצעו באמצעות שיטת החיוב בזמן ובחומר ב- [מצבור חיובי זמן וחומר](../proforma-invoicing/manage-billing-backlog.md#time-and-material-billing-backlog) וחיוב במחיר קבוע ב- [אבני דרך של מחיר קבוע](../proforma-invoicing/manage-billing-backlog.md#fixed-price-milestones). תצוגות אלו מאפשרות לך לסנן ולבחור עסקאות שצריכות להיכלל במחזור החיוב הבא ואז לסמן אותן **מוכנות לחשבונית**.

אתה יכול [ליצור ידנית חשבונית פרופורמה](../proforma-invoicing/create-manual-proforma-invoice.md) או להשתמש ב- [תהליך תקופתי](../proforma-invoicing/configure-automated-invoice-creation.md). מנהל הפרוייקט יכול [להתאים טיוטת חשבונית פרופורמה](../proforma-invoicing/manage-proforma-invoice.md) לפי הצורך ואז לאשר זאת.

חשבונית הפרופורמה שאושרה נשלחת למודול **ניהול פרוייקטים וחשבונאות** ב- Finance. רואה החשבון של הפרוייקט מעצב ומעדכן את הצעת חשבונית הפרוייקט, ואז מפרסם ומדפיס את המסמך. חשבוניות פרוייקט שפורסמו נרשמות בספר החשבונות הכללי, וכן בספרי המשנה של הלקוח ושל הפרוייקט.


[!INCLUDE[footer-include](../includes/footer-banner.md)]