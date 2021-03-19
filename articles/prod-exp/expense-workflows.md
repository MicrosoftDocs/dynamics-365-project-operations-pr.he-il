---
title: הגדרת זרימות עבודה לניהול הוצאות
description: באפשרותך להגדיר תהליך זרימת עבודה לבדיקה ולאישור מסמכי נסיעות והוצאות.
author: ShylaThompson
manager: AnnBe
ms.date: 09/13/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WorkflowtableListPageRnr
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 36ab1edc4769013684fa9248e6c5eac025637bbd
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271624"
---
# <a name="set-up-expense-management-workflows"></a><span data-ttu-id="16a06-103">הגדרת זרימות עבודה לניהול הוצאות</span><span class="sxs-lookup"><span data-stu-id="16a06-103">Set up Expense management workflows</span></span>

<span data-ttu-id="16a06-104">באפשרותך להגדיר תהליך זרימת עבודה המשמש לבדיקה ולאישור מסמכי נסיעות והוצאות.</span><span class="sxs-lookup"><span data-stu-id="16a06-104">You can set up a workflow process that is used to review and approve travel and expense documents.</span></span> <span data-ttu-id="16a06-105">המסמכים אשר עוברם ניתן להגדיר זרימות עבודה כוללים דוחות הוצאות, דרישות נסיעות ובקשות למקדמות במזומן.</span><span class="sxs-lookup"><span data-stu-id="16a06-105">The documents for which workflows can be defined include expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="16a06-106">זרימת עבודה מייצגת תהליך עסקי.</span><span class="sxs-lookup"><span data-stu-id="16a06-106">A workflow represents a business process.</span></span> <span data-ttu-id="16a06-107">הוא מגדיר כיצד מסמך זורם במערכת ומציין מי חייב לבצע משימה או לאשר מסמך.</span><span class="sxs-lookup"><span data-stu-id="16a06-107">It defines how a document flows through the system and indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="16a06-108">ישנם מספר יתרונות לשימוש במערכת זרימת העבודה בארגון שלך:</span><span class="sxs-lookup"><span data-stu-id="16a06-108">There are several benefits of using the workflow system in your organization:</span></span>

-   <span data-ttu-id="16a06-109">**תהליכים עקביים** – באפשרותך להגדיר את תהליך האישור למסמכים ספציפיים, כגון דרישות רכישה ודוחות הוצאות.</span><span class="sxs-lookup"><span data-stu-id="16a06-109">**Consistent processes** — You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="16a06-110">השימוש במערכת זרימת העבודה מסייע בהבטחת עיבוד עקבי ויעיל של מסמכים.</span><span class="sxs-lookup"><span data-stu-id="16a06-110">Using the workflow system helps to ensure that documents are processed and approved in a consistent and efficient manner.</span></span>

-   <span data-ttu-id="16a06-111">נראות התהליך – ניתן לעקוב אחר מדדי המצב, ההיסטוריה וביצועים של מופע זרימת עבודה ספציפי.</span><span class="sxs-lookup"><span data-stu-id="16a06-111">Process visibility — You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="16a06-112">זה עוזר לך לקבוע אם יש לבצע שינויים בתהליך העבודה כדי לשפר את היעילות.</span><span class="sxs-lookup"><span data-stu-id="16a06-112">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>

-   <span data-ttu-id="16a06-113">רשימת עבודה מרכזית – משתמשים יכולים להציג רשימת עבודה מרוכזת כדי להציג את משימות זרימת העבודה ואת האישורים שהוקצו להם.</span><span class="sxs-lookup"><span data-stu-id="16a06-113">Centralized work list — Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

<span data-ttu-id="16a06-114">**סוגי זרימות העבודה שניתן ליצור**</span><span class="sxs-lookup"><span data-stu-id="16a06-114">**The types of workflows you can create**</span></span>

<span data-ttu-id="16a06-115">בטבלה הבאה רשומים סוגי זרימות העבודה שניתן ליצור ב **הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="16a06-115">The following table lists the types of workflows that you can create in **Expense**.</span></span>


|              <span data-ttu-id="16a06-116"><strong>סוג</strong></span><span class="sxs-lookup"><span data-stu-id="16a06-116"><strong>Type</strong></span></span>              |                   <span data-ttu-id="16a06-117"><strong>השתמש בסוג זה כדי</strong></span><span class="sxs-lookup"><span data-stu-id="16a06-117"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|         <span data-ttu-id="16a06-118"><strong>דוח הוצאות</strong></span><span class="sxs-lookup"><span data-stu-id="16a06-118"><strong>Expense report</strong></span></span>         |            <span data-ttu-id="16a06-119">צור זרימות עבודה לדוחות הוצאות.</span><span class="sxs-lookup"><span data-stu-id="16a06-119">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="16a06-120"><strong>פרסום אוטומטי של דוח הוצאות</strong></span><span class="sxs-lookup"><span data-stu-id="16a06-120"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="16a06-121">צור זרימות עבודה לפרסום אוטומטי של דוחות הוצאות.</span><span class="sxs-lookup"><span data-stu-id="16a06-121">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="16a06-122"><strong>פריט של סעיף הוצאה</strong></span><span class="sxs-lookup"><span data-stu-id="16a06-122"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="16a06-123">צור זרימות עבודה לאישור עבור פריטי שורה בדוחות הוצאות.</span><span class="sxs-lookup"><span data-stu-id="16a06-123">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="16a06-124"><strong>פרסום אוטומטי של פריט בדוח הוצאות</strong></span><span class="sxs-lookup"><span data-stu-id="16a06-124"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="16a06-125">צור זרימות עבודה לפרסום אוטומטי עבור פריטי שורה בדוחות הוצאות.</span><span class="sxs-lookup"><span data-stu-id="16a06-125">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="16a06-126"><strong>דרישת נסיעה</strong></span><span class="sxs-lookup"><span data-stu-id="16a06-126"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="16a06-127">צור זרימות עבודה לאישור עבור דרישות נסיעה.</span><span class="sxs-lookup"><span data-stu-id="16a06-127">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="16a06-128"><strong>בקשה למקדמה במזומן</strong></span><span class="sxs-lookup"><span data-stu-id="16a06-128"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="16a06-129">צור זרימות עבודה לאישור עבור בקשות מקדמה במזומן.</span><span class="sxs-lookup"><span data-stu-id="16a06-129">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="16a06-130"><strong>החזר מע"מ</strong></span><span class="sxs-lookup"><span data-stu-id="16a06-130"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="16a06-131">צור זרימות עבודה לאישור עבור החזרי מס ערך מוסף (מע"מ).</span><span class="sxs-lookup"><span data-stu-id="16a06-131">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |



[!INCLUDE[footer-include](../includes/footer-banner.md)]