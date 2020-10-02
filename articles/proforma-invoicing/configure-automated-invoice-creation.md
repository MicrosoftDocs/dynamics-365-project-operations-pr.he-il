---
title: הגדרה של יצירת חשבוניות אוטומטית
description: נושא זה מספק מידע על הדרך להגדיר את המערכת ליצירת חשבוניות באופן אוטומטי.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
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
ms.openlocfilehash: 764fd4568619e4f5676ee3cbf7fce14ffb069548
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898127"
---
# <a name="configure-automated-invoice-creation"></a><span data-ttu-id="e9ced-103">הגדרה של יצירת חשבוניות אוטומטית</span><span class="sxs-lookup"><span data-stu-id="e9ced-103">Configure automated invoice creation</span></span>

<span data-ttu-id="e9ced-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="e9ced-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e9ced-105">השלם את השלבים הבאים להגדרת חשבונית אוטומטית המופעלת ב-Project Operations.</span><span class="sxs-lookup"><span data-stu-id="e9ced-105">Complete the following steps to configure an automated invoice run in Project operations.</span></span>

1. <span data-ttu-id="e9ced-106">עבור אל **הגדרות** \> **‎משימות אצווה**.</span><span class="sxs-lookup"><span data-stu-id="e9ced-106">Go to **Settings** \> **Batch jobs**.</span></span>
2. <span data-ttu-id="e9ced-107">צור משימת אצווה ושנה את שמה ל- **צור חשבוניות ב- Project Operations**.</span><span class="sxs-lookup"><span data-stu-id="e9ced-107">Create a batch job, and name it **Project operations create invoices**.</span></span> <span data-ttu-id="e9ced-108">שם משימת האצווה חייב לכלול את המונח "צור חשבוניות".</span><span class="sxs-lookup"><span data-stu-id="e9ced-108">The name of the batch job must include the term "create invoices."</span></span>
3. <span data-ttu-id="e9ced-109">בשדה **סוג משימה**, בחר **ללא**.</span><span class="sxs-lookup"><span data-stu-id="e9ced-109">In the **Job type** field, select **None**.</span></span> <span data-ttu-id="e9ced-110">כברירת מחדל, האפשרות **תדירות יומית** והאפשרות **הוא פעיל** מוגדרות בתור **כן**.</span><span class="sxs-lookup"><span data-stu-id="e9ced-110">By default, the **Frequency Daily** and **Is Active** options are set to **Yes**.</span></span>
4. <span data-ttu-id="e9ced-111">בחר **הפעל זרימת עבודה**.</span><span class="sxs-lookup"><span data-stu-id="e9ced-111">Select **Run Workflow**.</span></span> <span data-ttu-id="e9ced-112">בתיבת הדו-שיח **חיפוש רשומה** תראה שלוש זרימות עבודה:</span><span class="sxs-lookup"><span data-stu-id="e9ced-112">In the **Look Up Record** dialog box, you will see three workflows:</span></span>

    - <span data-ttu-id="e9ced-113">ProcessRunCaller</span><span class="sxs-lookup"><span data-stu-id="e9ced-113">ProcessRunCaller</span></span>
    - <span data-ttu-id="e9ced-114">ProcessRunner</span><span class="sxs-lookup"><span data-stu-id="e9ced-114">ProcessRunner</span></span>
    - <span data-ttu-id="e9ced-115">UpdateRoleUtilization</span><span class="sxs-lookup"><span data-stu-id="e9ced-115">UpdateRoleUtilization</span></span>

5. <span data-ttu-id="e9ced-116">בחר את **ProcessRunCaller** ולאחר מכן בחר **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="e9ced-116">Select **ProcessRunCaller**, and then select **Add**.</span></span>
6. <span data-ttu-id="e9ced-117">בתיבת הדו-שיח הבאה, בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="e9ced-117">In the next dialog box, select **OK**.</span></span> <span data-ttu-id="e9ced-118">אחרי זרימת עבודה **שינה** תופיע זרימת עבודה **תהליך**.</span><span class="sxs-lookup"><span data-stu-id="e9ced-118">A **Sleep** workflow is followed by a **Process** workflow.</span></span>

    <span data-ttu-id="e9ced-119">תוכל גם לבחור את **ProcessRunner** בשלב 5.</span><span class="sxs-lookup"><span data-stu-id="e9ced-119">You can also select **ProcessRunner** in step 5.</span></span> <span data-ttu-id="e9ced-120">לאחר מכן, כשתבחר **אישור**, אחרי זרימת העבודה **תהליך** תופיע זרימת עבודה **שינה**.</span><span class="sxs-lookup"><span data-stu-id="e9ced-120">Then, when you select **OK**, a **Process** workflow is followed by a **Sleep** workflow.</span></span>

