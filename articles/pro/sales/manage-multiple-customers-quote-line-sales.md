---
title: ניהול מספר רב של לקוחות בשורות הצעות מחיר מבוססות פרויקט
description: נושא זה מתאר כיצד לנהל לקוחות מרובים בשורות הצעת מחיר מבוססות פרויקט.
author: rumant
manager: Annbe
ms.date: 10/06/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 6a509fcf8d1fa11b4ce1ba1493d9c3cc64b4f22f
ms.sourcegitcommit: fd8ea1779db2bb39a428f459ae3293c4fd785572
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/06/2020
ms.locfileid: "3965799"
---
# <a name="managing-multiple-customers-on-project-based-quote-lines"></a><span data-ttu-id="f13f8-103">ניהול מספר רב של לקוחות בשורות הצעות מחיר מבוססות פרויקט</span><span class="sxs-lookup"><span data-stu-id="f13f8-103">Managing multiple customers on project-based quote lines</span></span>

<span data-ttu-id="f13f8-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="f13f8-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f13f8-105">שורות הצעות מחיר מבוססות פרויקט תומכות בתרחישים שבהם לכל שורת הצעת מחיר יש רשימה של לקוחות שמשלמים עבורה.</span><span class="sxs-lookup"><span data-stu-id="f13f8-105">Project-based quote lines support scenarios where each quote line has a list of customers that are paying for it.</span></span> <span data-ttu-id="f13f8-106">רשימת לקוחות זו בשורת הצעת מחיר מבוססת הפרויקט יכולה להיות זהה לרשימת הלקוחות בהצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="f13f8-106">This list of customers on the project-based quote line can be the same as the list of customers on the quote.</span></span> <span data-ttu-id="f13f8-107">ניתן גם לשנות את רשימת הלקוחות כך שהיא תהיה שונה.</span><span class="sxs-lookup"><span data-stu-id="f13f8-107">You can also change the list of customers to be different.</span></span> <span data-ttu-id="f13f8-108">כשזוכים בהצעת מחיר לפרויקט, רשימת הלקוחות בשורת הצעת המחיר מבוססת הפרויקט מועתקת לסעיף החוזה מבוסס הפרויקט המתאים, כדי ליצור את חוזה הפרויקט הסופי.</span><span class="sxs-lookup"><span data-stu-id="f13f8-108">When a project quote is won, the customer list on the project-based quote line is copied to the corresponding project–based contract line to create the eventual project contract.</span></span> <span data-ttu-id="f13f8-109">לקוחות בהצעת המחיר מבוססת הפרויקט מועתקים לחוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="f13f8-109">Customers on the project-based quote are copied to the project contract.</span></span>

<span data-ttu-id="f13f8-110">כאשר אתה מגיש חשבונית עבור חוזה הפרויקט הסופי, רשימת הלקוחות סעיף החוזה מבוסס הפרויקט מקבלת עדיפות על הרשימה בחוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="f13f8-110">When you invoice the eventual project contract, the customer list on the project-based contract line takes priority over the list on the project contract.</span></span> <span data-ttu-id="f13f8-111">רשימת הלקוחות בחוזה הפרויקט משמשת רק לברירות מחדל בסעיפי חוזה חדשים של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="f13f8-111">The customer list on the project contract is only used for defaults on new project contract lines.</span></span>

<span data-ttu-id="f13f8-112">כל הלקוחות של הצעת מחיר בכרטיסיה **לקוחות** של הצעת המחיר של הפרויקט, מופיעים, כבררת מחדל, כלקוחות של שורת הצעת מחיר בכל שורות הצעות המחיר מבוססת פרויקט חדשה שנוצרת עבור הצעת המחיר של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="f13f8-112">All quote customers on the **Customers** tab of the project quote default as quote line customers on any new project-based quote lines created for the project quote.</span></span> <span data-ttu-id="f13f8-113">שורות הצעת מחיר מבוססות פרויקט קיימות אינן יורשות רשומות חדשות של לקוחות הצעות מחיר שנוצרו אחריהן.</span><span class="sxs-lookup"><span data-stu-id="f13f8-113">Any existing project-based quote lines don't inherit new quote customer records created after them.</span></span>

