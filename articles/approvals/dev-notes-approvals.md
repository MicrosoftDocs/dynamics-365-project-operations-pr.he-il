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
ms.openlocfilehash: 9e4e910d0ff0a5f2603148fcc5daa0d423a4d174
ms.sourcegitcommit: a9dbcd3aff4c6ae495412e4980e105ae160fd1ec
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 11/10/2020
ms.locfileid: "4483949"
---
# <a name="developer-notes-for-approvals"></a><span data-ttu-id="c474e-103">הערות מפתחים לאישורים</span><span class="sxs-lookup"><span data-stu-id="c474e-103">Developer notes for Approvals</span></span>

<span data-ttu-id="c474e-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="c474e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c474e-105">Dynamics 365 Project Operations כוללות לוגיקת אימות המבטיחה מעבר רשומות נכון לאורך שלבי האישור.</span><span class="sxs-lookup"><span data-stu-id="c474e-105">Dynamics 365 Project Operations includes validation logic that ensures correct record transition through the approval stages.</span></span> <span data-ttu-id="c474e-106">מעבר רשומות נכון מבטיח:</span><span class="sxs-lookup"><span data-stu-id="c474e-106">Correct record transitions ensure:</span></span> 

  - <span data-ttu-id="c474e-107">כל השורות התומכות נוצרות בטבלאות קשורות, כגון יומנים ונתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="c474e-107">All supporting rows are created in related tables, such as journals and actuals.</span></span>
  - <span data-ttu-id="c474e-108">המאשר מסומן כ **מאשר פרוייקט** בפרויקט לפני שממשיך.</span><span class="sxs-lookup"><span data-stu-id="c474e-108">The approver is marked as a **Project Approver** in the project before proceeding.</span></span>
