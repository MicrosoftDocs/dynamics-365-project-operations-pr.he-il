---
title: הערות מפתחים לאישורים
description: נושא זה מספק מידע נוסף למפתחים לגבי עבודה עם אישורים.
author: stsporen
ms.date: 11/09/2020
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: a89ea669a262c145b9f391fddc19e79a425fabb5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996792"
---
# <a name="developer-notes-for-approvals"></a><span data-ttu-id="3bb6d-103">הערות מפתחים לאישורים</span><span class="sxs-lookup"><span data-stu-id="3bb6d-103">Developer notes for Approvals</span></span>

<span data-ttu-id="3bb6d-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="3bb6d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="3bb6d-105">Dynamics 365 Project Operations כולל לוגיקת אימות המבטיחה מעבר רשומות נכון לאורך שלבי האישור.</span><span class="sxs-lookup"><span data-stu-id="3bb6d-105">Dynamics 365 Project Operations includes validation logic that ensures correct record transition through the approval stages.</span></span> <span data-ttu-id="3bb6d-106">מעבר רשומות נכון מבטיח:</span><span class="sxs-lookup"><span data-stu-id="3bb6d-106">Correct record transitions ensure:</span></span> 

  - <span data-ttu-id="3bb6d-107">כל השורות התומכות נוצרות בטבלאות קשורות, כגון יומנים ונתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="3bb6d-107">All supporting rows are created in related tables, such as journals and actuals.</span></span>
  - <span data-ttu-id="3bb6d-108">המאשר מסומן כ **מאשר פרוייקט** בפרויקט לפני שממשיך.</span><span class="sxs-lookup"><span data-stu-id="3bb6d-108">The approver is marked as a **Project Approver** in the project before proceeding.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]