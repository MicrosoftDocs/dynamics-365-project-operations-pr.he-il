---
title: שילוב חשבונית פרויקט
description: נושא זה מספק מידע על שילוב כתיבה כפולה עבור יצירת חשבוניות ב- Project Operations.
author: sigitac
ms.date: 04/26/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 1e7294360f041b030efca225c6754fe3bbc0eadf
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/14/2022
ms.locfileid: "8581239"
---
# <a name="project-invoice-integration"></a>שילוב חשבונית פרויקט

נושא זה מספק מידע על שילוב כתיבה כפולה עבור יצירת חשבוניות ב- Project Operations.

ב-Project Operations מנהל הפרויקט מנהל את צבר חיובי הפרויקט ויוצר חשבונית פרופורמה עבור הלקוח ב- Microsoft Dataverse. בהתבסס על חשבונית פרופורמה זו, פקיד חשבונות חייבים או רואה חשבון פרויקט יוצר חשבונית המוצגת ללקוח. שילוב של כתיבה כפולה מוודא שפרטי חשבונית הפרופורמה יסונכרנו ביישומי Finance and Operations. לאחר פרסום החשבונית שמוצגת ללקוח, המערכת מעדכנת את נתוני הפרויקט הרלוונטיים ב- Dataverse עם הפרט החשבונאי. הגרפיקה הבאה מספקת סקירה קונספטואלית ברמה גבוהה על שילוב זה.

   ![שילוב חשבונית פרוייקט.](./media/DW5Invoicing.png)

לאחר שמנהל הפרוייקט יאשר את חשבונית הפרופורמה ב- Dataverse, פרטי הכותרת של חשבונית הפרופורמה יסונכרנו עם יישומי Finance and Operations באמצעות מפת הטבלה בכתיבה כפולה, **הצעת חשבונית פרוייקט V2 (חשבוניות)**. זהו שילוב חד-כיווני מ- Dataverse ליישומי Finance and Operations. אין תמיכה ביצירה או מחיקה של הצעות חשבונית פרוייקט ישירות ביישומי Finance and Operations.

אישור חשבונית ב- Dataverse מפעיל גם את ההיגיון העסקי ליצירת רשומות הקשורות לחיוב בישות **נתונים בפועל**. רשומות אלה מסונכרנות עם Finance and Operations באמצעות מפת הטבלה בכתיבה כפולה, **נתונים בפועל של שילוב Project Operations‏ (msdyn\_actuals)**. לקבלת מידע נוסף, ראה [הערכות ונתונים בפועל של פרויקט](resource-dual-write-estimates-actuals.md). 

שורות הצעת חשבונית לפרויקט נוצרות על ידי התהליך התקופתי **ייבוא אחסון זמני של טפסים**. תהליך זה מבוסס על פרטי נתוני המכירות בפועל המחויבים בטבלה **אחסון זמני של נתונים בפועל**. למידע נוסף ראה [ניהל הצעות חשבונית לפרויקט](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals). 
