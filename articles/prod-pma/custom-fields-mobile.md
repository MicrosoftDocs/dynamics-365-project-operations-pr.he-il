---
title: יישם שדות מותאמים אישית עבור האפליקציה למכשירים ניידים Microsoft Dynamics 365 Project Timesheet ב- iOS וב- Android
description: נושא זה מספק דפוסים נפוצים לשימוש בתוספים לצורך יישום שדות מותאמים אישית.
author: Yowelle
ms.date: 05/29/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.3
ms.search.validFrom: 2019-05-29
ms.openlocfilehash: 23b002559dcbb9118ccb2b36d70707ccb37b19ad
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003034"
---
# <a name="implement-custom-fields-for-the-microsoft-dynamics-365-project-timesheet-mobile-app-on-ios-and-android"></a><span data-ttu-id="6ea9a-103">יישם שדות מותאמים אישית עבור האפליקציה למכשירים ניידים Microsoft Dynamics 365 Project Timesheet ב- iOS וב- Android</span><span class="sxs-lookup"><span data-stu-id="6ea9a-103">Implement custom fields for the Microsoft Dynamics 365 Project Timesheet mobile app on iOS and Android</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="6ea9a-104">נושא זה מספק דפוסים נפוצים לשימוש בתוספים לצורך יישום שדות מותאמים אישית.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-104">This topic provides common patterns for using extensions to implement custom fields.</span></span> <span data-ttu-id="6ea9a-105">אלו הנושאים שמאמר זה סוקר:</span><span class="sxs-lookup"><span data-stu-id="6ea9a-105">The following topics are covered:</span></span>

- <span data-ttu-id="6ea9a-106">סוגי הנתונים השונים שמסגרת השדה המותאמת אישית תומכת בהם</span><span class="sxs-lookup"><span data-stu-id="6ea9a-106">The various data types that the custom field framework supports</span></span>
- <span data-ttu-id="6ea9a-107">כיצד להציג שדות לקריאה בלבד או לעריכה בערכי גליון הזמנים, ולשמור ערכים המסופקים על ידי המשתמש בחזרה למסד הנתונים</span><span class="sxs-lookup"><span data-stu-id="6ea9a-107">How to show read-only or editable fields on timesheet entries, and save user-provided values back to the database</span></span>
- <span data-ttu-id="6ea9a-108">כיצד להציג שדות לקריאה בלבד בכותרת גליון הזמנים</span><span class="sxs-lookup"><span data-stu-id="6ea9a-108">How to show read-only fields on the timesheet header</span></span>
- <span data-ttu-id="6ea9a-109">כיצד לשלב לוגיקה עסקית מותאמת אישית אחרת כדי להזין ערכי ברירת מחדל בשדות ולבצע אימות נוסף</span><span class="sxs-lookup"><span data-stu-id="6ea9a-109">How to integrate other custom business logic to enter default values in fields and do additional validation</span></span>

## <a name="audience"></a><span data-ttu-id="6ea9a-110">קהל</span><span class="sxs-lookup"><span data-stu-id="6ea9a-110">Audience</span></span>

<span data-ttu-id="6ea9a-111">הנושא מיועד למפתחים שמשלבים את השדות המותאמים אישית שלהם באפליקציה למכשירים ניידים Microsoft Dynamics 365 Project Timesheet הזמינה עבור Apple iOS ו- Google Android.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-111">This topic is intended for developers who are integrating their custom fields into the Microsoft Dynamics 365 Project Timesheet mobile application that is available for Apple iOS and Google Android.</span></span> <span data-ttu-id="6ea9a-112">ההנחה היא שהקוראים מכירים את הפיתוח של X++‎ ואת פונקציונליות לוח הזמנים של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-112">The assumption is that readers are familiar with X++ development and project timesheet functionality.</span></span>

## <a name="data-contract--tstimesheetcustomfield-x-class"></a><span data-ttu-id="6ea9a-113">חוזה נתונים - מחלקת TSTimesheetCustomField X++‎</span><span class="sxs-lookup"><span data-stu-id="6ea9a-113">Data contract – TSTimesheetCustomField X++ class</span></span>

<span data-ttu-id="6ea9a-114">מחלקת **TSTimesheetCustomField‎** היא מחלקת חוזה הנתונים X++‎ המייצגת מידע אודות שדה מותאם אישית לפונקציונליות של לוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-114">The **TSTimesheetCustomField** class is the X++ data contract class that represents information about a custom field for timesheet functionality.</span></span> <span data-ttu-id="6ea9a-115">רשימות של אובייקטים בשדה המותאם אישית מועברות הן בחוזה הנתונים TSTimesheetDetails והן בחוזה הנתונים TSTimesheetEntry כדי להציג שדות מותאמים אישית באפליקציה למכשירים ניידים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-115">Lists of the custom field objects are passed on both the TSTimesheetDetails data contract and the TSTimesheetEntry data contract to show custom fields in the mobile app.</span></span>

- <span data-ttu-id="6ea9a-116">**TSTimesheetDetails** - חוזה כותרת של גליון הזמנים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-116">**TSTimesheetDetails** - The timesheet header contract.</span></span>
- <span data-ttu-id="6ea9a-117">**TSTimesheetEntry** - חוזה העסקה בגליון הזמנים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-117">**TSTimesheetEntry** - The timesheet transaction contract.</span></span> <span data-ttu-id="6ea9a-118">קבוצות של אובייקטים אלה שיש להם את אותו מידע על הפרויקט וערך **timesheetLineRecId** מהווה שורה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-118">Groups of these objects that have the same project information and **timesheetLineRecId** value constitute a line.</span></span>

### <a name="fieldbasetype-types"></a><span data-ttu-id="6ea9a-119">fieldBaseType (סוגים)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-119">fieldBaseType (Types)</span></span>

<span data-ttu-id="6ea9a-120">המאפיין **FieldBaseType** שעל אובייקט **TsTimesheetCustom** קובע את סוג השדה שמופיע באפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-120">The **FieldBaseType** property on the **TsTimesheetCustom** object determines the type of the field that appears in the app.</span></span> <span data-ttu-id="6ea9a-121">הערכים **סוגים** הבאים שנתמכים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-121">The following **Types** values that are supported.</span></span>

