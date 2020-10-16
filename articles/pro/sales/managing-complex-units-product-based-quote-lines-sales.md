---
title: ניהול יחידות מורכבות, למשל לפי משתמש, או לפי חודש עבור שורות הצעות מחיר מבוססות מוצר
description: נושא זה מספק מידע על ניהול יחידות מורכבות עבור שורות הצעות מחיר מבוססות מוצר.
author: rumant
manager: Annbe
ms.date: 10/06/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 741230e69302138cce8f7379f520f7178e1c80af
ms.sourcegitcommit: fd8ea1779db2bb39a428f459ae3293c4fd785572
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/06/2020
ms.locfileid: "3965796"
---
# <a name="managing-complex-units-such-as-per-user-per-month-for-product-based-quote-lines"></a><span data-ttu-id="66d2e-103">ניהול יחידות מורכבות, למשל לפי משתמש, או לפי חודש עבור שורות הצעות מחיר מבוססות מוצר</span><span class="sxs-lookup"><span data-stu-id="66d2e-103">Managing complex units such as per-user, per-month for product-based quote lines</span></span>

<span data-ttu-id="66d2e-104">_**חל על**: פריסה בגרסת לייט – מהעסקה ועד להוצאת חשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="66d2e-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="66d2e-105">Dynamics 365 Project Operations משתמש בגורמי כמות כדי לתמוך במכירה של מוצרים מבוססי מנוי.</span><span class="sxs-lookup"><span data-stu-id="66d2e-105">Dynamics 365 Project Operations uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="66d2e-106">עבור מוצרים מבוססי מנוי, הכמות בהצעת המחיר או בסעיף החוזה של הפרויקט מבוטאת כמספר החודשים של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="66d2e-106">For subscription-based products, the quantity on the quote or project contract line is expressed as the number of user-months.</span></span>

<span data-ttu-id="66d2e-107">בדרך כלל, המחיר של תוכנת המנוי מאוחסן בקטלוג כמחיר לכל משתמש בחודש.</span><span class="sxs-lookup"><span data-stu-id="66d2e-107">Usually, the price of subscription software is stored in the catalog as the price per user per month.</span></span> <span data-ttu-id="66d2e-108">במהלך תהליך המכירה, המחיר בשורת הצעת המחיר הוא בדרך כלל מחיר לפי משתמש, לפי חודש, בתאם למשא ומתן שנוהל על-ידי סוכן מכירות של מחלקת ה- IT.</span><span class="sxs-lookup"><span data-stu-id="66d2e-108">During the sales process, the price on the quote line is usually the per-user, per-month price that was negotiated and discounted by the IT sales agent.</span></span> <span data-ttu-id="66d2e-109">לכל עסקה יש מספר שונה של משתמשים ומספר שונה של חודשי מנוי.</span><span class="sxs-lookup"><span data-stu-id="66d2e-109">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="66d2e-110">הכמות המשמשת לחישוב שורת הצעת המחיר היא תוצר של מספר המשתמשים ומספר חודשי המנוי.</span><span class="sxs-lookup"><span data-stu-id="66d2e-110">The quantity used to compute the quote line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="66d2e-111">כדי לתמוך בסוג זה של מכירה, Project Operations הציג את הרעיון של גורמי כמות.</span><span class="sxs-lookup"><span data-stu-id="66d2e-111">To support this type of sale, Project Operations introduced the concept of quantity factors.</span></span> <span data-ttu-id="66d2e-112">גורמי כמות מסתמכים על תכונות המוצר ב- Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="66d2e-112">Quantity factors rely on the product attributes in Dynamics 365.</span></span> <span data-ttu-id="66d2e-113">בעת קביעת תצורה של מאפיינים מסוימים עבור מוצר, Project Operations מאפשר לך לסמן בדגל קבוצת משנה, או את כל המאפיינים, כגורמי כמות.</span><span class="sxs-lookup"><span data-stu-id="66d2e-113">When you configure specific properties for a product, Project Operations lets you flag a subset, or all of the properties, as quantity factors.</span></span>

<span data-ttu-id="66d2e-114">Project Operations מאמתת שרק מאפיינים מספריים או מאפייני מוצר בעלי סוג נתונים מספרי מסומנים בדגל כגורמי כמות.</span><span class="sxs-lookup"><span data-stu-id="66d2e-114">Project Operations validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="66d2e-115">כשמוסיפים מוצר עם גורמי כמות לשורת הצעת מחיר, השדה **כמות** הופך לשדה לקריאה בלבד.</span><span class="sxs-lookup"><span data-stu-id="66d2e-115">When you add a product with quantity factors to a quote line, the **Quantity** field becomes read-only.</span></span> <span data-ttu-id="66d2e-116">לאחר הזנת ערכים עבור מאפייני מוצר שהם גורמי כמות, Project Operations מחשב את הכמות של שורת הצעת המחיר.</span><span class="sxs-lookup"><span data-stu-id="66d2e-116">After you enter values for product properties that are quantity factors, Project Operations calculates the quantity of the quote line.</span></span>

