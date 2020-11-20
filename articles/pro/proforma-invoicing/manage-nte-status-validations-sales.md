---
title: ניהול מצב ואימות של 'אין לחרוג'
description: נושא זה מספק מידע אודות בדיקות מגבולת 'אין לחרוג' שמבוצעות ב-Project Operations.
author: rumant
manager: Annbe
ms.date: 10/22/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 09dea414e91a365f33bd23089c427b5f63f55c8e
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4129994"
---
# <a name="manage-not-to-exceed-status-and-validations"></a><span data-ttu-id="b86db-103">ניהול מצב ואימות של 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="b86db-103">Manage not-to-exceed status and validations</span></span> 

<span data-ttu-id="b86db-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="b86db-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

## <a name="not-to-exceed-on-approvals"></a><span data-ttu-id="b86db-105">'אין לחרוג' באישורים</span><span class="sxs-lookup"><span data-stu-id="b86db-105">Not-to-exceed on approvals</span></span>

<span data-ttu-id="b86db-106">כאשר מוגש ערך זמן או הוצאה, נוצרת רשומת אישור.</span><span class="sxs-lookup"><span data-stu-id="b86db-106">When a time or expense entry is submitted, an approval record is created.</span></span> <span data-ttu-id="b86db-107">אם האישור ניתן לחיוב וממפה לסעיף חוזה של זמן וחומרים, המערכת מבצעת בדיקת אימות למגבלות 'אין לחרוג' ברמות הבאות:</span><span class="sxs-lookup"><span data-stu-id="b86db-107">If the approval is chargeable and maps to a time and material contract line, the system completes a not-to-exceed validation check at the following levels:</span></span>

  - <span data-ttu-id="b86db-108">בודקת מול המגבלה שהוגדרה ללקוח סעיף חוזה הפרויקט</span><span class="sxs-lookup"><span data-stu-id="b86db-108">Check against the limit set up for the customer on the project contract line</span></span>
  - <span data-ttu-id="b86db-109">בודקת מול המגבלה שהוגדרה בסעיף החוזה</span><span class="sxs-lookup"><span data-stu-id="b86db-109">Check against the limit set up on the contract line</span></span>
  - <span data-ttu-id="b86db-110">בודקת מול המגבלה שהוגדרה עבור הלקוח</span><span class="sxs-lookup"><span data-stu-id="b86db-110">Check against the limit set up for the customer</span></span>
  - <span data-ttu-id="b86db-111">בודקת מול המגבלה שהוגדרה בחוזה</span><span class="sxs-lookup"><span data-stu-id="b86db-111">Check against the limit set up on the contract</span></span>

<span data-ttu-id="b86db-112">הבדיקות בכל רמה כוללות הבטחה שכמות ערך המכירה באישור זה לא תפר את מגבלת 'אין לחרוג' באותה הרמה, לאחר התחשבות בסכום מצבור פרטי העבודה של חיוב שכבר נרשם, והסכום שעבורו הוגשו חשבוניות עד כה ברמה זו.</span><span class="sxs-lookup"><span data-stu-id="b86db-112">The checks at each level involve ensuring that the amount of sales value on this approval will not violate the not-to-exceed limit at that level after accounting for the amount of billing backlog already recorded, and the amount invoiced to date at that level.</span></span>

<span data-ttu-id="b86db-113">אם הבדיקה עוברת, האישור מקבל מצב אימות של **הצלחה**.</span><span class="sxs-lookup"><span data-stu-id="b86db-113">If the check passes, the approval is given a validation status of **Success**.</span></span>

<span data-ttu-id="b86db-114">אם הבדיקה נכשלת, האישור מקבל מצב אימות של **נכשל**.</span><span class="sxs-lookup"><span data-stu-id="b86db-114">If the check fails, the approval is given a validation status of **Failed**.</span></span> <span data-ttu-id="b86db-115">פרט האימות של 'אין לחרוג' יודיע למשתמש באיזו רמה האימות נכשל.</span><span class="sxs-lookup"><span data-stu-id="b86db-115">The not-to-exceed validation detail will inform the user at which level the validation failed.</span></span>

