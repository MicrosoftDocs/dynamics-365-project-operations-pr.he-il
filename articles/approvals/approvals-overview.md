---
title: מבט כולל על אישורים
description: נושא זה מספק מידע על עבודה עם אישורים ב-Project Operations.
author: stsporen
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 37994422e9146765076fdbb77f5c763b4f1d0802
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077168"
---
# <a name="approvals-overview"></a><span data-ttu-id="77ada-103">מבט כולל על אישורים</span><span class="sxs-lookup"><span data-stu-id="77ada-103">Approvals overview</span></span>

<span data-ttu-id="77ada-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="77ada-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="77ada-105">שליחות של זמן והוצאות עוברות דרך זרימת עבודה לאישור.</span><span class="sxs-lookup"><span data-stu-id="77ada-105">Time and Expense submissions move through an approval workflow.</span></span> <span data-ttu-id="77ada-106">לאחר אישור הערכים, העסקאות נרשמות בנתונים בפועל או שזמן מוזמן בלוח הזמנים.</span><span class="sxs-lookup"><span data-stu-id="77ada-106">After the entries are approved, transactions are recorded in actuals or time is booked in the schedule.</span></span>

## <a name="approvals-workflow"></a><span data-ttu-id="77ada-107">זרימת עבודה של אישורים</span><span class="sxs-lookup"><span data-stu-id="77ada-107">Approvals workflow</span></span>
<span data-ttu-id="77ada-108">כשאתה יוצר ושולח ערך זמן או הוצאה, נוצר ערך לאישור.</span><span class="sxs-lookup"><span data-stu-id="77ada-108">When you create and submit a time or expense entry, an approval entry is created.</span></span> <span data-ttu-id="77ada-109">מאשר הפרויקט או המנהל שלך בודק ומאשרים את הערך.</span><span class="sxs-lookup"><span data-stu-id="77ada-109">The Project approver or your manager reviews and approves your entry.</span></span> <span data-ttu-id="77ada-110">אם הערך קשור לפרויקט, הנתונים בפועל יווצרו לאחר אישורו.</span><span class="sxs-lookup"><span data-stu-id="77ada-110">If the entry is related to a project, when it's approved, the actuals will be created.</span></span> <span data-ttu-id="77ada-111">דבר זה מאפשר מעקב אחר העלות והחיוב.</span><span class="sxs-lookup"><span data-stu-id="77ada-111">This allows the cost and billing to be tracked.</span></span> 

## <a name="approve-an-entry"></a><span data-ttu-id="77ada-112">אישר ערך</span><span class="sxs-lookup"><span data-stu-id="77ada-112">Approve an entry</span></span>
<span data-ttu-id="77ada-113">הטופס **אישורים** מאפשר לך לעבור בין תצוגות שונות כדי שתוכל לרואת את סוגי האישורים השונים.</span><span class="sxs-lookup"><span data-stu-id="77ada-113">The **Approvals** form allows you to switch between different views so that you can view the different types of approvals.</span></span>
  
1. <span data-ttu-id="77ada-114">עבור אל הטופס **אישורים** ובחר **הוצאות** , **זמן** , או **אחזורים**.</span><span class="sxs-lookup"><span data-stu-id="77ada-114">Go to the **Approvals** form and select **Expenses** , **Time** , or **Recalls**.</span></span>
2. <span data-ttu-id="77ada-115">סקור כל אישור ובחר את האישורים שברצונך לאשר.</span><span class="sxs-lookup"><span data-stu-id="77ada-115">Review each approval, and select the ones you want to approve.</span></span>
3. <span data-ttu-id="77ada-116">בחר **אשר** כדי לאשר את הערכים שנבחרו.</span><span class="sxs-lookup"><span data-stu-id="77ada-116">Select **Approve** to approve the selected entries.</span></span>
<span data-ttu-id="77ada-117">המערכת תעבד ערכים אלה ותיצור נתונים בפועל או הזמנה.</span><span class="sxs-lookup"><span data-stu-id="77ada-117">The system will process these entries and create actuals or a booking.</span></span>

## <a name="reject-an-entry"></a><span data-ttu-id="77ada-118">דחיית ערך</span><span class="sxs-lookup"><span data-stu-id="77ada-118">Reject an entry</span></span>
<span data-ttu-id="77ada-119">כמאשר הפרויקט, ייתכן שיהיה עליך לשלוח ערך בחזרה למשתמש לצורך תיקון.</span><span class="sxs-lookup"><span data-stu-id="77ada-119">As the Project approver, you may have to send an entry back to a user for correction.</span></span>
  
