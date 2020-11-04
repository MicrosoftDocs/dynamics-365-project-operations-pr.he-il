---
title: מושגים מרכזיים לניהול משאבים
description: נושא זה מספק מידע על יכולות ניהול משאבים ב- Microsoft Dynamics Project Operations.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 124d9bad5cc0c16955417a8213db047a2d8bae1d
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077155"
---
# <a name="resource-management-key-concepts"></a><span data-ttu-id="6ca19-103">מושגים מרכזיים לניהול משאבים</span><span class="sxs-lookup"><span data-stu-id="6ca19-103">Resource management key concepts</span></span>

<span data-ttu-id="6ca19-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="6ca19-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="6ca19-105">משאבים הם הנכס החשוב ביותר של ארגון מבוסס-שירות.</span><span class="sxs-lookup"><span data-stu-id="6ca19-105">Resources are the most important asset of a service-based organization.</span></span> <span data-ttu-id="6ca19-106">היכולת למצוא את המשאבים הנכונים בזמן הנכון, להזמין משאבים אלה בפרויקטים ולהקפיד לנצל אותם, עוזרת לארגון לעמוד ביעדי ההכנסות וביעדי שביעות הרצון של הלקוחות.</span><span class="sxs-lookup"><span data-stu-id="6ca19-106">The ability to find the right resources at the right time, book those resources on projects and keep them utilized, helps the organization meet revenue targets and customer satisfaction goals.</span></span> <span data-ttu-id="6ca19-107">ניתן להשתמש בפונקציונליות של הקצאת משאבים בפרויקט ב- Dynamics 365 Project Operations כדי לבצע את המשימות הבאות:</span><span class="sxs-lookup"><span data-stu-id="6ca19-107">You can use the project resourcing functionality in Dynamics 365 Project Operations to do the following tasks:</span></span>

- <span data-ttu-id="6ca19-108">צור צוותי פרויקטים על-ידי הזמנת משאבים זמינים העומדים בדרישות.</span><span class="sxs-lookup"><span data-stu-id="6ca19-108">Form project teams by booking available and qualified resources.</span></span>
- <span data-ttu-id="6ca19-109">צור רשומות של חברי צוות כלליים והגדר את התפקידים שלהם ואת היחידה הארגונית של המשאב שלהם.</span><span class="sxs-lookup"><span data-stu-id="6ca19-109">Create generic team member records and define their roles and resource organization unit.</span></span>
- <span data-ttu-id="6ca19-110">צור דרישות משאבים עבור חברי צוות כלליים מהקצאות המשימה שלהם.</span><span class="sxs-lookup"><span data-stu-id="6ca19-110">Generate resource requirements for generic team members from their task assignments.</span></span>
- <span data-ttu-id="6ca19-111">התאם כישורים על-ידי זיהוי הכישורים שהוגדרו בביקוש למשאב מול הכישורים של משאבים זמינים.</span><span class="sxs-lookup"><span data-stu-id="6ca19-111">Match skills by identifying the skills defined on the resource demand against available resource skills.</span></span>
- <span data-ttu-id="6ca19-112">החלף משאבים.</span><span class="sxs-lookup"><span data-stu-id="6ca19-112">Substitute resources.</span></span>
- <span data-ttu-id="6ca19-113">התאם הקצאות של לוח זמני פרויקט והזמנות של משאבים.</span><span class="sxs-lookup"><span data-stu-id="6ca19-113">Align project schedule assignments and resource bookings.</span></span>
- <span data-ttu-id="6ca19-114">התאם בין הפרשים בהזמנות ובהקצאות.</span><span class="sxs-lookup"><span data-stu-id="6ca19-114">Reconcile differences in bookings and assignments.</span></span>
- <span data-ttu-id="6ca19-115">שנה הזמנות של משאבים בתגובה למצב 'מחוץ למשרד'.</span><span class="sxs-lookup"><span data-stu-id="6ca19-115">Change resource bookings in response to out-of-office status.</span></span>
- <span data-ttu-id="6ca19-116">שתף פעולה בין מנהלי פרויקטים ומנהלי משאבים.</span><span class="sxs-lookup"><span data-stu-id="6ca19-116">Collaborate between project managers and resource managers.</span></span>
- <span data-ttu-id="6ca19-117">הצג את ההיסטוריה של ניצול המשאב מול היעד, כולל פירוט האופן שבו נוצל הזמן של המשאבים.</span><span class="sxs-lookup"><span data-stu-id="6ca19-117">View the history of resource utilization against a target, including a breakdown of how the resources' time was utilized.</span></span>
- <span data-ttu-id="6ca19-118">צור מאגר של כישורים ומומחיות ושמור אותו.</span><span class="sxs-lookup"><span data-stu-id="6ca19-118">Maintain a skills and proficiency repository.</span></span>


<span data-ttu-id="6ca19-119">ניתן לאייש את הפרויקט בצוות של משאבים כלליים או בעלי שם ב- Project Operations.</span><span class="sxs-lookup"><span data-stu-id="6ca19-119">You can staff your project with a team of generic or named resources in Project Operations.</span></span> <span data-ttu-id="6ca19-120">ניתן להשתמש בשיטות שונות כדי להוסיף ולהקצות חברי צוות ולנהל את ההזמנות וההקצאות שלהם.</span><span class="sxs-lookup"><span data-stu-id="6ca19-120">You can use various methods to add and assign team members and to manage their bookings and assignments.</span></span> 
