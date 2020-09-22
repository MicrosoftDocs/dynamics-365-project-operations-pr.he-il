---
title: חוזי הפרוייקט
description: נושא זה מספק דוגמאות לחוזי הפרוייקט שניתן ליצור עבור סוגים שונים של פרוייקטים ומקורות מימון, וכיצד ניתן לנהל חוזים ולהפיק חשבוניות ללקוחות בפרוייקט.
author: KimANelson
manager: AnnBe
ms.date: 11/03/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectContractsListPage, ProjProjectsListPage
audience: Application User, IT Pro
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 23561
ms.assetid: bfd18d9b-d9a6-4e21-bc95-bf4af45f617f
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 854ddfe6db93b7e93a4ee640268a9c8f254f24e7
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751836"
---
# <a name="project-contracts"></a><span data-ttu-id="0ede2-103">חוזי הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="0ede2-103">Project contracts</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="0ede2-104">מאמר זה מספק דוגמאות לחוזי הפרוייקט שניתן ליצור עבור סוגים שונים של פרוייקטים ומקורות מימון, וכיצד ניתן לנהל חוזים ולהפיק חשבוניות ללקוחות בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-104">This article provides examples of the project contracts that you can create for various types of projects and funding sources, and how you can manage contracts and invoice project customers.</span></span>

<span data-ttu-id="0ede2-105">סוג הפרוייקט שתיצור עבור חוזה פרוייקט קובע את השיטה המשמשת להפקת חשבוניות ללקוחות בפרוייקטים.</span><span class="sxs-lookup"><span data-stu-id="0ede2-105">The type of project that you create for a project contract determines the method that is used to invoice project customers.</span></span> <span data-ttu-id="0ede2-106">תוכל לשנות חוזה פרוייקט ואת הפרוייקט הקשור, אך לא תוכל לשנות את סוג הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-106">You can change a project contract and the related project, but you can't change the project type.</span></span> 

<span data-ttu-id="0ede2-107">באמצעות חוזה פרוייקט, תוכל להפיק חשבוניות לפרוייקט אחד או יותר בו-זמנית.</span><span class="sxs-lookup"><span data-stu-id="0ede2-107">By using a project contract, you can invoice one or more projects at the same time.</span></span> <span data-ttu-id="0ede2-108">בנוסף, חוזה הפרוייקט עוזר להבטיח תהליך עקבי להפקת חשבוניות עבור פרוייקט משנה במבנה פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-108">The project contract also helps guarantee a consistent invoicing procedure for every subproject in a project structure.</span></span> 

<span data-ttu-id="0ede2-109">כל פרוייקט שתופק עבורו חשבונית חייב להיות משויך לחוזה פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-109">Every project that will be invoiced must be associated with a project contract.</span></span> <span data-ttu-id="0ede2-110">ההגדרות עבור חוזה פרוייקט חלות על כל הפרוייקטים ופרוייקטי המשנה שמשויכים לאותו חוזה פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-110">The settings for a project contract apply to all projects and subprojects that are associated with that project contract.</span></span> 

<span data-ttu-id="0ede2-111">חוזה פרוייקט יכול לציין מקור מימון אחד או יותר.</span><span class="sxs-lookup"><span data-stu-id="0ede2-111">A project contract can specify one or more sources of funding.</span></span> <span data-ttu-id="0ede2-112">לכן, ניתן לפצל את החיוב בין כמה מממנים, להגדיר מגבלות מימון כך שמקורות המימון לא יחויבו בסכום הגדול מהסכום המוגדר ולהגדיר כללי מימון לחיוב הוצאות כספיות.</span><span class="sxs-lookup"><span data-stu-id="0ede2-112">Therefore, you can split the billing among multiple funders, set up funding limits so that funding sources are not billed more than a specified amount, and configure funding rules for charging expenditures.</span></span>

## <a name="funding-for-project-contracts"></a><span data-ttu-id="0ede2-113">מימון לחוזי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="0ede2-113">Funding for project contracts</span></span>
<span data-ttu-id="0ede2-114">חוזי פרוייקט מסוימים מציינים שמספר גורמים חולקים את האחריות למימון עלויות הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-114">Some project contracts specify that multiple parties share the responsibility for funding the project costs.</span></span> <span data-ttu-id="0ede2-115">להלן מספר דוגמאות:</span><span class="sxs-lookup"><span data-stu-id="0ede2-115">Here are some examples:</span></span>

-   <span data-ttu-id="0ede2-116">לקוח גדול שיש לו כמה חטיבות מבקש לפצל את מימון הפרוייקט לפי חטיבה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-116">A large customer that has multiple divisions requests that funding of a project be split by division.</span></span>
-   <span data-ttu-id="0ede2-117">החברה שלך חולקת את העלויות של פרוייקט גדול עם ארגון חיצוני.</span><span class="sxs-lookup"><span data-stu-id="0ede2-117">Your company shares the costs of a large project with an external organization.</span></span>
-   <span data-ttu-id="0ede2-118">פרויקט כבישים ממומן על-ידי שתי ערים.</span><span class="sxs-lookup"><span data-stu-id="0ede2-118">A  road project is co-funded by two municipalities.</span></span>
-   <span data-ttu-id="0ede2-119">פרוייקט גשר ממומן על ידי מענק ממשלתי ותאגיד פרטי.</span><span class="sxs-lookup"><span data-stu-id="0ede2-119">A bridge project is funded by a government grant and a private corporation.</span></span>

<span data-ttu-id="0ede2-120">ב- Dynamics 365 Finance, תוכל לפצל את החיוב בגין עסקה אחת או פרוייקט שלם בין כמה לקוחות, מענקים או ארגונים.</span><span class="sxs-lookup"><span data-stu-id="0ede2-120">In Dynamics 365 Finance, you can split the billing for a single transaction or an entire project among multiple customers, grants, or organizations.</span></span> 

<span data-ttu-id="0ede2-121">בפרוייקטים שיש להם כמה מממנים, כל הגורמים שתורמים למימון של פרוייקט מימון מתקדם נקראים מקורות מימון.</span><span class="sxs-lookup"><span data-stu-id="0ede2-121">In projects that have multiple funders, all parties that contribute to the funding of an advanced funding project are called funding sources.</span></span> <span data-ttu-id="0ede2-122">לאחר שלקוח, ארגון או מענק מוגדרים כמקור מימון, ניתן להקצות אותו לכלל מימון אחד או יותר.</span><span class="sxs-lookup"><span data-stu-id="0ede2-122">After a customer, organization, or grant is defined as a funding source, it can be assigned to one or more funding rules.</span></span> <span data-ttu-id="0ede2-123">כללי המימון מכילים את הקריטריונים הקובעים את אופן הקצאת החיובים למקורות המימון השונים לפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-123">Funding rules contain the criteria that determines how charges are allocated to the various funding sources for a project.</span></span> 

<span data-ttu-id="0ede2-124">מכיוון שלא ניתן לפצל פריטים במלאי, כמו פריטים המופיעים בדרישות הרכש ובהזמנות הרכש, לא ניתן לפצל את סכום העלות בין מקורות מימון מרובים בזמן ההפצה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-124">Because stocked items, such as those that appear on purchase requisitions and purchase orders, can't be split, the cost amount can't be split among multiple funding sources at the time of distribution.</span></span> <span data-ttu-id="0ede2-125">לכן, ערך מקור המימון נשאר 0 (אפס) עד לפרסום הנפקת המלאי.</span><span class="sxs-lookup"><span data-stu-id="0ede2-125">Therefore, the funding source value remains 0 (zero) until the inventory issue is posted.</span></span> <span data-ttu-id="0ede2-126">עם פרסום הנפקת המלאי, סכום העלות מופץ על פי כללי ‏‫התפלגות תיק לקוח‬.</span><span class="sxs-lookup"><span data-stu-id="0ede2-126">When the inventory issue is posted, the cost amount is distributed according to the account distribution rules for the project.</span></span>

