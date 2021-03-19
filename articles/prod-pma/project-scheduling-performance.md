---
title: ביצועים של תזמון משאבי פרויקט
description: נושא זה מספק מידע על אופן השיפור בביצועים של תזמון משאבים למספר רב של פרויקטים.
author: Yowelle
manager: AnnBe
ms.date: 08/31/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.14
ms.search.validFrom: 2020-09-01
ms.openlocfilehash: 34c31570778f9b64c23387112cf56fa1139cd0fd
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289010"
---
# <a name="project-resource-scheduling-performance"></a><span data-ttu-id="15f07-103">ביצועים של תזמון משאבי פרויקט</span><span class="sxs-lookup"><span data-stu-id="15f07-103">Project resource scheduling performance</span></span>

[!include [banner](../includes/banner.md)]
[!include [banner](../includes/preview-banner.md)]


<span data-ttu-id="15f07-104">בעיות ביצועים הקשורות לתזמון משאבים יכולות להתרחש כאשר מספר הפרויקטים מגיע לאלפים.</span><span class="sxs-lookup"><span data-stu-id="15f07-104">Performance issues related to resource scheduling can occur when the number of projects reaches into the thousands.</span></span> <span data-ttu-id="15f07-105">כדי לשפר את ביצועי תזמון המשאבים, קיימת תכונה המאפשרת למשתמשים לצמצם את הזמן שנדרש להפעלת טופס זמינות המשאבים.</span><span class="sxs-lookup"><span data-stu-id="15f07-105">To improve resource scheduling performance, a feature is available that allows users to reduce the time that it takes to launch the resource availability form.</span></span> <span data-ttu-id="15f07-106">באופן ספציפי, היא מסירה את תהליך הסינכרון של אוסף קיבולת המשאבים ומשתמשת בטבלה **ResProjectResource** כדי להאיץ את חיפוש המשאבים.</span><span class="sxs-lookup"><span data-stu-id="15f07-106">Specifically, this removes the resource capacity roll-up synchronization process and uses the **ResProjectResource** table to speed up the resource lookup.</span></span> <span data-ttu-id="15f07-107">שים לב שהטבלה **ResRollup** כבר לא בשימוש.</span><span class="sxs-lookup"><span data-stu-id="15f07-107">Note that the **ResRollup** table will no longer be used.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="15f07-108">אם יש תלות בתהליך הסינכרון של אוסף קיבולת המשאבים או בטבלה **ResProjectResource**, אל תשתמש בתכונה זו.</span><span class="sxs-lookup"><span data-stu-id="15f07-108">If there is a dependency on either the resource capacity roll-up synchronization process or the **ResProjectResource** table, do not use this feature.</span></span>

## <a name="enable-resource-scheduling-performance-enhancement"></a><span data-ttu-id="15f07-109">הפעל שיפור ביצועי תזמון משאבים</span><span class="sxs-lookup"><span data-stu-id="15f07-109">Enable resource scheduling performance enhancement</span></span>
<span data-ttu-id="15f07-110">כדי להפעיל שיפור של ביצועי תזמון משאבים, בצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="15f07-110">To enable resource scheduling performance enhancement, complete the following steps.</span></span>

1. <span data-ttu-id="15f07-111">עבור אל **ניהול תכונות** > **הכל**, וברשימת התכונות מצא את **הפעל את תכונת שיפור ביצועי תזמון משאבי פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="15f07-111">Go to **Feature management** > **All**, and in the feature list, locate **Enable project resource scheduling performance enhancement feature**.</span></span>
2. <span data-ttu-id="15f07-112">בחר **הפוך לזמין כעת**.</span><span class="sxs-lookup"><span data-stu-id="15f07-112">Select **Enable now**.</span></span>

> [!NOTE]
> <span data-ttu-id="15f07-113">אם אינך יכול למצוא את התכונה ברשימה, בחר **בדוק עדכונים** כדי לרענן את הרשימה.</span><span class="sxs-lookup"><span data-stu-id="15f07-113">If you can't find the feature in the list, select **Check for updates** to refresh the list.</span></span>

