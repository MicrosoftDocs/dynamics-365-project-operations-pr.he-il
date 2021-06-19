---
title: קבוצות אישורים
description: נושא זה מספק מידע על קבוצות אישורים, בקשות וקבוצות משנה של פעולות אלה.
author: stsporen
manager: tfehr
ms.date: 05/28/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: ac73313420029ece740d0bdb9c21c7abaa9defc6
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116872"
---
# <a name="approval-sets"></a><span data-ttu-id="43c8b-103">קבוצות אישורים</span><span class="sxs-lookup"><span data-stu-id="43c8b-103">Approval sets</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="43c8b-104">בקבוצות אישורים מגדירים בקשות אישור יחד לקבוצות משנה קטנות יותר של פעולות.</span><span class="sxs-lookup"><span data-stu-id="43c8b-104">Approval sets group approval requests together into smaller subsets of operations.</span></span> <span data-ttu-id="43c8b-105">קיבוץ זה מאפשר לעבד אישורים לפי סדר בפרוייקט ומאפשר ניסיון מחדש ורצף.</span><span class="sxs-lookup"><span data-stu-id="43c8b-105">This grouping allows approvals to be processed in order by Project and allows for retrying and sequencing.</span></span> <span data-ttu-id="43c8b-106">קיבוץ משפר את האמינות והעקיבות של עיבוד האישורים אם יש כמויות גדולות של אישורים.</span><span class="sxs-lookup"><span data-stu-id="43c8b-106">Grouping improves the reliability and traceability of approval processing for large volumes of approvals.</span></span>

<span data-ttu-id="43c8b-107">קבוצות אישורים מציינות את מצב העיבוד הכולל של הרשומות הקשורות אליהם.</span><span class="sxs-lookup"><span data-stu-id="43c8b-107">Approval sets indicate the overall processing state of their related records.</span></span> <span data-ttu-id="43c8b-108">כאשר רשומת אישור מעובדת באמצעות קבוצת אישורים, הרשומה עוברת ממצב **הוגש** למצב **אושר**, והקישור שלה מקבוצת האישורים מבוטל.</span><span class="sxs-lookup"><span data-stu-id="43c8b-108">When an approval record is processed using an approval set, the record moves from **Submitted** to **Approved**, and is unlinked from the approval set.</span></span> <span data-ttu-id="43c8b-109">אם רשומה נכשלת כשהיא מוגשת לאישור, הרשומה נשארת במצב **הוגש** וקבוצת האישורים מסומנת 'נכשל'.</span><span class="sxs-lookup"><span data-stu-id="43c8b-109">If a record fails when it is submitted for approval, the record remains in a status of **Submitted** and the approval set is marked as failed.</span></span> <span data-ttu-id="43c8b-110">קבוצת האישורים רושמת את הודעת השגיאה של הכשל.</span><span class="sxs-lookup"><span data-stu-id="43c8b-110">The approval set logs the error message of the failure.</span></span>

## <a name="processing-approvals-and-approval-sets"></a><span data-ttu-id="43c8b-111">עיבוד אישורים וקבוצות אישורים</span><span class="sxs-lookup"><span data-stu-id="43c8b-111">Processing approvals and approval sets</span></span>
<span data-ttu-id="43c8b-112">אישורים שממתינים בתור לעיבוד מופיעים בתצוגה **עיבוד אישורים**.</span><span class="sxs-lookup"><span data-stu-id="43c8b-112">Approvals that are queued for processing are visible in the **Processing Approvals** view.</span></span> <span data-ttu-id="43c8b-113">המערכת מנסה לעבד את כל הערכים מספר פעמים בצורה אסינכרונית, כולל ניסיון אישור חוזר אם ניסיונות קודמים נכשלו.</span><span class="sxs-lookup"><span data-stu-id="43c8b-113">The system tries to process all the entries multiple times asynchronously, including retrying an approval if previous attempts failed.</span></span>

<span data-ttu-id="43c8b-114">השדה **אורך החיים מוגדר** מתעד את מספר הניסיונות שנותרו לעבד את הקבוצה לפני הסימון 'נכשל'.</span><span class="sxs-lookup"><span data-stu-id="43c8b-114">The **Approval Set Lifetime** field records the number of attempts left to process the set before it's marked as failed.</span></span>

