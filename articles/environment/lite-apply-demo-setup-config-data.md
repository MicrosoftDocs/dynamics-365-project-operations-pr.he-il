---
title: החלת נתוני ההדגמה והתצורה - לייט
description: נושא זה מספק מידע על אופן החלת הגדרת ההדגמה ונתוני התצורה עבור Project Operations.
author: sigitac
manager: Annbe
ms.date: 11/04/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5cfc270c07a568d692f6cd180b9c367ae185044c
ms.sourcegitcommit: 14aa380759214713d9bf560f5a7f619b7f4bd5b8
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 11/05/2020
ms.locfileid: "4401264"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a><span data-ttu-id="5f5e3-103">החל את נתוני ההדגמה והתצורה עבור Project Operations - לייט</span><span class="sxs-lookup"><span data-stu-id="5f5e3-103">Apply demo setup and configuration data for Project Operations - lite</span></span> 

<span data-ttu-id="5f5e3-104">_\*\*פריסת לייט - מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="5f5e3-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f5e3-105">דרישות מוקדמות</span><span class="sxs-lookup"><span data-stu-id="5f5e3-105">Prerequisites</span></span>

<span data-ttu-id="5f5e3-106">לפני שתתחיל בקביעת התצורה, צריך להיות לך סביבת Common Data Service ‏(CDS) שמוקצה עבור Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="5f5e3-106">Before you begin the configuration, you must have a Common Data Service (CDS) environment provisioned for Dynamics 365 Project Operations.</span></span>


## <a name="instructions"></a><span data-ttu-id="5f5e3-107">הוראות</span><span class="sxs-lookup"><span data-stu-id="5f5e3-107">Instructions</span></span>

