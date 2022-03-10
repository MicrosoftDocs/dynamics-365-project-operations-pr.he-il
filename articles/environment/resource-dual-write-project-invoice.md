---
title: שילוב חשבונית פרויקט
description: נושא זה מספק מידע על שילוב כתיבה כפולה עבור יצירת חשבוניות ב- Project Operations.
author: sigitac
ms.date: 04/26/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 37549080d76e3bffd7cb002aee8e3c46b9eeb18e3cec915cd971881b69747534
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 08/06/2021
ms.locfileid: "6993242"
---
# <a name="project-invoice-integration"></a>שילוב חשבונית פרויקט

נושא זה מספק מידע על שילוב כתיבה כפולה עבור יצירת חשבוניות ב- Project Operations.

ב-Project Operations מנהל הפרויקט מנהל את צבר חיובי הפרויקט ויוצר חשבונית פרופורמה עבור הלקוח ב- Microsoft Dataverse. בהתבסס על חשבונית פרופורמה זו, פקיד חשבונות חייבים או רואה חשבון פרויקט יוצר חשבונית המוצגת ללקוח. שילוב כתיבה כפולה מבטיח שפרטי חשבונית הפרופורמה מסונכרנים עם יישומי Finance and Operations. לאחר פרסום החשבונית שמוצגת ללקוח, המערכת מעדכנת את נתוני הפרויקט הרלוונטיים ב- Dataverse עם הפרט החשבונאי. הגרפיקה הבאה מספקת סקירה קונספטואלית ברמה גבוהה על שילוב זה.

   ![שילוב חשבונית פרוייקט.](./media/DW5Invoicing.png)

לאחר שמנהל הפרויקט מאשר את חשבונית הפרופורמה ב- Dataverse, המידע בכותרת חשבונית פרופורמה מסתנכרן עם ישומי Finance and Operations המשתמשות במפת טבלת הכתיבה הכפולה, **הצעת חשבונית פרויקט גרסה 2 (חשבוניות)**. זהו שילוב חד כיווני מ- Dataverse לישומי Finance and Operations. יצירה או מחיקה של הצעות חשבוניות לפרויקט ישירות בישומי Finance and Operations אינן נתמכות.

אישור חשבונית ב- Dataverse מפעיל גם את ההיגיון העסקי ליצירת רשומות הקשורות לחיוב בישות **נתונים בפועל**. רשומות של נתונים בפועל מסונכרנות עם ישומי Finance and Operations באמצעות במפת הטבלת הכתיבה הכפולה **נתוני שילוב בפועל של Project Operations ‏(msdyn\_actuals)**. לקבלת מידע נוסף, ראה [הערכות ונתונים בפועל של פרויקט](resource-dual-write-estimates-actuals.md). 

שורות הצעת חשבונית לפרויקט נוצרות על ידי התהליך התקופתי **ייבוא אחסון זמני של טפסים**. תהליך זה מבוסס על פרטי נתוני המכירות בפועל המחויבים בטבלה **אחסון זמני של נתונים בפועל**. למידע נוסף ראה [ניהל הצעות חשבונית לפרויקט](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals). 