| <span data-ttu-id="6ea9a-122">ערך סוגים</span><span class="sxs-lookup"><span data-stu-id="6ea9a-122">Types value</span></span> | <span data-ttu-id="6ea9a-123">סוג</span><span class="sxs-lookup"><span data-stu-id="6ea9a-123">Type</span></span>              | <span data-ttu-id="6ea9a-124">הערות</span><span class="sxs-lookup"><span data-stu-id="6ea9a-124">Notes</span></span> |
|-------------|-------------------|-------|
| <span data-ttu-id="6ea9a-125">0</span><span class="sxs-lookup"><span data-stu-id="6ea9a-125">0</span></span>           | <span data-ttu-id="6ea9a-126">מחרוזת (וספירה)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-126">String (and Enum)</span></span> | <span data-ttu-id="6ea9a-127">השדה מופיע כשדה טקסט.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-127">The field appears as a text field.</span></span> |
| <span data-ttu-id="6ea9a-128">1</span><span class="sxs-lookup"><span data-stu-id="6ea9a-128">1</span></span>           | <span data-ttu-id="6ea9a-129">Integer</span><span class="sxs-lookup"><span data-stu-id="6ea9a-129">Integer</span></span>           | <span data-ttu-id="6ea9a-130">הערך מוצג כמספר ללא מקומות עשרוניים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-130">The value is shown as a number without decimal places.</span></span> |
| <span data-ttu-id="6ea9a-131">2</span><span class="sxs-lookup"><span data-stu-id="6ea9a-131">2</span></span>           | <span data-ttu-id="6ea9a-132">אמיתי</span><span class="sxs-lookup"><span data-stu-id="6ea9a-132">Real</span></span>              | <span data-ttu-id="6ea9a-133">הערך מוצג כמספר עם מקומות עשרוניים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-133">The value is shown as a number that has decimal places.</span></span><p><span data-ttu-id="6ea9a-134">כדי להציג את הערך האמיתי כמטבע באפליקציה, השתמש בתוכנה **fieldExtenededType**.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-134">To show the real value as a currency in the app, use the **fieldExtenededType** property.</span></span> <span data-ttu-id="6ea9a-135">אתה יכול להשתמש במאפיין **numberOfDecimals** כדי לקבוע את מספר המקומות העשרוניים המוצגים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-135">You can use the **numberOfDecimals** property to set the number of decimal places that are shown.</span></span></p> |
| <span data-ttu-id="6ea9a-136">3</span><span class="sxs-lookup"><span data-stu-id="6ea9a-136">3</span></span>           | <span data-ttu-id="6ea9a-137">תאריך</span><span class="sxs-lookup"><span data-stu-id="6ea9a-137">Date</span></span>              | <span data-ttu-id="6ea9a-138">פורמטי התאריך נקבעים על פי הגדרת המשתמש **תאריך זמנים ופורמט מספרים** שמצוינת תחת **שפה והעדפת מדינה/אזור** ב- **אפשרויות משתמש**.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-138">Date formats are determined by the user's **Date, times, and number format** setting that is specified under **Language and country/region preference** in **User options**.</span></span> |
| <span data-ttu-id="6ea9a-139">4</span><span class="sxs-lookup"><span data-stu-id="6ea9a-139">4</span></span>           | <span data-ttu-id="6ea9a-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ea9a-140">Boolean</span></span>           | |
| <span data-ttu-id="6ea9a-141">15</span><span class="sxs-lookup"><span data-stu-id="6ea9a-141">15</span></span>          | <span data-ttu-id="6ea9a-142">GUID</span><span class="sxs-lookup"><span data-stu-id="6ea9a-142">GUID</span></span>              | |
| <span data-ttu-id="6ea9a-143">16</span><span class="sxs-lookup"><span data-stu-id="6ea9a-143">16</span></span>          | <span data-ttu-id="6ea9a-144">Int64</span><span class="sxs-lookup"><span data-stu-id="6ea9a-144">Int64</span></span>             | |

- <span data-ttu-id="6ea9a-145">אם המאפיין **stringOptions** אינו מסופק באובייקט **TSTimesheetCustomField**, שדה טקסט חופשי מסופק למשתמש.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-145">If the **stringOptions** property isn't provided on the **TSTimesheetCustomField** object, a free-text field is provided to the user.</span></span>

    <span data-ttu-id="6ea9a-146">ניתן להשתמש במאפיין **stringLength** כדי לקבוע את אורך המחרוזת המרבי שמשתמשים יכולים להזין.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-146">The **stringLength** property can be used to set the maximum string length that users can enter.</span></span>

- <span data-ttu-id="6ea9a-147">אם המאפיין **stringOptions** מסופק באובייקט **TSTimesheetCustomField**, הרכיבים שברשימה הם הערכים היחידים שמשתמשים יכולים לבחור באמצעות לחצני האפשרויות (לחצני הבחירה).</span><span class="sxs-lookup"><span data-stu-id="6ea9a-147">If the **stringOptions** property is provided on the **TSTimesheetCustomField** object, those list elements are the only values that users can select by using option buttons (radio buttons).</span></span>

    <span data-ttu-id="6ea9a-148">במקרה זה, שדה המחרוזת יכול לשמש כערך ספירה לצורך ערך המשתמש.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-148">In this case, the string field can act as an enum value for the purpose of user entry.</span></span> <span data-ttu-id="6ea9a-149">כדי לשמור את הערך למסד הנתונים כספירה, יש למפות את ערך המחרוזת באופן ידני בחזרה לערך ספירה לפני שמירתו במסד הנתונים באמצעות שרשרת הפקודה (עיין בסעיף "השתמש בשרשרת הפקודה במחלקה TSTimesheetEntryService כדי לשמור רשומת גליון זמנים מהאפליקציה חזרה למקטע מסד הנתונים בהמשך נושא זה לדוגמה).</span><span class="sxs-lookup"><span data-stu-id="6ea9a-149">To save the value to the database as an enum, manually map the string value back to the enum value before you save to the database by using chain of command (see the “Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database” section later in this topic for an example).</span></span>

### <a name="fieldextendedtype-tscustomfieldextendedtype"></a><span data-ttu-id="6ea9a-150">fieldExtendedType (TSCustomFieldExtendedType)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-150">fieldExtendedType (TSCustomFieldExtendedType)</span></span>

<span data-ttu-id="6ea9a-151">אתה יכול להשתמש במאפיין זה כדי לעצב ערכים אמיתיים כמטבע.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-151">You can use this property to format real values as currency.</span></span> <span data-ttu-id="6ea9a-152">גישה זו ישימה רק כאשר הערך **fieldBaseType** הוא **אמיתי**.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-152">This approach is applicable only when the **fieldBaseType** value is **Real**.</span></span>

- <span data-ttu-id="6ea9a-153">**TSCustomFieldExtendedType:ללא** – אין עיצוב מיושם.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-153">**TSCustomFieldExtendedType:None** – No formatting is applied.</span></span>
- <span data-ttu-id="6ea9a-154">**TSCustomFieldExtendedType::מטבע** – עצב את הערך כמטבע.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-154">**TSCustomFieldExtendedType::Currency** – Format the value as currency.</span></span>

    <span data-ttu-id="6ea9a-155">כאשר עיצוב מטבע פעיל, ניתן להשתמש בשדה **stringValue** כדי להעביר את קוד המטבע שאמור להיות מוצג באפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-155">When currency formatting is active, the **stringValue** field can be used pass the currency code that should be shown in the app.</span></span> <span data-ttu-id="6ea9a-156">הערך הוא ערך לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-156">The value is a read-only value.</span></span>

    <span data-ttu-id="6ea9a-157">השדה **realValue** מכיל את סכום הכסף שיש לשמור במסד הנתונים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-157">The **realValue** field contains the money amount that should be saved to the database.</span></span>

### <a name="fieldsection-tscustomfieldsection"></a><span data-ttu-id="6ea9a-158">fieldSection (TSCustomFieldSection)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-158">fieldSection (TSCustomFieldSection)</span></span>

