---
title: החל את הגדרת ההדגמה ואת נתוני התצורה
description: נושא זה מספק מידע על אופן החלת הגדרת ההדגמה ונתוני התצורה עבור Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 42e02f393e89d20b2a462645f519a3792bee8f2f
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948887"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations-lite-deployment---deal-to-proforma-invoicing"></a><span data-ttu-id="46ea7-103">החל את הגדרת ההדגמה ונתונה התצורה עבור פריסת לייט של Project Operations - מהעסקה ועד להוצאת חשבונית פרופורמה</span><span class="sxs-lookup"><span data-stu-id="46ea7-103">Apply demo setup and configuration data for Project Operations lite deployment - deal to proforma invoicing</span></span>

<span data-ttu-id="46ea7-104">_פריסת לייט - מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="46ea7-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

1. <span data-ttu-id="46ea7-105">הורד את [חבילת נתוני האב](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span><span class="sxs-lookup"><span data-stu-id="46ea7-105">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="46ea7-106">נווט לתיקיה *ProjOpsDemoDataSetupAndMaster - Integrated CMT* והפעל את קובץ ההפעלה, *DataMigrationUtility*.</span><span class="sxs-lookup"><span data-stu-id="46ea7-106">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="46ea7-107">בעמוד 1 של אשף הגדרת התצורה (CMT‏) של Common Data Service, בחר **ייבא נתונים** ואז בחר **המשך**.</span><span class="sxs-lookup"><span data-stu-id="46ea7-107">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![‏‫העברת תצורה](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="46ea7-109">בעמוד 2 של אשף ב-CMT בחר ב**Office 365** כ**סוג הפריסה**.</span><span class="sxs-lookup"><span data-stu-id="46ea7-109">On Page 2 of the CMT Wizard, select **Office 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="46ea7-110">בחר את תיבות הסימון **הצג רשימה של ארגונים זמינים** ו**הצג מתקדם**.</span><span class="sxs-lookup"><span data-stu-id="46ea7-110">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="46ea7-111">בחר את האזור של הדייר שלך, הזן את האישורים שלך ואז בחר **כניסה**.</span><span class="sxs-lookup"><span data-stu-id="46ea7-111">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

![כניסת תצורה](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="46ea7-113">בעמוד 3, מרשימת הארגונים בדייר, בחר לאיזה ארגון ברצונך לייבא את נתוני ההדגמה ואז בחר **כניסה**.</span><span class="sxs-lookup"><span data-stu-id="46ea7-113">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="46ea7-114">בעמוד 4 בחר את קובץ ה-zip, *MasterAndSetupData* מהתיקייה שפורקה, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span><span class="sxs-lookup"><span data-stu-id="46ea7-114">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

![קובץ Zip](./media/3ZipFile.png)

![בחר קובץ](./media/4SelectAFile.png)

9. <span data-ttu-id="46ea7-117">לאחר בחירת קובץ ה-zip בחר **ייבא נתונים**.</span><span class="sxs-lookup"><span data-stu-id="46ea7-117">After the zip file is selected, select **Import Data**.</span></span>

![יבא נתונים](./media/5ImportData.png)

10. <span data-ttu-id="46ea7-119">הייבוא יפעל בין שתיים לעשר דקות, תלוי במהירות הרשת שלך.</span><span class="sxs-lookup"><span data-stu-id="46ea7-119">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="46ea7-120">לאחר השלמת הייבוא, צא מאשף ה-CMT.</span><span class="sxs-lookup"><span data-stu-id="46ea7-120">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="46ea7-121">בדוק אם ישנם נתונים בארגון שלך ב-20 הישויות הבאות:</span><span class="sxs-lookup"><span data-stu-id="46ea7-121">Check your organization for data in the following 20 entities:</span></span>

- <span data-ttu-id="46ea7-122">מטבע</span><span class="sxs-lookup"><span data-stu-id="46ea7-122">Currency</span></span>
- <span data-ttu-id="46ea7-123">יחידה ארגונית</span><span class="sxs-lookup"><span data-stu-id="46ea7-123">Organizational Unit</span></span>
- <span data-ttu-id="46ea7-124">איש קשר</span><span class="sxs-lookup"><span data-stu-id="46ea7-124">Contact</span></span>
- <span data-ttu-id="46ea7-125">קבוצת מיסים</span><span class="sxs-lookup"><span data-stu-id="46ea7-125">Tax Group</span></span>
- <span data-ttu-id="46ea7-126">קבוצת לקוחות</span><span class="sxs-lookup"><span data-stu-id="46ea7-126">Customer Group</span></span>
- <span data-ttu-id="46ea7-127">יחידה</span><span class="sxs-lookup"><span data-stu-id="46ea7-127">Unit</span></span>
- <span data-ttu-id="46ea7-128">קבוצת יחידות</span><span class="sxs-lookup"><span data-stu-id="46ea7-128">Unit Group</span></span>
- <span data-ttu-id="46ea7-129">מחירון</span><span class="sxs-lookup"><span data-stu-id="46ea7-129">Price List</span></span>
- <span data-ttu-id="46ea7-130">מחירון פרמטרים של פרוייקט</span><span class="sxs-lookup"><span data-stu-id="46ea7-130">Project Parameter Price List</span></span>
- <span data-ttu-id="46ea7-131">תדירות חשבונית</span><span class="sxs-lookup"><span data-stu-id="46ea7-131">Invoice Frequency</span></span>
- <span data-ttu-id="46ea7-132">פרטי תדירות של הגשת חשבונית</span><span class="sxs-lookup"><span data-stu-id="46ea7-132">Invoice Frequency Detail</span></span>
- <span data-ttu-id="46ea7-133">קטגוריית משאבים הניתנים להזמנה</span><span class="sxs-lookup"><span data-stu-id="46ea7-133">Bookable Resource Category</span></span>
- <span data-ttu-id="46ea7-134">קטגוריית עסקה</span><span class="sxs-lookup"><span data-stu-id="46ea7-134">Transaction Category</span></span>
- <span data-ttu-id="46ea7-135">קטגוריית הוצאות</span><span class="sxs-lookup"><span data-stu-id="46ea7-135">Expense Category</span></span>
- <span data-ttu-id="46ea7-136">מחיר תפקיד</span><span class="sxs-lookup"><span data-stu-id="46ea7-136">Role Price</span></span>
- <span data-ttu-id="46ea7-137">מחיר קטגוריית עסקה</span><span class="sxs-lookup"><span data-stu-id="46ea7-137">Transaction Category Price</span></span>
- <span data-ttu-id="46ea7-138">מאפיין</span><span class="sxs-lookup"><span data-stu-id="46ea7-138">Characteristic</span></span>
- <span data-ttu-id="46ea7-139">משאב הניתן להזמנה</span><span class="sxs-lookup"><span data-stu-id="46ea7-139">Bookable Resource</span></span>
- <span data-ttu-id="46ea7-140">קטגוריות משאבים הניתנים להזמנה</span><span class="sxs-lookup"><span data-stu-id="46ea7-140">Bookable resource category Assn</span></span>
- <span data-ttu-id="46ea7-141">מאפיין של משאב הניתן להזמנה</span><span class="sxs-lookup"><span data-stu-id="46ea7-141">Bookable Resource Characteristic</span></span>

![השלם את הייבוא](./media/6CompleteImport.png)