1. <span data-ttu-id="5f5e3-108">הורד את [חבילת נתוני האב](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span><span class="sxs-lookup"><span data-stu-id="5f5e3-108">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="5f5e3-109">נווט לתיקיה *ProjOpsDemoDataSetupAndMaster - Integrated CMT* והפעל את קובץ ההפעלה, *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="5f5e3-109">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="5f5e3-110">בעמוד 1 של אשף הגדרת התצורה (CMT‏) של Common Data Service, בחר **ייבא נתונים** ואז בחר **המשך**.</span><span class="sxs-lookup"><span data-stu-id="5f5e3-110">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![‏‫העברת תצורה](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="5f5e3-112">בעמוד 2 של אשף ב-CMT בחר ב **Microsoft 365** כ **סוג הפריסה**.</span><span class="sxs-lookup"><span data-stu-id="5f5e3-112">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="5f5e3-113">בחר את תיבות הסימון **הצג רשימה של ארגונים זמינים** ו **הצג מתקדם**.</span><span class="sxs-lookup"><span data-stu-id="5f5e3-113">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="5f5e3-114">בחר את האזור של הדייר שלך, הזן את האישורים שלך ואז בחר **כניסה**.</span><span class="sxs-lookup"><span data-stu-id="5f5e3-114">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

![כניסת תצורה](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="5f5e3-116">בעמוד 3, מרשימת הארגונים בדייר, בחר לאיזה ארגון ברצונך לייבא את נתוני ההדגמה ואז בחר **כניסה**.</span><span class="sxs-lookup"><span data-stu-id="5f5e3-116">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="5f5e3-117">בעמוד 4 בחר את קובץ ה-zip, *MasterAndSetupData* מהתיקייה שפורקה, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span><span class="sxs-lookup"><span data-stu-id="5f5e3-117">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

![קובץ Zip](./media/3ZipFile.png)

![בחר קובץ](./media/4SelectAFile.png)

9. <span data-ttu-id="5f5e3-120">לאחר בחירת קובץ ה-zip בחר **ייבא נתונים**.</span><span class="sxs-lookup"><span data-stu-id="5f5e3-120">After the zip file is selected, select **Import Data**.</span></span>

![יבא נתונים](./media/5ImportData.png)

10. <span data-ttu-id="5f5e3-122">הייבוא יפעל בין שתיים לעשר דקות, תלוי במהירות הרשת שלך.</span><span class="sxs-lookup"><span data-stu-id="5f5e3-122">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="5f5e3-123">לאחר השלמת הייבוא, צא מאשף ה-CMT.</span><span class="sxs-lookup"><span data-stu-id="5f5e3-123">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="5f5e3-124">בדוק אם ישנם נתונים בארגון שלך ב-20 הישויות הבאות:</span><span class="sxs-lookup"><span data-stu-id="5f5e3-124">Check your organization for data in the following 20 entities:</span></span>

-   <span data-ttu-id="5f5e3-125">מטבע</span><span class="sxs-lookup"><span data-stu-id="5f5e3-125">Currency</span></span>
-   <span data-ttu-id="5f5e3-126">חשבון</span><span class="sxs-lookup"><span data-stu-id="5f5e3-126">Account</span></span>
-   <span data-ttu-id="5f5e3-127">יחידה ארגונית</span><span class="sxs-lookup"><span data-stu-id="5f5e3-127">Organizational Unit</span></span>
-   <span data-ttu-id="5f5e3-128">איש קשר</span><span class="sxs-lookup"><span data-stu-id="5f5e3-128">Contact</span></span>
-   <span data-ttu-id="5f5e3-129">קבוצת מיסים</span><span class="sxs-lookup"><span data-stu-id="5f5e3-129">Tax Group</span></span>
-   <span data-ttu-id="5f5e3-130">קבוצת לקוחות</span><span class="sxs-lookup"><span data-stu-id="5f5e3-130">Customer Group</span></span>
-   <span data-ttu-id="5f5e3-131">יחידה</span><span class="sxs-lookup"><span data-stu-id="5f5e3-131">Unit</span></span>
-   <span data-ttu-id="5f5e3-132">קבוצת יחידות</span><span class="sxs-lookup"><span data-stu-id="5f5e3-132">Unit Group</span></span>
-   <span data-ttu-id="5f5e3-133">מחירון</span><span class="sxs-lookup"><span data-stu-id="5f5e3-133">Price List</span></span>
-   <span data-ttu-id="5f5e3-134">מחירון פרמטרים של פרויקט</span><span class="sxs-lookup"><span data-stu-id="5f5e3-134">Project Parameter Price List</span></span> 
-   <span data-ttu-id="5f5e3-135">תדירות חשבונית</span><span class="sxs-lookup"><span data-stu-id="5f5e3-135">Invoice Frequency</span></span>
-   <span data-ttu-id="5f5e3-136">קטגוריית משאבים הניתנים להזמנה</span><span class="sxs-lookup"><span data-stu-id="5f5e3-136">Bookable Resource Category</span></span>
-   <span data-ttu-id="5f5e3-137">קטגוריית עסקה</span><span class="sxs-lookup"><span data-stu-id="5f5e3-137">Transaction Category</span></span>
-   <span data-ttu-id="5f5e3-138">קטגוריית הוצאות</span><span class="sxs-lookup"><span data-stu-id="5f5e3-138">Expense Category</span></span>
-   <span data-ttu-id="5f5e3-139">מחיר תפקיד</span><span class="sxs-lookup"><span data-stu-id="5f5e3-139">Role Price</span></span>
-   <span data-ttu-id="5f5e3-140">מחיר קטגוריית עסקה</span><span class="sxs-lookup"><span data-stu-id="5f5e3-140">Transaction Category Price</span></span>
-   <span data-ttu-id="5f5e3-141">מאפיין</span><span class="sxs-lookup"><span data-stu-id="5f5e3-141">Characteristic</span></span>
-   <span data-ttu-id="5f5e3-142">משאב הניתן להזמנה</span><span class="sxs-lookup"><span data-stu-id="5f5e3-142">Bookable Resource</span></span>
-   <span data-ttu-id="5f5e3-143">קטגוריות משאבים הניתנים להזמנה</span><span class="sxs-lookup"><span data-stu-id="5f5e3-143">Bookable resource category Assn</span></span>
-   <span data-ttu-id="5f5e3-144">מאפיין של משאב הניתן להזמנה</span><span class="sxs-lookup"><span data-stu-id="5f5e3-144">Bookable Resource Characteristic</span></span>

![השלם את הייבוא](./media/6CompleteImport.png)
