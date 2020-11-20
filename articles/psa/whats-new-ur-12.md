---
title: מה חדש או שונה במהדורה המעודכנת של Project Service Automation, 12 V3
description: נושא זה מספק מידע על מה חדש בעדכון המהדורה 12, V3 של Project Service Automation.
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
ms.openlocfilehash: fc92a5dcc111688159f9be5b2839b7c040404a3b
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4119959"
---
# <a name="project-service-automation-update-release-12-v3"></a><span data-ttu-id="1876e-103">מהדורה 12, V3 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="1876e-103">Project Service Automation Update Release 12, V3</span></span>
<span data-ttu-id="1876e-104">אנו שמחים להכריז על העדכון האחרון עבור יישום Dynamics 365 Project Service Automation‏ (PSA).</span><span class="sxs-lookup"><span data-stu-id="1876e-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="1876e-105">מהדורה זו כוללת כמה שיפורים חשובים באיכות, בביצועים ובשימושיות.</span><span class="sxs-lookup"><span data-stu-id="1876e-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="1876e-106">מהדורה זו תואמת את Dynamics 365 9.x.</span><span class="sxs-lookup"><span data-stu-id="1876e-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="1876e-107">כדי לעדכן למהדורה זו, בקר במרכז הניהול של Dynamics 365 ועבור לדף הפתרונות כדי להתקין את העדכון.</span><span class="sxs-lookup"><span data-stu-id="1876e-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="1876e-108">למידע נוסף: [התקנה, עדכון או הסרה של פתרון מועדף](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="1876e-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="1876e-109">נושא זה מפרט את התכונות והתיקונים החדשים או ששונו עבור מהדורה 12, עדכון V3 של Project Service Automation.</span><span class="sxs-lookup"><span data-stu-id="1876e-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 12.</span></span> <span data-ttu-id="1876e-110">מספר ה-build של גירסה זו הוא V3.10.2.34 והיא זמינה דרך עדכון עצמי החל מאוקטובר 2019.</span><span class="sxs-lookup"><span data-stu-id="1876e-110">This version has a build number of V3.10.2.34 and is generally available through a self-update in October 2019.</span></span>

## <a name="update-release-12"></a><span data-ttu-id="1876e-111">הפצת עדכון 12</span><span class="sxs-lookup"><span data-stu-id="1876e-111">Update Release 12</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="1876e-112">תיקוני באגים</span><span class="sxs-lookup"><span data-stu-id="1876e-112">Bug fixes</span></span>

- <span data-ttu-id="1876e-113">זמן והוצאה</span><span class="sxs-lookup"><span data-stu-id="1876e-113">Time and Expense</span></span>

    - <span data-ttu-id="1876e-114">תוקן: שגיאה בערך זמן עודכנה עם הקשר רלוונטי יותר.</span><span class="sxs-lookup"><span data-stu-id="1876e-114">Fixed: Time entry error messaging has been updated with more relevant context.</span></span>
    - <span data-ttu-id="1876e-115">תוקן: רשת של ערך זמן ותזמון מציגים כראוי את סרגל הגלילה האנכי במידת הצורך.</span><span class="sxs-lookup"><span data-stu-id="1876e-115">Fixed: Time entry grid and schedule correctly displays the vertical scrollbar when required.</span></span>
    - <span data-ttu-id="1876e-116">תוקן: ניתן לאשר הוצאה שנשלחה וערכי זמן שדווחו.</span><span class="sxs-lookup"><span data-stu-id="1876e-116">Fixed: Submitted expense and time entries can be approved.</span></span>
    - <span data-ttu-id="1876e-117">תוקן: הודעת הדו-שיח לאישור תוקנה כדי לשקף את מצב האישור בעת שינוי ממצב **אושר** למצב **נשלח**.</span><span class="sxs-lookup"><span data-stu-id="1876e-117">Fixed: Cancel approval confirmation dialog message has been corrected to reflect the status of the approval when changed from **Approved** to **Submitted**.</span></span>
    - <span data-ttu-id="1876e-118">תוקן: השדות **מחיר**, **יחידה**, ו- **כמות** נעולים כעת ברשומת ההוצאות לאחר אישורם.</span><span class="sxs-lookup"><span data-stu-id="1876e-118">Fixed: **Price**, **Unit**, and **Quantity** fields are now locked on the Expense record after it is has been approved.</span></span>

- <span data-ttu-id="1876e-119">ניהול פרויקט</span><span class="sxs-lookup"><span data-stu-id="1876e-119">Project Management</span></span>

    - <span data-ttu-id="1876e-120">תוקן: הפעולה **חדש** בטופס הראשי של **חבר צוות** הוסרה.</span><span class="sxs-lookup"><span data-stu-id="1876e-120">Fixed: **New** action on **Team member** main form has been removed.</span></span>
    - <span data-ttu-id="1876e-121">תוקן: הקצאות משאבים עודכנו כדי להתחשב בשגיאות עיגול לא מדויקות, מה שמוביל לשינוי בתאריך סיום המשימה.</span><span class="sxs-lookup"><span data-stu-id="1876e-121">Fixed: Resource assignments have been updated to account for inaccurate rounding errors, which lead to a shift in a task’s end date.</span></span>
    - <span data-ttu-id="1876e-122">תוקן: ברשת המשימות, שגיאות רלוונטיות בצד השרת יופיעו בפני המשתמש.</span><span class="sxs-lookup"><span data-stu-id="1876e-122">Fixed: In the task grid, relevant server-side errors will be surfaced to the user.</span></span>
    - <span data-ttu-id="1876e-123">תוקן: שמו של חבר הצוות מופיע כעת בבוחר אנשי המשימה במקום שם התפקיד.</span><span class="sxs-lookup"><span data-stu-id="1876e-123">Fixed: The team member’s name now renders in the task people picker instead of the position name.</span></span>

- <span data-ttu-id="1876e-124">ניהול משאבים</span><span class="sxs-lookup"><span data-stu-id="1876e-124">Resource Management</span></span>

    - <span data-ttu-id="1876e-125">תוקן: פרטי דרישת המשאבים לפרויקטים שנוצרו מתבנית משתמשים כעת בלוח השנה של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="1876e-125">Fixed: Resource requirement details for projects created from a template now use the project calendar.</span></span>
    - <span data-ttu-id="1876e-126">תוקן: מיומנויות וכישורים הם כעת כברירת מחדל מנתוני האב של תפקידים לדרישת המשאב שנוצרה עבור אותו תפקיד.</span><span class="sxs-lookup"><span data-stu-id="1876e-126">Fixed: Skills and competencies now default from role master data to the resource requirement created for that role.</span></span>

- <span data-ttu-id="1876e-127">Sales</span><span class="sxs-lookup"><span data-stu-id="1876e-127">Sales</span></span>

    - <span data-ttu-id="1876e-128">תוקן: מזהי אובייקטים כפולים שנמצאו בטופס **עיקרי חוזה**.</span><span class="sxs-lookup"><span data-stu-id="1876e-128">Fixed: Duplicate object IDs found on the **Contract main** form.</span></span>
    - <span data-ttu-id="1876e-129">תוקן: הלוגיקה עודכנה כדי להפוך את הכרטיסיה **ניתוח הצעת מחיר** לגלויה כך שהיא תציג את הגדרת המטא נתונים של הכרטיסיה.</span><span class="sxs-lookup"><span data-stu-id="1876e-129">Fixed: Logic has been updated to make the **Quote Analysis** tab visible so that it displays the metadata setup of the tab.</span></span>
    - <span data-ttu-id="1876e-130">תוקן: תאריך החשבונאות ברשומה בפועל מגיע כעת ממועד תאריך הזנת השעה/ההוצאה ולא ממועד האישור.</span><span class="sxs-lookup"><span data-stu-id="1876e-130">Fixed: Accounting date on the actual record now comes from the date of the time/expense entry date and not the date of the approval.</span></span>
