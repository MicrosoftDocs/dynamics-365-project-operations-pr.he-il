---
title: קביעת התצורה של חשבונאות לפרוייקטים פנימיים
description: נושא זה מספק מידע על אופן הגדרת נוהלי חשבונאות עבור פרויקטים פנימיים ב-Project Operations.
author: sigitac
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 504e7481cb2aee6310cb4ace2d0791d1c7fe360d
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077242"
---
# <a name="configure-accounting-for-internal-projects"></a><span data-ttu-id="15a16-103">קביעת התצורה של חשבונאות לפרוייקטים פנימיים</span><span class="sxs-lookup"><span data-stu-id="15a16-103">Configure accounting for internal projects</span></span>

<span data-ttu-id="15a16-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="15a16-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="15a16-105">פרויקטים פנימיים מאפשרים לחברות לעקוב אחר עלויות הקשורות לפעילויות שלא מחייבים עבורן את הלקוח.</span><span class="sxs-lookup"><span data-stu-id="15a16-105">Internal projects allow companies track cost related to activities that aren't being billed to a customer.</span></span> <span data-ttu-id="15a16-106">דוגמאות לפרויקטים פנימיים כוללים:</span><span class="sxs-lookup"><span data-stu-id="15a16-106">Examples of internal projects include:</span></span>

- <span data-ttu-id="15a16-107">פיתוח מוצר, כמו אפליקציה למכשירים ניידים, ומעקב אחר העלויות הכרוכות בפיתוח.</span><span class="sxs-lookup"><span data-stu-id="15a16-107">Developing a product, such as a mobile app, and tracking the cost associated with the development.</span></span>
- <span data-ttu-id="15a16-108">ניהול זמן והוצאות טרום-מכירה.</span><span class="sxs-lookup"><span data-stu-id="15a16-108">Managing pre-sale time and expense.</span></span> <span data-ttu-id="15a16-109">ניתן להמיר פרויקט טרום-מכירה פנימי זה מאוחר יותר לפרויקט לחיוב אם הצעת המחיר זוכה.</span><span class="sxs-lookup"><span data-stu-id="15a16-109">This pre-sale internal project can be converted later to a billable project if quote is won.</span></span>

<span data-ttu-id="15a16-110">כל פרויקט שאינו משויך לחוזה ב-Dynamics 365 Project Operations מטופל כפרויקט פנימי.</span><span class="sxs-lookup"><span data-stu-id="15a16-110">Any project not associated with a contract in Dynamics 365 Project Operations is treated as internal.</span></span> <span data-ttu-id="15a16-111">פרופילי העלות וההכנסות של פרויקט אינם משמשים לקביעת עקרונות החשבונאות עבור הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="15a16-111">Project cost and revenue profiles aren't used to determine accounting rules for the project.</span></span> <span data-ttu-id="15a16-112">עלות פרויקט פנימית נרשמת תמיד על פי עקרונות רווח והפסד.</span><span class="sxs-lookup"><span data-stu-id="15a16-112">Internal project cost is always posted using profit and loss principles.</span></span> <span data-ttu-id="15a16-113">חשבונות ספר ראשי עבור רישומים מוגדרים בדף **הגדרת רישום בספר ראשי**.</span><span class="sxs-lookup"><span data-stu-id="15a16-113">Ledger accounts for postings are defined on the **Ledger posting setup** page.</span></span>

- <span data-ttu-id="15a16-114">עסקאות זמן מתבצעות באמצעות חיוב חשבון **עלות** וזיכוי חשבון **הקצאת שכר**.</span><span class="sxs-lookup"><span data-stu-id="15a16-114">Time transactions are posted by debiting the **Cost** account and crediting the **Payroll allocation** account.</span></span>
- <span data-ttu-id="15a16-115">עסקאות של הוצאה נרשמות באמצעות חיוב חשבון **עלות** וזיכוי **חשבון קיזוז להוצאות**.</span><span class="sxs-lookup"><span data-stu-id="15a16-115">Expense transactions are posted by debiting the **Cost** account and crediting the **Offset account for expense**.</span></span>

<span data-ttu-id="15a16-116">לאחר רישום עסקאות בפרויקט, אם הפרויקט משויך לחוזה פרוייקט, המערכת מבטלת את כל העסקאות שנצברו ויוצרת עסקאות חדשות לחיוב.</span><span class="sxs-lookup"><span data-stu-id="15a16-116">After transactions are posted to the project, if the project is associated with a project contract, the system reverses all accumulated transactions and creates new billable transactions.</span></span> <span data-ttu-id="15a16-117">העסקאות לחיוב מתבצעות לפי כללי החשבונאות המוגדרים בפרופיל העלות וההכנסות של הפרויקט, בהתאמה.</span><span class="sxs-lookup"><span data-stu-id="15a16-117">The billable transactions follow the accounting rules defined in respective Project cost and revenue profile.</span></span>