<span data-ttu-id="0ede2-127">להלן מספר צעדים שתוכל לנקוט כדי להקל על פיצול החיוב בין מקורות מימון מרובים:</span><span class="sxs-lookup"><span data-stu-id="0ede2-127">Here are some steps that you can take to make it easier to split the billing among multiple funding sources:</span></span>

-   <span data-ttu-id="0ede2-128">ציין שכל העסקאות שהוזנו לפרוייקט משתמשות באותו מטבע מכירות כמו חוזה הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-128">Specify that all transactions that are entered for a project use the same sales currency as the project contract.</span></span>
-   <span data-ttu-id="0ede2-129">הגדר מגבלות מימון, כך שמקור מימון לא יחויב יותר מסכום מוגדר עבור פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-129">Set up funding limits, so that a funding source isn't invoiced more than a specified amount toward a project.</span></span>
-   <span data-ttu-id="0ede2-130">הגדר כללי מימון ומגבלות מימון עבור כל עובד, פריט, קטגוריה, קבוצת קטגוריה וסוג עסקה (או לכל סוגי העסקאות).</span><span class="sxs-lookup"><span data-stu-id="0ede2-130">Configure funding rules and funding limits for each worker, item, category, category group, and transaction type (or for all transaction types).</span></span>
-   <span data-ttu-id="0ede2-131">בחר תאריכי התחלה וסיום אופציונליים כדי להגדיר את התקופה שבה כל כלל מימון יהיה בתוקף.</span><span class="sxs-lookup"><span data-stu-id="0ede2-131">Select optional start and end dates to define the period when each funding rule is valid.</span></span>
-   <span data-ttu-id="0ede2-132">ציין את האחוז שעליו אחראי כל מקור מימון.</span><span class="sxs-lookup"><span data-stu-id="0ede2-132">Specify the percentage that each funding source is responsible for.</span></span>
-   <span data-ttu-id="0ede2-133">ציין איזה מקור מימון אחראי על הפרשי עיגול הנגרמים על ידי חישובי הקצאת מימון.</span><span class="sxs-lookup"><span data-stu-id="0ede2-133">Specify which funding source is responsible for rounding differences that are caused by funding allocation calculations.</span></span>
-   <span data-ttu-id="0ede2-134">הגדר כללים הקובעים כיצד עלויות פרוייקט יחויבו עבור לקוחות חיצוניים וכיצד הן יחויבו לארגונים פנימיים.</span><span class="sxs-lookup"><span data-stu-id="0ede2-134">Set up rules that determine how project costs are invoiced to external customers and charged to internal organizations.</span></span>
-   <span data-ttu-id="0ede2-135">תעד עסקאות בחשבון מימון בהחזקה עד לקבלת מימון נוסף, או עד שתחליט לשאת בעלויות באופן פנימי.</span><span class="sxs-lookup"><span data-stu-id="0ede2-135">Record transactions in an on-hold funding account until additional funding can be obtained, or until you decide to bear the costs internally.</span></span>

<span data-ttu-id="0ede2-136">כדי לקבוע איזו קבוצת מס לשייך לעסקה, מתבצע חיפוש בפרוייקט להקצאת קבוצת מס.</span><span class="sxs-lookup"><span data-stu-id="0ede2-136">To determine which tax group to associate with a transaction, the project is searched for a tax group assignment.</span></span> <span data-ttu-id="0ede2-137">אם לא בוצעה הקצאה לקבוצת מס ברמת הפרוייקט, מתבצע חיפוש בחוזה הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-137">If no tax group assignment has been made at the project level, the project contract is searched.</span></span>

### <a name="example-multiple-funding-sources-simple"></a><span data-ttu-id="0ede2-138">דוגמה: מקורות מימון מרובים (פשוט)</span><span class="sxs-lookup"><span data-stu-id="0ede2-138">Example: Multiple funding sources (simple)</span></span>

<span data-ttu-id="0ede2-139">הטבלה הבאה מציגה תרחישים לניהול הקצאת מימון בין מקורות מימון מרובים.</span><span class="sxs-lookup"><span data-stu-id="0ede2-139">The following table provides scenarios for managing funding allocation among multiple funding sources.</span></span> <span data-ttu-id="0ede2-140">תרחישים אלה מבוססים על ההנחות הבאות:</span><span class="sxs-lookup"><span data-stu-id="0ede2-140">These scenarios are based on the following assumptions:</span></span>

