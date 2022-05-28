---
title: שאלות נפוצות בנושא ניהול משאבים
description: נושא זה מספק תשובות לשאלות נפוצות לגבי ניהול משאבים.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
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
ms.openlocfilehash: c8ce1edf7d7c535271fa8076befd26f092fbd495
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8587495"
---
# <a name="resource-management-faq"></a>שאלות נפוצות בנושא ניהול משאבים

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

## <a name="what-is-the-difference-between-a-team-member-and-a-resource-requirement"></a>מה ההבדל בין חבר צוות לדרישת משאב?

ניתן להקצות חבר צוות של פרויקט למשימות שהוזמנו או למשימות בהזמנת יתר, ולהגדיר אותו כמאשר. דרישת משאב יכולה להתקיים ללא חבר צוות של פרויקט, כטיוטה של דרישה. 

## <a name="what-is-the-difference-between-proposed-and-soft-booked-hours"></a>מה ההבדל בין שעות מוצעות לשעות בהזמנה טנטטיבית?

שעות מוצעות ושעות בהזמנה טנטטיבית שונות בניראות שלהן. שעות מוצעות גלויות אך ורק למנהלי משאבים ולמנהל הפרויקט שיזם את הדרישה באמצעות בקשת משאב. שעות בהזמנה טנטטיבית גלויות לכל מי שיש לו גישה ללוח הזמנים.

## <a name="how-can-i-see-the-soft-booked-hours-for-resources-on-a-team"></a>כיצד ניתן לראות את שעות ההזמנה הטנטטיבית עבור משאבים בצוות?

ניתן ליצור הזמנות טנטטיביות בעת הזמנה של דרישת משאב. משאבים המוזמנים בהזמנה טנטטיבית בצוות פרויקט מופיעים כחברי צוות בעלי שעות הזמנה טנטטיבית. הם גם מופיעים בלוח הזמנים.

## <a name="how-do-i-change-the-required-hours-and-the-start-and-end-dates-for-a-resource-generic-or-named-that-i-booked"></a>כיצד ניתן לשנות את השעות הנדרשות ואת תאריכי ההתחלה והסיום, עבור משאב (כללי או בעל שם) שהזמנתי?

לאחר הזמנת משאבים, בחר **השאר את ההזמנות** כדי לבצע כל שינוי נדרש.

## <a name="what-resources-types-does-project-service-automation-support"></a>באילו סוגי משאבים תומך Project Service Automation?

**משתמש** ו **איש קשר** הם סוגי המשאבים היחידים הנתמכים ב- Dynamics 365 Project Service Automation. על אף שניתן ליצור סוגים אחרים של משאבים (לדוגמה, **ציוד** ו **קבוצה**), הם לא תומכים במקרי שימוש מקצה לקצה.

## <a name="what-is-the-difference-between-an-assignment-and-a-booking"></a>מה ההבדל בין הקצאה להזמנה?

הקצאות הן הקצאה של משאבים למשימות פרויקט בלוח הזמנים של הפרויקט. המשאבים יכולים להיות משאבים אמיתיים או משאבים כלליים. הזמנות הן הקצאה בטוחה או טנטטיבית של משאבים לפרויקט. הזמנות בטוחות צורכות קיבולת של משאב. באופן אידיאלי, עבור משאבים אמיתיים, ההזמנות וההקצאות צריכות להתאים, משום שהן לא שונות. עם זאת, PSA אינו אוכף הסכם זה. התצוגה 'התאמה' מציגה בפני מנהל פרויקט מקומות שבהם הזמנות וההקצאות של משאב אינן תואמות.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
