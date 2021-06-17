---
title: כיצד ניתן להתאים אישית את זרימת התהליך העסקי של שלבי פרוייקט?
description: מבט כולל על אופן ההתאמה האישית של זרימת התהליך העסקי של שלבי פרוייקט.
ms.custom:
- dyn365-projectservice
ms.date: 10/11/2018
ms.topic: article
author: JohnPBurrows
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
ms.openlocfilehash: 2e6c60fe67aea908013077bde40c2faeabc2f39e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993147"
---
# <a name="how-do-i-customize-the-project-stages-business-process-flow"></a><span data-ttu-id="b5ab2-103">כיצד ניתן להתאים אישית את זרימת התהליך העסקי של שלבי פרוייקט?</span><span class="sxs-lookup"><span data-stu-id="b5ab2-103">How do I customize the Project Stages business process flow?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-2-4x-9-0-platform](../includes/cc-applies-to-psa-app-2-4x-9-0-platform.md)]
[!INCLUDE[cc-applies-to-psa-app-1x-8-2-platform](../includes/cc-applies-to-psa-app-1x-8-2-platform.md)]

<span data-ttu-id="b5ab2-104">קיימת מגבלה מוכרת בגירסאות הקודמות של יישום Project Service שהשמות של שלבים בזרימת תהליך עסקי של שלבי פרוייקט חייבים להתאים בדיוק לשמות הצפויים באנגלית (**Quote**, **Plan**, **Plan**).</span><span class="sxs-lookup"><span data-stu-id="b5ab2-104">There's a known limitation in earlier versions of the Project Service application that the names of the stages in the Project Stages business process flow must exactly match the expected English names (**Quote**, **Plan**, **Close**).</span></span> <span data-ttu-id="b5ab2-105">אחרת, לוגיקה עסקית, המסתמכת על שמות השלבים באנגלית, אינה פועלת כצפוי.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-105">Otherwise, the business logic, which relies on the English stage names, doesn't work as expected.</span></span> <span data-ttu-id="b5ab2-106">לכן אינך רואה פעולות מוכרות כגון **Switch Process** או **Edit Process** זמינות בטופס פרוייקט, והתאמה אישית של זרימת תהליך עסקי אינה מומלצת.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-106">That's why you don't see familiar actions such as **Switch Process** or **Edit Process** available on the project form, and customizing the business process flow isn't encouraged.</span></span> 

<span data-ttu-id="b5ab2-107">מגבלה זו טופלה בגירסה 2.4.5.48 ואילך.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-107">This limitation has been addressed in version 2.4.5.48 and later.</span></span> <span data-ttu-id="b5ab2-108">המאמר מספק דרכים לעקיפת הבעיה עבור הגירסאות הקודמות אם עליך להתאים אישית את זרימת התהליך העסקי של ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-108">This article provides suggested workarounds if you need to customize the default business process flow for earlier versions.</span></span>  

## <a name="business-logic-requires-an-exact-match-with-english-stage-names"></a><span data-ttu-id="b5ab2-109">לוגיקה עסקית דורשת התאמה מדויקת עם שמות השלבים באנגלית</span><span class="sxs-lookup"><span data-stu-id="b5ab2-109">Business logic requires an exact match with English stage names</span></span>

<span data-ttu-id="b5ab2-110">זרימת תהליך עסקי של שלבי פרוייקט כוללת לוגיקה עסקית המניעה את אופני הפעולה הבאים ביישום:</span><span class="sxs-lookup"><span data-stu-id="b5ab2-110">The Project Stages business process flow includes business logic that drives the following behaviors in the app:</span></span>
- <span data-ttu-id="b5ab2-111">כאשר הפרוייקט משויך להצעת מחיר, הקוד מגדיר את זרימת תהליך עסקי לשלב **‎Quote**.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-111">When the project is associated with a quote, the code sets the business process flow to the **Quote** stage.</span></span>
- <span data-ttu-id="b5ab2-112">כאשר הפרוייקט משויך לאיש קשר, הקוד מגדיר את זרימת תהליך עסקי לשלב **‎Plan**.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-112">When the project is associated with a contract, the code sets the business process flow to the **Plan** stage.</span></span>
- <span data-ttu-id="b5ab2-113">כאשר זרימת התהליך העסקי מתקדמת לשלב **Close**, רשומת הפרוייקט מפסיקה לפעול.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-113">When the business process flow is advanced to the **Close** stage, the project record is deactivated.</span></span> <span data-ttu-id="b5ab2-114">כאשר הפרוייקט מבוטל, טופס הפרוייקט ומבנה התפלגות עבודה (WBS) מוגדרים לקריאה בלבד, הזמנות משאבים בעלי שם ישוחררו וכל המחירונים המשויכים יתבטלו.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-114">When the project is deactivated, the project form and work breakdown structure (WBS) are set to read-only, the named resource bookings are released, and any associated price lists are deactivated.</span></span>

