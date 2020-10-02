---
title: שדות של Project Operations כממדי תמחור
description: נושא זה מספק מידע על שימוש בשדות כממדי תמחור ב- Dynamics 365 Project Operations.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: 3ddf3098e45fdc9b99067b64df05e2adc0b6ad05
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896417"
---
# <a name="project-operations-fields-as-pricing-dimensions"></a><span data-ttu-id="34681-103">שדות של Project Operations כממדי תמחור</span><span class="sxs-lookup"><span data-stu-id="34681-103">Project Operations fields as pricing dimensions</span></span>

<span data-ttu-id="34681-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="34681-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="34681-105">לישות **‏‫נתונים בפועל‬** יש שדות רבים שיכולים לשמש כמידות תמחור לתמחור מבוסס משאבים.</span><span class="sxs-lookup"><span data-stu-id="34681-105">The **Actuals** entity has many fields that can be used as pricing dimensions for resource-based pricing.</span></span> <span data-ttu-id="34681-106">לדוגמה, שדה משותף אחד הוא **משאב ניתן להזמנה**.</span><span class="sxs-lookup"><span data-stu-id="34681-106">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="34681-107">חברות קטנות יותר, בעלות פחות מ- 20-30 משאבים הניתנים לחיוב, עשויות להחליט שהגישה הפשוטה ביותר היא להקצות תעריפי חיוב ועלות ספציפיים לכל משאב.</span><span class="sxs-lookup"><span data-stu-id="34681-107">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="34681-108">עם זאת, ככל שכוח העבודה שניתן לחיוב גדל, ייתכן שהתעריפים הספציפיים למשאבים לא יהיו מתאימים לתחזוקה.</span><span class="sxs-lookup"><span data-stu-id="34681-108">However, as the billable workforce grows, resource-secific rates could become unrealistic to maintain.</span></span> <span data-ttu-id="34681-109">עלויות המשאבים ושיעורי החיוב מתחילים להשתנות ככל שהמשאבים מקודמים, צוברים יותר ניסיון או רוכשים מיומנויות שונות.</span><span class="sxs-lookup"><span data-stu-id="34681-109">Resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different set of skills.</span></span> 

<span data-ttu-id="34681-110">דוגמה נוספת היא קטגוריית עסקה.</span><span class="sxs-lookup"><span data-stu-id="34681-110">Another example is that of transaction category.</span></span> <span data-ttu-id="34681-111">לקוחות ומיישמים משתמשים בקטגוריית העסקה כדי לסווג את העבודה, ומשתמשים בשדה לקביעת המחיר והעלות בהתאם לקטגוריית העבודה.</span><span class="sxs-lookup"><span data-stu-id="34681-111">Customers and Implementers have used the transaction category to classify work and use the field to price and cost based on the category of work.</span></span>
