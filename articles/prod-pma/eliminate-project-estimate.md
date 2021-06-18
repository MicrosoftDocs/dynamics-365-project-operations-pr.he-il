---
title: ביטול הערכת פרוייקט
description: נושא זה מספק מידע על ביטול הערכת הפרויקט לאחר השלמתו.
author: Yowelle
ms.date: 05/26/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: a4ad06bef7ed66a626c6d2ad7ef01ba5b99d1c0f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006917"
---
# <a name="eliminate-a-project-estimate"></a><span data-ttu-id="87777-103">ביטול הערכת פרוייקט</span><span class="sxs-lookup"><span data-stu-id="87777-103">Eliminate a project estimate</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="87777-104">הערכות הפרוייקט מספקות את הראיה הפיננסית עבור העבודה המשוערת והמתוזמנת עבור בפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="87777-104">Project estimates provide the financial view for work that is estimated and scheduled for a project.</span></span> <span data-ttu-id="87777-105">כדי לעבוד עם הערכות לפרויקט, עליך לצרף את הפרויקט לפרויקט הערכה.</span><span class="sxs-lookup"><span data-stu-id="87777-105">To work with estimates for a project, you must attach the project to an estimate project.</span></span> <span data-ttu-id="87777-106">פרויקט הערכה מבוסס תמיד על פרויקט קיים, אולם פרויקטים מרובים יכולים להתייחס לפרויקט הערכה יחיד.</span><span class="sxs-lookup"><span data-stu-id="87777-106">An estimate project is always based on an existing project, however multiple projects can refer to a single estimate project.</span></span> <span data-ttu-id="87777-107">ניתן לצרף רק פרויקטים של מחיר קבוע והשקעה לפרויקטי הערכה, ופרויקטים אלה חייבים להשתייך לאותה קבוצת פרויקטים אליה משתייך פרויקט ההערכה.</span><span class="sxs-lookup"><span data-stu-id="87777-107">Only fixed-price and investment projects can be attached to estimate projects, and those projects must belong to the same project group as the estimate project.</span></span>

<span data-ttu-id="87777-108">כדי לבטל פרויקט ערכה, יש להשלים אותו.</span><span class="sxs-lookup"><span data-stu-id="87777-108">To eliminate an estimate project, it must be complete.</span></span> <span data-ttu-id="87777-109">השלבים הבאים מסבירים כיצד לבטל הערכה.</span><span class="sxs-lookup"><span data-stu-id="87777-109">The following steps explain how to eliminate an estimate.</span></span>

