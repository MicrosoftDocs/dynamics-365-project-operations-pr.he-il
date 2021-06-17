---
title: ניהול מצב ואימות של 'אין לחרוג'
description: נושא זה מספק מידע אודות בדיקות מגבולת 'אין לחרוג' שמבוצעות ב-Project Operations.
author: rumant
ms.date: 04/05/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d51a61e441b004ae836037aefa172fdd20ac83ed
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003902"
---
# <a name="manage-not-to-exceed-status-and-validations"></a><span data-ttu-id="08e55-103">ניהול מצב ואימות של 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="08e55-103">Manage not-to-exceed status and validations</span></span> 

<span data-ttu-id="08e55-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="08e55-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

## <a name="not-to-exceed-on-approvals"></a><span data-ttu-id="08e55-105">'אין לחרוג' באישורים</span><span class="sxs-lookup"><span data-stu-id="08e55-105">Not-to-exceed on approvals</span></span>

<span data-ttu-id="08e55-106">בעת שליחה של ערך זמן, הוצאה או שימוש בחומרים, נוצרת רשומת אישור.</span><span class="sxs-lookup"><span data-stu-id="08e55-106">When a time, expense, or material usage entry is submitted, an approval record is created.</span></span> <span data-ttu-id="08e55-107">אם האישור ניתן לחיוב וממפה לסעיף חוזה של זמן וחומרים, המערכת מבצעת בדיקת אימות למגבלות 'אין לחרוג' ברמות הבאות:</span><span class="sxs-lookup"><span data-stu-id="08e55-107">If the approval is chargeable and maps to a time and material contract line, the system completes a not-to-exceed validation check at the following levels:</span></span>

  - <span data-ttu-id="08e55-108">בודקת מול המגבלה שהוגדרה ללקוח סעיף חוזה הפרויקט</span><span class="sxs-lookup"><span data-stu-id="08e55-108">Check against the limit set up for the customer on the project contract line</span></span>
  - <span data-ttu-id="08e55-109">בודקת מול המגבלה שהוגדרה בסעיף החוזה</span><span class="sxs-lookup"><span data-stu-id="08e55-109">Check against the limit set up on the contract line</span></span>
  - <span data-ttu-id="08e55-110">בודקת מול המגבלה שהוגדרה עבור הלקוח</span><span class="sxs-lookup"><span data-stu-id="08e55-110">Check against the limit set up for the customer</span></span>
  - <span data-ttu-id="08e55-111">בודקת מול המגבלה שהוגדרה בחוזה</span><span class="sxs-lookup"><span data-stu-id="08e55-111">Check against the limit set up on the contract</span></span>

<span data-ttu-id="08e55-112">הבדיקות בכל רמה כוללות הבטחה שכמות ערך המכירה באישור זה לא תפר את מגבלת 'אין לחרוג' באותה הרמה, לאחר התחשבות בסכום מצבור פרטי העבודה של חיוב שכבר נרשם, והסכום שעבורו הוגשו חשבוניות עד כה ברמה זו.</span><span class="sxs-lookup"><span data-stu-id="08e55-112">The checks at each level involve ensuring that the amount of sales value on this approval will not violate the not-to-exceed limit at that level after accounting for the amount of billing backlog already recorded, and the amount invoiced to date at that level.</span></span>

<span data-ttu-id="08e55-113">אם הבדיקה עוברת, האישור מקבל מצב אימות של **הצלחה**.</span><span class="sxs-lookup"><span data-stu-id="08e55-113">If the check passes, the approval is given a validation status of **Success**.</span></span>

<span data-ttu-id="08e55-114">אם הבדיקה נכשלת, האישור מקבל מצב אימות של **נכשל**.</span><span class="sxs-lookup"><span data-stu-id="08e55-114">If the check fails, the approval is given a validation status of **Failed**.</span></span> <span data-ttu-id="08e55-115">פרט האימות של 'אין לחרוג' יודיע למשתמש באיזו רמה האימות נכשל.</span><span class="sxs-lookup"><span data-stu-id="08e55-115">The not-to-exceed validation detail will inform the user at which level the validation failed.</span></span>