<span data-ttu-id="e9ced-121">זרימת העבודה **ProcessRunCaller** וזרימת העבודה **ProcessRunner** יוצרות חשבוניות.</span><span class="sxs-lookup"><span data-stu-id="e9ced-121">The **ProcessRunCaller** and **ProcessRunner** workflows create invoices.</span></span> <span data-ttu-id="e9ced-122">**ProcessRunCaller** קורא ל- **ProcessRunner**.</span><span class="sxs-lookup"><span data-stu-id="e9ced-122">**ProcessRunCaller** calls **ProcessRunner**.</span></span> <span data-ttu-id="e9ced-123">**ProcessRunner** היא למעשה זרימת העבודה שיוצרת למעשה את החשבוניות.</span><span class="sxs-lookup"><span data-stu-id="e9ced-123">**ProcessRunner** is the workflow that actually creates the invoices.</span></span> <span data-ttu-id="e9ced-124">היא עוברת על כל סעיפי החוזה שעבורם יש ליצור חשבונית, והיא יוצרת שורות עבור שורות אלו.</span><span class="sxs-lookup"><span data-stu-id="e9ced-124">It goes through all the contract lines that invoices must be created for, and it creates invoices for those lines.</span></span> <span data-ttu-id="e9ced-125">כדי לקבוע את סעיפי החוזה שעבורם יש ליצור חשבוניות, המשימה מחפשת תאריכים של הפעלת חשבוניות עבור סעיפי החוזה.</span><span class="sxs-lookup"><span data-stu-id="e9ced-125">To determine the contract lines that invoices must be created for, the job looks at invoice run dates for the contract lines.</span></span> <span data-ttu-id="e9ced-126">אם לסעיפי חוזה השייכים לחוזה אחד יש תאריך הפעלת חשבונית זהה, העסקאות משולבות לחשבונית אחת הכוללת שתי שורות בחשבונית.</span><span class="sxs-lookup"><span data-stu-id="e9ced-126">If contract lines that belong to one contract have the same invoice run date, the transactions are combined into one invoice that has two invoice lines.</span></span> <span data-ttu-id="e9ced-127">אם אין עסקאות שעבורן יש ליצור חשבוניות, המשימה מדלגת על יצירת חשבונית.</span><span class="sxs-lookup"><span data-stu-id="e9ced-127">If there are no transactions to create invoices for, the job skips invoice creation.</span></span>

<span data-ttu-id="e9ced-128">לאחר שהפעלת **ProcessRunner** הסתיימה, היא קוראת ל- **ProcessRunCaller**, מספקת את שעת הסיום ונסגרת.</span><span class="sxs-lookup"><span data-stu-id="e9ced-128">After **ProcessRunner** has finished running, it calls **ProcessRunCaller**, provides the end time, and is closed.</span></span> <span data-ttu-id="e9ced-129">לאחר מכן, **ProcessRunCaller** מפעילה שעון עצר הפועל במשך 24 שעות משעת הסיום שצוינה.</span><span class="sxs-lookup"><span data-stu-id="e9ced-129">**ProcessRunCaller** then starts a timer that runs for 24 hours from the specified end time.</span></span> <span data-ttu-id="e9ced-130">כששעון העצר מפסיק, **ProcessRunCaller** נסגרת.</span><span class="sxs-lookup"><span data-stu-id="e9ced-130">At the end of the timer, **ProcessRunCaller** is closed.</span></span>

<span data-ttu-id="e9ced-131">משימת תהליך האצווה ליצירת חשבוניות היא משימה חוזרת.</span><span class="sxs-lookup"><span data-stu-id="e9ced-131">The batch process job for creating invoices is a recurrent job.</span></span> <span data-ttu-id="e9ced-132">אם תהליך אצווה זה מופעל פעמים רבות, נוצרים מופעים מרובים של המשימה וגורמים לשגיאות.</span><span class="sxs-lookup"><span data-stu-id="e9ced-132">If this batch process is run many times, multiple instances of the job are created and cause errors.</span></span> <span data-ttu-id="e9ced-133">לכן עליך להתחיל את תהליך האצווה רק פעם אחת, ועליך להפעיל אותו מחדש רק אם הוא מפסיק לפעול.</span><span class="sxs-lookup"><span data-stu-id="e9ced-133">Therefore, you should start the batch process only one time, and you should restart it only if it stops running.</span></span>

> [!NOTE]
> <span data-ttu-id="e9ced-134">חשבונית אצווה פועלת רק עבור שורות חוזה בפרויקט המוגדרות על פי לוחות זמנים של חשבוניות.</span><span class="sxs-lookup"><span data-stu-id="e9ced-134">Batch invoicing only runs for project contract lines that are configured by invoice schedules.</span></span> <span data-ttu-id="e9ced-135">אבני דרך חייבים להיות מוגדרים בסעיף חוזה בשיטת חיוב במחיר קבוע.</span><span class="sxs-lookup"><span data-stu-id="e9ced-135">A contract line with a fixed price billing method must have milestones configured.</span></span> <span data-ttu-id="e9ced-136">סעיף חוזה בפרויקט בשיטת חיוב לפי זמן וחומר יצטרך הגדרה של לוח זמנים לחשבוניות המבוסס על תאריכים.</span><span class="sxs-lookup"><span data-stu-id="e9ced-136">A project contract line with a time and material billing method will need a date-based invoice schedule set up.</span></span> <span data-ttu-id="e9ced-137">כך גם בסעיף חוזה שמבוסס על פרויקטים.</span><span class="sxs-lookup"><span data-stu-id="e9ced-137">The same applies to a project-based contract line.</span></span>     