<span data-ttu-id="6ea9a-159">תוכל להשתמש במאפיין זה כדי לציין היכן השדה המותאם אישית אמור להופיע באפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-159">You can use this property specify where the custom field should appear in the app.</span></span>

- <span data-ttu-id="6ea9a-160">**TSCustomFieldSection::כותרת** - השדה יופיע במקטע **צפה בפרטים נוספים** באפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-160">**TSCustomFieldSection::Header** – The field will appear in the **View more details** section in the app.</span></span> <span data-ttu-id="6ea9a-161">שדות אלה הם תמיד לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-161">These fields are always read-only.</span></span>
- <span data-ttu-id="6ea9a-162">**TSCustomFieldSection::שורה** – השדה יופיע אחרי כל שדות השורה המוכנים לשימוש בערכי גליונות הזמנים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-162">**TSCustomFieldSection::Line** – The field will appear after all the out-of-box line fields on timesheet entries.</span></span> <span data-ttu-id="6ea9a-163">שדות אלה יכולים להיות ניתנים לעריכה או לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-163">These fields can be either editable or read-only.</span></span>

### <a name="fieldname-fieldnameshort"></a><span data-ttu-id="6ea9a-164">fieldName (FieldNameShort)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-164">fieldName (FieldNameShort)</span></span>

<span data-ttu-id="6ea9a-165">מאפיין זה מזהה את השדה כאשר הערכים שהאפליקציה מספקת נשמרים בחזרה למסד הנתונים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-165">This property identifies the field when values that the app provides are saved back to the database.</span></span>

### <a name="tablename-tablenameshort"></a><span data-ttu-id="6ea9a-166">tableName (TableNameShort)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-166">tableName (TableNameShort)</span></span>

<span data-ttu-id="6ea9a-167">מאפיין זה מזהה את השדה כאשר הערכים שהאפליקציה מספקת נשמרים בחזרה למסד הנתונים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-167">This property identifies the field when values that the app provides are saved back to the database.</span></span>

### <a name="iseditable-noyes"></a><span data-ttu-id="6ea9a-168">isEditable (NoYes)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-168">isEditable (NoYes)</span></span>

<span data-ttu-id="6ea9a-169">הגדר מאפיין זה כ- **כן** כדי לציין שהמשתמש במקטע הזנת גיליונות זמנים צריך להיות ניתן לעריכה על ידי המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-169">Set this property to **Yes** to specify that the field in the timesheet entry section should be editable by users.</span></span> <span data-ttu-id="6ea9a-170">הגדר את הנכס כ- **לא** כדי להפוך את השדה לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-170">Set the property to **No** to make the field read-only.</span></span>

### <a name="ismandatory-noyes"></a><span data-ttu-id="6ea9a-171">isMandatory (NoYes)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-171">isMandatory (NoYes)</span></span>

<span data-ttu-id="6ea9a-172">הגדר מאפיין זה כ- **כן** כדי לציין שהשדה במקטע הזנת גיליונות זמנים צריך להיות שדה חובה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-172">Set this property to **Yes** to specify that the field in the timesheet entry section should be mandatory.</span></span>

### <a name="label-str"></a><span data-ttu-id="6ea9a-173">תווית (str)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-173">label (str)</span></span>

<span data-ttu-id="6ea9a-174">מאפיין זה מציין את התווית המוצגת ליד השדה באפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-174">This property specifies the label that is shown next the field in the app.</span></span>

### <a name="stringoptions-list-of-strings"></a><span data-ttu-id="6ea9a-175">stringOptions (רשימת מיתרים)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-175">stringOptions (List of Strings)</span></span>

<span data-ttu-id="6ea9a-176">מאפיין זה חל רק כאשר **fieldBaseType** נקבע ל **מיתר**.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-176">This property is applicable only when **fieldBaseType** is set to **String**.</span></span> <span data-ttu-id="6ea9a-177">אם מוגדר **stringOptions**, ערכי המחרוזת הזמינים לבחירה באמצעות לחצני האפשרויות (לחצני רדיו) מוגדרים על ידי המחרוזות ברשימה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-177">If **stringOptions** is set, the string values that are available for selection via option buttons (radio buttons) are specified by the strings in the list.</span></span> <span data-ttu-id="6ea9a-178">אם לא מסופקות מחרוזות, מותר להזין טקסט חופשי בשדה המחרוזת (עיין בסעיף "השתמש בשרשרת הפקודה במחלקה TSTimesheetEntryService כדי לשמור ערך של לוח זמנים מהאפליקציה חזרה למסד הנתונים" בהמשך נושא זה לדוגמה).</span><span class="sxs-lookup"><span data-stu-id="6ea9a-178">If no strings are provided, free-text entry in the string field is allowed (see the “Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database” section later in this topic for an example).</span></span>

### <a name="stringlength-int"></a><span data-ttu-id="6ea9a-179">stringLength (int)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-179">stringLength (int)</span></span>

<span data-ttu-id="6ea9a-180">מאפיין זה מציין את האורך המקסימלי עבור שדה מחרוזת.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-180">This property specifies the maximum length for a string field.</span></span> <span data-ttu-id="6ea9a-181">מאפיין זה חל רק כאשר **fieldBaseType** נקבע ל- **מיתר**.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-181">It's applicable only when **fieldBaseType** is set to **String**.</span></span>

### <a name="numberofdecimals-int"></a><span data-ttu-id="6ea9a-182">numberOfDecimals (int)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-182">numberOfDecimals (int)</span></span>

<span data-ttu-id="6ea9a-183">מאפיין זה מציין את מספר המקומות העשרוניים המוצגים עבור שדה אמיתי.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-183">This property specifies the number of decimal places that are shown for a real field.</span></span> <span data-ttu-id="6ea9a-184">מאפיין זה חל רק כאשר **fieldBaseType** נקבע ל- **אמיתי**.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-184">It's applicable only when **fieldBaseType** is set to **Real**.</span></span>

### <a name="ordersequence-int"></a><span data-ttu-id="6ea9a-185">orderSequence (int)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-185">orderSequence (int)</span></span>

<span data-ttu-id="6ea9a-186">מאפיין זה שולט בסדר הצגת השדות המותאמים אישית באפליקציה כאשר מוגדר יותר משדה מותאם אישית אחד.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-186">This property controls the order in which the custom fields are shown in the app when more than one custom field is specified.</span></span> <span data-ttu-id="6ea9a-187">תחילה מוצגים שדות בעלי מספרים נמוכים יותר.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-187">Fields that have lower numbers are shown first.</span></span>

### <a name="booleanvalue-boolean"></a><span data-ttu-id="6ea9a-188">booleanValue (בוליאני)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-188">booleanValue (boolean)</span></span>

<span data-ttu-id="6ea9a-189">עבור שדות מסוג **בוליאני**, מאפיין זה מעביר את הערך הבוליאני של השדה בין השרת לאפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-189">For fields of the **Boolean** type, this property passes the Boolean value of the field between the server and the app.</span></span>

### <a name="guidvalue-guid"></a><span data-ttu-id="6ea9a-190">guidValue (guid)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-190">guidValue (guid)</span></span>

