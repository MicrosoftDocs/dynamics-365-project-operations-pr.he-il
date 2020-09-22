---
title: מה חדש במהדורה 13, V3 של Project Service Automation
description: נושא זה מספק מידע על מה חדש בעדכון המהדורה 13, V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: business-applications
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation 3.x
ms.assetid: c6f6a5b6-b5bb-467c-b7c7-7fb962504c6d
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5f1b6b3879c94a77ab62082aad1e470a3ba66552
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751805"
---
# <a name="project-service-automation-v3-update-release-13"></a><span data-ttu-id="f1ce0-103">מהדורה 13, עדכון V3 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="f1ce0-103">Project Service Automation V3, Update Release 13</span></span>
<span data-ttu-id="f1ce0-104">אנו שמחים להכריז על העדכון האחרון עבור יישום Dynamics 365 Project Service Automation‏ (PSA).</span><span class="sxs-lookup"><span data-stu-id="f1ce0-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="f1ce0-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="f1ce0-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="f1ce0-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="f1ce0-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="f1ce0-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="f1ce0-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="f1ce0-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="f1ce0-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="f1ce0-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 13, עדכון V3 של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="f1ce0-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 13.</span></span> <span data-ttu-id="f1ce0-110">מספר ה-Build של גרסה זו הוא V3.10.3.18 והיא זמינה בלוח הזמנים הבא:</span><span class="sxs-lookup"><span data-stu-id="f1ce0-110">This version has a build number of V3.10.3.18 and is available on the following schedule:</span></span>

- <span data-ttu-id="f1ce0-111">**זמינות כללית (עדכון עצמי):** נובמבר 2019</span><span class="sxs-lookup"><span data-stu-id="f1ce0-111">**General availability (self-update):** November 2019</span></span>
- <span data-ttu-id="f1ce0-112">**עדכון עצמי:** דצמבר 2019</span><span class="sxs-lookup"><span data-stu-id="f1ce0-112">**Auto-update:** December 2019</span></span>


## <a name="update-release-13"></a><span data-ttu-id="f1ce0-113">הפצת עדכון 13</span><span class="sxs-lookup"><span data-stu-id="f1ce0-113">Update Release 13</span></span> 

### <a name="bug-fixes"></a><span data-ttu-id="f1ce0-114">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="f1ce0-114">Bug fixes</span></span>

- <span data-ttu-id="f1ce0-115">זמן והוצאה</span><span class="sxs-lookup"><span data-stu-id="f1ce0-115">Time and Expense</span></span>

     - <span data-ttu-id="f1ce0-116">קבוע: פונקציונליות חיפוש בדף **אישור הוצאה** אינו פועל בעת חיפוש לפי מטרת ההוצאה.</span><span class="sxs-lookup"><span data-stu-id="f1ce0-116">Fixed: Search functionality on the **Expense approval** page does not work when searching by expense purpose.</span></span>

- <span data-ttu-id="f1ce0-117">ניהול משאבים</span><span class="sxs-lookup"><span data-stu-id="f1ce0-117">Resource Management</span></span>

     - <span data-ttu-id="f1ce0-118">קבוע: המספרים בהתאמה עודכנו כמיושרים לימין.</span><span class="sxs-lookup"><span data-stu-id="f1ce0-118">Fixed: Numbers in the reconciliation have been updated to be right justified.</span></span>
     - <span data-ttu-id="f1ce0-119">קבוע: לא ניתן להקצות משאבים עם שם למשימות דרך הכרטיסיה **לוח זמנים**.</span><span class="sxs-lookup"><span data-stu-id="f1ce0-119">Fixed: Named Resources can't be assigned to tasks through the **Schedule** tab.</span></span>

- <span data-ttu-id="f1ce0-120">ניהול פרוייקט</span><span class="sxs-lookup"><span data-stu-id="f1ce0-120">Project Management</span></span>

     - <span data-ttu-id="f1ce0-121">קבוע: חריגה מערך Null בעת הקצאת חבר צוות כאשר בערך **TransactionType‎** חסרים נתוני התקנה עבור **יחידה** ו- **DefaultGroup**.</span><span class="sxs-lookup"><span data-stu-id="f1ce0-121">Fixed: Null reference exception when assigning team member when the **TransactionType** is missing setup information for **Unit** and **DefaultGroup**.</span></span>

- <span data-ttu-id="f1ce0-122">Sales</span><span class="sxs-lookup"><span data-stu-id="f1ce0-122">Sales</span></span>

     - <span data-ttu-id="f1ce0-123">קבוע: רשומות מסוג עסקאות כפולות מחזירות שגיאה בעת יצירת רשומות של מחיר תפקיד.</span><span class="sxs-lookup"><span data-stu-id="f1ce0-123">Fixed: Duplicate transaction type records return an error when role price records are created.</span></span>
     - <span data-ttu-id="f1ce0-124">קבוע: לחצנים נוספים עבור **הזדמנות חדשה**, **הצעת מחיר**, **שורת הזמנה**, ו- **הוסף מוצר** שגלויים בפקודות עבור הזדמנויות, הצעות מחיר, הזמנת מוצרים ורשת המשנה מבוססת הפרויקטים.</span><span class="sxs-lookup"><span data-stu-id="f1ce0-124">Fixed: Extra buttons for **New Opportunity**, **Quote**, **Order Line**, and **Add Product** are visible in commands for Opportunities, Quotes, Order Products, and the project-based Lines sub-grid.</span></span>


