---
title: שאלות נפוצות בנושא ניהול משאבים
description: נושא זה מספק תשובות לשאלות נפוצות לגבי ניהול משאבים.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: fdf7f1e2-e4a2-4c68-aa03-4a41c7b10531
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 87da759b3b30ed6d38866c045194cde79837c209
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751857"
---
# <a name="resource-management-faq"></a>שאלות נפוצות בנושא ניהול משאבים

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

## <a name="what-is-the-difference-between-a-team-member-and-a-resource-requirement"></a>מה ההבדל בין חבר צוות לדרישת משאב?

ניתן להקצות חבר צוות של פרוייקט למשימות שהוזמנו או למשימות בהזמנת יתר, ולהגדיר אותו כמאשר. דרישת משאב יכולה להתקיים ללא חבר צוות של פרוייקט, כטיוטה של דרישה. 

## <a name="what-is-the-difference-between-proposed-and-soft-booked-hours"></a>מה ההבדל בין שעות מוצעות לשעות בהזמנה טנטטיבית?

שעות מוצעות ושעות בהזמנה טנטטיבית שונות בניראות שלהן. שעות מוצעות גלויות אך ורק למנהלי משאבים ולמנהל הפרוייקט שיזם את הדרישה באמצעות בקשת משאב. שעות בהזמנה טנטטיבית גלויות לכל מי שיש לו גישה ללוח הזמנים.

## <a name="how-can-i-see-the-soft-booked-hours-for-resources-on-a-team"></a>כיצד ניתן לראות את שעות ההזמנה הטנטטיבית עבור משאבים בצוות?

ניתן ליצור הזמנות טנטטיביות בעת הזמנה של דרישת משאב. משאבים המוזמנים בהזמנה טנטטיבית בצוות פרוייקט מופיעים כחברי צוות בעלי שעות הזמנה טנטטיבית. הם גם מופיעים בלוח הזמנים.

## <a name="how-do-i-change-the-required-hours-and-the-start-and-end-dates-for-a-resource-generic-or-named-that-i-booked"></a>כיצד ניתן לשנות את השעות הנדרשות ואת תאריכי ההתחלה והסיום, עבור משאב (כללי או בעל שם) שהזמנתי?

לאחר הזמנת משאבים, בחר **השאר את ההזמנות** כדי לבצע כל שינוי נדרש.

## <a name="what-resources-types-does-project-service-automation-support"></a>באילו סוגי משאבים תומך Project Service Automation?

**משתמש** ו**איש קשר** הם סוגי המשאבים היחידים הנתמכים ב- Dynamics 365 Project Service Automation. על אף שניתן ליצור סוגים אחרים של משאבים (לדוגמה, **ציוד** ו**קבוצה**), הם לא תומכים במקרי שימוש מקצה לקצה.

## <a name="what-is-the-difference-between-an-assignment-and-a-booking"></a>מה ההבדל בין הקצאה להזמנה?

הקצאות הן הקצאה של משאבים למשימות פרוייקט בלוח הזמנים של הפרוייקט. המשאבים יכולים להיות משאבים אמיתיים או משאבים כלליים. הזמנות הן הקצאה בטוחה או טנטטיבית של משאבים לפרוייקט. הזמנות בטוחות צורכות קיבולת של משאב. באופן אידיאלי, עבור משאבים אמיתיים, ההזמנות וההקצאות צריכות להתאים, משום שהן לא שונות. עם זאת, PSA אינו אוכף הסכם זה. התצוגה 'התאמה' מציגה בפני מנהל פרוייקט מקומות שבהם הזמנות וההקצאות של משאב אינן תואמות.
