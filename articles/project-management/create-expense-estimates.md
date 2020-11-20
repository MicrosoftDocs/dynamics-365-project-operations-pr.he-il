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
ms.openlocfilehash: 10872366453985561bda0c07e50cff7f5f6d333e
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131704"
---
# <a name="expense-estimates"></a><span data-ttu-id="47156-103">הערכות הוצאות</span><span class="sxs-lookup"><span data-stu-id="47156-103">Expense estimates</span></span>
<span data-ttu-id="47156-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="47156-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="47156-105">לצד הגדרת הערכות מבוססי-משאבים, Dynamics 365 Project Operations מאפשר למנהלי פרויקטים להגדיר הוצאות מבוססות-פרוייקט עבור כל פרויקט.</span><span class="sxs-lookup"><span data-stu-id="47156-105">Along with defining resource-based estimates, Dynamics 365 Project Operations allows Project managers to define project-based expenses for each project.</span></span> <span data-ttu-id="47156-106">ניתן לשייך כל פריט הוצאות למשימה ספציפית או לקטגוריית הוצאות.</span><span class="sxs-lookup"><span data-stu-id="47156-106">Each expense item can be associated with a specific project task or expense category.</span></span> <span data-ttu-id="47156-107">קטגוריות הוצאות מוגדרות בדרך כלל ברמה הארגונית.</span><span class="sxs-lookup"><span data-stu-id="47156-107">Expense categories are typically defined at the organizational level.</span></span> <span data-ttu-id="47156-108">תמחור עבור כל קטגוריית הוצאות מוגדר בדרך כלל בהיררכיה הבאה:</span><span class="sxs-lookup"><span data-stu-id="47156-108">Pricing for each expense category is typically defined in the following hierarchy:</span></span>

- <span data-ttu-id="47156-109">הארגון</span><span class="sxs-lookup"><span data-stu-id="47156-109">Organization</span></span>
- <span data-ttu-id="47156-110">לקוח</span><span class="sxs-lookup"><span data-stu-id="47156-110">Customer</span></span>
- <span data-ttu-id="47156-111">הצעת מחיר / חוזה</span><span class="sxs-lookup"><span data-stu-id="47156-111">Quote/contract</span></span>

<span data-ttu-id="47156-112">השלם את השלבים הבאים כדי להציג, להוסיף או למחוק הוצאה של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="47156-112">Complete the following steps to view, add, or delete a project expense.</span></span>

1. <span data-ttu-id="47156-113">עבור אל **פרויקטים**, ובחר את הפרויקט שעליו אתה רוצה לעבוד.</span><span class="sxs-lookup"><span data-stu-id="47156-113">Go to **Projects**, and select the project you want to work on.</span></span>
2. <span data-ttu-id="47156-114">בחר את הכרטיסיה **הערכות הפרויקט** והצג את רשימת הוצאות הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="47156-114">Select the **Project Estimates** tab and view the list of project expenses.</span></span>
3. <span data-ttu-id="47156-115">בחר **הוצאה חדשה** להוספת הוצאה.</span><span class="sxs-lookup"><span data-stu-id="47156-115">Select **New Expense** to add an expense.</span></span> <span data-ttu-id="47156-116">לחלופין, בחר הוצאה למחיקה ואז בחר **מחק הוצאה**.</span><span class="sxs-lookup"><span data-stu-id="47156-116">Or, select an expense to delete, and then select **Delete Expense**.</span></span>

<span data-ttu-id="47156-117">התכונות הבאות מוגדרות עובר כל פריט בשורת הוצאות:</span><span class="sxs-lookup"><span data-stu-id="47156-117">The following attributes are defined for each expense line item:</span></span>

- <span data-ttu-id="47156-118">**קטגוריה**: הקבוצות הנפוצות הנהוגות לתיאר כל ההוצאות שנגרמות בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="47156-118">**Category**: The common groupings used to describe all expenses incurred on a project.</span></span>
- <span data-ttu-id="47156-119">**תאריך התחלה**: התאריך שבו ההוצאה צפויה להיגרם.</span><span class="sxs-lookup"><span data-stu-id="47156-119">**Start Date**: The date when the expense is forecasted to be incurred.</span></span>
- <span data-ttu-id="47156-120">**כמות**: המספר המשוער של פריטי ההוצאות עבור קטגוריה מסוימת.</span><span class="sxs-lookup"><span data-stu-id="47156-120">**Quantity**: The estimated number of expense items for a specific category.</span></span>
- <span data-ttu-id="47156-121">**מחיר עלות יחידה**: מחיר היחידה המשמש לחישוב עלות ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="47156-121">**Unit Cost Price**: The unit price used to calculate to cost of the expense.</span></span>
- <span data-ttu-id="47156-122">**מחיר המכירה ליחידה**: מחיר היחידה המשמש לחישוב מחירי המכירה של ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="47156-122">**Unit Sales Price**: The unit price used to calculate the sale prices of the expense.</span></span>

