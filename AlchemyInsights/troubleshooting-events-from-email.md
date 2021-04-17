---
title: Отстраняване на неизправности със събития от имейл
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834828"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="62747-102">Отстраняване на неизправности със събития от имейл</span><span class="sxs-lookup"><span data-stu-id="62747-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="62747-103">Проверка на функцията е разрешена за пощенската кутия: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="62747-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="62747-104">След това погледнете регистрационните файлове "Събития от имейл" **Експортиране-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="62747-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="62747-105">В регистрационните файлове "Събития от имейл" намерете InternetMessageId, който отговаря на елемента в пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="62747-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="62747-106">TrustScore определя дали елементът е добавен или не.</span><span class="sxs-lookup"><span data-stu-id="62747-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="62747-107">Събития ще се добавят само ако TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="62747-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="62747-108">TrustScore се определя от свойствата SPF, Dkim или Dmarc, които са в заглавката на съобщението.</span><span class="sxs-lookup"><span data-stu-id="62747-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="62747-109">За да видите тези свойства:</span><span class="sxs-lookup"><span data-stu-id="62747-109">To view these properties:</span></span>

<span data-ttu-id="62747-110">**Настолната версия на Outlook**</span><span class="sxs-lookup"><span data-stu-id="62747-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="62747-111">Отваряне на елемента</span><span class="sxs-lookup"><span data-stu-id="62747-111">Open the item</span></span>
- <span data-ttu-id="62747-112">Свойства на > –> интернет заглавки</span><span class="sxs-lookup"><span data-stu-id="62747-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="62747-113">или</span><span class="sxs-lookup"><span data-stu-id="62747-113">or</span></span>

<span data-ttu-id="62747-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="62747-114">**MFCMapi**</span></span>

- <span data-ttu-id="62747-115">Навигиране до елемента в папката "Входящи"</span><span class="sxs-lookup"><span data-stu-id="62747-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="62747-116">Потърсете PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="62747-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="62747-117">Тези свойства се определят и записват по време на транспорт и маршрутизиране.</span><span class="sxs-lookup"><span data-stu-id="62747-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="62747-118">За по-нататъшно отстраняване на неизправности може да се наложи да следвате транспортната поддръжка за неизправностите в SPF, DKIM и.or DMARC.</span><span class="sxs-lookup"><span data-stu-id="62747-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>