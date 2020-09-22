---
title: מדוע איני יכול למחוק רשומות מהישות 'נתונים בפועל'?
description: נושא זה מספק מידע אודות הסיבה לכך שאין באפשרותך למחוק רשומות מישות הנתונים בפועל.
author: JPBurrows
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 11/6/2018
ms.topic: article
ms.prod: Project Service
ms.technology: Applies to all versions of Project Service
ms.assetid: ff504c34-7337-474f-89e8-d8afdd1e0a98
ms.author: Jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5817940933c161dccac0fe549fabacbe57e7077a
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751759"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="2317a-103">מדוע איני יכול למחוק רשומות מהישות 'נתונים בפועל'?</span><span class="sxs-lookup"><span data-stu-id="2317a-103">Why can’t I delete records from the Actuals entity?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="2317a-104">Project Service Automation‏ (PSA) אינו מאפשר לך למחוק נתונים בפועל משום שהם משמשים כמקור האמת עבור עסקאות בעלות השלכות פיננסיות על מערכות במורד הזרם, כגון ספר החשבונות הכללי.</span><span class="sxs-lookup"><span data-stu-id="2317a-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="2317a-105">אם הייתה אפשרות למחוק את הנתונים בפועל, תקינות הדיווח הפיננסי על עסקאות הייתה מוטלת בספק.</span><span class="sxs-lookup"><span data-stu-id="2317a-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="2317a-106">כדי ליצור נתיב ביקורת, על הלקוחות להשתמש ביומנים כדי ליצור עסקאות פיצוי.</span><span class="sxs-lookup"><span data-stu-id="2317a-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>

