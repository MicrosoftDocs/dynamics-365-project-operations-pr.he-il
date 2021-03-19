---
title: קביעת תצורה של שילוב Project Operations עבור כל ישות משפטית
description: נושא זה מספק מידע על הגדרת שילוב לפי ישות משפטית ב- Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/21/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ccdbdce6b7d006adc9be2b5f3573dd8e79dd2b8d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276979"
---
# <a name="configure-project-operations-integration-per-legal-entity"></a><span data-ttu-id="84176-103">קביעת תצורה של שילוב Project Operations עבור כל ישות משפטית</span><span class="sxs-lookup"><span data-stu-id="84176-103">Configure Project Operations integration per legal entity</span></span> 

<span data-ttu-id="84176-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="84176-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="84176-105">נושא זה מדריך אותך בשלבים הנדרשים להגדרה של Dynamics 365 Project Operations לכל ישות משפטית.</span><span class="sxs-lookup"><span data-stu-id="84176-105">This topic walks you through the steps required to configure Dynamics 365 Project Operations per legal entity.</span></span>

## <a name="enable-feature-keys-in-dynamics-365-finance"></a><span data-ttu-id="84176-106">הפעלת מפתחות של ישויות ב- Dynamics 365 Finance</span><span class="sxs-lookup"><span data-stu-id="84176-106">Enable feature keys in Dynamics 365 Finance</span></span>

<span data-ttu-id="84176-107">בצע את השלבים הבאים כדי להפעיל תכונות נדרשות.</span><span class="sxs-lookup"><span data-stu-id="84176-107">Complete the following steps to enable required features.</span></span>

1. <span data-ttu-id="84176-108">ב- Dynamics 365 Finance, עבור אל סביבת העבודה **ניהול ישויות**.</span><span class="sxs-lookup"><span data-stu-id="84176-108">In Dynamics 365 Finance, go to the **Feature Management** workspace.</span></span>
2. <span data-ttu-id="84176-109">ב **רשימת תכונות**, מצא והפעל את התכונות הבאות:</span><span class="sxs-lookup"><span data-stu-id="84176-109">In **Feature list**, find and enable the following features:</span></span>
  
    - <span data-ttu-id="84176-110">**הפעל מספר סעיפי חוזה לפרויקט**</span><span class="sxs-lookup"><span data-stu-id="84176-110">**Enable multiple contract lines for a project**</span></span>
    - <span data-ttu-id="84176-111">**הפעל את Project Operations ב- Dynamics 365 Customer Engagement**</span><span class="sxs-lookup"><span data-stu-id="84176-111">**Enable Project Operations on Dynamics 365 Customer Engagement**</span></span>

> [!NOTE]
> <span data-ttu-id="84176-112">אם אתה לא רואה את **מקשי התכונות** ברשימה, ודא שגרסת Finance שלך עומדת בדרישת הגרסה המינימלית (גרסת היישום 10.0.13 עם כל עדכוני האיכות שהוחלו ומעלה).</span><span class="sxs-lookup"><span data-stu-id="84176-112">If you don't see **Feature keys** listed, verify that your Finance version meets the minimum version requirement (application version 10.0.13 with all quality updates applied or higher).</span></span> <span data-ttu-id="84176-113">בחר **בדוק עדכונים** כדי לרענן את רשימת התכונות.</span><span class="sxs-lookup"><span data-stu-id="84176-113">Select **Check for updates** to refresh the feature list.</span></span>

## <a name="define-the-project-operations-deployment-scenario-for-a-legal-entity"></a><span data-ttu-id="84176-114">הגדר את תרחיש הפריסה ב- Project Operations עבור ישות משפטית</span><span class="sxs-lookup"><span data-stu-id="84176-114">Define the Project Operations deployment scenario for a legal entity</span></span>

<span data-ttu-id="84176-115">באפשרותך להפעיל את Project Operations ב- Dynamics 365 Customer Engagement ברמת הישות המשפטית.</span><span class="sxs-lookup"><span data-stu-id="84176-115">You can enable Project Operations on Dynamics 365 Customer Engagement on a legal entity level.</span></span> <span data-ttu-id="84176-116">יכולה להיות לך ישות משפטית אחת באמצעות Project Operations ב- Dynamics 365 Customer Engagement לתרחישים מבוססי משאבים/ללא מלאי.</span><span class="sxs-lookup"><span data-stu-id="84176-116">You can have one legal entity using Project Operations on Dynamics 365 Customer Engagement for resource/non-stocked based scenarios.</span></span> <span data-ttu-id="84176-117">באותה סביבה, יכולה להיות לך ישות משפטית אחרת המשתמשת ב- Project Operations לתרחישים בהזמנת מלאי/ייצור.</span><span class="sxs-lookup"><span data-stu-id="84176-117">In the same environment, you can have another legal entity using Project Operations for stocked/production order scenarios.</span></span>

