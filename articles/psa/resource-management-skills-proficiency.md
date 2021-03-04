---
title: כישורים ומודלים של מיומנות
description: נושא זה מספק מידע על אופן השימוש בכישורים ובמודלים של מיומנות.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/13/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: c7da8b2a7eda51b2aa7cf04e325a92f33d834efc
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147474"
---
# <a name="skills-and-proficiency-models"></a><span data-ttu-id="df681-103">כישורים ומודלים של מיומנות</span><span class="sxs-lookup"><span data-stu-id="df681-103">Skills and proficiency models</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="df681-104">כישורים הם מאפייני משאב המשותפים בין Dynamics 365 Project Service Automation ובמידה והוא קיים, Dynamics 365 Field Service.</span><span class="sxs-lookup"><span data-stu-id="df681-104">Skills are resource characteristics that are shared between Dynamics 365 Project Service Automation and if present, Dynamics 365 Field Service.</span></span> 

<span data-ttu-id="df681-105">כדי לשמור על מאגר הכישורים ב- Project Service Automation, עבור אל **משאבים** \> **כישורי משאבים**.</span><span class="sxs-lookup"><span data-stu-id="df681-105">To maintain the repository of skills in Project Service Automation, go to **Resources** \> **Resource Skills**.</span></span> 

> ![כישורי משאבים](media/Resource-Management-image84.png)

## <a name="use-proficiency-models-to-rate-resources"></a><span data-ttu-id="df681-107">שימוש במודלים של מיומנות כדי לדרג משאבים</span><span class="sxs-lookup"><span data-stu-id="df681-107">Use proficiency models to rate resources</span></span>

<span data-ttu-id="df681-108">כישורים עבור משאבים מדורגים לפי מודלים של מיומנות.</span><span class="sxs-lookup"><span data-stu-id="df681-108">Skills for resources are rated by proficiency models.</span></span> <span data-ttu-id="df681-109">הדירוגים הבודדים נמצאים במודל מיומנות.</span><span class="sxs-lookup"><span data-stu-id="df681-109">The individual ratings are in a proficiency model.</span></span> 

1. <span data-ttu-id="df681-110">כדי ליצור מודל מיומנות, עבור אל **משאבים** \> **מודלים של מיומנות** ולאחר מכן בחר **חדש**.</span><span class="sxs-lookup"><span data-stu-id="df681-110">To create a proficiency model, go to **Resources** \> **Proficiency Models**, and then select **New**.</span></span>
2. <span data-ttu-id="df681-111">במודל הדירוג החדש, ציין את ערך הדירוג המינימלי, את ערך הדירוג המרבי ואת הישות המדורגת.</span><span class="sxs-lookup"><span data-stu-id="df681-111">In the new rating model, specify the minimum rating value, the maximum rating value, and the entity that is being rated.</span></span>
3. <span data-ttu-id="df681-112">ברשת המשנה **ערכי דירוג**, ניתן להגדיר את ערכי הדירוג השונים, מהערך המינימלי לערך המרבי.</span><span class="sxs-lookup"><span data-stu-id="df681-112">In the **Rating Values** subgrid, you can define the different rating values, from the minimum to the maximum.</span></span>

> ![דירוגים מינימליים ומרביים הוגדרו](media/Resource-Management-image85.png)

<span data-ttu-id="df681-114">ערכי דירוג אלה מוצגים במסננים **דרישות משאב**, **לוח זמנים** ו **מסייע לוח הזמנים**.</span><span class="sxs-lookup"><span data-stu-id="df681-114">These rating values are shown on the **Resource Requirements**, **Schedule Board**, and **Schedule Assistant** filters.</span></span>
