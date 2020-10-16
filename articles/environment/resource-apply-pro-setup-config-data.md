---
title: הגדר והחל נתוני תצורה ב- Common Data Service עבור Project Operations
description: נושא זה מספק מידע על הגדרה והחלה של נתוני התצורה ב- Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d99ab4c7b2ebf6ba56b86a3e0151036c6247e484
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948890"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service-for-project-operations"></a><span data-ttu-id="1c36e-103">הגדר והחל נתוני תצורה ב- Common Data Service עבור Project Operations</span><span class="sxs-lookup"><span data-stu-id="1c36e-103">Set up and apply configuration data in the Common Data Service for Project Operations</span></span>

<span data-ttu-id="1c36e-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="1c36e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="1c36e-105">הגדרת התקנה ונתוני תצורה</span><span class="sxs-lookup"><span data-stu-id="1c36e-105">Install setup and configuration data</span></span>

1. <span data-ttu-id="1c36e-106">הורד, בטל חסימה ובטל דחיסה של [החבילה 'הגדרה ונתוני תצורה'](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span><span class="sxs-lookup"><span data-stu-id="1c36e-106">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span></span>
2. <span data-ttu-id="1c36e-107">נווט אל התיקיה שדחיסתה בוטלה והפעל את קובץ ההפעלה *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="1c36e-107">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="1c36e-108">בעמוד 1 של אשף הגדרת התצורה (CMT‏) של Common Data Service, בחר **ייבא נתונים** ואז בחר **המשך**.</span><span class="sxs-lookup"><span data-stu-id="1c36e-108">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![‏‫העברת תצורה](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="1c36e-110">בעמוד 2 של אשף ב-CMT בחר ב**Office 365** כ**סוג הפריסה**.</span><span class="sxs-lookup"><span data-stu-id="1c36e-110">On Page 2 of the CMT Wizard, select **Office 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="1c36e-111">בחר את תיבות הסימון **הצג רשימה של ארגונים זמינים** ו**הצג מתקדם**.</span><span class="sxs-lookup"><span data-stu-id="1c36e-111">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="1c36e-112">בחר את האזור של הדייר שלך, הזן את האישורים שלך ובחר **כניסה**.</span><span class="sxs-lookup"><span data-stu-id="1c36e-112">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![כניסת תצורה](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="1c36e-114">בעמוד 3, מרשימת הארגונים בדייר, בחר את הארגון שאליו אתה רוצה לייבא את נתוני ההדגמה ובחר **כניסה**.</span><span class="sxs-lookup"><span data-stu-id="1c36e-114">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="1c36e-115">בעמוד 4, בחר את קובץ ה- zip *SampleSetupAndConfigData* מהתיקיה שפורקה.</span><span class="sxs-lookup"><span data-stu-id="1c36e-115">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![בחירת קובץ Zip](./media/3ZipFile.png)

![בחר קובץ](./media/4SelectAFile.png)

9. <span data-ttu-id="1c36e-118">לאחר בחירת קובץ ה-zip בחר **ייבא נתונים**.</span><span class="sxs-lookup"><span data-stu-id="1c36e-118">After the zip file is selected, select **Import Data**.</span></span>

![יבא נתונים](./media/5ImportData.png)

10. <span data-ttu-id="1c36e-120">הייבוא יפעל בין שתיים לעשר דקות, תלוי במהירות הרשת שלך.</span><span class="sxs-lookup"><span data-stu-id="1c36e-120">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="1c36e-121">לאחר השלמת הייבוא, צא מאשף ה- CMT.</span><span class="sxs-lookup"><span data-stu-id="1c36e-121">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="1c36e-122">בדוק אם ישנם נתונים בארגון שלך ב-19 הישויות הבאות:</span><span class="sxs-lookup"><span data-stu-id="1c36e-122">Check your organization for data in the following 19 entities:</span></span>

  - <span data-ttu-id="1c36e-123">מטבע</span><span class="sxs-lookup"><span data-stu-id="1c36e-123">Currency</span></span>
  - <span data-ttu-id="1c36e-124">יחידה ארגונית</span><span class="sxs-lookup"><span data-stu-id="1c36e-124">Organizational Unit</span></span>
  - <span data-ttu-id="1c36e-125">איש קשר</span><span class="sxs-lookup"><span data-stu-id="1c36e-125">Contact</span></span>
  - <span data-ttu-id="1c36e-126">קבוצת מיסים</span><span class="sxs-lookup"><span data-stu-id="1c36e-126">Tax Group</span></span>
  - <span data-ttu-id="1c36e-127">קבוצת לקוחות</span><span class="sxs-lookup"><span data-stu-id="1c36e-127">Customer Group</span></span>
  - <span data-ttu-id="1c36e-128">יחידה</span><span class="sxs-lookup"><span data-stu-id="1c36e-128">Unit</span></span>
  - <span data-ttu-id="1c36e-129">קבוצת יחידות</span><span class="sxs-lookup"><span data-stu-id="1c36e-129">Unit Group</span></span>
  - <span data-ttu-id="1c36e-130">מחירון</span><span class="sxs-lookup"><span data-stu-id="1c36e-130">Price List</span></span>
  - <span data-ttu-id="1c36e-131">מחירון פרמטרים של פרוייקט</span><span class="sxs-lookup"><span data-stu-id="1c36e-131">Project Parameter Price List</span></span>
  - <span data-ttu-id="1c36e-132">תדירות חשבונית</span><span class="sxs-lookup"><span data-stu-id="1c36e-132">Invoice Frequency</span></span>
  - <span data-ttu-id="1c36e-133">קטגוריית משאבים הניתנים להזמנה</span><span class="sxs-lookup"><span data-stu-id="1c36e-133">Bookable Resource Category</span></span>
  - <span data-ttu-id="1c36e-134">קטגוריית עסקה</span><span class="sxs-lookup"><span data-stu-id="1c36e-134">Transaction Category</span></span>
  - <span data-ttu-id="1c36e-135">קטגוריית הוצאות</span><span class="sxs-lookup"><span data-stu-id="1c36e-135">Expense Category</span></span>
  - <span data-ttu-id="1c36e-136">מחיר תפקיד</span><span class="sxs-lookup"><span data-stu-id="1c36e-136">Role Price</span></span>
  - <span data-ttu-id="1c36e-137">מחיר קטגוריית עסקה</span><span class="sxs-lookup"><span data-stu-id="1c36e-137">Transaction Category Price</span></span>
  - <span data-ttu-id="1c36e-138">מאפיין</span><span class="sxs-lookup"><span data-stu-id="1c36e-138">Characteristic</span></span>
  - <span data-ttu-id="1c36e-139">משאב הניתן להזמנה</span><span class="sxs-lookup"><span data-stu-id="1c36e-139">Bookable Resource</span></span>
  - <span data-ttu-id="1c36e-140">קטגוריות משאבים הניתנים להזמנה</span><span class="sxs-lookup"><span data-stu-id="1c36e-140">Bookable resource category Assn</span></span>
  - <span data-ttu-id="1c36e-141">מאפיין של משאב הניתן להזמנה</span><span class="sxs-lookup"><span data-stu-id="1c36e-141">Bookable Resource Characteristic</span></span>

![השלם את הייבוא](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="1c36e-143">עדכן את התצורות של Project Operations</span><span class="sxs-lookup"><span data-stu-id="1c36e-143">Update Project Operations configurations</span></span>

1. <span data-ttu-id="1c36e-144">נווט אל סביבת CE.</span><span class="sxs-lookup"><span data-stu-id="1c36e-144">Navigate to the CE environment.</span></span> <span data-ttu-id="1c36e-145">אתה יכול למצוא אותה על-ידי פתיחת [מרכז הניהול של Power Platform](https://admin.powerplatform.microsoft.com/environments), בחירת הסביבה ואז בחירת האפשרות **פתח את הסביבה**.</span><span class="sxs-lookup"><span data-stu-id="1c36e-145">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![פתח את הסביבה](./media/7OpenEnvironment.png)

2. <span data-ttu-id="1c36e-147">כדי ליצור משאב הניתן להזמנה למשתמש שלך, עבור אל **פרויקטים** > **משאבים** ולאחר מכן בחר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="1c36e-147">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![משאבים הניתנים להזמנה](./media/8BookableResources.png)

3. <span data-ttu-id="1c36e-149">בכרטיסיה **כללי**, בחר את המשתמש שהוא מנהל המערכת שלך.</span><span class="sxs-lookup"><span data-stu-id="1c36e-149">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="1c36e-150">ודא שאזור הזמן תואם את זה שאתה נמצא בו.</span><span class="sxs-lookup"><span data-stu-id="1c36e-150">Verify that the time zone matches the one you are in.</span></span> 

![משאב חדש הניתן להזמנה](./media/9NewBookableResource.png)

4. <span data-ttu-id="1c36e-152">בכרטיסיה **תזמון**, בשדה **חברה**, בחר את החברה **USPM** ולאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="1c36e-152">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![כרטיסיית תזמון](./media/10SchedulingTab.png)

5. <span data-ttu-id="1c36e-154">בחר בכרטיסיה **שעות עבודה**.</span><span class="sxs-lookup"><span data-stu-id="1c36e-154">Select the **Work hours** tab.</span></span>  

![שעות עבודה](./media/11WorkHours.png)

6. <span data-ttu-id="1c36e-156">לחץ פעמיים על ערך כלשהו בלוח השנה ובחר **ערוך** > **כל האירועים בסדרה**.</span><span class="sxs-lookup"><span data-stu-id="1c36e-156">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![לוח שנה של עבודה](./media/12WorkCalendar.png)

7. <span data-ttu-id="1c36e-158">שנה את שעות העבודה לשמונה (8) שעות עבודה ביום, סמן סופי שבוע כימים שאינם ימי עבודה וכן וודא שאזור הזמן תואם לשלך.</span><span class="sxs-lookup"><span data-stu-id="1c36e-158">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="1c36e-159">בחר **שמור וסגור**.</span><span class="sxs-lookup"><span data-stu-id="1c36e-159">Select **Save and close**.</span></span>

![עדכן לוח שנה](./media/13UpdateCalendar.png)

9. <span data-ttu-id="1c36e-161">עבור אל **הגדרות** > **תבניות לוח שנה** ובחר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="1c36e-161">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![תבניות לוח שנה](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="1c36e-163">הזן שם, בחר את משאב התבנית שיצרת ולאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="1c36e-163">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![שמור תבנית לוח שנה](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="1c36e-165">עבור אל **פרמטרים** ולחץ פעמיים על הרשומה.</span><span class="sxs-lookup"><span data-stu-id="1c36e-165">Go to **Parameters** and double-click the record.</span></span> 
 
 ![פרמטרי פרויקט](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="1c36e-167">עדכן את השדות הבאים:</span><span class="sxs-lookup"><span data-stu-id="1c36e-167">Update the following fields:</span></span>

 - <span data-ttu-id="1c36e-168">**חברת ברירת מחדל**: USPM</span><span class="sxs-lookup"><span data-stu-id="1c36e-168">**Default company**: USPM</span></span>
 - <span data-ttu-id="1c36e-169">**יחידה ארגונית המוגדרת כברירת מחדל**: Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="1c36e-169">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="1c36e-170">**תדירות חשבונית**: היום השביעי והאחרון</span><span class="sxs-lookup"><span data-stu-id="1c36e-170">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="1c36e-171">**תבנית שעות עבודה**: שנה לתבנית שיצרת.</span><span class="sxs-lookup"><span data-stu-id="1c36e-171">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="1c36e-172">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="1c36e-172">Select **Save**.</span></span> 

![עדכן פרמטרי פרויקט](./media/17UpdatedProjectParameters.png)
