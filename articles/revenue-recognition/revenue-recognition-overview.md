---
title: מבט כולל על זיהוי הכנסה
description: נושא זו מספק מידע על זיהוי הכנסות ב-Project Operations.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 6844f4c5d4cda8a6a901b0302448f70f4c597f5d
ms.sourcegitcommit: 2d399bc9d07807626f0d6b2d0cf304240c47591c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 11/17/2020
ms.locfileid: "4531440"
---
# <a name="revenue-recognition-overview"></a><span data-ttu-id="8dfd7-103">מבט כולל על זיהוי הכנסה</span><span class="sxs-lookup"><span data-stu-id="8dfd7-103">Revenue recognition overview</span></span>

<span data-ttu-id="8dfd7-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="8dfd7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="8dfd7-105">ב- Dynamics 365 Project Operations, עקרונות של זיהוי הכנסות משתנים בהתאם לשיטת החיוב שנבחרה עבור פרויקט או חלק מהפרויקט.</span><span class="sxs-lookup"><span data-stu-id="8dfd7-105">In Dynamics 365 Project Operations, revenue recognition principles vary based on the selected billing method for a project or portion of the project.</span></span> <span data-ttu-id="8dfd7-106">נושא זו מספק מידע על זיהוי הכנסות ב-Project Operations.</span><span class="sxs-lookup"><span data-stu-id="8dfd7-106">This topic provides information about revenue recognition in Project Operations.</span></span>

## <a name="transactions-accounted-using-time-and-material-billing-method"></a><span data-ttu-id="8dfd7-107">עסקאות מחויבות לפי שיטת חיוב עבור זמן וחומר</span><span class="sxs-lookup"><span data-stu-id="8dfd7-107">Transactions accounted using time and material billing method</span></span>

