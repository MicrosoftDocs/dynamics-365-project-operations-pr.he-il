---
title: הבנת מצב הפרויקט
description: נושא זה מספק מידע על הסטטוס שהוקצה לפרויקטים ב- Dynamics 365 Project Operations.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: ad8c012b93bc65595dca33df1770562916c557e0
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993417"
---
# <a name="understand-project-status"></a><span data-ttu-id="b03e9-103">הבנת מצב הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="b03e9-103">Understand project status</span></span>

<span data-ttu-id="b03e9-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="b03e9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="b03e9-105">המקטע **מצב** בדף **ישות הפרויקט** מספק סיכום של תקינות הפרויקט על סמך עלות ומאמץ.</span><span class="sxs-lookup"><span data-stu-id="b03e9-105">The **Status** section on the **Project Entity** page provides a summary of a project's health based upon cost and effort.</span></span>


## <a name="status-summary-fields"></a><span data-ttu-id="b03e9-106">שדות סיכום מצב</span><span class="sxs-lookup"><span data-stu-id="b03e9-106">Status summary fields</span></span>

- <span data-ttu-id="b03e9-107">השדה **מצב פרויקט כולל‬** הוא שדה שניתן לערוך אותו ושמציג את המצב הכולל של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="b03e9-107">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="b03e9-108">בשדה זה נעשה שימוש בקידוד צבעים, כגון ירוק, צהוב ואדום, כדי לציין סיכון שמתגבר.</span><span class="sxs-lookup"><span data-stu-id="b03e9-108">This field uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> 
- <span data-ttu-id="b03e9-109">השדה **הערות** מאפשר למנהל הפרויקט להזין הערות ספציפיות לגבי המצב.</span><span class="sxs-lookup"><span data-stu-id="b03e9-109">The **Comments** field lets the project manager enter specific comments about the status.</span></span> 
- <span data-ttu-id="b03e9-110">השדה **המצב עודכן בתאריך** אינו ניתן לעריכה.</span><span class="sxs-lookup"><span data-stu-id="b03e9-110">The **Status updated on** field isn't editable.</span></span> <span data-ttu-id="b03e9-111">הערך בשדה זה הוא חותמת זמן המציינת מתי עודכן המצב לאחרונה.</span><span class="sxs-lookup"><span data-stu-id="b03e9-111">The value in this field is a timestamp that indicates when the status was last updated.</span></span>
- <span data-ttu-id="b03e9-112">השדות **‏‫ביצועי לוח הזמנים‬** ו **‏‫ביצועי עלות‬** מוגדרים מרשת המעקב.</span><span class="sxs-lookup"><span data-stu-id="b03e9-112">The **Schedule performance** and **Cost performance** fields are set from the tracking grid.</span></span> <span data-ttu-id="b03e9-113">כאשר סטיית לוח הזמנים והעלות עבור צומת הבסיס בתצוגה **מעקב מאמץ** חיוביות,  מתעדכנות ל **הקדמה‬**.</span><span class="sxs-lookup"><span data-stu-id="b03e9-113">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, these fields are updated to **Ahead**.</span></span> <span data-ttu-id="b03e9-114">כאשר סטיית לוח הזמנים והעלות עבור צומת הבסיס שלילית, שדות אלו מוגדרים כ **עיכוב**.</span><span class="sxs-lookup"><span data-stu-id="b03e9-114">When the schedule and cost variance for the root node are negative, these fields are set to **Behind**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]