<span data-ttu-id="08e55-116">כאשר ערך הזמן, ההוצאה או השימוש בחומר נחשב כאינו ניתן לחיוב, מצב האימות של 'אין לחרוג'‬ מוגדר בתור **לא ישים** ופרט האימות שווה ל **לא ישים**.</span><span class="sxs-lookup"><span data-stu-id="08e55-116">When the submitted time, expense, or material usage entry is considered non-chargeable, the not-to-exceed validation status is set to **Not Applicable** with the validation detail equal to **Not applicable**.</span></span>

## <a name="not-to-exceed-on-unbilled-sales-actuals"></a><span data-ttu-id="08e55-117">'אין לחרוג' בנתונים בפועל של מכירות שטרם חויבו</span><span class="sxs-lookup"><span data-stu-id="08e55-117">Not-to-exceed on unbilled sales actuals</span></span>

<span data-ttu-id="08e55-118">בעת אישור ערך הזמן, ההוצאה או השימוש בחומר, נוצרות רשומות נתונים בפועל של עלות ושל מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="08e55-118">When a time, expense, or material usage entry is approved, cost and unbilled sales actuals records are created.</span></span> <span data-ttu-id="08e55-119">אם הנתון בפועל של המכירות שנוצר ניתן לחיוב וממפה לסעיף חוזה של זמן וחומרים, אפליקציה מבצעת בדיקת אימות למגבלות 'אין לחרוג' ברמות הבאות:</span><span class="sxs-lookup"><span data-stu-id="08e55-119">If the unbilled sales actual being created is chargeable and maps to a time and material contract line, the application performs a not-to-exceed validation check at the following levels:</span></span>

  - <span data-ttu-id="08e55-120">בודקת מול המגבלה שהוגדרה ללקוח של סעיף חוזה הפרויקט</span><span class="sxs-lookup"><span data-stu-id="08e55-120">Check against the limit set up for the customer of the project contract line</span></span>
  - <span data-ttu-id="08e55-121">בודקת מול המגבלה שהוגדרה בסעיף החוזה</span><span class="sxs-lookup"><span data-stu-id="08e55-121">Check against the limit set up on the contract line</span></span>
  - <span data-ttu-id="08e55-122">בודקת מול המגבלה שהוגדרה עבור הלקוח</span><span class="sxs-lookup"><span data-stu-id="08e55-122">Check against the limit set up for the customer</span></span>
  - <span data-ttu-id="08e55-123">בודקת מול המגבלה שהוגדרה בחוזה</span><span class="sxs-lookup"><span data-stu-id="08e55-123">Check against the limit set up on the contract</span></span>

<span data-ttu-id="08e55-124">הבדיקות בכל רמה כוללות הבטחה שכמות ערך המכירה בנתון בפועל זה לא תפר את מגבלת 'אין לחרוג' באותה הרמה, לאחר התחשבות בסכום מצבור פרטי העבודה של חיוב שכבר נרשם, והסכום שעבורו הוגשו חשבוניות עד כה ברמה זו.</span><span class="sxs-lookup"><span data-stu-id="08e55-124">The checks at each level ensure that the amount of sales value on the actual will not violate the not-to-exceed limit at that level after accounting for the amount of billing backlog already recorded, and the amount invoiced to date at that level.</span></span>

<span data-ttu-id="08e55-125">אם הבדיקה עוברת, הנתון בפועל של המכירה שלא חויב מקבלת מצב 'אין לחרוג' של **מחויב**.</span><span class="sxs-lookup"><span data-stu-id="08e55-125">If the check passes, the unbilled sales actual is given a not-to-exceed status of **Committed**.</span></span>

<span data-ttu-id="08e55-126">אם הבדיקה עוברת, הנתון בפועל של המכירה שלא חויב מקבל מצב 'אין לחרוג' של **נכשל**.</span><span class="sxs-lookup"><span data-stu-id="08e55-126">If the check fails, the unbilled sales actual is given a not-to-exceed status of **Failed**.</span></span> <span data-ttu-id="08e55-127">פרט האימות מודיע למשתמש באיזו רמה האימות נכשל.</span><span class="sxs-lookup"><span data-stu-id="08e55-127">The validation detail informs the user at which level the validation failed.</span></span>

