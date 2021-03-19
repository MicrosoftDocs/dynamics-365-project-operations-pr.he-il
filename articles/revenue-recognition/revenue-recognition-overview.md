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
ms.openlocfilehash: 5e77a0442f634a50f8099fadec42ff400fee0e81
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5278869"
---
# <a name="revenue-recognition-overview"></a><span data-ttu-id="80052-103">מבט כולל על זיהוי הכנסה</span><span class="sxs-lookup"><span data-stu-id="80052-103">Revenue recognition overview</span></span>

<span data-ttu-id="80052-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="80052-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="80052-105">ב- Dynamics 365 Project Operations, עקרונות של זיהוי הכנסות משתנים בהתאם לשיטת החיוב שנבחרה עבור פרויקט או חלק מהפרויקט.</span><span class="sxs-lookup"><span data-stu-id="80052-105">In Dynamics 365 Project Operations, revenue recognition principles vary based on the selected billing method for a project or portion of the project.</span></span> <span data-ttu-id="80052-106">נושא זו מספק מידע על זיהוי הכנסות ב-Project Operations.</span><span class="sxs-lookup"><span data-stu-id="80052-106">This topic provides information about revenue recognition in Project Operations.</span></span>

## <a name="transactions-accounted-using-time-and-material-billing-method"></a><span data-ttu-id="80052-107">עסקאות מחויבות לפי שיטת חיוב עבור זמן וחומר</span><span class="sxs-lookup"><span data-stu-id="80052-107">Transactions accounted using time and material billing method</span></span>