1. <span data-ttu-id="84176-118">ב- Dynamics 365 Finance עבור אל **ניהול פרויקטים וחשבונאות** > **הגדרה** > **ניהול פרויקטים ופרמטרים חשבונאיים**.</span><span class="sxs-lookup"><span data-stu-id="84176-118">In Dynamics 365 Finance, go to **Project management and accounting** > **Setup** > **Global project management and accounting parameters**.</span></span>
2. <span data-ttu-id="84176-119">ברשימת הישויות המשפטיות הזמינות, בחר ישויות שבהן יש מספר סעיפי חוזה והתכונות של Project Operations ב- Dynamics 365 Customer Engagement פועלות.</span><span class="sxs-lookup"><span data-stu-id="84176-119">In the list of available legal entities, select entities where multiple contract lines and Project Operations on Dynamics 365 Customer Engagement features will be enabled.</span></span> <span data-ttu-id="84176-120">השאר את הישויות המשפטיות שישתמשו ב- Project Operations עבור תרחישים במלאי/הזמנת ייצור.</span><span class="sxs-lookup"><span data-stu-id="84176-120">Leave legal entities that will be using Project Operations for stocked/production order scenarios unselected.</span></span>

> [!NOTE]
> <span data-ttu-id="84176-121">ניתן לבחור ישות משפטית רק אם אין לה פרויקטים קיימים.</span><span class="sxs-lookup"><span data-stu-id="84176-121">A legal entity can be selected only if it doesn't have any existing projects.</span></span>

## <a name="configure-project-management-and-accounting-parameters"></a><span data-ttu-id="84176-122">הגדרה של ניהול פרויקטים ופרמטרים של חשבונאות</span><span class="sxs-lookup"><span data-stu-id="84176-122">Configure Project management and accounting parameters</span></span>

<span data-ttu-id="84176-123">כל ישות משפטית שמשתמשת ב- Project Operations ב- Dynamics 365 Customer Engagement צריכה קבוצה של פרמטרים המוגדרים כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="84176-123">Each legal entity using Project Operations on Dynamics 365 Customer Engagement needs a set of default parameters.</span></span> <span data-ttu-id="84176-124">פרמטרים אלה מוגדרים בכרטיסיה **Project Operations** בדף **ניהול פרויקטים ופרמטרים חשבונאיים**.</span><span class="sxs-lookup"><span data-stu-id="84176-124">These parameters are configured on the **Project Operations** tab on the **Project management and accounting parameters** page.</span></span> <span data-ttu-id="84176-125">הפרמטרים הם:</span><span class="sxs-lookup"><span data-stu-id="84176-125">The parameters are:</span></span>

  - <span data-ttu-id="84176-126">**ברירות מחדל של סוג חיוב**:‏ Project Operations משתמש בקבוצה קבועה של ברירות מחדל מסוג חיוב שיש למפות למאפייני השורות של Finance.</span><span class="sxs-lookup"><span data-stu-id="84176-126">**Billing type defaults**: Project Operations uses a fixed set of billing type defaults that must be mapped to line properties Finance.</span></span> <span data-ttu-id="84176-127">צור רשומה עבור כל סוג חיוב: **לא מוגדר**, **בתשלום**, **ללא חיוב**, **משלים** ו **לא זמין**.</span><span class="sxs-lookup"><span data-stu-id="84176-127">Create a record for each billing type: **Not specified**, **Chargeable**, **Non-chargeable**, **Complimentary**, and **Not available**.</span></span>
  - <span data-ttu-id="84176-128">**ברירות מחדל של קטגוריית הפרויקט**: בחר בקטגוריות הפרויקט המוגדרות כברירת מחדל לשימוש עבור כל סוג עסקה.</span><span class="sxs-lookup"><span data-stu-id="84176-128">**Project category defaults**: Select the default project categories to be used for each transaction type.</span></span> <span data-ttu-id="84176-129">ברירות מחדל אלה ישמשו ב- **כתב העת לשילוב Project Operations** ובהערכות שבהן לא מוגדרת קטגוריית עסקאות עבור הפרויקט בפועל.</span><span class="sxs-lookup"><span data-stu-id="84176-129">These defaults will be used in the **Project Operations Integration journal** and in estimates where no transaction category is specified for the project actual.</span></span>
  - <span data-ttu-id="84176-130">**תחזיות**: בחר במודל התחזית שישמש לאומדני זמן והוצאות.</span><span class="sxs-lookup"><span data-stu-id="84176-130">**Forecasts**: Select the forecast model to be used for time and expense estimates.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]