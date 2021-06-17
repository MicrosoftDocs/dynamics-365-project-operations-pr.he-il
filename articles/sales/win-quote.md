---
title: סגירת הצעת מחיר
description: נושא זה מספק מידע על סגירת הצעות מחיר ב- Project Operations.
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 3f46bf61bc3e492a648d65e86750a25609d5ab7a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995937"
---
# <a name="close-a-quote"></a><span data-ttu-id="ed3b5-103">סגירת הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="ed3b5-103">Close a quote</span></span>

<span data-ttu-id="ed3b5-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="ed3b5-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="ed3b5-105">ניתן לסגור הצעת מחיר של פרויקט כ'זכייה' או כ'הפסד'.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="ed3b5-106">מכיוון שהפעולות 'הפעלה' ו'שינוי' אינן נתמכות בהצעות מחיר ב- Microsoft Dynamics 365 Project Operations, ניתן לסגור טיוטה של הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-106">Because the functions Activate and Revise are not supported on quotes in Microsoft Dynamics 365 Project Operations, you can close a draft quote.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="ed3b5-107">סגירת הצעת מחיר כ'זכייה'</span><span class="sxs-lookup"><span data-stu-id="ed3b5-107">Close a quote as Won</span></span>

<span data-ttu-id="ed3b5-108">סגירת הצעת מחיר של פרויקט כ'זכייה' מגדירה את המצב של הצעת המחיר כ **סגורה** ואת סיבת המצב כ **זכייה**.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-108">Closing a project quote as Won will set the status of the quote to **Closed** and status reason to **Won**.</span></span> <span data-ttu-id="ed3b5-109">סגירת הצעת מחיר הופכת אותה לזמינה לקריאה בלבד ויוצרת טיוטת חוזה פרויקט עם כל פרטי הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-109">Closing the quotes makes it read-only and creates a draft project contract with all the quote information.</span></span> <span data-ttu-id="ed3b5-110">מכיוון שלא ניתן לפתוח הצעת מחיר סגורה, לפני שתסגור הצעת מחיר, תוצג לך תיבת דו-שיח לאישור השינויים שביצעת.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-110">Because a closed quote can't be reopened, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="ed3b5-111">חוזה הפרויקט שנוצר מהצעת מחיר של פרויקט זמין גם במודול 'ניהול פרויקטים וחשבונאות' של Project Operations.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-111">The project contract created from a project quote is also made available in the Project management and accounting module of Project Operations.</span></span> <span data-ttu-id="ed3b5-112">אם חוזה פרויקט לא ממופה לפרויקט באף אחד מהסעיפים שלו, חוזה פרויקט זה זמין כחוזה פרויקט לא פעיל, והופך פעיל ברגע שפרויקט ממופה ללפחות אחד מסעיפי החוזה שלו.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-112">If a project contract is not mapped to a project on any of its lines, this project contract is made available as an inactive project contract and becomes active as soon as a project is mapped to at least one of its contract lines.</span></span>

<span data-ttu-id="ed3b5-113">אם הצעת המחיר מצורפת להזדמנות, כל הצעת מחיר אחרת של הפרויקט המשויכת להזדמנות נסגרת באופן אוטומטי כ'הפסד'.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-113">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="ed3b5-114">ההשפעה הכספית של סגירת הצעת מחיר כ'זכייה'</span><span class="sxs-lookup"><span data-stu-id="ed3b5-114">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="ed3b5-115">אם היו נתונים בפועל עבור זמן שנרשם בפרויקט כשהוא עדיין מצורף לטיוטת הצעת מחיר, רק עלות הזמן או ההוצאה תירשם.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-115">If there have been any actuals for time recorded on a project while it is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="ed3b5-116">לאחר סגירת הצעת מחיר כ'זכייה', היישום יחשב מחדש את העלויות על-ידי ביטול הערך הקודם של עלויות בפועל ויצירה של הערך החדש של עלויות בפועל.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-116">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="ed3b5-117">היישום יעבד את נתוני העלות בפועל בהתבסס על שיטת החיוב של סעיף החוזה המשויך לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-117">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="ed3b5-118">אם נתוני העלות מתייחסים לסעיף חוזה הקשור ל'זמן וחומרים', המערכת תיצור באופן אוטומטי נתוני מכירה בפועל שאינם לחיוב עבור שלב סגירת הצעת המחיר ויצירת חוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-118">If the cost actuals reference a time and material contract line, the system will automatically create corresponding unbilled sales actuals for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="ed3b5-119">אם נתוני העלות בפועל מתייחסים לסעיף חוזה במחיר קבוע, היישום יפסיק לעבד מחדש את נתוני העלות בפועל בהתבסס על כללי החיוב המפוצל עבור לקוחות חוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-119">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals based on the split billing rules for the project contract customers.</span></span>

<span data-ttu-id="ed3b5-120">כל הנתונים בפועל‬ שעובדו מחדש זמינים במודול 'ניהול פרויקטים וחשבונאות' על מנת שרואה החשבון הממונה על הפרויקט יוכל לבדוק, לעדכן ולרשום אותם בספר החשבונות הראשי.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-120">All reprocessed actuals are available in the Project management and accounting module for the Project accountant to review, update, and post to the General ledger.</span></span> 

## <a name="close-a-quote-as-lost"></a><span data-ttu-id="ed3b5-121">סגירת הצעת מחיר כ'הפסד'</span><span class="sxs-lookup"><span data-stu-id="ed3b5-121">Close a quote as Lost</span></span>

<span data-ttu-id="ed3b5-122">סגירת הצעת מחיר של פרויקט כ'הפסד' מגדירה את המצב כ **סגורה** ואת סיבת המצב כ **הפסד**.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-122">Closing a project quote as Lost will set the status to **Closed** and status reason to **Lost**.</span></span> <span data-ttu-id="ed3b5-123">סגירת הצעת המחיר הופכת אותה לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-123">Closing the quote makes it read-only.</span></span> <span data-ttu-id="ed3b5-124">מכיוון שלא ניתן לפתוח הצעת מחיר סגורה, לפני שתסגור הצעת מחיר, תוצג לך תיבת דו-שיח לאישור השינויים שביצעת.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-124">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="ed3b5-125">אם הצעת המחיר של הפרויקט שנסגרה כ'הפסד' כוללת התייחסות לפרויקט בסעיף כלשהו מהסעיפים שלה, גם פרויקט זה מסומן כ'נסגר' וכל הזמנת משאבים מאותו יום ואילך מבוטלת.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-125">If the project quote that is closed as Lost has a project referenced on any of its lines, that project is also marked as Closed and any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="ed3b5-126">ב- Project Operations, סגירת הצעת מחיר כ'זכייה' או כ'הפסד' אינה משפיעה על המצב של ההזדמנות. ההזדמנות נשארת פתוחה עד לסגירה ידנית שלה.</span><span class="sxs-lookup"><span data-stu-id="ed3b5-126">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]