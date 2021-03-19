---
title: קביעת התצורה של יצירת חשבוניות אוטומטית
description: נושא זה מספק מידע על אופן קביעת התצורה של המערכת ליצירת חשבוניות באופן אוטומטי.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 0dddd963e79f8ecd91a96a6e684ab79e1b95bd6d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287914"
---
# <a name="configure-automatic-invoice-creation"></a><span data-ttu-id="652da-103">קביעת התצורה של יצירת חשבוניות אוטומטית</span><span class="sxs-lookup"><span data-stu-id="652da-103">Configure automatic invoice creation</span></span>

<span data-ttu-id="652da-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="652da-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="652da-105">השלם את השלבים הבאים להגדרת חשבונית אוטומטית המופעלת ב-Dynamics 365 Project operations.</span><span class="sxs-lookup"><span data-stu-id="652da-105">Complete the following steps to configure an automated invoice run in Dynamics 365 Project operations.</span></span>

1. <span data-ttu-id="652da-106">עבור אל **הגדרות** > **משימות אצווה**.</span><span class="sxs-lookup"><span data-stu-id="652da-106">Go to **Settings** > **Batch jobs**.</span></span>
2. <span data-ttu-id="652da-107">צור משימת אצווה ושנה את שמה ל- **צור חשבוניות ב- Project Operations**.</span><span class="sxs-lookup"><span data-stu-id="652da-107">Create a batch job, and name it **Project operations create invoices**.</span></span> <span data-ttu-id="652da-108">שם משימת האצווה חייב לכלול את המילים "צור חשבוניות."</span><span class="sxs-lookup"><span data-stu-id="652da-108">The name of the batch job must include the words "create invoices."</span></span>
3. <span data-ttu-id="652da-109">בשדה **סוג משימה**, בחר **ללא**.</span><span class="sxs-lookup"><span data-stu-id="652da-109">In the **Job Type** field, select **None**.</span></span> <span data-ttu-id="652da-110">כברירת מחדל, האפשרות **תדירות יומית** והאפשרות **הוא פעיל** מוגדרות בתור **כן**.</span><span class="sxs-lookup"><span data-stu-id="652da-110">By default, the **Frequency Daily** and **Is Active** options are set to **Yes**.</span></span>
4. <span data-ttu-id="652da-111">בחר **הפעל זרימת עבודה**.</span><span class="sxs-lookup"><span data-stu-id="652da-111">Select **Run Workflow**.</span></span> <span data-ttu-id="652da-112">בתיבת הדו-שיח **חיפוש רשומה** תראה שלוש זרימות עבודה:</span><span class="sxs-lookup"><span data-stu-id="652da-112">In the **Look Up Record** dialog box, you will see three workflows:</span></span>

    - <span data-ttu-id="652da-113">ProcessRunCaller</span><span class="sxs-lookup"><span data-stu-id="652da-113">ProcessRunCaller</span></span>
    - <span data-ttu-id="652da-114">ProcessRunner</span><span class="sxs-lookup"><span data-stu-id="652da-114">ProcessRunner</span></span>
    - <span data-ttu-id="652da-115">UpdateRoleUtilization</span><span class="sxs-lookup"><span data-stu-id="652da-115">UpdateRoleUtilization</span></span>

5. <span data-ttu-id="652da-116">בחר את **ProcessRunCaller** ולאחר מכן בחר **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="652da-116">Select **ProcessRunCaller**, and then select **Add**.</span></span>
6. <span data-ttu-id="652da-117">בתיבת הדו-שיח הבאה, בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="652da-117">In the next dialog box, select **OK**.</span></span> <span data-ttu-id="652da-118">אחרי זרימת עבודה **שינה** תופיע זרימת עבודה **תהליך**.</span><span class="sxs-lookup"><span data-stu-id="652da-118">A **Sleep** workflow is followed by a **Process** workflow.</span></span>

  > [!NOTE]
  > <span data-ttu-id="652da-119">תוכל גם לבחור את **ProcessRunner** בשלב 5.</span><span class="sxs-lookup"><span data-stu-id="652da-119">You can also select **ProcessRunner** in step 5.</span></span> <span data-ttu-id="652da-120">לאחר מכן, כשתבחר **אישור**, אחרי זרימת העבודה **תהליך** תופיע זרימת עבודה **שינה**.</span><span class="sxs-lookup"><span data-stu-id="652da-120">Then, when you select **OK**, a **Process** workflow is followed by a **Sleep** workflow.</span></span>

