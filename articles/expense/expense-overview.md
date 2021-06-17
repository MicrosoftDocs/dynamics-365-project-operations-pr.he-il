---
title: מבט כולל על הוצאה
description: נושא זה מספק מידע על פונקציונליות ההוצאות ב-Project Operations.
author: stsporen
ms.date: 10/06/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 2a26b321e15080cc6a4a6a3ed410be175e790a1b
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995397"
---
# <a name="expense-home-page"></a><span data-ttu-id="7d7af-103">דף הבית של הוצאה</span><span class="sxs-lookup"><span data-stu-id="7d7af-103">Expense home page</span></span>

<span data-ttu-id="7d7af-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="7d7af-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="7d7af-105">Dynamics 365 Project Operations תומך ביכולת לעבד הוצאות.</span><span class="sxs-lookup"><span data-stu-id="7d7af-105">Dynamics 365 Project Operations supports the ability to process expenses.</span></span> <span data-ttu-id="7d7af-106">עיבוד הוצאות מתרחש עם או בלי פרויקטים באמצעות זרימת עבודה הניתנת להתאמה אישית של קווי מדיניות, קטגוריות של עסקאות, ואישורים.</span><span class="sxs-lookup"><span data-stu-id="7d7af-106">Expense processing occurs with or without projects by using a customizable workflow of policies, transaction categories, and approvals.</span></span>

<span data-ttu-id="7d7af-107">ב-Project Operations, ישנם שני מודלים לפריסה נתמכים עבור הוצאות:</span><span class="sxs-lookup"><span data-stu-id="7d7af-107">In Project Operations, there are two supported deployment models for Expense:</span></span> 

- <span data-ttu-id="7d7af-108">**מלאה**: פריסה מלאה זמינה עבור **Project Operations עבור תרחישים מבוססי משאבים / ללא מלאי** אוֹ עבור **Project Operations לתרחישים מבוססי הזמנות ייצור**.</span><span class="sxs-lookup"><span data-stu-id="7d7af-108">**Full**: Full deployment is available for **Project Operations for resource/non-stocked based scenarios** or **Project Operations for production order-based scenarios**.</span></span>
- <span data-ttu-id="7d7af-109">**בסיסי**: פריסה בסיסית זמינה עבור **פעולות פרויקט לתרחישים מבוססי משאבים / ללא מלאי** ועובר **פריסת לייט - מהעסקה ועד להוצאת חשבונית פרופורמה**.</span><span class="sxs-lookup"><span data-stu-id="7d7af-109">**Basic**: Basic deployment is available for **Project Operations for resource/non-stocked based scenarios** and **Lite deployment – deal to proforma invoicing**.</span></span>

## <a name="full"></a><span data-ttu-id="7d7af-110">מלא</span><span class="sxs-lookup"><span data-stu-id="7d7af-110">Full</span></span> 
<span data-ttu-id="7d7af-111">פריסת הוצאות מלאה מספקת אכיפת מדיניות מלאה הכוללת את היכולת ליצור מדיניות, כגון:</span><span class="sxs-lookup"><span data-stu-id="7d7af-111">Full Expense deployment provides a complete policy enforcement that includes the ability to create policies, such as:</span></span>

  - <span data-ttu-id="7d7af-112">הגבלות קטגוריית ההוצאות</span><span class="sxs-lookup"><span data-stu-id="7d7af-112">Expense category limits</span></span>
  - <span data-ttu-id="7d7af-113">נסיעה</span><span class="sxs-lookup"><span data-stu-id="7d7af-113">Travel</span></span>
  - <span data-ttu-id="7d7af-114">אש"ל</span><span class="sxs-lookup"><span data-stu-id="7d7af-114">Per diem</span></span>
  - <span data-ttu-id="7d7af-115">ייבוא כרטיסי אשראי</span><span class="sxs-lookup"><span data-stu-id="7d7af-115">Credit card imports</span></span>
  - <span data-ttu-id="7d7af-116">קבלת זיהוי תווים אופטי</span><span class="sxs-lookup"><span data-stu-id="7d7af-116">Receipt optical character recognition</span></span>

## <a name="basic"></a><span data-ttu-id="7d7af-117">בסיסית</span><span class="sxs-lookup"><span data-stu-id="7d7af-117">Basic</span></span> 
<span data-ttu-id="7d7af-118">תרחיש פריסת הוצאות בסיסית מאפשר לך רק לרשום הוצאות בסיסיות כנגד פרויקט.</span><span class="sxs-lookup"><span data-stu-id="7d7af-118">Basic Expense deployment scenario only allows you to record basic expenses against a project.</span></span> 

<span data-ttu-id="7d7af-119">למידע נוסף ראה [ערך הוצאה (לייט)](basic-expense.md)</span><span class="sxs-lookup"><span data-stu-id="7d7af-119">For more information, see [Expense entry (lite)](basic-expense.md)</span></span>

## <a name="determine-your-expense-deployment"></a><span data-ttu-id="7d7af-120">קביעת סוג הפריסת ההוצאות</span><span class="sxs-lookup"><span data-stu-id="7d7af-120">Determine your Expense deployment</span></span>
<span data-ttu-id="7d7af-121">כדי לקבוע אם אתה מפעיל את פריסת ניהול ההוצאות הבסיסית, ודא שכתובת האתר מסתיימת ב-**.crm.dynamics.com**.</span><span class="sxs-lookup"><span data-stu-id="7d7af-121">To determine if you're running the Basic Expense management deployment, verify that the address URL ends with **.crm.dynamics.com**.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]