- <span data-ttu-id="80052-108">יש קשר בין עלויות לזיהוי הכנסות.</span><span class="sxs-lookup"><span data-stu-id="80052-108">Cost and revenue recognition are connected.</span></span> <span data-ttu-id="80052-109">עלות העסקה והמכירות שלא בוצעו נרשמות באמצעות [יומן לשילוב Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="80052-109">Transaction cost and unbilled sales are posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span>
- <span data-ttu-id="80052-110">עלות הפרויקט ופרופיל ההכנסות קובעים אם עסקאות מכירה שלא בוצעו נרשמות בספר החשבונות הכללי.</span><span class="sxs-lookup"><span data-stu-id="80052-110">Project cost and revenue profile determine if unbilled sales transactions are posted to the general ledger.</span></span> <span data-ttu-id="80052-111">אם נבחרה **צבירת הכנסות**, המערכת משתמשת בנתונים **ערך מכירות WIP** ו- **שווי מכירות שהצטברו** במהלך הפרסום.</span><span class="sxs-lookup"><span data-stu-id="80052-111">If **Accrue revenue** is selected, the system uses the **WIP sales value** and the **Accrued revenue sales value** accounts during posting.</span></span> <span data-ttu-id="80052-112">להלן דוגמה לשיטה זו.</span><span class="sxs-lookup"><span data-stu-id="80052-112">The following is an example of this method.</span></span>  

  | <span data-ttu-id="80052-113">סוג עסקה</span><span class="sxs-lookup"><span data-stu-id="80052-113">Transaction type</span></span> | <span data-ttu-id="80052-114">חיוב/אשראי</span><span class="sxs-lookup"><span data-stu-id="80052-114">Debit/Credit</span></span> | <span data-ttu-id="80052-115">סכום</span><span class="sxs-lookup"><span data-stu-id="80052-115">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="80052-116">ערך מכירה של WIP</span><span class="sxs-lookup"><span data-stu-id="80052-116">WIP Sales value</span></span> | <span data-ttu-id="80052-117">חיוב</span><span class="sxs-lookup"><span data-stu-id="80052-117">Debit</span></span> | <span data-ttu-id="80052-118">100</span><span class="sxs-lookup"><span data-stu-id="80052-118">100</span></span> |
  | <span data-ttu-id="80052-119">ערך מכירה של הכנסה נצברת</span><span class="sxs-lookup"><span data-stu-id="80052-119">Accrued revenue sales value</span></span> | <span data-ttu-id="80052-120">אשראי</span><span class="sxs-lookup"><span data-stu-id="80052-120">Credit</span></span> | <span data-ttu-id="80052-121">100</span><span class="sxs-lookup"><span data-stu-id="80052-121">100</span></span> |

- <span data-ttu-id="80052-122">ההכנסה מזוהה בעת הפקת החשבונית.</span><span class="sxs-lookup"><span data-stu-id="80052-122">Revenue is recognized during invoicing.</span></span> <span data-ttu-id="80052-123">המערכת משתמשת בחשבון **הכנסות מחשבוניות** במהלך הפרסום.</span><span class="sxs-lookup"><span data-stu-id="80052-123">The system uses the **Invoiced revenue** account during posting.</span></span> <span data-ttu-id="80052-124">להלן דוגמה לשיטה זו.</span><span class="sxs-lookup"><span data-stu-id="80052-124">The following is an example of this method.</span></span>  

  | <span data-ttu-id="80052-125">סוג עסקה</span><span class="sxs-lookup"><span data-stu-id="80052-125">Transaction type</span></span> | <span data-ttu-id="80052-126">חיוב/אשראי</span><span class="sxs-lookup"><span data-stu-id="80052-126">Debit/Credit</span></span> | <span data-ttu-id="80052-127">סכום</span><span class="sxs-lookup"><span data-stu-id="80052-127">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="80052-128">יתרת לקוחות</span><span class="sxs-lookup"><span data-stu-id="80052-128">Customer balance</span></span> | <span data-ttu-id="80052-129">חיוב</span><span class="sxs-lookup"><span data-stu-id="80052-129">Debit</span></span> | <span data-ttu-id="80052-130">120</span><span class="sxs-lookup"><span data-stu-id="80052-130">120</span></span> |
  | <span data-ttu-id="80052-131">מס מכירות לתשלום</span><span class="sxs-lookup"><span data-stu-id="80052-131">Sales tax payable</span></span> | <span data-ttu-id="80052-132">אשראי</span><span class="sxs-lookup"><span data-stu-id="80052-132">Credit</span></span> | <span data-ttu-id="80052-133">20</span><span class="sxs-lookup"><span data-stu-id="80052-133">20</span></span> |
  | <span data-ttu-id="80052-134">הכנסה שחויבה</span><span class="sxs-lookup"><span data-stu-id="80052-134">Invoiced Revenue</span></span> | <span data-ttu-id="80052-135">אשראי</span><span class="sxs-lookup"><span data-stu-id="80052-135">Credit</span></span> | <span data-ttu-id="80052-136">100</span><span class="sxs-lookup"><span data-stu-id="80052-136">100</span></span> |

- <span data-ttu-id="80052-137">אם הצטברו הכנסות בעת רישום מכירות שלא בוצעו, המערכת תהפוך את ההכנסות שנצברו בחשבונית.</span><span class="sxs-lookup"><span data-stu-id="80052-137">If revenue was accrued when the unbilled sales are posted, the system will reverse the accrued revenue at invoicing.</span></span>

  | <span data-ttu-id="80052-138">סוג עסקה</span><span class="sxs-lookup"><span data-stu-id="80052-138">Transaction type</span></span> | <span data-ttu-id="80052-139">חיוב/אשראי</span><span class="sxs-lookup"><span data-stu-id="80052-139">Debit/Credit</span></span> | <span data-ttu-id="80052-140">סכום</span><span class="sxs-lookup"><span data-stu-id="80052-140">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="80052-141">ערך מכירה של WIP</span><span class="sxs-lookup"><span data-stu-id="80052-141">WIP Sales value</span></span> | <span data-ttu-id="80052-142">אשראי</span><span class="sxs-lookup"><span data-stu-id="80052-142">Credit</span></span> | <span data-ttu-id="80052-143">100</span><span class="sxs-lookup"><span data-stu-id="80052-143">100</span></span> |
  | <span data-ttu-id="80052-144">ערך מכירה של הכנסה נצברת</span><span class="sxs-lookup"><span data-stu-id="80052-144">Accrued revenue sales value</span></span> | <span data-ttu-id="80052-145">חיוב</span><span class="sxs-lookup"><span data-stu-id="80052-145">Debit</span></span> | <span data-ttu-id="80052-146">100</span><span class="sxs-lookup"><span data-stu-id="80052-146">100</span></span> |

## <a name="transactions-accounted-using-the-fixed-price-billing-method"></a><span data-ttu-id="80052-147">עסקאות מחויבות לפי שיטת חיוב של מחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="80052-147">Transactions accounted using the fixed price billing method</span></span>

- <span data-ttu-id="80052-148">אין קשר בין עלויות לזיהוי הכנסות.</span><span class="sxs-lookup"><span data-stu-id="80052-148">Cost and revenue recognition are separate.</span></span> <span data-ttu-id="80052-149">עלות העסקה מפורסמת באמצעות [יומן לשילוב Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="80052-149">Transaction cost is posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="80052-150">לא נוצרות עסקאות מכירה שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="80052-150">Unbilled sales transactions aren't created.</span></span>
- <span data-ttu-id="80052-151">הכנסה יכולה להיות מזוהה במהלך הפקת החשבונית אם לעלות הפרויקט ולפרופיל ההכנסות יש **עקרון המשמש לחישובי השלמת הפרויקט** שמוגדר **ללא WIP**.</span><span class="sxs-lookup"><span data-stu-id="80052-151">Revenue can be recognized during invoicing if the project cost and revenue profile have **Principle used for project completion calculations** set to **No WIP**.</span></span> <span data-ttu-id="80052-152">השתמש בשיטה זו בפרויקטים פשוטים לטווח קצר.</span><span class="sxs-lookup"><span data-stu-id="80052-152">Only use this method for short term, simple projects.</span></span>
- <span data-ttu-id="80052-153">ניתן לזהות הכנסות באמצעות אומדני הכנסות עם מחירים קבועים, כאשר השיטה **חוזה שהושלם** או **זיהוי אחוזים מהכנסות שהושלמו**.</span><span class="sxs-lookup"><span data-stu-id="80052-153">Revenue can be recognized using fixed price revenue estimates, with either the **Completed contract** or **Percent completion revenue recognition** method.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="80052-154">משאבים נוספים</span><span class="sxs-lookup"><span data-stu-id="80052-154">Additional resources</span></span>
[<span data-ttu-id="80052-155">מאמר על קביעת תצורה של חשבונאות לפרויקטים הניתנים לחיוב</span><span class="sxs-lookup"><span data-stu-id="80052-155">Configure accounting for billable projects article</span></span>](../project-accounting/configure-accounting-billable-projects.md)

[<span data-ttu-id="80052-156">פרוייקטים של הערכת הכנסה במחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="80052-156">Fixed price revenue estimate projects</span></span>](rev-rec-percentage-completion-method.md)

[<span data-ttu-id="80052-157">ניהול הערכות הכנסה</span><span class="sxs-lookup"><span data-stu-id="80052-157">Manage revenue estimates</span></span>](rev-rec-completed-contract-method.md)

[<span data-ttu-id="80052-158">עלות להשלמת שיטות</span><span class="sxs-lookup"><span data-stu-id="80052-158">Cost to complete methods</span></span>](cost-complete-methods.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]