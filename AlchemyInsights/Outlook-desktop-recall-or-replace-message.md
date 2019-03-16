---
title: Outlook работния плот оттегляне или заместване имейл съобщение
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: aad9f863bc9fd7d5522c480bd1a7d15f3a80ff4f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/15/2019
ms.locfileid: "30657033"
---
# <a name="recall-or-replace-an-email-message"></a><span data-ttu-id="66ffd-102">Върнете или замените имейл съобщение</span><span class="sxs-lookup"><span data-stu-id="66ffd-102">Recall or replace an email message</span></span>

- <span data-ttu-id="66ffd-103">Като администратор можете да **припомни съобщения от името на потребителите, използване на PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="66ffd-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="66ffd-104">Вие не може да си припомни съобщения от центъра за администрация на.</span><span class="sxs-lookup"><span data-stu-id="66ffd-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="66ffd-105">Можете **само припомни съобщения, които се изпращат до хората във вашата организация**.</span><span class="sxs-lookup"><span data-stu-id="66ffd-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="66ffd-106">Ако съобщението е изпратено до адрес в Gmail, например, не може да си спомняте.</span><span class="sxs-lookup"><span data-stu-id="66ffd-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="66ffd-107">Можете да **само припомни съобщения, изпратени от перспектива 2016 на Компютъра**.</span><span class="sxs-lookup"><span data-stu-id="66ffd-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="66ffd-108">Ако даден потребител изпрати съобщение, като използвате Outlook за Mac или Outlook в мрежата, не може да си спомняте.</span><span class="sxs-lookup"><span data-stu-id="66ffd-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="66ffd-109">За да върнете или замените имейл съобщение:</span><span class="sxs-lookup"><span data-stu-id="66ffd-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="66ffd-110">В екрана с папки вляво на прозореца на Outlook изберете папката "изпратени".</span><span class="sxs-lookup"><span data-stu-id="66ffd-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="66ffd-111">Щракнете двукратно върху съобщението, което искате да оттеглите да го отворите.</span><span class="sxs-lookup"><span data-stu-id="66ffd-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="66ffd-112">Изберете раздела **съобщение** и след това изберете **действия** > **Оттегляне на съобщението**.</span><span class="sxs-lookup"><span data-stu-id="66ffd-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="66ffd-113">Изберете **изтрият непрочетените копия на това съобщение** или **изтриват непрочетените копия и се заместват с ново съобщение**и след това изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="66ffd-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="66ffd-114">Ако изпращате съобщение за подмяна, съставяне на съобщение и изберете **Изпрати**.</span><span class="sxs-lookup"><span data-stu-id="66ffd-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="66ffd-115">За успеха или неуспеха на съобщение оттеглянето зависи от настройките на получателя в Outlook.</span><span class="sxs-lookup"><span data-stu-id="66ffd-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="66ffd-116">Стъпки за проверка на отзовавам, вижте [тази статия](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="66ffd-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="66ffd-117">Търсене и изтриване на имейл съобщения във вашата организация</span><span class="sxs-lookup"><span data-stu-id="66ffd-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="66ffd-118">Ако не сте един глобален администратор, вашата сметка трябва да се добавят към ролята на мениджър на eDiscovery или съответствието търсене управленска роля за търсене на съобщения.</span><span class="sxs-lookup"><span data-stu-id="66ffd-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="66ffd-119">За да изтриете съобщения, трябва да се присъединят към ролевата група на управление на организацията или търсене и чистка управленска роля.</span><span class="sxs-lookup"><span data-stu-id="66ffd-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="66ffd-120">Разрешения за тези роли се присвояват в [центъра за защита и съответствие](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="66ffd-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="66ffd-121">[Създаване на съдържание за търсене](https://docs.microsoft.com/office365/securitycompliance/content-search) да намерите съобщението за изтриване.</span><span class="sxs-lookup"><span data-stu-id="66ffd-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="66ffd-122">[Свързване към сигурността и съответствието център PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="66ffd-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="66ffd-123">Ако използвате удостоверяване, вижте [Свързване към Office 365 защита и съответствие център PowerShell използва удостоверяване](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="66ffd-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>