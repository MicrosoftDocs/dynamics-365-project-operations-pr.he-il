---
title: הגדרת Project Service Automation
description: שלבים להגדרת Project Service
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: ec5381f91b1fe5198bd93ac8d6015b1fea38738d
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5146934"
---
# <a name="configure-project-service"></a><span data-ttu-id="1afd9-103">הגדרת Project Service</span><span class="sxs-lookup"><span data-stu-id="1afd9-103">Configure Project Service</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="1afd9-104">לפני שתוכל להשתמש ביכולות האוטומציה של [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] ב- [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] כדי לנהל תיקי לקוחות, פרוייקטים ומשאבים, עליך להשלים מספר שלבים של קביעת תצורה כדי להבטיח שהפתרון של [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] תואם לצרכי הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="1afd9-104">Before you can use the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] automation capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] to manage your accounts, projects, and resources, you need to complete a few configuration steps to ensure the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] solution matches your organization’s needs.</span></span> <span data-ttu-id="1afd9-105">השלבים האלה כוללים:</span><span class="sxs-lookup"><span data-stu-id="1afd9-105">These steps include:</span></span>  
  
-   <span data-ttu-id="1afd9-106">[הגדרת יחידות זמן](../psa/set-up-time-units.md).</span><span class="sxs-lookup"><span data-stu-id="1afd9-106">[Set up time units](../psa/set-up-time-units.md).</span></span> <span data-ttu-id="1afd9-107">הגדר את יחידות הזמן בקטלוג המוצרים שבהן תשתמש כבסיס לתזמון וחיוב הפרוייקטים שלך.</span><span class="sxs-lookup"><span data-stu-id="1afd9-107">Configure the time units in the product catalog that you’ll use as a base for scheduling and billing your projects.</span></span>  
  
-   <span data-ttu-id="1afd9-108">[הגדרת מטבעות ושערי חליפין](../psa/set-up-currencies-exchange-rates.md).</span><span class="sxs-lookup"><span data-stu-id="1afd9-108">[Set up currencies and exchange rates](../psa/set-up-currencies-exchange-rates.md).</span></span> <span data-ttu-id="1afd9-109">הגדר את המטבעות לשימוש עבור הפרוייקטים שלך.</span><span class="sxs-lookup"><span data-stu-id="1afd9-109">Set up the currencies to use for your projects.</span></span>  
  
-   <span data-ttu-id="1afd9-110">[יצירת יחידות ארגוניות](../psa/create-organizational-units.md).</span><span class="sxs-lookup"><span data-stu-id="1afd9-110">[Create organizational units](../psa/create-organizational-units.md).</span></span> <span data-ttu-id="1afd9-111">הגדר את הקבוצות שהחברה שלך משתמשת בהן כדי לחלק את עסקיה, בין אם לפי אזור גיאוגרפי, פונקציה עסקית או חלוקה לוגית אחרת.</span><span class="sxs-lookup"><span data-stu-id="1afd9-111">Set up the groups that your company uses to divide its business, whether by geography, business function, or other logical division.</span></span>  
  
-   <span data-ttu-id="1afd9-112">[הגדרת תדירויות חשבוניות](../psa/set-up-invoice-frequencies.md).</span><span class="sxs-lookup"><span data-stu-id="1afd9-112">[Set up invoice frequencies](../psa/set-up-invoice-frequencies.md).</span></span> <span data-ttu-id="1afd9-113">הגדר תקופות זמן שבהן ברצונך להשתמש לחיוב הלקוחות שלך.</span><span class="sxs-lookup"><span data-stu-id="1afd9-113">Set up time periods that you want to use for billing your clients.</span></span>  
  
-   <span data-ttu-id="1afd9-114">[הגדרת קטגוריות עסקאות](../psa/configure-transaction-categories.md).</span><span class="sxs-lookup"><span data-stu-id="1afd9-114">[Configure transaction categories](../psa/configure-transaction-categories.md).</span></span> <span data-ttu-id="1afd9-115">הגדר קטגוריות עסקאות שבהן היועצים שלך יכולים לחייב את ההוצאות שניתנות לחיוב והוצאות שלא ניתנות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="1afd9-115">Set up transaction categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="1afd9-116">[הגדרת קטגוריות הוצאות](../psa/configure-expense-categories.md).</span><span class="sxs-lookup"><span data-stu-id="1afd9-116">[Configure expense categories](../psa/configure-expense-categories.md).</span></span> <span data-ttu-id="1afd9-117">הגדר את הקטגוריות שבהן היועצים שלך יכולים לחייב את ההוצאות שניתנות לחיוב והוצאות שלא ניתנות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="1afd9-117">Set up the categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="1afd9-118">[יצירת פריטי קטלוג המוצרים](../psa/create-product-catalog-items.md).</span><span class="sxs-lookup"><span data-stu-id="1afd9-118">[Create product catalog items](../psa/create-product-catalog-items.md).</span></span> <span data-ttu-id="1afd9-119">הוסף את המוצרים שאתה מוכר, כגון רישיונות תוכנה, לקטלוג המוצרים.</span><span class="sxs-lookup"><span data-stu-id="1afd9-119">Add the products you sell, such as software licenses, to the product catalog.</span></span>  
  
-   <span data-ttu-id="1afd9-120">[יצירת מחירון](../psa/create-price-list.md).</span><span class="sxs-lookup"><span data-stu-id="1afd9-120">[Create a price list](../psa/create-price-list.md).</span></span> <span data-ttu-id="1afd9-121">הגדר מחירונים שונים, בהתאם למידה שבה ברצונך לחייב את הלקוחות שלך עבור כל תפקיד שדורש הפרוייקט שלהם.</span><span class="sxs-lookup"><span data-stu-id="1afd9-121">Configure different price lists, depending on how much you want to charge your clients for each role their project requires.</span></span>  
  
-   <span data-ttu-id="1afd9-122">[הגדרת משאבים](../psa/set-up-resources.md).</span><span class="sxs-lookup"><span data-stu-id="1afd9-122">[Set up resources](../psa/set-up-resources.md).</span></span> <span data-ttu-id="1afd9-123">הוסף את הכישורים, את המומחיות, את תפקידי המשאבים ומידע אחר לגבי המשאבים שתזדקק לו עבור הפרוייקטים שלך.</span><span class="sxs-lookup"><span data-stu-id="1afd9-123">Add the skills, proficiencies, resource roles, and other resource information that you’ll need for your projects.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="1afd9-124">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="1afd9-124">See Also</span></span>  
 <span data-ttu-id="1afd9-125">[מבט כולל על Project Service Automation](../psa/overview.md) </span><span class="sxs-lookup"><span data-stu-id="1afd9-125">[Overview of Project Service Automation](../psa/overview.md) </span></span>  
 <span data-ttu-id="1afd9-126">[הגדרת Project Service Automation](../psa/configure.md) </span><span class="sxs-lookup"><span data-stu-id="1afd9-126">[Configure Project Service Automation](../psa/configure.md) </span></span>  
 <span data-ttu-id="1afd9-127">[מדריך למנהלי תיקי לקוחות](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="1afd9-127">[Account Manager Guide](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="1afd9-128">[מדריך למנהל פרוייקט](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="1afd9-128">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 <span data-ttu-id="1afd9-129">[מדריך למנהל משאבים](../psa/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="1afd9-129">[Resource Manager Guide](../psa/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="1afd9-130">‏‫מדריך בנושאי זמן, הוצאות ושיתוף פעולה</span><span class="sxs-lookup"><span data-stu-id="1afd9-130">Time, Expense, and Collaboration Guid</span></span>](../psa/time-expense-collaboration-guide.md)
