---
title: רכישת חומרים שאינם במלאי באמצעות חשבוניות ספק בהמתנה
description: נושא זה מסביר כיצד לתעד חשבוניות ספק בהמתנה.
author: sigitac
ms.date: 04/12/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b5e6632d73c8a211b1f0d568be8e10ef47be77e2
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993795"
---
# <a name="purchase-non-stocked-materials-using-a-pending-vendor-invoice"></a><span data-ttu-id="4b6db-103">רכישת חומרים שאינם במלאי באמצעות חשבוניות ספק בהמתנה</span><span class="sxs-lookup"><span data-stu-id="4b6db-103">Purchase non-stocked materials using a pending vendor invoice</span></span>

<span data-ttu-id="4b6db-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="4b6db-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="4b6db-105">כשחברה רוכשת חומרים שאינם במלאי לפרויקט, ניתן לרשום את העלויות כנגד הפרויקט באופן מיידי.</span><span class="sxs-lookup"><span data-stu-id="4b6db-105">As a company procures non-stocked materials for a project, the costs can be immediately recorded against the project.</span></span> 

<span data-ttu-id="4b6db-106">לדוגמה, Contoso Robotics USמבצעת פרויקט חידוש ציוד וזקוקה לרישיונות תוכנה.</span><span class="sxs-lookup"><span data-stu-id="4b6db-106">For example, Contoso Robotics US is performing an equipment renewal project and needs software licenses.</span></span> <span data-ttu-id="4b6db-107">רישיונות אלה נרכשים מספק צד שלישי.</span><span class="sxs-lookup"><span data-stu-id="4b6db-107">These licenses are procured from a third-party vendor.</span></span>  <span data-ttu-id="4b6db-108">באמצעות Dynamics 365 Finance, פקיד החשבונות זכאים מתעד מסמך חשבונית ספק בהמתנה ומייחס את עלויות הרישיון ישירות כנגד פרויקט חידוש הציוד.</span><span class="sxs-lookup"><span data-stu-id="4b6db-108">Using Dynamics 365 Finance, the Accounts payable clerk records a pending vendor invoice document and attributes the license costs directly against the equipment renewal project.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="4b6db-109">לפני שתשתמש בפונקציונליות המתוארת בנושא זה, יש לסקור ולהחיל את התצורות הנדרשות.</span><span class="sxs-lookup"><span data-stu-id="4b6db-109">Before you use the functionality described in this topic, review and apply the required configurations.</span></span> <span data-ttu-id="4b6db-110">למידע נוסף ראה [הפוך חומרים שאינם במלאי וחשבונית ספק בהמתנה לזמינים](configure-materials-nonstocked.md).</span><span class="sxs-lookup"><span data-stu-id="4b6db-110">For more information, see [Enable non-stocked materials and pending vendor invoices](configure-materials-nonstocked.md).</span></span> 

## <a name="post-a-project-related-pending-vendor-invoice"></a><span data-ttu-id="4b6db-111">רישום חשבונית ספק בהמתנה שקשורה לפרויקט</span><span class="sxs-lookup"><span data-stu-id="4b6db-111">Post a project-related pending vendor invoice</span></span> 

<span data-ttu-id="4b6db-112">ניתן לתעד חשבוניות ספק בהמתנה בדף **חשבוניות ספק בהמתנה** (**חשבונות זכאים** > **חשבוניות** > **חשבוניות ספק בהמתנה**).</span><span class="sxs-lookup"><span data-stu-id="4b6db-112">Pending vendor invoices can be recorded on the **Pending vendor invoices** page (**Accounts payable** > **Invoices** > **Pending vendor invoices**).</span></span> <span data-ttu-id="4b6db-113">בצע את השלבים הבאים כדי לרשום חשבונית ספק בהמתנה הקשורה לפרויקט:</span><span class="sxs-lookup"><span data-stu-id="4b6db-113">Complete the following steps to post a project-related pending vendor invoice:</span></span>