3. <span data-ttu-id="15f07-114">רענן את הדפדפן ועבור אל **ניהול פרויקטים וחשבונאות** > **תקופתי** > **משאבי פרויקט** > **סנכרן את יכולות יומני המשאבים בכל החברות**.</span><span class="sxs-lookup"><span data-stu-id="15f07-114">Refresh your browser, and then go to **Project management and accounting** > **Periodic** > **Project resources** > **Synchronize resource calendars capacity across all companies**.</span></span>
4. <span data-ttu-id="15f07-115">הגדר את **הסר רשומות קיבולת קיימות** שיהיו **כן** כדי להסיר נתונים קודמים.</span><span class="sxs-lookup"><span data-stu-id="15f07-115">Set **Remove existing capacity records** to **Yes** to remove previous data.</span></span> <span data-ttu-id="15f07-116">אם ברצונך ליצור נתונים מצטברים, הגדר **לא**.</span><span class="sxs-lookup"><span data-stu-id="15f07-116">If you want generate incremental data, set it to **No**.</span></span>
5. <span data-ttu-id="15f07-117">בשדה **קוד תקופה**, בחר את התקופה שבה יש ליצור נתונים.</span><span class="sxs-lookup"><span data-stu-id="15f07-117">In the **Period code** field, select the period in which data should be generated.</span></span> <span data-ttu-id="15f07-118">אם אתה בוחר קוד תקופתי, אין צורך להגדיר תאריך התחלה וסיום.</span><span class="sxs-lookup"><span data-stu-id="15f07-118">If you select a period code, a start and end date do not need to be defined.</span></span>
6. <span data-ttu-id="15f07-119">אם אתה משאיר את השדה **קוד תקופה** ריק, בחר תאריכי התחלה וסיום ספציפיים ליצירת נתונים.</span><span class="sxs-lookup"><span data-stu-id="15f07-119">If you leave the **Period code** field blank, select specific start and end dates to generate data.</span></span>
7. <span data-ttu-id="15f07-120">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="15f07-120">Select **OK**.</span></span>

 > [!NOTE]
 > <span data-ttu-id="15f07-121">זה יפיץ נתונים כלליים לטבלה **ResCalendarCapacity** בכל החברות בסביבתך, כך שעבודת האצווה צריכה להתנהל רק בישות משפטית אחת.</span><span class="sxs-lookup"><span data-stu-id="15f07-121">This will distribute general data to the **ResCalendarCapacity** table across all companies in your environment, so the batch job only needs to be run in one legal entity.</span></span> <span data-ttu-id="15f07-122">הנתונים במשימת אצווה זו נדרשים לחישוב יכולת המשאבים דרך לוח השנה המשויך.</span><span class="sxs-lookup"><span data-stu-id="15f07-122">The data in this batch job is needed to calculate resource capacity through the associated calendar.</span></span>

8. <span data-ttu-id="15f07-123">עבור אל **ניהול פרויקטים וחשבונאות** > **תקופתי** > **משאבי פרויקט** > **אכלס משאבי פרויקטים בכל החברות** ובחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="15f07-123">Go to **Project management and accounting** > **Periodic** > **Project resources** > **Populate project resources across all companies** and then select **OK**.</span></span> <span data-ttu-id="15f07-124">זהו סקריפט לשדרוג הנתונים עבור נתונים כלליים בטבלאות **ResProjectResource**, **ResCalendarDateTimeRange**, **ResEffectiveDateTimeRange**.</span><span class="sxs-lookup"><span data-stu-id="15f07-124">This is the data upgrade script for general data in the **ResProjectResource**, **ResCalendarDateTimeRange**, and **ResEffectiveDateTimeRange** tables.</span></span> <span data-ttu-id="15f07-125">ערכים עבור השדה **PSAPRojSchedRole.RootActivity** עודכנו.</span><span class="sxs-lookup"><span data-stu-id="15f07-125">Values for the **PSAPRojSchedRole.RootActivity** field are also updated.</span></span> <span data-ttu-id="15f07-126">אם זה לא מופעל, תקבל אזהרה כשתנסה לבצע פעולות תזמון משאבים.</span><span class="sxs-lookup"><span data-stu-id="15f07-126">If this is not run, you will receive a warning when you try to execute resource scheduling operations.</span></span>
 
