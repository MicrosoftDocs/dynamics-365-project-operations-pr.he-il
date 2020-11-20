---
title: יצירת חשבונית פרופורמה ידנית - לייט
description: נושא זה מספק מידע על יצירת חשבוניות פרופורמה ידנית ב-Project Operations.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 87ef090454b2a7ab997e7c21d8d10badc31c8235
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176387"
---
# <a name="create-a-manual-proforma-invoice---lite"></a><span data-ttu-id="c1a72-103">יצירת חשבונית פרופורמה ידנית - לייט</span><span class="sxs-lookup"><span data-stu-id="c1a72-103">Create a manual proforma invoice - lite</span></span>

<span data-ttu-id="c1a72-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="c1a72-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c1a72-105">ב-Dynamics 365 Project Operations, ניתן ליצור חשבוניות פרופורמה באופן ידני לפי הצורך.</span><span class="sxs-lookup"><span data-stu-id="c1a72-105">In Dynamics 365 Project Operations, proforma invoices can be created manually as needed.</span></span> <span data-ttu-id="c1a72-106">ניתן ליצור ידנית חשבונית פרופורמה מדף הרשימה של **חוזי פרויקט** או מדף הפרטים של **חוזה פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="c1a72-106">You can manually create a proforma invoice from the **Project Contracts** list page or from the **Project Contract** details page.</span></span>

##  <a name="project-contracts-list-page"></a><span data-ttu-id="c1a72-107">דף הרשימה של חוזי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="c1a72-107">Project Contracts list page</span></span>

<span data-ttu-id="c1a72-108">בדף הרשימה של **חוזי פרויקט**, בחר חוזה פרויקט אחד או יותר וצור חשבוניות עבור כל הרשומות שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="c1a72-108">From **Project Contracts** list page, select one or more project contracts, and create invoices for all of the selected records.</span></span>

<span data-ttu-id="c1a72-109">המערכת בודקת לאילו מחוזי הפרויקט שנבחרו יש מצבור פרטי עבודה ש **מוכן לחשבונית** המתוארך לפני התאריך של היום.</span><span class="sxs-lookup"><span data-stu-id="c1a72-109">The system checks to see which of the selected project contracts has a **Ready to Invoice** backlog  dated before today's date.</span></span> <span data-ttu-id="c1a72-110">מאותם החוזים, המערכת יוצרת טיוטת של חשבוניות פרופורמה.</span><span class="sxs-lookup"><span data-stu-id="c1a72-110">From those contracts, the system creates draft proforma invoices.</span></span> <span data-ttu-id="c1a72-111">אם לחוזה פרויקט מספר לקוחות, יתכן שייווצר חשבונית אחת לכל לקוח, וחשבוניות מרובות לכל חוזה פרויקט.</span><span class="sxs-lookup"><span data-stu-id="c1a72-111">If a project contract has multiple customers, there may be one invoice created per customer, and multiple invoices per project contract.</span></span>

<span data-ttu-id="c1a72-112">כל חשבוניות הפרויקט שנוצרו זמינות בדף **חשבונית** במקטע **חיוב** של האזור **מכירות**.</span><span class="sxs-lookup"><span data-stu-id="c1a72-112">All of the created project invoices are available on the **Invoice** page in the **Billing** section of the **Sales** area.</span></span>

## <a name="project-contract-details-page"></a><span data-ttu-id="c1a72-113">דף פרטי סעיף חוזה של פרויקט</span><span class="sxs-lookup"><span data-stu-id="c1a72-113">Project Contract details page</span></span>

<span data-ttu-id="c1a72-114">ניתן ליצור חשבונית פרופורמה מדף הפרטים של **חוזה פרויקט**, היוצר את החשבונית עבור אותו חוזה פרויקט ספציפי.</span><span class="sxs-lookup"><span data-stu-id="c1a72-114">A proforma invoice can also be created from the **Project Contract** details page, which creates the invoice for that specific project contract.</span></span> <span data-ttu-id="c1a72-115">המערכת מאמתת שלחוזה הפרויקט יש מצבור פרטי עבודה ש **מוכן לחשבונית** המתוארך לפני התאריך של היום.</span><span class="sxs-lookup"><span data-stu-id="c1a72-115">The system verifies that the project contract has a **Ready to Invoice** backlog that is dated before today's date.</span></span> <span data-ttu-id="c1a72-116">מתוך חוזים אלה המערכת יוצרת טיוטת של חשבוניות פרופורמה המבוססות על מספר הלקוחות בכל סעיף חוזה.</span><span class="sxs-lookup"><span data-stu-id="c1a72-116">From these contracts, the system creates draft proforma invoices based on the number of customers on each contract line.</span></span>

<span data-ttu-id="c1a72-117">כאשר נוצרת חשבונית פרופורמה בודדת, הדף **חשבונית** נפתח.</span><span class="sxs-lookup"><span data-stu-id="c1a72-117">When there's a single proforma invoice created, the **Invoice** page opens.</span></span> <span data-ttu-id="c1a72-118">אם נוצרות מספר חשבוניות עבור חוזה הפרויקט המדובר, דף רשימת ה **חשבוניות** נפתח כדי להציג את כל החשבוניות שנוצרו.</span><span class="sxs-lookup"><span data-stu-id="c1a72-118">If there are multiple invoices created for that project contract, then the **Invoices** list page opens to show all of the created invoices.</span></span>