-   <span data-ttu-id="0ede2-141">הגדרות עדיפות משוקללות בהקצאת הכספים לפני החלת קריטריונים אחרים של כלל המימון.</span><span class="sxs-lookup"><span data-stu-id="0ede2-141">Priority settings are factored into the allocation of funds before other funding rule criteria are applied.</span></span>
-   <span data-ttu-id="0ede2-142">לא צוין טווח תאריכים שיגדיר את התקופה שבה כלל המימון תקף.</span><span class="sxs-lookup"><span data-stu-id="0ede2-142">No date range has been specified to define the period d when the funding rule is valid.</span></span>

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="0ede2-143"><strong>תרחיש</strong></span><span class="sxs-lookup"><span data-stu-id="0ede2-143"><strong>Scenario</strong></span></span></td>
<td><span data-ttu-id="0ede2-144"><strong>מקור מימון</strong></span><span class="sxs-lookup"><span data-stu-id="0ede2-144"><strong>Funding source</strong></span></span></td>
<td><span data-ttu-id="0ede2-145"><strong>אחוז הקצאה</strong></span><span class="sxs-lookup"><span data-stu-id="0ede2-145"><strong>Allocation percentage</strong></span></span></td>
<td><span data-ttu-id="0ede2-146"><strong>עדיפות הקצאה</strong></span><span class="sxs-lookup"><span data-stu-id="0ede2-146"><strong>Allocation priority</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0ede2-147">ברצונך להקצות עלויות למקור מימון אחד עד למיצוי הכספים, להקצות עלויות למקור מימון שני עד למיצוי הכספי שלו ולבסוף להקצות את העלויות הנותרות למקור מימון שלישי.</span><span class="sxs-lookup"><span data-stu-id="0ede2-147">You want to allocate costs to one funding source until its funds are exhausted, allocate costs to a second funding source until its funds are exhausted, and finally allocate the remaining costs to a third funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="0ede2-148">מקור　מימון　1</span><span class="sxs-lookup"><span data-stu-id="0ede2-148">Funding　source　1</span></span></li>
<li><span data-ttu-id="0ede2-149">מקור　מימון　2</span><span class="sxs-lookup"><span data-stu-id="0ede2-149">Funding　source　2</span></span></li>
<li><span data-ttu-id="0ede2-150">מקור　מימון　3</span><span class="sxs-lookup"><span data-stu-id="0ede2-150">Funding　source　3</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="0ede2-151">100%</span><span class="sxs-lookup"><span data-stu-id="0ede2-151">100%</span></span></li>
<li><span data-ttu-id="0ede2-152">100%</span><span class="sxs-lookup"><span data-stu-id="0ede2-152">100%</span></span></li>
<li><span data-ttu-id="0ede2-153">100%</span><span class="sxs-lookup"><span data-stu-id="0ede2-153">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="0ede2-154">1</span><span class="sxs-lookup"><span data-stu-id="0ede2-154">1</span></span></li>
<li><span data-ttu-id="0ede2-155">2</span><span class="sxs-lookup"><span data-stu-id="0ede2-155">2</span></span></li>
<li><span data-ttu-id="0ede2-156">3</span><span class="sxs-lookup"><span data-stu-id="0ede2-156">3</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0ede2-157">ברצונך להקצות 75 אחוז מהעלויות למקור מימון אחד ו- 25 אחוז למקור מימון שני.</span><span class="sxs-lookup"><span data-stu-id="0ede2-157">You want to allocate 75 percent of costs to one funding source and 25 percent to a second funding source.</span></span> <span data-ttu-id="0ede2-158">כאשר אחד ממקורות המימון הללו מוצה, תרצה לשלם את העלויות הנותרות ממקור מימון שלישי.</span><span class="sxs-lookup"><span data-stu-id="0ede2-158">When either of those funding sources is exhausted, you want to pay the remaining costs from a third funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="0ede2-159">מקור　מימון　1</span><span class="sxs-lookup"><span data-stu-id="0ede2-159">Funding　source　1</span></span></li>
<li><span data-ttu-id="0ede2-160">מקור　מימון　2</span><span class="sxs-lookup"><span data-stu-id="0ede2-160">Funding　source　2</span></span></li>
<li><span data-ttu-id="0ede2-161">מקור　מימון　3</span><span class="sxs-lookup"><span data-stu-id="0ede2-161">Funding　source　3</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="0ede2-162">75%</span><span class="sxs-lookup"><span data-stu-id="0ede2-162">75%</span></span></li>
<li><span data-ttu-id="0ede2-163">25%</span><span class="sxs-lookup"><span data-stu-id="0ede2-163">25%</span></span></li>
<li><span data-ttu-id="0ede2-164">100%</span><span class="sxs-lookup"><span data-stu-id="0ede2-164">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="0ede2-165">1</span><span class="sxs-lookup"><span data-stu-id="0ede2-165">1</span></span></li>
<li><span data-ttu-id="0ede2-166">1</span><span class="sxs-lookup"><span data-stu-id="0ede2-166">1</span></span></li>
<li><span data-ttu-id="0ede2-167">2</span><span class="sxs-lookup"><span data-stu-id="0ede2-167">2</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0ede2-168">ברצונך להקצות 75 אחוז מהעלויות למקור מימון אחד ו- 25 אחוז למקור מימון שני.</span><span class="sxs-lookup"><span data-stu-id="0ede2-168">You want to allocate 75 percent of costs to one funding source and 25 percent to a second funding source.</span></span> <span data-ttu-id="0ede2-169">כאשר אחד ממקורות המימון הללו מוצה, תרצה לפצל את העלויות הנותרות בין מקור מימון שלישי ומקור מימון רביעי.</span><span class="sxs-lookup"><span data-stu-id="0ede2-169">When either of those funding sources is exhausted, you want to split the remaining costs between a third funding source and a fourth funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="0ede2-170">מקור　מימון　1</span><span class="sxs-lookup"><span data-stu-id="0ede2-170">Funding　source　1</span></span></li>
<li><span data-ttu-id="0ede2-171">מקור　מימון　2</span><span class="sxs-lookup"><span data-stu-id="0ede2-171">Funding　source　2</span></span></li>
<li><span data-ttu-id="0ede2-172">מקור　מימון　3</span><span class="sxs-lookup"><span data-stu-id="0ede2-172">Funding　source　3</span></span></li>
<li><span data-ttu-id="0ede2-173">מקור　מימון　4</span><span class="sxs-lookup"><span data-stu-id="0ede2-173">Funding　source　4</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="0ede2-174">75%</span><span class="sxs-lookup"><span data-stu-id="0ede2-174">75%</span></span></li>
<li><span data-ttu-id="0ede2-175">25%</span><span class="sxs-lookup"><span data-stu-id="0ede2-175">25%</span></span></li>
<li><span data-ttu-id="0ede2-176">50%</span><span class="sxs-lookup"><span data-stu-id="0ede2-176">50%</span></span></li>
<li><span data-ttu-id="0ede2-177">50%</span><span class="sxs-lookup"><span data-stu-id="0ede2-177">50%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="0ede2-178">1</span><span class="sxs-lookup"><span data-stu-id="0ede2-178">1</span></span></li>
<li><span data-ttu-id="0ede2-179">1</span><span class="sxs-lookup"><span data-stu-id="0ede2-179">1</span></span></li>
<li><span data-ttu-id="0ede2-180">2</span><span class="sxs-lookup"><span data-stu-id="0ede2-180">2</span></span></li>
<li><span data-ttu-id="0ede2-181">2</span><span class="sxs-lookup"><span data-stu-id="0ede2-181">2</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0ede2-182">ברצונך להקצות את 25 האחוזים הראשונים מהעלויות למקור מימון אחד ואת השאר למקור מימון שני.</span><span class="sxs-lookup"><span data-stu-id="0ede2-182">You want to allocate the first 25 percent of costs to one funding source and the rest to a second funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="0ede2-183">מקור　מימון　1</span><span class="sxs-lookup"><span data-stu-id="0ede2-183">Funding　source　1</span></span></li>
<li><span data-ttu-id="0ede2-184">מקור　מימון　2</span><span class="sxs-lookup"><span data-stu-id="0ede2-184">Funding　source　2</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="0ede2-185">25%</span><span class="sxs-lookup"><span data-stu-id="0ede2-185">25%</span></span></li>
<li><span data-ttu-id="0ede2-186">100%</span><span class="sxs-lookup"><span data-stu-id="0ede2-186">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="0ede2-187">1</span><span class="sxs-lookup"><span data-stu-id="0ede2-187">1</span></span></li>
<li><span data-ttu-id="0ede2-188">2</span><span class="sxs-lookup"><span data-stu-id="0ede2-188">2</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

### <a name="example-multiple-funding-sources-complex"></a><span data-ttu-id="0ede2-189">דוגמה: מקורות מימון מרובים (מורכב)</span><span class="sxs-lookup"><span data-stu-id="0ede2-189">Example: Multiple funding sources (complex)</span></span>

<span data-ttu-id="0ede2-190">יש לך שלושה מקורות מימון שבהם ברצונך להשתמש בסדר הבא:</span><span class="sxs-lookup"><span data-stu-id="0ede2-190">You have three funding sources that you want to use in the following order:</span></span>

1.  <span data-ttu-id="0ede2-191">השתמש במקור מימון 2 ובמקור מימון 3 באופן שווה עד למיצוי מקור מימון 2.</span><span class="sxs-lookup"><span data-stu-id="0ede2-191">Use funding source 2 and funding source 3 equally until funding source 2 is exhausted.</span></span>
2.  <span data-ttu-id="0ede2-192">המשך להשתמש במקור מימון 3 עד למיצויו.</span><span class="sxs-lookup"><span data-stu-id="0ede2-192">Continue to use funding source 3 until it is exhausted.</span></span>
3.  <span data-ttu-id="0ede2-193">השתמש במקור מימון 1 לאחר שמיצוי מקור מימון 3.</span><span class="sxs-lookup"><span data-stu-id="0ede2-193">Use funding source 1 after funding source 3 is exhausted.</span></span>

<span data-ttu-id="0ede2-194">כדי להשיג יעד זה, עליך לבצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="0ede2-194">To accomplish this goal, you must do the following:</span></span>