## <a name="create-update-or-delete-a-quote-line-customer-record"></a><span data-ttu-id="f13f8-114">יצירה, עדכון או מחיקה של רשומת לקוח של שורת הצעת מחיר</span><span class="sxs-lookup"><span data-stu-id="f13f8-114">Create, update, or delete a quote line customer record</span></span>

<span data-ttu-id="f13f8-115">ניתן ליצור, לעדכן או למחוק לקוח של שורת הצעות מחיר בכרטיסיה **לקוחות של שורת הצעת מחיר** בדף **שורת הצעת מחיר מבוססת פרויקט**.</span><span class="sxs-lookup"><span data-stu-id="f13f8-115">You can create, update, or delete a quote line customer on the **Quote line customers** tab on the **Project-based quote line** page.</span></span> <span data-ttu-id="f13f8-116">כאשר אתה מוסיף לקוח חדש בשורת הצעת מחיר מבוססת הפרויקט, הלקוח מתווסף גם להצעת המחיר הכוללת כלקוח הצעת מחיר, כאשר ברירת המחדל היא אחוז פיצול חיוב בהצעת המחיר הכוללת של 0%.</span><span class="sxs-lookup"><span data-stu-id="f13f8-116">When you add a new customer on the project-based quote line, the customer is also added to the overall quote as a quote customer, with a default billing split percentage on the overall quote of 0%.</span></span> <span data-ttu-id="f13f8-117">אחוז פיצול החיוב בהצעת המחיר הכוללת מועתק לשורות הצעת מחיר חדשות ולחוזה הפרויקט הסופי.</span><span class="sxs-lookup"><span data-stu-id="f13f8-117">The billing split percentage on the overall quote is copied to new quote lines and to the eventual project contract.</span></span> <span data-ttu-id="f13f8-118">עם זאת, בעת הגשת חשבונית מהחוזה, משתמשים באחוזי פיצול החיוב ברמת שורת הצעת המחיר, ולא באחוזי פיצול החיוב ברמת החוזה הכוללת.</span><span class="sxs-lookup"><span data-stu-id="f13f8-118">However, when invoicing from the contract, the billing split percentage at the quote line level is used, not the billing split percentage at the overall contract level.</span></span> 

<span data-ttu-id="f13f8-119">הטבלה הבאה מציגה את השדות ברשומת הלקוח של שורת הצעת המחיר בשורת הצעת מחיר מבוססת פרויקט.</span><span class="sxs-lookup"><span data-stu-id="f13f8-119">The following table shows the fields on the quote line customer record of a project-based quote line.</span></span>

