---
title: שילוב חשבונית פרויקט
description: מאמר זה מספק מידע על שילוב הפקת חשבוניות לקוח ב- Project Operations באמצעות כתיבה כפולה.
author: sigitac
ms.date: 04/26/2021
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 5ee2d78f1ca1d78f6909d9995a92ac301f06d6a6
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912103"
---
# <a name="project-invoice-integration"></a>שילוב חשבונית פרויקט

מאמר זה מספק מידע על שילוב הפקת חשבוניות לקוח ב- Project Operations באמצעות כתיבה כפולה.

ב-Project Operations מנהל הפרויקט מנהל את צבר חיובי הפרויקט ויוצר חשבונית פרופורמה עבור הלקוח ב- Microsoft Dataverse. בהתבסס על חשבונית פרופורמה זו, פקיד חשבונות חייבים או רואה חשבון פרויקט יוצר חשבונית המוצגת ללקוח. שילוב של כתיבה כפולה מוודא שפרטי חשבונית הפרופורמה יסונכרנו ביישומי Finance and Operations. לאחר פרסום החשבונית שמוצגת ללקוח, המערכת מעדכנת את נתוני הפרויקט הרלוונטיים ב- Dataverse עם הפרט החשבונאי. הגרפיקה הבאה מספקת סקירה קונספטואלית ברמה גבוהה על שילוב זה.

   ![שילוב חשבונית פרוייקט.](./media/DW5Invoicing.png)

לאחר שמנהל הפרוייקט יאשר את חשבונית הפרופורמה ב- Dataverse, פרטי הכותרת של חשבונית הפרופורמה יסונכרנו עם יישומי Finance and Operations באמצעות מפת הטבלה בכתיבה כפולה, **הצעת חשבונית פרוייקט V2 (חשבוניות)**. זהו שילוב חד-כיווני מ- Dataverse ליישומי Finance and Operations. אין תמיכה ביצירה או מחיקה של הצעות חשבונית פרוייקט ישירות ביישומי Finance and Operations.

אישור חשבונית ב- Dataverse מפעיל גם את ההיגיון העסקי ליצירת רשומות הקשורות לחיוב בישות **נתונים בפועל**. רשומות אלה מסונכרנות עם Finance and Operations באמצעות מפת הטבלה בכתיבה כפולה, **נתונים בפועל של שילוב Project Operations‏ (msdyn\_actuals)**. לקבלת מידע נוסף, ראה [הערכות ונתונים בפועל של פרויקט](resource-dual-write-estimates-actuals.md). 

שורות הצעת חשבונית לפרויקט נוצרות על ידי התהליך התקופתי **ייבוא אחסון זמני של טפסים**. תהליך זה מבוסס על פרטי נתוני המכירות בפועל המחויבים בטבלה **אחסון זמני של נתונים בפועל**. למידע נוסף ראה [ניהל הצעות חשבונית לפרויקט](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals). 
