---
title: יישם שדות מותאמים אישית עבור האפליקציה למכשירים ניידים Microsoft Dynamics 365 Project Timesheet ב- iOS וב- Android
description: נושא זה מספק דפוסים נפוצים לשימוש בתוספים לצורך יישום שדות מותאמים אישית.
author: Yowelle
manager: AnnBe
ms.date: 05/29/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
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
ms.openlocfilehash: 5dae571fce746b49281587f5349774a7f2c4111b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5270994"
---
# <a name="implement-custom-fields-for-the-microsoft-dynamics-365-project-timesheet-mobile-app-on-ios-and-android"></a>יישם שדות מותאמים אישית עבור האפליקציה למכשירים ניידים Microsoft Dynamics 365 Project Timesheet ב- iOS וב- Android

[!include [banner](../includes/banner.md)]

נושא זה מספק דפוסים נפוצים לשימוש בתוספים לצורך יישום שדות מותאמים אישית. אלו הנושאים שמאמר זה סוקר:

- סוגי הנתונים השונים שמסגרת השדה המותאמת אישית תומכת בהם
- כיצד להציג שדות לקריאה בלבד או לעריכה בערכי גליון הזמנים, ולשמור ערכים המסופקים על ידי המשתמש בחזרה למסד הנתונים
- כיצד להציג שדות לקריאה בלבד בכותרת גליון הזמנים
- כיצד לשלב לוגיקה עסקית מותאמת אישית אחרת כדי להזין ערכי ברירת מחדל בשדות ולבצע אימות נוסף

## <a name="audience"></a>קהל

הנושא מיועד למפתחים שמשלבים את השדות המותאמים אישית שלהם באפליקציה למכשירים ניידים Microsoft Dynamics 365 Project Timesheet הזמינה עבור Apple iOS ו- Google Android. ההנחה היא שהקוראים מכירים את הפיתוח של X++‎ ואת פונקציונליות לוח הזמנים של הפרויקט.

## <a name="data-contract--tstimesheetcustomfield-x-class"></a>חוזה נתונים - מחלקת TSTimesheetCustomField X++‎

מחלקת **TSTimesheetCustomField‎** היא מחלקת חוזה הנתונים X++‎ המייצגת מידע אודות שדה מותאם אישית לפונקציונליות של לוח הזמנים. רשימות של אובייקטים בשדה המותאם אישית מועברות הן בחוזה הנתונים TSTimesheetDetails והן בחוזה הנתונים TSTimesheetEntry כדי להציג שדות מותאמים אישית באפליקציה למכשירים ניידים.

- **TSTimesheetDetails** - חוזה כותרת של גליון הזמנים.
- **TSTimesheetEntry** - חוזה העסקה בגליון הזמנים. קבוצות של אובייקטים אלה שיש להם את אותו מידע על הפרויקט וערך **timesheetLineRecId** מהווה שורה.

### <a name="fieldbasetype-types"></a>fieldBaseType (סוגים)

המאפיין **FieldBaseType** שעל אובייקט **TsTimesheetCustom** קובע את סוג השדה שמופיע באפליקציה. הערכים **סוגים** הבאים שנתמכים.

| ערך סוגים | סוג              | הערות |
|-------------|-------------------|-------|
| 1           | מחרוזת (וספירה) | השדה מופיע כשדה טקסט. |
| 1           | Integer           | הערך מוצג כמספר ללא מקומות עשרוניים. |
| 2           | אמיתי              | הערך מוצג כמספר עם מקומות עשרוניים.<p>כדי להציג את הערך האמיתי כמטבע באפליקציה, השתמש בתוכנה **fieldExtenededType**. אתה יכול להשתמש במאפיין **numberOfDecimals** כדי לקבוע את מספר המקומות העשרוניים המוצגים.</p> |
| 3           | תאריך              | פורמטי התאריך נקבעים על פי הגדרת המשתמש **תאריך זמנים ופורמט מספרים** שמצוינת תחת **שפה והעדפת מדינה/אזור** ב- **אפשרויות משתמש**. |
| 4           | Boolean           | |
| 15          | GUID              | |
| 16          | Int64             | |

