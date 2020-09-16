---
title: Отстраняване на неизправности при събития от имейл
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658723"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="dbf0a-102">Отстраняване на неизправности при събития от имейл</span><span class="sxs-lookup"><span data-stu-id="dbf0a-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="dbf0a-103">Проверете дали тази функция е разрешена за пощенската кутия: **get <mailbox> -EventsFromEmailConfiguration-самоличност**</span><span class="sxs-lookup"><span data-stu-id="dbf0a-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="dbf0a-104">След това погледнете "събития от имейл" регистрационни файлове за **експортиране – MailboxDiagnosticLogs <mailbox> – Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="dbf0a-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="dbf0a-105">В регистрите "събития от имейл" Намерете свойството InternetMessageId, което съответства на елемента в пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="dbf0a-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="dbf0a-106">Свойството TrustScore определя дали елементът е добавен, или не.</span><span class="sxs-lookup"><span data-stu-id="dbf0a-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="dbf0a-107">Събития ще бъдат добавени само ако TrustScore = "доверен".</span><span class="sxs-lookup"><span data-stu-id="dbf0a-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="dbf0a-108">Свойството TrustScore се определя чрез SPF, DKIM или dMarc свойства, които са в заглавката на съобщението.</span><span class="sxs-lookup"><span data-stu-id="dbf0a-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="dbf0a-109">За да видите тези свойства:</span><span class="sxs-lookup"><span data-stu-id="dbf0a-109">To view these properties:</span></span>

<span data-ttu-id="dbf0a-110">**Настолна версия на Outlook**</span><span class="sxs-lookup"><span data-stu-id="dbf0a-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="dbf0a-111">Отваряне на елемента</span><span class="sxs-lookup"><span data-stu-id="dbf0a-111">Open the item</span></span>
- <span data-ttu-id="dbf0a-112">Свойства на > на файл – > интернет заглавки</span><span class="sxs-lookup"><span data-stu-id="dbf0a-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="dbf0a-113">или</span><span class="sxs-lookup"><span data-stu-id="dbf0a-113">or</span></span>

<span data-ttu-id="dbf0a-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="dbf0a-114">**MFCMapi**</span></span>

- <span data-ttu-id="dbf0a-115">Придвижете се до елемента в папката "Входящи"</span><span class="sxs-lookup"><span data-stu-id="dbf0a-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="dbf0a-116">Потърсете PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="dbf0a-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="dbf0a-117">Тези свойства се определят и записват по време на транспорта и маршрутизирането.</span><span class="sxs-lookup"><span data-stu-id="dbf0a-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="dbf0a-118">За по-нататъшно отстраняване на неизправности може да се наложи да се придържате към поддръжката на транспорта за неуспехите в SPF, DKIM и. or DMARC.</span><span class="sxs-lookup"><span data-stu-id="dbf0a-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>