<span data-ttu-id="08e55-128">כאשר הנתון בפועל של המכירה נחשבת כבלתי ניתנת לחיוב או ללא תשלום, אם אין הגדרת מגבלת 'אין לחרוג' בכל אחת מארבע הרמות, או אם הנתון בפועל שנוצר הוא עלות, ריטיינר, יחידת הקצאת משאבים או מכירות בין ארגוניות, יש להגדיר את השדות **מצב 'אין לחרוג'** ו **פרטי האימות של 'אין לחרוג'** כ **לא ישים**.</span><span class="sxs-lookup"><span data-stu-id="08e55-128">When the unbilled sales actual is considered non-chargeable or complimentary, if there is no not-to-exceed limit setup at any of the four levels, or if the actual being created is Cost, Retainer, Resourcing Unit, or Inter-organization Sales, the **Not-to-Exceed Status** and **Not-to-Exceed Validation Detail** fields must be set to **Not Applicable**.</span></span>

## <a name="reset-the-not-to-exceed-status"></a><span data-ttu-id="08e55-129">איפוס המצב 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="08e55-129">Reset the not-to-exceed status</span></span>

<span data-ttu-id="08e55-130">באפשרותך לבצע איפוס בצובר של מצב 'אין לחרוג'.</span><span class="sxs-lookup"><span data-stu-id="08e55-130">You can perform a bulk reset of the not-to-exceed status.</span></span> <span data-ttu-id="08e55-131">מנהלי פרויקטים יכולים להתאים את האימות של 'אין לחרוג' כדי לתעדף את הפקת חשבוניות של גוף עבודה, זמן, הוצאה או שימוש בחומר מסוימים על פני אחרים שכבר התחייבו מהסכום הזמין של 'אין לחרוג'.</span><span class="sxs-lookup"><span data-stu-id="08e55-131">Project managers can adjust the not-to-exceed validation to prioritize invoicing of one particular body of work, time, expense, or material usage over others that are already committed from the available not-to-exceed amount.</span></span>

<span data-ttu-id="08e55-132">לאחר איפוס מצב ה'לא יחרוג' בנתונים בפועל של מכירות שטרם חויבו, מופחת הסכום המחויב.</span><span class="sxs-lookup"><span data-stu-id="08e55-132">After the not-to-exceed status is reset on unbilled sales actuals, the committed amount is reduced.</span></span> <span data-ttu-id="08e55-133">מנהל הפרויקט יכול לבחור ערך אחר של גוף עבודה, זמן, הוצאה או שימוש בחומר שנכשל בעבר באימות של 'אין לחרוג' ולבצע הערכה מחדש.</span><span class="sxs-lookup"><span data-stu-id="08e55-133">The Project manager can select another body of work, time, expense, or material usage entry that previously failed the not-to-exceed validation and reevaluate.</span></span> <span data-ttu-id="08e55-134">עם הפחתת הסכום המוקצה, נתונים בפועל אלו עוברים כעת את האימות שמסייע למנהל הפרויקט להשפיע יותר ולשלוט בעסקאות שניתן להפיק עבורן לחשבונית לתקופה זו.</span><span class="sxs-lookup"><span data-stu-id="08e55-134">With the reduction in the committed amount, these actuals now pass the validation which helps the Project manager exert greater influence and control over the invoiceable transactions for that period.</span></span>

<span data-ttu-id="08e55-135">כדי לאפס את המצב ה'אין לחרוג', בחר נתון בפועל אחד או יותר מתוך תצוגת **‏‫מצבור פריטי עבודה של חיוב זמן וחומרים‬** אוֹ **נתונים בפועל** ולאחר מכן בחר **איפוס מצב 'אין לחרוג'**.</span><span class="sxs-lookup"><span data-stu-id="08e55-135">To reset the not-to-exceed status, select one or more actuals from the **Time and Material Billing Backlog** or **Actuals** view, and then select **Reset Not-to-Exceed Status**.</span></span>

