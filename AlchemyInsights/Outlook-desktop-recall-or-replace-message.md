---
title: Изтегляне на Outlook десктоп или заместване на имейл съобщение
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502308"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="7f45e-102">Оттегляне или замяна на имейл съобщение от Outlook</span><span class="sxs-lookup"><span data-stu-id="7f45e-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="7f45e-103">Като администратор, можете да **припомните съобщения от името на потребителите, които използват PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="7f45e-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="7f45e-104">Не можете да си спомните съобщения от центъра за администриране.</span><span class="sxs-lookup"><span data-stu-id="7f45e-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="7f45e-105">Можете да **си спомните само съобщения, които са изпратени на хора във вашата организация**.</span><span class="sxs-lookup"><span data-stu-id="7f45e-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="7f45e-106">Ако съобщението е изпратено до адрес в Gmail например, не можете да го върнете.</span><span class="sxs-lookup"><span data-stu-id="7f45e-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="7f45e-107">Можете да **си спомните само съобщенията, изпратени от Outlook 2016 на компютъра.**</span><span class="sxs-lookup"><span data-stu-id="7f45e-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="7f45e-108">Ако потребителят изпраща съобщение с помощта на Outlook за Mac или Outlook в мрежата, не можете да го си спомните.</span><span class="sxs-lookup"><span data-stu-id="7f45e-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="7f45e-109">За да си спомните или замените имейл съобщение:</span><span class="sxs-lookup"><span data-stu-id="7f45e-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="7f45e-110">В прозореца на папката вляво от прозореца на Outlook изберете папката "Изпратени".</span><span class="sxs-lookup"><span data-stu-id="7f45e-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="7f45e-111">Щракнете двукратно върху съобщението, което искате да си припомните, за да го отворите.</span><span class="sxs-lookup"><span data-stu-id="7f45e-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="7f45e-112">Изберете раздела **съобщение** и след това изберете **Действия**  >  **Си припомняне на това съобщение**.</span><span class="sxs-lookup"><span data-stu-id="7f45e-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="7f45e-113">Изберете **Изтриване на непрочетени копия на това съобщение** или Изтриване на **непрочетени копия и замяна с ново съобщение**, след което изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="7f45e-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="7f45e-114">Ако изпращате съобщение за замяна, съставете съобщението и след това изберете **Изпращане**.</span><span class="sxs-lookup"><span data-stu-id="7f45e-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="7f45e-115">Успехът или неуспехът на извикване на съобщение зависи от настройките на получателя в Outlook.</span><span class="sxs-lookup"><span data-stu-id="7f45e-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="7f45e-116">За стъпки, за да проверите изземването, вижте [тази статия](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="7f45e-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="7f45e-117">Търсене и изтриване на имейл съобщения във вашата организация</span><span class="sxs-lookup"><span data-stu-id="7f45e-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="7f45e-118">Ако не сте глобален администратор, профилът ви трябва да бъде добавен към ролята на мениджъра на електронни данни или ролята за управление на търсенето на съответствие, за да търсите съобщения.</span><span class="sxs-lookup"><span data-stu-id="7f45e-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="7f45e-119">За да изтриете съобщения, трябва да се присъедините към групата роля "Управление на организацията" или към ролята за управление на търсене и изтриване.</span><span class="sxs-lookup"><span data-stu-id="7f45e-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="7f45e-120">Разрешенията за тези роли се присвояват в [центъра за защита и съответствие](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="7f45e-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="7f45e-121">[Създайте търсене на съдържание,](https://docs.microsoft.com/microsoft-365/compliance/content-search) за да намерите съобщението за изтриване.</span><span class="sxs-lookup"><span data-stu-id="7f45e-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="7f45e-122">[Свързване към центъра за защита и съответствие PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="7f45e-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="7f45e-123">Ако използвате удостоверяване, вижте Свързване [към Microsoft 365 защита и Център за съответствие PowerShell с помощта на удостоверяване](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="7f45e-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>