<span data-ttu-id="66d2e-117">לדוגמה, ייתכן שב-Dynamics 365 Sales יהיו המאפיינים הבאים:</span><span class="sxs-lookup"><span data-stu-id="66d2e-117">For example, Dynamics 365 Sales might have the following properties:</span></span>

- <span data-ttu-id="66d2e-118">**מס' המשתמשים**: מספר המשתמשים</span><span class="sxs-lookup"><span data-stu-id="66d2e-118">**No of users**: The number of users</span></span>
- <span data-ttu-id="66d2e-119">**מס' החודשים**: מספר חודשי המנוי</span><span class="sxs-lookup"><span data-stu-id="66d2e-119">**No of Months**: The number of subscription months</span></span>
- <span data-ttu-id="66d2e-120">**SKU של מוצר**</span><span class="sxs-lookup"><span data-stu-id="66d2e-120">**Product SKU**</span></span>

<span data-ttu-id="66d2e-121">ניתן לסמן בדגל את המאפיין **מס' המשתמשים** ואת המאפיין **מס' החודשים** כגורמי כמות על ידי עריכת המאפיינים של שורת המוצר.</span><span class="sxs-lookup"><span data-stu-id="66d2e-121">You can flag the **No of Users** and **No of Months** properties as quantity factors by editing the properties of the product line.</span></span>

<span data-ttu-id="66d2e-122">ליצירת גורמי כמות ממאפייני המוצר, בצע את הצעדים הבאים:</span><span class="sxs-lookup"><span data-stu-id="66d2e-122">To create Quantity factors from Product properties, follow these steps:</span></span>

1. <span data-ttu-id="66d2e-123">בחלונית הניווט הימנית של Project Operations, עבור אל **מכירות** > **מוצרים**.</span><span class="sxs-lookup"><span data-stu-id="66d2e-123">On the Project Operations left navigation pane, go to **Sales** > **Products**.</span></span>
2. <span data-ttu-id="66d2e-124">פתח את המוצר שעבורו עליך להגדיר גורמי כמות.</span><span class="sxs-lookup"><span data-stu-id="66d2e-124">Open the product for which you need to configure quantity factors.</span></span> <span data-ttu-id="66d2e-125">ודא שלמוצר יש מאפיינים שכבר הוגדרו.</span><span class="sxs-lookup"><span data-stu-id="66d2e-125">Make sure the product has properties already configured.</span></span>
3. <span data-ttu-id="66d2e-126">בדף **פרטי הפרויקט** של המוצר, בחר את הכרטיסיה **גורמי כמות**.</span><span class="sxs-lookup"><span data-stu-id="66d2e-126">On the **Project Information** page for the Product, select the **Quantity Factors** tab.</span></span>
4. <span data-ttu-id="66d2e-127">ברשת המשנה, בחר **+ חישוב שדה חדש‬**.</span><span class="sxs-lookup"><span data-stu-id="66d2e-127">In the subgrid, select **+ New field computation**.</span></span>
5. <span data-ttu-id="66d2e-128">הזן את שם גורם הכמות ובחר את ערך המאפיין הממופה לחישוב השדה.</span><span class="sxs-lookup"><span data-stu-id="66d2e-128">Enter the name of the Quantity factor and select the property value that maps to the field computation.</span></span>
6. <span data-ttu-id="66d2e-129">שמור וסגור את הטופס.</span><span class="sxs-lookup"><span data-stu-id="66d2e-129">Save and close the form.</span></span> <span data-ttu-id="66d2e-130">חזור על שלבים אלה עבור כל המאפיינים שישמשו לחישוב הכמות עבור שורת הצעת המחיר מבוססת המוצר.</span><span class="sxs-lookup"><span data-stu-id="66d2e-130">Repeat these steps for all properties to use for computing the quantity for the product-based quote line.</span></span>

<span data-ttu-id="66d2e-131">כאשר יוצרים שורת הצעת מחיר מבוססת מוצר עבור מוצר, כמות שורת הצעת המחיר תינעל.</span><span class="sxs-lookup"><span data-stu-id="66d2e-131">When you create a product-based quote line for a product, the quantity of the quote line will be locked.</span></span> <span data-ttu-id="66d2e-132">הכמות תחושב כמוצר של ערכי המאפיינים שהזנת עבור אותה שורת הצעת מחיר.</span><span class="sxs-lookup"><span data-stu-id="66d2e-132">The quantity will be computed as a product of the property values that you input for that quote line.</span></span>