<span data-ttu-id="6ea9a-191">עבור שדות מסוג **GUID‎**, מאפיין זה מעביר את הערך מזהה ייחודי כללי (GUID‎) של השדה בין השרת לאפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-191">For fields of the **GUID** type, this property passes the globally unique identifier (GUID) value of the field between the server and the app.</span></span>

### <a name="int64value-int64"></a><span data-ttu-id="6ea9a-192">int64Value (int64)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-192">int64Value (int64)</span></span>

<span data-ttu-id="6ea9a-193">עבור שדות מסוג **Int64**, מאפיין זה מעביר את הערך int64 של השדה בין השרת לאפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-193">For fields of the **Int64** type, this property passes the int64 value of the field between the server and the app.</span></span>

### <a name="intvalue-int"></a><span data-ttu-id="6ea9a-194">intValue (int)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-194">intValue (int)</span></span>

<span data-ttu-id="6ea9a-195">עבור שדות מסוג **Int**, מאפיין זה מעביר את הערך Int של השדה בין השרת לאפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-195">For fields of the **Int** type, this property passes the int value of the field between the server and the app.</span></span>

### <a name="realvalue-real"></a><span data-ttu-id="6ea9a-196">realValue (אמיתי)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-196">realValue (real)</span></span>

<span data-ttu-id="6ea9a-197">עבור שדות מסוג **אמיתי**, מאפיין זה מעביר את הערך 'אמיתי' של השדה בין השרת לאפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-197">For fields of the **Real** type, this property passes the real value of the field between the server and the app .</span></span>

### <a name="stringvalue-str"></a><span data-ttu-id="6ea9a-198">stringValue (str)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-198">stringValue (str)</span></span>

<span data-ttu-id="6ea9a-199">עבור שדות מסוג **מחרוזת**, מאפיין זה מעביר את הערך 'מחרוזת' של השדה בין השרת לאפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-199">For fields of the **String** type, this property passes the string value of the field between the server and the app.</span></span> <span data-ttu-id="6ea9a-200">הוא משמש גם לשדות של הסוג **אמיתי** המעוצב כמטבע.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-200">It's also used for fields of the **Real** type that are formatted as currency.</span></span> <span data-ttu-id="6ea9a-201">עבור שדות אלה, המאפיין משמש להעברת קוד המטבע לאפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-201">For those fields, the property is used to pass the currency code to the app.</span></span>

### <a name="datevalue-date"></a><span data-ttu-id="6ea9a-202">dateValue (תאריך)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-202">dateValue (date)</span></span>

<span data-ttu-id="6ea9a-203">עבור שדות מסוג **תאריך**, מאפיין זה מעביר את הערך 'תאריך' של השדה בין השרת לאפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-203">For fields of the **Date** type, this property passes the date value of the field between the server and the app.</span></span>

## <a name="show-and-save-a-custom-field-in-the-timesheet-entry-section"></a><span data-ttu-id="6ea9a-204">הצג שדה מותאם אישית במקטע הזנת גיליונות הזמנים ושמור אותו</span><span class="sxs-lookup"><span data-stu-id="6ea9a-204">Show and save a custom field in the timesheet entry section</span></span>

<span data-ttu-id="6ea9a-205">להלן צילום מסך מהאפליקציה למכשירים ניידים של יצירת ערכים בגיליונות זמנים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-205">Below is a screenshot from the mobile app of a timesheet entry creation.</span></span> <span data-ttu-id="6ea9a-206">הוא מציג את השדות המוכנים לשימוש ושדה מותאם אישית במקטע "ערך זמן" הנקרא "מחרוזת בדיקה" עם ערך ספירה של "אפשרות שנייה" שכבר הוגדר.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-206">It shows the out-of-box fields and a custom field in the "Time entry" section called "Test string" with an enum value of "Second option" already set.</span></span>

![שדה מותאם אישית של מחרוזת בדיקה באפליקציה](media/timesheet-entry.jpg)



<span data-ttu-id="6ea9a-208">להלן צילום מסך מהאפליקציה למכשירים ניידים של המשתמש בבחירת אחת מאפשרויות הספירה הזמינות עבור השדה המותאם אישית "מחרוזת בדיקה".</span><span class="sxs-lookup"><span data-stu-id="6ea9a-208">Below is a screenshot from the mobile app of the user selecting one of the enum options available for the "Test string" custom field.</span></span>  <span data-ttu-id="6ea9a-209">שתי האפשרויות הן "אפשרות ראשונה" ו"אפשרות שנייה" המוצגות ככפתורי בחירה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-209">The two options are "First option" and "Second option" shown as radio buttons.</span></span> <span data-ttu-id="6ea9a-210">האפשרות השנייה נבחרת כרגע.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-210">The second option is currently selected.</span></span>

![לחצני אפשרות (לחצני רדיו) עבור השדה המותאם אישית של מחרוזת בדיקה](media/enum-option.jpg)



### <a name="extend-the-tstimesheetline-table-so-that-it-has-a-custom-field"></a><span data-ttu-id="6ea9a-212">הרחב את הטבלה TSTimesheetLine כך שיהיה לה שדה מותאם אישית</span><span class="sxs-lookup"><span data-stu-id="6ea9a-212">Extend the TSTimesheetLine table so that it has a custom field</span></span>

<span data-ttu-id="6ea9a-213">בתרחישים נפוצים, סביר להניח שהנתונים עבור שדה מותאם אישית במקטע של ערך גיליונות הזמנים יישמרו בטבלת TSTimesheetLine.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-213">In typical scenarios, it's likely that the data for a custom field in the timesheet entry section will be saved to the TSTimesheetLine table.</span></span> <span data-ttu-id="6ea9a-214">עם זאת, ניתן להשתמש בטבלאות אחרות אם ניתן לאחזר את הנתונים על סמך רשומת TSTimesheetTrans המסופקת, או אם אין לו הקשר רשומות ספציפי (למשל, אם השדה מוגדר לקריאה בלבד בפרמטרים של הפרויקט) .</span><span class="sxs-lookup"><span data-stu-id="6ea9a-214">However, other tables can be used if the data can be retrieved based on a TSTimesheetTrans record that is provided, or if it doesn't have specific record context (for example, if the field is set as read-only in the project parameters).</span></span>

<span data-ttu-id="6ea9a-215">שים לב כי לשדות מותאמים אישית לא חייבים להיות רשומות בסיס נתונים כלשהן.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-215">Note that custom fields don't have to have any backing database records.</span></span> <span data-ttu-id="6ea9a-216">ניתן ליצור אותם באופן דינמי על סמך לוגיקה של X++‎.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-216">They can be dynamically generated based on X++ logic.</span></span> <span data-ttu-id="6ea9a-217">גישה זו יכולה להיות שימושית בתרחישים לקריאה בלבד (עיין במקטע "השתמש בשרשרת פקודה במחלקה TSTimesheetDetails, שיטת buildCustomFieldListForHeader למילוי פרטי גיליונות זמנים" כדוגמה לערכי שדות מותאמים אישית שנוצרו באופן דינמי.)</span><span class="sxs-lookup"><span data-stu-id="6ea9a-217">This approach can be useful in read-only scenarios (see the “Use chain of command on the TSTimesheetDetails class, buildCustomFieldListForHeader method to fill in timesheet details” section for an example of dynamically generated custom field values.)</span></span>

