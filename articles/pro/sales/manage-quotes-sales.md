---
title: ניהול הצעות מחיר של פרוייקט
description: נושא זו מספק מידע על הצעות מחיר של פרויקט.
author: rumant
ms.date: 10/26/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 8e0b20d4780a14edc3c242e261e22d4905f783a4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994812"
---
# <a name="manage-project-quotes"></a><span data-ttu-id="f2c46-103">ניהול הצעות מחיר של פרוייקט</span><span class="sxs-lookup"><span data-stu-id="f2c46-103">Manage project quotes</span></span>

<span data-ttu-id="f2c46-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="f2c46-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f2c46-105">ב- Dynamics 365 Project Operations, הצעות מחיר של פרויקט נועדו לסייע בבניית הצעות לעבודה בפרויקט.</span><span class="sxs-lookup"><span data-stu-id="f2c46-105">In Dynamics 365 Project Operations, project quotes are designed to help build proposals for project work.</span></span> <span data-ttu-id="f2c46-106">מבנה הצעת המחיר לפרויקט ב-Project Operations בנוי להצעות פרויקט עם המרכיבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="f2c46-106">The structure of a project quote in Project Operations is structured for project proposals with the following components:</span></span>

  - <span data-ttu-id="f2c46-107">שורות של הצעות מחיר המזהים את רכיבי העבודה הנפרדים שיוצגו כרכיבים ברמה גבוהה.</span><span class="sxs-lookup"><span data-stu-id="f2c46-107">Quote lines that identify the discrete components of work that will be presented as high-level components.</span></span>
  - <span data-ttu-id="f2c46-108">פרטי שורת הצעת מחיר המזהים ומעריכים את העבודה עבור כל רכיב או שורת הצעת מחיר ברמה גבוהה.</span><span class="sxs-lookup"><span data-stu-id="f2c46-108">Quote line details that identify and estimate the work for each high-level component or quote line.</span></span> <span data-ttu-id="f2c46-109">הערכות של לוח הזמנים או תאריכים וההיבטים הכספיים של עבודה הקשורים לאותה שורת הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="f2c46-109">Schedule or date estimates and the financial aspects for the work are tied to that quote line.</span></span>
  - <span data-ttu-id="f2c46-110">מודלים לחוזים ורכיבים הניתנים לחיוב מוגדרים לכל שורת הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="f2c46-110">Contracting models and chargeable components are set up for each quote line.</span></span> <span data-ttu-id="f2c46-111">מערך זה מסייע להעריך את פריסת ההכנסות, ההוצאות והרווחיות עבור כל שורת הצעות מחיר ועבור הצעת המחיר הכוללת.</span><span class="sxs-lookup"><span data-stu-id="f2c46-111">This set up helps estimate the spread of revenue, spend, and profitability for each quote line and the overall quote.</span></span>

## <a name="view-all-project-based-quotes"></a><span data-ttu-id="f2c46-112">תצוגה של כל הצעות המחיר המבוססות הפרוייקטים</span><span class="sxs-lookup"><span data-stu-id="f2c46-112">View all project-based quotes</span></span>

<span data-ttu-id="f2c46-113">ניתן לראות רשימה של כל הצעות המחיר של פרויקט בדף הרשימה **הצעות מחיר**.</span><span class="sxs-lookup"><span data-stu-id="f2c46-113">A list of all the project quotes can be seen from the **Quotes** list page.</span></span> 

1. <span data-ttu-id="f2c46-114">עבור אל **מכירות** > **הצעות מחיר**.</span><span class="sxs-lookup"><span data-stu-id="f2c46-114">Go to **Sales** > **Quotes**.</span></span> <span data-ttu-id="f2c46-115">מוצגת רשימה של כל הצעות המחיר של פרויקט במערכת.</span><span class="sxs-lookup"><span data-stu-id="f2c46-115">A list of all your project quotes in the system are shown.</span></span> 
2. <span data-ttu-id="f2c46-116">השתמש ב **במחליף התצוגות** כדי לבחור תצוגות מסוננות אחרות של הצעות המחיר.</span><span class="sxs-lookup"><span data-stu-id="f2c46-116">Use the **View Switcher** to select other filtered views of the quotes.</span></span> <span data-ttu-id="f2c46-117">באמצעות קריטריוני סינון מותאמים אישית, ניתן להגדיר אפשרויות תצוגוה וניווט משלך.</span><span class="sxs-lookup"><span data-stu-id="f2c46-117">Using custom filter criteria, you can configure your own views and navigation options.</span></span>

<span data-ttu-id="f2c46-118">ניתן ליצור או למחוק הצעות מחיר מדף רשימה זה או מדפי הפרטים.</span><span class="sxs-lookup"><span data-stu-id="f2c46-118">Quotes can be created or deleted from this list page or detail pages.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]