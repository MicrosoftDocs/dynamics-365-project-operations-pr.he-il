---
title: יצירת מודלי תחזית לתקציבי הפרוייקט
description: נושא מתאר כיצד ליצור מודל תחזית לתקציבים שנותרו.
author: Yowelle
ms.date: 04/24/2020
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
ms.openlocfilehash: 3549b41fce72b44230ab27de081dade15a912266
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6006287"
---
# <a name="create-forecast-models-for-project-budgets"></a><span data-ttu-id="662e7-103">יצירת מודלי תחזית לתקציבי הפרוייקט</span><span class="sxs-lookup"><span data-stu-id="662e7-103">Create forecast models for project budgets</span></span> 

[!include [banner](../includes/banner.md)]

<span data-ttu-id="662e7-104">נושא מתאר כיצד ליצור מודל תחזית לתקציבים שנותרו.</span><span class="sxs-lookup"><span data-stu-id="662e7-104">This topic describes how to create a forecast model for remaining budgets.</span></span> <span data-ttu-id="662e7-105">פרויקט הנתון לבקרת תקציב משתמש בשני סוגים של תקציבים: מקורי ונותר.</span><span class="sxs-lookup"><span data-stu-id="662e7-105">A project that is subject to budget control uses two types of budgets: original and remaining.</span></span> <span data-ttu-id="662e7-106">בעת יצירת תקציב פרויקט, עליך לציין את מודלי תחזית התקציב המקורי והנותר שנוצרו בדף **מודלי תחזית**.</span><span class="sxs-lookup"><span data-stu-id="662e7-106">When you create a project budget, you must specify the original and remaining budget forecast models that were created in the **Forecast models** page.</span></span> <span data-ttu-id="662e7-107">תקציבי פרויקט שמבוססים על המודלים שצוינו נוצרים כאשר אתה מבצע את תקציב הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="662e7-107">Project budgets based on the specified models are created when you commit the project budget.</span></span>

> [!NOTE]
> <span data-ttu-id="662e7-108">מודל תחזית המשמש לבקרת תקציב אינו יכול להיות בעל מודל משנה או לשמש כמודל משנה.</span><span class="sxs-lookup"><span data-stu-id="662e7-108">A forecast model that is used for budget control can’t have a submodel or be used as a submodel.</span></span>

