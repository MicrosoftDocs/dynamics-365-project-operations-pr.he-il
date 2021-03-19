---
title: יצירת ערכי זמן
description: נושא זה מספק מידע לגבי האופן שבו יוצרים ערכי זמן.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 05/20/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 8f86f69090e869bf5e6a7505a4cb1ad1c69b475b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5282154"
---
# <a name="create-time-entries"></a><span data-ttu-id="8fda3-103">יצירת ערכי זמן</span><span class="sxs-lookup"><span data-stu-id="8fda3-103">Create time entries</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="8fda3-104">בגירסאות קודמות של Dynamics 365 Project Service Automation, ערכי זמן הוזנו על בסיס שבועי.</span><span class="sxs-lookup"><span data-stu-id="8fda3-104">In previous versions of Dynamics 365 Project Service Automation, time entries were entered on a weekly basis.</span></span> <span data-ttu-id="8fda3-105">בגירסה 3 של Project Service Automation, ערכי זמן מוזנים על בסיס יומי.</span><span class="sxs-lookup"><span data-stu-id="8fda3-105">In version 3 of Project Service Automation, time entries are entered on a daily basis.</span></span> <span data-ttu-id="8fda3-106">עם זאת, לאחר יצירה של כמה ערכי זמן, תוכל ליצור אותם בצובר או להעתיק אותם.</span><span class="sxs-lookup"><span data-stu-id="8fda3-106">However, after a few time entries have been created, you can bulk create or copy them.</span></span>

## <a name="create-a-time-entry"></a><span data-ttu-id="8fda3-107">יצירת ערך זמן</span><span class="sxs-lookup"><span data-stu-id="8fda3-107">Create a time entry</span></span>

<span data-ttu-id="8fda3-108">בצע את השלבים הבאים כדי ליצור ערך זמן.</span><span class="sxs-lookup"><span data-stu-id="8fda3-108">Follow these steps to create a time entry.</span></span>

1. <span data-ttu-id="8fda3-109">בדף **ערכי זמן**, בחר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="8fda3-109">On the **Time Entries** page, select **New**.</span></span>
2. <span data-ttu-id="8fda3-110">בתיבת הדו-שיח **יצירה מהירה: ערך זמן**, הזן את המשך של ערך הזמן בדקות, בשעות או בימים.</span><span class="sxs-lookup"><span data-stu-id="8fda3-110">In the **Quick Create: Time Entry** dialog box, enter the duration of the time entry in minutes, hours, or days.</span></span> <span data-ttu-id="8fda3-111">יש להזין את משך הזמן בתבנית הבאה: *x* דקות, *x* שעות או *x* ימים.</span><span class="sxs-lookup"><span data-stu-id="8fda3-111">The duration must be entered in the following format: *x* minutes, *x* hours, or *x* days.</span></span> <span data-ttu-id="8fda3-112">ניתן גם להזין שעות וימים כערכים עשרוניים, כגון *x.x* שעות או *x.x* ימים.</span><span class="sxs-lookup"><span data-stu-id="8fda3-112">Hours and days can also be entered as decimal values, such as *x.x* hours or *x.x* days.</span></span>
3. <span data-ttu-id="8fda3-113">בחר את סוג ערך הזמן ואת הפרויקט שבו אתה מזין את ערך הזמן.</span><span class="sxs-lookup"><span data-stu-id="8fda3-113">Select the type of time entry and the project that you're entering the time entry for.</span></span>
4. <span data-ttu-id="8fda3-114">בשדה **משימת פרויקט**, חפש את המשימה עבור ערך זמן זה.</span><span class="sxs-lookup"><span data-stu-id="8fda3-114">In the **Project Task** field, find the task for this time entry.</span></span>

    > [!NOTE]
    > <span data-ttu-id="8fda3-115">אם אתה יוצר ערך זמן עבור משימה שאינה מוקצית למשתמש, בשדה **‏‫משימת פרויקט**, בחר את לחצן **חיפוש**, בחר **שנה תצוגה** ולאחר מכן בחר **כל משימות הפרויקט הפעיל‬** לפירוט של כל המשימות.</span><span class="sxs-lookup"><span data-stu-id="8fda3-115">If you're creating a time entry for a task that isn't assigned to a user, in the **Project Task** field, select the **Search** button, select **Change View**, and then select **All Active Project Tasks** to list all tasks.</span></span>