<span data-ttu-id="b86db-116">כאשר ערך הזמן או ההוצאה שהוגשו נחשבת כבלתי ניתנות לחיוב, מצב האימות של 'אין לחרוג' מוגדר ל **לא ישים** עם פרט האימות שווה ל **לא ישים**.</span><span class="sxs-lookup"><span data-stu-id="b86db-116">When the submitted time or expense entry is considered non-chargeable, the not-to-exceed validation status is set to **Not Applicable** with the validation detail equal to **Not applicable**.</span></span>

## <a name="not-to-exceed-on-unbilled-sales-actuals"></a><span data-ttu-id="b86db-117">'אין לחרוג' בנתונים בפועל של מכירות שטרם חויבו</span><span class="sxs-lookup"><span data-stu-id="b86db-117">Not-to-exceed on unbilled sales actuals</span></span>

<span data-ttu-id="b86db-118">כאשר מאושרת ערך זמן או הוצאה, נוצרים רשומות של עלויות ומכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="b86db-118">When a time or expense entry is approved, cost and unbilled sales actuals records are created.</span></span> <span data-ttu-id="b86db-119">אם הנתון בפועל של המכירות שנוצר ניתן לחיוב וממפה לסעיף חוזה של זמן וחומרים, אפליקציה מבצעת בדיקת אימות למגבלות 'אין לחרוג' ברמות הבאות:</span><span class="sxs-lookup"><span data-stu-id="b86db-119">If the unbilled sales actual being created is chargeable and maps to a time and material contract line, the application performs a not-to-exceed validation check at the following levels:</span></span>

  - <span data-ttu-id="b86db-120">בודקת מול המגבלה שהוגדרה ללקוח של סעיף חוזה הפרויקט</span><span class="sxs-lookup"><span data-stu-id="b86db-120">Check against the limit set up for the customer of the project contract line</span></span>
  - <span data-ttu-id="b86db-121">בודקת מול המגבלה שהוגדרה בסעיף החוזה</span><span class="sxs-lookup"><span data-stu-id="b86db-121">Check against the limit set up on the contract line</span></span>
  - <span data-ttu-id="b86db-122">בודקת מול המגבלה שהוגדרה עבור הלקוח</span><span class="sxs-lookup"><span data-stu-id="b86db-122">Check against the limit set up for the customer</span></span>
  - <span data-ttu-id="b86db-123">בודקת מול המגבלה שהוגדרה בחוזה</span><span class="sxs-lookup"><span data-stu-id="b86db-123">Check against the limit set up on the contract</span></span>

<span data-ttu-id="b86db-124">הבדיקות בכל רמה כוללות הבטחה שכמות ערך המכירה בנתון בפועל זה לא תפר את מגבלת 'אין לחרוג' באותה הרמה, לאחר התחשבות בסכום מצבור פרטי העבודה של חיוב שכבר נרשם, והסכום שעבורו הוגשו חשבוניות עד כה ברמה זו.</span><span class="sxs-lookup"><span data-stu-id="b86db-124">The checks at each level ensure that the amount of sales value on the actual will not violate the not-to-exceed limit at that level after accounting for the amount of billing backlog already recorded, and the amount invoiced to date at that level.</span></span>

<span data-ttu-id="b86db-125">אם הבדיקה עוברת, הנתון בפועל של המכירה שלא חויב מקבלת מצב 'אין לחרוג' של **מחויב**.</span><span class="sxs-lookup"><span data-stu-id="b86db-125">If the check passes, the unbilled sales actual is given a not-to-exceed status of **Committed**.</span></span>

<span data-ttu-id="b86db-126">אם הבדיקה עוברת, הנתון בפועל של המכירה שלא חויב מקבל מצב 'אין לחרוג' של **נכשל**.</span><span class="sxs-lookup"><span data-stu-id="b86db-126">If the check fails, the unbilled sales actual is given a not-to-exceed status of **Failed**.</span></span> <span data-ttu-id="b86db-127">פרט האימות מודיע למשתמש באיזו רמה האימות נכשל.</span><span class="sxs-lookup"><span data-stu-id="b86db-127">The validation detail informs the user at which level the validation failed.</span></span>

