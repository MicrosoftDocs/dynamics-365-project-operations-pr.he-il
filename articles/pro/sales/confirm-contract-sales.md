---
title: אישור חוזה פרויקט
description: נושא זה מספק מידע על אופן אישור פרויקט ב-Project Operations .
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 24da0887c0266d51bddcbbf8efd6f2644b6d0f4f
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 10/28/2020
ms.locfileid: "4128284"
---
# <a name="confirm-a-project-contract"></a><span data-ttu-id="04e46-103">אישור חוזה פרויקט</span><span class="sxs-lookup"><span data-stu-id="04e46-103">Confirm a project contract</span></span>

<span data-ttu-id="04e46-104">_**חל על:** Project Operations לתרחישים מבוססי משאבים/לא מלאי, פריסה קלה - עסקה בחשבונית פרופורמה_</span><span class="sxs-lookup"><span data-stu-id="04e46-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="04e46-105">חוזה פרויקט ב-Dynamics 365 Project Operations יכול להיות פעיל עם סיבת מצב **מאושר**, או סגור עם סיבת מצב **הפסד**.</span><span class="sxs-lookup"><span data-stu-id="04e46-105">A project contract in Dynamics 365 Project Operations can be active with a reason of **Confirmed**, or closed with a reason of **Lost**.</span></span> <span data-ttu-id="04e46-106">כאשר מאשרים חוזה פרויקט, המצב מתעדכן מ **טיוטה** ל **פעיל** וסיבת המצב היא **מאושר**.</span><span class="sxs-lookup"><span data-stu-id="04e46-106">When you confirm a project contract, the status updates from **Draft** to **Active** and the status reason is **Confirmed**.</span></span> <span data-ttu-id="04e46-107">לא ניתן לערוך או לפתוח חוזה פעיל או סגור.</span><span class="sxs-lookup"><span data-stu-id="04e46-107">An active or closed contract can't be edited or reopened.</span></span> 

### <a name="financial-impact-of-confirming-a-project-contract"></a><span data-ttu-id="04e46-108">השפעה פיננסית של אישור חוזה פרויקט</span><span class="sxs-lookup"><span data-stu-id="04e46-108">Financial impact of confirming a project contract</span></span>

<span data-ttu-id="04e46-109">לאחר אישור חוזה פרויקט, היישום יחשב מחדש את העלויות על-ידי ביטול נתוני עלות בפועל ישנים יותר ויצירה של נתוני עלות בפועל חדשים.</span><span class="sxs-lookup"><span data-stu-id="04e46-109">After a project contract is confirmed, the application recalculates the costs by reversing the older cost actuals and creating new cost actuals.</span></span> <span data-ttu-id="04e46-110">אחר כך היישום יעבד את נתוני העלות בפועל החדשים בהתבסס על שיטת החיוב של סעיף החוזה המשויך לפרוייקט.</span><span class="sxs-lookup"><span data-stu-id="04e46-110">The new cost actuals are then processed based on the billing method of the associated project contract line.</span></span> <span data-ttu-id="04e46-111">אם נתוני העלות בפועל מתייחסים לסעיף חוזה של זמן וחומרים, היישום יוצר מחדש נתוני המכירות בפועל תואמים שלא חויבו.</span><span class="sxs-lookup"><span data-stu-id="04e46-111">If the cost actuals reference a Time and Material contract line, the application automatically re-creates corresponding unbilled sales actuals.</span></span> <span data-ttu-id="04e46-112">אם נתוני העלות בפועל מתייחסים לשורת חוזה של מחיר קבוע, היישום מפסיק לעבד מחדש את נתוני העלות בפועל.</span><span class="sxs-lookup"><span data-stu-id="04e46-112">If the cost actuals reference a Fixed Price contract line, the application stops reprocessing the cost actuals.</span></span>

<span data-ttu-id="04e46-113">ממגבלות 'אין לחרוג', הגדרת חיוב ותמחור ותמחיר בנתונים בפועל עוברים הערכה ולאחר מכן מתעדכנים כחלק מתהליך האישורים.</span><span class="sxs-lookup"><span data-stu-id="04e46-113">Not-to-exceed limits, chargeability setup, and pricing and costing on the actuals is evaluated and then updated as part of the confirmations process.</span></span>

## <a name="close-a-project-contract-as-lost"></a><span data-ttu-id="04e46-114">סגירת חוזה פרויקט כהפסד</span><span class="sxs-lookup"><span data-stu-id="04e46-114">Close a project contract as lost</span></span>

<span data-ttu-id="04e46-115">כאשר סוגרים חוזה פרויקט כהספד, מצב החוזה מתעדכן ל **סגור** וה-סיבת המצב הוא **הפסד**.</span><span class="sxs-lookup"><span data-stu-id="04e46-115">When you close a project contract as lost, the contract status is updated to **Closed** and the status reason is **Lost**.</span></span> <span data-ttu-id="04e46-116">חוזה הפרויקט עובר למצב 'לקריאה בלבד'.</span><span class="sxs-lookup"><span data-stu-id="04e46-116">The project contract becomes read-only.</span></span> <span data-ttu-id="04e46-117">מוצגת תיבת דו-שיח לאישור לפני השלמת השינויים מכיוון שלא ניתן לפתוח חוזה פרויקט סגור מחדש.</span><span class="sxs-lookup"><span data-stu-id="04e46-117">A confirmation dialog is provided before the changes are complete because you can't reopen a closed project contract.</span></span>

<span data-ttu-id="04e46-118">אם חוזה הפרויקט שנסגר כהפסד מתייחס לפרויקט בסעיפים שלו, גם פרויקט מסומן גם כסגור.</span><span class="sxs-lookup"><span data-stu-id="04e46-118">If the project contract that is closed as lost references a project on its lines, that project is also marked as closed.</span></span> <span data-ttu-id="04e46-119">כל הזמנות המשאבים מאותו יום ואילך מבוטלות.</span><span class="sxs-lookup"><span data-stu-id="04e46-119">Any resource bookings from that day forward are canceled.</span></span> <span data-ttu-id="04e46-120">כל נתוני המכירות בפועל שטרם חויבו בחוזה הפרויקט, אשר עדיין לא רשומים בחשבונית, יבוטלו.</span><span class="sxs-lookup"><span data-stu-id="04e46-120">Any unbilled sales actuals on the project contract that aren't already on an invoice, will be reversed.</span></span>

> [!NOTE]
> <span data-ttu-id="04e46-121">ב-Dynamics 365 Project Operations, סגירת חוזה פרויקט כהפסד לא תשפיע על המצב של ההזדמנות המשויכת.</span><span class="sxs-lookup"><span data-stu-id="04e46-121">In Dynamics 365 Project Operations, closing a project contract as lost will not impact that status of the associated opportunity.</span></span> <span data-ttu-id="04e46-122">ההזדמנות תישאר פתוחה ויש לסגור אותה ידנית.</span><span class="sxs-lookup"><span data-stu-id="04e46-122">The opportunity will remain open and must be manually closed.</span></span>
