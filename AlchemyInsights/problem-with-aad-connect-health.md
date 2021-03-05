---
title: Проблем със здравето на пад Connect
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480993"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="6ace4-102">Проблем със здравето на пад Connect</span><span class="sxs-lookup"><span data-stu-id="6ace4-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="6ace4-103">Уверете се, че сте упълномощени за извършване на операцията.</span><span class="sxs-lookup"><span data-stu-id="6ace4-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="6ace4-104">Глобалните администратори имат достъп по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="6ace4-104">Global Admins have access by default.</span></span> <span data-ttu-id="6ace4-105">Освен това можете да използвате [управление на достъпа, базирано на роли](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , за да предоставите разрешение за регистрация на представители.</span><span class="sxs-lookup"><span data-stu-id="6ace4-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="6ace4-106">Уверете се, че задължителните крайни точки са разрешени и не са блокирани поради защитната стена.</span><span class="sxs-lookup"><span data-stu-id="6ace4-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="6ace4-107">За подробности вижте [изисквания](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="6ace4-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="6ace4-108">Регистрирането може да се провали поради изходящата комуникация, която се подлага на SSL проверка от мрежовия слой.</span><span class="sxs-lookup"><span data-stu-id="6ace4-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="6ace4-109">Уверете се, че сте проверили настройките за известяване за Azure AD Connect Health.</span><span class="sxs-lookup"><span data-stu-id="6ace4-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="6ace4-110">Моля, прегледайте настройката си.</span><span class="sxs-lookup"><span data-stu-id="6ace4-110">Please review your setting.</span></span> <span data-ttu-id="6ace4-111">Това [ръководство](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) може да ви помогне да разберете как да конфигурирате настройките за известяване за известия за изправност на Azure ad Connect.</span><span class="sxs-lookup"><span data-stu-id="6ace4-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="6ace4-112">За да научите повече за отчета за здравословно синхронизиране на пад-свързване и как да го изтеглите, вижте [отчет за синхронизиране на ниво на обект](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="6ace4-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="6ace4-113">За отстраняване на неизправности при свързване с пад на здравето, следвайте инструкциите [за отстраняване на неизправности за пад на известията за изправност на данните](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) и често задавани въпроси вижте [Общи въпроси за инсталиране на здравето на пад](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="6ace4-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
