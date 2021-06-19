---
title: עבודה עם הוצאות אישיות בדוח הוצאות
description: נושא זה מספק מידע על אופן העבודה עם הוצאות אישיות שהוצאו לעובדים בזמן נסיעה למטרות עסקיות.
author: suvaidya
ms.date: 05/11/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: ae25eca08089d224f1e17e95eeb571054de8a5c0
ms.sourcegitcommit: fd6e9ff78392c7bac35591d9130c00d2750438ae
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/12/2021
ms.locfileid: "6025685"
---
# <a name="work-with-personal-expenses-on-an-expense-report"></a><span data-ttu-id="b45dd-103">עבודה עם הוצאות אישיות בדוח הוצאות</span><span class="sxs-lookup"><span data-stu-id="b45dd-103">Work with personal expenses on an expense report</span></span>

<span data-ttu-id="b45dd-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="b45dd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b45dd-105">במהלך נסיעות עסקים, עובד עשוי לגבות הוצאות אישיות בכרטיס האשראי הארגוני שלו.</span><span class="sxs-lookup"><span data-stu-id="b45dd-105">During business travel, an employee might charge personal expenses to their corporate credit card.</span></span> <span data-ttu-id="b45dd-106">אם לא הוגדר תהליך לטיפול בהוצאות אישיות, תהליך אישור דוח ההוצאות עלול להיפגע כאשר עובד מגיש את דוח ההוצאות המפורט שלו.</span><span class="sxs-lookup"><span data-stu-id="b45dd-106">If a process hasn't been defined for handling personal expenses, the expense report approval process might be disrupted when an employee submits their itemized expense report.</span></span>

<span data-ttu-id="b45dd-107">ישנן שתי שיטות שבהן ניתן להשתמש כדי לעבוד עם הוצאות אישיות של העובד:</span><span class="sxs-lookup"><span data-stu-id="b45dd-107">There are two methods you can use to work with an employee's personal expenses:</span></span>

  - <span data-ttu-id="b45dd-108">**משולם על ידי עובד**: הארגון שלך לא משלם הוצאות אישיות המופיעות בחשבון עבור כרטיס האשראי הארגוני.</span><span class="sxs-lookup"><span data-stu-id="b45dd-108">**Paid by employee**: Your organization doesn't pay personal expenses that appear on the bill for the corporate credit card.</span></span> <span data-ttu-id="b45dd-109">במקום זאת, העובד משלם לספק כרטיסי האשראי ישירות עבור ההוצאות.</span><span class="sxs-lookup"><span data-stu-id="b45dd-109">Instead, the employee pays the credit card vendor directly for the expenses.</span></span> 
  - <span data-ttu-id="b45dd-110">**משולם על ידי החברה**: הארגון שלך משלם את החשבון המלא עבור כרטיס האשראי הארגוני, ואז מחייב את חשבון העובד בגין ההוצאות האישיות.</span><span class="sxs-lookup"><span data-stu-id="b45dd-110">**Paid by company**: Your organization pays the full bill for the corporate credit card, and then debits the worker's account for the personal expenses.</span></span>

<span data-ttu-id="b45dd-111">אתה יכול לבחור את השיטה שבה משתמש הארגון שלך בדף **פרמטרים לניהול הוצאות**.</span><span class="sxs-lookup"><span data-stu-id="b45dd-111">You can select the method that your organization uses on the **Expense management parameters** page.</span></span>


## <a name="enable-split-expense-function-when-personal-amount-field-has-value-defined"></a><span data-ttu-id="b45dd-112">הפעל פונקציית הוצאות מפוצלות כאשר מוגדר ערך בשדה הסכום האישי</span><span class="sxs-lookup"><span data-stu-id="b45dd-112">Enable split expense function when personal amount field has value defined</span></span>

<span data-ttu-id="b45dd-113">התכונה **הפעל פונקציית הוצאות מפוצלות כאשר מוגדר ערך בשדה הסכום האישי** חלה רק על דוחות הוצאות שאושרו באמצעות זרימת עבודה ברמת השורה.</span><span class="sxs-lookup"><span data-stu-id="b45dd-113">The feature, **Enable split expense function when personal amount field has value defined** only applies to expense reports that are approved using a line-level workflow.</span></span> <span data-ttu-id="b45dd-114">הדוחות מאושרים על ידי מעבר אל **עיבוד דוחות הוצאות** > **דוחות הוצאות שהוקצו לי** > **דוח הוצאות פתוח**.</span><span class="sxs-lookup"><span data-stu-id="b45dd-114">Reports are approved by going to **Process expense reports** > **Expense reports assigned to me** > **Open expense report**.</span></span> 

<span data-ttu-id="b45dd-115">כדי להפעיל תכונה זו, עבור אל **סביבות עבודה** > **ניהול תכונות**, בחר **הפעל פונקציית הוצאות מפוצלות כאשר מוגדר ערך בשדה הסכום האישי** ולאחר מכן בחר **הפעל עכשיו**.</span><span class="sxs-lookup"><span data-stu-id="b45dd-115">To enable this feature, go to **Workspaces** > **Feature Management**, select **Enable split expense function when personal amount field has value defined**, and then select **Enable now**.</span></span> 

<span data-ttu-id="b45dd-116">כאשר התכונה מופעלת, שורות הוצאות שמשתמשות בפונקציונליות זו מייצרות שתי שורות בעת הגשת הדוח.</span><span class="sxs-lookup"><span data-stu-id="b45dd-116">When the feature is enabled, expense lines that use this functionality generate two lines when the report is submitted.</span></span> <span data-ttu-id="b45dd-117">נוצרות שתי שורות כך שהמאשר יכול לאשר כל שורה בנפרד.</span><span class="sxs-lookup"><span data-stu-id="b45dd-117">Two lines are generated so that the approver can approve each line separately.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
