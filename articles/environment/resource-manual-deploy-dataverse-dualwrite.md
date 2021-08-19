---
title: פריסה ידנית של אפליקציית Dataverse ‏Project Operations עם תמיכה בכתיבה כפולה
description: נושא זה מסביר כיצד לפרוס ידנית את האפליקציה Dataverse של Project Operations כך שהיא תתמוך בכתיבה כפולה.
author: stsporen
ms.date: 06/18/2021
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 06325a9a9f9084d1f506f2493c32565fe7b7c52ae6fe22c81339b9c1d632e688
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/06/2021
ms.locfileid: "6986447"
---
# <a name="manually-deploy-the-project-operations-dataverse-app-with-dual-write-support"></a>פריסה ידנית של אפליקציית Dataverse ‏Project Operations עם תמיכה בכתיבה כפולה

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

נושא זה מסביר כיצד לפרוס ידנית את Microsoft Dynamics 365 Project Operations ב- Microsoft Dataverse כך שהיא תתמוך בכתיבה כפולה. Project Operations מזהה את תצורת הסביבה ומוסיף תמיכה בכתיבה כפולה אם מתקיימים התנאים המוקדמים.

במהלך פריסה דרך Microsoft Dynamics Lifecycle Services (LCS), אם בצעת את ההנחיות בנושא זה, תוכל לדלג על הפריסה של שילוב Microsoft Power Platform (נקראה קודם סביבת Common Data Service).

לתהליך הפרידה של Project Operations ב- Dataverse לצורך תמיכה בכתיבה כפולה יש ארבעה שלבים עיקריים:

1. [צור סביבה חדשה ב- Dataverse התומכת בכתיבה כפולה](#create).
2. [הוסף תנאים מוקדמים לכתיבה כפולה לסביבה](#prerequisites).
3. [הוסף את אפליקציית Project Operations Dataverse](#dataverse).
4. [קשר אל הסביבות שלך](#link).

## <a name="create-a-new-environment-in-dataverse-that-supports-dual-write"></a><a name="create"></a>צור סביבה חדשה ב- Dataverse התומכת בכתיבה כפולה

להשלמת הליך זה, עליך להתחבר כמנהל מערכת.

1. פתח את [מרכז הניהול של Power Platform](https://admin.powerplatform.com) והיכנס כמנהל מערכת.
2. צור סביבה חדשה ותן לה שם.
3. בחר את סוג הסביבה. אם נרשמת לגירסת הניסיון, בחר **גירסת ניסיון (מבוסס מנוי)**.
4. אשר את אזור הפריסה.
5. הפעל את האפשרות **צור מסד נתונים עבור סביבה זו**. 
6. אשר את השפה ולאחר מכן אשר שהמטבע תואם למטבע של יישומי Finance and Operations.
7. הפעל את האפשרות **יישומי Dynamics 365**, ואשר שהשדה **פרוס יישומים אלה באופן אוטומטי** מוגדר **אף אחד**.
8. הוסף קבוצת אבטחה אם נדרשת קבוצת אבטחה.
9. בחר **שמור** כדי ליצור סביבה חדשה.
10. המתן עד להשלמת הפריסה כך שהסביבה מגיעה למצב **מוכן**.

## <a name="add-dual-write-prerequisites-to-the-environment"></a><a name="prerequisites"></a>הוסף תנאים מוקדמים לכתיבה כפולה לסביבה

תמיכה בכתיבה כפולה כוללת שדות נוספים שמתווספים לישויות מפתח, כמו הישות **חברה**. אם אתה מוסיף תמיכה בכתיבה כפולה לסביבה קיימת, ייתכן שיהיה עליך לעדכן את הנתונים כדי לאפשר את התמיכה. למידע על אופן האתחול של הנתונים, ראה [נתוני חברת Bootstrap](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data). למידע נוסף על כתיבה כפולה, ראה [דרישות מערכת לכתיבה כפולה](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req).

השלם הליך זה כדי להוסיף את התנאים המוקדמים לכתיבה כפולה לסביבה שלך.

1. פתח את הסביבה שיצרת זה עתה, ועבור אל **משאב** \> **יישומי Dynamics 365**.
2. בחר **פתרון ליבה של כתיבה כפולה** ברשימת האפליקציות והתקן אותו.
3. המתן עד לסיום ההתקנה. בחר **פתרון התיאום של הכתיבה הכפולה** ברשימת האפליקציות והתקן אותו.

## <a name="add-the-project-operations-dataverse-app"></a><a name="dataverse"></a>הוסף את אפליקציית Dataverse של Project Operations

ניתן להשלים הליך זה רק אם השלמת את השלבים הקודמים לפני שהתקנת את Project Operations. במהלך ההתקנה, המערכת מנתחת את תצורת הסביבה ומוסיפה תמיכה בכתיבה כפולה אם היא נדרשת.

1. פתח את הסביבה שיצרת, ועבור אל **משאב** \> **יישומי Dynamics 365**.
2. בחר **Microsoft Dynamics 365 Project Operations** ברשימת האפליקציות והתקן אותה.

## <a name="link-your-environments"></a><a name="link"></a>קשר אל הסביבות שלך

לאחר הפריסה של סביבת Dataverse, אתה יכול להגדיר את הקישור לאפליקציות Finance and Operations. בצע את השלבים במקטע [השתמש באשף הכתיבה הכפולה לקישור הסביבות שלך](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment).
