---
title: מדוע איני יכול למחוק רשומות מהישות 'נתונים בפועל'?
description: נושא זה מספק מידע אודות הסיבה לכך שאין באפשרותך למחוק רשומות מישות הנתונים בפועל.
author: JPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 11/6/2018
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
ms.openlocfilehash: 36cd241c7c7a2ff6ae018c94d691bc95d1f0c912
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5148959"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="666da-103">מדוע איני יכול למחוק רשומות מהישות 'נתונים בפועל'?</span><span class="sxs-lookup"><span data-stu-id="666da-103">Why can’t I delete records from the Actuals entity?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="666da-104">Project Service Automation‏ (PSA) אינו מאפשר לך למחוק נתונים בפועל משום שהם משמשים כמקור האמת עבור עסקאות בעלות השלכות פיננסיות על מערכות במורד הזרם, כגון ספר החשבונות הכללי.</span><span class="sxs-lookup"><span data-stu-id="666da-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="666da-105">אם הייתה אפשרות למחוק את הנתונים בפועל, תקינות הדיווח הפיננסי על עסקאות הייתה מוטלת בספק.</span><span class="sxs-lookup"><span data-stu-id="666da-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="666da-106">כדי ליצור נתיב ביקורת, על הלקוחות להשתמש ביומנים כדי ליצור עסקאות פיצוי.</span><span class="sxs-lookup"><span data-stu-id="666da-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>

