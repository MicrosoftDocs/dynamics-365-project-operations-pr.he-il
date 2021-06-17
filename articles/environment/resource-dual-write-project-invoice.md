---
title: שילוב חשבונית פרויקט
description: נושא זה מספק מידע על שילוב כתיבה כפולה עבור יצירת חשבוניות ב- Project Operations.
author: sigitac
ms.date: 04/26/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7407c98aad79806dcbaf25e81ff3e08397b41ffe
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996567"
---
# <a name="project-invoice-integration"></a>שילוב חשבונית פרויקט

נושא זה מספק מידע על שילוב כתיבה כפולה עבור יצירת חשבוניות ב- Project Operations.

ב-Project Operations מנהל הפרויקט מנהל את צבר חיובי הפרויקט ויוצר חשבונית פרופורמה עבור הלקוח ב- Microsoft Dataverse. בהתבסס על חשבונית פרופורמה זו, פקיד חשבונות חייבים או רואה חשבון פרויקט יוצר חשבונית המוצגת ללקוח. שילוב כתיבה כפולה מבטיח שפרטי חשבונית הפרופורמה מסונכרנים עם יישומי Finance and Operations. לאחר פרסום החשבונית שמוצגת ללקוח, המערכת מעדכנת את נתוני הפרויקט הרלוונטיים ב- Dataverse עם הפרט החשבונאי. הגרפיקה הבאה מספקת סקירה קונספטואלית ברמה גבוהה על שילוב זה.

   ![שילוב חשבונית פרויקט](./media/DW5Invoicing.png)

לאחר שמנהל הפרויקט מאשר את חשבונית הפרופורמה ב- Dataverse, המידע בכותרת חשבונית פרופורמה מסתנכרן עם ישומי Finance and Operations המשתמשות במפת טבלת הכתיבה הכפולה, **הצעת חשבונית פרויקט גרסה 2 (חשבוניות)**. זהו שילוב חד כיווני מ- Dataverse לישומי Finance and Operations. יצירה או מחיקה של הצעות חשבוניות לפרויקט ישירות בישומי Finance and Operations אינן נתמכות.

אישור חשבונית ב- Dataverse מפעיל גם את ההיגיון העסקי ליצירת רשומות הקשורות לחיוב בישות **נתונים בפועל**. רשומות של נתונים בפועל מסונכרנות עם ישומי Finance and Operations באמצעות במפת הטבלת הכתיבה הכפולה **נתוני שילוב בפועל של Project Operations ‏(msdyn\_actuals)**. לקבלת מידע נוסף, ראה [הערכות ונתונים בפועל של פרויקט](resource-dual-write-estimates-actuals.md). 

שורות הצעת חשבונית לפרויקט נוצרות על ידי התהליך התקופתי **ייבוא אחסון זמני של טפסים**. תהליך זה מבוסס על פרטי נתוני המכירות בפועל המחויבים בטבלה **אחסון זמני של נתונים בפועל**. למידע נוסף ראה [ניהל הצעות חשבונית לפרויקט](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals). 
