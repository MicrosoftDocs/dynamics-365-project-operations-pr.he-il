---
title: פרוייקטים של הערכת הכנסה במחיר קבוע
description: נושא זו מספק מידע לגבי הכנסה של מחיר קבוע בפרויקטים.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 80fe1d4171d80ca39e8b7ebb1eefaa524a4f2b07
ms.sourcegitcommit: 2d399bc9d07807626f0d6b2d0cf304240c47591c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 11/17/2020
ms.locfileid: "4531444"
---
# <a name="fixed-price-revenue-estimate-projects"></a><span data-ttu-id="f3034-103">פרוייקטים של הערכת הכנסה במחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="f3034-103">Fixed price revenue estimate projects</span></span> 

<span data-ttu-id="f3034-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="f3034-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="f3034-105">כאשר אתה יוצר סעיף חוזה של פרויקט עם התכונות הבאות של Dynamics 365 Project Operations ב- Microsoft Dataverse, המערכת יוצרת באופן אוטומטי פרויקט אומדן עם הכנסות במחיר קבוע.</span><span class="sxs-lookup"><span data-stu-id="f3034-105">When you create a project contract line with the following attributes in Dynamics 365 Project Operations on Microsoft Dataverse, the system automatically creates a fixed price revenue estimate project.</span></span> <span data-ttu-id="f3034-106">המידע בפרויקט זה מבוסס על הדברים הבאים:</span><span class="sxs-lookup"><span data-stu-id="f3034-106">The information in this project is based on the following:</span></span>

  - <span data-ttu-id="f3034-107">שיטת חיוב במחיר קבוע.</span><span class="sxs-lookup"><span data-stu-id="f3034-107">A fixed price billing method.</span></span>
  - <span data-ttu-id="f3034-108">פרויקט משויך.</span><span class="sxs-lookup"><span data-stu-id="f3034-108">An associated project.</span></span>
  - <span data-ttu-id="f3034-109">לפחות אבן דרך אחת שהוגדרה בכרטיסיה **לוח זמנים לחשבונית** בדף **סעיף חוזה של פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="f3034-109">At least one milestone defined on the **Invoice schedule** tab on the **Project contract line** page.</span></span>

## <a name="review-fixed-price-revenue-estimates-projects"></a><span data-ttu-id="f3034-110">בדיקת פרויקטים של אומדן הכנסה במחיר קבוע</span><span class="sxs-lookup"><span data-stu-id="f3034-110">Review fixed price revenue estimates projects</span></span>
<span data-ttu-id="f3034-111">לבדיקת פרויקטים של אומדני הכנסות במחירים קבועים, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="f3034-111">To review fixed price revenue estimates projects, complete the following steps:</span></span>

1. <span data-ttu-id="f3034-112">בסביבת Dynamics 365 Finance, עבור אל **ניהול פרויקטים וחשבונאות** > **פרויקטים** > **פרויקטים של אומדן הכנסות במחירים קבועים**.</span><span class="sxs-lookup"><span data-stu-id="f3034-112">In the Dynamics 365 Finance environment, go to **Projects management and accounting** > **Projects** > **Fixed price revenue estimate projects**.</span></span>
2. <span data-ttu-id="f3034-113">בחר את הפרויקט שברצונך להציג ולחץ פעמיים על **הערכת מזהה פרויקט** כדי לפתוח את הרשומה ולסקור את פרטי הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="f3034-113">Select the project that you want to view and double-click the **Estimate project ID** to open the record and review the details of the project.</span></span>
3. <span data-ttu-id="f3034-114">הרחב את הכרטיסיה **פרויקט**. תראה פרויקט אחד ברשת **פרויקטים נבחרים**.</span><span class="sxs-lookup"><span data-stu-id="f3034-114">Expand the **Project** tab. You will see one project in the **Selected projects** grid.</span></span> <span data-ttu-id="f3034-115">המערכת משתמשת בזה כפרויקט ברירת המחדל מכיוון שזה הפרויקט המשויך לסעיף חוזה של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="f3034-115">The system uses this as default project because it is the project associated to the project contract line.</span></span> 
4. <span data-ttu-id="f3034-116">כדי לשנות את השיוך, בחר פרויקטים נוספים והוסף אותם לרשת **פרויקטים נבחרים**.</span><span class="sxs-lookup"><span data-stu-id="f3034-116">To change the association, select additional projects and add them to the **Selected projects** grid.</span></span> <span data-ttu-id="f3034-117">אם נבחרים מספר פרויקטים ברשת זו, אחוזי השלמת הפרויקט ואומדני ההכנסות מחושבים יחד עבור כל הפרויקטים שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="f3034-117">If multiple projects are selected in this grid, the project percentage completion and revenue estimates are calculated together for of the all selected projects.</span></span>

  <span data-ttu-id="f3034-118">ניתן להגדיר ידנית את עלות הפרויקט, פרופיל ההכנסות, תבנית עלות וקוד התקופה.</span><span class="sxs-lookup"><span data-stu-id="f3034-118">Project cost, revenue profile, cost template, and the period code can be set manually.</span></span> <span data-ttu-id="f3034-119">אם הם לא מוגדרים באופן ידני, הערכים הם ברירת המחדל במהלך חישוב האומדן הראשון לפרויקט תוך שימוש בכללים שהוגדרו לפרופילי עלות הפרויקט וההכנסות.</span><span class="sxs-lookup"><span data-stu-id="f3034-119">If they aren't set manually, the values default during the first estimate calculation for the project using the rules configured for project cost and revenue profiles.</span></span>