<span data-ttu-id="6ea9a-218">להלן צילום מסך מתוך Visual Studio של עץ אובייקט האפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-218">Below is a screenshot from Visual Studio of the Application Object Tree.</span></span> <span data-ttu-id="6ea9a-219">הוא מציג הרחבה של טבלת TSTimesheetLine כשהשדה TestLineString נוסף כשדה מותאם אישית.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-219">It shows an extension of the TSTimesheetLine table with the TestLineString field added as a custom field.</span></span>

![מחרוזת קו](media/b6756b4a3fc5298093327a088a7710fd.png)

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-timesheet-entry-section"></a><span data-ttu-id="6ea9a-221">השתמש בשרשרת הפקודה בשיטת buildCustomFieldList של המחלקה TSTimesheetSettings כדי להציג שדה במקטע ערך גיליונות.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-221">Use chain of command on the buildCustomFieldList method of the TSTimesheetSettings class to show a field in the timesheet entry section</span></span>

<span data-ttu-id="6ea9a-222">קוד זה שולט בהגדרות התצוגה של השדה באפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-222">This code controls the display settings for the field in the app.</span></span> <span data-ttu-id="6ea9a-223">לדוגמה, הוא שולט בסוג השדה, בתווית, האם השדה הוא חובה ובאיזה קטע השדה מופיע.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-223">For example, it controls the type of field, the label, whether the field is mandatory, and what section the field appears in.</span></span>

<span data-ttu-id="6ea9a-224">הדוגמה הבאה מציגה שדה מחרוזת בערכי זמן.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-224">The following example shows a string field on time entries.</span></span> <span data-ttu-id="6ea9a-225">לשדה זה שתי אפשרויות, **אפשרות ראשונה** ו- **אפשרות שנייה**, הזמינים באמצעות לחצני אפשרויות (לחצני רדיו).</span><span class="sxs-lookup"><span data-stu-id="6ea9a-225">This field has two options, **First option** and **Second option**, that are available via option buttons (radio buttons).</span></span> <span data-ttu-id="6ea9a-226">השדה באפליקציה משויך לשדה **TestLineString** שנוסף לטבלת TSTimesheetLine.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-226">The field in the app is associated with the **TestLineString** field that is added to the TSTimesheetLine table.</span></span>

<span data-ttu-id="6ea9a-227">שים לב לשימוש בשיטה **TSTimesheetCustomField::newFromMetatdata()** כדי לפשט את האתחול של מאפייני השדה המותאמים אישית: **fieldBaseType**, **tableName**, **fieldname**, **label**, **isEditable**, **isMandatory**, **stringLength** ו- **numberOfDecimals**.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-227">Note the use of the **TSTimesheetCustomField::newFromMetatdata()** method to simplify the initialization of the custom field properties: **fieldBaseType**, **tableName**, **fieldname**, **label**, **isEditable**, **isMandatory**, **stringLength**, and **numberOfDecimals**.</span></span> <span data-ttu-id="6ea9a-228">אתה יכול גם להגדיר פרמטרים אלה באופן ידני, לפי העדפתך.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-228">You can also set these parameters manually, as you prefer.</span></span>

