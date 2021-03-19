---
title: פתרון מחירי עלות בהערכות ובנתונים בפועל - לייט
description: נושא זה מספק מידע אודות אופן פתרון מחירי העלות של הערכות ונתונים ופועלים.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: bbb79fdc5c68d67530b5aa34fe6105211eff1768
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274550"
---
# <a name="resolve-cost-prices-on-estimates-and-actuals---lite"></a><span data-ttu-id="65bb2-103">פתרון מחירי עלות בהערכות ובנתונים בפועל - לייט</span><span class="sxs-lookup"><span data-stu-id="65bb2-103">Resolve cost prices on estimates and actuals - lite</span></span>

<span data-ttu-id="65bb2-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="65bb2-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="65bb2-105">כדי לפתור מחירי עלות ומחירון העלויות להערכות ולנתונים בפועל, המערכת משתמשת במידע שמופיע בשדות **תאריך**, **מטבע**, ו **יחידת החוזה** של הפרויקט הקשור.</span><span class="sxs-lookup"><span data-stu-id="65bb2-105">To resolve cost prices and the cost price list for estimates and actuals, the system uses the information in the **Date**, **Currency**, and **Contracting Unit** fields of the related project.</span></span> <span data-ttu-id="65bb2-106">לאחר פתרון מחירון העלות, היישום פותר את תעריף העלות.</span><span class="sxs-lookup"><span data-stu-id="65bb2-106">After the cost price list is resolved, the application resolves the cost rate.</span></span>

## <a name="resolving-cost-rates-on-actual-and-estimate-lines-for-time"></a><span data-ttu-id="65bb2-107">פתרון תעריפי עלות בנתונים בפועל והערכת עבור 'זמן'</span><span class="sxs-lookup"><span data-stu-id="65bb2-107">Resolving cost rates on actual and estimate lines for Time</span></span>

<span data-ttu-id="65bb2-108">שורות הערכה ל'זמן' מתייחסים לפרטי הצעת המחיר וסעיף החוזה להקצאת זמן ומשאבים בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="65bb2-108">Estimate lines for Time refer to the quote and contract line details for time and resource assignments on a project.</span></span>

<span data-ttu-id="65bb2-109">לאחר פתרון מחירון עלות, השדות **תפקיד** ו **יחידת משאבים** בשורת האומדן עבור זמן מותאמים לשורות מחיר התפקיד במחירון.</span><span class="sxs-lookup"><span data-stu-id="65bb2-109">After a cost price list is resolved, the **Role** and **Resourcing Unit** fields on the estimate line for Time are matched against the role price lines in the price list.</span></span> <span data-ttu-id="65bb2-110">התאמה זו מניחה שאתה משתמש בממדי התמחור הסטנדרטיים עבור עלות העבודה.</span><span class="sxs-lookup"><span data-stu-id="65bb2-110">This match assumes that you're using the standard pricing dimensions for labor cost.</span></span> <span data-ttu-id="65bb2-111">אם הגדרת את המערכת כך שתתאים שדות במקום, או בנוסף לשדות **תפקיד** ו **יחידת הקצאת משאבים**, שילוב אחר ישימש כדי לאחזר שורת מחיר תפקיד תואם.</span><span class="sxs-lookup"><span data-stu-id="65bb2-111">If you configured the system to match fields instead of, or in addition to **Role** and **Resourcing Unit**, then a different combination will be used to retrieve a matching role price line.</span></span> <span data-ttu-id="65bb2-112">אם היישום מוצא שורת מחיר תפקיד שיש לה תעריף עלות עבור השילוב בין **תפקיד** ו **יחידת הקצאת משאבים**, זהו תעריף ברירת המחדל של עלות.</span><span class="sxs-lookup"><span data-stu-id="65bb2-112">If the application finds a role price line that has a cost rate for the **Role** and **Resourcing Unit** combination, that is the default cost rate.</span></span> <span data-ttu-id="65bb2-113">אם היישום אינו יכול להתאים את הערכים של **תפקיד** ו **יחידת הקצאת משאבים**, הוא מאחזר שורות מחיר תפקיד עם תפקיד תואם, אך עם ערכי Null עבור **יחידת הקצאת משאבים**.</span><span class="sxs-lookup"><span data-stu-id="65bb2-113">If the application can't match the **Role** and **Resourcing Unit** values, then it retrieves role price lines with a matching role, but null values of the **Resourcing Unit**.</span></span> <span data-ttu-id="65bb2-114">לאחר שמצא רשומת מחיר תפקיד תואם, ברירת המחדל של תעריף העלות נקבעת מאותה רשומה.</span><span class="sxs-lookup"><span data-stu-id="65bb2-114">After it has a matching role price record, the cost rate defaults from that record.</span></span> 

