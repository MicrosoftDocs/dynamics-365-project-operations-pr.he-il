---
title: סוגי תקופות
description: נושא זה מספק מידע על אופן הגדרת סוגי תקופות להערכת הכנסות.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 107cecbc1dabdf13147d847bf1816f44cc2703c5
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287284"
---
# <a name="period-types"></a><span data-ttu-id="f32f7-103">סוגי תקופות</span><span class="sxs-lookup"><span data-stu-id="f32f7-103">Period types</span></span>

<span data-ttu-id="f32f7-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="f32f7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="f32f7-105">סוג תקופה מגדיר את תדירות ההערכה של הכנסות בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="f32f7-105">A period type defines how frequently revenue on a project is estimated.</span></span> <span data-ttu-id="f32f7-106">נושא זה מספק מידע על אופן הגדרת סוגי תקופות להערכת הכנסות.</span><span class="sxs-lookup"><span data-stu-id="f32f7-106">This topic provides information about how to set up period types for revenue estimation.</span></span> 

## <a name="create-and-work-with-period-types"></a><span data-ttu-id="f32f7-107">יצירה ועבודה עם סוגי תקופות</span><span class="sxs-lookup"><span data-stu-id="f32f7-107">Create and work with period types</span></span>
<span data-ttu-id="f32f7-108">כדי ליצור ולעבוד עם סוגי תקופות, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="f32f7-108">To create and work with period types, complete the following steps:</span></span>

1. <span data-ttu-id="f32f7-109">בסביבת Dynamics 365 Finance שלך, עבור אל **ניהול פרויקטים וחשבונאות** > **הגדרה** > **אומדנים** > **סוגי תקופות**.</span><span class="sxs-lookup"><span data-stu-id="f32f7-109">In your Dynamics 365 Finance environment, go to **Project management and accounting** > **Setup** > **Estimates** > **Period types**.</span></span>
2. <span data-ttu-id="f32f7-110">ליצירת סוג תקופה חדש, בחר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="f32f7-110">Select **New** to create new period type.</span></span> <span data-ttu-id="f32f7-111">הזן שם ותיאור.</span><span class="sxs-lookup"><span data-stu-id="f32f7-111">Enter a name and description.</span></span>
3. <span data-ttu-id="f32f7-112">בשדה **תדירות** בחר ערך:</span><span class="sxs-lookup"><span data-stu-id="f32f7-112">In the **Frequency** field, select a value:</span></span>

    - <span data-ttu-id="f32f7-113">אם תבחר **שבוע**, **דו-שבועי**, **פעמיים בחודש**, **חודש**, **יום**, **רבעון**, או **שנה**, לוח השנה ישמש ליצירת התקופות.</span><span class="sxs-lookup"><span data-stu-id="f32f7-113">If you select **Week**, **Bi-weekly**, **Semi-monthly**, **Month**, **Day**, **Quarter**, or **Year**, the calendar will be used to generate the periods.</span></span> 
    - <span data-ttu-id="f32f7-114">אם תבחר **תקופת ספר חשבונות**, תקופות ספר החשבונות מתצורת ספר החשבונות הכללי ישמשו ליצירת תקופות.</span><span class="sxs-lookup"><span data-stu-id="f32f7-114">If you select **Ledger period**, ledger periods from the General ledger configuration will be used to generate periods.</span></span>
    - <span data-ttu-id="f32f7-115">אם תבחר **ללא הגבלה**, אתה יכול לציין תקופות מותאמות אישית.</span><span class="sxs-lookup"><span data-stu-id="f32f7-115">If you select **Unlimited**, you can specify custom periods.</span></span>
4. <span data-ttu-id="f32f7-116">בחר את הרשומה של סוג התקופה ובחר **צור תקופות** כדי ליצור תקופות עבור סוג התקופה.</span><span class="sxs-lookup"><span data-stu-id="f32f7-116">Select the period type record and then select **Generate periods** to create periods for the period type.</span></span> <span data-ttu-id="f32f7-117">בהתבסס על תדירות התקופה שבחרת, ייתכן שתהיה לך אפשרות לציין תאריך התחלה או את מספר התקופות שייווצרו.</span><span class="sxs-lookup"><span data-stu-id="f32f7-117">Based on the period frequency that you selected, you might have the option to specify a start date or the number of periods to generate.</span></span>
5. <span data-ttu-id="f32f7-118">בחר **תקופות** כדי לסקור את התקופות שנוצרו.</span><span class="sxs-lookup"><span data-stu-id="f32f7-118">Select **Periods** to review generated periods.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]