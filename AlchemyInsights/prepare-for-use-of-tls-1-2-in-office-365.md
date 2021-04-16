---
title: Подготовка за използване на TLS 1.2 в Microsoft 365
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085893"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="23c84-102">Подготовка за използване на TLS 1.2 в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="23c84-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="23c84-103">Считано от 31 октомври 2018 г., Microsoft 365 ще продължи преминаването към TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="23c84-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="23c84-104">От 15 октомври 2020 г. O365 ще започне намаляването на TLS 1,0 и 1,1 в цялата услуга.</span><span class="sxs-lookup"><span data-stu-id="23c84-104">Starting October 15, 2020, O365 will begin the deprecation of TLS 1.0 and 1.1 across the service.</span></span> <span data-ttu-id="23c84-105">Започването на тази промяна ще продължи през следващите няколко седмици и месеци, но клиентите трябва да предполагат, че няма повиквания на TLS 1.0/1.1, когато се ангажират с O365 от 15 октомври 2020 г.</span><span class="sxs-lookup"><span data-stu-id="23c84-105">The rollout of this change will continue over the next few weeks and months, but customers should assume no TLS 1.0/1.1 calls will work when engaging with O365 starting Oct 15, 2020.</span></span> <span data-ttu-id="23c84-106">Както беше съобщено по-рано (MC126199 през декември 2017 г., MC128929 през февруари 2018 г., MC186827 през юли 2019 г. и MC218794 през юли 2020 г.), преместваме всички наши онлайн услуги към Защита на транспортния слой (TLS) 1,2+, за да предоставим най-доброто в класа шифроване и да гарантираме, че услугата ни е по-защитена по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="23c84-106">As previously communicated (MC126199 in Dec 2017, MC128929 in Feb 2018, MC186827 in July 2019, and MC218794 in July 2020), we are moving all of our online services to Transport Layer Security (TLS) 1.2+ to provide best-in-class encryption, and to ensure our service is more secure, by default.</span></span> <span data-ttu-id="23c84-107">Клиентите все още могат да изберат TLS 1.0/1.1 на своите сървъри и ресурси, но трябва да предполагат, че само TLS 1,2 или по-нова версия ще работят при взаимодействие с ресурси на O365.</span><span class="sxs-lookup"><span data-stu-id="23c84-107">Customers can still choose to have TLS 1.0/1.1 on their servers and resources, but they should assume only TLS 1.2 or higher will work when interacting with O365 resources.</span></span>
  
<span data-ttu-id="23c84-108">За да научите повече за тези промени, вижте [тук](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) и [тук](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="23c84-108">To learn more about these changes, please see [here](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) and [here](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span></span>

  