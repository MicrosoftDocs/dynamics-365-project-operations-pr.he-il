---
title: הגדר תהליכי עבודה לניהול הוצאות
description: באפשרותך להגדיר תהליך זרימת עבודה המשמש לבדיקה ולאישור מסמכי נסיעות והוצאות.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: af6463b07e282ae1ff6aa7dc1a540ff7c8cc318a
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127699"
---
# <a name="set-up-workflows-for-expense-management"></a><span data-ttu-id="134c4-103">הגדר תהליכי עבודה לניהול הוצאות</span><span class="sxs-lookup"><span data-stu-id="134c4-103">Set up workflows for Expense management</span></span>

<span data-ttu-id="134c4-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="134c4-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="134c4-105">באפשרותך להגדיר תהליך זרימת עבודה לבדיקה ולאישור מסמכי נסיעות והוצאות.</span><span class="sxs-lookup"><span data-stu-id="134c4-105">You can set up a workflow process to review and approve travel and expense documents.</span></span> <span data-ttu-id="134c4-106">באפשרותך להגדיר זרימות עבודה לדוחות הוצאות, דרישות נסיעות ובקשות למקדמות במזומן.</span><span class="sxs-lookup"><span data-stu-id="134c4-106">You can define workflows for expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="134c4-107">זרימת עבודה מייצגת תהליך עסקי ומגדירה כיצד מסמך זורם במערכת.</span><span class="sxs-lookup"><span data-stu-id="134c4-107">A workflow represents a business process and defines how a document flows through the system.</span></span> <span data-ttu-id="134c4-108">זרימת העבודה מציינת גם מי חייב להשלים משימה או לאשר מסמך.</span><span class="sxs-lookup"><span data-stu-id="134c4-108">The workflow also indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="134c4-109">ישנם מספר יתרונות לשימוש במערכת זרימת העבודה בארגון שלך:</span><span class="sxs-lookup"><span data-stu-id="134c4-109">There are several benefits of using the workflow system in your organization:</span></span>

- <span data-ttu-id="134c4-110">**תהליכים עקביים**: באפשרותך להגדיר את תהליך האישור למסמכים ספציפיים, כגון דרישות רכישה ודוחות הוצאות.</span><span class="sxs-lookup"><span data-stu-id="134c4-110">**Consistent processes**: You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="134c4-111">השימוש במערכת זרימת העבודה מסייע להבטיח עיבוד של מסמכים באופן עקבי ויעיל.</span><span class="sxs-lookup"><span data-stu-id="134c4-111">Using the workflow system helps ensure that documents are processed and approved in a consistent and efficient manner.</span></span>
- <span data-ttu-id="134c4-112">**נראות התהליך**: ניתן לעקוב אחר מדדי המצב, ההיסטוריה וביצועים של מופע זרימת עבודה ספציפי.</span><span class="sxs-lookup"><span data-stu-id="134c4-112">**Process visibility**: You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="134c4-113">זה עוזר לך לקבוע אם יש לבצע שינויים בתהליך העבודה כדי לשפר את היעילות.</span><span class="sxs-lookup"><span data-stu-id="134c4-113">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>
- <span data-ttu-id="134c4-114">**רשימת עבודה מרכזית**: המשתמשים יכולים להציג רשימת עבודה מרוכזת כדי להציג את משימות זרימת העבודה ואת האישורים שהוקצו להם.</span><span class="sxs-lookup"><span data-stu-id="134c4-114">**Centralized work list**: Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

## <a name="workflow-types"></a><span data-ttu-id="134c4-115">סוגי זרימת עבודה</span><span class="sxs-lookup"><span data-stu-id="134c4-115">Workflow types</span></span>

<span data-ttu-id="134c4-116">בטבלה הבאה רשומים סוגי תהליכי העבודה שבאפשרותך ליצור ב **ניהול הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="134c4-116">The following table lists the types of workflows that you can create in **Expense Management**.</span></span>


|              <span data-ttu-id="134c4-117"><strong>סוג</strong></span><span class="sxs-lookup"><span data-stu-id="134c4-117"><strong>Type</strong></span></span>              |                   <span data-ttu-id="134c4-118"><strong>השתמש בסוג זה כדי</strong></span><span class="sxs-lookup"><span data-stu-id="134c4-118"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|   <span data-ttu-id="134c4-119"><strong>אישור אוטומטי של דוח הוצאות</strong></span><span class="sxs-lookup"><span data-stu-id="134c4-119"><strong>Expense report auto approval</strong></span></span> |            <span data-ttu-id="134c4-120">צור זרימות עבודה לדוחות הוצאות.</span><span class="sxs-lookup"><span data-stu-id="134c4-120">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="134c4-121"><strong>פרסום אוטומטי של דוח הוצאות</strong></span><span class="sxs-lookup"><span data-stu-id="134c4-121"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="134c4-122">צור זרימות עבודה לפרסום אוטומטי של דוחות הוצאות.</span><span class="sxs-lookup"><span data-stu-id="134c4-122">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="134c4-123"><strong>פריט של סעיף הוצאה</strong></span><span class="sxs-lookup"><span data-stu-id="134c4-123"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="134c4-124">צור זרימות עבודה לאישור עבור פריטי שורה בדוחות הוצאות.</span><span class="sxs-lookup"><span data-stu-id="134c4-124">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="134c4-125"><strong>פרסום אוטומטי של פריט בדוח הוצאות</strong></span><span class="sxs-lookup"><span data-stu-id="134c4-125"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="134c4-126">צור זרימות עבודה לפרסום אוטומטי עבור פריטי שורה בדוחות הוצאות.</span><span class="sxs-lookup"><span data-stu-id="134c4-126">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="134c4-127"><strong>דרישת נסיעה</strong></span><span class="sxs-lookup"><span data-stu-id="134c4-127"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="134c4-128">צור זרימות עבודה לאישור עבור דרישות נסיעה.</span><span class="sxs-lookup"><span data-stu-id="134c4-128">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="134c4-129"><strong>בקשה למקדמה במזומן</strong></span><span class="sxs-lookup"><span data-stu-id="134c4-129"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="134c4-130">צור זרימות עבודה לאישור עבור בקשות מקדמה במזומן.</span><span class="sxs-lookup"><span data-stu-id="134c4-130">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="134c4-131"><strong>החזר מע"מ</strong></span><span class="sxs-lookup"><span data-stu-id="134c4-131"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="134c4-132">צור זרימות עבודה לאישור עבור החזרי מס ערך מוסף (מע"מ).</span><span class="sxs-lookup"><span data-stu-id="134c4-132">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |
