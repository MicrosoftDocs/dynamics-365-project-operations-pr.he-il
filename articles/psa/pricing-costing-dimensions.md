---
title: דף הבית לממדי תמחור ותמחיר
description: נושא זה מספק מבט כולל על ממדי תמחור.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 515a2e2e518614884b414ca43702e8bfea2c6919
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077349"
---
# <a name="pricing-and-costing-dimensions-home-page"></a>דף הבית לממדי תמחור ותמחיר

הממדים המשמשים לקביעת תמחור עבודה ועלות בארגונים מבוססי פרויקטים מושפעים מהתכונות הבאות:

- אנשים שעושים עבודה הדומה לניסיון, לתפקיד או למיקום הגיאוגרפי שלהם
- עבודה שתתבצע בדומה למורכבותה או לשעה ביום

בהתחשב במה שמאפיין תכונות אלה של העבודה והאנשים הנדרשים לביצוע העבודה, ישנם שני סוגים של ערכי ממד תמחור שזמינים ב- Project Service Automation: 

- **קבוצות של אפשרויות** - ממדים שהם ספירות קבועות עבור קבוצת ערכים.
- **ערכים מבוססי ישויות** - תכונות שיכולות לכלול סט ערכים שונה אך סופי יכולות להשתנות לאורך זמן.

## <a name="pricing-dimensions"></a>ממדי תמחור

PSA מסופק עם קבוצה של ממדי תמחור בברירת מחדל. תוכל להציג אותם על-ידי מעבר אל **Project Service** > **פרמטרים**. ברשומת הפרמטר, בכרטיסיה **‬‏‫ממדי תמחור מבוססי-כמות** , ודא שבתפקיד, **msdyn_resourcecategory** וביחידה הארגונית להקצאת משאבים, **msdyn_organizationalunit** השדה **‏‫חל על מכירות‬** והשדה **‏‫חל על עלות‬** מוגדרים בתור **כן**. כך תוכל להגדיר את המחיר ואת העלות עבור כל שילוב של תפקיד ויחידה ארגונית.

![צילום מסך של פרמטרי Project Service כאשר "חל על מכירות" מודגש](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> אם השתמשת בשדות המוכנים לשימוש של תפקיד ויחידה ארגונית כממדי תמחור לפי גירסה 3 של PSA, לא יהיו שינויים נראים לעין. באפשרותך להמשיך להשתמש ב- Project Service כרגיל. 

אם אתה צריך מחיר או עלות עבור המשאבים שלך באמצעות תכונות נוספות, תוכל ליצור שדות, ישויות וממדים מותאמים אישית. לקבלת מידע נוסף, עיין בנושאים הבאים, אך שים לב שעליך להשלים את ההליכים בסדר המפורט להלן:

- [יצירת שדות וישויות מותאמים אישית](create-custom-fields-entities.md)
- [הוספת שדות מותאמים אישית להגדרת מחיר וישויות של טרנזקציות](field-references.md)
- [הגדרת שדות מותאמים אישית כממדי תמחור ](set-up-pricing-dimensions.md)
- [עדכון תכונות של יישום Plug-in כדי לכלול ממדי תמחור חדשים](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a>תמחור זמן של משאב אנושי
כיצד ארגון מתמחר זמן של משאב אנושי הוא לרוב שיקול אסטרטגי חשוב שמשפיע ישירות על רווחיות הארגון. עבוד עם הצוותים הפיננסיים וראשי אגפים כאשר הארגון שלך מוכן לזהות כיצד הוא מעוניין להגדיר את תעריפי עלויות וחיוב עבור הזמן של המשאב האנושי.

שיקולים אחרים לתמחור כוללים אם להשתמש מחדש בשדות או בישויות שאינם כרגע ממדי תמחור, אך מוחלים כממד תמחור עבור הארגון שלך. שדות כמו **קטגוריית עסקה** ( **msdyn_transactioncategory** ) ו **משאב ניתן להזמנה** ( **bookableresource** ) הם דוגמאות לממדים מועמדים. 

כדאי לשקול גם אם ממד התמחור שלך צריך להיות טבלה או קבוצת אפשרויות. אם אתה צופה שינויים בערכים של ממד שיחרוג מ- 10 או 12 ואתה זקוק לתכונות נוספות בערכים אלה, תוכל ליצור ישות במקום קבוצת אפשרויות. תחזוקה של קבוצת אפשרויות, כגון הוספה או הסרה של ערכים, מחייבת מנהל מערכת או מפתח בעוד שהוספת שורות חדשות לטבלה יכולה להתבצע על-ידי רוב המשתמשים העסקיים.

הדוגמה הבאה מציגה את תעריפי החיוב שמוגדרים בהתאם לתפקיד וליחידה הארגונית להקצאת משאבים שאליה המשאב שייך. תעריפי עלויות מבוססים בדרך כלל על טווח השכר של העובד ועל היחידה הארגונית שאליה הוא שייך. בדוגמה זו, הטבלאות של תעריף החיוב ותעריף העלויות ייראו כך.

**תעריפי חיוב לדוגמה**

| תפקיד        | יחידה ארגונית    |יחידה      |מחיר      |מטבע  |
| ------------|-------------|----------|----------:|----------|
| מפתח   | Contoso US  |Hour | 200|USD     |
| מפתח   | Contoso India |Hour|   112|USD     |


**תעריפי עלויות לדוגמה**

| טווח שכר     | יחידה ארגונית    |יחידה      |מחיר      |מטבע  |
| ----------------|-------------|----------|----------:|----------|
| טווח1_של החברה שלי | Contoso US  |Hour | 145|USD     |
| טווח2_של החברה שלי | Contoso India |Hour|   67|USD     |