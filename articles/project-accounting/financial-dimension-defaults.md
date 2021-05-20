---
title: ברירות מחדל של ממד פיננסי
description: נושא זה מספק מידע על אופן הגדרת ברירות מחדל של ממד פיננסי.
author: sigitac
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 0a76447bb1a81a7157fccc0cd58eddd1eb5995de
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2021
ms.locfileid: "5950130"
---
# <a name="financial-dimension-defaults"></a><span data-ttu-id="57ef2-103">ברירות מחדל של ממד פיננסי</span><span class="sxs-lookup"><span data-stu-id="57ef2-103">Financial dimension defaults</span></span>

<span data-ttu-id="57ef2-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="57ef2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="57ef2-105">Dynamics 365 Project Operations משתמש במסגרת [ממדים פיננסיים](/dynamics365/finance/general-ledger/financial-dimensions) ב- Dynamics 365 Finance כדי לספק תובנות נוספות על עסקאות ספר משנה וספר ראשי של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="57ef2-105">Dynamics 365 Project Operations uses the [Financial dimensions](/dynamics365/finance/general-ledger/financial-dimensions) framework in Dynamics 365 Finance to provide additional insights on project subledger and general ledger transactions.</span></span>

<span data-ttu-id="57ef2-106">ניתן להגדיר את ברירת המחדל של ממדים פיננסיים לפי לקוח, מקור מימון פרויקט, אבן דרך, סעיף חוזה פרויקט או פרויקט.</span><span class="sxs-lookup"><span data-stu-id="57ef2-106">Default financial dimensions can be set on a customer, project funding source, milestone, project contract line, or project.</span></span>

## <a name="define-default-financial-dimensions-for-a-customer"></a><span data-ttu-id="57ef2-107">הגדרת ממדים פינסיים ברירת מחדל עבור לקוח</span><span class="sxs-lookup"><span data-stu-id="57ef2-107">Define default financial dimensions for a customer</span></span>

<span data-ttu-id="57ef2-108">ברירות המחדל של ממד פיננסי ללקוח מוגדרות Finance.</span><span class="sxs-lookup"><span data-stu-id="57ef2-108">Customer dimension defaults are specified in Finance.</span></span> <span data-ttu-id="57ef2-109">להגדרת ברירות מחדל של מימדים יש להשלים את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="57ef2-109">Complete the following steps to set dimension defaults.</span></span>

1. <span data-ttu-id="57ef2-110">עבור אל **חשבונות חייבים** > **לקוחות** > **כל הלקוחות**.</span><span class="sxs-lookup"><span data-stu-id="57ef2-110">Go to **Accounts receivable** > **Customers** > **All customers**.</span></span>
2. <span data-ttu-id="57ef2-111">בדף **לקוחות**, בכרטיסיה **ממדים פיננסיים**, הגדר את ערכי המימד הכספי עבור לקוח ספציפי.</span><span class="sxs-lookup"><span data-stu-id="57ef2-111">On the **Customers** page, on the **Financial dimensions** tab, set the financial dimension values for specific customer.</span></span>

## <a name="define-default-financial-dimensions-for-project-contracts"></a><span data-ttu-id="57ef2-112">הגדרת ממדים פינסיים ברירת מחדל עבור חוזי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="57ef2-112">Define default financial dimensions for project contracts</span></span>

<span data-ttu-id="57ef2-113">חוזי הפרויקט נוצרים ומתוחזקים ב-Common Data Service ‏(CDS).</span><span class="sxs-lookup"><span data-stu-id="57ef2-113">Project contracts are created and maintained in Common Data Service (CDS).</span></span> <span data-ttu-id="57ef2-114">תכונות חשבונאות עבור חוזי פרויקט מוגדרים במודול **ניהול פרויקטים וחשבונאות** ב-Finance.</span><span class="sxs-lookup"><span data-stu-id="57ef2-114">Accounting attributes for project contracts are set in the **Project management and accounting** module in Finance.</span></span>

### <a name="set-financial-dimensions-for-a-project-funding-source"></a><span data-ttu-id="57ef2-115">הגדרת ממדים פיננסיים עבור מקור מימון פרויקטים</span><span class="sxs-lookup"><span data-stu-id="57ef2-115">Set financial dimensions for a project funding source</span></span>

1. <span data-ttu-id="57ef2-116">עבור אל **ניהול פרויקטים וחשבונאות** > **פרויקטים** > **חוזי פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="57ef2-116">Go to **Project management and accounting** > **Projects** > **Project contracts**.</span></span>
2. <span data-ttu-id="57ef2-117">בחר את הרשומה שברצונך לעדכן ובכרטיסיה **חוזה פרויקט** בחר **הצג חשבונאות ברירת מחדל**.</span><span class="sxs-lookup"><span data-stu-id="57ef2-117">Select the record you want to update, and on the **Project contract** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="57ef2-118">הרחב את **מידע קשור** ובחר את הכרטיסיה **מקורות מימון**.</span><span class="sxs-lookup"><span data-stu-id="57ef2-118">Expand **Related information** and select the **Funding sources** tab.</span></span>
4. <span data-ttu-id="57ef2-119">הגדרת ברירות המחדל של הממד פיננסי.</span><span class="sxs-lookup"><span data-stu-id="57ef2-119">Set the financial dimension defaults.</span></span> <span data-ttu-id="57ef2-120">שים לב שהממדים הפיננסים מוגדרים כברירת המחדל מחשבון הלקוח.</span><span class="sxs-lookup"><span data-stu-id="57ef2-120">Notice that the financial dimensions default from the customer account.</span></span>

