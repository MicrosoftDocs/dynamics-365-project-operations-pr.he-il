---
title: פרמטרי שילוב של Project Service Automation
description: נושא זה מסביר כיצד להגדיר את אופן הזנת הנתונים בברירת מחדל בעת שילוב Microsoft Dynamics 365 for Project Service Automation עם Microsoft Dynamics 365 Finance.
author: ruhercul
manager: AnnBe
ms.date: 03/03/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: ruhercul
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 1a0cee090e0ecb306aa3bda62c79a57dfade93c0
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077448"
---
# <a name="project-service-automation-integration-parameters"></a>פרמטרי שילוב של Project Service Automation

[!include[banner](../includes/banner.md)]

בדף **פרמטרי שילוב של Service Automation** , תוכל להגדיר כיצד נתוני ברירת המחדל יוזנו בעת שילוב Dynamics 365 Project Service Automation עם Dynamics 365 Finance. כדי לסנכרן בהצלחה פרויקטים מ- Project Service Automation ל- Finance, עליך להגדיר את השדות הבאים.

כדי לפתוח את הדף **פרמטרי שילוב של Project Service Automation** , עבור אל **ניהול פרויקטים וחשבונאות** \> **הגדרה** \> **פרמטרי שילוב של Dynamics 365 for Project Service Automation**. 

> [!NOTE]
> - שילוב משימות פרויקט, קטגוריות של עסקאות הוצאות, הערכות לשעות, הערכות להוצאות ונעילת פונקציונליות זמינים בגירסה 8.0.
> - שילוב נתונים בפועל זמין בגירסה 8.0.1 ואילך.


| כרטיסייה                    | שדה                | תיאור |
|------------------------|----------------------|-------------|
| כללי                | סוג פרויקט ברירת מחדל | בחר את סוג פרויקט ברירת המחדל. כאשר פרויקטים מסונכרנים מ- Project Service Automation, נעשה שימוש בערך זה אם לא סיפקת ערך ברירת מחדל בתבנית השילוב. במהלך הסנכרון, השדה **סוג פרויקט** של פרויקטים חדשים מוגדר לערך זה. עם זאת, ייתכן שהערך יעודכן כשסעיפי החוזה של הפרויקט יסונכרנו מ- Project Service Automation. |
|                        | קטגוריית זמן        | בחר את קטגוריית ברירת המחדל של הזמן. ערך זה משמש כאשר הערכות לשעות מסונכרנות מ- Project Service Automation. כשהערכות לשעות ונתונים בפועל לשעות מסונכרנים מ- Project Service Automation, השדה **קטגוריה** של תחזיות השעות בפרויקט החדש ב- Finance מוגדר לערך זה. |
|                        | קטגוריית עמלה         | בחר את קטגוריית ברירת המחדל של העמלה. ערך זה משמש כאשר נתונים בפועל של עמלות מסונכרנים מ- Project Service Automation. כשהנתונים בפועל לעמלות מסונכרנים מ- Project Service Automation, השדה **קטגוריה** של תחזיות העמלות ב- Finance מוגדר לערך זה. |
| ברירות מחדל של קבוצת פרויקטים | סוג פרויקט         | לחץ על **חדש** כדי להוסיף שורה שבה תוכל לבחור את סוג הפרויקט שאליו יש להגדיר את קבוצת הפרויקטים בברירת מחדל. ניתן לבחור סוג פרויקט ספציפי פעם אחת בלבד בתצורה. |
|                        | קבוצת פרויקטים        | בחר את קבוצת הפרויקטים המוגדרת כברירת מחדל עבור סוג הפרויקט שנבחר. כשפרויקטים חדשים מסונכרנים מ- Project Service Automation, השדה **קבוצת פרויקטים** מוגדרת לערך ברירת המחדל עבור סוג הפרויקט אם לא סיפקת ערך ברירת מחדל בתבנית השילוב. |
| ברירות מחדל לסוג חיוב  | סוג חיוב         | לחץ על **חדש** כדי להוסיף שורה שבה תוכל לבחור את סוג החיוב שאליו יש להגדיר את מאפיין השורה בברירת מחדל. ניתן לבחור סוג חיוב ספציפי פעם אחת בלבד בתצורה. |
|                        | מאפיין שורה        | בחר את מאפיין השורה המוגדר כברירת מחדל עבור סוג החיוב שנבחר. כשהערכות השעות החדשות, הערכות ההוצאות החדשות או הנתונים בפועל החדשים מסונכרנים מ- Project Service Automation, השדה **מאפיין שורה** מוגדר לערך ברירת המחדל עבור סוג החיוב. |
| נעילת פונקציונליות  | לא ישים       | בחר את הפונקציונליות כדי להשבית את Finance עבור פרויקטים וחוזים שמקורם ב- Project Service Automation. לדוגמה באפשרותך לכבות את היכולת לערוך חוזים ופרויקטים, ליצור מבנים של התפלגות עבודה ולהזין גליונות זמנים ב- Finance. שדות הקשורים לחשבונאות ימשיכו להיות זמינים, גם אם הם הפכו ללא זמינים באמצעות הגדרת הפרמטר. כברירת מחדל, כל פריטי הפונקציונליות זמינים. |
