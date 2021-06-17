---
title: יחידות וקבוצות של יחידות
description: נושא זה מספק מידע על אופן יצירת יחידות וקבוצות יחידות ב- Dynamics 365 Project Operations.
author: rumant
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 646e20189efb4aab56972f01a52b1bff19f2e79f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996072"
---
# <a name="units-and-unit-groups"></a><span data-ttu-id="99cab-103">יחידות וקבוצות של יחידות</span><span class="sxs-lookup"><span data-stu-id="99cab-103">Units and unit groups</span></span>

<span data-ttu-id="99cab-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="99cab-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="99cab-105">יחידות הן הכמויות או המידות שבהן אתה מוכר את המוצרים או השירותים שלך.</span><span class="sxs-lookup"><span data-stu-id="99cab-105">Units are the quantities or measurements that you sell your products or services in.</span></span> <span data-ttu-id="99cab-106">לדוגמה, אם אתה מוכר מוצרים לגן, אתה יכול למכור זרעים ביחידות של מנות, תיבות או משטחים.</span><span class="sxs-lookup"><span data-stu-id="99cab-106">For example, if you sell gardening supplies, you might sell seeds in units of packets, boxes, and pallets.</span></span> <span data-ttu-id="99cab-107">קבוצת יחידות היא אוסף של יחידות שונות.</span><span class="sxs-lookup"><span data-stu-id="99cab-107">A unit group is a collection of these different units.</span></span>

<span data-ttu-id="99cab-108">להשלמת השלבים בנושא זה, ודא שהוקצה לך תפקיד של מנהל מערכת או מנהל Sales Professional או שיש לך הרשאות שוות ערך.</span><span class="sxs-lookup"><span data-stu-id="99cab-108">To complete the steps in this topic, make sure that you have been assigned to the System Administrator or Sales Professional Manager role or have equivalent permissions.</span></span>

## <a name="create-a-unit-group"></a><span data-ttu-id="99cab-109">יצירת קבוצת יחידות</span><span class="sxs-lookup"><span data-stu-id="99cab-109">Create a unit group</span></span>

1. <span data-ttu-id="99cab-110">במפת אתר, בחר **יחידות‬**.</span><span class="sxs-lookup"><span data-stu-id="99cab-110">In the site map, select **Units**.</span></span>
2. <span data-ttu-id="99cab-111">בחר **חדש**, ובתיבת הדו-שיח **צור קבוצת יחידות** הזן את שם היחידה.</span><span class="sxs-lookup"><span data-stu-id="99cab-111">Select **New**, and in the **Create Unit Group** dialog box, enter the unit name.</span></span>
3. <span data-ttu-id="99cab-112">בשדה **יחידה ראשית** הקלד את יחידת המידה המשותפת הקטנה ביותר שבה יימכר המוצר.</span><span class="sxs-lookup"><span data-stu-id="99cab-112">In the **Primary unit** field, enter the lowest common unit of measure that the product will be sold in.</span></span> <span data-ttu-id="99cab-113">לדוגמה, אפשר להזין "חתיכה" או "אונקיה".</span><span class="sxs-lookup"><span data-stu-id="99cab-113">For example, you might enter "piece" or "ounce".</span></span>
4. <span data-ttu-id="99cab-114">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="99cab-114">Select **OK**.</span></span>

## <a name="add-units-to-a-unit-group"></a><span data-ttu-id="99cab-115">הוספת יחידות לקבוצת יחידות</span><span class="sxs-lookup"><span data-stu-id="99cab-115">Add units to a unit group</span></span>

1. <span data-ttu-id="99cab-116">פתח קבוצת יחידות ובכרטיסיה **קשור** בחר **יחידות**.</span><span class="sxs-lookup"><span data-stu-id="99cab-116">Open a unit group, and on the **Related** tab, select **Units**.</span></span> <span data-ttu-id="99cab-117">תראה שהיחידה הראשית כבר נוספה.</span><span class="sxs-lookup"><span data-stu-id="99cab-117">You will see that the primary unit is already added.</span></span>
2. <span data-ttu-id="99cab-118">בחר **הוסף יחידה חדשה**, ובדף **יצירה מהירה: יחידה**, בשדה **שם**, הזן את שם היחידה.</span><span class="sxs-lookup"><span data-stu-id="99cab-118">Select **Add New Unit**, and on the **Quick Create: Unit** page, in the **Name** field, enter the nanem of the unit.</span></span>
3. <span data-ttu-id="99cab-119">בשדה **כמות**, הזן את הכמות שהיחידה תכיל.</span><span class="sxs-lookup"><span data-stu-id="99cab-119">In the **QUantity** field, enter the quantity that the unit will contain.</span></span> <span data-ttu-id="99cab-120">לדוגמה, אם תיבה מכילה שתי יחידות, הקלד "2".</span><span class="sxs-lookup"><span data-stu-id="99cab-120">For example, if a box contains two pieces, enter "2".</span></span> 
4. <span data-ttu-id="99cab-121">בשדה **יחידת בסיס**, בחר יחידת בסיס לקביעת יחידת המדידה הנמוכה ביותר ליחידה.</span><span class="sxs-lookup"><span data-stu-id="99cab-121">In the **Base unit** field, select a base unit to establish the lowest unit of measurement for the unit.</span></span> <span data-ttu-id="99cab-122">לדוגמה, ייתכן שתבחר באפשרות "חתיכה".</span><span class="sxs-lookup"><span data-stu-id="99cab-122">For example, you might select "Piece".</span></span>
5. <span data-ttu-id="99cab-123">בחר **שמור**:</span><span class="sxs-lookup"><span data-stu-id="99cab-123">Select **Save**:</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]