<span data-ttu-id="08e55-136">המצב 'אין לחרוג' מאופס ל **לא מוערך** בכל הנתונים בפועל הרלוונטיים שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="08e55-136">The not-to-exceed status is reset to **Not Evaluated** on all of the relevant selected actuals.</span></span> <span data-ttu-id="08e55-137">נתונים בפועל שמצב ה'אין לחרוג' שלהם אופס, הם נתונים בפועל של מכירות שטרם חויבו, אינם נמצאים בטיוטת חשבונית ומסומנים כניתנים לחיוב.</span><span class="sxs-lookup"><span data-stu-id="08e55-137">Actuals that have their not-to-exceed status reset are unbilled sales actuals that aren't already invoiced, not on a draft invoice, and are marked as chargeable.</span></span> <span data-ttu-id="08e55-138">המערכת מתעלמת מכל שאר הנתונים בפועל שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="08e55-138">Any other selected actuals are ignored.</span></span>

## <a name="reevaluate-not-to-exceed-status"></a><span data-ttu-id="08e55-139">הערכה מחדש של מצב 'אין לחרוג'</span><span class="sxs-lookup"><span data-stu-id="08e55-139">Reevaluate not-to-exceed status</span></span>

<span data-ttu-id="08e55-140">באפשרותך לבצע הערכה מחדש בצובר של מצב 'אין לחרוג'.</span><span class="sxs-lookup"><span data-stu-id="08e55-140">You can perform a bulk re-evaluation of the not-to-exceed status.</span></span> <span data-ttu-id="08e55-141">הערכה מחודשת של המצב 'אין לחרוג' מועילה כאשר:</span><span class="sxs-lookup"><span data-stu-id="08e55-141">Re-evaluation of the not-to-exceed status is useful when:</span></span>

  - <span data-ttu-id="08e55-142">התנהל משא ומתן מחדש של על מגבלות 'אין לחרוג' עם הלקוח, ויהיה צורך להעריך מחדש את הנתונים בפועל.</span><span class="sxs-lookup"><span data-stu-id="08e55-142">There was a renegotiation of not-to-exceed limits with the customer and actuals will need to be reevaluated.</span></span>
  - <span data-ttu-id="08e55-143">מנהל הפרויקט רוצה לכוונן את הפקת החשבוניות בגין מצבור פרטי עבודה של מכירה שלא חויבו על ידי מתן עדיפות גוף עבודה אחד על פני אחר.</span><span class="sxs-lookup"><span data-stu-id="08e55-143">The Project manager wants to fine-tune the invoicing of unbilled sales backlog by prioritizing one body of work over another.</span></span>

<span data-ttu-id="08e55-144">כדי להעריך מחדש את המצב ה'אין לחרוג', בחר נתון בפועל אחד או יותר מתוך תצוגת **‏‫מצבור פריטי עבודה של חיוב זמן וחומרים‬** אוֹ **נתונים בפועל** ולאחר מכן בחר **הערכה מחדש של מצב 'אין לחרוג'**.</span><span class="sxs-lookup"><span data-stu-id="08e55-144">To reevaluate the not-to-exceed status, select one or more actuals from the **Time and Material Billing Backlog** or **Actuals** view, and select **Reevaluate Not-to-Exceed Status**.</span></span>

<span data-ttu-id="08e55-145">כל הנתונים בפועל הרלוונטיים שנבחרו עם מגבלה 'אין לחרוג' יוערכו כנגד להגדרת מגבלת ה'אין לחרוג'.</span><span class="sxs-lookup"><span data-stu-id="08e55-145">All of the relevant selected actuals with a not-to-exceed limit will be evaluated against the not-to-exceed limit setup.</span></span> <span data-ttu-id="08e55-146">נתונים בפועל שהם רלוונטיים לביצוע הערכה מחדש למצב ה'אין לחרוג' שלהם, הם נתונים בפועל של מכירות שטרם חויבו, אינם נמצאים בטיוטת חשבונית ומסומנים כניתנים לחיוב.</span><span class="sxs-lookup"><span data-stu-id="08e55-146">Actuals that are relevant for re-evaluating the not-to-exceed status are unbilled sales actuals that are not invoiced, not on a draft invoice, and are marked as chargeable.</span></span> <span data-ttu-id="08e55-147">כל נתונים בפועל אחר שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="08e55-147">Any other select actuals selected.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
