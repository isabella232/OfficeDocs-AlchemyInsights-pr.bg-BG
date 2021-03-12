---
title: Не можете да изпращате/получавате имейл до/от Office 365, тъй като е дезактивирано TLS 1,0 и TLS 1,1
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
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743187"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="af05f-102">Не можете да изпращате/получавате имейл до/от Office 365, тъй като е дезактивирано TLS 1,0 и TLS 1,1</span><span class="sxs-lookup"><span data-stu-id="af05f-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="af05f-103">Както е потвърдено от центъра за съобщения Post MC229914, TLS 1,0 и неодобрението на TLS 1,1 започва да прилага за крайни точки за пощенския поток за Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="af05f-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="af05f-104">Скоро Office 365 вече няма да приема TLS 1,0 и TLS 1,1 имейл връзки от външни източници.</span><span class="sxs-lookup"><span data-stu-id="af05f-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="af05f-105">Освен това Exchange Online никога няма да използва TLS 1,0 или 1,1, за да изпраща изходящи имейли.</span><span class="sxs-lookup"><span data-stu-id="af05f-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="af05f-106">Ако сте изправени пред проблеми поради TLS 1,0 или 1,1 за инвалидност, е възможно да се сблъскате с една от следните грешки:</span><span class="sxs-lookup"><span data-stu-id="af05f-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="af05f-107">Подателят получава отскачане на NDR обратно-"421 4.4.2 връзката е спаднал поради SocketError"</span><span class="sxs-lookup"><span data-stu-id="af05f-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="af05f-108">Грешка в визуализатора на опашката на локален сървър, който изпраща имейл до служител 365-"421 4.4.2 връзката е спаднал поради SocketError"</span><span class="sxs-lookup"><span data-stu-id="af05f-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="af05f-109">Грешка при изпращане на [регистрационен файл на протокола](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) за свързване на сървъра за изпращане на имейл до Office 365 – TLS неуспешно водене на преговори с грешка SocketError</span><span class="sxs-lookup"><span data-stu-id="af05f-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="af05f-110">Грешка при изпращане или получаване на регистрационен файл на свързващия протокол – "451 5.7.3 трябва първо да издаде командата STARTTLS"</span><span class="sxs-lookup"><span data-stu-id="af05f-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="af05f-111">Ако имате някоя от горните грешки, се уверете, че сървърът, на който се изпращат или получават имейли, има активиран TLS 1,2, като отметнете следните ключове от системния регистър:</span><span class="sxs-lookup"><span data-stu-id="af05f-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="af05f-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ клиент] **"DisabledByDefault" = DWORD: 00000000 "активиран" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ Server] **"DisabledByDefault" = DWORD: 00000000 "активиран" = DWORD: 00000001**</span><span class="sxs-lookup"><span data-stu-id="af05f-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="af05f-113">Ако направите промяна в горните ключове от системния регистър, за да разрешите TLS 1,2, рестартирайте сървъра, за да влязат в сила промените.</span><span class="sxs-lookup"><span data-stu-id="af05f-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="af05f-114">Също така се уверете, че разполагате с най-новите актуализации за Windows и Exchange.</span><span class="sxs-lookup"><span data-stu-id="af05f-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="af05f-115">За повече информация вижте:</span><span class="sxs-lookup"><span data-stu-id="af05f-115">For more information, see:</span></span>

- [<span data-ttu-id="af05f-116">Ръководство за TLS за Exchange Server, част 1: подготовка за TLS 1,2 – общност на Microsoft Tech</span><span class="sxs-lookup"><span data-stu-id="af05f-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="af05f-117">Ориентиране на Exchange Server TLS част 2: разрешаване на TLS 1,2 и идентифициране на клиенти, които не го използват – общност на Microsoft Tech</span><span class="sxs-lookup"><span data-stu-id="af05f-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="af05f-118">Разберете сценариите за имейл, ако не могат да бъдат договорени версии на TLS с Exchange Online – общност на Microsoft Tech</span><span class="sxs-lookup"><span data-stu-id="af05f-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