- <span data-ttu-id="8dfd7-108">יש קשר בין עלויות לזיהוי הכנסות.</span><span class="sxs-lookup"><span data-stu-id="8dfd7-108">Cost and revenue recognition are connected.</span></span> <span data-ttu-id="8dfd7-109">עלות העסקה והמכירות שלא בוצעו נרשמות באמצעות [יומן לשילוב Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="8dfd7-109">Transaction cost and unbilled sales are posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span>
- <span data-ttu-id="8dfd7-110">עלות הפרויקט ופרופיל ההכנסות קובעים אם עסקאות מכירה שלא בוצעו נרשמות בספר החשבונות הכללי.</span><span class="sxs-lookup"><span data-stu-id="8dfd7-110">Project cost and revenue profile determine if unbilled sales transactions are posted to the general ledger.</span></span> <span data-ttu-id="8dfd7-111">אם נבחרה **צבירת הכנסות**, המערכת משתמשת בנתונים **ערך מכירות WIP** ו- **שווי מכירות שהצטברו** במהלך הפרסום.</span><span class="sxs-lookup"><span data-stu-id="8dfd7-111">If **Accrue revenue** is selected, the system uses the **WIP sales value** and the **Accrued revenue sales value** accounts during posting.</span></span> <span data-ttu-id="8dfd7-112">להלן דוגמה לשיטה זו.</span><span class="sxs-lookup"><span data-stu-id="8dfd7-112">The following is an example of this method.</span></span>  

  | <span data-ttu-id="8dfd7-113">סוג עסקה</span><span class="sxs-lookup"><span data-stu-id="8dfd7-113">Transaction type</span></span> | <span data-ttu-id="8dfd7-114">חיוב/אשראי</span><span class="sxs-lookup"><span data-stu-id="8dfd7-114">Debit/Credit</span></span> | <span data-ttu-id="8dfd7-115">סכום</span><span class="sxs-lookup"><span data-stu-id="8dfd7-115">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="8dfd7-116">ערך מכירה של WIP</span><span class="sxs-lookup"><span data-stu-id="8dfd7-116">WIP Sales value</span></span> | <span data-ttu-id="8dfd7-117">חיוב</span><span class="sxs-lookup"><span data-stu-id="8dfd7-117">Debit</span></span> | <span data-ttu-id="8dfd7-118">100</span><span class="sxs-lookup"><span data-stu-id="8dfd7-118">100</span></span> |
  | <span data-ttu-id="8dfd7-119">ערך מכירה של הכנסה נצברת</span><span class="sxs-lookup"><span data-stu-id="8dfd7-119">Accrued revenue sales value</span></span> | <span data-ttu-id="8dfd7-120">אשראי</span><span class="sxs-lookup"><span data-stu-id="8dfd7-120">Credit</span></span> | <span data-ttu-id="8dfd7-121">100</span><span class="sxs-lookup"><span data-stu-id="8dfd7-121">100</span></span> |

- <span data-ttu-id="8dfd7-122">ההכנסה מזוהה בעת הפקת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="8dfd7-122">Revenue is recognized during invoicing.</span></span> <span data-ttu-id="8dfd7-123">המערכת משתמשת בחשבון **הכנסות מחשבוניות** במהלך הפרסום.</span><span class="sxs-lookup"><span data-stu-id="8dfd7-123">The system uses the **Invoiced revenue** account during posting.</span></span> <span data-ttu-id="8dfd7-124">להלן דוגמה לשיטה זו.</span><span class="sxs-lookup"><span data-stu-id="8dfd7-124">The following is an example of this method.</span></span>  

  | <span data-ttu-id="8dfd7-125">סוג עסקה</span><span class="sxs-lookup"><span data-stu-id="8dfd7-125">Transaction type</span></span> | <span data-ttu-id="8dfd7-126">חיוב/אשראי</span><span class="sxs-lookup"><span data-stu-id="8dfd7-126">Debit/Credit</span></span> | <span data-ttu-id="8dfd7-127">סכום</span><span class="sxs-lookup"><span data-stu-id="8dfd7-127">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="8dfd7-128">יתרת לקוחות</span><span class="sxs-lookup"><span data-stu-id="8dfd7-128">Customer balance</span></span> | <span data-ttu-id="8dfd7-129">חיוב</span><span class="sxs-lookup"><span data-stu-id="8dfd7-129">Debit</span></span> | <span data-ttu-id="8dfd7-130">120</span><span class="sxs-lookup"><span data-stu-id="8dfd7-130">120</span></span> |
  | <span data-ttu-id="8dfd7-131">מס מכירות לתשלום</span><span class="sxs-lookup"><span data-stu-id="8dfd7-131">Sales tax payable</span></span> | <span data-ttu-id="8dfd7-132">אשראי</span><span class="sxs-lookup"><span data-stu-id="8dfd7-132">Credit</span></span> | <span data-ttu-id="8dfd7-133">20</span><span class="sxs-lookup"><span data-stu-id="8dfd7-133">20</span></span> |
  | <span data-ttu-id="8dfd7-134">הכנסה שחויבה</span><span class="sxs-lookup"><span data-stu-id="8dfd7-134">Invoiced Revenue</span></span> | <span data-ttu-id="8dfd7-135">אשראי</span><span class="sxs-lookup"><span data-stu-id="8dfd7-135">Credit</span></span> | <span data-ttu-id="8dfd7-136">100</span><span class="sxs-lookup"><span data-stu-id="8dfd7-136">100</span></span> |

- <span data-ttu-id="8dfd7-137">אם הצטברו הכנסות בעת רישום מכירות שלא בוצעו, המערכת תהפוך את ההכנסות שנצברו בחשבונית.</span><span class="sxs-lookup"><span data-stu-id="8dfd7-137">If revenue was accrued when the unbilled sales are posted, the system will reverse the accrued revenue at invoicing.</span></span>

  | <span data-ttu-id="8dfd7-138">סוג עסקה</span><span class="sxs-lookup"><span data-stu-id="8dfd7-138">Transaction type</span></span> | <span data-ttu-id="8dfd7-139">חיוב/אשראי</span><span class="sxs-lookup"><span data-stu-id="8dfd7-139">Debit/Credit</span></span> | <span data-ttu-id="8dfd7-140">סכום</span><span class="sxs-lookup"><span data-stu-id="8dfd7-140">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="8dfd7-141">ערך מכירה של WIP</span><span class="sxs-lookup"><span data-stu-id="8dfd7-141">WIP Sales value</span></span> | <span data-ttu-id="8dfd7-142">אשראי</span><span class="sxs-lookup"><span data-stu-id="8dfd7-142">Credit</span></span> | <span data-ttu-id="8dfd7-143">100</span><span class="sxs-lookup"><span data-stu-id="8dfd7-143">100</span></span> |
  | <span data-ttu-id="8dfd7-144">ערך מכירה של הכנסה נצברת</span><span class="sxs-lookup"><span data-stu-id="8dfd7-144">Accrued revenue sales value</span></span> | <span data-ttu-id="8dfd7-145">חיוב</span><span class="sxs-lookup"><span data-stu-id="8dfd7-145">Debit</span></span> | <span data-ttu-id="8dfd7-146">100</span><span class="sxs-lookup"><span data-stu-id="8dfd7-146">100</span></span> |

## <a name="transactions-accounted-using-the-fixed-price-billing-method"></a><span data-ttu-id="8dfd7-147">עסקאות מחויבות לפי שיטת חיוב של מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="8dfd7-147">Transactions accounted using the fixed price billing method</span></span>

- <span data-ttu-id="8dfd7-148">אין קשר בין עלויות לזיהוי הכנסות.</span><span class="sxs-lookup"><span data-stu-id="8dfd7-148">Cost and revenue recognition are separate.</span></span> <span data-ttu-id="8dfd7-149">עלות העסקה מפורסמת באמצעות [יומן לשילוב Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="8dfd7-149">Transaction cost is posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="8dfd7-150">לא נוצרות עסקאות מכירה שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="8dfd7-150">Unbilled sales transactions aren't created.</span></span>
- <span data-ttu-id="8dfd7-151">הכנסה יכולה להיות מזוהה במהלך הפקת החשבונית אם לעלות הפרויקט ולפרופיל ההכנסות יש **עקרון המשמש לחישובי השלמת הפרויקט** שמוגדר **ללא WIP**.</span><span class="sxs-lookup"><span data-stu-id="8dfd7-151">Revenue can be recognized during invoicing if the project cost and revenue profile have **Principle used for project completion calculations** set to **No WIP**.</span></span> <span data-ttu-id="8dfd7-152">השתמש בשיטה זו בפרויקטים פשוטים לטווח קצר.</span><span class="sxs-lookup"><span data-stu-id="8dfd7-152">Only use this method for short term, simple projects.</span></span>
- <span data-ttu-id="8dfd7-153">ניתן לזהות הכנסות באמצעות אומדני הכנסות עם מחירים קבועים, כאשר השיטה **חוזה שהושלם** או **זיהוי אחוזים מהכנסות שהושלמו**.</span><span class="sxs-lookup"><span data-stu-id="8dfd7-153">Revenue can be recognized using fixed price revenue estimates, with either the **Completed contract** or **Percent completion revenue recognition** method.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="8dfd7-154">משאבים נוספים</span><span class="sxs-lookup"><span data-stu-id="8dfd7-154">Additional resources</span></span>
[<span data-ttu-id="8dfd7-155">מאמר על קביעת תצורה של חשבונאות לפרויקטים הניתנים לחיוב</span><span class="sxs-lookup"><span data-stu-id="8dfd7-155">Configure accounting for billable projects article</span></span>](../project-accounting/configure-accounting-billable-projects.md)

[<span data-ttu-id="8dfd7-156">פרוייקטים של הערכת הכנסה במחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="8dfd7-156">Fixed price revenue estimate projects</span></span>](rev-rec-percentage-completion-method.md)

[<span data-ttu-id="8dfd7-157">ניהול הערכות הכנסה</span><span class="sxs-lookup"><span data-stu-id="8dfd7-157">Manage revenue estimates</span></span>](rev-rec-completed-contract-method.md)

[<span data-ttu-id="8dfd7-158">עלות להשלמת שיטות</span><span class="sxs-lookup"><span data-stu-id="8dfd7-158">Cost to complete methods</span></span>](cost-complete-methods.md)
