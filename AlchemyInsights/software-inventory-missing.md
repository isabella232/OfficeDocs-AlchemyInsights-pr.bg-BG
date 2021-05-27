---
title: Софтуерните наличности липсват или са неточни
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676081"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="79b5d-102">Софтуерните наличности липсват или са неточни</span><span class="sxs-lookup"><span data-stu-id="79b5d-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="79b5d-103">Софтуерните наличности в Threat and Vulnerability Management (TVM) е списък на известен софтуер във вашата организация с официални enumerations на обща платформа (CPE).</span><span class="sxs-lookup"><span data-stu-id="79b5d-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="79b5d-104">Софтуерните продукти без официална CPE нямат публикувани уязвимости.</span><span class="sxs-lookup"><span data-stu-id="79b5d-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="79b5d-105">Инвентарът включва и подробности, като например името на доставчика, броя на слабите страни, заплахите и броя на експонираните устройства.</span><span class="sxs-lookup"><span data-stu-id="79b5d-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="79b5d-106">Промените в софтуера на устройства обикновено се отразяват в порталите за защита в рамките на два часа.</span><span class="sxs-lookup"><span data-stu-id="79b5d-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="79b5d-107">Понякога обаче може да отнеме повече време.</span><span class="sxs-lookup"><span data-stu-id="79b5d-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="79b5d-108">В момента няма начин за принудително синхронизиране; това е непрекъсната непрекъсната оценка.</span><span class="sxs-lookup"><span data-stu-id="79b5d-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="79b5d-109">Ако сте направили промяна на софтуера и промяната не е точно отразена в TVM след 5 часа, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="79b5d-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="79b5d-110">Проверете секцията за софтуерни доказателства, за да разберете как е открит софтуерът.</span><span class="sxs-lookup"><span data-stu-id="79b5d-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="79b5d-111">Уверете се, че софтуерът се поддържа.</span><span class="sxs-lookup"><span data-stu-id="79b5d-111">Make sure that the software is supported.</span></span> <span data-ttu-id="79b5d-112">Софтуерът може да се вижда само на ниво устройство дори ако в момента не се поддържа от Threat and Vulnerability Management.</span><span class="sxs-lookup"><span data-stu-id="79b5d-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="79b5d-113">Налични са обаче само ограничени данни.</span><span class="sxs-lookup"><span data-stu-id="79b5d-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="79b5d-114">За стъпки, за да съобщите за неточност от портала, вижте [Докладване на неточност](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span><span class="sxs-lookup"><span data-stu-id="79b5d-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="79b5d-115">**Забележка:** Съобщаването за неточност от портала на MDE е еднопосочен канал за инженерни дейности.</span><span class="sxs-lookup"><span data-stu-id="79b5d-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="79b5d-116">Ако проблемът е спешен, отворете билет за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="79b5d-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="79b5d-117">За повече информация вижте [Софтуерни наличности – Threat and Vulnerability Management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="79b5d-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>