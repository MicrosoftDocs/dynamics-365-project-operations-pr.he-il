---
title: מאשרים מרובים בדוח הוצאות
description: נושא זה מספק מידע על דוחות הוצאות הדורשים את אישורם של אנשים מרובים.
author: saraschi2
manager: AnnBe
ms.date: 02/23/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvExpensesReportList
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: ce24b156a268f9f5aada35f9314d2d9c6607200b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077464"
---
# <a name="multiple-approvers-on-an-expense-report"></a><span data-ttu-id="2df15-103">מאשרים מרובים בדוח הוצאות</span><span class="sxs-lookup"><span data-stu-id="2df15-103">Multiple approvers on an expense report</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="2df15-104">בהתאם לקווי המדיניות של הארגון שלך לאישור הוצאות, ייתכן שיותר מאדם אחד יצטרך לאשר דוח הוצאות שהוגש על ידי עובד.</span><span class="sxs-lookup"><span data-stu-id="2df15-104">Depending on your organization's expense approval policies, more than one person might have to approve an expense report that is submitted by an employee.</span></span> <span data-ttu-id="2df15-105">כאשר אתה מגדיר את תהליך זרימת העבודה לאישור דוח הוצאות, באפשרותך להוסיף אלמנטים של זרימת עבודה הכוללים משימות או צעדים עבור מאשר דוח הוצאות אחד או יותר.</span><span class="sxs-lookup"><span data-stu-id="2df15-105">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="2df15-106">לדוגמה, ייתכן שתדרוש שכל דוחות ההוצאות יאושרו קודם על ידי המנהל הישיר של העובד שהגיש את הדו"ח ואחר כך על ידי רכז חשבונות זכאים.</span><span class="sxs-lookup"><span data-stu-id="2df15-106">For example, you might require that all expense reports be approved first by the manager of the employee who submitted the report and then by the Accounts payable coordinator.</span></span>

<span data-ttu-id="2df15-107">אם תחליט לדרוש מספר מאשרים לדוחות הוצאות, תוכל להוסיף את רכיבי זרימת העבודה באחת מהדרכים הבאות:</span><span class="sxs-lookup"><span data-stu-id="2df15-107">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="2df15-108">הוסף רכיב אישור אחד בעל שלב אחד.</span><span class="sxs-lookup"><span data-stu-id="2df15-108">Add one approval element that has one step.</span></span> <span data-ttu-id="2df15-109">לדוגמה, השלב עשוי לדרוש כי דוח ההוצאות יוקצה לקבוצת משתמשים, ויאושר על ידי 50 אחוז מחברי קבוצת המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="2df15-109">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="2df15-110">הוסף רכיב אישור אחד בעל מספר שלבים.</span><span class="sxs-lookup"><span data-stu-id="2df15-110">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="2df15-111">לדוגמה, רכיב האישור עשוי לכלול את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="2df15-111">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="2df15-112">המנהל הישיר של העובד שהגיש את דוח ההוצאות מאשר זאת.</span><span class="sxs-lookup"><span data-stu-id="2df15-112">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="2df15-113">פקיד החשבונות הזכאים מאמת את הקבלות ואת פריטי דוח ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="2df15-113">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="2df15-114">בעל התקציב מאשר את דוח ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="2df15-114">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="2df15-115">הוסף רכיבי אישור מרובים, שלכל אחד מהם שלב אחד.</span><span class="sxs-lookup"><span data-stu-id="2df15-115">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="2df15-116">לדוגמה, תוכל להוסיף רכיב אישור נפרד לכל אחד מהשלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="2df15-116">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="2df15-117">המנהל הישיר של העובד מאשר את דוח ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="2df15-117">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="2df15-118">בעל התקציב מאשר את דוח ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="2df15-118">The budget owner approves the expense report.</span></span>
