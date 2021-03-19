---
title: הוצאות בין-חברתיות
description: נושא זה מספק מידע על אופן השימוש בהוצאות בין-חברות להקצאת הוצאות של עובדים לישות המשפטית שעבורה בוצעה העבודה.
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
ms.openlocfilehash: d908a1c062f5b7f01cf340dcd6f7f24714a992bf
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271534"
---
# <a name="intercompany-expenses"></a><span data-ttu-id="23ebf-103">הוצאות בין-חברתיות</span><span class="sxs-lookup"><span data-stu-id="23ebf-103">Intercompany expenses</span></span>

<span data-ttu-id="23ebf-104">עובד המועסק על ידי ישות משפטית אחת בארגון עשוי לבצע עבודה עבור ישות משפטית אחרת באותו ארגון.</span><span class="sxs-lookup"><span data-stu-id="23ebf-104">A worker who is employed by one legal entity in an organization might perform work for another legal entity in the same organization.</span></span> <span data-ttu-id="23ebf-105">ניתן להשתמש בהוצאות בין-חברות להקצאת הוצאות של עובדים לישות המשפטית שעבורה בוצעה העבודה.</span><span class="sxs-lookup"><span data-stu-id="23ebf-105">You can use intercompany expenses to assign the worker’s expenses to the legal entity for which the  work was performed.</span></span> <span data-ttu-id="23ebf-106">הישות המשפטית המעסיקה את העובד נקראת הישות המשפטית המשאילה.</span><span class="sxs-lookup"><span data-stu-id="23ebf-106">The legal entity that employs the worker is called the loaning legal entity.</span></span> <span data-ttu-id="23ebf-107">היישות המשפטית שעבורה העובד צובר הוצאות נקראת הישות המשפטית הלווה.</span><span class="sxs-lookup"><span data-stu-id="23ebf-107">The legal entity for which the worker incurs expenses is called the borrowing legal entity.</span></span> 

<span data-ttu-id="23ebf-108">כדי שעובד יוכל ליצור ולהגיש הוצאות בין-חברות, עליך להפעיל שורות של הוצאות בין-חברות.</span><span class="sxs-lookup"><span data-stu-id="23ebf-108">Before a worker can create and submit intercompany expenses, you must enable intercompany expense lines.</span></span> <span data-ttu-id="23ebf-109">בישות המשפטית המשאילה, בדף **פרמטרים לניהול הוצאות**, בחר **אפשר שורות הוצאות בין חברות**.</span><span class="sxs-lookup"><span data-stu-id="23ebf-109">In the loaning legal entity, on the **Expense management parameters** page, select **Allow intercompany expense lines**.</span></span> 

## <a name="tax-posting-for-intercompany-expenses"></a><span data-ttu-id="23ebf-110">רישום מס בגין הוצאות בין חברותיות</span><span class="sxs-lookup"><span data-stu-id="23ebf-110">Tax posting for intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="23ebf-111">לפני שתוכל להשתמש בקבוצות מס המשויכות לישות המשפטית (המקור) במקום לישות המשפטית הלווה (היעד) בדוח ההוצאות שלך, עליך להפעיל את הפונקציונליות בהגדרת מס מכירות בספר החשבונות הראשי.</span><span class="sxs-lookup"><span data-stu-id="23ebf-111">Before you can use tax groups that are associated with the loaning (source) legal entity instead of the borrowing (destination) legal entity in your expense report, you must enable the functionality in the General ledger sales tax setup.</span></span> <span data-ttu-id="23ebf-112">כאשר הפרמטר **ישות משפטית לרישום מס בין חברות** מוגדר **מקור** ההפרמטר **החל כללי מיסוי מס** נקבע **לא**, נעשה שימוש בשילוב המס של הישות המשפטית המלווה.</span><span class="sxs-lookup"><span data-stu-id="23ebf-112">When the **Legal entity for intercompany tax posting** parameter is set to **Source** and **Apply sales tax taxation rules** is set to **No**, the tax combination for the loaning legal entity is used.</span></span> <span data-ttu-id="23ebf-113">כאשר אותו פרמטר מוגדר ל **יעד**, ישמש שילוב מס בגין היישות משפטית הלווה.</span><span class="sxs-lookup"><span data-stu-id="23ebf-113">When the same parameter is set to **Destination**, the tax combination for borrowing legal entity will be used.</span></span> <span data-ttu-id="23ebf-114">עבור ישויות משפטיות בארצות הברית, כאשר הפרמטר מוגדר כ **מקור**, יש להגדיר גם את השדה **מע"מ לגביה** גם בדף **קבוצות רישום בספר החשבונות**.</span><span class="sxs-lookup"><span data-stu-id="23ebf-114">For legal entities in the United States, when the parameter is set to **Source**, the **Sales tax receivable** field must also be configured on the new **Ledger posting groups** page.</span></span> <span data-ttu-id="23ebf-115">מנוע הנהלת החשבונות ישתמש במידע משדה זה לצורך הזנות חשבונאות הקשורה למס.</span><span class="sxs-lookup"><span data-stu-id="23ebf-115">The accounting engine will use the information from this field for tax-related accounting entry.</span></span>   
<span data-ttu-id="23ebf-116">אופן הפעולה עקבית עבור שורות הוצאות שנרשמו עם או בלי פרויקט.</span><span class="sxs-lookup"><span data-stu-id="23ebf-116">The behavior is consistent for expense lines posted with or without a project.</span></span>  


[!INCLUDE[footer-include](../includes/footer-banner.md)]