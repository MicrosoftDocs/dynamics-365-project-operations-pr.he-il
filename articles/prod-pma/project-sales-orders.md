---
title: הזמנות מכירה בפרויקטים עבור פרויקטים של זמן וחומר
description: נושא זה מסביר כיצד ליצור הזמנות מכירה מבוססות פרויקטים עבור פרויקטים של זמן וחומר.
author: Yowelle
manager: AnnBe
ms.date: 04/05/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2019-04-05
ms.dyn365.ops.version: AX 10.0.2
ms.openlocfilehash: 74a90ea0bdb8f760273c0f6b1c61bffcb70b6c8d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289055"
---
# <a name="project-sales-orders-for-time-and-material-projects"></a><span data-ttu-id="b73cb-103">הזמנות מכירה בפרויקטים עבור פרויקטים של זמן וחומר</span><span class="sxs-lookup"><span data-stu-id="b73cb-103">Project sales orders for time and material projects</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="b73cb-104">נושא זה מתאר כיצד ליצור הזמנת מכירות לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="b73cb-104">This topic describes how to create a sales order for a project.</span></span> <span data-ttu-id="b73cb-105">ניתן ליצור הזמנות מכירה רק עבור פרויקטיים מסוג **זמן וחומר**.</span><span class="sxs-lookup"><span data-stu-id="b73cb-105">Sales orders can only be created for projects of type **time and material**.</span></span>

<span data-ttu-id="b73cb-106">אם לפרויקט זמן וחומר יש כמה מקורות מימון בחוזה הפרויקט, עליך להפוך את הפרמטר **אפשר הזמנות מכירה עבור פרויקטים עם כמה מקורות מימון** לזמין בדף **ניהול פרויקטים ופרמטרים חשבונאיים**.</span><span class="sxs-lookup"><span data-stu-id="b73cb-106">If a time and material project has multiple funding sources on the project contract, you must enable the **Allow sales orders for projects with multiple funding sources** parameter on the **Project management and accounting parameters** page.</span></span> 

> [!NOTE]
> - <span data-ttu-id="b73cb-107">תמיכה בהזמנות מכירה של פרויקטים עם כמה מקורות מימון זמינה החל ממהדורת יישום 10.0.2 ואילך.</span><span class="sxs-lookup"><span data-stu-id="b73cb-107">Support for project sales orders with multiple funding sources is available starting with application release 10.0.2 and higher.</span></span>
> - <span data-ttu-id="b73cb-108">הפרמטר להפעלת תמיכה בהזמנות מכירה של פרויקט עם כמה מקורות מימון יוסר בגל ההפצה של אפריל 2020, שלאחריו הפונקציונליות תמיד תהיה מופעלת.</span><span class="sxs-lookup"><span data-stu-id="b73cb-108">The parameter to enable the support for project sales orders with multiple funding sources will be removed in the April 2020 release wave, after which the functionality will always be enabled.</span></span>

<span data-ttu-id="b73cb-109">ניתן ליצור הזמנות מכירה מבוססות פרויקט בשתי דרכים:</span><span class="sxs-lookup"><span data-stu-id="b73cb-109">You can create project-based sales orders in two ways:</span></span>

- <span data-ttu-id="b73cb-110">מעבר אל הפרויקט עצמו.</span><span class="sxs-lookup"><span data-stu-id="b73cb-110">Go to the project itself.</span></span> <span data-ttu-id="b73cb-111">בחלונית הפעולות, בחר **ניהול > משימות פריט > הזמנת מכירות**.</span><span class="sxs-lookup"><span data-stu-id="b73cb-111">On the Action Pane, select **Manage > Item tasks > Sales order**.</span></span> <span data-ttu-id="b73cb-112">פרטי הפרויקט יוגדרו כברירת מחדל להזמנת המכירות מהפרויקט.</span><span class="sxs-lookup"><span data-stu-id="b73cb-112">The project information will default to the sales order from the project.</span></span> <span data-ttu-id="b73cb-113">אם בחוזה הפרויקט יש יותר ממקור מימון אחד, יהיה עליך לבחור במקור המימון כדי להגדיר את הלקוח להזמנת המכירות.</span><span class="sxs-lookup"><span data-stu-id="b73cb-113">If the project contract has more than one funding source, you will need to select the funding source to set the customer for the sales order.</span></span> <span data-ttu-id="b73cb-114">אם יש רק מקור מימון אחד לפרויקט, הלקוח יוגדר אוטומטית.</span><span class="sxs-lookup"><span data-stu-id="b73cb-114">If there is only one funding source for the project, the customer will be automatically set.</span></span>
- <span data-ttu-id="b73cb-115">עבור אל דף הרשימה **כל הזמנות המכירה** וצור הזמנת מכירות חדשה.</span><span class="sxs-lookup"><span data-stu-id="b73cb-115">Go to the **All sales order** list page and create a new sales order.</span></span> <span data-ttu-id="b73cb-116">עליך לבחור את הפרויקט להזמנת המכירות.</span><span class="sxs-lookup"><span data-stu-id="b73cb-116">You will need to select the project for the sales order.</span></span> <span data-ttu-id="b73cb-117">לאחר בחירת הפרויקט, הלקוח יוגדר ממקור המימון או שתצטרך לבחור את מקור המימון אם לחוזה הפרויקט יש כמה מקורות מימון.</span><span class="sxs-lookup"><span data-stu-id="b73cb-117">After the project is selected, the customer will be set from the funding source or you will need to select the funding source if the project contract has multiple funding sources.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]