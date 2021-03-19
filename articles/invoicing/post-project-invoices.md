---
title: מבט כולל על תהליך הוצאת חשבוניות
description: נושא זה מספק סקירה כללית על הפקת חשבוניות ב- Project Operations עבור תרחישים מבוססי משאבים/ללא מלאי.
author: sigitac
manager: Annbe
ms.date: 01/29/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 9dc424cf69abfccc10bf551272a14e5cefb3dff0
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5275808"
---
# <a name="invoicing-process-overview"></a><span data-ttu-id="074f8-103">מבט כולל על תהליך הוצאת חשבוניות</span><span class="sxs-lookup"><span data-stu-id="074f8-103">Invoicing process overview</span></span>

<span data-ttu-id="074f8-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="074f8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="074f8-105">Project Operations לתרחישים מבוססי משאבים/ללא מלאי מציע יכולות מקיפות המותאמות לצרכים של מנהל הפרוייקט ושל פקיד החשבונות/רואה החשבון של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="074f8-105">Project Operations for resource/non-stocked based scenarios offers comprehensive capabilities tailored to fit the needs of both Project manager and Accounts receivable clerk/project accountant.</span></span> <span data-ttu-id="074f8-106">בתהליך הפקת החשבונית מנהל הפרוייקט מנהל את צבר החיובים בפרוייקט ומנהל החשבונות/החשב של הפרוייקט יוצר מסמך חשבוניות תואם ומדויק שמיועד ללקוח.</span><span class="sxs-lookup"><span data-stu-id="074f8-106">For the invoicing process, the Project manager manages the project billing backlog and the Accounts receivable clerk/project accountant creates a compliant and accurate customer-facing invoice document.</span></span>

![תרשים זרימה של הפקת חשבונית](./media/invoicing-flow.png)

<span data-ttu-id="074f8-108">סעיף חוזה הפרוייקט מגדיר את שיטת החיוב עבור עסקאות פרוייקט משויכות.</span><span class="sxs-lookup"><span data-stu-id="074f8-108">The project contract line defines the billing method for associated project transactions.</span></span> <span data-ttu-id="074f8-109">כאשר מנהל הפרוייקט מאשר עסקאות זמן והוצאות, המערכת רושמת את העסקאות בישות **פרוייקטים אמיתיים** ושולחת את המידע אל המודול **ניהול פרוייקטים וחשבונאות** ב- Dynamics 365 Finance.</span><span class="sxs-lookup"><span data-stu-id="074f8-109">When the Project manager approves time and expense transactions, the system records the transactions in the **Project Actuals** entity and sends the information to the **Project management and accounting** module in Dynamics 365 Finance.</span></span> <span data-ttu-id="074f8-110">חשב הפרוייקט סוקר ומפרסם את הרשומות באמצעות [יומן השילוב של Project Operations](../project-accounting/project-operations-integration-journal.md).</span><span class="sxs-lookup"><span data-stu-id="074f8-110">The Project accountant then reviews and posts the records using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="074f8-111">יומן זה כולל פרטים חשבונאיים חשובים עבור הנתונים בפועל של הפרוייקט, כגון חיוב, קבוצת מס מכירה, קבוצת מס מכירות של פריטי חיוב וממדים פיננסיים.</span><span class="sxs-lookup"><span data-stu-id="074f8-111">This journal includes important accounting details for project actuals, such as billing, sales tax group, billing item sales tax group, and financial dimensions.</span></span>

<span data-ttu-id="074f8-112">מנהל הפרוייקט יכול לבדוק עסקאות מכירה שלא בוצעו באמצעות שיטת החיוב בזמן ובחומר ב- [מצבור חיובי זמן וחומר](../proforma-invoicing/manage-billing-backlog.md#time-and-material-billing-backlog) וחיוב במחיר קבוע ב- [אבני דרך של מחיר קבוע](../proforma-invoicing/manage-billing-backlog.md#fixed-price-milestones).</span><span class="sxs-lookup"><span data-stu-id="074f8-112">The Project manager can review unbilled sales transactions using the time and material billing method in the [Time and material billing backlog](../proforma-invoicing/manage-billing-backlog.md#time-and-material-billing-backlog) and fixed price billing in [Fixed price milestones](../proforma-invoicing/manage-billing-backlog.md#fixed-price-milestones).</span></span> <span data-ttu-id="074f8-113">תצוגות אלו מאפשרות לך לסנן ולבחור עסקאות שצריכות להיכלל במחזור החיוב הבא ואז לסמן אותן **מוכנות לחשבונית**.</span><span class="sxs-lookup"><span data-stu-id="074f8-113">These views allow you to filter and select transactions that need to be included in the next billing cycle and then mark them as **Ready to Invoice**.</span></span>

<span data-ttu-id="074f8-114">אתה יכול [ליצור ידנית חשבונית פרופורמה](../proforma-invoicing/create-manual-proforma-invoice.md) או להשתמש ב- [תהליך תקופתי](../proforma-invoicing/configure-automated-invoice-creation.md).</span><span class="sxs-lookup"><span data-stu-id="074f8-114">You can [manually create a proforma invoice](../proforma-invoicing/create-manual-proforma-invoice.md) or use a [periodic process](../proforma-invoicing/configure-automated-invoice-creation.md).</span></span> <span data-ttu-id="074f8-115">מנהל הפרוייקט יכול [להתאים טיוטת חשבונית פרופורמה](../proforma-invoicing/manage-proforma-invoice.md) לפי הצורך ואז לאשר זאת.</span><span class="sxs-lookup"><span data-stu-id="074f8-115">The Project manager can [adjust a draft proforma invoice](../proforma-invoicing/manage-proforma-invoice.md) as needed and then confirm it.</span></span>

<span data-ttu-id="074f8-116">חשבונית הפרופורמה שאושרה נשלחת למודול **ניהול פרוייקטים וחשבונאות** ב- Finance.</span><span class="sxs-lookup"><span data-stu-id="074f8-116">The confirmed proforma invoice is sent to the **Project management and accounting** module in Finance.</span></span> <span data-ttu-id="074f8-117">רואה החשבון של הפרוייקט מעצב ומעדכן את הצעת חשבונית הפרוייקט, ואז מפרסם ומדפיס את המסמך.</span><span class="sxs-lookup"><span data-stu-id="074f8-117">The Project accountant formats and updates the project invoice proposal, and then posts and prints the document.</span></span> <span data-ttu-id="074f8-118">חשבוניות פרוייקט שפורסמו נרשמות בספר החשבונות הכללי, וכן בספרי המשנה של הלקוח ושל הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="074f8-118">Posted project invoices are recorded in the General ledger, as well as the Customer and Project subledgers.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]