---
title: מה חדש או השתנה בגירסה ‎3.x wave 1 2020 של Project Service Automation
description: נושא זה מספק מידע על מה חדש ומה שהשתנה בגירסה 3, גל 1 2020 של Project Service Automation.
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 01/24/2020
ms.topic: article
ms.prod: ''
ms.technology: Dynamics 365 Project Service Automation 3.x wave 1 2020
author: stsporen
ms.assetid: 48b408c1-11e7-4005-abac-8fd7c0b064b1
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 478080c0570b71188c9f1e12b18b5aadc13903e5
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751801"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3-wave-1-2020"></a><span data-ttu-id="6d358-103">מה חדש או השתנה בגירסה ‎3 גל 1 2020 של Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="6d358-103">What's new or changed in Project Service Automation version 3 wave 1 2020</span></span>
<span data-ttu-id="6d358-104">הנושא מדגיש את השיקולים המרכזיים לשדרוג בעת המעבר למהדורה האחרונה של Project Service Automation‏ (PSA) גירסה ‎ 3.xגל 1 2020.</span><span class="sxs-lookup"><span data-stu-id="6d358-104">The topic highlights key upgrade considerations when moving to the latest release of Project Service Automation (PSA) version 3.x wave 1 2020.</span></span>

## <a name="time-entry"></a><span data-ttu-id="6d358-105">ערך זמן</span><span class="sxs-lookup"><span data-stu-id="6d358-105">Time entry</span></span>
<span data-ttu-id="6d358-106">החוויה של הכנסת ערך הזמן הורחבה כדי לספק יכולות להארכת ערכי הזמן לתרחישים רבים יותר של לקוחות.</span><span class="sxs-lookup"><span data-stu-id="6d358-106">The time entry experience has been extended to deliver capabilities for extending time entry into more customer scenarios.</span></span> <span data-ttu-id="6d358-107">זה כולל את היכולת להוסיף סוגי ערכים, מה שמניע כעת התנהגות ספציפית על סמך שם סכימת השדה **הגדרות ערך זמן**, שמוצג בתור **מקור זמן**.</span><span class="sxs-lookup"><span data-stu-id="6d358-107">This includes the capability to add entry types, which now drive specific behavior based on the field schema name **Time Entry Settings**, displayed as **Time Source**.</span></span>

### <a name="upgrade-consideration"></a><span data-ttu-id="6d358-108">שיקולים לגבי שדרוג</span><span class="sxs-lookup"><span data-stu-id="6d358-108">Upgrade consideration</span></span>
<span data-ttu-id="6d358-109">כדי לתמוך בפונקציונליות זו, התפקידים בתוך PSA עודכנו כך שהם כוללים הרשאות חדשות.</span><span class="sxs-lookup"><span data-stu-id="6d358-109">To support this functionality, the roles within PSA have been updated to include new privileges.</span></span> <span data-ttu-id="6d358-110">הרשאות אלה מעניקות גישה לקריאה לישות החדשה, **הגדרות ערך זמן**.</span><span class="sxs-lookup"><span data-stu-id="6d358-110">These privileges grant read access to the new entity, **Time Entry Settings**.</span></span>

<span data-ttu-id="6d358-111">משתמשים הזקוקים ליכולת רישום זמן צריכים לקבל את תפקיד המשתמש **משתמש עם ערך זמן** בנוסף לתפקידים הקיימים.</span><span class="sxs-lookup"><span data-stu-id="6d358-111">Users who require the ability to log time should be granted the user role **Time Entry User** in addition to existing roles.</span></span> <span data-ttu-id="6d358-112">תפקיד זה כולל את הפונקציונליות החדשה ומבטיח שערך הזמן ימשיך לעבוד.</span><span class="sxs-lookup"><span data-stu-id="6d358-112">This role includes the new functionality and ensures that time entry will continue to work.</span></span>

### <a name="currently-extended-time-entry-changes"></a><span data-ttu-id="6d358-113">שינויים נוכחיים בערכי זמן מורחבים</span><span class="sxs-lookup"><span data-stu-id="6d358-113">Currently extended time entry changes</span></span>
<span data-ttu-id="6d358-114">כדי למזער את ההשפעה על המשתמשים הנוכחיים בערכי זמן, שינוי תפקיד זה הוא הדרישה המרכזית היחידה הנחוצה כדי להמשיך ולהשתמש בערכי זמן.</span><span class="sxs-lookup"><span data-stu-id="6d358-114">To minimize the impact to current users of time entry, this role change is the only core requirement necessary to continue utilizing time entry.</span></span> <span data-ttu-id="6d358-115">אם יצרת תצוגות מותאמות אישית או חוויות נפרדות של ערכי זמן, עליך להגדיר את השדות של **הגדרת ערך זמן** לערך ה-PSA הנכון.</span><span class="sxs-lookup"><span data-stu-id="6d358-115">If you have created custom views or separate time entry experiences, you must set the **Time Entry Setting** fields to the correct PSA value.</span></span>
