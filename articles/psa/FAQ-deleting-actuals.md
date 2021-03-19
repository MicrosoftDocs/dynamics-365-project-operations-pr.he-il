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
ms.openlocfilehash: e3122c5d9495b3ff9a683f477e719ce0c228a84d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286069"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="e503c-103">מדוע איני יכול למחוק רשומות מהישות 'נתונים בפועל'?</span><span class="sxs-lookup"><span data-stu-id="e503c-103">Why can’t I delete records from the Actuals entity?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="e503c-104">Project Service Automation‏ (PSA) אינו מאפשר לך למחוק נתונים בפועל משום שהם משמשים כמקור האמת עבור עסקאות בעלות השלכות פיננסיות על מערכות במורד הזרם, כגון ספר החשבונות הכללי.</span><span class="sxs-lookup"><span data-stu-id="e503c-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="e503c-105">אם הייתה אפשרות למחוק את הנתונים בפועל, תקינות הדיווח הפיננסי על עסקאות הייתה מוטלת בספק.</span><span class="sxs-lookup"><span data-stu-id="e503c-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="e503c-106">כדי ליצור נתיב ביקורת, על הלקוחות להשתמש ביומנים כדי ליצור עסקאות פיצוי.</span><span class="sxs-lookup"><span data-stu-id="e503c-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]