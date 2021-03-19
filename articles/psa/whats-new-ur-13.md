---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 13 V3
description: נושא זה מספק מידע על מה חדש בעדכון המהדורה 13, V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: dbdcb811bfeacf17e841d679f097c591c16cd4c0
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5281029"
---
# <a name="project-service-automation-update-release-13-v3"></a><span data-ttu-id="9b136-103">מהדורה 13, V3 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="9b136-103">Project Service Automation Update Release 13, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="9b136-104">אנו שמחים להכריז על העדכון האחרון עבור יישום Dynamics 365 Project Service Automation‏ (PSA).</span><span class="sxs-lookup"><span data-stu-id="9b136-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="9b136-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="9b136-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="9b136-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="9b136-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="9b136-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="9b136-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="9b136-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="9b136-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="9b136-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 13, עדכון V3 של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="9b136-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 13.</span></span> <span data-ttu-id="9b136-110">מספר ה-Build של גרסה זו הוא V3.10.3.18 והיא זמינה בלוח הזמנים הבא:</span><span class="sxs-lookup"><span data-stu-id="9b136-110">This version has a build number of V3.10.3.18 and is available on the following schedule:</span></span>

- <span data-ttu-id="9b136-111">**זמינות כללית (עדכון עצמי):** נובמבר 2019</span><span class="sxs-lookup"><span data-stu-id="9b136-111">**General availability (self-update):** November 2019</span></span>
- <span data-ttu-id="9b136-112">**עדכון עצמי:** דצמבר 2019</span><span class="sxs-lookup"><span data-stu-id="9b136-112">**Auto-update:** December 2019</span></span>


## <a name="update-release-13"></a><span data-ttu-id="9b136-113">הפצת עדכון 13</span><span class="sxs-lookup"><span data-stu-id="9b136-113">Update Release 13</span></span> 

### <a name="bug-fixes"></a><span data-ttu-id="9b136-114">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="9b136-114">Bug fixes</span></span>

- <span data-ttu-id="9b136-115">זמן והוצאה</span><span class="sxs-lookup"><span data-stu-id="9b136-115">Time and Expense</span></span>

     - <span data-ttu-id="9b136-116">קבוע: פונקציונליות חיפוש בדף **אישור הוצאה** אינו פועל בעת חיפוש לפי מטרת ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="9b136-116">Fixed: Search functionality on the **Expense approval** page does not work when searching by expense purpose.</span></span>

- <span data-ttu-id="9b136-117">ניהול משאבים</span><span class="sxs-lookup"><span data-stu-id="9b136-117">Resource Management</span></span>

     - <span data-ttu-id="9b136-118">קבוע: המספרים בהתאמה עודכנו כמיושרים לימין.</span><span class="sxs-lookup"><span data-stu-id="9b136-118">Fixed: Numbers in the reconciliation have been updated to be right justified.</span></span>
     - <span data-ttu-id="9b136-119">קבוע: לא ניתן להקצות משאבים עם שם למשימות דרך הכרטיסיה **לוח זמנים**.</span><span class="sxs-lookup"><span data-stu-id="9b136-119">Fixed: Named Resources can't be assigned to tasks through the **Schedule** tab.</span></span>

- <span data-ttu-id="9b136-120">ניהול פרויקט</span><span class="sxs-lookup"><span data-stu-id="9b136-120">Project Management</span></span>

     - <span data-ttu-id="9b136-121">קבוע: חריגה מערך Null בעת הקצאת חבר צוות כאשר בערך **TransactionType‎** חסרים נתוני התקנה עבור **יחידה** ו- **DefaultGroup**.</span><span class="sxs-lookup"><span data-stu-id="9b136-121">Fixed: Null reference exception when assigning team member when the **TransactionType** is missing setup information for **Unit** and **DefaultGroup**.</span></span>

- <span data-ttu-id="9b136-122">Sales</span><span class="sxs-lookup"><span data-stu-id="9b136-122">Sales</span></span>

     - <span data-ttu-id="9b136-123">קבוע: רשומות מסוג עסקאות כפולות מחזירות שגיאה בעת יצירת רשומות של מחיר תפקיד.</span><span class="sxs-lookup"><span data-stu-id="9b136-123">Fixed: Duplicate transaction type records return an error when role price records are created.</span></span>
     - <span data-ttu-id="9b136-124">תוקן: לחצנים נוספים עבור **הזדמנות חדשה**, **הצעת מחיר**, **שורת הזמנה**, ו **הוסף מוצר** גלויים בפקודות עבור הזדמנויות, הצעות מחיר, הזמנת מוצרים ורשת המשנה של שורות מבוססות פרויקט.</span><span class="sxs-lookup"><span data-stu-id="9b136-124">Fixed: Extra buttons for **New Opportunity**, **Quote**, **Order Line**, and **Add Product** are visible in commands for Opportunities, Quotes, Order Products, and the project-based Lines subgrid.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]