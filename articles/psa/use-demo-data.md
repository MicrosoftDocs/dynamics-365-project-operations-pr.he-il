---
title: התנסות בנתוני הדגמה
description: כיצד להוריד נתוני הדגמה עבור Project Service Automation ולהתנסות עמם
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 5445095f0583caf80882568adcdbaede98882f72
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5281614"
---
# <a name="experiment-with-demo-data-project-service"></a><span data-ttu-id="b1503-103">התנסות בנתוני הדגמה‬‏‫ (Project Service)</span><span class="sxs-lookup"><span data-stu-id="b1503-103">Experiment with demo data (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="b1503-104">כדי להכיר את Dynamics 365 Project Service Automation, כדאי שתהיה לך סביבה מוגדרת מראש שתרצה להכיר.</span><span class="sxs-lookup"><span data-stu-id="b1503-104">To become familiar with Dynamics 365 Project Service Automation, it’s useful to have a pre-configured environment to explore.</span></span> <span data-ttu-id="b1503-105">למטרה זו, יצרנו חבילת התקנה נפרדת עם נתונים לדוגמה (באנגלית בלבד לעת עתה) המקלה על הכרת פתרונות אלה.</span><span class="sxs-lookup"><span data-stu-id="b1503-105">For this purpose, we’ve created a separate sample data installation package (English-language only at this time) that makes it easier to learn about these solutions.</span></span> 

<span data-ttu-id="b1503-106">חבילת ההתקנה זמינה ב: [מרכז ההורדות של Microsoft](https://go.microsoft.com/fwlink/?linkid=859966).</span><span class="sxs-lookup"><span data-stu-id="b1503-106">The installation package is available on the [Microsoft Download Center](https://go.microsoft.com/fwlink/?linkid=859966).</span></span>  

<span data-ttu-id="b1503-107">הפעלת ההתקנה של Package Deployer מבצעת את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="b1503-107">Running the Package Deployer install performs the following actions:</span></span> 
  
-   <span data-ttu-id="b1503-108">יוצרת או מגדירה פרמטרי ברירת מחדל שמכתיבים אופן פעולה של Project Service</span><span class="sxs-lookup"><span data-stu-id="b1503-108">Creates or sets default parameters that drive behavior of Project Service</span></span>  
  
-   <span data-ttu-id="b1503-109">מייבאת נתונים לדוגמה, כגון משאבים הניתנים להזמנה, תפקידים, מכירות ומחירונים, יחידות ארגוניות, רשומות רלוונטיות של תהליכי מכירות, הזמנות עבודה ופרויקטים</span><span class="sxs-lookup"><span data-stu-id="b1503-109">Imports sample data such as Bookable Resources, Roles, Sales and Cost Price lists, Organizational Units, relevant sales process records, Work Orders and Projects</span></span>    
  
> [!IMPORTANT]
> <span data-ttu-id="b1503-110">**אין דרך להסיר את התקנת נתוני ההדגמה.**</span><span class="sxs-lookup"><span data-stu-id="b1503-110">**There is no way to un-install the demo data.**</span></span> <span data-ttu-id="b1503-111">לכן, עליך להשתמש בחבילה זו רק במערכות הדגמה, הערכה, הדרכה ובדיקה.</span><span class="sxs-lookup"><span data-stu-id="b1503-111">Therefore, you should only use this package on demonstration, evaluation, training and test systems.</span></span>

<span data-ttu-id="b1503-112">לקבלת מידע נוסף, ראה [בלוג](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data) זה.</span><span class="sxs-lookup"><span data-stu-id="b1503-112">For more information, see this [blog](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data).</span></span>





  
### <a name="see-also"></a><span data-ttu-id="b1503-113">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="b1503-113">See Also</span></span>  
 <span data-ttu-id="b1503-114">[מדריך למנהל מערכת](../psa/admin-guide.md) </span><span class="sxs-lookup"><span data-stu-id="b1503-114">[Administrator Guide](../psa/admin-guide.md) </span></span>  
 <span data-ttu-id="b1503-115">[מדריך למנהלי תיקי לקוחות](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="b1503-115">[Account Manager Guide](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="b1503-116">[מדריך למנהל פרויקט](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="b1503-116">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 <span data-ttu-id="b1503-117">[מדריך למנהל משאבים](../psa/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="b1503-117">[Resource Manager Guide](../psa/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="b1503-118">‏‫מדריך בנושאי זמן, הוצאות ושיתוף פעולה</span><span class="sxs-lookup"><span data-stu-id="b1503-118">Time, Expense, and Collaboration Guide</span></span>](../psa/time-expense-collaboration-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]