-   <span data-ttu-id="0ede2-195">הגדר מגבלות מימון למקור מימון 2 ולמקור מימון 3, עבור הסכומים המתאימים שלהם.</span><span class="sxs-lookup"><span data-stu-id="0ede2-195">Set up funding limits for funding source 2 and funding source 3, for their respective amounts.</span></span>
-   <span data-ttu-id="0ede2-196">צור את כללי המימון הבאים:</span><span class="sxs-lookup"><span data-stu-id="0ede2-196">Create the following funding rules:</span></span>
    -   <span data-ttu-id="0ede2-197">כלל 1 (עדיפות 1): הקצה 50 אחוז מהעסקאות למקור מימון 2 ו- 50 אחוז למקור מימון 3.</span><span class="sxs-lookup"><span data-stu-id="0ede2-197">Rule 1 (Priority 1): Allocate 50 percent of transactions to funding source 2 and 50 percent to funding source 3.</span></span>
    -   <span data-ttu-id="0ede2-198">כלל 2 (עדיפות 2): הקצה 100 אחוז מהעסקאות למקור מימון 3.</span><span class="sxs-lookup"><span data-stu-id="0ede2-198">Rule 2 (Priority 2): Allocate 100 percent of transactions to funding source 3.</span></span>
    -   <span data-ttu-id="0ede2-199">כלל 3 (עדיפות 3): הקצה 100 אחוז מהעסקאות למקור מימון 1.</span><span class="sxs-lookup"><span data-stu-id="0ede2-199">Rule 3 (Priority 3): Allocate 100 percent of transactions to funding source 1.</span></span>

<span data-ttu-id="0ede2-200">הגדרה זו פועלת מכיוון שעסקאות נבדקות כנגד כללים ומגבלות כדי לקבוע אם אחד מהם חל על העסקה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-200">This setup works because transactions are checked against rules and limits to determine whether any of them apply to the transaction.</span></span> <span data-ttu-id="0ede2-201">אם לא חלים כללים או מגבלות ספציפיים על העסקה, הכלל 'כל העסקאות' חל.</span><span class="sxs-lookup"><span data-stu-id="0ede2-201">If no specific rules or limits apply to the transaction, the All transactions rule applies.</span></span> <span data-ttu-id="0ede2-202">הכלל 'כל העסקאות' מתאים לכל העסקאות.</span><span class="sxs-lookup"><span data-stu-id="0ede2-202">The All transactions rule matches all transactions.</span></span> 

<span data-ttu-id="0ede2-203">אם נמצא כלל התואם לעסקה, תחילה מוחל האחוז שהוקצה לכלל זה, אך רק לאחר בדיקת ההתאמות מול מגבלות שהוגדרו.</span><span class="sxs-lookup"><span data-stu-id="0ede2-203">If a rule is found that matches a transaction, the percentage that has been allocated in that rule is applied first, but only after the matches are checked against any limits that have been set up.</span></span> <span data-ttu-id="0ede2-204">אם התקיימה מגבלה, ומוצו הכספים של מקור המימון, המערכת מתעלמת מכלל המימון שמשויך למגבלת המימון והתוכנית מחפשת את הכלל הבא שחל.</span><span class="sxs-lookup"><span data-stu-id="0ede2-204">If a limit has been met, and a funding source’s funds are exhausted, the funding rule that is associated with the funding limit is disregarded, and the program checks for the next rule that applies.</span></span> 

<span data-ttu-id="0ede2-205">במקרים מסוימים, ניתן להקצות רק חלק מהעסקה תחת כלל.</span><span class="sxs-lookup"><span data-stu-id="0ede2-205">In some cases, only part of a transaction can be allocated under a rule.</span></span> <span data-ttu-id="0ede2-206">זה עשוי לקרות מכיוון שמגבלה הושגה בעת הקצאת העסקה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-206">This might happen because a limit is reached when the transaction is allocated.</span></span> <span data-ttu-id="0ede2-207">במקרה כזה, רק סכום מסוים מוקצה לפי כלל זה, כגון 50 אחוז לכל מקור מימון.</span><span class="sxs-lookup"><span data-stu-id="0ede2-207">In this case, only a certain amount is allocated according to that rule, such as 50 percent to each funding source.</span></span> <span data-ttu-id="0ede2-208">זהו המקרה בכלל 1, שתיארנו קודם לכן בסעיף זה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-208">This is the case in rule 1, which is described earlier in this section.</span></span> <span data-ttu-id="0ede2-209">היתרה מוקצית בהתאם לכלל הבא ברצף.</span><span class="sxs-lookup"><span data-stu-id="0ede2-209">The remainder is allocated according to the next rule in the sequence.</span></span> 