- אם המאפיין **stringOptions** אינו מסופק באובייקט **TSTimesheetCustomField**, שדה טקסט חופשי מסופק למשתמש.

    ניתן להשתמש במאפיין **stringLength** כדי לקבוע את אורך המחרוזת המרבי שמשתמשים יכולים להזין.

- אם המאפיין **stringOptions** מסופק באובייקט **TSTimesheetCustomField**, הרכיבים שברשימה הם הערכים היחידים שמשתמשים יכולים לבחור באמצעות לחצני האפשרויות (לחצני הבחירה).

    במקרה זה, שדה המחרוזת יכול לשמש כערך ספירה לצורך ערך המשתמש. כדי לשמור את הערך למסד הנתונים כספירה, יש למפות את ערך המחרוזת באופן ידני בחזרה לערך ספירה לפני שמירתו במסד הנתונים באמצעות שרשרת הפקודה (עיין בסעיף "השתמש בשרשרת הפקודה במחלקה TSTimesheetEntryService כדי לשמור רשומת גליון זמנים מהאפליקציה חזרה למקטע מסד הנתונים בהמשך נושא זה לדוגמה).

### <a name="fieldextendedtype-tscustomfieldextendedtype"></a>fieldExtendedType (TSCustomFieldExtendedType)

אתה יכול להשתמש במאפיין זה כדי לעצב ערכים אמיתיים כמטבע. גישה זו ישימה רק כאשר הערך **fieldBaseType** הוא **אמיתי**.

- **TSCustomFieldExtendedType:ללא** – אין עיצוב מיושם.
- **TSCustomFieldExtendedType::מטבע** – עצב את הערך כמטבע.

    כאשר עיצוב מטבע פעיל, ניתן להשתמש בשדה **stringValue** כדי להעביר את קוד המטבע שאמור להיות מוצג באפליקציה. הערך הוא ערך לקריאה בלבד.

    השדה **realValue** מכיל את סכום הכסף שיש לשמור במסד הנתונים.

### <a name="fieldsection-tscustomfieldsection"></a>fieldSection (TSCustomFieldSection)

תוכל להשתמש במאפיין זה כדי לציין היכן השדה המותאם אישית אמור להופיע באפליקציה.

- **TSCustomFieldSection::כותרת** - השדה יופיע במקטע **צפה בפרטים נוספים** באפליקציה. שדות אלה הם תמיד לקריאה בלבד.
- **TSCustomFieldSection::שורה** – השדה יופיע אחרי כל שדות השורה המוכנים לשימוש בערכי גליונות הזמנים. שדות אלה יכולים להיות ניתנים לעריכה או לקריאה בלבד.

### <a name="fieldname-fieldnameshort"></a>fieldName (FieldNameShort)

מאפיין זה מזהה את השדה כאשר הערכים שהאפליקציה מספקת נשמרים בחזרה למסד הנתונים.

### <a name="tablename-tablenameshort"></a>tableName (TableNameShort)

מאפיין זה מזהה את השדה כאשר הערכים שהאפליקציה מספקת נשמרים בחזרה למסד הנתונים.

### <a name="iseditable-noyes"></a>isEditable (NoYes)

הגדר מאפיין זה כ- **כן** כדי לציין שהמשתמש במקטע הזנת גיליונות זמנים צריך להיות ניתן לעריכה על ידי המשתמשים. הגדר את הנכס כ- **לא** כדי להפוך את השדה לקריאה בלבד.

### <a name="ismandatory-noyes"></a>isMandatory (NoYes)

הגדר מאפיין זה כ- **כן** כדי לציין שהשדה במקטע הזנת גיליונות זמנים צריך להיות שדה חובה.

### <a name="label-str"></a>תווית (str)

מאפיין זה מציין את התווית המוצגת ליד השדה באפליקציה.

### <a name="stringoptions-list-of-strings"></a>stringOptions (רשימת מיתרים)

מאפיין זה חל רק כאשר **fieldBaseType** נקבע ל **מיתר**. אם מוגדר **stringOptions**, ערכי המחרוזת הזמינים לבחירה באמצעות לחצני האפשרויות (לחצני רדיו) מוגדרים על ידי המחרוזות ברשימה. אם לא מסופקות מחרוזות, מותר להזין טקסט חופשי בשדה המחרוזת (עיין בסעיף "השתמש בשרשרת הפקודה במחלקה TSTimesheetEntryService כדי לשמור ערך של לוח זמנים מהאפליקציה חזרה למסד הנתונים" בהמשך נושא זה לדוגמה).

### <a name="stringlength-int"></a>stringLength (int)

מאפיין זה מציין את האורך המקסימלי עבור שדה מחרוזת. מאפיין זה חל רק כאשר **fieldBaseType** נקבע ל- **מיתר**.

### <a name="numberofdecimals-int"></a>numberOfDecimals (int)

מאפיין זה מציין את מספר המקומות העשרוניים המוצגים עבור שדה אמיתי. מאפיין זה חל רק כאשר **fieldBaseType** נקבע ל- **אמיתי**.

### <a name="ordersequence-int"></a>orderSequence (int)

מאפיין זה שולט בסדר הצגת השדות המותאמים אישית באפליקציה כאשר מוגדר יותר משדה מותאם אישית אחד. תחילה מוצגים שדות בעלי מספרים נמוכים יותר.

### <a name="booleanvalue-boolean"></a>booleanValue (בוליאני)

עבור שדות מסוג **בוליאני**, מאפיין זה מעביר את הערך הבוליאני של השדה בין השרת לאפליקציה.

### <a name="guidvalue-guid"></a>guidValue (guid)

עבור שדות מסוג **GUID‎**, מאפיין זה מעביר את הערך מזהה ייחודי כללי (GUID‎) של השדה בין השרת לאפליקציה.

### <a name="int64value-int64"></a>int64Value (int64)

עבור שדות מסוג **Int64**, מאפיין זה מעביר את הערך int64 של השדה בין השרת לאפליקציה.

### <a name="intvalue-int"></a>intValue (int)

עבור שדות מסוג **Int**, מאפיין זה מעביר את הערך Int של השדה בין השרת לאפליקציה.

### <a name="realvalue-real"></a>realValue (אמיתי)

עבור שדות מסוג **אמיתי**, מאפיין זה מעביר את הערך 'אמיתי' של השדה בין השרת לאפליקציה.

### <a name="stringvalue-str"></a>stringValue (str)

עבור שדות מסוג **מחרוזת**, מאפיין זה מעביר את הערך 'מחרוזת' של השדה בין השרת לאפליקציה. הוא משמש גם לשדות של הסוג **אמיתי** המעוצב כמטבע. עבור שדות אלה, המאפיין משמש להעברת קוד המטבע לאפליקציה.

### <a name="datevalue-date"></a>dateValue (תאריך)

עבור שדות מסוג **תאריך**, מאפיין זה מעביר את הערך 'תאריך' של השדה בין השרת לאפליקציה.

## <a name="show-and-save-a-custom-field-in-the-timesheet-entry-section"></a>הצג שדה מותאם אישית במקטע הזנת גיליונות הזמנים ושמור אותו

להלן צילום מסך מהאפליקציה למכשירים ניידים של יצירת ערכים בגיליונות זמנים. הוא מציג את השדות המוכנים לשימוש ושדה מותאם אישית במקטע "ערך זמן" הנקרא "מחרוזת בדיקה" עם ערך ספירה של "אפשרות שנייה" שכבר הוגדר.

![שדה מותאם אישית של מחרוזת בדיקה באפליקציה](media/timesheet-entry.jpg)



להלן צילום מסך מהאפליקציה למכשירים ניידים של המשתמש בבחירת אחת מאפשרויות הספירה הזמינות עבור השדה המותאם אישית "מחרוזת בדיקה".  שתי האפשרויות הן "אפשרות ראשונה" ו"אפשרות שנייה" המוצגות ככפתורי בחירה. האפשרות השנייה נבחרת כרגע.

![לחצני אפשרות (לחצני רדיו) עבור השדה המותאם אישית של מחרוזת בדיקה](media/enum-option.jpg)



### <a name="extend-the-tstimesheetline-table-so-that-it-has-a-custom-field"></a>הרחב את הטבלה TSTimesheetLine כך שיהיה לה שדה מותאם אישית

בתרחישים נפוצים, סביר להניח שהנתונים עבור שדה מותאם אישית במקטע של ערך גיליונות הזמנים יישמרו בטבלת TSTimesheetLine. עם זאת, ניתן להשתמש בטבלאות אחרות אם ניתן לאחזר את הנתונים על סמך רשומת TSTimesheetTrans המסופקת, או אם אין לו הקשר רשומות ספציפי (למשל, אם השדה מוגדר לקריאה בלבד בפרמטרים של הפרויקט) .

שים לב כי לשדות מותאמים אישית לא חייבים להיות רשומות בסיס נתונים כלשהן. ניתן ליצור אותם באופן דינמי על סמך לוגיקה של X++‎. גישה זו יכולה להיות שימושית בתרחישים לקריאה בלבד (עיין במקטע "השתמש בשרשרת פקודה במחלקה TSTimesheetDetails, שיטת buildCustomFieldListForHeader למילוי פרטי גיליונות זמנים" כדוגמה לערכי שדות מותאמים אישית שנוצרו באופן דינמי.)

להלן צילום מסך מתוך Visual Studio של עץ אובייקט האפליקציה. הוא מציג הרחבה של טבלת TSTimesheetLine כשהשדה TestLineString נוסף כשדה מותאם אישית.

![מחרוזת קו](media/b6756b4a3fc5298093327a088a7710fd.png)

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-timesheet-entry-section"></a>השתמש בשרשרת הפקודה בשיטת buildCustomFieldList של המחלקה TSTimesheetSettings כדי להציג שדה במקטע ערך גיליונות.

קוד זה שולט בהגדרות התצוגה של השדה באפליקציה. לדוגמה, הוא שולט בסוג השדה, בתווית, האם השדה הוא חובה ובאיזה קטע השדה מופיע.

הדוגמה הבאה מציגה שדה מחרוזת בערכי זמן. לשדה זה שתי אפשרויות, **אפשרות ראשונה** ו- **אפשרות שנייה**, הזמינים באמצעות לחצני אפשרויות (לחצני רדיו). השדה באפליקציה משויך לשדה **TestLineString** שנוסף לטבלת TSTimesheetLine.

שים לב לשימוש בשיטה **TSTimesheetCustomField::newFromMetatdata()** כדי לפשט את האתחול של מאפייני השדה המותאמים אישית: **fieldBaseType**, **tableName**, **fieldname**, **label**, **isEditable**, **isMandatory**, **stringLength** ו- **numberOfDecimals**. אתה יכול גם להגדיר פרמטרים אלה באופן ידני, לפי העדפתך.

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

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforentry-method-of-the-tstimesheetentry-class-to-enter-values-in-a-timesheet-entry"></a>השתמש בשרשרת הפקודה בשיטת buildCustomFieldListForEntry של המחלקה TSTimesheetEntry כדי להזין ערכים בערך גיליונות.

השיטה **buildCustomFieldListForEntry** משמשת להזנת ערכים בקווי הגליון השמורים באפליקציה למכשירים ניידים. נדרשת רשומת TSTimesheetTrans כפרמטר. ניתן להשתמש בשדות מאותה רשומה למילוי ערך השדה המותאם אישית באפליקציה.

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

### <a name="use-chain-of-command-on-the-tstimesheetentryservice-class-to-save-a-timesheet-entry-from-the-app-back-to-the-database"></a>השתמש בשרשרת הפקודה במחלקה TSTimesheetEntryService כדי לשמור ערך גיליון זמנים מהאפליקציה בחזרה למסד הנתונים

כדי לשמור שדה מותאם אישית בחזרה למסד הנתונים בשימוש אופייני, עליך להרחיב מספר שיטות:

- השיטה **timesheetLineNeedsUpdating** משמשת כדי לקבוע אם רשומת השורה שונתה על ידי המשתמש באפליקציה ויש לשמור אותה במסד הנתונים. אם ביצועים אינם מהווים עניין, ניתן לפשט שיטה זו כך שתמיד תחזיר **true**.
- ניתן להרחיב את השיטות **populateTimesheetLineFromEntryDuringCreate** ו- **populateTimesheetLineFromEntryDuringUpdate** כך שהן מזינות ערכים ברשומת מסד הנתונים TSTimesheetLine מתוך רשומת חוזה הנתונים של TSTimesheetEntry המסופקת. בדוגמה הבאה, שים לב כיצד המיפוי בין שדה מסד הנתונים לשדה ההזנה נעשה באופן ידני באמצעות קוד X++‎.
- ניתן גם להרחיב את השיטה **populateTimesheetWeekFromEntry** אם השדה המותאם אישית שממופה לאובייקט **TSTimesheetEntry** חייב לכתוב חזרה לטבלת מסד הנתונים TSTimesheetLineweek.

> [!NOTE]
> הדוגמה הבאה שומרת את הערך **firstOption** או **secondOption** שהמשתמש בוחר למסד הנתונים כערך מחרוזת גולמי. אם שדה מסד הנתונים הוא שדה מסוג **ספירה**, ניתן למפות ידנית את הערכים לערך ספירה ואז לשמור אותם בשדה ספירה בטבלת מסד הנתונים.

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

## <a name="show-a-custom-field-in-the-timesheet-header-section"></a>הצג שדה מותאם אישית במקטע כותרת גיליונות הזמנים ושמור אותו

להלן צילום מסך מהאפליקציה למכשירים ניידים של משתמש המציג גיליון זמנים. הלחצן "מידע נוסף" נבחר בפינה השמאלית העליונה כדי להציג את האפשרות "הצג פרטים נוספים".  

![הצג פקודה של פרטים נוספים](media/show-more.png)

להלן צילום מסך מהאפליקציה למכשירים ניידים המציג את המקטע "עוד" של גיליון זמנים. שדה מותאם אישית בשם "קצב ניצול של גיליון זמנים זה (שדה מותאם אישית מחושב)" נוסף למקטע כותרת גיליון הזמנים. ערך לקריאה בלבד של "0.667" מוגדר בשדה המותאם אישית.

![מקטע נוסף](media/more-section.jpg)

### <a name="extend-the-tstimesheettable-table-so-that-it-has-a-custom-field"></a>הרחב את הטבלה TSTimesheetTable כך שיהיה לה שדה מותאם אישית

בתרחישים נפוצים, סביר להניח שהנתונים עבור שדה מותאם אישית במקטע הכותרת יגיעו מהטבלה TSTimesheetHeader. עם זאת, ניתן להשתמש בטבלאות אחרות אם ניתן לאחזר את הנתונים על סמך רשומת TSTimesheetTable המסופקת, או אם אין לו הקשר רשומות ספציפי (למשל, אם השדה מוגדר לקריאה בלבד בפרמטרים של הפרויקט).

שים לב כי לשדות מותאמים אישית לא חייבים להיות רשומות בסיס נתונים כלשהן. ניתן ליצור אותם באופן דינמי על סמך לוגיקה של X++‎. הדוגמה הבאה מציגה גישה זו.

שדות במקטע הכותרת נחשבים תמיד כקריאה בלבד באפליקציה.

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-header-section"></a>השתמש בשרשרת הפקודה בשיטת buildCustomFieldList של המחלקה TSTimesheetSettings כדי להציג שדה במקטע הכותרת

קוד זה שולט בהגדרות התצוגה של השדה באפליקציה. לדוגמה, הוא שולט בסוג השדה, בתווית, האם השדה הוא חובה ובאיזה קטע השדה מופיע.

הדוגמה הבאה מציגה ערך מחושב במקטע הכותרת באפליקציה.

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

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforheader-method-of-the-tstimesheetdetails-class-to-fill-in-timesheet-details"></a>השתמש בשרשרת הפקודה בשיטת buildCustomFieldListForHeader של המחלקה TSTimesheetDetails כדי למלא פרטים בגיליון הזמנים

השיטה **buildCustomFieldListForHeader** משמשת למילוי פרטי כותרת גיליון הזמנים באפליקציה למכשירים ניידים. נדרשת רשומת TSTimesheetTable כפרמטר. ניתן להשתמש בשדות מאותה רשומה למילוי ערך השדה המותאם אישית באפליקציה. הדוגמה הבאה לא קוראת שום ערך ממסד הנתונים. במקום זאת, היא משתמשת בלוגיקת X++‎ כדי ליצור ערך מחושב שלאחר מכן מוצג באפליקציה.


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

## <a name="other-configurabilityextensibility-opportunities"></a>הזדמנויות להגדרה / הרחבה אחרות

### <a name="adding-additional-validation-for-the-app"></a>הוספת אימות נוסף לאפליקציה

לוגיקה קיימת לפונקציונליות של גיליון זמנים ברמת מסד הנתונים עדיין תפעל כצפוי. כדי להפריע להשלמת השמירה או שליחת פעולות וכדי להציג הודעת שגיאה ספציפית, אתה יכול להוסיף **שגיאת זריקה ("הודעה למשתמש")** לקוד באמצעות שרשרת של סיומת פקודה. להלן שלוש דוגמאות לשיטות הניתנות להרחבה:

- אם **validateWrite** בטבלה TSTimesheetLine מחזיר **false** במהלך פעולת שמירה עבור שורה בגיליון זמנים, הודעת שגיאה מוצגת באפליקציה למכשירים ניידים.
- אם **validateSubmit** בטבלה TSTimesheetTable מחזיר **false** במהלך שליחת גיליון זמנים באפליקציה, הודעת שגיאה מוצגת למשתמש.
- לוגיקה שממלאת שדות (למשל, **מאפיין שורה**) במהלך שיטת **insert** בטבלת TSTimesheetLine עדיין תפעל.

### <a name="hiding-and-marking-out-of-box-fields-as-read-only-via-configuration"></a>הסתרה וסימון שדות מוכנים לשימוש כקריאה בלבד באמצעות הגדרת תצורה

מהפרמטרים של הפרויקט, באפשרותך להפוך שדות מוכנים לשימוש לקריאה בלבד או מוסתרים באפליקציה למכשירים ניידים. הגדר את האפשרויות במקטע **גיליונות זמנים לנייד** בכרטיסייה **גיליון זמנים** של הדף **ניהול פרויקטים ופרמטרים חשבונאיים**.

![פרמטרים של פרויקט](media/5753b8ecccd1d8bb2b002dd538b3f762.png)

### <a name="changing-the-activities-that-are-available-for-selection-via-extensions"></a>שינוי הפעילויות הזמינות לבחירה באמצעות הרחבות

הפעילויות הזמינות לבחירה לפרויקט מתמלאות באמצעות השיטות **getActivitiesForProject ()** ו- **getActivityQuery ()** במחלקה **TsTimesheetProjectService**. באפשרותך להשתמש בשרשרת הפקודה כדי לשנות התנהגות זו כך שתתאים לתרחיש העסקי שלך לפעילויות הזמינות לבחירה עבור פרויקט ספציפי.

### <a name="entering-a-default-project-category-on-timesheet-entries"></a>הזנת קטגוריית ברירת מחדל של פרויקט בערכי גיליון זמנים

הזנת קטגוריית ברירת מחדל של פרויקט בערכי גיליון זמנים מתרחשת בשלוש רמות. אתה יכול להשתמש בשרשרת הפקודה כדי להרחיב את ההתנהגות בכל אחת מהרמות הללו או בכולן כדי להשיג את ההתנהגות הרצויה. נעשה שימוש בהיררכיה הבאה:

1. האפליקציה מנסה להציב את קטגוריית ברירת המחדל ממשאב הפרויקט. קטגוריית ברירת מחדל זו מוגדרת בשיטות **getCurrentUserResource** ו- **getDelegatedResourcesForCurrentUser** במחלקה **TSTimesheetSettingsService**.
2. אם קטגוריית ברירת המחדל אינה מסופקת ברמת משאבי הפרויקט, האפליקציה מנסה לשלוף אותה מפעילות הפרויקט. קטגוריית ברירת מחדל זו מוגדרת בשיטה **getActivitiesForProject** שבמחלקה **TSTimesheetProjectService**.
3. אם קטגוריית ברירת המחדל אינה מסופקת ברמת פעילות הפרויקט, קטגוריית ברירת המחדל נשלפת מפרמטרי הפרויקט. קטגוריית ברירת מחדל זו מוגדרת בשיטה **getProjectDetailsbyRule** שבמחלקה **TSTimesheetProjectService**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]