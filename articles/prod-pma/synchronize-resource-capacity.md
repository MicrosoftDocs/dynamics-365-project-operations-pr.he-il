---
title: סנכרון הקיבולת של משאב
description: נושא זה מספק מידע על אופן הסנכרון של קיבולת המשאב בין לוחות שנה ופרויקטים.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: e6b63ccb5b0f04dedb8a942e22d6e1993204dc20
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288561"
---
# <a name="synchronize-resource-capacity"></a><span data-ttu-id="05c24-103">סנכרון הקיבולת של משאב</span><span class="sxs-lookup"><span data-stu-id="05c24-103">Synchronize resource capacity</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="05c24-104">התהליכים לסנכרון משאבים מסייעים להבטיח שמידע עבור לוח השנה ובסיס היומן זולג לתזמון משאבי הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="05c24-104">The processes for resource synchronization help guarantee that information for the calendar and base calendar trickles down into project resource scheduling.</span></span> <span data-ttu-id="05c24-105">אם לוח השנה משתנה, התהליכים מבצעים את העדכונים הנדרשים לתזמון משאבי הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="05c24-105">If the calendar is changed, the processes make the required updates to the scheduling of project resources.</span></span> <span data-ttu-id="05c24-106">התהליכים גם עוזרים בשיפור הביצועים מכיוון שמידע המשאבים של לוח השנה מסונכרן מראש.</span><span class="sxs-lookup"><span data-stu-id="05c24-106">The processes also help improve performance, because the calendar's resource information is synchronized in advance.</span></span> <span data-ttu-id="05c24-107">לכן, עדכונים למידע על תזמון משאבים מתרחשים במהירות רבה יותר.</span><span class="sxs-lookup"><span data-stu-id="05c24-107">Therefore, updates to resource scheduling information occur more quickly.</span></span> <span data-ttu-id="05c24-108">אנו ממליצים לתזמן את התהליכים כאצווה אחת במקום אחד בכל פעם.</span><span class="sxs-lookup"><span data-stu-id="05c24-108">We recommend that you schedule the processes as a batch instead of one at a time.</span></span> <span data-ttu-id="05c24-109">אחרת, קיים סיכון שמישהו ישכח את התאריכים הכלולים שבהם המידע סונכרן לאחרונה.</span><span class="sxs-lookup"><span data-stu-id="05c24-109">Otherwise, there is a risk that someone will forget the inclusive dates when the information was last synchronized.</span></span> <span data-ttu-id="05c24-110">אם לא משתמשים בתאריכים כוללניים, עלולים להיווצר פערים במהלך סנכרון התאריכים.</span><span class="sxs-lookup"><span data-stu-id="05c24-110">If inclusive dates aren't used, gaps can occur during date synchronization.</span></span>

![סנכרון לוח שנה](./media/projectresourcing04-1024x471.jpg)

## <a name="synchronize-resource-capacity-roll-ups"></a><span data-ttu-id="05c24-112">סנכרן את פעולות הסיכום של קיבולת המשאב</span><span class="sxs-lookup"><span data-stu-id="05c24-112">Synchronize resource capacity roll-ups</span></span>

<span data-ttu-id="05c24-113">תהליך הסנכרון נועד לסנכרן את כל המידע שביומן המשאבים.</span><span class="sxs-lookup"><span data-stu-id="05c24-113">The synchronization process is designed to synchronize all resource calendar information.</span></span> <span data-ttu-id="05c24-114">מידע זה כולל מידע בסיסי ביומן אודות כל שינוי בטבלת קיבולת לוח השנה של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="05c24-114">This information includes base calendar information about any changes to the project's Resource calendar capacity table.</span></span> <span data-ttu-id="05c24-115">אם מתווספים משאבים חדשים בפרויקט הסנכרון עוזר להבטיח שמידע לוח השנה המעודכן זמין.</span><span class="sxs-lookup"><span data-stu-id="05c24-115">If new resources are added in the project, synchronization helps guarantee that the updated calendar information is available.</span></span> <span data-ttu-id="05c24-116">ניתן לבצע סינכרון זה בכל עת.</span><span class="sxs-lookup"><span data-stu-id="05c24-116">This synchronization can be done at any time.</span></span>

<span data-ttu-id="05c24-117">אנו ממליצים לך להשתמש באצווה.</span><span class="sxs-lookup"><span data-stu-id="05c24-117">We recommend that you use a batch.</span></span> <span data-ttu-id="05c24-118">האפשרויות זמינות במהלך סנכרון הזמנות קיבולת.</span><span class="sxs-lookup"><span data-stu-id="05c24-118">The options are available during synchronization of capacity reservations.</span></span>

1. <span data-ttu-id="05c24-119">בחר **ניהול פרויקטים וחשבונאות** &gt; **תקופתי** &gt; **סנכרון קיבולת** &gt; **סנכרן פעולות סיכום של קיבולת משאבים**.</span><span class="sxs-lookup"><span data-stu-id="05c24-119">Select **Project management and accounting** &gt; **Periodic** &gt; **Capacity synchronization** &gt; **Synchronize resources capacity roll-ups**.</span></span>
2. <span data-ttu-id="05c24-120">הגדר את האפשרויות השונות שבטבלה הבאה.</span><span class="sxs-lookup"><span data-stu-id="05c24-120">Set the options in the following table.</span></span>

    | <span data-ttu-id="05c24-121">אפשרות</span><span class="sxs-lookup"><span data-stu-id="05c24-121">Option</span></span>      | <span data-ttu-id="05c24-122">תיאור</span><span class="sxs-lookup"><span data-stu-id="05c24-122">Description</span></span> |
    |-------------|-------------|
    | <span data-ttu-id="05c24-123">קוד תקופה</span><span class="sxs-lookup"><span data-stu-id="05c24-123">Period code</span></span> | <span data-ttu-id="05c24-124">בחר באופן אופציונלי את קוד מרווח תאריכי ספר החשבונות הכללי כדי לקבוע את תאריכי ההתחלה והסיום לתהליך הסנכרון עבור פעולות סיכום של קיבולת משאבים.</span><span class="sxs-lookup"><span data-stu-id="05c24-124">Optionally select the General ledger date interval code to set the start and end dates for the synchronization process for resource capacity roll-ups.</span></span> |
    | <span data-ttu-id="05c24-125">תאריך התחלה</span><span class="sxs-lookup"><span data-stu-id="05c24-125">Start date</span></span>  | <span data-ttu-id="05c24-126">הזן את תאריך ההתחלה של תהליך הסנכרון עבור פעולות סיכום של קיבולת משאבים.</span><span class="sxs-lookup"><span data-stu-id="05c24-126">Enter the start date for the synchronization process for resource capacity roll-ups.</span></span> |
    | <span data-ttu-id="05c24-127">תאריך סיום</span><span class="sxs-lookup"><span data-stu-id="05c24-127">End date</span></span>    | <span data-ttu-id="05c24-128">הזן את תאריך הסיום של תהליך הסנכרון עבור פעולות סיכום של קיבולת משאבים.</span><span class="sxs-lookup"><span data-stu-id="05c24-128">Enter the end date for the synchronization process for resource capacity roll-ups.</span></span> |

<span data-ttu-id="05c24-129">[![תהליך הסינכרון](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)</span><span class="sxs-lookup"><span data-stu-id="05c24-129">[![Synchronization process](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]