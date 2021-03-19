---
title: הערות מפתחים לאישורים
description: נושא זה מספק מידע נוסף למפתחים לגבי עבודה עם אישורים.
author: stsporen
manager: Annbe
ms.date: 11/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: d58c776b0341c08b0292e1b459a7d7ebac550bcc
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290270"
---
# <a name="developer-notes-for-approvals"></a><span data-ttu-id="f8c80-103">הערות מפתחים לאישורים</span><span class="sxs-lookup"><span data-stu-id="f8c80-103">Developer notes for Approvals</span></span>

<span data-ttu-id="f8c80-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="f8c80-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f8c80-105">Dynamics 365 Project Operations כולל לוגיקת אימות המבטיחה מעבר רשומות נכון לאורך שלבי האישור.</span><span class="sxs-lookup"><span data-stu-id="f8c80-105">Dynamics 365 Project Operations includes validation logic that ensures correct record transition through the approval stages.</span></span> <span data-ttu-id="f8c80-106">מעבר רשומות נכון מבטיח:</span><span class="sxs-lookup"><span data-stu-id="f8c80-106">Correct record transitions ensure:</span></span> 

  - <span data-ttu-id="f8c80-107">כל השורות התומכות נוצרות בטבלאות קשורות, כגון יומנים ונתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="f8c80-107">All supporting rows are created in related tables, such as journals and actuals.</span></span>
  - <span data-ttu-id="f8c80-108">המאשר מסומן כ **מאשר פרוייקט** בפרויקט לפני שממשיך.</span><span class="sxs-lookup"><span data-stu-id="f8c80-108">The approver is marked as a **Project Approver** in the project before proceeding.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]