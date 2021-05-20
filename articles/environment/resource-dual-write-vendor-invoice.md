---
title: שילוב חשבונית ספק
description: נושא זה מספק מידע על שילו חשבוניות ספק ב- Project Operations.
author: sigitac
manager: Annbe
ms.date: 04/27/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 07839436c3777b0554e0721d250bff643e38c088
ms.sourcegitcommit: 02f00960198cc78a5e96955a9e4390c2c6393bbf
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/28/2021
ms.locfileid: "5955762"
---
# <a name="vendor-invoice-integration"></a><span data-ttu-id="a5da9-103">שילוב חשבונית ספק</span><span class="sxs-lookup"><span data-stu-id="a5da9-103">Vendor invoice integration</span></span>

<span data-ttu-id="a5da9-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="a5da9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="a5da9-105">ניתן לתעד רכש הקשור לפרויקט ב- Dynamics 365 Project Operations על ידי מעבר אל **חשבונות זכאים** > **חשבוניות** > **חשבוניות ספק בהמתנה** ושימוש במסמך חשבונית ספק בהמתנה.</span><span class="sxs-lookup"><span data-stu-id="a5da9-105">Project-related procurement in Dynamics 365 Project Operations can be recorded by going to **Accounts Payable** > **Invoices** > **Pending vendor invoices** and using a pending vendor invoice document.</span></span> <span data-ttu-id="a5da9-106">למידע נוסף ראה [רכוש חומרים שאינם במלאי באמצעות חשבונית ספק בהמתנה](../procurement/pending-vendor-invoices.md).</span><span class="sxs-lookup"><span data-stu-id="a5da9-106">For more information, see [Purchase non-stocked materials using a pending vendor invoice](../procurement/pending-vendor-invoices.md).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a5da9-107">לפני שתשתמש בפונקציונליות המתוארת בנושא זה, יש לסקור ולהחיל את התצורות הנדרשות.</span><span class="sxs-lookup"><span data-stu-id="a5da9-107">Before you use the functionality described in this topic, review and apply the required configurations.</span></span> <span data-ttu-id="a5da9-108">למידע נוסף ראה [הפוך חומרים שאינם במלאי וחשבונית ספק בהמתנה לזמינים](../procurement/configure-materials-nonstocked.md).</span><span class="sxs-lookup"><span data-stu-id="a5da9-108">For more information, see [Enable non-stocked materials and pending vendor invoices](../procurement/configure-materials-nonstocked.md).</span></span>

<span data-ttu-id="a5da9-109">ב- Project Operations, חשבוניו ספק הקשורות לפרויקט נרשמות לפי כללי רישום מיוחדים:</span><span class="sxs-lookup"><span data-stu-id="a5da9-109">In Project Operations, project-related vendor invoices are posted using special posting rules:</span></span>

- <span data-ttu-id="a5da9-110">עלות הקשורה לפרויקט (כולל מס שאינו בר-השבה) אינה נרשמת מיד בחשבון עלות הפרויקט בספר הראשי.</span><span class="sxs-lookup"><span data-stu-id="a5da9-110">Project-related cost (including non-recoverable tax) isn't immediately posted to the project cost account in the general ledger.</span></span> <span data-ttu-id="a5da9-111">במקום זאת, העלות נרשמת ב **חשבון שילוב רכש**.</span><span class="sxs-lookup"><span data-stu-id="a5da9-111">Instead, the cost is posted to the **Procurement integration account**.</span></span> <span data-ttu-id="a5da9-112">חשבון זה מוגדר ב **ניהול פרויקטים וחשבונאות** > **הגדרה** > **פרמטרים של ניהול פרויקטים חשבונאות**, ב **Project Operations בכרטיסיה Dynamics 365 Customer Engagement**.</span><span class="sxs-lookup"><span data-stu-id="a5da9-112">This account is configured in **Project management and accounting** > **Setup** > **Project management and accounting parameters** on the **Project Operations on Dynamics 365 Customer engagement** tab.</span></span>
- <span data-ttu-id="a5da9-113">כתיבה כפולה מסנכרנת את פרטי חשבונית הספק עם Microsoft Dataverse באמצעות מפות הטבלה הבאות:</span><span class="sxs-lookup"><span data-stu-id="a5da9-113">Dual-write synchronizes vendor invoice details to Microsoft Dataverse using the following table maps:</span></span>

     - <span data-ttu-id="a5da9-114">**ישות ייצוא חשבוניות ספק של פרויקט של שילוב של ‏Project Operations (‏‎msdyn_projectvendorinvoices‏)**: מפת טבלה זו מסנכרנת את פרטי כותרת חשבוניות הספק.</span><span class="sxs-lookup"><span data-stu-id="a5da9-114">**Project Operations integration project vendor invoice export entity (msdyn_projectvendorinvoices)**: This table map synchronizes vendor invoice header information.</span></span> <span data-ttu-id="a5da9-115">רק חשבוניות ספק עם שורה אחת לפחות המכילה מזהה פרויקט שמסונכרנות עם Dataverse.</span><span class="sxs-lookup"><span data-stu-id="a5da9-115">Only vendor invoices with at least one line that contains a project ID are synchronized to Dataverse.</span></span>
     - <span data-ttu-id="a5da9-116">**ישות ייצוא של שורת חשבוניות ספק של פרויקט שילוב של ‏Project Operations (‏‎msdyn_projectvendorinvoices‏)**: מפת טבלה זו מסנכרנת את פרטי כותרת חשבוניות הספק.</span><span class="sxs-lookup"><span data-stu-id="a5da9-116">**Project Operations integration project vendor invoice line export entity (msdyn_projectvendorinvoicelines)**: This table map synchronizes vendor invoice line information.</span></span> <span data-ttu-id="a5da9-117">רק שורות המכילות מזהה פרויקט מסונכרנות עם Dataverse.</span><span class="sxs-lookup"><span data-stu-id="a5da9-117">Only lines that contain a project ID are synchronized to Dataverse.</span></span>

     > [!NOTE]
     > <span data-ttu-id="a5da9-118">פרטי חשבונית הספק ב- Dataverse אינם ניתנים לעריכה.</span><span class="sxs-lookup"><span data-stu-id="a5da9-118">Vendor invoice details in Dataverse are not editable.</span></span>

