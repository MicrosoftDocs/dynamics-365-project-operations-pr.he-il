---
title: הגדרה והחלה של נתוני  תצורה ב-Common Data Service
description: נושא זה מספק מידע על הגדרה והחלה של נתוני התצורה ב- Project Operations.
author: sigitac
manager: Annbe
ms.date: 11/04/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 1651d3b3b85d3dc581bf61976fada249bafd6b7b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289820"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service"></a><span data-ttu-id="c8328-103">הגדרה והחלה של נתוני  תצורה ב-Common Data Service</span><span class="sxs-lookup"><span data-stu-id="c8328-103">Set up and apply configuration data in the Common Data Service</span></span> 

<span data-ttu-id="c8328-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="c8328-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="c8328-105">דרישות מוקדמות</span><span class="sxs-lookup"><span data-stu-id="c8328-105">Prerequisites</span></span>

<span data-ttu-id="c8328-106">לפני תחילת קביעת התצורה של נתונים ב-Common Data Service ‏(CDS), התנאים המוקדמים הבאים חייבים להתקיים:</span><span class="sxs-lookup"><span data-stu-id="c8328-106">Before you beging to configure data in the Common Data Service (CDS), the following prerequisites must be met:</span></span>

1.  <span data-ttu-id="c8328-107">הקצאת סביבת CDS וסביבת Dynamics 365 Finance ל-Project Operations.</span><span class="sxs-lookup"><span data-stu-id="c8328-107">Provision a CDS environment and a Dynamics 365 Finance environment for Project Operations.</span></span>
2.  <span data-ttu-id="c8328-108">מידע על הישות המשפטית מ-Dynamics 365 Finance משותף בסביבת CDS.</span><span class="sxs-lookup"><span data-stu-id="c8328-108">Legal entity information from Dynamics 365 Finance is shared to the CDS environment.</span></span> <span data-ttu-id="c8328-109">פירוש הדבר שישות **חברה** ב- CDS כוללת את רשומות החברה הבאות:</span><span class="sxs-lookup"><span data-stu-id="c8328-109">This means that the **Company** entity in CDS has the following company records:</span></span>
  - <span data-ttu-id="c8328-110">THPM</span><span class="sxs-lookup"><span data-stu-id="c8328-110">THPM</span></span>
  - <span data-ttu-id="c8328-111">USPM</span><span class="sxs-lookup"><span data-stu-id="c8328-111">USPM</span></span>
  - <span data-ttu-id="c8328-112">GBPM</span><span class="sxs-lookup"><span data-stu-id="c8328-112">GBPM</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="c8328-113">הגדרת התקנה ונתוני תצורה</span><span class="sxs-lookup"><span data-stu-id="c8328-113">Install setup and configuration data</span></span>