```xpp
...
[ExtensionOf(classStr(TsTimesheetSettings))]
final class TSTimesheetSettings_Extension
{
    protected List buildCustomFieldList()
    {
        List customFieldList = next buildCustomFieldList();
        TSTimesheetCustomField tsTimesheetCustomField;
        tsTimesheetCustomField =
        TSTimesheetCustomField::newFromMetadata(tableNum(TsTimesheetLine),
        fieldNum(TSTimesheetLine, TestLineString));
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Line);
        tsTimesheetCustomField.parmOrderSequence(1);
        List stringOptions = new List(Types::String);
        stringOptions.addEnd('First option');
        stringOptions.addEnd('Second option');
        tsTimesheetCustomField.parmStringOptions(stringOptions);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforentry-method-of-the-tstimesheetentry-class-to-enter-values-in-a-timesheet-entry"></a><span data-ttu-id="6ea9a-229">השתמש בשרשרת הפקודה בשיטת buildCustomFieldListForEntry של המחלקה TSTimesheetEntry כדי להזין ערכים בערך גיליונות.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-229">Use chain of command on the buildCustomFieldListForEntry method of the TSTimesheetEntry class to enter values in a timesheet entry</span></span>

<span data-ttu-id="6ea9a-230">השיטה **buildCustomFieldListForEntry** משמשת להזנת ערכים בקווי הגליון השמורים באפליקציה למכשירים ניידים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-230">The **buildCustomFieldListForEntry** method is used to enter values on the saved timesheet lines in the mobile app.</span></span> <span data-ttu-id="6ea9a-231">נדרשת רשומת TSTimesheetTrans כפרמטר.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-231">It takes a TSTimesheetTrans record as a parameter.</span></span> <span data-ttu-id="6ea9a-232">ניתן להשתמש בשדות מאותה רשומה למילוי ערך השדה המותאם אישית באפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-232">Fields from that record can be used to fill in the custom field value in the app.</span></span>

```xpp
...
[ExtensionOf(classStr(TsTimesheetEntry))]
final class TsTimesheetEntry_Extension
{
    protected List buildCustomFieldListForEntry(TSTimesheetTrans _tsTimesheetTrans)
    {
        List customFieldList = next buildCustomFieldListForEntry(_tsTimesheetTrans);
        TSTimesheetLine tsTimesheetLine = _tsTimesheetTrans.timesheetLine();
        TSTimesheetCustomField tsTimesheetCustomField;
        tsTimesheetCustomField =
        TSTimesheetCustomField::newFromMetadata(tableNum(TsTimesheetLine),
        fieldNum(TSTimesheetLine, TestLineString));
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Line);
        tsTimesheetCustomField.parmOrderSequence(1);
        tsTimesheetCustomField.parmStringValue(tsTimesheetLine.TestLineString);
        List stringOptions = new List(Types::String);
        stringOptions.addEnd('First option');
        stringOptions.addEnd('second option;);
        tsTimesheetCustomField.parmStringOptions(stringOptions);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-tstimesheetentryservice-class-to-save-a-timesheet-entry-from-the-app-back-to-the-database"></a><span data-ttu-id="6ea9a-233">השתמש בשרשרת הפקודה במחלקה TSTimesheetEntryService כדי לשמור ערך גיליון זמנים מהאפליקציה בחזרה למסד הנתונים</span><span class="sxs-lookup"><span data-stu-id="6ea9a-233">Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database</span></span>

<span data-ttu-id="6ea9a-234">כדי לשמור שדה מותאם אישית בחזרה למסד הנתונים בשימוש אופייני, עליך להרחיב מספר שיטות:</span><span class="sxs-lookup"><span data-stu-id="6ea9a-234">To save a custom field back to the database in typical usage, you must extend multiple methods:</span></span>

- <span data-ttu-id="6ea9a-235">השיטה **timesheetLineNeedsUpdating** משמשת כדי לקבוע אם רשומת השורה שונתה על ידי המשתמש באפליקציה ויש לשמור אותה במסד הנתונים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-235">The **timesheetLineNeedsUpdating** method is used to determine whether the line record has been changed by the user in the app and must be saved to the database.</span></span> <span data-ttu-id="6ea9a-236">אם ביצועים אינם מהווים עניין, ניתן לפשט שיטה זו כך שתמיד תחזיר **true**.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-236">If performance isn't a concern, this method can be simplified so that it always returns **true**.</span></span>
- <span data-ttu-id="6ea9a-237">ניתן להרחיב את השיטות **populateTimesheetLineFromEntryDuringCreate** ו- **populateTimesheetLineFromEntryDuringUpdate** כך שהן מזינות ערכים ברשומת מסד הנתונים TSTimesheetLine מתוך רשומת חוזה הנתונים של TSTimesheetEntry המסופקת.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-237">The **populateTimesheetLineFromEntryDuringCreate** and **populateTimesheetLineFromEntryDuringUpdate** methods can be extended so that they enter values in the TSTimesheetLine database record from the TSTimesheetEntry data contract record that is provided.</span></span> <span data-ttu-id="6ea9a-238">בדוגמה הבאה, שים לב כיצד המיפוי בין שדה מסד הנתונים לשדה ההזנה נעשה באופן ידני באמצעות קוד X++‎.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-238">In the example that follows, notice how the mapping between the database field and the entry field is manually done via X++ code.</span></span>
- <span data-ttu-id="6ea9a-239">ניתן גם להרחיב את השיטה **populateTimesheetWeekFromEntry** אם השדה המותאם אישית שממופה לאובייקט **TSTimesheetEntry** חייב לכתוב חזרה לטבלת מסד הנתונים TSTimesheetLineweek.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-239">The **populateTimesheetWeekFromEntry** method can also be extended if the custom field that is mapped to the **TSTimesheetEntry** object must write back to the TSTimesheetLineweek database table.</span></span>

> [!NOTE]
> <span data-ttu-id="6ea9a-240">הדוגמה הבאה שומרת את הערך **firstOption** או **secondOption** שהמשתמש בוחר למסד הנתונים כערך מחרוזת גולמי.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-240">The following example saves the **firstOption** or **secondOption** value that the user selects to the database as a raw string value.</span></span> <span data-ttu-id="6ea9a-241">אם שדה מסד הנתונים הוא שדה מסוג **ספירה**, ניתן למפות ידנית את הערכים לערך ספירה ואז לשמור אותם בשדה ספירה בטבלת מסד הנתונים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-241">If the database field is a field of the **Enum** type, those values can be manually mapped to an enum value and then saved to an enum field on the database table.</span></span>

```xpp
...
[ExtensionOf(classStr(TSTimesheetEntryService))]
final class TSTimesheetEntryService_Extension
{
    protected boolean timesheetLineNeedsUpdating(TSTimesheetLine _tsTimesheetLine,
    TsTimesheetEntry _tsTimesheetEntry)
    {
        boolean ret = next timesheetLineNeedsUpdating(_tsTimesheetLine,
        _tsTimesheetEntry);
        if (!ret)
        {
            */ Loop through custom fields to see if value needs updating*/
            ListEnumerator enumerator =  _tsTimesheetEntry.parmCustomFields().getEnumerator();
            while (enumerator.moveNext())
            {
                TSTimesheetCustomField customField = enumerator.current();
                if (customField.parmFieldName() == fieldId2Name(tableNum(TsTimesheetLine),
                fieldNum(TSTimesheetLine, TestLineString)))
                {
                    */ If Custom field value for TestLineString field has changed, We need to update the timesheet line.*/
                    if (_tsTimesheetLine.TestLineString != customField.parmStringValue())
                    {
                        ret = true;
                    }
                }
            }
        }
        return ret;
    }
    protected void populateTimesheetLineFromEntryDuringCreate(TSTimesheetLine
    _tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
    {
        next populateTimesheetLineFromEntryDuringCreate(_tsTimesheetLine,
        _tsTimesheetEntry);
        this.populateTimesheetLineFromCustomFields(_tsTimesheetLine,
        _tsTimesheetEntry);
        }
        protected void populateTimesheetLineFromEntryDuringUpdate(TSTimesheetLine
        \_tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
        {
            next populateTimesheetLineFromEntryDuringUpdate(_tsTimesheetLine,
            _tsTimesheetEntry);
            this.populateTimesheetLineFromCustomFields(_tsTimesheetLine,
            _tsTimesheetEntry);
        }
        private void populateTimesheetLineFromCustomFields(TSTimesheetLine
        _tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
        {
            ListEnumerator enumerator =
            _tsTimesheetEntry.parmCustomFields().getEnumerator();
            while (enumerator.moveNext())
            {
                TSTimesheetCustomField customField = enumerator.current();
                if (customField.parmFieldName() == fieldId2Name(tableNum(TsTimesheetLine),
                fieldNum(TSTimesheetLine, TestLineString)))
                {
                    _tsTimesheetLine.TestLineString = customField.parmStringValue();
                }
            }
        }
    }
...
```

## <a name="show-a-custom-field-in-the-timesheet-header-section"></a><span data-ttu-id="6ea9a-242">הצג שדה מותאם אישית במקטע כותרת גיליונות הזמנים ושמור אותו</span><span class="sxs-lookup"><span data-stu-id="6ea9a-242">Show a custom field in the timesheet header section</span></span>

<span data-ttu-id="6ea9a-243">להלן צילום מסך מהאפליקציה למכשירים ניידים של משתמש המציג גיליון זמנים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-243">Below is a screenshot from the mobile app of a user viewing a timesheet.</span></span> <span data-ttu-id="6ea9a-244">הלחצן "מידע נוסף" נבחר בפינה השמאלית העליונה כדי להציג את האפשרות "הצג פרטים נוספים".</span><span class="sxs-lookup"><span data-stu-id="6ea9a-244">The "More information" button has been selected in the upper-right corner to show the "View more details" option.</span></span>  

![הצג פקודה של פרטים נוספים](media/show-more.png)

<span data-ttu-id="6ea9a-246">להלן צילום מסך מהאפליקציה למכשירים ניידים המציג את המקטע "עוד" של גיליון זמנים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-246">Below is a screenshot from the mobile app showing the “More” section of a timesheet.</span></span> <span data-ttu-id="6ea9a-247">שדה מותאם אישית בשם "קצב ניצול של גיליון זמנים זה (שדה מותאם אישית מחושב)" נוסף למקטע כותרת גיליון הזמנים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-247">A custom field called “Utilization rate of this timesheet (computed custom field)” has been added to the timesheet header section.</span></span> <span data-ttu-id="6ea9a-248">ערך לקריאה בלבד של "0.667" מוגדר בשדה המותאם אישית.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-248">A read-only value of "0.667" is set on the custom field.</span></span>

![מקטע נוסף](media/more-section.jpg)

### <a name="extend-the-tstimesheettable-table-so-that-it-has-a-custom-field"></a><span data-ttu-id="6ea9a-250">הרחב את הטבלה TSTimesheetTable כך שיהיה לה שדה מותאם אישית</span><span class="sxs-lookup"><span data-stu-id="6ea9a-250">Extend the TSTimesheetTable table so that it has a custom field</span></span>

<span data-ttu-id="6ea9a-251">בתרחישים נפוצים, סביר להניח שהנתונים עבור שדה מותאם אישית במקטע הכותרת יגיעו מהטבלה TSTimesheetHeader.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-251">In typical scenarios, it's likely that the data for a custom field in the header section will be pulled from the TSTimesheetHeader table.</span></span> <span data-ttu-id="6ea9a-252">עם זאת, ניתן להשתמש בטבלאות אחרות אם ניתן לאחזר את הנתונים על סמך רשומת TSTimesheetTable המסופקת, או אם אין לו הקשר רשומות ספציפי (למשל, אם השדה מוגדר לקריאה בלבד בפרמטרים של הפרויקט).</span><span class="sxs-lookup"><span data-stu-id="6ea9a-252">However, other tables can be used if the data can be retrieved based on a TSTimesheetTable record that is provided, or if it doesn't have specific record context (for example, if the field is set as read-only in the project parameters).</span></span>

<span data-ttu-id="6ea9a-253">שים לב כי לשדות מותאמים אישית לא חייבים להיות רשומות בסיס נתונים כלשהן.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-253">Note that custom fields don't have to have any backing database records.</span></span> <span data-ttu-id="6ea9a-254">ניתן ליצור אותם באופן דינמי על סמך לוגיקה של X++‎.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-254">They can be dynamically generated based on X++ logic.</span></span> <span data-ttu-id="6ea9a-255">הדוגמה הבאה מציגה גישה זו.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-255">The example that follows shows this approach.</span></span>

<span data-ttu-id="6ea9a-256">שדות במקטע הכותרת נחשבים תמיד כקריאה בלבד באפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-256">Fields in the header section are always read-only in the app.</span></span>

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-header-section"></a><span data-ttu-id="6ea9a-257">השתמש בשרשרת הפקודה בשיטת buildCustomFieldList של המחלקה TSTimesheetSettings כדי להציג שדה במקטע הכותרת</span><span class="sxs-lookup"><span data-stu-id="6ea9a-257">Use chain of command on the buildCustomFieldList method of the TSTimesheetSettings class to show a field in the header section</span></span>

<span data-ttu-id="6ea9a-258">קוד זה שולט בהגדרות התצוגה של השדה באפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-258">This code controls the display settings for the field in the app.</span></span> <span data-ttu-id="6ea9a-259">לדוגמה, הוא שולט בסוג השדה, בתווית, האם השדה הוא חובה ובאיזה קטע השדה מופיע.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-259">For example, it controls the type of field, the label, whether the field is mandatory, and what section the field appears in.</span></span>

<span data-ttu-id="6ea9a-260">הדוגמה הבאה מציגה ערך מחושב במקטע הכותרת באפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-260">The following example shows a computed value in the header section in the app.</span></span>

```xpp
...
[ExtensionOf(classStr(TsTimesheetSettings))]
final class TSTimesheetSettings_Extension
{
    protected List buildCustomFieldList()
    {
        List customFieldList = next buildCustomFieldList();
        TSTimesheetCustomField tsTimesheetCustomField;

        */ Computed utilization rate*/
        tsTimesheetCustomField = new TSTimesheetCustomField();
        tsTimesheetCustomField.parmFieldBaseType(Types::Real);
        tsTimesheetCustomField.parmLabel("Utilization rate of this timesheet (computed
        custom field)");
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Header);
        tsTimesheetCustomField.parmOrderSequence(2);
        tsTimesheetCustomField.parmNumberOfDecimals(3);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforheader-method-of-the-tstimesheetdetails-class-to-fill-in-timesheet-details"></a><span data-ttu-id="6ea9a-261">השתמש בשרשרת הפקודה בשיטת buildCustomFieldListForHeader של המחלקה TSTimesheetDetails כדי למלא פרטים בגיליון הזמנים</span><span class="sxs-lookup"><span data-stu-id="6ea9a-261">Use chain of command on the buildCustomFieldListForHeader method of the TSTimesheetDetails class to fill in timesheet details</span></span>

<span data-ttu-id="6ea9a-262">השיטה **buildCustomFieldListForHeader** משמשת למילוי פרטי כותרת גיליון הזמנים באפליקציה למכשירים ניידים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-262">The **buildCustomFieldListForHeader** method is used to fill in the timesheet header details in the mobile app.</span></span> <span data-ttu-id="6ea9a-263">נדרשת רשומת TSTimesheetTable כפרמטר.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-263">It takes a TSTimesheetTable record as a parameter.</span></span> <span data-ttu-id="6ea9a-264">ניתן להשתמש בשדות מאותה רשומה למילוי ערך השדה המותאם אישית באפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-264">Fields from that record can be used to fill in the custom field value in the app.</span></span> <span data-ttu-id="6ea9a-265">הדוגמה הבאה לא קוראת שום ערך ממסד הנתונים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-265">The following example doesn't read any values from the database.</span></span> <span data-ttu-id="6ea9a-266">במקום זאת, היא משתמשת בלוגיקת X++‎ כדי ליצור ערך מחושב שלאחר מכן מוצג באפליקציה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-266">Instead, it uses X++ logic to generate a computed value that is then shown in the app.</span></span>


```xpp
...
[ExtensionOf(classStr(TSTimesheetDetails))]
final class TSTimesheetDetails_Extension
{
    protected List buildCustomFieldListForHeader(TSTimesheetTable
    _tsTimesheetTable)
    {
        List customFieldList = next buildCustomFieldListForHeader(_tsTimesheetTable);
        TSTimesheetCustomField tsTimesheetCustomField;

        */ Computed utilization rate*/
        tsTimesheetCustomField = new TSTimesheetCustomField();
        tsTimesheetCustomField.parmFieldBaseType(Types::Real);
        tsTimesheetCustomField.parmLabel("Utilization rate of this timesheet (computed
        custom field)");
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Header);
        tsTimesheetCustomField.parmOrderSequence(2);
        tsTimesheetCustomField.parmNumberOfDecimals(3);
        real utilizationRate = 0;
        if (_tsTimesheetTable.totalHours() != 0)
        {
            utilizationRate = _tsTimesheetTable.totalHoursBillable() /
            _tsTimesheetTable.totalHours();
        }
        tsTimesheetCustomField.parmRealValue(utilizationRate);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

## <a name="other-configurabilityextensibility-opportunities"></a><span data-ttu-id="6ea9a-267">הזדמנויות להגדרה / הרחבה אחרות</span><span class="sxs-lookup"><span data-stu-id="6ea9a-267">Other configurability/extensibility opportunities</span></span>

### <a name="adding-additional-validation-for-the-app"></a><span data-ttu-id="6ea9a-268">הוספת אימות נוסף לאפליקציה</span><span class="sxs-lookup"><span data-stu-id="6ea9a-268">Adding additional validation for the app</span></span>

<span data-ttu-id="6ea9a-269">לוגיקה קיימת לפונקציונליות של גיליון זמנים ברמת מסד הנתונים עדיין תפעל כצפוי.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-269">Existing logic for timesheet functionality at the database level will still work as expected.</span></span> <span data-ttu-id="6ea9a-270">כדי להפריע להשלמת השמירה או שליחת פעולות וכדי להציג הודעת שגיאה ספציפית, אתה יכול להוסיף **שגיאת זריקה ("הודעה למשתמש")** לקוד באמצעות שרשרת של סיומת פקודה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-270">To interrupt the completion of save or submit operations and show a specific error message, you can add **throw error("message to user")** to the code via a chain of command extension.</span></span> <span data-ttu-id="6ea9a-271">להלן שלוש דוגמאות לשיטות הניתנות להרחבה:</span><span class="sxs-lookup"><span data-stu-id="6ea9a-271">Here are three examples of useful extensible methods:</span></span>

- <span data-ttu-id="6ea9a-272">אם **validateWrite** בטבלה TSTimesheetLine מחזיר **false** במהלך פעולת שמירה עבור שורה בגיליון זמנים, הודעת שגיאה מוצגת באפליקציה למכשירים ניידים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-272">If **validateWrite** on the TSTimesheetLine table returns **false** during a save operation for a timesheet line, an error message is shown in the mobile app.</span></span>
- <span data-ttu-id="6ea9a-273">אם **validateSubmit** בטבלה TSTimesheetTable מחזיר **false** במהלך שליחת גיליון זמנים באפליקציה, הודעת שגיאה מוצגת למשתמש.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-273">If **validateSubmit** on the TSTimesheetTable table returns **false** during timesheet submission in the app, an error message is shown to the user.</span></span>
- <span data-ttu-id="6ea9a-274">לוגיקה שממלאת שדות (למשל, **מאפיין שורה**) במהלך שיטת **insert** בטבלת TSTimesheetLine עדיין תפעל.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-274">Logic that fills in fields (for example, **Line Property**) during the **insert** method on the TSTimesheetLine table will still run.</span></span>

### <a name="hiding-and-marking-out-of-box-fields-as-read-only-via-configuration"></a><span data-ttu-id="6ea9a-275">הסתרה וסימון שדות מוכנים לשימוש כקריאה בלבד באמצעות הגדרת תצורה</span><span class="sxs-lookup"><span data-stu-id="6ea9a-275">Hiding and marking out-of-box fields as read-only via configuration</span></span>

<span data-ttu-id="6ea9a-276">מהפרמטרים של הפרויקט, באפשרותך להפוך שדות מוכנים לשימוש לקריאה בלבד או מוסתרים באפליקציה למכשירים ניידים.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-276">From the project parameters, you can make out-of-box fields read-only or hidden in the mobile app.</span></span> <span data-ttu-id="6ea9a-277">הגדר את האפשרויות במקטע **גיליונות זמנים לנייד** בכרטיסייה **גיליון זמנים** של הדף **ניהול פרויקטים ופרמטרים חשבונאיים**.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-277">Set the options in the **Mobile timesheets** section on the **Timesheet** tab of the **Project management and accounting parameters** page.</span></span>

![פרמטרים של פרויקט](media/5753b8ecccd1d8bb2b002dd538b3f762.png)

### <a name="changing-the-activities-that-are-available-for-selection-via-extensions"></a><span data-ttu-id="6ea9a-279">שינוי הפעילויות הזמינות לבחירה באמצעות הרחבות</span><span class="sxs-lookup"><span data-stu-id="6ea9a-279">Changing the activities that are available for selection via extensions</span></span>

<span data-ttu-id="6ea9a-280">הפעילויות הזמינות לבחירה לפרויקט מתמלאות באמצעות השיטות **getActivitiesForProject ()** ו- **getActivityQuery ()** במחלקה **TsTimesheetProjectService**.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-280">The activities that are available for selection for a project are filled in via the **getActivitiesForProject()** and **getActivityQuery()** methods in the **TsTimesheetProjectService** class.</span></span> <span data-ttu-id="6ea9a-281">באפשרותך להשתמש בשרשרת הפקודה כדי לשנות התנהגות זו כך שתתאים לתרחיש העסקי שלך לפעילויות הזמינות לבחירה עבור פרויקט ספציפי.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-281">You can use chain of command to change this behavior to match your business scenario for the activities that are available for selection for a specific project.</span></span>

### <a name="entering-a-default-project-category-on-timesheet-entries"></a><span data-ttu-id="6ea9a-282">הזנת קטגוריית ברירת מחדל של פרויקט בערכי גיליון זמנים</span><span class="sxs-lookup"><span data-stu-id="6ea9a-282">Entering a default project category on timesheet entries</span></span>

<span data-ttu-id="6ea9a-283">הזנת קטגוריית ברירת מחדל של פרויקט בערכי גיליון זמנים מתרחשת בשלוש רמות.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-283">Entry of a default project category on timesheet entries occurs at three levels.</span></span> <span data-ttu-id="6ea9a-284">אתה יכול להשתמש בשרשרת הפקודה כדי להרחיב את ההתנהגות בכל אחת מהרמות הללו או בכולן כדי להשיג את ההתנהגות הרצויה.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-284">You can use chain of command to extend the behavior at any or all of these levels to achieve the desired behavior.</span></span> <span data-ttu-id="6ea9a-285">נעשה שימוש בהיררכיה הבאה:</span><span class="sxs-lookup"><span data-stu-id="6ea9a-285">The following hierarchy is used:</span></span>

1. <span data-ttu-id="6ea9a-286">האפליקציה מנסה להציב את קטגוריית ברירת המחדל ממשאב הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-286">The app tries to put the default category from the project resource.</span></span> <span data-ttu-id="6ea9a-287">קטגוריית ברירת מחדל זו מוגדרת בשיטות **getCurrentUserResource** ו- **getDelegatedResourcesForCurrentUser** במחלקה **TSTimesheetSettingsService**.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-287">This default category is set in the **getCurrentUserResource** and **getDelegatedResourcesForCurrentUser** methods in the **TSTimesheetSettingsService** class.</span></span>
2. <span data-ttu-id="6ea9a-288">אם קטגוריית ברירת המחדל אינה מסופקת ברמת משאבי הפרויקט, האפליקציה מנסה לשלוף אותה מפעילות הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-288">If the default category isn't provided at the project resource level, the app tries to pull it from the project activity.</span></span> <span data-ttu-id="6ea9a-289">קטגוריית ברירת מחדל זו מוגדרת בשיטה **getActivitiesForProject** שבמחלקה **TSTimesheetProjectService**.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-289">This default category is set in the **getActivitiesForProject** method in the **TSTimesheetProjectService** class.</span></span>
3. <span data-ttu-id="6ea9a-290">אם קטגוריית ברירת המחדל אינה מסופקת ברמת פעילות הפרויקט, קטגוריית ברירת המחדל נשלפת מפרמטרי הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-290">If the default category isn't provided at the project activity level, the default category it taken from the project parameters.</span></span> <span data-ttu-id="6ea9a-291">קטגוריית ברירת מחדל זו מוגדרת בשיטה **getProjectDetailsbyRule** שבמחלקה **TSTimesheetProjectService**.</span><span class="sxs-lookup"><span data-stu-id="6ea9a-291">This default category is set in the **getProjectDetailsbyRule** method in the **TSTimesheetProjectService** class.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]