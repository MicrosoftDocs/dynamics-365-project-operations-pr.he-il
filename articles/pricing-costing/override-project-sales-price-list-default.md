---
title: עקיפת מחירוני מכירות של פרויקט
description: נושא זה מספק מידע על יצירת מחירוני מכירה מותאמים אישית.
author: rumant
ms.date: 10/22/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: db2ff6acaad6ab4cbcc98d3d5b06b36ed23b758f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995082"
---
# <a name="override-project-sales-price-lists"></a><span data-ttu-id="69500-103">עקיפת מחירוני מכירות של פרויקט</span><span class="sxs-lookup"><span data-stu-id="69500-103">Override project sales price lists</span></span>

<span data-ttu-id="69500-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="69500-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

## <a name="customer-specific-project-price-lists"></a><span data-ttu-id="69500-105">מחירוני פרוייקט ספציפיים ללקוח</span><span class="sxs-lookup"><span data-stu-id="69500-105">Customer-specific project price lists</span></span>

<span data-ttu-id="69500-106">ניתן להגדיר הסכמי מחירים ספציפיים ללקוח כמחירוני פרוייקט ברשומת תיק לקוח ב- Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="69500-106">Customer-specific price agreements can be set up as project price lists on an account record in Dynamics 365 Project Operations.</span></span>

<span data-ttu-id="69500-107">להגדרת מחירון פרויקט ספציפי ללקוח, באזור **מכירות**, נווט לרשומת תיק לקוח.</span><span class="sxs-lookup"><span data-stu-id="69500-107">To set up a customer-specific project price list, in the **Sales** area, navigate to the account record.</span></span>

1. <span data-ttu-id="69500-108">פתח את הדף הרשימה **תיקי לקוח**.</span><span class="sxs-lookup"><span data-stu-id="69500-108">Open the **Accounts** list page.</span></span>
2. <span data-ttu-id="69500-109">אתר ולחץ פעמיים על רשומת לקוח כדי לפתוח את דף הפרטים של **תיק לקוח**.</span><span class="sxs-lookup"><span data-stu-id="69500-109">Locate and double-click a customer record to open the **Account** details page.</span></span>
3. <span data-ttu-id="69500-110">בכרטיסיה **מחירוני הפרויקט** בחר **+מחירון פרויקט חדש**.</span><span class="sxs-lookup"><span data-stu-id="69500-110">On the **Project Price lists** tab, select **+ New Project Price List**.</span></span>
4. <span data-ttu-id="69500-111">בדף **מחירון פרוייקט חדש**, בחר מחירון מהתפריט הנפתח.</span><span class="sxs-lookup"><span data-stu-id="69500-111">On the **New Project Price List** page, select a price list from the drop-down.</span></span> <span data-ttu-id="69500-112">רק מחירונים שההקשר מוגדר ל **מכירות** ושהמטבע שלהם תואם את מטבע תיק הלקוח יכללו.</span><span class="sxs-lookup"><span data-stu-id="69500-112">Only price lists that have the context set to **Sales** and whose currency matches the account currency are included.</span></span>
5. <span data-ttu-id="69500-113">תן שם לשיוך ולאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="69500-113">Name the association, and then select **Save**.</span></span> <span data-ttu-id="69500-114">נוצר מחירון פרוייקט ספציפי ללקוח.</span><span class="sxs-lookup"><span data-stu-id="69500-114">A customer-specific project price list is created.</span></span> <span data-ttu-id="69500-115">מחירון זה ישמש כברירת מחדל למחירי פרויקטים בהצעות מחיר או חוזים של פרויקט שנוצרו עבור לקוח זה, כאשר התאריך היצירה של הצעת המחיר או חוזה הפרויקט נמצא במסגרת תוקף התאריך של המחירון.</span><span class="sxs-lookup"><span data-stu-id="69500-115">This price list will be used to default project prices on project quotes or contracts created for this customer where the created date of the quote or project contract falls within the date effectivity of the price list.</span></span>

## <a name="custom-pricing-on-project-quotes"></a><span data-ttu-id="69500-116">תמחור מותאם אישית בהצעות מחיר</span><span class="sxs-lookup"><span data-stu-id="69500-116">Custom pricing on project quotes</span></span>