5. <span data-ttu-id="8fda3-116">הזן תיאור, אם נדרש תיאור ולאחר מכן בחר **שמור וסגור**.</span><span class="sxs-lookup"><span data-stu-id="8fda3-116">Enter a description, if a description is required, and then select **Save and Close**.</span></span>

<span data-ttu-id="8fda3-117">לאחר שערך הזמן נוצר ונשמר, ניתן לערוך אותו ברשת ערכי הזמן.</span><span class="sxs-lookup"><span data-stu-id="8fda3-117">After the time entry is created and saved, you can edit it in the time entry grid.</span></span> <span data-ttu-id="8fda3-118">רשת ערכי הזמן תומכת בשתי תבניות:</span><span class="sxs-lookup"><span data-stu-id="8fda3-118">The time entry grid supports two formats:</span></span>

- <span data-ttu-id="8fda3-119">ניתן להזין ערכי זמן בתבנית **hh:mm**.</span><span class="sxs-lookup"><span data-stu-id="8fda3-119">You can enter time entries in **hh:mm** format.</span></span> <span data-ttu-id="8fda3-120">כעת מומרת תבנית זו לשעות ולשברים.</span><span class="sxs-lookup"><span data-stu-id="8fda3-120">This format is then converted to hours and fractions.</span></span>
- <span data-ttu-id="8fda3-121">ניתן להזין שעות ושברים ישירות.</span><span class="sxs-lookup"><span data-stu-id="8fda3-121">You can enter hours and fractions directly.</span></span>

<span data-ttu-id="8fda3-122">שים לב ששברים של שעה אינם דקות.</span><span class="sxs-lookup"><span data-stu-id="8fda3-122">Note that the fractions of an hour aren't minutes.</span></span> <span data-ttu-id="8fda3-123">לכן, 1.5 שעות מייצגת 1 שעה ו- 30 דקות.</span><span class="sxs-lookup"><span data-stu-id="8fda3-123">Therefore, 1.5 hours represents 1 hour and 30 minutes.</span></span> <span data-ttu-id="8fda3-124">אותו הכלל חל על שברים של יום.</span><span class="sxs-lookup"><span data-stu-id="8fda3-124">The same rule applies to fractions of a day.</span></span> <span data-ttu-id="8fda3-125">יום אחד הוא 24 שעות ו- 0.5 יום מייצג 12 שעות.</span><span class="sxs-lookup"><span data-stu-id="8fda3-125">One day is 24 hours, and 0.5 days represents 12 hours.</span></span>

## <a name="bulk-create-time-entries"></a><span data-ttu-id="8fda3-126">יצירה של ערכי זמן בצובר</span><span class="sxs-lookup"><span data-stu-id="8fda3-126">Bulk create time entries</span></span>

<span data-ttu-id="8fda3-127">לאחר שנוצרו כמה ערכי זמן, תוכל להעתיק אותם כדי ליצור ערכי זמן נוספים בצובר.</span><span class="sxs-lookup"><span data-stu-id="8fda3-127">After a few time entries have been created, you can copy them to create additional time entries in bulk.</span></span>