<span data-ttu-id="0ede2-210">הטבלה הבאה בוחנת תרחיש זה ביתר פירוט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-210">The following table examines this scenario in more detail.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="0ede2-211"><strong>מוקד</strong></span><span class="sxs-lookup"><span data-stu-id="0ede2-211"><strong>Focus</strong></span></span></td>
<td><span data-ttu-id="0ede2-212"><strong>פרטים</strong></span><span class="sxs-lookup"><span data-stu-id="0ede2-212"><strong>Details</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0ede2-213">כללי מימון</span><span class="sxs-lookup"><span data-stu-id="0ede2-213">Funding rules</span></span></td>
<td><ul>
<li><span data-ttu-id="0ede2-214">כלל 1 (עדיפות 1): כל העסקאות.</span><span class="sxs-lookup"><span data-stu-id="0ede2-214">Rule 1 (Priority 1): All transactions.</span></span> <span data-ttu-id="0ede2-215">הקצה את מקור המימון 2 ל- 50% ואת מקור המימון 3 ל- 50%.</span><span class="sxs-lookup"><span data-stu-id="0ede2-215">Allocate funding source 2 at 50% and funding source 3 at 50%.</span></span></li>
<li><span data-ttu-id="0ede2-216">כלל 2 (עדיפות 2): כל העסקאות.</span><span class="sxs-lookup"><span data-stu-id="0ede2-216">Rule 2 (Priority 2): All transactions.</span></span> <span data-ttu-id="0ede2-217">הקצה את מקור המימון 3 ב- 100%.</span><span class="sxs-lookup"><span data-stu-id="0ede2-217">Allocate funding source 3 at 100%.</span></span></li>
<li><span data-ttu-id="0ede2-218">כלל 3 (עדיפות 2): כל העסקאות.</span><span class="sxs-lookup"><span data-stu-id="0ede2-218">Rule 3 (Priority 2): All transactions.</span></span> <span data-ttu-id="0ede2-219">הקצה את מקור המימון 1 ב- 100%.</span><span class="sxs-lookup"><span data-stu-id="0ede2-219">Allocate funding source 1 at 100%.</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0ede2-220">מגבלות מימון</span><span class="sxs-lookup"><span data-stu-id="0ede2-220">Funding limits</span></span></td>
<td><ul>
<li><span data-ttu-id="0ede2-221">מגבלת מקור מימון 1 = 10,000.00</span><span class="sxs-lookup"><span data-stu-id="0ede2-221">Funding source 1 limit = 10,000.00</span></span></li>
<li><span data-ttu-id="0ede2-222">מגבלת מקור מימון 2 = 500.00</span><span class="sxs-lookup"><span data-stu-id="0ede2-222">Funding source 2 limit = 500.00</span></span></li>
<li><span data-ttu-id="0ede2-223">מגבלת מקור מימון 3 = 750.00</span><span class="sxs-lookup"><span data-stu-id="0ede2-223">Funding source 3 limit = 750.00</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0ede2-224">עסקה 1</span><span class="sxs-lookup"><span data-stu-id="0ede2-224">Transaction 1</span></span></td>
<td><span data-ttu-id="0ede2-225"><strong>סכום העסקה:</strong> 100.00<strong>מימון:</strong> העסקה משולמת בהתאם לכלל 1 בלבד, בגלל שהעסקה משולמת במלואה לאחר שכלל 1 חל.</span><span class="sxs-lookup"><span data-stu-id="0ede2-225"><strong>Transaction amount:</strong> 100.00<strong>Funding:</strong> The transaction is paid according to rule 1 only, because the transaction is fully paid after rule 1 is applied.</span></span> <span data-ttu-id="0ede2-226">העסקה ממומנת באופן שווה בין מקור מימון 2 ומקור מימון 3.</span><span class="sxs-lookup"><span data-stu-id="0ede2-226">The transaction is funded equally between funding source 2 and funding source 3.</span></span>
<ul>
<li><span data-ttu-id="0ede2-227">מקור מימון 2:‏ 50.00</span><span class="sxs-lookup"><span data-stu-id="0ede2-227">Funding source 2: 50.00</span></span></li>
<li><span data-ttu-id="0ede2-228">מקור מימון 3:‏ 50.00</span><span class="sxs-lookup"><span data-stu-id="0ede2-228">Funding source 3: 50.00</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0ede2-229">עסקה 2</span><span class="sxs-lookup"><span data-stu-id="0ede2-229">Transaction 2</span></span></td>
<td><span data-ttu-id="0ede2-230"><strong>סכום העסקה:</strong> 5,000.00<strong>מימון:</strong> העסקה משולמת בהתאם לשלושת הכללים.</span><span class="sxs-lookup"><span data-stu-id="0ede2-230"><strong>Transaction amount:</strong> 5,000.00<strong>Funding:</strong> The transaction is paid according to all three rules.</span></span> <span data-ttu-id="0ede2-231"><strong>כלל 1</strong>
</span><span class="sxs-lookup"><span data-stu-id="0ede2-231"><strong>Rule 1</strong>
</span></span><ul>
<li><span data-ttu-id="0ede2-232">מקור מימון 2:‏ 450.00</span><span class="sxs-lookup"><span data-stu-id="0ede2-232">Funding source 2: 450.00</span></span></li>
<li><span data-ttu-id="0ede2-233">מקור מימון 3:‏ 450.00</span><span class="sxs-lookup"><span data-stu-id="0ede2-233">Funding source 3: 450.00</span></span></li>
</ul><span data-ttu-id="0ede2-234">
<strong>כלל 2</strong>
</span><span class="sxs-lookup"><span data-stu-id="0ede2-234">
<strong>Rule 2</strong>
</span></span><ul>
<li><span data-ttu-id="0ede2-235">מקור מימון 3:‏ 250.00 (= ‎750.00 – 50.00 – 450.00)</span><span class="sxs-lookup"><span data-stu-id="0ede2-235">Funding source 3: 250.00 (= 750.00 – 50.00 – 450.00)</span></span></li>
</ul><span data-ttu-id="0ede2-236">
<strong>כלל 3</strong>
</span><span class="sxs-lookup"><span data-stu-id="0ede2-236">
<strong>Rule 3</strong>
</span></span><ul>
<li><span data-ttu-id="0ede2-237">מקור מימון 1:‏ 3,850.00 (= ‎5,000.00 – 450.00 – 450.00 – 250.00)</span><span class="sxs-lookup"><span data-stu-id="0ede2-237">Funding source 1: 3,850.00 (= 5,000.00 – 450.00 – 450.00 – 250.00)</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0ede2-238">סך הכספים המחולקים לכל מקור מימון</span><span class="sxs-lookup"><span data-stu-id="0ede2-238">Total funds that are distributed for each funding source</span></span></td>
<td><ul>
<li><span data-ttu-id="0ede2-239">מקור מימון 1:‏ 3,850.00</span><span class="sxs-lookup"><span data-stu-id="0ede2-239">Funding source 1: 3,850.00</span></span></li>
<li><span data-ttu-id="0ede2-240">מקור מימון 2:‏ 500.00</span><span class="sxs-lookup"><span data-stu-id="0ede2-240">Funding source 2: 500.00</span></span></li>
<li><span data-ttu-id="0ede2-241">מקור מימון 3:‏ 750.00</span><span class="sxs-lookup"><span data-stu-id="0ede2-241">Funding source 3: 750.00</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

## <a name="billing-rules"></a><span data-ttu-id="0ede2-242">כללי חיוב</span><span class="sxs-lookup"><span data-stu-id="0ede2-242">Billing rules</span></span>
<span data-ttu-id="0ede2-243">בעת ניהול משא ומתן על חוזה פרוייקט עם לקוח, אתה מגדיר כיצד ומתי תוכל לחייב את הלקוח בגין עבודה בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-243">When you negotiate a project contract with a customer, you define how and when you can invoice the customer for work on a project.</span></span> <span data-ttu-id="0ede2-244">לאחר שתגדיר את חוזה הפרוייקט ואת הפרוייקט, תוכל להגדיר כללי חיוב עבור הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-244">After you set up the project contract and the project, you can set up billing rules for the project.</span></span> <span data-ttu-id="0ede2-245">כללי החיוב מבוססים על תנאי הפרוייקט המפורטים בחוזה הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-245">Billing rules are based on the project terms that are specified in the project contract.</span></span> <span data-ttu-id="0ede2-246">כללי החיוב שתוכל ליצור תלויים בתנאים של חוזה הפרוייקט ובסוג הפרוייקט, כגון זמן וחומר או מחיר קבוע, שתשייך לכלל החיוב.</span><span class="sxs-lookup"><span data-stu-id="0ede2-246">The billing rules that you can create depend on the terms of the project contract and the project type, such as Time and material or Fixed-price, that you associate with the billing rule.</span></span> <span data-ttu-id="0ede2-247">תוכל ליצור יותר מכלל חיוב אחד עבור חוזה פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-247">You can create more than one billing rule for a project contract.</span></span> <span data-ttu-id="0ede2-248">תוכל גם להקצות כלל חיוב לפרוייקטים מרובים משויכים לאותו חוזה פרוייקט ועם תנאי חיוב זהים.</span><span class="sxs-lookup"><span data-stu-id="0ede2-248">You can also assign a billing rule to multiple projects that are associated with the same project contract and have similar billing terms.</span></span> 

<span data-ttu-id="0ede2-249">תוכל להגדיר את הסוגים הבאים של כללי חיוב:</span><span class="sxs-lookup"><span data-stu-id="0ede2-249">You can set up the following types of billing rules:</span></span>

-   <span data-ttu-id="0ede2-250">**יחידת מסירה** – הפק חשבונית ללקוח בעת השלמת יחידת מסירה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-250">**Unit of delivery** – Invoice a customer when you complete a unit of delivery.</span></span> <span data-ttu-id="0ede2-251">אתה מגדיר את יחידות המסירה בחוזה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-251">You define the units of delivery in the contract.</span></span>
-   <span data-ttu-id="0ede2-252">**התקדמות** – הפק חשבונית ללקוח בעת השלמת אחוז מסוים בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-252">**Progress** – Invoice a customer when you complete a specified percentage of the project.</span></span> <span data-ttu-id="0ede2-253">באפשרותך להגדיר כלל חיוב לחישוב אוטומטי של אחוזי העבודה שהושלמה, או שתוכל לחשב ידנית את אחוז העבודה שהושלמה ואת הסכום לחיוב הלקוח.</span><span class="sxs-lookup"><span data-stu-id="0ede2-253">You can set up a billing rule to automatically calculate the percentage of work completed, or you can manually calculate the percentage of work completed and the amount to invoice the customer.</span></span>
-   <span data-ttu-id="0ede2-254">**אבן דרך** – הפק חשבונית ללקוח עבור הסכום המלא של אבן דרך בפרוייקט כשמושגת אבן הדרך.</span><span class="sxs-lookup"><span data-stu-id="0ede2-254">**Milestone** – Invoice a customer for the full amount of a project milestone when the milestone is reached.</span></span>
-   <span data-ttu-id="0ede2-255">**תשלום** – הפק חשבונית ללקוח עבור השירותים שלך בתוספת דמי ניהול, שהם בדרך כלל אחוז מעלות השירותים.</span><span class="sxs-lookup"><span data-stu-id="0ede2-255">**Fee** – Invoice a customer for your services plus a management fee, which is typically a percentage of the cost of services.</span></span>
-   <span data-ttu-id="0ede2-256">**זמן וחומר** – הפק חשבונית ללקוח עבור ערך הזמן והחומרים המשמשים לפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-256">**Time and material** – Invoice a customer for the value of time and materials that are used on a project.</span></span>

