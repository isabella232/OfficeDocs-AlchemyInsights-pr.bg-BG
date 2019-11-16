---
title: Outlook Desktop извикване или заместване на имейл съобщение
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/15/2019
ms.locfileid: "36496100"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="af191-102">Изтегляне или заместване на имейл съобщение на Outlook</span><span class="sxs-lookup"><span data-stu-id="af191-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="af191-103">Като администратор, можете да **Припомняме съобщения от името на потребителите, използващи PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="af191-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="af191-104">Не можете да си припомняме съобщения от центъра за администриране.</span><span class="sxs-lookup"><span data-stu-id="af191-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="af191-105">Можете да си **Припомняме само съобщения, които се изпращат на хора във вашата организация**.</span><span class="sxs-lookup"><span data-stu-id="af191-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="af191-106">Ако съобщението е изпратено до адрес в Gmail, например, не можете да го помните.</span><span class="sxs-lookup"><span data-stu-id="af191-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="af191-107">Можете да си **спомните само съобщенията, изпратени от Outlook 2016 на компютъра**.</span><span class="sxs-lookup"><span data-stu-id="af191-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="af191-108">Ако потребителят изпраща съобщение с помощта на Outlook за Mac или Outlook в мрежата, не можете да го помните.</span><span class="sxs-lookup"><span data-stu-id="af191-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="af191-109">За да върнете или замените имейл съобщение:</span><span class="sxs-lookup"><span data-stu-id="af191-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="af191-110">В прозореца на папките отляво на прозореца на Outlook изберете папката "изпратени".</span><span class="sxs-lookup"><span data-stu-id="af191-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="af191-111">Щракнете двукратно върху съобщението, което искате да си спомните, за да го отворите.</span><span class="sxs-lookup"><span data-stu-id="af191-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="af191-112">Изберете раздела **съобщение** , след което изберете **действия** > , които**изземат това съобщение**.</span><span class="sxs-lookup"><span data-stu-id="af191-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="af191-113">Изберете **Изтрий непрочетените копия на това съобщение** или **Изтрийте непрочетените копия и заменете с ново съобщение**, след което изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="af191-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="af191-114">Ако изпращате заместващо съобщение, Съставете съобщението, след което изберете **Изпращане**.</span><span class="sxs-lookup"><span data-stu-id="af191-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="af191-115">Успехът или Неуспехът на изтеглянето на съобщението зависи от настройките на получателя в Outlook.</span><span class="sxs-lookup"><span data-stu-id="af191-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="af191-116">За стъпки, за да проверите изтеглянето, вижте [тази статия](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="af191-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="af191-117">Търсене и изтриване на имейл съобщения във вашата организация</span><span class="sxs-lookup"><span data-stu-id="af191-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="af191-118">Ако не сте глобален администратор, профилът ви трябва да бъде добавен към ролята на мениджър за откриване на откриването на нови функции или управлението на търсенето на съответствие за търсене на съобщения.</span><span class="sxs-lookup"><span data-stu-id="af191-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="af191-119">За да изтриете съобщения, ще трябва да се присъедините към ролева група за управление на организацията или ролята за управление на търсенето и прочистване.</span><span class="sxs-lookup"><span data-stu-id="af191-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="af191-120">Разрешенията за тези роли се присвояват в [центъра за защита и съответствие](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="af191-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="af191-121">[Създаване на търсене на съдържание](https://docs.microsoft.com/office365/securitycompliance/content-search) , за да намерите съобщението за изтриване.</span><span class="sxs-lookup"><span data-stu-id="af191-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="af191-122">[Свързване към защита и съответствие център PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="af191-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="af191-123">Ако използвате многофакторно удостоверяване, вижте [Свързване към Office 365 защита и съответствие център PowerShell използване на многофакторно удостоверяване](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="af191-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>