<span data-ttu-id="b5ab2-115">לוגיקה עסקית זו מסתמכת על השמות באנגלית עבור שלבי הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-115">This business logic relies on the English names for the project stages.</span></span> <span data-ttu-id="b5ab2-116">תלות זו בשמות השלבים באנגלית היא הסיבה העיקרית מדוע התאמה אישית של זרימת תהליך עסקי של שלבי פרוייקט אינה מומלצת, כמו גם מדוע אינך רואה פעולות נפוצות של זרימת תהליך עסקי כמו **Switch Process** או **Edit Process** בישות הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-116">This dependency on the English stage names is the main reason why customization of the Project Stages business process flow isn't encouraged, as well as why you don’t see the common business process flow actions like **Switch Process** or **Edit Process** on the project entity.</span></span>

## <a name="what-happens-if-the-stage-names-dont-match-the-english-names"></a><span data-ttu-id="b5ab2-117">מה קורה אם שמות השלבים אינם תואמים לשמות באנגלית?</span><span class="sxs-lookup"><span data-stu-id="b5ab2-117">What happens if the stage names don't match the English names?</span></span>

<span data-ttu-id="b5ab2-118">ביישום Project Service גירסה 1. x בפלטפורמה 8.2, כאשר שמות השלבים בזרימת התהליך העסקי אינם תואמים בדיוק לשמות השלבים באנגלית, הלוגיקה העסקית שמגדירה את השלב הנכון עבור הצעות מחיר או חוזים, או אשר סוגרת את הפרוייקט, מדולגת על-ידי המערכת.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-118">In the Project Service app version 1.x on the 8.2 platform, when the stage names in the business process flow don’t match the English stage names exactly, the business logic that sets the right stage for quotes or contracts, or that closes the project, is skipped.</span></span> <span data-ttu-id="b5ab2-119">לא מוצגות הודעות שגיאה.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-119">No error messages are displayed.</span></span> <span data-ttu-id="b5ab2-120">לכן נראה כי באפשרותך להתאים אישית את זרימת התהליך העסקי של שלבי פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-120">Therefore it appears that you are able to customize the Project Stages business process flow.</span></span> <span data-ttu-id="b5ab2-121">עם זאת, אף אחד מהתהליכים האוטומטיים לא יעבוד עבור הצעות מחיר, חוזים וסגירת פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-121">However, you won’t see any of the automatic processes working for quotes, contracts, and project close.</span></span>

<span data-ttu-id="b5ab2-122">ביישום Project Service גירסה 2.4.4.30 ומטה בפלטפורמה 9.0, היה שינוי ארכיטקטוני משמעותי בזרימות תהליך עסקי, שדרש לכתוב מחדש את הלוגיקה העסקית של זרימת תהליך עסקי.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-122">In the Project Service app version 2.4.4.30 or earlier on the 9.0 platform, there was a significant architectural change to business process flows, which required a re-write of the business process flow business logic.</span></span> <span data-ttu-id="b5ab2-123">כתוצאה מכך, אם שמות שלבי התהליך אינם תואמים לשמות הצפויים באנגלית, תקבל הודעת שגיאה.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-123">As a result, if the process stage names don’t match the expected English names, you do receive an error message.</span></span> 

<span data-ttu-id="b5ab2-124">לכן, אם ברצונך להתאים אישית את זרימת התהליך העסקי של שלבי פרוייקט עבור הישות פרוייקט, באפשרותך להוסיף רק שלבים חדשים לגמרי לזרימת התהליך העסקי המהווה ברירת מחדל עבור הישות פרוייקט, תוך השארת השלבים **Quote**, **Plan** ו- **‎Close** כמו שהם.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-124">Therefore, if you want to customize the Project Stages business process flow for the project entity, you can only add brand new stages to the default business process flow for the project entity, while keeping the **Quote**, **Plan**, and **Close** stages as-is.</span></span> <span data-ttu-id="b5ab2-125">הגבלה זו מבטיחה כי אינך תקבל שגיאות מהלוגיקה העסקית אשר מצפה לשמות השלבים באנגלית בזרימת תהליך עסקי.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-125">This restriction ensures that you don’t get errors from the business logic that expects the English stage names in the business process flow.</span></span>

<span data-ttu-id="b5ab2-126">בגירסה 2.4.5.48 ואילך, לוגיקה עסקית המתוארת במאמר זה מוסרת מזרימת תהליך עסקי של ברירת המחדל עבור הישות פרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-126">In version 2.4.5.48 or later, the business logic described in this article has been removed from the default business process flow for the project entity.</span></span> <span data-ttu-id="b5ab2-127">שדרוג לגירסה זו ומעלה יאפשר לך לבצע התאמה אישית או להחליף את זרימת התהליך העסקי של ברירת המחדל לזרימה משלך.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-127">Upgrading to that version or later will let you customize or replace the default business process flow with one of your own.</span></span> 