<span data-ttu-id="b86db-128">כאשר הנתון בפועל של המכירה נחשבת כבלתי ניתנת לחיוב או ללא תשלום, אם אין הגדרת מגבלת 'אין לחרוג' בכל אחת מארבע הרמות, או אם הנתון בפועל שנוצר הוא עלות, ריטיינר, יחידת הקצאת משאבים או מכירות בין ארגוניות, יש להגדיר את השדות **מצב 'אין לחרוג'** ו **פרטי האימות של 'אין לחרוג'** כ **לא ישים**.</span><span class="sxs-lookup"><span data-stu-id="b86db-128">When the unbilled sales actual is considered non-chargeable or complimentary, if there is no not-to-exceed limit setup at any of the four levels, or if the actual being created is Cost, Retainer, Resourcing Unit, or Inter-organization Sales, the **Not-to-Exceed Status** and **Not-to-Exceed Validation Detail** fields must be set to **Not Applicable**.</span></span>

## <a name="reset-the-not-to-exceed-status"></a><span data-ttu-id="b86db-129">איפוס המצב 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="b86db-129">Reset the not-to-exceed status</span></span>

<span data-ttu-id="b86db-130">באפשרותך לבצע איפוס בצובר של מצב 'אין לחרוג'.</span><span class="sxs-lookup"><span data-stu-id="b86db-130">You can perform a bulk reset of the not-to-exceed status.</span></span> <span data-ttu-id="b86db-131">זה מאפשר למנהלי הפרויקט לכונן את האימות 'אין לחרוג' למתן עדיפות להפקת חשבונית של גוף עבודה, זמן או הוצאות מסוים על פני אחרים שכבר מחוייבים מתוך מסכום ה'אין לחרוג' הזמין.</span><span class="sxs-lookup"><span data-stu-id="b86db-131">This allows Project managers to adjust not-to-exceed validation to prioritize invoicing of one particular body of work, time, or expenses over others that are already committed from the available not-to-exceed amount.</span></span>

<span data-ttu-id="b86db-132">לאחר איפוס מצב ה'לא יחרוג' בנתונים בפועל של מכירות שטרם חויבו, מופחת הסכום המחויב.</span><span class="sxs-lookup"><span data-stu-id="b86db-132">After the not-to-exceed status is reset on unbilled sales actuals, the committed amount is reduced.</span></span> <span data-ttu-id="b86db-133">מנהל הפרויקט יכול לבחור גוף אחר של עבודה, זמן או הוצאות שנכשלו בעבר באימות ה'אין לחרוג', ולבצע עבורם הערכה מחדש.</span><span class="sxs-lookup"><span data-stu-id="b86db-133">The Project manager can select another body of work, time, or expenses that previously failed the not-to-exceed validation and reevaluate them.</span></span> <span data-ttu-id="b86db-134">עם הפחתת הסכום המחויב, נתונים בפועל אלו יעברו כעת את האימות.</span><span class="sxs-lookup"><span data-stu-id="b86db-134">With the reduction in the committed amount, these actuals will now pass the validation.</span></span> <span data-ttu-id="b86db-135">זה מסייע למנהל הפרויקט לקיים השפעה ושליטה רבה יותר על עסקאות אשר ניתן להפיק עבורם חשבוניות בתקופה זו.</span><span class="sxs-lookup"><span data-stu-id="b86db-135">This helps the Project manager exert greater influence and control over the invoiceable transactions for that period.</span></span>

<span data-ttu-id="b86db-136">כדי לאפס את המצב ה'אין לחרוג', בחר נתון בפועל אחד או יותר מתוך תצוגת **‏‫מצבור פריטי עבודה של חיוב זמן וחומרים‬** אוֹ **נתונים בפועל** ולאחר מכן בחר **איפוס מצב 'אין לחרוג'**.</span><span class="sxs-lookup"><span data-stu-id="b86db-136">To reset the not-to-exceed status, select one or more actuals from the **Time and Material Billing Backlog** or **Actuals** view, and then select **Reset Not-to-Exceed Status**.</span></span>

