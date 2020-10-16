---
title: סגירת הצעות מחיר
description: נושא זה מספק מידע על סגירת הצעת מחיר ב- Project Operations.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: cc3b2cdeb1ac46b7d927c1f96e94e9154d3eebf8
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896192"
---
# <a name="close-quotes"></a><span data-ttu-id="ca236-103">סגירת הצעות מחיר</span><span class="sxs-lookup"><span data-stu-id="ca236-103">Close quotes</span></span> 

<span data-ttu-id="ca236-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="ca236-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ca236-105">ניתן לסגור הצעת מחיר של פרוייקט כ'זכייה' או כ'הפסד'.</span><span class="sxs-lookup"><span data-stu-id="ca236-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="ca236-106">הפעולות 'הפעל' ו'תקן' אינן נתמכות בהצעות מחיר ב- Microsoft Dynamics 365 Project Operations, ולכן ניתן לסגור טיוטה של הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="ca236-106">The Activate and Revise operations on quotes is not supported in Microsoft Dynamics 365 Project Operations, so a draft quote can be closed.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="ca236-107">סגירת הצעת מחיר כ'זכייה'</span><span class="sxs-lookup"><span data-stu-id="ca236-107">Close a quote as Won</span></span>

<span data-ttu-id="ca236-108">סגירת הצעת מחיר של פרוייקט כ'זכייה' סוגרת את הצעת המחיר עם המצב 'סגורה' וסיבת המצב 'זכייה'.</span><span class="sxs-lookup"><span data-stu-id="ca236-108">Closing a project quote as Won will close the quote with the status set to Closed and the status reason set to Won.</span></span> <span data-ttu-id="ca236-109">סגירת הצעת המחיר של פרוייקט הופכת אותה לזמינה לקריאה בלבד ויוצרת טיוטת חוזה פרוייקט עם פרטי הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="ca236-109">Closing the quote makes the project quote read-only and creates a draft project contract that contains the quote information.</span></span> <span data-ttu-id="ca236-110">‏‫מכיוון שלא ניתן לפתוח מחדש הצעת מחיר סגורה והשינויים המבוצעים בלתי הפיכים, לפני ביצוע שינויים מוצגת תיבת דו-שיח ובה שאלה אם אתה מאשר אותם.</span><span class="sxs-lookup"><span data-stu-id="ca236-110">Because a closed quote can't be reopened, a confirmation dialog There is a confirmation dialog before the changes are done since a closed quote cannot be re-opened and the changes are irreversible.</span></span>

<span data-ttu-id="ca236-111">אם הצעת המחיר מצורפת להזדמנות, כל הצעת מחיר אחרת של הפרוייקט המשויכת להזדמנות נסגרת באופן אוטומטי כ'הפסד'.</span><span class="sxs-lookup"><span data-stu-id="ca236-111">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="ca236-112">ההשפעה הכספית של סגירת הצעת מחיר כ'זכייה'</span><span class="sxs-lookup"><span data-stu-id="ca236-112">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="ca236-113">אם היו נתונים בפועל עבור זמן שנרשם בפרוייקט כשהוא עדיין מצורף לטיוטת הצעת מחיר, רק עלות הזמן או ההוצאה תירשם.</span><span class="sxs-lookup"><span data-stu-id="ca236-113">If there have been any actuals for time recorded on a project while it is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="ca236-114">לאחר סגירת הצעת מחיר כ'זכייה', היישום יחשב מחדש את העלויות על-ידי ביטול הערך הקודם של עלויות בפועל ויצירה של הערך החדש של עלויות בפועל.</span><span class="sxs-lookup"><span data-stu-id="ca236-114">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="ca236-115">היישום יעבד את נתוני העלות בפועל בהתבסס על שיטת החיוב של סעיף החוזה המשויך לפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="ca236-115">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="ca236-116">אם נתוני העלות מתייחסים לסעיף חוזה הקשור ל'זמן וחומרים', המערכת תיצור באופן אוטומטי נתוני מכירה בפועל שאינם לחיוב עבור שלב סגירת הצעת המחיר ויצירת חוזה הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="ca236-116">If the cost actuals reference a time and material contract line, the system will automatically create corresponding unbilled sales actuals for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="ca236-117">אם נתוני העלות בפועל מתייחסים לסעיף חוזה במחיר קבוע, היישום יפסיק לעבד מחדש את נתוני העלות בפועל בהתבסס על כללי החיוב המפוצל עבור לקוחות חוזה הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="ca236-117">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals based on the split billing rules for the project contract customers.</span></span>

## <a name="closing-a-quote-as-lost"></a><span data-ttu-id="ca236-118">סגירת הצעת מחיר כ'הפסד':</span><span class="sxs-lookup"><span data-stu-id="ca236-118">Closing a quote as lost:</span></span>

<span data-ttu-id="ca236-119">סגירת הצעת מחיר של פרוייקט כ'הפסד' מגדירה את המצב כ'סגורה' ואת סיבת המצב כ'הפסד'.</span><span class="sxs-lookup"><span data-stu-id="ca236-119">Closing a project quote as Lost will set the status to Closed and status reason to Lost.</span></span> <span data-ttu-id="ca236-120">סגירת הצעת המחיר הופכת את הצעת המחיר של הפרוייקט לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="ca236-120">Closing the quote makes the project quote read-only.</span></span> <span data-ttu-id="ca236-121">מכיוון שלא ניתן לפתוח הצעת מחיר סגורה, לפני שתסגור הצעת מחיר, תוצג לך תיבת דו-שיח לאישור השינויים שביצעת.</span><span class="sxs-lookup"><span data-stu-id="ca236-121">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="ca236-122">אם הצעת המחיר של הפרוייקט שנסגרה כ'הפסד' כוללת התייחסות לפרוייקט בסעיף כלשהו מהסעיפים שלה, גם פרוייקט זה מסומן כ'נסגר' וכל הזמנת משאבים מאותו יום ואילך מבוטלת.</span><span class="sxs-lookup"><span data-stu-id="ca236-122">If the project quote that is closed as Lost has a project referenced on any of its lines, that project is also marked as Closed and any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="ca236-123">ב- Project Operations, סגירת הצעת מחיר כ'זכייה' או כ'הפסד' אינה משפיעה על המצב של ההזדמנות. ההזדמנות נשארת פתוחה עד לסגירה ידנית שלה.</span><span class="sxs-lookup"><span data-stu-id="ca236-123">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>