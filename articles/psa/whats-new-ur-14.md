---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 14 V3
description: נושא זה מספק מידע על מה חדש בעדכון המהדורה 14 V3 של Project Service Automation.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/29/2020
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
ms.openlocfilehash: b811bf7ccfb626e6944801dffa943d2afab0c5e8
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4124819"
---
# <a name="project-service-automation-update-release-14-v3"></a><span data-ttu-id="c3979-103">מהדורה 14, V3 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="c3979-103">Project Service Automation Update Release 14, V3</span></span>
<span data-ttu-id="c3979-104">אנו שמחים להכריז על העדכון האחרון עבור יישום Dynamics 365 Project Service Automation‏ (PSA).</span><span class="sxs-lookup"><span data-stu-id="c3979-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="c3979-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="c3979-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="c3979-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="c3979-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="c3979-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="c3979-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="c3979-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="c3979-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="c3979-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 14, עדכון V3 של PSA.</span><span class="sxs-lookup"><span data-stu-id="c3979-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 14.</span></span> <span data-ttu-id="c3979-110">מספר ה-Build של גרסה זו הוא V3.10.4.21 והיא זמינה בלוח הזמנים הבא:</span><span class="sxs-lookup"><span data-stu-id="c3979-110">This version has a build number of V3.10.4.21 and is available on the following schedule:</span></span>

- <span data-ttu-id="c3979-111">**זמינות כללית (עדכון עצמי):** ינואר 2020</span><span class="sxs-lookup"><span data-stu-id="c3979-111">**General availability (self-update):** January 2020</span></span>
- <span data-ttu-id="c3979-112">**עדכון אוטומטי:** פברואר 2020</span><span class="sxs-lookup"><span data-stu-id="c3979-112">**Auto-update:** February 2020</span></span>

## <a name="update-release-14"></a><span data-ttu-id="c3979-113">הפצת עדכון 14</span><span class="sxs-lookup"><span data-stu-id="c3979-113">Update Release 14</span></span>

### <a name="enhancements"></a><span data-ttu-id="c3979-114">שיפורים</span><span class="sxs-lookup"><span data-stu-id="c3979-114">Enhancements</span></span>

- <span data-ttu-id="c3979-115">Sales</span><span class="sxs-lookup"><span data-stu-id="c3979-115">Sales</span></span>

     - <span data-ttu-id="c3979-116">ערכי שדה מותאמים אישית מ- **פרטי שורת הצעת מחיר** מועתקים אל **פרטי סעיף חוזה בפרויקט** כאשר הצעת מחיר מתעדכנת ל **נסגרה כזכייה**.</span><span class="sxs-lookup"><span data-stu-id="c3979-116">Custom field values from **Quote Line Details** are copied to **Project Contract Line Details** when a quote is updated to **Closed as won**.</span></span>
     - <span data-ttu-id="c3979-117">פרויקטים שאושרו יכולים להיות **נסגר כהפסד**.</span><span class="sxs-lookup"><span data-stu-id="c3979-117">Confirmed projects can be **Closed as lost**.</span></span>

- <span data-ttu-id="c3979-118">ניהול משאבים</span><span class="sxs-lookup"><span data-stu-id="c3979-118">Resource Management</span></span>

     - <span data-ttu-id="c3979-119">בעת הארכת הזמנות, המשתמשים יתבקשו דרך תיבת דו-שיח לאישור לסכם את תוצאות ההזמנה ולספק קישור לשמירה על הזמנות.</span><span class="sxs-lookup"><span data-stu-id="c3979-119">When extending bookings, users will be prompted with a confirmation dialog box to summarize booking results and provide a link to Maintain Bookings.</span></span>


### <a name="bug-fixes"></a><span data-ttu-id="c3979-120">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="c3979-120">Bug fixes</span></span>

- <span data-ttu-id="c3979-121">זמן והוצאה</span><span class="sxs-lookup"><span data-stu-id="c3979-121">Time and Expense</span></span>

     - <span data-ttu-id="c3979-122">תוקן: שופרה חווית המשתמש כאשר המשתמש לא בחר ערכים לתיקון.</span><span class="sxs-lookup"><span data-stu-id="c3979-122">Fixed: Improved the user experience when the user has not selected any entries to be corrected.</span></span>

- <span data-ttu-id="c3979-123">ניהול משאבים</span><span class="sxs-lookup"><span data-stu-id="c3979-123">Resource Management</span></span>

     - <span data-ttu-id="c3979-124">תוקן: הזמנת משאב פעמים רבות גורמת לשם המשאב הניתן לספירה להופיע פעמים רבות.</span><span class="sxs-lookup"><span data-stu-id="c3979-124">Fixed: Booking a resource multiple times overflows the name of the bookable resource.</span></span>

- <span data-ttu-id="c3979-125">Sales</span><span class="sxs-lookup"><span data-stu-id="c3979-125">Sales</span></span>

     - <span data-ttu-id="c3979-126">תוקן: מחיר המכירה הכולל לא מחושב עד שהמשתמש מכניס מחיר עלות להערכות ההוצאות על פרויקט.</span><span class="sxs-lookup"><span data-stu-id="c3979-126">Fixed: The total sales price is not calculated until the user also inputs a cost price for expense estimates on a project.</span></span>
     - <span data-ttu-id="c3979-127">תוקן: סגירת הצעת מחיר בתור **זכייה** נכשלה אם חוזה הפרויקט המשויך אינו במצב **טיוטה**.</span><span class="sxs-lookup"><span data-stu-id="c3979-127">Fixed: Closing a quote as **Won** fails if the associated project contract is not in a **Draft** state.</span></span>

