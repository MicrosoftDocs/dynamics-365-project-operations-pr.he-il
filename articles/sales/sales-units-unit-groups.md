---
title: יחידות וקבוצות של יחידות
description: נושא זה מספק מידע על אופן יצירת יחידות וקבוצות יחידות ב- Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 345a4f38ad0bc5acddb90cfd8cb3e92154e46513
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077431"
---
# <a name="units-and-unit-groups"></a><span data-ttu-id="8826e-103">יחידות וקבוצות של יחידות</span><span class="sxs-lookup"><span data-stu-id="8826e-103">Units and unit groups</span></span>

<span data-ttu-id="8826e-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="8826e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8826e-105">יחידות הן הכמויות או המידות שבהן אתה מוכר את המוצרים או השירותים שלך.</span><span class="sxs-lookup"><span data-stu-id="8826e-105">Units are the quantities or measurements that you sell your products or services in.</span></span> <span data-ttu-id="8826e-106">לדוגמה, אם אתה מוכר מוצרים לגן, אתה יכול למכור זרעים ביחידות של מנות, תיבות או משטחים.</span><span class="sxs-lookup"><span data-stu-id="8826e-106">For example, if you sell gardening supplies, you might sell seeds in units of packets, boxes, and pallets.</span></span> <span data-ttu-id="8826e-107">קבוצת יחידות היא אוסף של יחידות שונות.</span><span class="sxs-lookup"><span data-stu-id="8826e-107">A unit group is a collection of these different units.</span></span>

<span data-ttu-id="8826e-108">להשלמת השלבים בנושא זה, ודא שהוקצה לך תפקיד של מנהל מערכת או מנהל Sales Professional או שיש לך הרשאות שוות ערך.</span><span class="sxs-lookup"><span data-stu-id="8826e-108">To complete the steps in this topic, make sure that you have been assigned to the System Administrator or Sales Professional Manager role or have equivalent permissions.</span></span>

## <a name="create-a-unit-group"></a><span data-ttu-id="8826e-109">יצירת קבוצת יחידות</span><span class="sxs-lookup"><span data-stu-id="8826e-109">Create a unit group</span></span>

1. <span data-ttu-id="8826e-110">במפת אתר, בחר **יחידות‬**.</span><span class="sxs-lookup"><span data-stu-id="8826e-110">In the site map, select **Units**.</span></span>
2. <span data-ttu-id="8826e-111">בחר **חדש** , ובתיבת הדו-שיח **צור קבוצת יחידות** הזן את שם היחידה.</span><span class="sxs-lookup"><span data-stu-id="8826e-111">Select **New** , and in the **Create Unit Group** dialog box, enter the unit name.</span></span>
3. <span data-ttu-id="8826e-112">בשדה **יחידה ראשית** הקלד את יחידת המידה המשותפת הקטנה ביותר שבה יימכר המוצר.</span><span class="sxs-lookup"><span data-stu-id="8826e-112">In the **Primary unit** field, enter the lowest common unit of measure that the product will be sold in.</span></span> <span data-ttu-id="8826e-113">לדוגמה, אפשר להזין "חתיכה" או "אונקיה".</span><span class="sxs-lookup"><span data-stu-id="8826e-113">For example, you might enter "piece" or "ounce".</span></span>
4. <span data-ttu-id="8826e-114">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="8826e-114">Select **OK**.</span></span>

## <a name="add-units-to-a-unit-group"></a><span data-ttu-id="8826e-115">הוספת יחידות לקבוצת יחידות</span><span class="sxs-lookup"><span data-stu-id="8826e-115">Add units to a unit group</span></span>

1. <span data-ttu-id="8826e-116">פתח קבוצת יחידות ובכרטיסיה **קשור** בחר **יחידות**.</span><span class="sxs-lookup"><span data-stu-id="8826e-116">Open a unit group, and on the **Related** tab, select **Units**.</span></span> <span data-ttu-id="8826e-117">תראה שהיחידה הראשית כבר נוספה.</span><span class="sxs-lookup"><span data-stu-id="8826e-117">You will see that the primary unit is already added.</span></span>
2. <span data-ttu-id="8826e-118">בחר **הוסף יחידה חדשה** , ובדף **יצירה מהירה: יחידה** , בשדה **שם** , הזן את שם היחידה.</span><span class="sxs-lookup"><span data-stu-id="8826e-118">Select **Add New Unit** , and on the **Quick Create: Unit** page, in the **Name** field, enter the nanem of the unit.</span></span>
3. <span data-ttu-id="8826e-119">בשדה **כמות** , הזן את הכמות שהיחידה תכיל.</span><span class="sxs-lookup"><span data-stu-id="8826e-119">In the **QUantity** field, enter the quantity that the unit will contain.</span></span> <span data-ttu-id="8826e-120">לדוגמה, אם תיבה מכילה שתי יחידות, הקלד "2".</span><span class="sxs-lookup"><span data-stu-id="8826e-120">For example, if a box contains two pieces, enter "2".</span></span> 
4. <span data-ttu-id="8826e-121">בשדה **יחידת בסיס** , בחר יחידת בסיס לקביעת יחידת המדידה הנמוכה ביותר ליחידה.</span><span class="sxs-lookup"><span data-stu-id="8826e-121">In the **Base unit** field, select a base unit to establish the lowest unit of measurement for the unit.</span></span> <span data-ttu-id="8826e-122">לדוגמה, ייתכן שתבחר באפשרות "חתיכה".</span><span class="sxs-lookup"><span data-stu-id="8826e-122">For example, you might select "Piece".</span></span>
5. <span data-ttu-id="8826e-123">בחר **שמור** :</span><span class="sxs-lookup"><span data-stu-id="8826e-123">Select **Save** :</span></span>
