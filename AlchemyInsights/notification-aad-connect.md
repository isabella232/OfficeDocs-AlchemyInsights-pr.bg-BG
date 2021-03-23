---
title: Свързване чрез пад на известията
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034916"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="4f789-102">Свързване чрез пад на известията</span><span class="sxs-lookup"><span data-stu-id="4f789-102">Notification AAD Connect</span></span>

- <span data-ttu-id="4f789-103">Уверете се, че сте упълномощени за извършване на операцията.</span><span class="sxs-lookup"><span data-stu-id="4f789-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="4f789-104">Глобалните администратори имат достъп по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="4f789-104">Global Admins have access by default.</span></span> <span data-ttu-id="4f789-105">Освен това можете да използвате [управление на достъпа, базирано на роли](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , за да предоставите разрешение за регистрация на представители.</span><span class="sxs-lookup"><span data-stu-id="4f789-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="4f789-106">Уверете се, че задължителните крайни точки са разрешени и не са блокирани поради защитната стена.</span><span class="sxs-lookup"><span data-stu-id="4f789-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="4f789-107">За подробности вижте [изисквания](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="4f789-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="4f789-108">Регистрирането може да се провали поради изходящата комуникация, която се подлага на SSL проверка от мрежовия слой.</span><span class="sxs-lookup"><span data-stu-id="4f789-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="4f789-109">Уверете се, че сте проверили настройките за известяване за Azure AD Connect Health и прегледайте настройката си.</span><span class="sxs-lookup"><span data-stu-id="4f789-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="4f789-110">За да разберете как да конфигурирате настройките за известия за уведомления за Azure AD Connect Health, вижте това [ръководство](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span><span class="sxs-lookup"><span data-stu-id="4f789-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="4f789-111">За да научите повече за отчета за здравословно синхронизиране на пад-свързване и как да го изтеглите, вижте [отчет за синхронизиране на ниво на обект](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="4f789-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="4f789-112">За отстраняване на неизправности при известия за изправност на пад следвайте инструкциите [за отстраняване на неизправности за пад на известията за изправност на изправността](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) и често задавани въпроси вижте [Общи въпроси за инсталиране на здравето на пад](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="4f789-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