<span data-ttu-id="a5da9-119">ספר משנה של מיסים, ספר משנה של ספקים, ורישומים פיננסיים נוספים נרשמים באופן המתאים ב- Dynamics 365 Finance בעת רישום חשבונית הספק.</span><span class="sxs-lookup"><span data-stu-id="a5da9-119">Tax subledger, vendor subledger, and other financial postings are recorded as applicable in Dynamics 365 Finance when the vendor invoice is posted.</span></span>

![שילוב חשבונית ספק](media/DW7VendorInvoice.png)

<span data-ttu-id="a5da9-121">כאשר רשומות נכתבות לישות **חשבונית ספק** ב- Dataverse, מתחיל תהליך אישור אוטומטי של הרשומות.</span><span class="sxs-lookup"><span data-stu-id="a5da9-121">When records are written to a **Vendor invoice** entity in Dataverse, an automated approval process of the records begins.</span></span> <span data-ttu-id="a5da9-122">במידת הצורך, ניתן לבחון את מצב תהליך האישור האוטומטי ב- Dataverse על ידי מעבר אל **הגדרות מתקדמות** > **מערכת** > **משימות מערכת**.</span><span class="sxs-lookup"><span data-stu-id="a5da9-122">If needed, the automated approval process status can be reviewed in Dataverse by going to **Advanced settings** > **System** > **System jobs**.</span></span> <span data-ttu-id="a5da9-123">לאחר השלמת האישור, רשומות מחלקת העסקאות 'חומרים' נוצרות בישות **נתונים בפועל**.</span><span class="sxs-lookup"><span data-stu-id="a5da9-123">After the approval is complete, the system creates material transaction class records in the **Actuals** entity.</span></span>

<span data-ttu-id="a5da9-124">נתונים בפועל הקשורים לחומרים מעובדות באמצעות מפת הטבלת הכתיבה הכפולה **נתוני שילוב בפעול של Project Operations‏ (msdyn_actuals)**.</span><span class="sxs-lookup"><span data-stu-id="a5da9-124">Material-related actuals are then processed using the dual-write table map, **Project Operations integration actuals (msdyn_actuals)**.</span></span> <span data-ttu-id="a5da9-125">לקבלת מידע נוסף, ראה [הערכות ונתונים בפועל של פרויקט](resource-dual-write-estimates-actuals.md).</span><span class="sxs-lookup"><span data-stu-id="a5da9-125">For more information, see [Project estimates and actuals](resource-dual-write-estimates-actuals.md).</span></span>

<span data-ttu-id="a5da9-126">התהליך התקופתי, **ייבא מאחסון זמני** יוצר שורות יומן הקשורות לחשבוניות ספק ביומן השילוב של Project Operations.</span><span class="sxs-lookup"><span data-stu-id="a5da9-126">The periodic process, **Import from staging** creates vendor invoice-related Project Operations integration journal lines.</span></span> <span data-ttu-id="a5da9-127">ברירת המחדל של החשבון הנגדי היא חשבון שילוב רכש.</span><span class="sxs-lookup"><span data-stu-id="a5da9-127">The offset account defaults to the procurement integration account.</span></span> <span data-ttu-id="a5da9-128">כשנרשם יומן השילוב, מנוקה יתרת החשבון עבור עסקת חשבונית הספק ומעביר את סכום השורה לחשבון עלות הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="a5da9-128">When the integration journal is posted, the account balance is cleared for the vendor invoice transaction and the line amount is moved to the project cost account.</span></span> <span data-ttu-id="a5da9-129">המערכת יוצרת גם עסקאות ספר משנה למטרות הנפקת חשבונית והכרה בהכנסות במורד הזרם.</span><span class="sxs-lookup"><span data-stu-id="a5da9-129">Project subledger transactions are also created for downstream invoicing and revenue recognition purposes.</span></span>
