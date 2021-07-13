---
title: Набор за изходящи релета
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381575"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="6d80a-102">Набор за изходящи релета</span><span class="sxs-lookup"><span data-stu-id="6d80a-102">Outbound relay pool</span></span>

<span data-ttu-id="6d80a-103">Microsoft прави някои промени в конфигурацията за препращане или препращане на имейл чрез Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6d80a-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="6d80a-104">Съобщенията в определени сценарии се препращат или препращат през Microsoft 365 с помощта на специален набор от релета.</span><span class="sxs-lookup"><span data-stu-id="6d80a-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="6d80a-105">Съобщенията, изпратени с помощта на набора от релета, може да се появи в папката за нежелана поща на получателя.</span><span class="sxs-lookup"><span data-stu-id="6d80a-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="6d80a-106">За повече информация вижте [Изходящи пулове за доставка](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="6d80a-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="6d80a-107">За да избегнете сценарий с помощта на набора релета, уверете се, че препратените/препредаваните съобщения отговарят на един от следните критерии:</span><span class="sxs-lookup"><span data-stu-id="6d80a-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="6d80a-108">Изходящите податели са приет домейн на клиента.</span><span class="sxs-lookup"><span data-stu-id="6d80a-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="6d80a-109">Рамката за правила за податели (SPF) преминава, когато съобщението се Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6d80a-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="6d80a-110">Идентифицираната поща на DomainKeys (DKIM) в домейна на подателя на P2 преминава, когато съобщението се Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6d80a-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="6d80a-111">Съобщенията, които отговарят на горните критерии, не се препредава през набора от релета.</span><span class="sxs-lookup"><span data-stu-id="6d80a-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="6d80a-112">Ако MX записът за вашия домейн е насочен към сървър на друг или на локалния сървър, използвайте разширено филтриране, за да се уверите, че проверката на SPF е правилна за входящите имейли и за да избегнете изпращането на имейли през набора от релета.</span><span class="sxs-lookup"><span data-stu-id="6d80a-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="6d80a-113">**Как можем да кажем дали сме засегнати от набора за релета?**</span><span class="sxs-lookup"><span data-stu-id="6d80a-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="6d80a-114">Ако вашите препратени или препредавани имейли използват един от горните критерии, съобщенията няма да бъдат предавани през набора релета.</span><span class="sxs-lookup"><span data-stu-id="6d80a-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="6d80a-115">Ако обаче съобщение се изпраща през набор за реле, IP адресът на изходящия сървър е в диапазона 40.95.0.0/16 и името на изходящия сървър включва **rly** в името.</span><span class="sxs-lookup"><span data-stu-id="6d80a-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