1. <span data-ttu-id="662e7-109">בחר **ניהול פרויקטים וחשבונאות** > **הגדרה** > **תחזיות**  > **מודלי תחזית**.</span><span class="sxs-lookup"><span data-stu-id="662e7-109">Select **Project management and accounting** > **Setup** > **Forecasts**  > **Forecast models**.</span></span>
2. <span data-ttu-id="662e7-110">בחר **חדש** כדי ליצור מודל תחזית חדש ולאחר מכן הזן מספר מזהה מודל ושם עבור המודל החדש.</span><span class="sxs-lookup"><span data-stu-id="662e7-110">Select **New** to create a new forecast model, and then enter a model ID number and name for the new model.</span></span> 
3. <span data-ttu-id="662e7-111">הגדר את האפשרות **הופסק** ל **כן** כדי למנוע שינויים בשורות התחזית עבור מודל התחזית.</span><span class="sxs-lookup"><span data-stu-id="662e7-111">Set the **Stopped** option to **Yes** to prevent any changes to the forecast lines for the forecast model.</span></span> 
4. <span data-ttu-id="662e7-112">אם שורת התחזית שהמודל משויך אליהם אמורים לייצר תחזיות תזרים מזומנים בספר הראשי, הגדר את **כלול בתחזיות תזרים מזומנים** ל **כן.**</span><span class="sxs-lookup"><span data-stu-id="662e7-112">If the forecast lines that the model is associated with should generate cash flow forecasts in the general ledger, set **Include in Cash flow forecasts** to **Yes.**</span></span> 
5. <span data-ttu-id="662e7-113">כדי להשתמש בתאריך הפרויקט כתאריך החשבונית, הגדר את **תאריך חשבונית התחזית** ל **כן**.</span><span class="sxs-lookup"><span data-stu-id="662e7-113">To use the project date as the invoice date, set **Forecast Invoice date** to **Yes**.</span></span> 
6. <span data-ttu-id="662e7-114">בשדה **סוג התקציב** בחר אחד מסוגי המודלים הבאים:</span><span class="sxs-lookup"><span data-stu-id="662e7-114">In the **Budget type** field, select one of the following model types:</span></span>

   - <span data-ttu-id="662e7-115">**תקציב מקורי**: השתמש בסכומי התקציב המקוריים שחויבו כאשר התקציב הראשוני נוצר ואושר.</span><span class="sxs-lookup"><span data-stu-id="662e7-115">**Original budget**: Use the original budget amounts that are committed when the initial budget is created and approved.</span></span>
   - <span data-ttu-id="662e7-116">**תקציב שנותר**: השתמש בסכומי התקציב שנותרו במהלך חיי הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="662e7-116">**Remaining budget**: Use the remaining budget amounts during the life of the project.</span></span> <span data-ttu-id="662e7-117">היתרות במודל תחזית זה מצטמצמות על ידי עסקאות בפועל וגדלות או פחתות על ידי תיקוני תקציב.</span><span class="sxs-lookup"><span data-stu-id="662e7-117">The balances in this forecast model are reduced by actual transactions and increased or decreased by budget revisions.</span></span>
   - <span data-ttu-id="662e7-118">**העברה**: השתמש בסכומי התקציב המועברים לפרויקט.</span><span class="sxs-lookup"><span data-stu-id="662e7-118">**Carry-forward**: Use the carry-forward budget amounts for the project.</span></span> <span data-ttu-id="662e7-119">העברה היא תהליך אופציונלי שניתן להריץ להעברת סכומי תקציב שלא נשעה בהם שימוש משנת כספים אחת לאחרת.</span><span class="sxs-lookup"><span data-stu-id="662e7-119">Carry-forward is an optional process that can be run to transfer unused budget amounts from one fiscal year to another.</span></span>

7. <span data-ttu-id="662e7-120">הגדר את האפשרויות הבאות לפי הצורך:</span><span class="sxs-lookup"><span data-stu-id="662e7-120">Set the following options as required:</span></span>

   - <span data-ttu-id="662e7-121">הפוך לזמין את **תאריך חשבונית התחזית** כדי להשתמש בתאריך הפרויקט כתאריך החשבונית.</span><span class="sxs-lookup"><span data-stu-id="662e7-121">Enable **Forecast invoice date** to use the project date as the invoice date.</span></span>
   - <span data-ttu-id="662e7-122">הפוך לזמין את האפשרות **תחזית עם WIP** לתחזית המבוססת על עבודה בתהליך (WIP), ואז בחר את סוג ה-WIP.</span><span class="sxs-lookup"><span data-stu-id="662e7-122">Enable **Forecast with WIP** to forecast based on work in progress (WIP), and then select the type of WIP.</span></span> 
   - <span data-ttu-id="662e7-123">ניתן לשמור את **סוג תקציב** ברירת המחדל כ **ללא** או הזן סוג חדש.</span><span class="sxs-lookup"><span data-stu-id="662e7-123">You can keep the default **Budget type** as **None** or enter a new type.</span></span> <span data-ttu-id="662e7-124">לא ניתן לשנות את סוג התקציב לאחר שינוי רשומה.</span><span class="sxs-lookup"><span data-stu-id="662e7-124">The budget type can't be changed after you change a record.</span></span>     
    > [!NOTE]
    > <span data-ttu-id="662e7-125">אם תשנה את סוג התקציב המוגדר כברירת מחדל, כל שאר האפשרויות לא יהיו זמינות לעדכונים ולא תוכל לעשות שימוש חוזר במודל התחזית הזה.</span><span class="sxs-lookup"><span data-stu-id="662e7-125">If you change the default budget type, all other options will become unavailable for updates, and you can't reuse this forecast model.</span></span> 
   


 



[!INCLUDE[footer-include](../includes/footer-banner.md)]