---
title: הגדרת תעריפי עלות ומכירה עבור קטלוג מוצרים - לייט
description: נושא זה מספק מידע על הדרך להגדרת תעריפי עלות ומכירות עבור פריטים בקטלוג המוצרים.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5e851193df8151821e112e01a9f33df5afee7df7
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764552"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products---lite"></a><span data-ttu-id="10316-103">הגדרת תעריפי עלות ומכירה עבור קטלוג מוצרים - לייט</span><span class="sxs-lookup"><span data-stu-id="10316-103">Set up cost and sales rates for catalog products - lite</span></span>

<span data-ttu-id="10316-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="10316-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="10316-105">הגדרת תמחור עבור פריטי קטלוג מוצרים ב- Dynamics 365 Project Operations זהה לזה של Dynamics 365 Sales.</span><span class="sxs-lookup"><span data-stu-id="10316-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="10316-106">ב- Project Operations, לא ניתן לאמוד מוצרים או להשתמש בהם בפרוייקטים, ולכן אין צורך לקבוע את מחירי קטלוג המוצרים במחירונים של פרוייקטים לקבלת הצעות מחיר וחוזים.</span><span class="sxs-lookup"><span data-stu-id="10316-106">In Project Operations, products can't be estimated or used on projects, so product catalog prices don't need to be set on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="10316-107">השתמש בשדה **מחיר מוצר** של הצעת מחיר, חוזה או תיק לקוח להגדרת מחירים של קטלוג מוצרים.</span><span class="sxs-lookup"><span data-stu-id="10316-107">Use the **Product Price** field of a quote, contract, or account to set up product catalog prices.</span></span> <span data-ttu-id="10316-108">אל תגדיר מחירים של קטלוג מוצרים במחירונים של הפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="10316-108">Don't set up product catalog prices in the project price lists.</span></span> <span data-ttu-id="10316-109">מחירוני הפרויקט בלעדיים ל- Project Operations.</span><span class="sxs-lookup"><span data-stu-id="10316-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="10316-110">לוגיקה עסקית ספציפית ליישום מעתיקה את המחירונים מהצעת מחיר לחוזה.</span><span class="sxs-lookup"><span data-stu-id="10316-110">Application-specific business logic copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="10316-111">התוצאה היא מחירון לפרויקט שספציפי לחוזה.</span><span class="sxs-lookup"><span data-stu-id="10316-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="10316-112">פעולת ההעתקה עשויה לעכב את תהליך הזכייה בהצעת המחיר אם מחירון הפרויקט בהצעת המחיר נהיה גדול מדי.</span><span class="sxs-lookup"><span data-stu-id="10316-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="10316-113">מחירוני מוצרים אינם מועתקים כדי ליצור מחירונים מותאמים אישית בחוזים.</span><span class="sxs-lookup"><span data-stu-id="10316-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="10316-114">מכיוון שלא מדובר בהעתקה, הביצועים של תהליך הצעת המחיר אינם מושפעים.</span><span class="sxs-lookup"><span data-stu-id="10316-114">Because there's no copying involved, the performance of the quote process isn't affected.</span></span>