1. <span data-ttu-id="77ada-120">עבור אל הטופס **אישורים** ובחר את הערך לדחייה.</span><span class="sxs-lookup"><span data-stu-id="77ada-120">Go to the **Approvals** form and select the entry to reject.</span></span> 
2. <span data-ttu-id="77ada-121">בחר **דחה**.</span><span class="sxs-lookup"><span data-stu-id="77ada-121">Select **Reject**.</span></span>
3. <span data-ttu-id="77ada-122">אופציונלי - הוסף תגובה בשיח **הערות דחייה** כדי ליידע את המשתמש בסיבה לדחיית הערך.</span><span class="sxs-lookup"><span data-stu-id="77ada-122">Optional - Add a comment in the **Rejection Comments** dialog to inform the user why the entry is being rejected.</span></span>
4. <span data-ttu-id="77ada-123">בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="77ada-123">Select **OK**.</span></span> <span data-ttu-id="77ada-124">הערך יוחזר למשתמש.</span><span class="sxs-lookup"><span data-stu-id="77ada-124">The entry will be returned to the user.</span></span>
  
## <a name="recall-entries"></a><span data-ttu-id="77ada-125">אחזור ערכים</span><span class="sxs-lookup"><span data-stu-id="77ada-125">Recall entries</span></span>
<span data-ttu-id="77ada-126">בשלב מסוים, ייתכן שתצטרך לאחזר ערך שנשלח.</span><span class="sxs-lookup"><span data-stu-id="77ada-126">At some point, you might need to recall a submitted entry.</span></span> <span data-ttu-id="77ada-127">אם ערך לא אושר, הוא יוחזר מיד.</span><span class="sxs-lookup"><span data-stu-id="77ada-127">If the entry has not been approved, it will be returned immediately.</span></span> <span data-ttu-id="77ada-128">יחד עם זאת, לערך שאושר עשוי להיות השפעה מהותית.</span><span class="sxs-lookup"><span data-stu-id="77ada-128">An approved entry however, may have a material impact.</span></span> <span data-ttu-id="77ada-129">מאשר הפרויקט נדרש לאשר את האחזור על מנת להמיר את העסקה ב'נתונים בפועל'.</span><span class="sxs-lookup"><span data-stu-id="77ada-129">The Project approver is required to approve the recall in order to reverse the transaction in Actuals.</span></span>

## <a name="specify-project-approvers"></a><span data-ttu-id="77ada-130">קביעת מאשרי פרוייקט</span><span class="sxs-lookup"><span data-stu-id="77ada-130">Specify Project approvers</span></span>
<span data-ttu-id="77ada-131">בכל פרויקט יש מספר חברי צוות של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="77ada-131">Each project has a number of project team members.</span></span> <span data-ttu-id="77ada-132">ניתן לקבוע אילו חברי צוות הם גם המאשרים של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="77ada-132">You can specify which team members are also Project approvers.</span></span>

1. <span data-ttu-id="77ada-133">עבור אל הטופס **פרויקטים** ופתח את הפרויקט מתוך הרשימה.</span><span class="sxs-lookup"><span data-stu-id="77ada-133">Go to the **Projects** form and open the project from the list.</span></span>
2. <span data-ttu-id="77ada-134">בכרטיסיה **צוות** בחר את חבר הצוות שיהיה מאשר הפרויקט ואז בחר **עריכה**.</span><span class="sxs-lookup"><span data-stu-id="77ada-134">On the **Team** tab, select the team member who will be a Project approver and then select **Edit**.</span></span>
3. <span data-ttu-id="77ada-135">הגדר את שדה **מאשר הפרויקט** ל **כן**.</span><span class="sxs-lookup"><span data-stu-id="77ada-135">Set the **Project Approver** field to **Yes**.</span></span>
4. <span data-ttu-id="77ada-136">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="77ada-136">Select **Save**.</span></span>
5. <span data-ttu-id="77ada-137">חזור על שלבים 2-4‏ כדי להוסיף מאשרי פרויקט נוספים.</span><span class="sxs-lookup"><span data-stu-id="77ada-137">Repeat steps 2-4 to add additional Project approvers.</span></span>

## <a name="configure-the-users-manager"></a><span data-ttu-id="77ada-138">קבע את התצורה של מנהל המשתמש</span><span class="sxs-lookup"><span data-stu-id="77ada-138">Configure the user's manager</span></span>

1. <span data-ttu-id="77ada-139">עבור אל **הגדרות** > **אבטחה** > **משתמשים**.</span><span class="sxs-lookup"><span data-stu-id="77ada-139">Go to **Settings** > **Security** > **Users**.</span></span>
2. <span data-ttu-id="77ada-140">בחר את המשתמש אליו אתה מקצה מנהל ובתוך האזור **מידע על הארגון** , בחר את המנהל מתוך הרשימה.</span><span class="sxs-lookup"><span data-stu-id="77ada-140">Select the user to whom you are assigning a manager and in the **Organization Information** area, select the manager from the list.</span></span> 
3. <span data-ttu-id="77ada-141">בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="77ada-141">Select **Save**.</span></span>


