---
title: הערכות הוצאות
description: נושא זה מספק מידע על הגדרת או הערכת הוצאות מבוססות פרויקט.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 3f0429366c69346113003355679c055cd2c74ca3
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287059"
---
# <a name="expense-estimates"></a><span data-ttu-id="bd330-103">הערכות הוצאות</span><span class="sxs-lookup"><span data-stu-id="bd330-103">Expense estimates</span></span>
<span data-ttu-id="bd330-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="bd330-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="bd330-105">לצד הגדרת אומדנים מבוססי משאבים, Dynamics 365 Project Operations מאפשר למנהלי פרוייקטים להגדיר הוצאות מבוססות פרוייקט עבור כל פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="bd330-105">Along with defining resource-based estimates, Dynamics 365 Project Operations allows Project managers to define project-based expenses for each project.</span></span> <span data-ttu-id="bd330-106">ניתן לשייך כל פריט הוצאות למשימה ספציפית או לקטגוריית הוצאות.</span><span class="sxs-lookup"><span data-stu-id="bd330-106">Each expense item can be associated with a specific project task or expense category.</span></span> <span data-ttu-id="bd330-107">קטגוריות הוצאות מוגדרות בדרך כלל ברמה הארגונית.</span><span class="sxs-lookup"><span data-stu-id="bd330-107">Expense categories are typically defined at the organizational level.</span></span> <span data-ttu-id="bd330-108">תמחור עבור כל קטגוריית הוצאות מוגדר בדרך כלל בהיררכיה הבאה:</span><span class="sxs-lookup"><span data-stu-id="bd330-108">Pricing for each expense category is typically defined in the following hierarchy:</span></span>

- <span data-ttu-id="bd330-109">הארגון</span><span class="sxs-lookup"><span data-stu-id="bd330-109">Organization</span></span>
- <span data-ttu-id="bd330-110">לקוח</span><span class="sxs-lookup"><span data-stu-id="bd330-110">Customer</span></span>
- <span data-ttu-id="bd330-111">הצעת מחיר / חוזה</span><span class="sxs-lookup"><span data-stu-id="bd330-111">Quote/contract</span></span>

<span data-ttu-id="bd330-112">השלם את השלבים הבאים כדי להציג, להוסיף או למחוק הוצאה של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="bd330-112">Complete the following steps to view, add, or delete a project expense.</span></span>

1. <span data-ttu-id="bd330-113">עבור אל **פרויקטים**, ובחר את הפרויקט שעליו אתה רוצה לעבוד.</span><span class="sxs-lookup"><span data-stu-id="bd330-113">Go to **Projects**, and select the project you want to work on.</span></span>
2. <span data-ttu-id="bd330-114">בחר את הכרטיסיה **הערכות הפרויקט** והצג את רשימת הוצאות הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="bd330-114">Select the **Project Estimates** tab and view the list of project expenses.</span></span>
3. <span data-ttu-id="bd330-115">בחר **הוצאה חדשה** להוספת הוצאה.</span><span class="sxs-lookup"><span data-stu-id="bd330-115">Select **New Expense** to add an expense.</span></span> <span data-ttu-id="bd330-116">לחלופין, בחר הוצאה למחיקה ואז בחר **מחק הוצאה**.</span><span class="sxs-lookup"><span data-stu-id="bd330-116">Or, select an expense to delete, and then select **Delete Expense**.</span></span>

<span data-ttu-id="bd330-117">התכונות הבאות מוגדרות עובר כל פריט בשורת הוצאות:</span><span class="sxs-lookup"><span data-stu-id="bd330-117">The following attributes are defined for each expense line item:</span></span>

- <span data-ttu-id="bd330-118">**קטגוריה**: הקבוצות הנפוצות הנהוגות לתיאר כל ההוצאות שנגרמות בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="bd330-118">**Category**: The common groupings used to describe all expenses incurred on a project.</span></span>
- <span data-ttu-id="bd330-119">**תאריך התחלה**: התאריך שבו ההוצאה צפויה להיגרם.</span><span class="sxs-lookup"><span data-stu-id="bd330-119">**Start Date**: The date when the expense is forecasted to be incurred.</span></span>
- <span data-ttu-id="bd330-120">**כמות**: המספר המשוער של פריטי ההוצאות עבור קטגוריה מסוימת.</span><span class="sxs-lookup"><span data-stu-id="bd330-120">**Quantity**: The estimated number of expense items for a specific category.</span></span>
- <span data-ttu-id="bd330-121">**מחיר עלות יחידה**: מחיר היחידה המשמש לחישוב עלות ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="bd330-121">**Unit Cost Price**: The unit price used to calculate to cost of the expense.</span></span>
- <span data-ttu-id="bd330-122">**מחיר המכירה ליחידה**: מחיר היחידה המשמש לחישוב מחירי המכירה של ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="bd330-122">**Unit Sales Price**: The unit price used to calculate the sale prices of the expense.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]