### <a name="set-financial-dimensions-for-a-project-contract-line"></a><span data-ttu-id="57ef2-121">הגדרת ממדים פיננסיים עבור סעיף חוזה פרוייקט</span><span class="sxs-lookup"><span data-stu-id="57ef2-121">Set financial dimensions for a project contract line</span></span>

1. <span data-ttu-id="57ef2-122">עבור אל **ניהול פרויקטים וחשבונאות** > **פרויקטים** > **חוזי פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="57ef2-122">Go to **Project management and accounting** > **Projects** > **Project contracts**.</span></span>
2. <span data-ttu-id="57ef2-123">בחר את הרשומה שברצונך לעדכן ובכרטיסיה **חוזה פרויקט** בחר **הצג חשבונאות ברירת מחדל**.</span><span class="sxs-lookup"><span data-stu-id="57ef2-123">Select the record you want to update and on the **Project contract** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="57ef2-124">הרחב את **מידע קשור** ובחר את הכרטיסיה **סעיפי חוזה**.</span><span class="sxs-lookup"><span data-stu-id="57ef2-124">Expand **Related information** and select the **Contract lines** tab.</span></span>
4. <span data-ttu-id="57ef2-125">הגדרת ברירות המחדל של הממד פיננסי.</span><span class="sxs-lookup"><span data-stu-id="57ef2-125">Set the financial dimension defaults.</span></span> <span data-ttu-id="57ef2-126">ברירות המחדל של המימד הכספי ישימות וניתן להשתמש בהן רק עם סעיפי חוזה של מחיר קבוע (אבן דרך).</span><span class="sxs-lookup"><span data-stu-id="57ef2-126">The financial dimension defaults are applicable and can be used only with Fixed price (milestone) contract lines.</span></span>

<span data-ttu-id="57ef2-127">ברירות מחדל אלה משמשות לעסקאות לחשבון ושורות חשבונית קשורות של פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="57ef2-127">These defaults are used on related project on-account transactions and invoice lines.</span></span>

## <a name="define-default-financial-dimensions-for-projects"></a><span data-ttu-id="57ef2-128">הגדרת ממדים פינסיים ברירת מחדל עבור פרוייקטים</span><span class="sxs-lookup"><span data-stu-id="57ef2-128">Define default financial dimensions for projects</span></span>

<span data-ttu-id="57ef2-129">הפרויקט נוצרים ומתוחזקים ב-CDS.</span><span class="sxs-lookup"><span data-stu-id="57ef2-129">Projects are created and maintained in CDS.</span></span> <span data-ttu-id="57ef2-130">תכונות חשבונאות עבור פרויקטים מוגדרים במודול **ניהול פרויקטים וחשבונאות** ב-Finance.</span><span class="sxs-lookup"><span data-stu-id="57ef2-130">Accounting attributes for projects are set in the **Project management and accounting** module in Finance.</span></span>

1. <span data-ttu-id="57ef2-131">עבור אל **ניהול פרוייקטים וחשבונאות** > **פרוייקטים** > **כל הפרוייקטים**.</span><span class="sxs-lookup"><span data-stu-id="57ef2-131">Go to **Project management and accounting** > **Projects** > **All projects**.</span></span>
2. <span data-ttu-id="57ef2-132">בחר את הרשומה שברצונך לעדכן ובכרטיסיה **פרוייקט** בחר **הצג חשבונאות ברירת מחדל**.</span><span class="sxs-lookup"><span data-stu-id="57ef2-132">Select the record that you want to update and on the **Project** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="57ef2-133">הרחב את **מידע קשור** ובחר את הכרטיסיה **הגדרה**.</span><span class="sxs-lookup"><span data-stu-id="57ef2-133">Expand **Related information** and select the **Setup** tab.</span></span>
4. <span data-ttu-id="57ef2-134">הגדרת ברירות המחדל של הממד פיננסי.</span><span class="sxs-lookup"><span data-stu-id="57ef2-134">Set the financial dimension defaults.</span></span> <span data-ttu-id="57ef2-135">שים לב שהממדים הפיננסים מוגדרים כברירת המחדל מתיק הלקוח.</span><span class="sxs-lookup"><span data-stu-id="57ef2-135">Notice that financial dimensions default from the customer account.</span></span> <span data-ttu-id="57ef2-136">אם הפרויקט משויך לסעיף חוזה עם מספר לקוחות חוזה פרויקט, הלקוח הראשי משמש להגדרת ברירת המחדל של הממדים הפיננסיים.</span><span class="sxs-lookup"><span data-stu-id="57ef2-136">If the project is associated with a contract line with multiple project contract customers, the primary customer is used to default financial dimensions.</span></span>

<span data-ttu-id="57ef2-137">ממדים פיננסיים המוגדרים כברירת מחדל של הפרויקט משמשים להגדרת ברירות מחדל של יומן עבור עסקאות זמן, הוצאות ועמלות ב **יומן שילוב של Project Pperations** ובשורות חשבוניות פרויקטים קשורות.</span><span class="sxs-lookup"><span data-stu-id="57ef2-137">Project default financial dimensions are used to set journal line defaults for time, expense, and fee transactions in the **Project Operations Integration Journal** and on related project invoice lines.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]