| <span data-ttu-id="f13f8-120">שדה</span><span class="sxs-lookup"><span data-stu-id="f13f8-120">Field</span></span> | <span data-ttu-id="f13f8-121">מיקום</span><span class="sxs-lookup"><span data-stu-id="f13f8-121">Location</span></span> | <span data-ttu-id="f13f8-122">תיאור והדרכה</span><span class="sxs-lookup"><span data-stu-id="f13f8-122">Description and guidance</span></span> | <span data-ttu-id="f13f8-123">השפעה במורד הזרם</span><span class="sxs-lookup"><span data-stu-id="f13f8-123">Downstream impact</span></span> |
| --- | --- | --- | --- |
| <span data-ttu-id="f13f8-124">**תיק לקוח**</span><span class="sxs-lookup"><span data-stu-id="f13f8-124">**Account**</span></span> | <span data-ttu-id="f13f8-125">רשת הניתנת לעריכה בכרטיסיה **לקוחות של שורת הצעת מחיר**, הטופס הראשי והטפסים ליצירה מהירה עבור לקוח של שורת הצעות מחיר.</span><span class="sxs-lookup"><span data-stu-id="f13f8-125">An editable grid on the **Quote line customers** tab, the main form, and the quick create forms for a quote line customer.</span></span> | <span data-ttu-id="f13f8-126">מכיל את כל תיקי הלקוח הפעילים.</span><span class="sxs-lookup"><span data-stu-id="f13f8-126">Lists all active accounts.</span></span> <span data-ttu-id="f13f8-127">שדה זה ננעל לאחר יצירת הרשומה.</span><span class="sxs-lookup"><span data-stu-id="f13f8-127">This field is locked after the record is created.</span></span> <span data-ttu-id="f13f8-128">אם צריך לעדכן את השדה, מחק את הרשומה וצור אותה מחדש.</span><span class="sxs-lookup"><span data-stu-id="f13f8-128">If you need to update the field, delete and recreate the record.</span></span> <span data-ttu-id="f13f8-129">אם רשמת נתונים בפועל, אינך יכול למחוק את הרשומה.</span><span class="sxs-lookup"><span data-stu-id="f13f8-129">If you recorded any actuals, you can't delete the record.</span></span> | <span data-ttu-id="f13f8-130">כשבוחרים תיק לקוח מהרשימה הראשית של תיקי לקוח להוספה, לקוח שורת הצעת המחיר נוסף גם כלקוח הצעת מחיר כששומרים אותו.</span><span class="sxs-lookup"><span data-stu-id="f13f8-130">When you pick an account from the master list of accounts to add, the quote line customer is also added as a quote customer when you save it.</span></span> <span data-ttu-id="f13f8-131">כשזוכים בהצעת מחיר, לקוחות של שורת הצעת מחיר מועתקים ללקוחות סעיף חוזה של הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="f13f8-131">When a quote is won, quote line customers are copied to the project contract line customers.</span></span> |
| <span data-ttu-id="f13f8-132">**אחוז פיצול חיוב**</span><span class="sxs-lookup"><span data-stu-id="f13f8-132">**Billing split percent**</span></span> | <span data-ttu-id="f13f8-133">רשת הניתנת לעריכה בכרטיסיה **לקוחות של שורת הצעת מחיר**, הטופס הראשי והטפסים ליצירה מהירה עבור לקוח של שורת הצעות מחיר.</span><span class="sxs-lookup"><span data-stu-id="f13f8-133">An editable grid on the **Quote line customers** tab, the main form, and the quick create forms for a quote line customer.</span></span> | <span data-ttu-id="f13f8-134">מייצג את האחוז של כל עסקת מכירה שלא חויבה, אשר יזוקף ללקוח שורת הצעת מחיר זה.</span><span class="sxs-lookup"><span data-stu-id="f13f8-134">Represents the percentage of each unbilled sales transaction that will be attributed to this quote line customer.</span></span> | <span data-ttu-id="f13f8-135">מועתקים אל לקוחות של סעיף חוזה של פרויקט.</span><span class="sxs-lookup"><span data-stu-id="f13f8-135">Copied over to project contract line customers.</span></span> |
| <span data-ttu-id="f13f8-136">**מגבלת 'אין לחרוג'**</span><span class="sxs-lookup"><span data-stu-id="f13f8-136">**Not-to-exceed limit**</span></span> | <span data-ttu-id="f13f8-137">רשת הניתנת לעריכה בכרטיסיה **לקוחות של שורת הצעת מחיר**, הטופס הראשי והטפסים ליצירה מהירה עבור לקוח של שורת הצעות מחיר.</span><span class="sxs-lookup"><span data-stu-id="f13f8-137">An editable grid on the **Quote line customers** tab, the main form, and the quick create forms for a quote line customer.</span></span> | <span data-ttu-id="f13f8-138">מציין אם קיימת מגבלה או תקרה שסוכמה במשא ומתן עבור הסכום הכולל שבו יחויב לקוח זה עבור השורת הצעת מחיר זו.</span><span class="sxs-lookup"><span data-stu-id="f13f8-138">Indicates whether there is a negotiated limit or cap to the overall amount that will be invoiced to this customer for this quoted line.</span></span> | <span data-ttu-id="f13f8-139">מועתק ללקוחות סעיף חוזה של פרויקט כאשר זוכים בהצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="f13f8-139">Copied over to project contract line customers when a quote is won.</span></span> |
| <span data-ttu-id="f13f8-140">**מעגל**</span><span class="sxs-lookup"><span data-stu-id="f13f8-140">**Is rounding**</span></span> | <span data-ttu-id="f13f8-141">רשת הניתנת לעריכה בכרטיסיה **לקוחות של שורת הצעת מחיר**, הטופס הראשי והטפסים ליצירה מהירה עבור לקוח של שורת הצעות מחיר.</span><span class="sxs-lookup"><span data-stu-id="f13f8-141">An editable grid on the **Quote line customers** tab, the main form, and the quick create forms for a quote line customer.</span></span> | <span data-ttu-id="f13f8-142">מציין אם מתבצע עיגול עבור לקוח זה כברירת מחדל עבור שורת הצעת מחיר מבוססת פרויקט זו.</span><span class="sxs-lookup"><span data-stu-id="f13f8-142">Indicates whether this customer is a default rounding customer for this project-based quote line.</span></span> | <span data-ttu-id="f13f8-143">מועתק ללקוחות סעיף חוזה של פרויקט כאשר זוכים בהצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="f13f8-143">Copied over to project contract customers when a quote is won.</span></span> |

