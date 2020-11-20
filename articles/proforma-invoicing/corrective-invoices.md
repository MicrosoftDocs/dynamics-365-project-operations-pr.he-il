---
title: חשבוניות שתוקנו
description: נושא זה מספק מידע על הפקת חשבוניות שתוקנו.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 1ebfec053a59bbadd261d4333f6737cf16292e81
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122389"
---
# <a name="corrected-invoices"></a><span data-ttu-id="ea07a-103">חשבוניות שתוקנו</span><span class="sxs-lookup"><span data-stu-id="ea07a-103">Corrected invoices</span></span>

<span data-ttu-id="ea07a-104">_**חל על:** ‏Project Operations לתרחישים מבוססי משאבים/ללא מלאי_</span><span class="sxs-lookup"><span data-stu-id="ea07a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="ea07a-105">ניתן לערוך חשבוניות שתוקנו.</span><span class="sxs-lookup"><span data-stu-id="ea07a-105">Confirmed invoices can be edited.</span></span> <span data-ttu-id="ea07a-106">בעת עריכה של חשבונית מאושרת, נוצרת טיוטה חדשה לחשבונית תיקון.</span><span class="sxs-lookup"><span data-stu-id="ea07a-106">When you edit a confirmed invoice, a draft of the corrected invoice is created.</span></span> <span data-ttu-id="ea07a-107">מכיוון שההנחה היא שברצונך לבטל את כל העסקאות והכמויות מהחשבונית המקורית, חשבונית תיקון זו כוללת את כל העסקאות מהחשבונית המקורית וכל הכמויות שבה הן אפס (0).</span><span class="sxs-lookup"><span data-stu-id="ea07a-107">Because the assumption is that you want to reverse all the transactions and quantities from the original invoice, the corrected invoice includes all the transactions from the original invoice, and all the quantities on it are zero (0).</span></span>

<span data-ttu-id="ea07a-108">כאשר עסקאות לא דורשות תיקון, תוכל להסיר אותן מהטיוטה של חשבונית התיקון.</span><span class="sxs-lookup"><span data-stu-id="ea07a-108">When transactions don't require correction, you can remove them from the draft corrective invoice.</span></span> <span data-ttu-id="ea07a-109">כדי לבטל או להחזיר כמות חלקית בלבד, תוכל לערוך את השדה כמות בפירוט השורה.</span><span class="sxs-lookup"><span data-stu-id="ea07a-109">To reverse or return only a partial quantity, you can edit the Quantity field on the line detail.</span></span> <span data-ttu-id="ea07a-110">אם תפתח את הפירוט בשורת החשבונית, תוכל לראות את הכמות בחשבונית המקורית.</span><span class="sxs-lookup"><span data-stu-id="ea07a-110">If you open the invoice line detail, you can see the original invoice quantity.</span></span> <span data-ttu-id="ea07a-111">לאחר מכן תוכל לערוך את הכמות בחשבונית הנוכחית כך שתהיה קטנה או גדולה מהכמות בחשבונית המקורית.</span><span class="sxs-lookup"><span data-stu-id="ea07a-111">You can then edit the current invoice quantity so that it's less than or more than the original invoice quantity.</span></span>

<span data-ttu-id="ea07a-112">בעת אישור חשבונית תיקון, הנתונים בפועל המקוריים של המכירות שחויבו מבוטלים, ונוצרים נתונים בפועל חדשים למכירות שחויבו.</span><span class="sxs-lookup"><span data-stu-id="ea07a-112">When you confirm a corrective invoice, the original billed sales actual is reversed, and a new billed sales actual is created.</span></span> <span data-ttu-id="ea07a-113">אם הכמות הופחתה, ההפרש יגרום גם ליצירה של נתונים בפועל חדשים של מכירות שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="ea07a-113">If the quantity was reduced, the difference will cause a new unbilled sales actual to be created too.</span></span> <span data-ttu-id="ea07a-114">לדוגמה, אם המכירה המקורית שחויבה היתה עבור שמונה שעות, ובפרטי שורת חשבונית התיקון יש כמות מופחתת של שש שעות, השורה המקורית של המכירות תבוטל וייווצרו שני נתונים בפועל חדשים:</span><span class="sxs-lookup"><span data-stu-id="ea07a-114">For example, if the original billed sale was for eight hours, and the corrected invoice line detail has a reduced quantity of six hours, the original billed sales line is revered and two new actuals are created:</span></span>

- <span data-ttu-id="ea07a-115">נתונים בפועל למכירות שחויבו עבור שש שעות.</span><span class="sxs-lookup"><span data-stu-id="ea07a-115">A billed sales actual for six hours.</span></span>
- <span data-ttu-id="ea07a-116">נתונים בפועל למכירות שלא חויבו עבור השעתיים שנותרו.</span><span class="sxs-lookup"><span data-stu-id="ea07a-116">An unbilled sales actual for the remaining two hours.</span></span> <span data-ttu-id="ea07a-117">ניתן לחייב עסקה זו במועד מאוחר יותר או לסמנה כלא ניתנת לחיוב, בהתאם למשא ומתן עם הלקוח.</span><span class="sxs-lookup"><span data-stu-id="ea07a-117">This transaction can either be billed later or marked as non-chargeable, depending on the negotiations with the customer.</span></span>
