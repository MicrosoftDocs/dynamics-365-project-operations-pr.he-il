---
title: הוצאות בין-חברתיות
description: עובד המועסק על ידי ישות משפטית אחת בארגון עשוי לבצע עבודה עבור ישות משפטית אחרת באותו ארגון. במצב זה, ניתן להשתמש בתכונת ההוצאות הבין-חברתי כדי להקצות את הוצאות העובד לישות המשפטית שעבורה בוצעה העבודה.
author: ShylaThompson
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 0967f23e4e1f8e0431c55d4d54554e7e90e2451c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077459"
---
# <a name="intercompany-expenses"></a><span data-ttu-id="99be2-104">הוצאות בין-חברתיות</span><span class="sxs-lookup"><span data-stu-id="99be2-104">Intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="99be2-105">עובד המועסק על ידי ישות משפטית אחת בארגון עשוי לבצע עבודה עבור ישות משפטית אחרת באותו ארגון.</span><span class="sxs-lookup"><span data-stu-id="99be2-105">A worker who is employed by one legal entity in an organization might perform work for another legal entity in the same organization.</span></span> <span data-ttu-id="99be2-106">במצב זה, ניתן להשתמש בתכונת ההוצאות הבין-חברתי כדי להקצות את הוצאות העובד לישות המשפטית שעבורה בוצעה העבודה.</span><span class="sxs-lookup"><span data-stu-id="99be2-106">In this situation, you can use the intercompany expense feature to assign the worker’s expenses to the legal entity for which the work was performed.</span></span> <span data-ttu-id="99be2-107">הישות המשפטית המעסיקה את העובד נקראת הישות המשפטית המשאילה.</span><span class="sxs-lookup"><span data-stu-id="99be2-107">The legal entity that employs the worker is called the loaning legal entity.</span></span> <span data-ttu-id="99be2-108">היישות המשפטית שעבורה העובד צובר הוצאות נקראת הישות המשפטית הלווה.</span><span class="sxs-lookup"><span data-stu-id="99be2-108">The legal entity for which the worker incurs expenses is called the borrowing legal entity.</span></span> 

<span data-ttu-id="99be2-109">לפני שעובד יכול ליצור ולהגיש הוצאות בגין עבודה המתבצעת עבור ישות משפטית אחרת, בישות המשפטית המשאילה, בדף **פרמטרים לניהול הוצאות** בחר את האפשרות **אפשר שורות הוצאות בין חברתיות**.</span><span class="sxs-lookup"><span data-stu-id="99be2-109">Before a worker can create and submit expenses for work that is performed for a different legal entity, in the loaning legal entity, on the **Expense management parameters** page, select the **Allow intercompany expense lines** option.</span></span> 

## <a name="tax-posting-for-intercompany-expenses"></a><span data-ttu-id="99be2-110">רישום מס בגין הוצאות בין חברותיות</span><span class="sxs-lookup"><span data-stu-id="99be2-110">Tax posting for intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="99be2-111">אם ברצונך להשתמש בקבוצות מס המשויכות לישות המשפטית המשאילה (המקור) במקום לישות המשפטית הלווה (היעד) בדוח ההוצאות שלך, יהיה עליך להגדיר זאת במס מכירות ספר החשבונות הראשי.</span><span class="sxs-lookup"><span data-stu-id="99be2-111">If you want to use tax groups that are associated with the loaning (source) legal entity instead of the borrowing (destination) legal entity in your expense report, you will need to configure this in the General ledger sales tax set up.</span></span> <span data-ttu-id="99be2-112">כאשר פרמטר ספר החשבונות הראשי, **ישות משפטית לרישום מס בין חברתי** מוגדר כ **מקור** ו **החל כללי מיסוי של מס מכירות** מוגדר כ **לא** , ישמש שילוב המס בגין הישות המשפטית המשאילה.</span><span class="sxs-lookup"><span data-stu-id="99be2-112">When the General ledger parameter, **Legal entity for intercompany tax posting** is set to **Source** and **Apply sales tax taxation rules** is set to **No** , the tax combination for the loaning legal entity will be used.</span></span> <span data-ttu-id="99be2-113">כאשר אותו פרמטר מוגדר ל **יעד** , ישמש שילוב מס בגין היישות משפטית הלווה.</span><span class="sxs-lookup"><span data-stu-id="99be2-113">When the same parameter is set to **Destination** , the tax combination for borrowing legal entity will be used.</span></span> <span data-ttu-id="99be2-114">עבור ישויות משפטיות בארצות הברית, כאשר הפרמטר מוגדר כ **מקור** , יש להגדיר גם את השדה **מע"מ לגביה** גם בדף **קבוצות רישום בספר החשבונות**.</span><span class="sxs-lookup"><span data-stu-id="99be2-114">For legal entities in the United States, when the parameter is set to **Source** , the **Sales tax receivable** field must also be configured on the new **Ledger posting groups** page.</span></span> <span data-ttu-id="99be2-115">מנוע הנהלת החשבונות ישתמש במידע משדה זה לצורך הזנות חשבונאות הקשורה למס.</span><span class="sxs-lookup"><span data-stu-id="99be2-115">The accounting engine will use the information from this field for tax related accounting entry.</span></span>   
<span data-ttu-id="99be2-116">אופן הפעולה עקבית עבור שורות הוצאות שנרשמו עם או בלי פרויקט.</span><span class="sxs-lookup"><span data-stu-id="99be2-116">The behavior is consistent for expense lines posted with or without a project.</span></span>  