## <a name="failed-approvals-and-approval-sets"></a><span data-ttu-id="43c8b-115">אישורים וקבוצות אישורים שנכשלו</span><span class="sxs-lookup"><span data-stu-id="43c8b-115">Failed approvals and approval sets</span></span>
<span data-ttu-id="43c8b-116">התצוגה **אישורים שנכשלו** מפרטת את כל האישורים שדורשים התערבות משתמש.</span><span class="sxs-lookup"><span data-stu-id="43c8b-116">The **Failed Approvals** view lists all approvals that require user intervention.</span></span> <span data-ttu-id="43c8b-117">פתח את יומני קבוצות האישורים המשויכים כדי לזהות את הגורם לכשל.</span><span class="sxs-lookup"><span data-stu-id="43c8b-117">Open the associated approval set logs to identify the cause of the failure.</span></span>
<span data-ttu-id="43c8b-118">בחירה באפשרות **נסה שוב** מוסיפה למשך החיים של קבוצת האישורים, מעבירה את קבוצת האישורים למצב **בעיבוד**, ומנסה לעבד את הרשומות שנותרו.</span><span class="sxs-lookup"><span data-stu-id="43c8b-118">Selecting **Retry** adds to the approval set lifetime count, moves the approval set back to a status of **Processing**, and attempts to process the remaining records.</span></span>

## <a name="configure-approval-sets"></a><span data-ttu-id="43c8b-119">הגדר קבוצות אישורים</span><span class="sxs-lookup"><span data-stu-id="43c8b-119">Configure approval sets</span></span>

###  <a name="enable-the-approval-sets-feature"></a><span data-ttu-id="43c8b-120">הפעל את התכונה 'קבוצות אישורים'</span><span class="sxs-lookup"><span data-stu-id="43c8b-120">Enable the Approval sets feature</span></span>
<span data-ttu-id="43c8b-121">לפני שתפעיל את התכונה 'קבוצות אישורים', ודא שאין כרגע אישורים בעיבוד.</span><span class="sxs-lookup"><span data-stu-id="43c8b-121">Before you enable the Approval sets feature, verify that there are no approvals currently being processed.</span></span>

- <span data-ttu-id="43c8b-122">עבור אל הדף **פרמטרים של הפרוייקט** ובחר **בקרת תכונות** > **הפעל אישורים מודרניים**.</span><span class="sxs-lookup"><span data-stu-id="43c8b-122">Go to the **Project parameters** page and select **Feature Control** > **Enable Modern Approvals**.</span></span>

### <a name="turn-off-the-approval-sets-feature"></a><span data-ttu-id="43c8b-123">השבת את התכונה 'קבוצות אישורים'</span><span class="sxs-lookup"><span data-stu-id="43c8b-123">Turn off the Approval sets feature</span></span>
<span data-ttu-id="43c8b-124">לפני שתשבית את התכונה 'קבוצות אישורים', ודא שאין כרגע אישורים בעיבוד.</span><span class="sxs-lookup"><span data-stu-id="43c8b-124">Before you turn off the Approval sets feature, verify that there are no approvals currently being processed.</span></span>

- <span data-ttu-id="43c8b-125">עבור אל הדף **פרמטרים של הפרוייקט** ובחר **בקרת תכונות** > **השבת אישורים מודרניים**.</span><span class="sxs-lookup"><span data-stu-id="43c8b-125">Go to the **Project Parameters** page and select **Feature Control** > **Disable Modern Approvals**.</span></span>

### <a name="configuring-the-asynchronous-threshold"></a><span data-ttu-id="43c8b-126">הגדרת סף אסינכרוני</span><span class="sxs-lookup"><span data-stu-id="43c8b-126">Configuring the asynchronous threshold</span></span> 
<span data-ttu-id="43c8b-127">כאשר נוצרות קבוצות אישורים, העיבוד עובר לרקע כאשר מספר הרשומות שנבחר לאישור חורג מהסף המצוין.</span><span class="sxs-lookup"><span data-stu-id="43c8b-127">When approval sets are created, processing moves to the background when the selected number of records for approval exceeds the indicated threshold.</span></span> <span data-ttu-id="43c8b-128">השתמש בשדה **סף אסינכרוני** כדי להגדיר מתי עיבוד האישורים צריך להיות מופעל באופן סינכרוני או אסינכרוני.</span><span class="sxs-lookup"><span data-stu-id="43c8b-128">Use the **Asynchronous Threshold** field to configure when approval processing should be run synchronously or asynchronously.</span></span>
<span data-ttu-id="43c8b-129">הערכים החוקיים הם:</span><span class="sxs-lookup"><span data-stu-id="43c8b-129">Valid values are:</span></span>

  - <span data-ttu-id="43c8b-130">אפס: יש לעבד את כל הבקשות בצורה אסינכרונית.</span><span class="sxs-lookup"><span data-stu-id="43c8b-130">Zero: All requests should be processed asynchronously.</span></span> 
  - <span data-ttu-id="43c8b-131">מספרים הגדולים מאפס: האישורים מעובדים בצורה אסינכרונית רק כאשר מספר האישורים שהוגש עולה על ערך זה.</span><span class="sxs-lookup"><span data-stu-id="43c8b-131">Numbers greater than zero: Approvals are processed asynchronously only when the submitted number of approvals exceeds this value.</span></span>

[!INCLUDE[footer-include](../includes/footer-banner.md)]