## <a name="workarounds-for-earlier-versions"></a><span data-ttu-id="b5ab2-128">פתרונות עבור הגירסאות הקודמות</span><span class="sxs-lookup"><span data-stu-id="b5ab2-128">Workarounds for earlier versions</span></span>

<span data-ttu-id="b5ab2-129">אם אין אפשרות לבצע שדרוג, באפשרותך להתאים אישית את זרימת התהליך העסקי של שלבי פרוייקט עבור הישות פרוייקט באחת משתי הדרכים הבאות:</span><span class="sxs-lookup"><span data-stu-id="b5ab2-129">If upgrading isn't an option, you can customize the Project Stages business process flow for the project entity in one of these two ways:</span></span>

1. <span data-ttu-id="b5ab2-130">הוסף שלבים נוספים לתצורת ברירת המחדל, תוך שמירת שמות השלבים באנגלית עבור **Quote**, **Plan** ו- **Close**.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-130">Add additional stages to the default configuration, while retaining the English stage names for **Quote**, **Plan**, and **Close**.</span></span>


![צילום מסך של הוספת שלבים לתצורת ברירת המחדל](media/FAQ-Customize-BPF-1.png)
 
2. <span data-ttu-id="b5ab2-132">צור זרימת תהליך עסקי משלך והפוך אותה זרימת התהליך העסקי הראשית עבור הישות פרוייקט, מה שייאפשר לך לנהל את כל שמות השלבים הרצויים.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-132">Create your own business process flow and make it the primary business process flow for the project entity, which lets you have any stage names you want.</span></span> <span data-ttu-id="b5ab2-133">עם זאת, אם ברצונך להשתמש באותם שלבי הפרוייקט הרגילים **Quote**, **Plan** ו- **Close**, עליך לבצע התאמות אישיות מסוימות שנובעות משמות השלבים המותאמים אישית שלך.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-133">However, if you want to use the same standard project stages **Quote**, **Plan**, and **Close**, you need to do some customizations that are driven off your custom stage names.</span></span> <span data-ttu-id="b5ab2-134">הלוגיקה המורכבת יותר היא בסגירת הפרוייקט, שבאפשרותך להפעיל עדיין על-ידי ביטול רשומת הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-134">The more complex logic is in the closing of the project, which you can still trigger by just deactivating the project record.</span></span>

![התאמה אישית BPD](media/FAQ-Customize-BPF-2.png)

### <a name="additional-considerations-for-project-service-app-version-24430-or-earlier-on-platform-90"></a><span data-ttu-id="b5ab2-136">שיקולים נוספים עבור יישום Project Service גירסה 2.4.4.30 ומטה בפלטפורמה 9.0</span><span class="sxs-lookup"><span data-stu-id="b5ab2-136">Additional considerations for Project Service app version 2.4.4.30 or earlier on platform 9.0</span></span>

<span data-ttu-id="b5ab2-137">ב-Project Service גירסה 2.4.4.30 ומטה בפלטפורמה 9.0, עם זרימת תהליך עיסקי מותאמת אישית השדה **שם שלב** בישות הפרוייקט נמצא בשימוש בתרשים **פרוייקט לפי שלב** ותצוגות רשימת פרוייקטים לא מתעדכנות, מכיוון שהן משולבות עם זרימת תהליך עסקי של שלבי פרוייקט בברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-137">In Project Service 2.4.4.30 or earlier on platform 9.0, with a custom business process flow the **Stage Name** field on the project entity used in the **Project By Stage** chart and project list views won’t update, because it’s coupled to the default Project Stages business process flow.</span></span> <span data-ttu-id="b5ab2-138">ניתן לטפל בבעיה זו על-ידי ביצוע השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="b5ab2-138">You can address this issue with the following steps:</span></span>

- <span data-ttu-id="b5ab2-139">הוסף שדה מותאם אישית כדי ללכוד את השלב הנוכחי של זרימת תהליך עסקי שמתעדכן ככל שהמשתמש מתקדם בזרימת תהליך עיסקי מותאמת אישית.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-139">Add a custom field to capture the current business process flow stage that is updated as the user advances through the custom business process flow.</span></span>

- <span data-ttu-id="b5ab2-140">שנה את התרשים **פרוייקט לפי שלב** כדי לעבוד עם השדה המותאם אישית שלך במקום בתצורת ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-140">Modify the **Project By Stage** chart to work with your custom field instead of the default configuration.</span></span>

### <a name="steps-to-create-your-own-business-process-flow-for-the-project-entity"></a><span data-ttu-id="b5ab2-141">שלבים ליצירת זרימת תהליך עסקי משלך עבור הישות פרוייקט</span><span class="sxs-lookup"><span data-stu-id="b5ab2-141">Steps to create your own business process flow for the project entity</span></span>