<span data-ttu-id="0ede2-257">עבור כל סוגי כללי החיוב, ניתן לציין אחוז שמירה שמנוכה מחשבוניות הלקוח עד שהפרוייקט יגיע לשלב מוסכם.</span><span class="sxs-lookup"><span data-stu-id="0ede2-257">For all types of billing rules, you can specify a retention percentage that is deducted from customer invoices until a project reaches an agreed-upon stage.</span></span> <span data-ttu-id="0ede2-258">אחוז שמירת התשלום מוגדר בחוזה הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-258">The payment retention percentage is specified in the project contract.</span></span> <span data-ttu-id="0ede2-259">הסכום מחושב על סמך הערך הכולל של השורות בחשבונית לקוח ומופחת ממנו.</span><span class="sxs-lookup"><span data-stu-id="0ede2-259">The amount is calculated based on, and subtracted from, the total value of the lines in a customer invoice.</span></span> 

<span data-ttu-id="0ede2-260">עבור כלל החיוב **זמן וחומר** וכלל החיוב **התקדמות**, תוכל להקצות קטגוריות ניתנות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="0ede2-260">For **Time and material** and **Progress** billing rules, you can assign chargeable categories.</span></span> <span data-ttu-id="0ede2-261">קטגוריות ניתנות לחיוב מציינות את העסקאות שצריכות להיכלל בחשבוניות הלקוח.</span><span class="sxs-lookup"><span data-stu-id="0ede2-261">Chargeable categories indicate the transactions that should be included in customer invoices.</span></span> 

<span data-ttu-id="0ede2-262">כשתהיה מוכן להפיק חשבונית ללקוח, הסכום בחשבונית עבור הפרוייקט מחושב בהתאם לכללי החיוב ונוצרת הצעה לחשבונית פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-262">When you are ready to invoice the customer, the amount to invoice for the project is calculated based on the billing rules, and a project invoice proposal is generated.</span></span> 

<span data-ttu-id="0ede2-263">הסעיפים הבאים מספקים דוגמאות המראות כיצד להגדיר ולנהל כללי חיוב עבור פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-263">The following sections provide examples that show how to set up and manage billing rules for a project.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-the-number-of-units-delivered"></a><span data-ttu-id="0ede2-264">דוגמה: יצירת כלל חיוב המבוסס על מספר היחידות שנמסרו</span><span class="sxs-lookup"><span data-stu-id="0ede2-264">Example: Create a billing rule that is based on the number of units delivered</span></span>

<span data-ttu-id="0ede2-265">הארגון שלך מתקשר בהסכם לספק בסך הכל חמישה מפגשי הדרכה לעובדי הלקוח בעלות של 10,000 לכל מפגש הדרכה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-265">Your organization enters into an agreement to provide a total of five training sessions to a customer’s employees at a cost of 10,000 per training session.</span></span> <span data-ttu-id="0ede2-266">אתה מפיק חשבונית ללקוח לאחר כל מפגש הדרכה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-266">You invoice the customer after each training session.</span></span> 

<span data-ttu-id="0ede2-267">בעת הגדרת כללי החיוב עבור החוזה, אתה משתמש בערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="0ede2-267">When you set up the billing rules for the contract, you use the following values:</span></span>

-   <span data-ttu-id="0ede2-268">יחידת המסירה הינה מפגש הדרכה אחד.</span><span class="sxs-lookup"><span data-stu-id="0ede2-268">The unit of delivery is one training session.</span></span>
-   <span data-ttu-id="0ede2-269">מחיר היחידה הוא 10,000 לכל מפגש הדרכה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-269">The unit price is 10,000 per training session.</span></span>
-   <span data-ttu-id="0ede2-270">מספר היחידות הכולל הוא חמישה מפגשי הדרכה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-270">The total number of units is five training sessions.</span></span>

<span data-ttu-id="0ede2-271">לאחר שתשלים מפגש הדרכה אחד, תוכל ליצור חשבונית בסך 10,000 עבור היחידה הראשונה שנמסרה ולשלוח את החשבונית ללקוח.</span><span class="sxs-lookup"><span data-stu-id="0ede2-271">When you have completed one training session, you can create an invoice for 10,000, for the first unit that was delivered, and send the invoice to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-manual-calculation"></a><span data-ttu-id="0ede2-272">דוגמה: יצירת כלל חיוב המבוסס על אחוז השלמת הפרוייקט המוגדר (חישוב ידני)</span><span class="sxs-lookup"><span data-stu-id="0ede2-272">Example: Create a billing rule that is based on a specified percentage of project completion (manual calculation)</span></span>

<span data-ttu-id="0ede2-273">הארגון שלך, חברה לייעוץ תוכנה, מתקשרת בהסכם עם לקוח לפיתוח חלק ממוצר שהלקוח מפתח.</span><span class="sxs-lookup"><span data-stu-id="0ede2-273">Your organization, a software consulting firm, enters into an agreement with a customer to develop part of a product that the customer is developing.</span></span> <span data-ttu-id="0ede2-274">הארגון שלך מסכים לספק את קוד התוכנה לתקופה של שישה חודשים.</span><span class="sxs-lookup"><span data-stu-id="0ede2-274">Your organization agrees to deliver the software code over a period of six months.</span></span> <span data-ttu-id="0ede2-275">הלקוח מסכים לשלם לארגון סכום כולל של 100,000 עבור העבודה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-275">The customer agrees to pay your organization a total of 100,000 for the work.</span></span> <span data-ttu-id="0ede2-276">אתה יוצר כלל חיוב כדי לחייב את הלקוח על בסיס אחוז העבודה שהושלמה בפרוייקט, כמפורט בחוזה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-276">You create a billing rule to invoice the customer based on the percentage of work that is completed on the project, as specified in the contract.</span></span>

-   <span data-ttu-id="0ede2-277">בסוף החודש הראשון אתה נפגש עם הלקוח כדי לקבוע את אחוז העבודה שהושלמה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-277">At the end of the first month, you meet with the customer to determine the percentage of work completed.</span></span> <span data-ttu-id="0ede2-278">לאחר שאתה והלקוח בדקתם את הפרוייקט, אתה מחליט שאחוז השלמת הפרוייקט הוא 15 אחוז.</span><span class="sxs-lookup"><span data-stu-id="0ede2-278">After you and the customer review the project, you decide that the project is 15 percent completed.</span></span>
-   <span data-ttu-id="0ede2-279">אתה יוצר חשבונית עבור 15,000 (15 אחוזים של 100,000) ושולח אותה ללקוח.</span><span class="sxs-lookup"><span data-stu-id="0ede2-279">You create an invoice for 15,000 (15 percent of 100,000) and send it to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-automatic-calculation"></a><span data-ttu-id="0ede2-280">דוגמה: יצירת כלל חיוב המבוסס על אחוז השלמת הפרוייקט המוגדר (חישוב אוטומטי)</span><span class="sxs-lookup"><span data-stu-id="0ede2-280">Example: Create a billing rule that is based on a specified percentage of project completion (automatic calculation)</span></span>

