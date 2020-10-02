---
title: עדכון הערכה בעת סיום
description: נושא זה מספק מידע על עדכון הקרנת המאמץ בפרויקט.
author: ruhercul
manager: AnnBe
ms.date: 09/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 42824cc4cfc2b934f69d319944fe7ee43183955c
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897767"
---
# <a name="update-estimate-at-completion"></a><span data-ttu-id="c5e9f-103">עדכון הערכה בעת סיום</span><span class="sxs-lookup"><span data-stu-id="c5e9f-103">Update estimate at completion</span></span>

<span data-ttu-id="c5e9f-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="c5e9f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c5e9f-105">מקובל שמנהל פרויקט ישנה את ההערכות המקוריות במשימה.</span><span class="sxs-lookup"><span data-stu-id="c5e9f-105">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="c5e9f-106">חיזויים מחדש של פרויקט הם תפיסות של מנהל הפרויקט להערכות, בהינתן המצב הנוכחי של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="c5e9f-106">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="c5e9f-107">אולם, אנחנו לא ממליצים למנהל הפרויקט לשנות את המספרים הבסיסיים, מכיוון שבסיס הפרויקט מייצג את מקור האמת המבוסס של הערכת העלות ולוח הזמנים של הפרויקט, וכל בעלי העניין של הפרויקט הסכימו עליו.</span><span class="sxs-lookup"><span data-stu-id="c5e9f-107">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="c5e9f-108">קיימות שתי דרכים שבהן מנהל פרויקט יכול לבצע חיזוי מחדש של מאמץ במשימות:</span><span class="sxs-lookup"><span data-stu-id="c5e9f-108">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="c5e9f-109">עקוף את הערכת ברירת המחדל כדי להשלים (ETC) בעזרת הערכה חדשה של המאמץ בפועל שנותר במשימה.</span><span class="sxs-lookup"><span data-stu-id="c5e9f-109">Override the default estimate to complete (ETC) with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="c5e9f-110">עקוף את אחוז ההתקדמות שבברירת מחדל בעזרת הערכה חדשה של ההתקדמות האמיתית במשימה.</span><span class="sxs-lookup"><span data-stu-id="c5e9f-110">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="c5e9f-111">כל אחת מהגישות האלו גורמת לחישוב מחדש של ה- ETC, הערכה בשלב ההשלמה (‏EAC) ואחוז ההתקדמות במשימה ושל סטיית המאמץ החזוי במשימה.</span><span class="sxs-lookup"><span data-stu-id="c5e9f-111">Each of these approaches cause a recalculation of the task's ETC, estimate at complete (EAC), and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="c5e9f-112">ה- EAC, ‏ETC ואחוז ההתקדמות בפעילויות הערסל מחושבים ומפיקים חיזוי חדש לסטיית המאמץ.</span><span class="sxs-lookup"><span data-stu-id="c5e9f-112">The EAC, ETC, and progress percentage on the summary tasks are recalculated, and produce a new projection of effort variance.</span></span>
