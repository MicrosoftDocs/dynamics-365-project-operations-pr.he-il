---
title: הבנת מצב הפרוייקט
description: נושא זה מספק מידע על המצב המוקצה לפרוייקטים ב- Dynamics 365 Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 336e479ad39653af14cca7930fe63e906b7de489
ms.sourcegitcommit: fd8ea1779db2bb39a428f459ae3293c4fd785572
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/06/2020
ms.locfileid: "3965677"
---
# <a name="understand-project-status"></a><span data-ttu-id="8d78c-103">הבנת מצב הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="8d78c-103">Understand project status</span></span>

<span data-ttu-id="8d78c-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="8d78c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="8d78c-105">המקטע  **מצב** בדף **ישות הפרוייקט** כולל סיכום של תקינות הפרוייקט על סמך עלות ומאמץ.</span><span class="sxs-lookup"><span data-stu-id="8d78c-105">The **Status** section on the **Project Entity** page provides a summary of a project's health based upon cost and effort.</span></span>


## <a name="status-summary-fields"></a><span data-ttu-id="8d78c-106">שדות סיכום מצב</span><span class="sxs-lookup"><span data-stu-id="8d78c-106">Status summary fields</span></span>

- <span data-ttu-id="8d78c-107">השדה **מצב פרוייקט כולל‬** הוא שדה ניתן לעריכה שמציג את המצב הכולל של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="8d78c-107">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="8d78c-108">בשדה זה נעשה שימוש בקידוד צבעים, כגון ירוק, צהוב ואדום, כדי לציין סיכון שמתגבר.</span><span class="sxs-lookup"><span data-stu-id="8d78c-108">This field uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> 
- <span data-ttu-id="8d78c-109">השדה **הערות** מאפשר למנהל הפרוייקט להזין הערות ספציפיות לגבי המצב.</span><span class="sxs-lookup"><span data-stu-id="8d78c-109">The **Comments** field lets the project manager enter specific comments about the status.</span></span> 
- <span data-ttu-id="8d78c-110">השדה **המצב עודכן בתאריך** אינו ניתן לעריכה.</span><span class="sxs-lookup"><span data-stu-id="8d78c-110">The **Status updated on** field isn't editable.</span></span> <span data-ttu-id="8d78c-111">הערך בשדה זה הוא חותמת זמן המציינת מתי עודכן המצב לאחרונה.</span><span class="sxs-lookup"><span data-stu-id="8d78c-111">The value in this field is a timestamp that indicates when the status was last updated.</span></span>
- <span data-ttu-id="8d78c-112">השדות **ביצועי לוח זמנים** ו **ביצועי עלות**‏‫ נקבעים מרשת המעקב.</span><span class="sxs-lookup"><span data-stu-id="8d78c-112">The **Schedule performance** and **Cost performance** fields are set from the tracking grid.</span></span> <span data-ttu-id="8d78c-113">כאשר לוח הזמנים וסטיית העלות עבור צומת הבסיס בתצוגה **מעקב מאמץ** חיוביים, שדות אלו מתעדכנים ל **הקדמה**.</span><span class="sxs-lookup"><span data-stu-id="8d78c-113">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, these fields are updated to **Ahead**.</span></span> <span data-ttu-id="8d78c-114">כאשר לוח הזמנים וסטיית העלות עבור צומת הבסיס שליליים, שדות אלו מוגדרים כ **עיכוב**.</span><span class="sxs-lookup"><span data-stu-id="8d78c-114">When the schedule and cost variance for the root node are negative, these fields are set to **Behind**.</span></span>
