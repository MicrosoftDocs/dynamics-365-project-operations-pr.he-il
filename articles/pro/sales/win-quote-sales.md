---
title: סגירת הצעת מחיר - לייט
description: נושא זה מספק מידע על סגירת הצעת מחיר ב- Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 6214e1b5bec5c9173a6b6e69578de14654da633e
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5272276"
---
# <a name="close-a-quote---lite"></a><span data-ttu-id="51de4-103">סגירת הצעת מחיר - לייט</span><span class="sxs-lookup"><span data-stu-id="51de4-103">Close a quote - lite</span></span>

<span data-ttu-id="51de4-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="51de4-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="51de4-105">ניתן לסגור הצעת מחיר של פרויקט כ'זכייה' או כ'הפסד'.</span><span class="sxs-lookup"><span data-stu-id="51de4-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="51de4-106">ניתן לסגור טיוטה של הצעת מחיר מכיוון שהפעולות 'הפעלה' ו'שינוי' בהצעות מחיר אינן נתמכות ב- Microsoft Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="51de4-106">A draft quote can be closed because the Activate and Revise operations on quotes isn't supported in Microsoft Dynamics 365 Project Operations.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="51de4-107">סגירת הצעת מחיר כ'זכייה'</span><span class="sxs-lookup"><span data-stu-id="51de4-107">Close a quote as Won</span></span>

<span data-ttu-id="51de4-108">כשאתה סוגר הצעת מחיר כ'זכייה', הסטטוס שלה מוגדר 'סגור' וסיבת המצב הוא 'זכייה'.</span><span class="sxs-lookup"><span data-stu-id="51de4-108">When you close a project quote as Won, the status is set to Closed and the status reason is Won.</span></span> <span data-ttu-id="51de4-109">סגירת הצעת המחיר של פרויקט הופכת אותה לזמינה לקריאה בלבד ויוצרת טיוטת חוזה פרויקט עם פרטי הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="51de4-109">Closing the quote makes the project quote read-only and creates a draft project contract that contains the quote information.</span></span> <span data-ttu-id="51de4-110">מכיוון שלא ניתן לפתוח הצעת מחיר סגורה, תיבת דו-שיח לאישור תאשר את השינויים שלך.</span><span class="sxs-lookup"><span data-stu-id="51de4-110">Because a closed quote can't be reopened, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="51de4-111">אם הצעת המחיר מצורפת להזדמנות, כל הצעת מחיר אחרת של הפרויקט המשויכת להזדמנות נסגרת באופן אוטומטי כ'הפסד'.</span><span class="sxs-lookup"><span data-stu-id="51de4-111">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="51de4-112">ההשפעה הכספית של סגירת הצעת מחיר כ'זכייה'</span><span class="sxs-lookup"><span data-stu-id="51de4-112">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="51de4-113">אם יש נתונים בפועל בפרוייקט בזמן שהוא עדיין מצורף להצעת מחיר, רק עלות הזמן או ההוצאה נרשמים.</span><span class="sxs-lookup"><span data-stu-id="51de4-113">If there are any actuals for time on a project while is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="51de4-114">לאחר סגירת הצעת מחיר כ'זכייה', היישום יחשב מחדש את העלויות על-ידי ביטול הערך הקודם של עלויות בפועל ויצירה של הערך החדש של עלויות בפועל.</span><span class="sxs-lookup"><span data-stu-id="51de4-114">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="51de4-115">היישום יעבד את נתוני העלות בפועל בהתבסס על שיטת החיוב של סעיף החוזה המשויך לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="51de4-115">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="51de4-116">אם נתוני העלות מתייחסים לסעיף חוזה בפועל של זמן וחומרים, נתונים בפועל נוצרים למכירה מתאימה שלא חויבה עבור סגירת הצעת המחיר ויצירת חוזה הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="51de4-116">If the cost actuals reference a time and material contract line, corresponding unbilled sales actuals are created for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="51de4-117">אם נתוני העלות מתייחסים לסעיף חוזה במחיר קבוע, היישום יפסיק לעבד מחדש את עלויות הרישום המבוססות על כללי החיוב המפוצלים עבור לקוחות חוזה הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="51de4-117">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals that are based on the split billing rules for the project contract customers.</span></span>

## <a name="closing-a-quote-as-lost"></a><span data-ttu-id="51de4-118">סגירת הצעת מחיר כ'הפסד':</span><span class="sxs-lookup"><span data-stu-id="51de4-118">Closing a quote as lost:</span></span>

<span data-ttu-id="51de4-119">כשאתה סוגר הצעת מחיר כ'הפסד‬', הסטטוס שלה מוגדר 'סגור' וסיבת המצב הוא 'הפסד‬'.</span><span class="sxs-lookup"><span data-stu-id="51de4-119">When you close a project quote as Lost, the status is set to Closed and status reason is Lost.</span></span> <span data-ttu-id="51de4-120">סגירת הצעת המחיר הופכת את הצעת המחיר של הפרויקט לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="51de4-120">Closing the quote makes the project quote read-only.</span></span> <span data-ttu-id="51de4-121">מכיוון שלא ניתן לפתוח הצעת מחיר סגורה, לפני שתסגור הצעת מחיר, תוצג לך תיבת דו-שיח לאישור השינויים שביצעת.</span><span class="sxs-lookup"><span data-stu-id="51de4-121">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="51de4-122">אם הצעת המחיר של הפרוייקט שנסגרה כ'הפסד‬' מתייחסת לפרוייקט בכל הסעיפים שלו, הפרוייקט הזה מסומן גם 'סגור'.</span><span class="sxs-lookup"><span data-stu-id="51de4-122">If the project quote that is closed as Lost references a project on any of its lines, that project is also marked as Closed.</span></span> <span data-ttu-id="51de4-123">כל הזמנות המשאבים מאותו יום ואילך מבוטלות.</span><span class="sxs-lookup"><span data-stu-id="51de4-123">Any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="51de4-124">ב- Project Operations, סגירת הצעת מחיר כ'זכייה' או כ'הפסד' אינה משפיעה על המצב של ההזדמנות. ההזדמנות נשארת פתוחה עד לסגירה ידנית שלה.</span><span class="sxs-lookup"><span data-stu-id="51de4-124">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]