<span data-ttu-id="69500-117">בהצעות מחיר לפרויקט, תוכלו לקבוע תמחור לפרויקט שמתחיל במחירון סטנדרטי המוגדר כברירת מחדל מהלקוח או מפרמטרי הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="69500-117">On project quotes, you can have project pricing that starts with a default standard price list that defaults from the customer or from the project parameters.</span></span>

<span data-ttu-id="69500-118">כאשר אתה זקוק לתמחור מותאם אישית לעבודה הקשורה לפרויקט בהצעת מחיר מסוימת, תוכל לקבל את זה מהישות המשויכת למחירוני הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="69500-118">When you need custom pricing for project-related work on a particular quote, you can get that from the project price lists associated entity.</span></span>

<span data-ttu-id="69500-119">בצע את השלבים הבאים להגדרת תמחור פרויקט ספציפי להצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="69500-119">Complete the following steps to set up quote-specific project pricing.</span></span>

1. <span data-ttu-id="69500-120">בהצעת מחיר הפרויקט בחר בכרטיסיה **מחירוני פרוייקט**.</span><span class="sxs-lookup"><span data-stu-id="69500-120">Open the project quote and select the **Project Price Lists** tab.</span></span>
2. <span data-ttu-id="69500-121">ברשת המשנה בחר **צור תמחור מותאם אישית**.</span><span class="sxs-lookup"><span data-stu-id="69500-121">In the subgrid, select **Create custom pricing**.</span></span>

<span data-ttu-id="69500-122">כל מחירוני הפרויקט המצורפים להצעת המחיר מועתקים למחירונים חדשים.</span><span class="sxs-lookup"><span data-stu-id="69500-122">All the project price lists that are attached to the quote are copied to new price lists.</span></span> <span data-ttu-id="69500-123">שמות המחירונים החדשים משקפים את שם הצעת המחיר עם חותמת תאריך שעה למועד יצירת מחירונים אלה.</span><span class="sxs-lookup"><span data-stu-id="69500-123">The names of the new price lists reflect the name of quote with a date-time stamp for when these price lists were created.</span></span>

<span data-ttu-id="69500-124">באפשרותך להשתמש בכל אחד מאותם מחירונים ולעדכן את מחירי העבודה (מחיר התפקיד) ומחירי ההוצאות (מחיר הקטגוריה).</span><span class="sxs-lookup"><span data-stu-id="69500-124">You can use each of those price lists and make updates to labor (role price) and expense (category price) prices.</span></span> <span data-ttu-id="69500-125">מחירים אלה יחולו רק על הצעת מחיר לפרויקט זו.</span><span class="sxs-lookup"><span data-stu-id="69500-125">These prices will only be applicable to this project quote.</span></span>

## <a name="price-lists-on-a-project-contract"></a><span data-ttu-id="69500-126">מחירונים בחוזה פרוייקט‬</span><span class="sxs-lookup"><span data-stu-id="69500-126">Price lists on a project contract</span></span>

<span data-ttu-id="69500-127">בחוזה פרוייקט, ברירת המחדל של תמחור הפרויקט הוא תמיד מחירון מותאם אישית עם שם החוזה וחותמת התאריך שנוצר מצורף לשם.</span><span class="sxs-lookup"><span data-stu-id="69500-127">On a project contract, project pricing always defaults as a custom price list with the name of contract and the created date time stamp appended to the name.</span></span> <span data-ttu-id="69500-128">זה נכון בין אם החוזה נוצר כאשר הצעת המחיר זכתה ובין אם החוזה נוצר מאפס.</span><span class="sxs-lookup"><span data-stu-id="69500-128">This is true whether the contract was created when the quote was won or if the contract was created from scratch.</span></span> <span data-ttu-id="69500-129">במידת הצורך, ניתן להסיר שיוך זה למחירון המותאם אישית ולשיך במקום זאת מחירון סטנדרטי לחוזה הפרויקט.</span><span class="sxs-lookup"><span data-stu-id="69500-129">If needed, you can remove this association to the custom price list and associate a standard price list to the project contract instead.</span></span>

<span data-ttu-id="69500-130">כאשר משייכים מחירון סטנדרטי למחירוני הפרויקט בהצעת מחיר או חוזה, כל שינוי שנעשה במחירים במחירון ישפיע על כל הצעות המחיר והחוזים שמשתמשים במחירון.</span><span class="sxs-lookup"><span data-stu-id="69500-130">When you associate a standard price list to the project price lists on quote or contract, any changes made to the prices in the price list will impact all quotes and contracts that use the price list.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]