<span data-ttu-id="b86db-137">המצב 'אין לחרוג' מאופס ל **לא מוערך** בכל הנתונים בפועל הרלוונטיים שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="b86db-137">The not-to-exceed status is reset to **Not Evaluated** on all of the relevant selected actuals.</span></span> <span data-ttu-id="b86db-138">נתונים בפועל שמצב ה'אין לחרוג' שלהם אופס, הם נתונים בפועל של מכירות שטרם חויבו, אינם נמצאים בטיוטת חשבונית ומסומנים כניתנים לחיוב.</span><span class="sxs-lookup"><span data-stu-id="b86db-138">Actuals that have their not-to-exceed status reset are unbilled sales actuals that aren't already invoiced, not on a draft invoice, and are marked as chargeable.</span></span> <span data-ttu-id="b86db-139">המערכת מתעלמת מכל שאר הנתונים בפועל שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="b86db-139">Any other selected actuals are ignored.</span></span>

## <a name="reevaluate-not-to-exceed-status"></a><span data-ttu-id="b86db-140">הערכה מחדש של מצב 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="b86db-140">Reevaluate not-to-exceed status</span></span>

<span data-ttu-id="b86db-141">באפשרותך לבצע הערכה מחדש בצובר של מצב 'אין לחרוג'.</span><span class="sxs-lookup"><span data-stu-id="b86db-141">You can perform a bulk re-evaluation of the not-to-exceed status.</span></span> <span data-ttu-id="b86db-142">הערכה מחודשת של המצב 'אין לחרוג' מועילה כאשר:</span><span class="sxs-lookup"><span data-stu-id="b86db-142">Re-evaluation of the not-to-exceed status is useful when:</span></span>

  - <span data-ttu-id="b86db-143">התנהל משא ומתן מחדש של על מגבלות 'אין לחרוג' עם הלקוח, ויהיה צורך להעריך מחדש את הנתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="b86db-143">There was a renegotiation of not-to-exceed limits with the customer and actuals will need to be reevaluated.</span></span>
  - <span data-ttu-id="b86db-144">מנהל הפרויקט רוצה לכוונן את הפקת החשבוניות בגין מצבור פרטי עבודה של מכירה שלא חויבו על ידי מתן עדיפות גוף עבודה אחד על פני אחר.</span><span class="sxs-lookup"><span data-stu-id="b86db-144">The Project manager wants to fine-tune the invoicing of unbilled sales backlog by prioritizing one body of work over another.</span></span>

<span data-ttu-id="b86db-145">כדי להעריך מחדש את המצב ה'אין לחרוג', בחר נתון בפועל אחד או יותר מתוך תצוגת **‏‫מצבור פריטי עבודה של חיוב זמן וחומרים‬** אוֹ **נתונים בפועל** ולאחר מכן בחר **הערכה מחדש של מצב 'אין לחרוג'**.</span><span class="sxs-lookup"><span data-stu-id="b86db-145">To reevaluate the not-to-exceed status, select one or more actuals from the **Time and Material Billing Backlog** or **Actuals** view, and select **Reevaluate Not-to-Exceed Status**.</span></span>

<span data-ttu-id="b86db-146">כל הנתונים בפועל הרלוונטיים שנבחרו עם מגבלה 'אין לחרוג' יוערכו כנגד להגדרת מגבלת ה'אין לחרוג'.</span><span class="sxs-lookup"><span data-stu-id="b86db-146">All of the relevant selected actuals with a not-to-exceed limit will be evaluated against the not-to-exceed limit setup.</span></span> <span data-ttu-id="b86db-147">נתונים בפועל שהם רלוונטיים לביצוע הערכה מחדש למצב ה'אין לחרוג' שלהם, הם נתונים בפועל של מכירות שטרם חויבו, אינם נמצאים בטיוטת חשבונית ומסומנים כניתנים לחיוב.</span><span class="sxs-lookup"><span data-stu-id="b86db-147">Actuals that are relevant for re-evaluating the not-to-exceed status are unbilled sales actuals that are not invoiced, not on a draft invoice, and are marked as chargeable.</span></span> <span data-ttu-id="b86db-148">כל נתונים בפועל אחר שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="b86db-148">Any other select actuals selected.</span></span>
