---
title: Спиране на съобщенията да се преместват автоматично в архива
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523604"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="d9a39-102">Спиране на съобщенията да се преместват автоматично в архива</span><span class="sxs-lookup"><span data-stu-id="d9a39-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="d9a39-103">Ако използвате правила за съхранение, можете да промените възрастта за съхранение в тези правила, за да спрете автоматичното архивиране на съобщения.</span><span class="sxs-lookup"><span data-stu-id="d9a39-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="d9a39-104">Ето как:</span><span class="sxs-lookup"><span data-stu-id="d9a39-104">Here's how:</span></span>

1. <span data-ttu-id="d9a39-105">В [центъра за администриране на Exchange](https://go.microsoft.com/fwlink/?linkid=2059104)изберете етикети за запазване **на управлението на съответствието**  >  .</span><span class="sxs-lookup"><span data-stu-id="d9a39-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="d9a39-106">Намерете своя бутон за преместване в архивен етикет за съхранение.</span><span class="sxs-lookup"><span data-stu-id="d9a39-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="d9a39-107">В етикета за съхранение променете периода за съхранение (период на архивиране), за да **не** позволите на елементите да се архивират автоматично от правилата за съхранение.</span><span class="sxs-lookup"><span data-stu-id="d9a39-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="d9a39-108">Това ще промени настройката за архивиране за всички пощенски кутии с този етикет за съхранение, към който са приложени.</span><span class="sxs-lookup"><span data-stu-id="d9a39-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
