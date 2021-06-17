---
title: אש"ל
description: נושא זה מספק מידע אודות כללי האש"ל המשמשים בניהול הוצאות.
author: suvaidya
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: b1476bfc0386412762c30e5a00acaff65bfbe3c7
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995262"
---
# <a name="per-diems"></a><span data-ttu-id="3a349-103">אש"ל</span><span class="sxs-lookup"><span data-stu-id="3a349-103">Per diems</span></span>

<span data-ttu-id="3a349-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="3a349-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="3a349-105">דמי אש"ל הם קצבה המשולמת לעובד הנוסע למטרות עבודה.</span><span class="sxs-lookup"><span data-stu-id="3a349-105">A per diem is an allowance that is paid to a worker who is traveling for work.</span></span> <span data-ttu-id="3a349-106">בניהול הוצאות, ניתן ליצור כללי אש"ל עבור מצבי נסיעה שונים.</span><span class="sxs-lookup"><span data-stu-id="3a349-106">In Expense management, you can create per diem rules for  various travel situations.</span></span> <span data-ttu-id="3a349-107">תעריפי אש"ל יכולים להתבסס על תקופת השנה, על יעד הנסיעה או על שניהם.</span><span class="sxs-lookup"><span data-stu-id="3a349-107">Per diem rates can be based on the time of year, the travel location, or both.</span></span> <span data-ttu-id="3a349-108">כשיוצרים כלל לדמי אש"ל, אפשר לקבוע שאחוז תעריף האש"ל ההנאה ינוכה אם עובד מקבל ארוחות או שירותים בחינם.</span><span class="sxs-lookup"><span data-stu-id="3a349-108">When you create a per diem  rule, you can specify that a percentage of the per diem rate will be withheld if a worker receives complimentary meals or services.</span></span> <span data-ttu-id="3a349-109">ניתן גם להגדיר מספר שעות מינימלי ומקסימאלי להחלת דמי אש"ל על נסיעה של עובד.</span><span class="sxs-lookup"><span data-stu-id="3a349-109">You can also set a minimum and maximum number of hours that the per diem rate can apply to a worker's travel.</span></span>

## <a name="configuration"></a><span data-ttu-id="3a349-110">תצורה</span><span class="sxs-lookup"><span data-stu-id="3a349-110">Configuration</span></span> 

1. <span data-ttu-id="3a349-111">כדי להוסיף מיקומים לאש"ל, עבור אל **הגדרות** > **חישובים וקודים** > **מיקומי אש"ל**.</span><span class="sxs-lookup"><span data-stu-id="3a349-111">To add per diem locations, go to **Set up** > **Calculations and codes** > **Per diem locations**.</span></span>
2. <span data-ttu-id="3a349-112">עבור כל אחד מהמיקומים שנוספו לעיל, בחרו תעריף אש"ל ומטבע, שתקף בין תאריך התחלה וסיום ספציפיים עבור מלון, ארוחות והוצאות אחרות.</span><span class="sxs-lookup"><span data-stu-id="3a349-112">For each of the locations added above, select a per diem rate and currency that is valid between a specific start and end date for hotel, meals, and other expenses.</span></span> <span data-ttu-id="3a349-113">תעריפי האש"ל והמטבעות מוגדרים תחת **הגדרות** > **חישובים וקודים** > **דמי אש"ל**.</span><span class="sxs-lookup"><span data-stu-id="3a349-113">Per diem rates and currencies are configured under **Set up** > **Calculations and codes** > **Per diems**.</span></span>
3. <span data-ttu-id="3a349-114">בדף **מיקומים לאש"ל**, הגדר את הרמות של תעריף אש"ל.</span><span class="sxs-lookup"><span data-stu-id="3a349-114">On the **Per diem locations** page, configure per diem rate tiers.</span></span> <span data-ttu-id="3a349-115">רמות תעריף האש"ל מאפשרות לך להגדיר את אחוז הפיצול של הקצבה היומית עבור מלון, ארוחות והוצאות אחרות.</span><span class="sxs-lookup"><span data-stu-id="3a349-115">Per diem rate tiers allow you to define the percentage split of a daily allowance for hotel, meal, and other expenses.</span></span> 
4. <span data-ttu-id="3a349-116">כדי לציין את הפחתת האחוזים לארוחות בוקר, צהריים או ערב, יש עדכן את השדות בדף **פרמטרים לניהול הוצאות** בכרטיסיה **אש"ל**.</span><span class="sxs-lookup"><span data-stu-id="3a349-116">To specify the meal percentage reduction for breakfast, lunch, or dinner, update the fields on the **Expense management parameters** page on the **Per diem** tab.</span></span> 
    
## <a name="submit-expenses-using-per-diem"></a><span data-ttu-id="3a349-117">הגשת הוצאות באמצעות אש"ל</span><span class="sxs-lookup"><span data-stu-id="3a349-117">Submit expenses using per diem</span></span>
<span data-ttu-id="3a349-118">כדי להגיש הוצאות באמצעות אש"ל , השתמש בקטגוריית ההוצאות **אש"ל** בעת יצירת דוח הוצאות.</span><span class="sxs-lookup"><span data-stu-id="3a349-118">To submit expenses utilizing per diems, use the **Per diem** expense category when you create an expense report.</span></span> <span data-ttu-id="3a349-119">הזן את הערכים **אש"ל מהתאריך**, **אש"ל עד לתאריך**, ואת **מיקום האש"ל**.</span><span class="sxs-lookup"><span data-stu-id="3a349-119">Enter the **Per diem from date**, **Per diem to date**,  and the **Per diem location**.</span></span> <span data-ttu-id="3a349-120">הסכום יחושב בהתבסס על תעריפי האש"ל עבור המיקום הנבחר והפחתת הארוחות תחושב על סמך רמות תעריפי האש"ל.</span><span class="sxs-lookup"><span data-stu-id="3a349-120">The amount will be calculated based on the per diem rates for the selected location and meal reduction will be calculated based on the per diem rate tiers.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]