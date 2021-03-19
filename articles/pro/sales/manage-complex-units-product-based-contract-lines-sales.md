---
title: ניהול יחידות מורכבות עבור סעיפי חוזה המבוססי מוצר - לייט
description: נושא זה מספק מידע על תמיכה במכירת מוצרים מבוססי מנוי.
author: rumant
manager: Annbe
ms.date: 10/28/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 029d2aa4fd20fc036a34ae6136fe12454f3b7703
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5273334"
---
# <a name="manage-complex-units-for-product-based-contract-lines---lite"></a><span data-ttu-id="5bbd1-103">ניהול יחידות מורכבות עבור סעיפי חוזה המבוססי מוצר - לייט</span><span class="sxs-lookup"><span data-stu-id="5bbd1-103">Manage complex units for product-based contract lines - lite</span></span>

<span data-ttu-id="5bbd1-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="5bbd1-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="5bbd1-105">Dynamics 365 Project Operations משתמש בגורמי כמות כדי לתמוך במכירה של מוצרים מבוססי מנוי.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-105">Dynamics 365 Project Operations uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="5bbd1-106">עבור מוצרים מבוססי מנוי, הכמות בחוזה או בסעיף החוזה של הפרויקט מבוטאת כמספר החודשי משתמש.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-106">For subscription-based products, the quantity on the contract or project contract line is expressed as the number of user-months.</span></span>

<span data-ttu-id="5bbd1-107">בדרך כלל, המחיר של תוכנת המנוי מאוחסן בקטלוג כמחיר למשתמש לחודש.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-107">The price of subscription software is stored in the catalog as the price per-user, per-month.</span></span> <span data-ttu-id="5bbd1-108">במהלך תהליך המכירה, המחיר בסעיף החוזה הוא בדרך כלל מחיר למשתמש, לחודש, שעליו הוסכם עם במשא ומתן שנוהל על-ידי סוכן מכירות.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-108">During the sales process, the price on the contract line is usually the per-user, per-month price that was negotiated and discounted by the sales agent.</span></span> <span data-ttu-id="5bbd1-109">לכל עסקה יש מספר שונה של משתמשים ומספר שונה של חודשי מנוי.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-109">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="5bbd1-110">הכמות המשמשת לחישוב הסכום של סעיף החוזה היא תוצר של מספר המשתמשים ומספר חודשי המנוי.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-110">The quantity used to calculate the amount of the contract line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="5bbd1-111">כדי לתמוך בסוג זה של מכירה, Project Operations תומכת במושג של *גורמי כמות*.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-111">To support this type of sale, Project Operations supports the concept of *quantity factors*.</span></span> <span data-ttu-id="5bbd1-112">גורמי כמות מסתמכים על תכונות המוצר.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-112">Quantity factors rely on product attributes.</span></span> <span data-ttu-id="5bbd1-113">בעת קביעת תצורה של מאפיינים מסוימים עבור מוצר, אפשר לסמן קבוצת משנה של מאפיינים אלה, או את כל המאפיינים, כגורמי כמות.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-113">When you configure specific properties for a product, you can flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="5bbd1-114">Project Operations מאמתת שרק מאפיינים מספריים או מאפייני מוצר בעלי סוג נתונים מספרי מסומנים בדגל כגורמי כמות.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-114">Project Operations validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="5bbd1-115">כאשר מוצר עם גורמי כמות מוגדרים מתווסף לסעיף חוזה, השדה **כמות** הופך לשדה לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-115">When a product with configured quantity factors is added to a contract line, the **Quantity** field  becomes read-only.</span></span> <span data-ttu-id="5bbd1-116">לאחר הזנת ערכים עבור מאפייני מוצר שהם גורמי כמות, Project Operations מחשב את הכמות של סעיף החוזה.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-116">After you enter values for product properties that are quantity factors, Project Operations calculates the quantity of the contract line.</span></span>

<span data-ttu-id="5bbd1-117">לדוגמה, ייתכן שב-Dynamics 365 Sales יהיו המאפיינים הבאים:</span><span class="sxs-lookup"><span data-stu-id="5bbd1-117">For example, Dynamics 365 Sales might have the following properties:</span></span>

- <span data-ttu-id="5bbd1-118">**מס' המשתמשים**: מספר המשתמשים.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-118">**No of users**: The number of users.</span></span>
- <span data-ttu-id="5bbd1-119">**מס' החודשים**: מספר חודשי המנוי.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-119">**No of Months**: The number of subscription months.</span></span>
- <span data-ttu-id="5bbd1-120">**SKU של מוצר**: יחידת אחסון המלאי (SKU) עבור המוצר.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-120">**Product SKU**: The stock keeping unit (SKU) for the product.</span></span>

<span data-ttu-id="5bbd1-121">ניתן לסמן את המאפיין **מס' המשתמשים** ואת המאפיין **מס' החודשים** כגורמי כמות על-ידי עריכת המאפיינים של שורת המוצר.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-121">The **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span>

<span data-ttu-id="5bbd1-122">כדי ליצור גורמי כמות ממאפייני המוצר, בצע את השלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-122">To create quantity factors from product properties, complete the following steps.</span></span>

1. <span data-ttu-id="5bbd1-123">ב-**Project Operations**, בחר **מוצרי מכירה**.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-123">On the **Project Operations**, select **Sales-Products**.</span></span>
2. <span data-ttu-id="5bbd1-124">פתח את המוצר שעבורו אתה צריך להגדיר גורמי כמות.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-124">Open the product for which you need to set up quantity factors.</span></span> <span data-ttu-id="5bbd1-125">וודא שלמוצר יש מאפיינים שכבר הוגדרו.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-125">Make sure that the product has properties already set up.</span></span>
3. <span data-ttu-id="5bbd1-126">בדף **פרטי פרויקט** בחר את הכרטיסיה **גורמי כמות**.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-126">On the **Project Information** page, select the **Quantity Factors** tab.</span></span>
4. <span data-ttu-id="5bbd1-127">ברשת המשנה, בחר **+ חישוב שדה חדש‬**.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-127">In the subgrid, select **+ New field computation**.</span></span>
5. <span data-ttu-id="5bbd1-128">הזן את שם **גורם הכמות** ובחר את ערך המאפיין הממופה לחישוב השדה.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-128">Enter the name of the **Quantity Factor** and select the property value that maps to the field computation.</span></span>
6. <span data-ttu-id="5bbd1-129">שמור וסגור את הטופס.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-129">Save and close the form.</span></span>
7. <span data-ttu-id="5bbd1-130">חזור על שלבים 2-6 עבור כל המאפיינים שביחד יהוו את הכמות עבור סעיף החוזה מבוסס המוצר.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-130">Repeat steps 2-6 for all the properties that together will make up the quantity for the product-based contract line.</span></span>

<span data-ttu-id="5bbd1-131">לאחר הגדרת גורמי כמות, כאשר המשתמש יוצר סעיף חוזה עבור מוצר זה, הכמות של סעיף החוזה נעולה.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-131">With quantity factors set up, when the user creates a contract line for this product, the quantity of the contract line is locked.</span></span> <span data-ttu-id="5bbd1-132">הכמות מחושבת לאחר מכן כתוצר של ערכי המאפיינים עבור אותו סעיף חוזה.</span><span class="sxs-lookup"><span data-stu-id="5bbd1-132">The quantity is then calculated as a product of the property values for that contract line.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]