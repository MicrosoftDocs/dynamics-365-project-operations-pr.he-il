---
title: שילוב כתיבה כפולה של Project Operations
description: נושא זה מספק מבט על של שילוב כתיבה כפולה ב- Project Operations.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d9d6a7c367872219b4aca32aecb15d6837ebe296
ms.sourcegitcommit: 02f00960198cc78a5e96955a9e4390c2c6393bbf
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/28/2021
ms.locfileid: "5955659"
---
# <a name="project-operations-dual-write-integration-overview"></a>מבט על של שילוב כתיבה כפולה ב- Project Operations

_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_

Project Operations משתמש ב[יכולות כתיבה כפולה](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) כדי לסנכרן נתונים ב- Microsoft Dataverse ו- Dynamics 365 Finance.

האיור הבא מראה כיצד נתונים מסונכרנים כחלק משילוב זה בין Dataverse ו- Finance.

![מבט כולל על זרימות נתונים ב- Project Operations](./media/ProjectOperationsFlows.jpg)

Project Operations ב- Dataverse מספק ממשק משתמש (UI) מודרני שניתן להרחבה בקלות ללא קוד או עם מעט קוד באמצעות יכולות Power Platform. מנהלי פרויקטים, מנהלי משאבים, אנשי צוות פרוייקטים משתמשי משרד חזיתי אחרים, מבצעים את פעולותיהם ב- Project Operations ב- Dataverse.

Project Operations ב- Finance מספקת תמיכה בחשבונאות פרויקט ובהכרת הכנסות. Project Operations מתחברות למסגרת הפיננסית ב- Finance לצורך חישוב מע"מ, שערי חליפין, דיווח מימד פיננסי ועוד. חוויות רואה החשבון הפרויקט נמצאות בעיקר ב- Finance.

שילוב Project Operations מורכב משילוב הרכיבים הבא:


- [שילוב נתוני התקנה ותצורה של Project Operations](resource-dual-write-setup-integration.md) 
- [הערכות ונתונים בפועל של פרויקט](resource-dual-write-estimates-actuals.md)
- [חשבוניות פרוייקט](resource-dual-write-project-invoice.md)
- [ניהול הוצאות](resource-dual-write-expense.md)
- [חשבונית ספק](resource-dual-write-vendor-invoice.md)