## <a name="edit-billing-split-percentages"></a><span data-ttu-id="f13f8-144">עריכת אחוזי פיצול חיוב</span><span class="sxs-lookup"><span data-stu-id="f13f8-144">Edit billing split percentages</span></span>

<span data-ttu-id="f13f8-145">ניתן לערוך את אחוזי פיצול החיוב בשורה.</span><span class="sxs-lookup"><span data-stu-id="f13f8-145">You can edit billing split percentages in-line.</span></span> <span data-ttu-id="f13f8-146">כאשר אחוזי פיצול החיוב אינם מסתכמים ב-100%, מתרחשת שגיאה.</span><span class="sxs-lookup"><span data-stu-id="f13f8-146">When the billing split percentages don't total 100%, an error occurs.</span></span> <span data-ttu-id="f13f8-147">לאחר עריכת אחוזי הפיצול לחיוב, רענן את דף שורת הצעת המחיר כדי להסיר את השגיאה.</span><span class="sxs-lookup"><span data-stu-id="f13f8-147">After you edit the billing split percentages, refresh the quote line page to remove the error.</span></span>

<span data-ttu-id="f13f8-148">השתמש בפעולת ההפצה השווה ברשת המשנה של לקוחות שורת הצעת מחיר כדי להקצות פיצולי חיוב לכל לקוחות שורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="f13f8-148">Use the evenly distribute action on the quote line customers subgrid to allocate billing splits to all quote line customers.</span></span> <span data-ttu-id="f13f8-149">אם קיים גורם עיגול, הוא יתווסף ללקוחות שעבורם מתבצע עיגול.</span><span class="sxs-lookup"><span data-stu-id="f13f8-149">If there's a rounding factor, that will be added to the rounding customer.</span></span> <span data-ttu-id="f13f8-150">אחד מלקוחות שורת הצעת המחיר מתויג תמיד כלקוח שעבורו מתבצע עיגול, ומשמעות הדבר היא שברשומת הלקוח של שורת הצעת המחיר,  דגל העיגול מוגדר ל**כן**.</span><span class="sxs-lookup"><span data-stu-id="f13f8-150">One of the quote line customers is always tagged as the rounding customer, which means that quote line customer record has the rounding flag set to **Yes**.</span></span> 