<span data-ttu-id="652da-121">זרימת העבודה **ProcessRunCaller** וזרימת העבודה **ProcessRunner** יוצרות חשבוניות.</span><span class="sxs-lookup"><span data-stu-id="652da-121">The **ProcessRunCaller** and **ProcessRunner** workflows create invoices.</span></span> <span data-ttu-id="652da-122">**ProcessRunCaller** קורא ל- **ProcessRunner**.</span><span class="sxs-lookup"><span data-stu-id="652da-122">**ProcessRunCaller** calls **ProcessRunner**.</span></span> <span data-ttu-id="652da-123">**ProcessRunner** היא למעשה זרימת העבודה שיוצרת למעשה את החשבוניות.</span><span class="sxs-lookup"><span data-stu-id="652da-123">**ProcessRunner** is the workflow that actually creates the invoices.</span></span> <span data-ttu-id="652da-124">היא עוברת על כל סעיפי החוזה שעבורם יש ליצור חשבונית, והיא יוצרת שורות עבור שורות אלו.</span><span class="sxs-lookup"><span data-stu-id="652da-124">It goes through all the contract lines that invoices must be created for, and it creates invoices for those lines.</span></span> <span data-ttu-id="652da-125">כדי לקבוע את סעיפי החוזה שעבורם יש ליצור חשבוניות, המשימה מחפשת תאריכים של הפעלת חשבוניות עבור סעיפי החוזה.</span><span class="sxs-lookup"><span data-stu-id="652da-125">To determine the contract lines that invoices must be created for, the job looks at invoice run dates for the contract lines.</span></span> <span data-ttu-id="652da-126">אם לסעיפי חוזה השייכים לחוזה אחד יש תאריך הפעלת חשבונית זהה, העסקאות משולבות לחשבונית אחת הכוללת שתי שורות בחשבונית.</span><span class="sxs-lookup"><span data-stu-id="652da-126">If contract lines that belong to one contract have the same invoice run date, the transactions are combined into one invoice that has two invoice lines.</span></span> <span data-ttu-id="652da-127">אם אין עסקאות שעבורן יש ליצור חשבוניות, המשימה מדלגת על יצירת חשבונית.</span><span class="sxs-lookup"><span data-stu-id="652da-127">If there are no transactions to create invoices for, the job skips invoice creation.</span></span>

<span data-ttu-id="652da-128">לאחר שהפעלת **ProcessRunner** הסתיימה, היא קוראת ל- **ProcessRunCaller**, מספקת את שעת הסיום ונסגרת.</span><span class="sxs-lookup"><span data-stu-id="652da-128">After **ProcessRunner** has finished running, it calls **ProcessRunCaller**, provides the end time, and is closed.</span></span> <span data-ttu-id="652da-129">לאחר מכן, **ProcessRunCaller** מפעילה שעון עצר הפועל במשך 24 שעות משעת הסיום שצוינה.</span><span class="sxs-lookup"><span data-stu-id="652da-129">**ProcessRunCaller** then starts a timer that runs for 24 hours from the specified end time.</span></span> <span data-ttu-id="652da-130">כששעון העצר מפסיק, **ProcessRunCaller** נסגרת.</span><span class="sxs-lookup"><span data-stu-id="652da-130">At the end of the timer, **ProcessRunCaller** is closed.</span></span>

<span data-ttu-id="652da-131">משימת תהליך האצווה ליצירת חשבוניות היא משימה חוזרת.</span><span class="sxs-lookup"><span data-stu-id="652da-131">The batch process job for creating invoices is a recurrent job.</span></span> <span data-ttu-id="652da-132">אם תהליך אצווה זה מופעל פעמים רבות, נוצרים מופעים מרובים של המשימה וגורמים לשגיאות.</span><span class="sxs-lookup"><span data-stu-id="652da-132">If this batch process is run many times, multiple instances of the job are created and cause errors.</span></span> <span data-ttu-id="652da-133">לכן עליך להתחיל את תהליך האצווה רק פעם אחת, ועליך להפעיל אותו מחדש רק אם הוא מפסיק לפעול.</span><span class="sxs-lookup"><span data-stu-id="652da-133">Therefore, you should start the batch process only one time, and you should restart it only if it stops running.</span></span>

> [!NOTE]
> <span data-ttu-id="652da-134">חשבונית אצווה פועלת רק עבור שורות חוזה בפרויקט המוגדרות על פי לוחות זמנים של חשבוניות.</span><span class="sxs-lookup"><span data-stu-id="652da-134">Batch invoicing only runs for project contract lines that are configured by invoice schedules.</span></span> <span data-ttu-id="652da-135">אבני דרך חייבים להיות מוגדרים בסעיף חוזה בשיטת חיוב במחיר קבוע.</span><span class="sxs-lookup"><span data-stu-id="652da-135">A contract line with a fixed price billing method must have milestones configured.</span></span> <span data-ttu-id="652da-136">סעיף חוזה בפרויקט בשיטת חיוב לפי זמן וחומר יצטרך הגדרה של לוח זמנים לחשבוניות המבוסס על תאריכים.</span><span class="sxs-lookup"><span data-stu-id="652da-136">A project contract line with a time and material billing method will need a date-based invoice schedule set up.</span></span> <span data-ttu-id="652da-137">כך גם בסעיף חוזה שמבוסס על פרויקטים.</span><span class="sxs-lookup"><span data-stu-id="652da-137">The same applies to a project-based contract line.</span></span>     


[!INCLUDE[footer-include](../includes/footer-banner.md)]