<span data-ttu-id="b5ab2-142">ליצירת זרימת תהליך עסקי משלך עבור הישות פרוייקט, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="b5ab2-142">To create your own business process flow for the project entity do the following:</span></span>

1. <span data-ttu-id="b5ab2-143">עבור אל **הגדרות** > **מרכז התהליכים**.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-143">Go to **Settings** > **Process Center**.</span></span> <span data-ttu-id="b5ab2-144">אל תעתיק את זרימת התהליך העסקי של שלבי פרוייקט מאחר שזה מעתיק גם את הלוגיקה העסקית של Project Service.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-144">Don’t copy the Project Stages business process flow because that also copies the Project Service business logic.</span></span>

  ![יצירת תהליך](media/FAQ-Customize-BPF-3.png)

2. <span data-ttu-id="b5ab2-146">השתמש במעצב התהליכים ליצירת שמות השלבים הרצויים.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-146">Use the Process Designer to create the stage names you want.</span></span> <span data-ttu-id="b5ab2-147">אם אתה רוצה לקבל פונקציונליות זהה לזו של שלבי ברירת המחדל עבור **Quote**, **Plan** ו- **Close**, יהיה עליך ליצור אותה בהתבסס על שמות השלבים של זרימת תהליך עיסקי מותאמת אישית שלך.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-147">If you want the same functionality as the default stages for **Quote**, **Plan**, and **Close**, you’ll have to create that based on your custom business process flow’s stage names.</span></span>

   ![צילום מסך של מעצב תהליכים המשמש להתאמה אישית של BPF](media/FAQ-Customize-BPF-4.png) 

3. <span data-ttu-id="b5ab2-149">ב'מעצב התהליכים, לחץ על **‏‫סדר זרימות תהליך‬** כדי להפוך זרימת תהליך עסקי מותאמת אישית לזרימת תהליך עסקי ראשית עבור הישות פרוייקט על-ידי העברתה מעל זרימת התהליך העסקי של שלבי פרוייקט לראש הרשימה.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-149">In the Process Designer, click **Order Process Flow** to make the custom business process flow the primary business process flow for the project entity by moving it above the Project Stages business process flow to the top of the list.</span></span>


   [<span data-ttu-id="b5ab2-150">צילום מסך של שימוש בסדר זרימות תהליך</span><span class="sxs-lookup"><span data-stu-id="b5ab2-150">Screenshot of using Order Process Flow</span></span>](media/FAQ-Customize-BPF-5-720.png)

### <a name="the-following-steps-apply-to-project-service-app-24430-or-earlier-on-the-90-platform"></a><span data-ttu-id="b5ab2-151">השלבים הבאים חלים על יישום Project Service גירסה 2.4.4.30 ומטה בפלטפורמה 9.0</span><span class="sxs-lookup"><span data-stu-id="b5ab2-151">The following steps apply to Project Service app 2.4.4.30 or earlier on the 9.0 platform</span></span>

4. <span data-ttu-id="b5ab2-152">הוסף שדה מותאם אישית חדש לישות פרוייקט כדי ללכוד את השלבים המותאמים אישית בזרימת התהליך העסקי המותאמת אישית שלך.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-152">Add a new custom field to the project entity to capture the custom stages in your custom business process flow.</span></span> <span data-ttu-id="b5ab2-153">יהיה עליך להוסיף לוגיקה עסקית (תוסף/זרימת עבודה) כדי לעדכן שדה זה כאשר השלב בזרימת התהליך העיסקי המותאמת אישית מתעדכן.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-153">You’ll need to add business logic (plugin/workflow) to update this field when the stage on the custom business process flow is updated.</span></span>

   ![צילום מסך של התאמה אישית של הישות פרוייקט](media/FAQ-Customize-BPF-6-720.png)

5. <span data-ttu-id="b5ab2-155">שנה את התרשים **פרוייקט לפי שלב** כדי להשתמש בשדה המותאם אישית החדש שלך עבור שלבים.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-155">Modify the **Project By Stage** chart to use your new custom field for stages.</span></span>

   ![צילום מסך של שימוש בתרשים 'פרוייקט לפי שלב'](media/FAQ-Customize-BPF-7-720.png)

6. <span data-ttu-id="b5ab2-157">שנה את כל התצוגות עבור הישות פרוייקט כדי לכלול את השדה המותאם אישית החדש עבור שלבים.</span><span class="sxs-lookup"><span data-stu-id="b5ab2-157">Modify any views for the project entity to include your new custom field for stages.</span></span>

   ![צילום מסך של שינוי תצוגות בישות פרוייקט](media/FAQ-Customize-BPF-8-720.png)



[!INCLUDE[footer-include](../includes/footer-banner.md)]