1. <span data-ttu-id="87777-110">עבור אל **ניהול פרויקטים וחשבונאות** > **כל הפרויקטים** ופתח את הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="87777-110">Go to **Project management and accounting** > **All Projects** and open the project.</span></span> 
2. <span data-ttu-id="87777-111">בכרטיסיה **ניהול** בחר **הערכות**, ועל דף **ההערכות** בחר **בטל**.</span><span class="sxs-lookup"><span data-stu-id="87777-111">On the **Manage** tab, select **Estimates**, and on the **Estimate** page select **Eliminate**.</span></span>
3. <span data-ttu-id="87777-112">בדף **בטל הערכה**  בכרטיסיה **כללי**, הגדר את האפשרויות הבאות:</span><span class="sxs-lookup"><span data-stu-id="87777-112">On the **Eliminate estimate** page on the **General** tab, set the following options:</span></span>

   - <span data-ttu-id="87777-113">**קוד תקופה**: בחר את קוד התקופה לבחירת פרויקטי ההערכה המתאימים.</span><span class="sxs-lookup"><span data-stu-id="87777-113">**Period code**: Select the period code to choose the appropriate estimate projects.</span></span> 
   - <span data-ttu-id="87777-114">**תאריך הערכה**: בחר את תאריך ההערכה המתאים לביטול.</span><span class="sxs-lookup"><span data-stu-id="87777-114">**Estimate date**: Select the appropriate estimate date for elimination.</span></span>
   - <span data-ttu-id="87777-115">**הסר עם אזהרות WIP**: אפשר אפשרות זו כדי לספק הודעה כאשר הערכה המשויכת לעבודה בתהליך (WIP) מבוטל.</span><span class="sxs-lookup"><span data-stu-id="87777-115">**Eliminate with WIP warnings**: Enable this option to provide notification when an estimate that is associated with a work in progress (WIP) will be eliminated.</span></span> <span data-ttu-id="87777-116">כאשר אפשרות זו אינה זמינה, לא ניתן להמשיך בביטול אם קיימות עסקאות שאינן משוערות.</span><span class="sxs-lookup"><span data-stu-id="87777-116">When this option is not enabled, elimination can’t continue if any non-estimated transactions exist.</span></span> 
   > [!NOTE]
   > <span data-ttu-id="87777-117">אפשרות זו זמינה רק כאשר ביטול מוחל על פרויקט הערכה.</span><span class="sxs-lookup"><span data-stu-id="87777-117">This option is available only when elimination is applied to an estimate project.</span></span> <span data-ttu-id="87777-118">היא אינה זמינה אם משתמשים רשומים תקופתיים.</span><span class="sxs-lookup"><span data-stu-id="87777-118">It is not available if you are using periodic postings.</span></span> <span data-ttu-id="87777-119">הגדרה זו עובדת עם ההגדרות בכרטיסיה **הערכה** בדף **פרמטרי הפרויקט** , בקבוצת השדות **אפשר ביטול כאשר קיימות עסקאות שאינן משוערות**.</span><span class="sxs-lookup"><span data-stu-id="87777-119">This setting works with the settings on the **Estimate** tab on the **Project parameters** page, in the **Allow elimination when non-estimated transactions exist** field group.</span></span>
   - <span data-ttu-id="87777-120">**הגדר את שלב להסתיים**: אפשר אפשרות זו כדי להגדיר את שלב הפרויקט ההערכה ל **הסתיים** לאחר הפעלת הביטול.</span><span class="sxs-lookup"><span data-stu-id="87777-120">**Set stage to Finished**: Enable this option to set the estimate project’s stage to **Finished** after you run the elimination.</span></span>
   - <span data-ttu-id="87777-121">**הדפסת רשימת הערכות**: בחר במידע שיש לכלול בעת הדפסת רשימת הערכות.</span><span class="sxs-lookup"><span data-stu-id="87777-121">**Print estimate list**: Select the information to be included when the estimate list is printed.</span></span>
   - <span data-ttu-id="87777-122">**הצג Infolog**: הפוך אפשרות זו לזמינה כדי להציג את ה-Infolog.</span><span class="sxs-lookup"><span data-stu-id="87777-122">**Show Infolog**: Enable this option to display the Infolog.</span></span>
   - <span data-ttu-id="87777-123">**תאריך רישום**: בחר את תאריך הרישום של ההערכה בספר הראשי.</span><span class="sxs-lookup"><span data-stu-id="87777-123">**Posting date**: Choose the ledger posting date of the estimate.</span></span>

4.  <span data-ttu-id="87777-124">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="87777-124">Select **OK**.</span></span>
5. <span data-ttu-id="87777-125">לאחר סיום תהליך הביטול, מוצג פרויקט ההערכה המבוטל עם ערך שלילי.</span><span class="sxs-lookup"><span data-stu-id="87777-125">After the elimination process is complete, the eliminated estimate project is displayed with a negative value.</span></span> 

<span data-ttu-id="87777-126">אם לא התכוונת לבטל הערכה, תוכל לבחור בהערכה שבוטלה ולבחור **היפוך ביטול**.</span><span class="sxs-lookup"><span data-stu-id="87777-126">If you did not intend to eliminate an estimate, you can select the eliminated estimate and select **Reverse elimination**.</span></span>   


[!INCLUDE[footer-include](../includes/footer-banner.md)]