<span data-ttu-id="0ede2-281">הארגון שלך, חברה לפיתוח תוכנה, מסכים לפתח חבילת תוכנות שכר ללקוח תמורת 30,000.</span><span class="sxs-lookup"><span data-stu-id="0ede2-281">Your organization, a software development firm, agrees to develop a payroll accounting package for a customer for 30,000.</span></span> <span data-ttu-id="0ede2-282">הלקוח מסכים לשלם לארגון בהתאם לאחוז העבודה שהושלמה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-282">The customer agrees to pay your organization based on the percentage of work completed.</span></span> <span data-ttu-id="0ede2-283">אתה מעריך שעלויות הפרוייקט הן 20,000.</span><span class="sxs-lookup"><span data-stu-id="0ede2-283">You estimate that the project costs are 20,000.</span></span> <span data-ttu-id="0ede2-284">חוזה הפרוייקט מציין את קטגוריות העבודה שבהן אתה משתמש בתהליך החיוב.</span><span class="sxs-lookup"><span data-stu-id="0ede2-284">The project contract specifies the categories of work that you use in the billing process.</span></span> <span data-ttu-id="0ede2-285">אתה מגדיר כללי חיוב המחשבים אוטומטית את סכומי החשבונית עבור אחוז העבודה שהושלמה בכל קטגוריה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-285">You set up billing rules that automatically calculate the invoice amounts for the percentage of work that is completed for each category.</span></span> <span data-ttu-id="0ede2-286">הגדרת תקציב לכל קטגוריה:</span><span class="sxs-lookup"><span data-stu-id="0ede2-286">You set up a budget for each category:</span></span>

-   <span data-ttu-id="0ede2-287">**פיתוח** – עלות של 15,000 והכנסה של 20,000</span><span class="sxs-lookup"><span data-stu-id="0ede2-287">**Development** – Cost of 15,000 and revenue of 20,000</span></span>
-   <span data-ttu-id="0ede2-288">**התקנה** – עלות של 5,000 והכנסה של 10,000</span><span class="sxs-lookup"><span data-stu-id="0ede2-288">**Installation** – Cost of 5,000 and revenue of 10,000</span></span>

<span data-ttu-id="0ede2-289">בעת יצירת חשבונית ללקוח בפעם הראשונה, סכום החשבונית מחושב באופן אוטומטי בהתאם למידע הבא:</span><span class="sxs-lookup"><span data-stu-id="0ede2-289">When you create a customer invoice for the first time, the invoice amount is automatically calculated based on the following information:</span></span>

-   <span data-ttu-id="0ede2-290">לאחר חודש, העובד בפרוייקט מגיש גליון זמנים לפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-290">After a month, the worker on the project submits a timesheet for the project.</span></span> <span data-ttu-id="0ede2-291">עלות שעות העובד היא 5,000 לפיתוח ו- 1,000 להתקנה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-291">The cost of the worker’s hours is 5,000 for development and 1,000 for installation.</span></span> <span data-ttu-id="0ede2-292">עבודות הפיתוח הושלמו ב- 33% (5,000 עלות בפועל/15,000 עלות תקציב), ועבודות ההתקנה הושלמו ב- 20% (1,000 עלויות בפועל/5,000 עלות תקציב).</span><span class="sxs-lookup"><span data-stu-id="0ede2-292">The development work is 33 percent completed (5,000 actual cost/15,000 budget cost), and the installation work is 20 percent completed (1,000 actual cost/5,000 budget cost).</span></span>
-   <span data-ttu-id="0ede2-293">סכום החשבונית של 8,667 מחושב אוטומטית (33 אחוזים מ- 20,000 + 20 אחוזים מ- 10,000).</span><span class="sxs-lookup"><span data-stu-id="0ede2-293">The invoice amount of 8,667 is automatically calculated (33 percent of 20,000 + 20 percent of 10,000).</span></span>
-   <span data-ttu-id="0ede2-294">אתה יוצר חשבונית עבור 8,667 ושולח אותה ללקוח.</span><span class="sxs-lookup"><span data-stu-id="0ede2-294">You create an invoice for 8,667 and send it to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-agreed-upon-milestones"></a><span data-ttu-id="0ede2-295">דוגמה: יצירת כלל חיוב המבוסס על אבני דרך מוסכמות</span><span class="sxs-lookup"><span data-stu-id="0ede2-295">Example: Create a billing rule that is based on agreed-upon milestones</span></span>

<span data-ttu-id="0ede2-296">הארגון שלך, חברה לייעוץ אסטרטגי, מסכים לערוך חקר שוק עבור מוצר צריכה שהלקוח מתכנן למכור.</span><span class="sxs-lookup"><span data-stu-id="0ede2-296">Your organization, a management consulting firm, agrees to conduct market research for a consumer product that the customer plans to sell.</span></span> <span data-ttu-id="0ede2-297">הלקוח מסכים להשתמש בשירותים שלך לתקופה של שלושה חודשים, החל מחודש מרץ, ומסכים לשלם לארגון 50,000.</span><span class="sxs-lookup"><span data-stu-id="0ede2-297">The customer agrees to use your services for a period of three months, starting in March, and agrees to pay your organization 50,000.</span></span> <span data-ttu-id="0ede2-298">לפרוייקט יש שלוש אבני דרך:</span><span class="sxs-lookup"><span data-stu-id="0ede2-298">The project has three milestones:</span></span>

-   <span data-ttu-id="0ede2-299">ציון דרך 1: איסוף נתוני צרכנים – 31 במרץ</span><span class="sxs-lookup"><span data-stu-id="0ede2-299">Milestone 1: Collect consumer data – March 31</span></span>
-   <span data-ttu-id="0ede2-300">ציון דרך 2: ניתוח נתוני הצרכנים – 30 באפריל</span><span class="sxs-lookup"><span data-stu-id="0ede2-300">Milestone 2: Analyze consumer data – April 30</span></span>
-   <span data-ttu-id="0ede2-301">ציון דרך 3: הצגת הצעת כדאיות למוצר – 31 במאי</span><span class="sxs-lookup"><span data-stu-id="0ede2-301">Milestone 3: Present a product viability proposal – May 31</span></span>

<span data-ttu-id="0ede2-302">הלקוח מסכים לשלם לארגון 10,000 עבור אבן הדרך הראשונה, 20,000 עבור אבן הדרך השנייה ו- 20,000 עבור אבן הדרך השלישית.</span><span class="sxs-lookup"><span data-stu-id="0ede2-302">The customer agrees to pay your organization 10,000 for the first milestone, 20,000 for the second milestone, and 20,000 for the third milestone.</span></span> 

<span data-ttu-id="0ede2-303">בעת הגדרת חוזה הפרוייקט, אתה מסכים לחייב את הלקוח בהתאם לאבן הדרך שהושלמה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-303">When you set up the project contract, you agree to bill the customer based on the milestone that has been completed.</span></span> <span data-ttu-id="0ede2-304">הגדרת כלל החיוב כוללת את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="0ede2-304">The billing rule setup includes the following steps:</span></span>

-   <span data-ttu-id="0ede2-305">הגדר את אבני הדרך של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-305">Define the project milestones.</span></span>
-   <span data-ttu-id="0ede2-306">הגדר את הסכום לחיוב הלקוח לאחר השלמת כל אבן דרך.</span><span class="sxs-lookup"><span data-stu-id="0ede2-306">Define the amount to invoice the customer when each milestone is completed.</span></span>

<span data-ttu-id="0ede2-307">בעת השלמת אבן הדרך הראשונה ב- 31 במרץ, אתה מסמן את אבן הדרך כהושלמה ולאחר מכן יוצר חשבונית עבור 10,000 ושולח אותה ללקוח.</span><span class="sxs-lookup"><span data-stu-id="0ede2-307">When the first milestone is completed on March 31, you mark the milestone as completed, and then create an invoice for 10,000 and send it to the customer.</span></span> <span data-ttu-id="0ede2-308">אינך יכול ליצור חשבונית עבור אבן דרך עד שסימנת את אבן הדרך כהושלמה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-308">You can’t create an invoice for a milestone until you have marked the milestone as completed.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-services-plus-a-management-fee"></a><span data-ttu-id="0ede2-309">דוגמה: יצירת כלל חיוב המבוסס על שירותים בתוספת דמי ניהול</span><span class="sxs-lookup"><span data-stu-id="0ede2-309">Example: Create a billing rule that is based on services plus a management fee</span></span>