1. <span data-ttu-id="4b6db-114">עבור אל **חשבונות זכאים** > **חשבוניות** ובחר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="4b6db-114">Go to **Accounts payable** > **Invoices** and select **New**.</span></span> 
2. <span data-ttu-id="4b6db-115">בשדה **חשבון חשבונית** בחר ספק ובשדה **מספר**, הזן את מזהה חשבונית הספק.</span><span class="sxs-lookup"><span data-stu-id="4b6db-115">In the **Invoice account** field, select a vendor and in the **Number** field, enter the vendor invoice identification.</span></span>
3. <span data-ttu-id="4b6db-116">הוסף שורה לחשבונית הספק ובשדה **מספר פריט** בחר את הפריט שאינו מצויד במלאי שנרכש מהספק.</span><span class="sxs-lookup"><span data-stu-id="4b6db-116">Add a line to the vendor invoice and in the **Item number** field, select the non-stocked item purchased from the vendor.</span></span> 

    > [!NOTE]
    > <span data-ttu-id="4b6db-117">לא ניתן לתעד שורות חשבוניות ספק המבוססות על קטגוריית רכש כנגד הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="4b6db-117">Vendor invoice lines that are based on a procurement category can't be recorded against the project.</span></span> 
    
5. <span data-ttu-id="4b6db-118">הוסף את הכמות שנרכשה.</span><span class="sxs-lookup"><span data-stu-id="4b6db-118">Add the quantity purchased.</span></span> <span data-ttu-id="4b6db-119">המערכת תאכלס את מחיר היחידה בהתבסס על תצורת מחירי הפריטים שאינם במלאי.</span><span class="sxs-lookup"><span data-stu-id="4b6db-119">The system will populate the unit price based on the non-stocked item price configuration.</span></span> 
6. <span data-ttu-id="4b6db-120">אמת את הסכום הכולל ופרטים אחרים שנדרשים בשורה.</span><span class="sxs-lookup"><span data-stu-id="4b6db-120">Verify the total amount and other required details on the line.</span></span>
7. <span data-ttu-id="4b6db-121">על פרטי השורה, בכרטיסיה **פרויקט** בחר את מזהה הפרויקט שבו יתועד פריט זה.</span><span class="sxs-lookup"><span data-stu-id="4b6db-121">On the line details, on the **Project** tab, select the ID of the project that this item will be recorded to.</span></span>
8. <span data-ttu-id="4b6db-122">לחלופין, אפשר לבחור את מספר הפעילות ולעדכן את קטגוריית הפרויקט ומאפיין השורה.</span><span class="sxs-lookup"><span data-stu-id="4b6db-122">Optionally, select the activity number, and update the project category and line property.</span></span>
9. <span data-ttu-id="4b6db-123">רישום חשבונית ספק בהמתנה.</span><span class="sxs-lookup"><span data-stu-id="4b6db-123">Post pending vendor invoice.</span></span> <span data-ttu-id="4b6db-124">כאשר החשבונית נרשמת, המערכת מתעדת את:</span><span class="sxs-lookup"><span data-stu-id="4b6db-124">When the invoice is posted, the system records:</span></span>
    
    - <span data-ttu-id="4b6db-125">סכום יתרת הספק.</span><span class="sxs-lookup"><span data-stu-id="4b6db-125">The vendor balance amount.</span></span>
    - <span data-ttu-id="4b6db-126">סכום המע"מ.</span><span class="sxs-lookup"><span data-stu-id="4b6db-126">The sales tax amount.</span></span>
    - <span data-ttu-id="4b6db-127">העלות כנגד הפרויקט נרשמת בחשבון שילוב הרכש.</span><span class="sxs-lookup"><span data-stu-id="4b6db-127">The cost against the project is recorded to the procurement integration account.</span></span>
    - <span data-ttu-id="4b6db-128">העסקה בפועל של הפרויקט ב- Dataverse.</span><span class="sxs-lookup"><span data-stu-id="4b6db-128">The project actual transaction in Dataverse.</span></span> <span data-ttu-id="4b6db-129">עיבוד נוסף של עסקה זו מתבצע באמצעות [יומן השילוב של Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="4b6db-129">This transaction is further processed using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="4b6db-130">רישום ביומן זה מעביר את הסכום מחשבון שילוב הרכש לחשבון עלות הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="4b6db-130">Posting this journal moves the amount from the procurement integration account to the project cost account.</span></span>
