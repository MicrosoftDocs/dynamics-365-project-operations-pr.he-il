---
title: מה חדש או השתנה בגירסה ‎3.x wave 1 2020 של Project Service Automation
description: נושא זה מספק מידע על מה חדש ומה שהשתנה בגירסה 3, גל 1 2020 של Project Service Automation.
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 05/15/2020
ms.topic: article
author: stsporen
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 5110679038ae7ed1e21a3e7dc80a4657e0752b49
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5150939"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3-wave-1-2020"></a><span data-ttu-id="c0490-103">מה חדש או השתנה בגירסה ‎3 גל 1 2020 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="c0490-103">What's new or changed in Project Service Automation version 3 wave 1 2020</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="c0490-104">הנושא מדגיש את השיקולים המרכזיים לשדרוג בעת המעבר למהדורה האחרונה של Project Service Automation‏ (PSA) גירסה ‎ 3.xגל 1 2020.</span><span class="sxs-lookup"><span data-stu-id="c0490-104">The topic highlights key upgrade considerations when moving to the latest release of Project Service Automation (PSA) version 3.x wave 1 2020.</span></span>

## <a name="time-entry"></a><span data-ttu-id="c0490-105">ערך זמן</span><span class="sxs-lookup"><span data-stu-id="c0490-105">Time entry</span></span>
<span data-ttu-id="c0490-106">החוויה של הכנסת ערך הזמן הורחבה כדי לספק יכולות להארכת ערכי הזמן לתרחישים רבים יותר של לקוחות.</span><span class="sxs-lookup"><span data-stu-id="c0490-106">The time entry experience has been extended to deliver capabilities for extending time entry into more customer scenarios.</span></span> <span data-ttu-id="c0490-107">זה כולל את היכולת להוסיף סוגי ערכים, מה שמניע כעת התנהגות ספציפית על סמך שם סכימת השדה **הגדרות ערך זמן**, שמוצג בתור **מקור זמן**.</span><span class="sxs-lookup"><span data-stu-id="c0490-107">This includes the capability to add entry types, which now drive specific behavior based on the field schema name **Time Entry Settings**, displayed as **Time Source**.</span></span> <span data-ttu-id="c0490-108">פתרון חדש, שנקרא 'זמן, הוצאה, סטטוס ואישורים' (TESA) נוסף לתמיכה בפונקציונליות זו.</span><span class="sxs-lookup"><span data-stu-id="c0490-108">A new solution, called Time, Expense, Statusing, and Approvals (TESA) has been added to support this functionality.</span></span>

### <a name="upgrade-consideration"></a><span data-ttu-id="c0490-109">שיקולים לגבי שדרוג</span><span class="sxs-lookup"><span data-stu-id="c0490-109">Upgrade consideration</span></span>
<span data-ttu-id="c0490-110">כדי לתמוך בפונקציונליות זו, התפקידים בתוך PSA עודכנו כך שהם כוללים הרשאות חדשות.</span><span class="sxs-lookup"><span data-stu-id="c0490-110">To support this functionality, the roles within PSA have been updated to include new privileges.</span></span> <span data-ttu-id="c0490-111">הרשאות אלה מעניקות גישה לקריאה לישות החדשה, **הגדרות ערך זמן**.</span><span class="sxs-lookup"><span data-stu-id="c0490-111">These privileges grant read access to the new entity, **Time Entry Settings**.</span></span>

<span data-ttu-id="c0490-112">משתמשים הזקוקים ליכולת רישום זמן צריכים לקבל את תפקיד המשתמש **משתמש עם ערך זמן** בנוסף לתפקידים הקיימים.</span><span class="sxs-lookup"><span data-stu-id="c0490-112">Users who require the ability to log time should be granted the user role **Time Entry User** in addition to existing roles.</span></span> <span data-ttu-id="c0490-113">תפקיד זה כולל את הפונקציונליות החדשה ומבטיח שערך הזמן ימשיך לעבוד.</span><span class="sxs-lookup"><span data-stu-id="c0490-113">This role includes the new functionality and ensures that time entry will continue to work.</span></span>

<span data-ttu-id="c0490-114">בנוסף, אם ברשותך מודולי אפליקציה מותאמים אישית הכוללים את כל הטפסים עבור ישות הזנת הזמן, תידרש להסיר את **טופס ליצירה מהירה של זמן TESA** מהמודול.</span><span class="sxs-lookup"><span data-stu-id="c0490-114">Additionally, if you have any custom app modules that include all forms for the time entry entity, you will be required to remove the **TESA time Entry Quick Create Form** from the module.</span></span>

### <a name="currently-extended-time-entry-changes"></a><span data-ttu-id="c0490-115">שינויים נוכחיים בערכי זמן מורחבים</span><span class="sxs-lookup"><span data-stu-id="c0490-115">Currently extended time entry changes</span></span>
<span data-ttu-id="c0490-116">כדי למזער את ההשפעה על המשתמשים הנוכחיים בערכי זמן, שינוי תפקיד זה הוא הדרישה המרכזית היחידה הנחוצה כדי להמשיך ולהשתמש בערכי זמן.</span><span class="sxs-lookup"><span data-stu-id="c0490-116">To minimize the impact to current users of time entry, this role change is the only core requirement necessary to continue utilizing time entry.</span></span> <span data-ttu-id="c0490-117">אם יצרת תצוגות מותאמות אישית או חוויות נפרדות של ערכי זמן, עליך להגדיר את השדות של **הגדרת ערך זמן** לערך ה-PSA הנכון.</span><span class="sxs-lookup"><span data-stu-id="c0490-117">If you have created custom views or separate time entry experiences, you must set the **Time Entry Setting** fields to the correct PSA value.</span></span>
