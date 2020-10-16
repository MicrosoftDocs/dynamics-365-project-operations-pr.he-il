---
title: הערכות הוצאות
description: נושא זה מספק מידע על הגדרת או הערכת הוצאות מבוססות פרויקט.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 2afe4ff2f84fc5426c409e6314da73b11a4de281
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908186"
---
# <a name="expense-estimates"></a><span data-ttu-id="f30b8-103">הערכות הוצאות</span><span class="sxs-lookup"><span data-stu-id="f30b8-103">Expense estimates</span></span>
<span data-ttu-id="f30b8-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="f30b8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f30b8-105">לצד הגדרת הערכות מבוססי-משאבים, Dynamics 365 Project Operations מאפשר למנהלי פרויקטים להגדיר הוצאות מבוססות-פרוייקט עבור כל פרויקט.</span><span class="sxs-lookup"><span data-stu-id="f30b8-105">Along with defining resource-based estimates, Dynamics 365 Project Operations allows Project managers to define project-based expenses for each project.</span></span> <span data-ttu-id="f30b8-106">ניתן לשייך כל פריט הוצאות למשימה ספציפית או לקטגוריית הוצאות.</span><span class="sxs-lookup"><span data-stu-id="f30b8-106">Each expense item can be associated with a specific project task or expense category.</span></span> <span data-ttu-id="f30b8-107">קטגוריות הוצאות מוגדרות בדרך כלל ברמה הארגונית.</span><span class="sxs-lookup"><span data-stu-id="f30b8-107">Expense categories are typically defined at the organizational level.</span></span> <span data-ttu-id="f30b8-108">תמחור עבור כל קטגוריית הוצאות מוגדר בדרך כלל בהיררכיה הבאה:</span><span class="sxs-lookup"><span data-stu-id="f30b8-108">Pricing for each expense category is typically defined in the following hierarchy:</span></span>

- <span data-ttu-id="f30b8-109">הארגון</span><span class="sxs-lookup"><span data-stu-id="f30b8-109">Organization</span></span>
- <span data-ttu-id="f30b8-110">לקוח</span><span class="sxs-lookup"><span data-stu-id="f30b8-110">Customer</span></span>
- <span data-ttu-id="f30b8-111">הצעת מחיר / חוזה</span><span class="sxs-lookup"><span data-stu-id="f30b8-111">Quote/contract</span></span>

<span data-ttu-id="f30b8-112">השלם את השלבים הבאים כדי להציג, להוסיף או למחוק הוצאה של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="f30b8-112">Complete the following steps to view, add, or delete a project expense.</span></span>

1. <span data-ttu-id="f30b8-113">עבור אל **פרויקטים**, ובחר את הפרויקט שעליו אתה רוצה לעבוד.</span><span class="sxs-lookup"><span data-stu-id="f30b8-113">Go to **Projects**, and select the project you want to work on.</span></span>
2. <span data-ttu-id="f30b8-114">בחר את הכרטיסיה **הערכות הפרויקט** והצג את רשימת הוצאות הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="f30b8-114">Select the **Project Estimates** tab and view the list of project expenses.</span></span>
3. <span data-ttu-id="f30b8-115">בחר **הוצאה חדשה** להוספת הוצאה.</span><span class="sxs-lookup"><span data-stu-id="f30b8-115">Select **New Expense** to add an expense.</span></span> <span data-ttu-id="f30b8-116">לחלופין, בחר הוצאה למחיקה ואז בחר **מחק הוצאה**.</span><span class="sxs-lookup"><span data-stu-id="f30b8-116">Or, select an expense to delete, and then select **Delete Expense**.</span></span>

<span data-ttu-id="f30b8-117">התכונות הבאות מוגדרות עובר כל פריט בשורת הוצאות:</span><span class="sxs-lookup"><span data-stu-id="f30b8-117">The following attributes are defined for each expense line item:</span></span>

- <span data-ttu-id="f30b8-118">**קטגוריה**: הקבוצות הנפוצות הנהוגות לתיאר כל ההוצאות שנגרמות בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="f30b8-118">**Category**: The common groupings used to describe all expenses incurred on a project.</span></span>
- <span data-ttu-id="f30b8-119">**תאריך התחלה**: התאריך שבו ההוצאה צפויה להיגרם.</span><span class="sxs-lookup"><span data-stu-id="f30b8-119">**Start Date**: The date when the expense is forecasted to be incurred.</span></span>
- <span data-ttu-id="f30b8-120">**כמות**: המספר המשוער של פריטי ההוצאות עבור קטגוריה מסוימת.</span><span class="sxs-lookup"><span data-stu-id="f30b8-120">**Quantity**: The estimated number of expense items for a specific category.</span></span>
- <span data-ttu-id="f30b8-121">**מחיר עלות יחידה**: מחיר היחידה המשמש לחישוב עלות ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="f30b8-121">**Unit Cost Price**: The unit price used to calculate to cost of the expense.</span></span>
- <span data-ttu-id="f30b8-122">**מחיר המכירה ליחידה**: מחיר היחידה המשמש לחישוב מחירי המכירה של ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="f30b8-122">**Unit Sales Price**: The unit price used to calculate the sale prices of the expense.</span></span>

