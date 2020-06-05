---
title: Отстраняване на неизправности при събития от имейл
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44568907"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="71b1f-102">Отстраняване на неизправности при събития от имейл</span><span class="sxs-lookup"><span data-stu-id="71b1f-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="71b1f-103">Проверете функцията е разрешена за пощенска кутия: \*\*Get-EventsFromEmailConfiguration -самоличност <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="71b1f-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="71b1f-104">След това погледнете "Събития от имейл" регистрационни файлове **експортиране-пощенска кутияDiagnosticLogs-Component <mailbox> TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="71b1f-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="71b1f-105">В регистрационните файлове "Събития от имейл" намерете InternetMessageId, който отговаря на елемента в пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="71b1f-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="71b1f-106">В TrustScore се определя дали елементът е добавен или не.</span><span class="sxs-lookup"><span data-stu-id="71b1f-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="71b1f-107">Събитията ще бъдат добавени само ако доверителният талона = "Надежден".</span><span class="sxs-lookup"><span data-stu-id="71b1f-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="71b1f-108">TrustScore се определя от SPF, Dkim или Dmarc свойства, които са в заглавната част на съобщението.</span><span class="sxs-lookup"><span data-stu-id="71b1f-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="71b1f-109">За да видите тези свойства:</span><span class="sxs-lookup"><span data-stu-id="71b1f-109">To view these properties:</span></span>

<span data-ttu-id="71b1f-110">**Работен плот На Outlook**</span><span class="sxs-lookup"><span data-stu-id="71b1f-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="71b1f-111">Отваряне на елемента</span><span class="sxs-lookup"><span data-stu-id="71b1f-111">Open the item</span></span>
- <span data-ttu-id="71b1f-112">Свойства на > файлове -> интернет заглавки</span><span class="sxs-lookup"><span data-stu-id="71b1f-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="71b1f-113">Или</span><span class="sxs-lookup"><span data-stu-id="71b1f-113">or</span></span>

<span data-ttu-id="71b1f-114">**1000000000000**</span><span class="sxs-lookup"><span data-stu-id="71b1f-114">**MFCMapi**</span></span>

- <span data-ttu-id="71b1f-115">Навигирайте до елемента във входящата поща</span><span class="sxs-lookup"><span data-stu-id="71b1f-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="71b1f-116">Търси PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="71b1f-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="71b1f-117">Тези свойства се определят и записват по време на транспортиране и маршрутизиране.</span><span class="sxs-lookup"><span data-stu-id="71b1f-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="71b1f-118">За по-нататъшно отстраняване на неизправности може да се наложи да проследите транспортната поддръжка за неизправностите в SPF, DKIM и.or DMARC.</span><span class="sxs-lookup"><span data-stu-id="71b1f-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>