---
title: התנסות בנתוני הדגמה
description: כיצד להוריד נתוני הדגמה עבור Project Service Automation ולהתנסות עמם
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: b195e5c8-63bc-4e90-914c-f29b8d565942
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 76dd5ff14cbafbfc5341885f0469a6e3e71dd66f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751839"
---
# <a name="experiment-with-demo-data-project-service"></a><span data-ttu-id="ae93c-103">התנסות בנתוני הדגמה‬‏‫ (Project Service)</span><span class="sxs-lookup"><span data-stu-id="ae93c-103">Experiment with demo data (Project Service)</span></span>

<span data-ttu-id="ae93c-104">כדי להכיר את Dynamics 365 Project Service Automation, כדאי שתהיה לך סביבה מוגדרת מראש שתרצה להכיר.</span><span class="sxs-lookup"><span data-stu-id="ae93c-104">To become familiar with Dynamics 365 Project Service Automation, it’s useful to have a pre-configured environment to explore.</span></span> <span data-ttu-id="ae93c-105">למטרה זו, יצרנו חבילת התקנה נפרדת עם נתונים לדוגמה (באנגלית בלבד לעת עתה) המקלה על הכרת פתרונות אלה.</span><span class="sxs-lookup"><span data-stu-id="ae93c-105">For this purpose, we’ve created a separate sample data installation package (English-language only at this time) that makes it easier to learn about these solutions.</span></span> 

<span data-ttu-id="ae93c-106">חבילת ההתקנה זמינה ב: [מרכז ההורדות של Microsoft](https://go.microsoft.com/fwlink/?linkid=859966).</span><span class="sxs-lookup"><span data-stu-id="ae93c-106">The installation package is available on the [Microsoft Download Center](https://go.microsoft.com/fwlink/?linkid=859966).</span></span>  

<span data-ttu-id="ae93c-107">הפעלת ההתקנה של Package Deployer מבצעת את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="ae93c-107">Running the Package Deployer install performs the following actions:</span></span> 
  
-   <span data-ttu-id="ae93c-108">יוצרת או מגדירה פרמטרי ברירת מחדל שמכתיבים אופן פעולה של Project Service</span><span class="sxs-lookup"><span data-stu-id="ae93c-108">Creates or sets default parameters that drive behavior of Project Service</span></span>  
  
-   <span data-ttu-id="ae93c-109">מייבאת נתונים לדוגמה, כגון משאבים הניתנים להזמנה, תפקידים, מכירות ומחירונים, יחידות ארגוניות, רשומות רלוונטיות של תהליכי מכירות, הזמנות עבודה ופרוייקטים</span><span class="sxs-lookup"><span data-stu-id="ae93c-109">Imports sample data such as Bookable Resources, Roles, Sales and Cost Price lists, Organizational Units, relevant sales process records, Work Orders and Projects</span></span>    
  
> [!IMPORTANT]
> <span data-ttu-id="ae93c-110">**אין דרך להסיר את התקנת נתוני ההדגמה.**</span><span class="sxs-lookup"><span data-stu-id="ae93c-110">**There is no way to un-install the demo data.**</span></span> <span data-ttu-id="ae93c-111">לכן, עליך להשתמש בחבילה זו רק במערכות הדגמה, הערכה, הדרכה ובדיקה.</span><span class="sxs-lookup"><span data-stu-id="ae93c-111">Therefore, you should only use this package on demonstration, evaluation, training and test systems.</span></span>

<span data-ttu-id="ae93c-112">לקבלת מידע נוסף, ראה [בלוג](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data) זה.</span><span class="sxs-lookup"><span data-stu-id="ae93c-112">For more information, see this [blog](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data).</span></span>





  
### <a name="see-also"></a><span data-ttu-id="ae93c-113">למידע נוסף</span><span class="sxs-lookup"><span data-stu-id="ae93c-113">See Also</span></span>  
 <span data-ttu-id="ae93c-114">[מדריך למנהל מערכת](../project-service/admin-guide.md) </span><span class="sxs-lookup"><span data-stu-id="ae93c-114">[Administrator Guide](../project-service/admin-guide.md) </span></span>  
 <span data-ttu-id="ae93c-115">[מדריך למנהלי תיקי לקוחות](../project-service/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="ae93c-115">[Account Manager Guide](../project-service/account-manager-guide.md) </span></span>  
 <span data-ttu-id="ae93c-116">[מדריך למנהל פרוייקט](../project-service/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="ae93c-116">[Project Manager Guide](../project-service/project-manager-guide.md) </span></span>  
 <span data-ttu-id="ae93c-117">[מדריך למנהל משאבים](../project-service/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="ae93c-117">[Resource Manager Guide](../project-service/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="ae93c-118">‏‫מדריך בנושאי זמן, הוצאות ושיתוף פעולה</span><span class="sxs-lookup"><span data-stu-id="ae93c-118">Time, Expense, and Collaboration Guide</span></span>](../project-service/time-expense-collaboration-guide.md)
