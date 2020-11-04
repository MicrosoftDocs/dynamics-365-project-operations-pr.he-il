---
title: דוחות הוצאות ומאשרים מרובים
description: נושא זה מספק מידע על דוחות הוצאות הדורשים אישור של יותר מאדם אחד.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 548673541cee5ce598721f94415c0444995c8325
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077311"
---
# <a name="expense-reports-and-multiple-approvers"></a><span data-ttu-id="0b9ab-103">דוחות הוצאות ומאשרים מרובים</span><span class="sxs-lookup"><span data-stu-id="0b9ab-103">Expense reports and multiple approvers</span></span>

<span data-ttu-id="0b9ab-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="0b9ab-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="0b9ab-105">בהתאם למדיניות אישור ההוצאות של הארגון שלך, ייתכן שיותר מאדם אחד צריך לאשר דוח הוצאות שהוגש.</span><span class="sxs-lookup"><span data-stu-id="0b9ab-105">Depending on your organization's expense approval policies, more than one person might have to approve a submitted expense report.</span></span> <span data-ttu-id="0b9ab-106">כאשר אתה מגדיר את תהליך זרימת העבודה לאישור דוח הוצאות, באפשרותך להוסיף אלמנטים של זרימת עבודה הכוללים משימות או צעדים עבור מאשר דוח הוצאות אחד או יותר.</span><span class="sxs-lookup"><span data-stu-id="0b9ab-106">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="0b9ab-107">לדוגמה, ייתכן שתדרוש שכל דוחות ההוצאות יאושרו על ידי שני אנשים נפרדים, המנהל הישיר של העובד שהגיש את הדו"ח ורכז החשבונות.</span><span class="sxs-lookup"><span data-stu-id="0b9ab-107">For example, you might require that all expense reports be approved by two separate people, the manager of the employee who submitted the report and the Accounts payable coordinator.</span></span>

<span data-ttu-id="0b9ab-108">אם תחליט לדרוש מספר מאשרים לדוחות הוצאות, תוכל להוסיף את רכיבי זרימת העבודה באחת מהדרכים הבאות:</span><span class="sxs-lookup"><span data-stu-id="0b9ab-108">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="0b9ab-109">הוסף רכיב אישור אחד בעל שלב אחד.</span><span class="sxs-lookup"><span data-stu-id="0b9ab-109">Add one approval element that has one step.</span></span> <span data-ttu-id="0b9ab-110">לדוגמה, השלב עשוי לדרוש כי דוח ההוצאות יוקצה לקבוצת משתמשים, ויאושר על ידי 50 אחוז מחברי קבוצת המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="0b9ab-110">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="0b9ab-111">הוסף רכיב אישור אחד בעל מספר שלבים.</span><span class="sxs-lookup"><span data-stu-id="0b9ab-111">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="0b9ab-112">לדוגמה, רכיב האישור עשוי לכלול את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="0b9ab-112">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="0b9ab-113">המנהל הישיר של העובד שהגיש את דוח ההוצאות מאשר זאת.</span><span class="sxs-lookup"><span data-stu-id="0b9ab-113">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="0b9ab-114">פקיד החשבונות הזכאים מאמת את הקבלות ואת פריטי דוח ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="0b9ab-114">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="0b9ab-115">בעל התקציב מאשר את דוח ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="0b9ab-115">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="0b9ab-116">הוסף רכיבי אישור מרובים, שלכל אחד מהם שלב אחד.</span><span class="sxs-lookup"><span data-stu-id="0b9ab-116">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="0b9ab-117">לדוגמה, תוכל להוסיף רכיב אישור נפרד לכל אחד מהשלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="0b9ab-117">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="0b9ab-118">המנהל הישיר של העובד מאשר את דוח ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="0b9ab-118">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="0b9ab-119">בעל התקציב מאשר את דוח ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="0b9ab-119">The budget owner approves the expense report.</span></span>