1. <span data-ttu-id="8fda3-128">בדף **ערכי זמן**, בחר **העתק שבוע**.</span><span class="sxs-lookup"><span data-stu-id="8fda3-128">On the **Time Entries** page, select **Copy Week**.</span></span>
2. <span data-ttu-id="8fda3-129">בקבוצת השדות **תקופת התחלה**, בשדות **תאריך התחלה** ו **תאריך סיום**, הגדר את טווח התאריכים שמתוכם יועתקו ערכי זמן.</span><span class="sxs-lookup"><span data-stu-id="8fda3-129">In the **From Period** field group, in the **Start Date** and **End Date** fields, define the date range to copy time entries from.</span></span>
3. <span data-ttu-id="8fda3-130">בקבוצת השדות **תקופת סיום**, בשדה **תאריך התחלה**, ציין את התאריך שעבורו יש ליצור ערכי זמן.</span><span class="sxs-lookup"><span data-stu-id="8fda3-130">In the **To Period** field group, in the **Start Date** field, specify the date to create time entries for.</span></span>
4. <span data-ttu-id="8fda3-131">בחר **העתק** כדי ליצור עותק של ערכי הזמן המתאימים ליום בשבוע שצוין בקבוצת השדות **תקופת סיום**.</span><span class="sxs-lookup"><span data-stu-id="8fda3-131">Select **Copy** to create a copy of the time entries that correspond to the day of the week that is specified in the **To Period** field group.</span></span> <span data-ttu-id="8fda3-132">לדוגמה, ערך הזמן עבור יום שני בשבוע שעבר מועתק ליום שני בשבוע שצוין בקבוצת השדות **תקופת סיום**.</span><span class="sxs-lookup"><span data-stu-id="8fda3-132">For example, the time entry for Monday of last week is copied to Monday of the week that is specified in the **To Period** field group.</span></span>

## <a name="import-data-for-time-entries"></a><span data-ttu-id="8fda3-133">ייבוא נתונים עבור ערכי זמן</span><span class="sxs-lookup"><span data-stu-id="8fda3-133">Import data for time entries</span></span>

<span data-ttu-id="8fda3-134">ניתן לייבא נתונים מהזמנות והקצאות של פרויקטים.</span><span class="sxs-lookup"><span data-stu-id="8fda3-134">You can import data from project bookings and assignments.</span></span> <span data-ttu-id="8fda3-135">בעת ייבוא נתונים, ניתן לציין את טווח התאריכים של ההזמנות לייבוא ולאחר מכן לבחור באופן מפורש בהזמנות שיש ליצור כערכי זמן **טיוטה**.</span><span class="sxs-lookup"><span data-stu-id="8fda3-135">When you import data, you can specify the date range of the bookings to import and then explicitly select the bookings that should be created as **Draft** time entries.</span></span>

## <a name="group-by-sort-search-and-filter-capabilities"></a><span data-ttu-id="8fda3-136">יכולות 'קבץ לפי', 'מיון', 'חיפוש' ו'סינון'</span><span class="sxs-lookup"><span data-stu-id="8fda3-136">Group by, sort, search, and filter capabilities</span></span>

<span data-ttu-id="8fda3-137">ניתן לקבץ ולסנן ערכי זמן לפי הממדים שצוינו בעמודות.</span><span class="sxs-lookup"><span data-stu-id="8fda3-137">You can group and filter time entries by the dimensions that are specified in the columns.</span></span> <span data-ttu-id="8fda3-138">בשדה **קבץ לפי**, בחר את הממד שיש להשתמש בו כדי לסנן ערכי זמן.</span><span class="sxs-lookup"><span data-stu-id="8fda3-138">In the **Group by** field, select the dimension to use to filter time entries.</span></span> <span data-ttu-id="8fda3-139">ניתן גם למיין את רשומות ערכי הזמן לפי סדר עולה או יורד באמצעות חץ המיון שבכותרות העמודות.</span><span class="sxs-lookup"><span data-stu-id="8fda3-139">You can also sort the time entry records in ascending or descending order by using the sort arrow on the column headings.</span></span> <span data-ttu-id="8fda3-140">כמו כן, ניתן להציג או להסתיר ערכים על-ידי בחירה בלחצן **סינון** בכותרות העמודות ולאחר מכן, בתיבה **חיפוש**, יש להזין את הטקסט אשר ישמש לחיפוש ערכי זמן לפי שם פרויקט, משימת פרויקט, ערך זמן או משאב.</span><span class="sxs-lookup"><span data-stu-id="8fda3-140">Additionally, you can show or hide entries by selecting the **Filter** button on the column headings, and then, in the **Search** box, entering the text that should be used to search for time entries by project name, project task, time entry, or resource.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]