---
title: הגדרת תעריפי עלות ומכירות עבור קטלוג מוצרים
description: נושא זה מספק מידע על הדרך להגדרת תעריפי עלות ומכירות עבור פריטים בקטלוג המוצרים.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d5178a9143536bf4b2573403125325017861cdd5
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077375"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products"></a><span data-ttu-id="85361-103">הגדרת תעריפי עלות ומכירות עבור קטלוג מוצרים</span><span class="sxs-lookup"><span data-stu-id="85361-103">Set up cost and sales rates for catalog products</span></span>

<span data-ttu-id="85361-104">_**חל על** : פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="85361-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="85361-105">הגדרת תמחור עבור פריטי קטלוג מוצרים ב- Dynamics 365 Project Operations זהה לתהליך ב- Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="85361-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="85361-106">מכיוון שלא ניתן לאמוד מוצרים או להשתמש בהם בפרויקטים במסגרת Project Operations, אין צורך לקבוע מחירים של קטלוג מוצרים במחירונים של פרויקטים לקבלת הצעות מחיר וחוזים.</span><span class="sxs-lookup"><span data-stu-id="85361-106">Because products can't be estimated or used on projects in Project Operations, there is no need to set product catalog prices on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="85361-107">יש לקבוע את מחירי קטלוג המוצרים בשדה **מחיר מוצר** של הצעת מחיר, חוזה או תיק לקוח.</span><span class="sxs-lookup"><span data-stu-id="85361-107">Product catalog prices should be set up in the **Product Price** field of a quote, contract, or account.</span></span> <span data-ttu-id="85361-108">אל תגדיר מחירים של קטלוג מוצרים במחירוני הפרויקט עבור ישויות אלה.</span><span class="sxs-lookup"><span data-stu-id="85361-108">Don't set up product catalog prices in the project price lists for these entities.</span></span> <span data-ttu-id="85361-109">מחירוני הפרויקט בלעדיים ל- Project Operations.</span><span class="sxs-lookup"><span data-stu-id="85361-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="85361-110">יש היגיון עסקי שספציפי ליישום שמעתיק את המחירונים מהצעת מחיר לחוזה.</span><span class="sxs-lookup"><span data-stu-id="85361-110">There is application-specific business logic that copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="85361-111">התוצאה היא מחירון לפרויקט שספציפי לחוזה.</span><span class="sxs-lookup"><span data-stu-id="85361-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="85361-112">פעולת ההעתקה עשויה לעכב את תהליך הזכייה בהצעת המחיר אם מחירון הפרויקט בהצעת המחיר נהיה גדול מדי.</span><span class="sxs-lookup"><span data-stu-id="85361-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="85361-113">מחירוני מוצרים אינם מועתקים כדי ליצור מחירונים מותאמים אישית בחוזים.</span><span class="sxs-lookup"><span data-stu-id="85361-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="85361-114">המשמעות היא שמחירוני מוצרים אינם משפיעים על ביצועי תהליך הזכייה בהצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="85361-114">This means that product price lists don't impact the performance of the quote win process.</span></span>