1. <span data-ttu-id="c8328-114">הורד, בטל חסימה ובטל דחיסה של [החבילה 'הגדרה ונתוני תצורה'](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span><span class="sxs-lookup"><span data-stu-id="c8328-114">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span></span>
2. <span data-ttu-id="c8328-115">נווט אל התיקיה שדחיסתה בוטלה והפעל את קובץ ההפעלה *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="c8328-115">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="c8328-116">בעמוד 1 של אשף הגדרת התצורה (CMT‏) של Common Data Service, בחר **ייבא נתונים** ואז בחר **המשך**.</span><span class="sxs-lookup"><span data-stu-id="c8328-116">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![‏‫העברת תצורה](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="c8328-118">בעמוד 2 של אשף ב-CMT בחר ב **Microsoft 365** כ **סוג הפריסה**.</span><span class="sxs-lookup"><span data-stu-id="c8328-118">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="c8328-119">בחר את תיבות הסימון **הצג רשימה של ארגונים זמינים** ו **הצג מתקדם**.</span><span class="sxs-lookup"><span data-stu-id="c8328-119">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="c8328-120">בחר את האזור של הדייר שלך, הזן את האישורים שלך ובחר **כניסה**.</span><span class="sxs-lookup"><span data-stu-id="c8328-120">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![כניסת תצורה](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="c8328-122">בעמוד 3, מרשימת הארגונים בדייר, בחר את הארגון שאליו אתה רוצה לייבא את נתוני ההדגמה ובחר **כניסה**.</span><span class="sxs-lookup"><span data-stu-id="c8328-122">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="c8328-123">בעמוד 4, בחר את קובץ ה- zip *SampleSetupAndConfigData* מהתיקיה שפורקה.</span><span class="sxs-lookup"><span data-stu-id="c8328-123">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![בחירת קובץ Zip](./media/3ZipFile.png)

![בחר קובץ](./media/4SelectAFile.png)

9. <span data-ttu-id="c8328-126">לאחר בחירת קובץ ה-zip בחר **ייבא נתונים**.</span><span class="sxs-lookup"><span data-stu-id="c8328-126">After the zip file is selected, select **Import Data**.</span></span>

![יבא נתונים](./media/5ImportData.png)

10. <span data-ttu-id="c8328-128">הייבוא יפעל בין שתיים לעשר דקות, תלוי במהירות הרשת שלך.</span><span class="sxs-lookup"><span data-stu-id="c8328-128">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="c8328-129">לאחר השלמת הייבוא, צא מאשף ה- CMT.</span><span class="sxs-lookup"><span data-stu-id="c8328-129">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="c8328-130">בדוק אם ישנם נתונים בארגון שלך ב-19 הישויות הבאות:</span><span class="sxs-lookup"><span data-stu-id="c8328-130">Check your organization for data in the following 19 entities:</span></span>

  - <span data-ttu-id="c8328-131">מטבע</span><span class="sxs-lookup"><span data-stu-id="c8328-131">Currency</span></span>
  - <span data-ttu-id="c8328-132">יחידה ארגונית</span><span class="sxs-lookup"><span data-stu-id="c8328-132">Organizational Unit</span></span>
  - <span data-ttu-id="c8328-133">איש קשר</span><span class="sxs-lookup"><span data-stu-id="c8328-133">Contact</span></span>
  - <span data-ttu-id="c8328-134">קבוצת מיסים</span><span class="sxs-lookup"><span data-stu-id="c8328-134">Tax Group</span></span>
  - <span data-ttu-id="c8328-135">קבוצת לקוחות</span><span class="sxs-lookup"><span data-stu-id="c8328-135">Customer Group</span></span>
  - <span data-ttu-id="c8328-136">יחידה</span><span class="sxs-lookup"><span data-stu-id="c8328-136">Unit</span></span>
  - <span data-ttu-id="c8328-137">קבוצת יחידות</span><span class="sxs-lookup"><span data-stu-id="c8328-137">Unit Group</span></span>
  - <span data-ttu-id="c8328-138">מחירון</span><span class="sxs-lookup"><span data-stu-id="c8328-138">Price List</span></span>
  - <span data-ttu-id="c8328-139">מחירון פרמטרים של פרויקט</span><span class="sxs-lookup"><span data-stu-id="c8328-139">Project Parameter Price List</span></span>
  - <span data-ttu-id="c8328-140">תדירות חשבונית</span><span class="sxs-lookup"><span data-stu-id="c8328-140">Invoice Frequency</span></span>
  - <span data-ttu-id="c8328-141">קטגוריית משאבים הניתנים להזמנה</span><span class="sxs-lookup"><span data-stu-id="c8328-141">Bookable Resource Category</span></span>
  - <span data-ttu-id="c8328-142">קטגוריית עסקה</span><span class="sxs-lookup"><span data-stu-id="c8328-142">Transaction Category</span></span>
  - <span data-ttu-id="c8328-143">קטגוריית הוצאות</span><span class="sxs-lookup"><span data-stu-id="c8328-143">Expense Category</span></span>
  - <span data-ttu-id="c8328-144">מחיר תפקיד</span><span class="sxs-lookup"><span data-stu-id="c8328-144">Role Price</span></span>
  - <span data-ttu-id="c8328-145">מחיר קטגוריית עסקה</span><span class="sxs-lookup"><span data-stu-id="c8328-145">Transaction Category Price</span></span>
  - <span data-ttu-id="c8328-146">מאפיין</span><span class="sxs-lookup"><span data-stu-id="c8328-146">Characteristic</span></span>
  - <span data-ttu-id="c8328-147">משאב הניתן להזמנה</span><span class="sxs-lookup"><span data-stu-id="c8328-147">Bookable Resource</span></span>
  - <span data-ttu-id="c8328-148">קטגוריות משאבים הניתנים להזמנה</span><span class="sxs-lookup"><span data-stu-id="c8328-148">Bookable resource category Assn</span></span>
  - <span data-ttu-id="c8328-149">מאפיין של משאב הניתן להזמנה</span><span class="sxs-lookup"><span data-stu-id="c8328-149">Bookable Resource Characteristic</span></span>

![השלם את הייבוא](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="c8328-151">עדכן את התצורות של Project Operations</span><span class="sxs-lookup"><span data-stu-id="c8328-151">Update Project Operations configurations</span></span>

1. <span data-ttu-id="c8328-152">נווט אל סביבת CE.</span><span class="sxs-lookup"><span data-stu-id="c8328-152">Navigate to the CE environment.</span></span> <span data-ttu-id="c8328-153">אתה יכול למצוא אותה על-ידי פתיחת [מרכז הניהול של Power Platform](https://admin.powerplatform.microsoft.com/environments), בחירת הסביבה ואז בחירת האפשרות **פתח סביבה**.</span><span class="sxs-lookup"><span data-stu-id="c8328-153">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![פתח את הסביבה](./media/7OpenEnvironment.png)

2. <span data-ttu-id="c8328-155">כדי ליצור משאב הניתן להזמנה למשתמש שלך, עבור אל **פרויקטים** > **משאבים** ולאחר מכן בחר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="c8328-155">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![משאבים הניתנים להזמנה](./media/8BookableResources.png)

3. <span data-ttu-id="c8328-157">בכרטיסיה **כללי**, בחר את המשתמש שהוא מנהל המערכת שלך.</span><span class="sxs-lookup"><span data-stu-id="c8328-157">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="c8328-158">ודא שאזור הזמן תואם את זה שאתה נמצא בו.</span><span class="sxs-lookup"><span data-stu-id="c8328-158">Verify that the time zone matches the one you are in.</span></span> 

![משאב חדש הניתן להזמנה](./media/9NewBookableResource.png)

4. <span data-ttu-id="c8328-160">בכרטיסיה **תזמון**, בשדה **חברה**, בחר את החברה **USPM** ולאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="c8328-160">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![כרטיסיית תזמון](./media/10SchedulingTab.png)

5. <span data-ttu-id="c8328-162">בחר בכרטיסיה **שעות עבודה**.</span><span class="sxs-lookup"><span data-stu-id="c8328-162">Select the **Work hours** tab.</span></span>  

![שעות עבודה](./media/11WorkHours.png)

6. <span data-ttu-id="c8328-164">לחץ פעמיים על ערך כלשהו בלוח השנה ובחר **ערוך** > **כל האירועים בסדרה**.</span><span class="sxs-lookup"><span data-stu-id="c8328-164">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![לוח שנה של עבודה](./media/12WorkCalendar.png)

7. <span data-ttu-id="c8328-166">שנה את שעות העבודה לשמונה (8) שעות עבודה ביום, סמן סופי שבוע כימים שאינם ימי עבודה וכן וודא שאזור הזמן תואם לשלך.</span><span class="sxs-lookup"><span data-stu-id="c8328-166">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="c8328-167">בחר **שמור וסגור**.</span><span class="sxs-lookup"><span data-stu-id="c8328-167">Select **Save and close**.</span></span>

![עדכן לוח שנה](./media/13UpdateCalendar.png)

9. <span data-ttu-id="c8328-169">עבור אל **הגדרות** > **תבניות לוח שנה** ובחר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="c8328-169">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![תבניות לוח שנה](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="c8328-171">הזן שם, בחר את משאב התבנית שיצרת ולאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="c8328-171">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![שמור תבנית לוח שנה](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="c8328-173">עבור אל **פרמטרים** ולחץ פעמיים על הרשומה.</span><span class="sxs-lookup"><span data-stu-id="c8328-173">Go to **Parameters** and double-click the record.</span></span> 
 
 ![פרמטרי פרויקט](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="c8328-175">עדכן את השדות הבאים:</span><span class="sxs-lookup"><span data-stu-id="c8328-175">Update the following fields:</span></span>

 - <span data-ttu-id="c8328-176">**חברת ברירת מחדל**: USPM</span><span class="sxs-lookup"><span data-stu-id="c8328-176">**Default company**: USPM</span></span>
 - <span data-ttu-id="c8328-177">**יחידה ארגונית המוגדרת כברירת מחדל**: Contoso Robotics Global</span><span class="sxs-lookup"><span data-stu-id="c8328-177">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="c8328-178">**תדירות חשבונית**: היום השביעי והאחרון</span><span class="sxs-lookup"><span data-stu-id="c8328-178">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="c8328-179">**תבנית שעות עבודה**: שנה לתבנית שיצרת.</span><span class="sxs-lookup"><span data-stu-id="c8328-179">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="c8328-180">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="c8328-180">Select **Save**.</span></span> 

![עדכן פרמטרי פרויקט](./media/17UpdatedProjectParameters.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]