## <a name="turn-off-resource-scheduling-performance-enhancement"></a><span data-ttu-id="15f07-127">השבת את שיפור ביצועי תזמון משאבים</span><span class="sxs-lookup"><span data-stu-id="15f07-127">Turn off resource scheduling performance enhancement</span></span>

1. <span data-ttu-id="15f07-128">עבור אל **ניהול תכונות** > **הכל**, וחפש את **הפעל את תכונת שיפור ביצועי תזמון משאבי פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="15f07-128">Go to **Feature management** > **All**  and search for **Enable project resource scheduling performance enhancement feature**.</span></span>
2. <span data-ttu-id="15f07-129">בחר את התכונה, ואז בחר בלחצן **השבת**.</span><span class="sxs-lookup"><span data-stu-id="15f07-129">Select the feature, and then select the **Disable** button.</span></span>
3. <span data-ttu-id="15f07-130">רענן את הדפדפן.</span><span class="sxs-lookup"><span data-stu-id="15f07-130">Refresh your browser.</span></span>
4. <span data-ttu-id="15f07-131">עבור אל **ניהול פרויקטים וחשבונאות** > **תקופתי** > **סנכרון קיבולת** > **סנכרון פעולות סיכום של קיבולת משאבים**.</span><span class="sxs-lookup"><span data-stu-id="15f07-131">Go to **Project management and accounting** > **Periodic** > **Capacity synchronization** > **Synchronize resource capacity roll-ups**.</span></span>
5. <span data-ttu-id="15f07-132">בדף **סנכרון סיכום קיבולת**, הגדר **הסר רשומות קיבולת קיימות** שיהיו **כן** כדי להסיר נתונים קודמים.</span><span class="sxs-lookup"><span data-stu-id="15f07-132">On the **Capacity roll-up synchronization** page, set **Remove existing capacity records** to **Yes** to remove previous data.</span></span> <span data-ttu-id="15f07-133">אם ברצונך ליצור נתונים מצטברים, הגדר **לא**.</span><span class="sxs-lookup"><span data-stu-id="15f07-133">If you want to generate incremental data, set it to **No**.</span></span>
6. <span data-ttu-id="15f07-134">בשדה **קוד תקופה**, בחר את התקופה שבה יש ליצור נתונים.</span><span class="sxs-lookup"><span data-stu-id="15f07-134">In the **Period code** field, select the period in which data should be generated.</span></span> <span data-ttu-id="15f07-135">אם אתה בוחר קוד תקופתי, אין צורך להגדיר תאריך התחלה וסיום.</span><span class="sxs-lookup"><span data-stu-id="15f07-135">If you select a period code, a start and end date do not need to be defined.</span></span>
7. <span data-ttu-id="15f07-136">אם אתה משאיר את השדה **קוד תקופה** ריק, בחר תאריכי התחלה וסיום ספציפיים ליצירת נתונים.</span><span class="sxs-lookup"><span data-stu-id="15f07-136">If you leave the **Period code** field blank, select specific start and end dates to generate data.</span></span>
8. <span data-ttu-id="15f07-137">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="15f07-137">Select **OK**.</span></span>

> [!NOTE]
> <span data-ttu-id="15f07-138">זה יפיץ נתונים כלליים לטבלה **ResRollup‎** בכל החברות בסביבתך, כך שעבודת האצווה צריכה להתנהל רק בישות משפטית אחת.</span><span class="sxs-lookup"><span data-stu-id="15f07-138">This will distribute general data to the **ResRollup** table across all companies in your environment, so the batch job only needs to be run in one legal entity.</span></span> <span data-ttu-id="15f07-139">עבודת אצווה זו נחוצה לכל התצוגות של **זמינות משאבים**.</span><span class="sxs-lookup"><span data-stu-id="15f07-139">This batch job is needed for all **Resource Availability** views.</span></span> <span data-ttu-id="15f07-140">אם עבודת אצווה זו לא מופעלת, נתוני **ResRollup** ייווצרו בזמן אמת, וזה יכול לקחת זמן.</span><span class="sxs-lookup"><span data-stu-id="15f07-140">If this batch job is not run, the **ResRollup** data will be generated on the fly, which can take time.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]