> [!NOTE]
> <span data-ttu-id="65bb2-115">אם מגדירים עדיפות שונה ל **תפקיד** ול **יחידת הקצאת משאבים**, או אם יש לך ממדים אחרים בעלי עדיפות גבוהה יותר, אופן פעולה זה ישתנה בהתאם.</span><span class="sxs-lookup"><span data-stu-id="65bb2-115">If you configure a different prioritization of **Role** and **Resourcing Unit**, or if you have other dimensions that have higher priority, this behavior will change accordingly.</span></span> <span data-ttu-id="65bb2-116">המערכת מאחזרת רשומות של מחירי תפקידים עם ערכים התואמים לכל אחד מערכי ממדי התמחור לפי סדר העדיפות עם שורות בעלות ערכי Null עבור אותם ממדים בעלי העדיפות הנמוכה ביותר.</span><span class="sxs-lookup"><span data-stu-id="65bb2-116">The system retrieves role price records with values that match each of the pricing dimension values in order of priority with rows that have null values for those dimensions coming last.</span></span>

## <a name="resolving-cost-rates-on-actual-and-estimate-lines-for-expense"></a><span data-ttu-id="65bb2-117">פתרון תעריפי עלות בשורות של נתונים בפועל ושל הערכת עבור 'הוצאה'</span><span class="sxs-lookup"><span data-stu-id="65bb2-117">Resolving cost rates on actual and estimate lines for Expense</span></span>

<span data-ttu-id="65bb2-118">שורות הערכה ל'הוצאה' מתייחסות לפרטי ההוצאת של הצעת המחיר וסעיף החוזה ולשורות הערכת ההוצאות בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="65bb2-118">Estimate lines for Expense refer to the quote and contract line details for expenses and the expense estimate lines on a project.</span></span>

<span data-ttu-id="65bb2-119">לאחר פתרון של מחירון העלויות, המערכת משתמשת בשילוב של השדות **קטגוריה** ו **יחידה** בשורת אומדן ההוצאות כדי להתאים לשורות **מחיר קטגוריה** במחירון שנקבע.</span><span class="sxs-lookup"><span data-stu-id="65bb2-119">After a cost price list is resolved, the system uses a combination of the **Category** and **Unit** fields on the expense estimate line to match against the **Category Price** lines on the resolved price list.</span></span> <span data-ttu-id="65bb2-120">אם היישום מוצא שורת מחיר של קטגורה שיש לה תעריף עלות עבור השילוב בין השדות **קטגוריה** ו **יחידה**, זהו תעריף ברירת המחדל של עלות.</span><span class="sxs-lookup"><span data-stu-id="65bb2-120">If the system finds a category price line that has a cost rate for the **Category** and **Unit** field combination, the cost rate is defaulted.</span></span> <span data-ttu-id="65bb2-121">אם המערכת לא יכולה להתאים את הערכים של **קטגוריה** ו **יחידה**, או אם היא מצליחה למצוא שורת מחיר שתואמת לקטגוריה אך שיטת התמחור אינה **מחיר ליחידה**, ברירת המחדל של שיעור העלות היא אפס (0).</span><span class="sxs-lookup"><span data-stu-id="65bb2-121">If the system can't match the **Category** and **Unit** values, or if it's able to find a matching category price line but the pricing method isn't **Price Per Unit**, the cost rate defaults to zero(0).</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]