<span data-ttu-id="0ede2-310">הארגון שלך, חברה לייעוץ אסטרטגי, מסכים לבצע מחקר שוק כדי להעריך את כדאיות המוצר שהלקוח, חברה קמעונאית, מפתח.</span><span class="sxs-lookup"><span data-stu-id="0ede2-310">Your organization, a management consulting firm, agrees to conduct market research to evaluate the viability of a product that the customer, a retail company, is developing.</span></span> <span data-ttu-id="0ede2-311">בתנאי ההסכם נקבע כי תספק את שירותיהם של שלושת יועצי האסטרטגיה המובילים שלך, שיבצעו את המחקר על בסיס זמן וחומרים.</span><span class="sxs-lookup"><span data-stu-id="0ede2-311">The terms of the agreement specify that you will provide the services of your top three management consultants, who will conduct the research on a time-and-materials basis.</span></span> <span data-ttu-id="0ede2-312">הלקוח מסכים לשלם 100 לשעה, בתוספת דמי ניהול של 10 אחוזים עבור שעות הייעוץ שמחויבות לפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-312">The customer agrees to pay 100 per hour, plus a 10 percent management fee for the consulting hours that are charged to the project.</span></span> 

<span data-ttu-id="0ede2-313">בעת הגדרת חוזה הפרוייקט, צור כלל חיוב כדי להוסיף דמי ניהול של 10 אחוז לשעות הייעוץ שמחויבות בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-313">When you set up the project contract, create a billing rule to add a 10 percent management fee to the consulting hours that are charged to the project.</span></span> 

<span data-ttu-id="0ede2-314">בעת יצירת חשבונית עבור הלקוח, הלקוח מחויב בדמי ניהול של 10 אחוז בתוספת עלות שעות הייעוץ.</span><span class="sxs-lookup"><span data-stu-id="0ede2-314">When you create an invoice for the customer, the customer is billed a 10 percent management fee plus the cost of the consulting hours.</span></span> <span data-ttu-id="0ede2-315">לדוגמה, אם שלושת היועצים עבדו בסך הכל 200 שעות על הפרוייקט, נוצרת חשבונית עבור 22,000 על סמך החישוב הבא:</span><span class="sxs-lookup"><span data-stu-id="0ede2-315">For example, if the three consultants worked a total of 200 hours on the project, an invoice for 22,000 is created based on the following calculation:</span></span>

-   <span data-ttu-id="0ede2-316">200 שעות ב- 100 לשעה = 20,000</span><span class="sxs-lookup"><span data-stu-id="0ede2-316">200 hours at 100 per hour = 20,000</span></span>
-   <span data-ttu-id="0ede2-317">דמי ניהול של 10 אחוזים = 2,000</span><span class="sxs-lookup"><span data-stu-id="0ede2-317">10 percent management fee = 2,000</span></span>
-   <span data-ttu-id="0ede2-318">סכום חשבונית כולל = 22,000</span><span class="sxs-lookup"><span data-stu-id="0ede2-318">Total invoice amount = 22,000</span></span>

<span data-ttu-id="0ede2-319">אם עמלות חייבות במס ללקוח, ואתה בוחר קבוצת מס מכירה בחוזה הפרוייקט, קבוצת מס מכירה מוזנת באופן אוטומטי בכלל חיוב בגין עמלות.</span><span class="sxs-lookup"><span data-stu-id="0ede2-319">If fees are taxable to a customer, and you select a sales tax group in the project contract, the sales tax group is automatically entered in a billing rule for fees.</span></span>

### <a name="example-create-a-billing-rule-for-the-value-of-time-and-materials"></a><span data-ttu-id="0ede2-320">דוגמה: יצירת כלל חיוב עבור ערך הזמן והחומרים</span><span class="sxs-lookup"><span data-stu-id="0ede2-320">Example: Create a billing rule for the value of time and materials</span></span>

<span data-ttu-id="0ede2-321">הארגון שלך, חברה לייעוץ תוכנה, מסכים לספק חמישה יועצים טכנים שיעבדו בפרוייקט פיתוח תוכנה עבור לקוח בחצי השנה הקרובה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-321">Your organization, a software consulting firm, agrees to provide five technical consultants to work on a software development project for a customer for the next six months.</span></span> <span data-ttu-id="0ede2-322">הלקוח מסכים לשלם 150 עבור כל שעת ייעוץ בתוספת עלות הציוד המשרדי.</span><span class="sxs-lookup"><span data-stu-id="0ede2-322">The customer agrees to pay 150 for each consulting hour, plus the cost of office supplies.</span></span> <span data-ttu-id="0ede2-323">הארגון שלך שולח חשבונית ללקוח בסוף כל חודש.</span><span class="sxs-lookup"><span data-stu-id="0ede2-323">Your organization sends an invoice to the customer at the end of each month.</span></span> 

<span data-ttu-id="0ede2-324">כאשר אתה מגדיר את חוזה הפרוייקט, אתה מסכים לחייב את הלקוח בכל חודש בגין זמן וחומרים בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-324">When you set up the project contract, you agree to bill the customer each month for time and materials on the project.</span></span> <span data-ttu-id="0ede2-325">אתה יוצר כלל חיוב הכולל את המידע הבא:</span><span class="sxs-lookup"><span data-stu-id="0ede2-325">You create a billing rule that includes the following information:</span></span>

-   <span data-ttu-id="0ede2-326">תקופת החוזה היא שישה חודשים.</span><span class="sxs-lookup"><span data-stu-id="0ede2-326">The contract period is six months.</span></span>
-   <span data-ttu-id="0ede2-327">זמן הייעוץ מחושב בתעריף של 150 לשעה.</span><span class="sxs-lookup"><span data-stu-id="0ede2-327">Consulting time is calculated at a rate of 150 per hour.</span></span>
-   <span data-ttu-id="0ede2-328">הציוד המשרדי מחויב בעלות, והעלות הכוללת של הפרוייקט לא תעלה על 10,000.</span><span class="sxs-lookup"><span data-stu-id="0ede2-328">Office supplies are invoiced at cost, and the total cost for the project must not exceed 10,000.</span></span>
-   <span data-ttu-id="0ede2-329">אתה יוצר חשבונית לקוח בסוף כל חודש קלנדרי במהלך הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-329">You create a customer invoice at the end of each calendar month during the project.</span></span>

<span data-ttu-id="0ede2-330">במהלך החודש הראשון, נרשמו בסך הכל 800 שעות על ידי היועצים בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="0ede2-330">During the first month, a total of 800 hours are recorded by the consultants on the project.</span></span> <span data-ttu-id="0ede2-331">עלות הציוד המשרדי שמחויב בפרוייקט היא 2,000.</span><span class="sxs-lookup"><span data-stu-id="0ede2-331">The cost of office supplies that are charged to the project is 2,000.</span></span> <span data-ttu-id="0ede2-332">לכן, בסוף החודש אתה יוצר חשבונית עבור 122,000 המחושבת כ- 800 שעות בתעריף 150 לשעה, בתוספת 2,000 עבור ציוד משרדי.</span><span class="sxs-lookup"><span data-stu-id="0ede2-332">Therefore, at the end of the month, you create an invoice for 122,000, which is calculated as 800 hours at 150 per hour, plus 2,000 for office supplies.</span></span>



