---
title: שילוב חשבונית פרויקט
description: נושא זה מספק מידע על שילוב כתיבה כפולה עבור יצירת חשבוניות ב- Project Operations.
author: sigitac
ms.date: 04/26/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 7407c98aad79806dcbaf25e81ff3e08397b41ffe
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996567"
---
# <a name="project-invoice-integration"></a><span data-ttu-id="5d2e3-103">שילוב חשבונית פרויקט</span><span class="sxs-lookup"><span data-stu-id="5d2e3-103">Project invoice integration</span></span>

<span data-ttu-id="5d2e3-104">נושא זה מספק מידע על שילוב כתיבה כפולה עבור יצירת חשבוניות ב- Project Operations.</span><span class="sxs-lookup"><span data-stu-id="5d2e3-104">This topic provides information about Project Operations dual-write integration for customer invoicing.</span></span>

<span data-ttu-id="5d2e3-105">ב-Project Operations מנהל הפרויקט מנהל את צבר חיובי הפרויקט ויוצר חשבונית פרופורמה עבור הלקוח ב- Microsoft Dataverse.</span><span class="sxs-lookup"><span data-stu-id="5d2e3-105">In Project Operations, the Project manager manages the project billing backlog and creates a proforma invoice for the customer in Microsoft Dataverse.</span></span> <span data-ttu-id="5d2e3-106">בהתבסס על חשבונית פרופורמה זו, פקיד חשבונות חייבים או רואה חשבון פרויקט יוצר חשבונית המוצגת ללקוח.</span><span class="sxs-lookup"><span data-stu-id="5d2e3-106">Based on this proforma invoice, the Accounts receivable clerk or Project accountant creates a customer-facing invoice.</span></span> <span data-ttu-id="5d2e3-107">שילוב כתיבה כפולה מבטיח שפרטי חשבונית הפרופורמה מסונכרנים עם יישומי Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="5d2e3-107">Dual-write integration ensures that the proforma invoice details are synchronized to Finance and Operations apps.</span></span> <span data-ttu-id="5d2e3-108">לאחר פרסום החשבונית שמוצגת ללקוח, המערכת מעדכנת את נתוני הפרויקט הרלוונטיים ב- Dataverse עם הפרט החשבונאי.</span><span class="sxs-lookup"><span data-stu-id="5d2e3-108">After the customer-facing invoice is posted, the system updates the relevant project actuals in Dataverse with the accounting detail.</span></span> <span data-ttu-id="5d2e3-109">הגרפיקה הבאה מספקת סקירה קונספטואלית ברמה גבוהה על שילוב זה.</span><span class="sxs-lookup"><span data-stu-id="5d2e3-109">The following graphic provides a high-level conceptual overview of this integration.</span></span>

   ![שילוב חשבונית פרויקט](./media/DW5Invoicing.png)

<span data-ttu-id="5d2e3-111">לאחר שמנהל הפרויקט מאשר את חשבונית הפרופורמה ב- Dataverse, המידע בכותרת חשבונית פרופורמה מסתנכרן עם ישומי Finance and Operations המשתמשות במפת טבלת הכתיבה הכפולה, **הצעת חשבונית פרויקט גרסה 2 (חשבוניות)**.</span><span class="sxs-lookup"><span data-stu-id="5d2e3-111">After the Project manager confirms the proforma invoice in Dataverse, the proforma invoice header information synchronizes to Finance and Operations apps using the dual-write table map, **Project invoice proposal V2 (invoices)**.</span></span> <span data-ttu-id="5d2e3-112">זהו שילוב חד כיווני מ- Dataverse לישומי Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="5d2e3-112">This is a one-way integration from Dataverse to Finance and Operations apps.</span></span> <span data-ttu-id="5d2e3-113">יצירה או מחיקה של הצעות חשבוניות לפרויקט ישירות בישומי Finance and Operations אינן נתמכות.</span><span class="sxs-lookup"><span data-stu-id="5d2e3-113">Creating or deleting Project invoice proposals directly in Finance and Operations apps isn't supported.</span></span>

<span data-ttu-id="5d2e3-114">אישור חשבונית ב- Dataverse מפעיל גם את ההיגיון העסקי ליצירת רשומות הקשורות לחיוב בישות **נתונים בפועל**.</span><span class="sxs-lookup"><span data-stu-id="5d2e3-114">Invoice confirmation in Dataverse also triggers the business logic to create billing-related records in the **Actuals** entity.</span></span> <span data-ttu-id="5d2e3-115">רשומות של נתונים בפועל מסונכרנות עם ישומי Finance and Operations באמצעות במפת הטבלת הכתיבה הכפולה **נתוני שילוב בפועל של Project Operations ‏(msdyn\_actuals)**.</span><span class="sxs-lookup"><span data-stu-id="5d2e3-115">These records are synchronized to Finance and Operations using the dual-write table map, **Project Operations integration actuals (msdyn\_actuals).**</span></span> <span data-ttu-id="5d2e3-116">לקבלת מידע נוסף, ראה [הערכות ונתונים בפועל של פרויקט](resource-dual-write-estimates-actuals.md).</span><span class="sxs-lookup"><span data-stu-id="5d2e3-116">For more information, see [Project estimates and actuals](resource-dual-write-estimates-actuals.md).</span></span> 

<span data-ttu-id="5d2e3-117">שורות הצעת חשבונית לפרויקט נוצרות על ידי התהליך התקופתי **ייבוא אחסון זמני של טפסים**.</span><span class="sxs-lookup"><span data-stu-id="5d2e3-117">Project invoice proposal lines are created by the periodic process, **Import form staging**.</span></span> <span data-ttu-id="5d2e3-118">תהליך זה מבוסס על פרטי נתוני המכירות בפועל המחויבים בטבלה **אחסון זמני של נתונים בפועל**.</span><span class="sxs-lookup"><span data-stu-id="5d2e3-118">This process is based on the billed sales actuals details in the **Actuals staging** table.</span></span> <span data-ttu-id="5d2e3-119">למידע נוסף ראה [ניהל הצעות חשבונית לפרויקט](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals).</span><span class="sxs-lookup"><span data-stu-id="5d2e3-119">For more information, see [Manage project invoice proposals](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals).</span></span> 
