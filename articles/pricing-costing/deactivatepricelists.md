---
title: השבתת מחירונים
description: נושא זה מסביר כיצד להשבית או להסיר מחירונים שאינם בשימוש או ישנים.
author: rumant
ms.date: 03/19/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Professional Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: d5d6cf6b4b097c08edca5a3235ed1b438a0eae2d
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001337"
---
# <a name="deactivate-price-lists"></a><span data-ttu-id="562ae-103">השבתת מחירונים</span><span class="sxs-lookup"><span data-stu-id="562ae-103">Deactivate price lists</span></span> 

<span data-ttu-id="562ae-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="562ae-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="562ae-105">כדי להסיר מחירונים ישנים או שאינם בשימוש מ-Dynamics 365 Project Operations ישנם שני שלבים שעליך לבצע.</span><span class="sxs-lookup"><span data-stu-id="562ae-105">To remove old or unused price lists from Dynamics 365 Project Operations, there are two steps you must complete.</span></span> 

1. <span data-ttu-id="562ae-106">הסר או מחק את המחירון מדפים ספציפיים.</span><span class="sxs-lookup"><span data-stu-id="562ae-106">Remove or delete the price list from specific pages.</span></span>
2. <span data-ttu-id="562ae-107">השבת או מחק את המחירון מהמחירונים הפעילים בדף **מחירונים**.</span><span class="sxs-lookup"><span data-stu-id="562ae-107">Deactivate or delete the price list from the Active price lists on the **Price Lists** page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="562ae-108">עליך להשלים את שני השלבים כדי להסיר מחירון במלואו.</span><span class="sxs-lookup"><span data-stu-id="562ae-108">You must complete both steps to fully remove a price list.</span></span> <span data-ttu-id="562ae-109">ביצוע שלב 2 בלבד, שהוא מחיקה או השבתה ישירה של המחירון מתצוגת מחירונים פעילים, אינו מספיק.</span><span class="sxs-lookup"><span data-stu-id="562ae-109">Only performing step 2, which is to directly delete or deactivate the price list from the Active Price Lists view, is not sufficient.</span></span> <span data-ttu-id="562ae-110">עליך למחוק גם את שיוך המחירון הזה מכל המקומות שהוזכרו בשלב 1.</span><span class="sxs-lookup"><span data-stu-id="562ae-110">You must also delete the association of this price list from all the places mentioned in step 1.</span></span>

## <a name="delete-the-price-list-from-specific-pages"></a><span data-ttu-id="562ae-111">מחיקת המחירון מדפים ספציפיים</span><span class="sxs-lookup"><span data-stu-id="562ae-111">Delete the price list from specific pages</span></span>
1. <span data-ttu-id="562ae-112">כדי למחוק מחירון מ-Project Operations, עבור לדפים הבאים:</span><span class="sxs-lookup"><span data-stu-id="562ae-112">To delete a price list from Project Operations, go to the following pages:</span></span>  

      - <span data-ttu-id="562ae-113">הדף **פרמטרי פרויקט** > הכרטיסיה **מחירונים**</span><span class="sxs-lookup"><span data-stu-id="562ae-113">**Project parameters** page > **Price Lists** tab</span></span>
      - <span data-ttu-id="562ae-114">הדף **יחידה ארגונית** > רשת **מחירונים**</span><span class="sxs-lookup"><span data-stu-id="562ae-114">**Organizational Unit** page > **Price Lists** grid</span></span>
      - <span data-ttu-id="562ae-115">הדף **חשבון** > רשת **מחירוני פרויקט**</span><span class="sxs-lookup"><span data-stu-id="562ae-115">**Account** page > **Project Price Lists** grid</span></span>
      - <span data-ttu-id="562ae-116">הדף **הצעות מחיר של פרויקט** > רשת **מחירוני פרויקט**: זה חל על כל הצעות המחיר הפעילות של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="562ae-116">**Project Quotes** page > **Project Price Lists** grid: This applies to all active project quotes.</span></span>
      - <span data-ttu-id="562ae-117">הדף **חוזי פרויקט** > רשת **מחירוני פרויקט**: זה חל על כל החוזים הפעילים של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="562ae-117">**Project Contracts** page > **Project Price Lists** grid: This applies to all active project contracts.</span></span>

 2. <span data-ttu-id="562ae-118">עבור כל דף, עליך לבחור את המחירון שברצונך למחוק, ואז לבחור באפשרות **מחיקה**.</span><span class="sxs-lookup"><span data-stu-id="562ae-118">For each page, you need to select the price list that you want to delete, and then select **Delete**.</span></span> 
 
## <a name="delete-or-deactivate-the-price-list-from-the-price-lists-page"></a><span data-ttu-id="562ae-119">השבתה או מחיקה של המחירון מהדף 'מחירונים'</span><span class="sxs-lookup"><span data-stu-id="562ae-119">Delete or deactivate the price list from the Price Lists page</span></span>
 
1. <span data-ttu-id="562ae-120">כדי למחוק מחירון מהמחירונים הפעילים, עבור אל **מכירות** > **לקוחות** > **מחירונים**.</span><span class="sxs-lookup"><span data-stu-id="562ae-120">To delete a price list from the active price lists, go to **Sales** > **Customers** > **Price Lists**.</span></span> 
2. <span data-ttu-id="562ae-121">בחר את המחירון שברצונך למחוק, ואז בחר באפשרות **מחיקה**.</span><span class="sxs-lookup"><span data-stu-id="562ae-121">Select the price list that you want to delete and then select **Delete**.</span></span> <span data-ttu-id="562ae-122">אם יש הפניה למחירון בעסקאות קיימות כלשהן, לא תוכל למחוק אותו.</span><span class="sxs-lookup"><span data-stu-id="562ae-122">If the price list is referenced on any existing transactions, you won't be able to delete it.</span></span> <span data-ttu-id="562ae-123">אם זה קורה, אתה יכול להשבית את מחירון כך שהוא לא יופיע בשום תצוגה.</span><span class="sxs-lookup"><span data-stu-id="562ae-123">If this happens, you can deactivate the price list so that it doesn't appear in any views.</span></span> 
3. <span data-ttu-id="562ae-124">כדי להשבית את המחירון, בחר שוב במחירון ולאחר מכן בחר **השבת**.</span><span class="sxs-lookup"><span data-stu-id="562ae-124">To deactivate the price list, select the price list again, and then select **Deactivate**.</span></span>   
