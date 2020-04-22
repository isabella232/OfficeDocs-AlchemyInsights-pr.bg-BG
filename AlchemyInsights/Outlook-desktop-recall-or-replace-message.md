---
title: Outlook Desktop извикване или заместване на имейл съобщение
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687499"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="f0990-102">Извикване или заместване на имейл съобщение в Outlook</span><span class="sxs-lookup"><span data-stu-id="f0990-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="f0990-103">Като администратор можете да **си спомните съобщения от името на потребителите, използващи PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="f0990-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="f0990-104">Не можете да си спомните съобщения от центъра за администриране.</span><span class="sxs-lookup"><span data-stu-id="f0990-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="f0990-105">Можете да **си спомните само съобщения, които се изпращат до хора във вашата организация**.</span><span class="sxs-lookup"><span data-stu-id="f0990-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="f0990-106">Ако например съобщението е изпратено на адрес в Gmail, не можете да го върнете.</span><span class="sxs-lookup"><span data-stu-id="f0990-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="f0990-107">Можете да **си спомните съобщения, изпратени от Outlook 2016 на компютъра**.</span><span class="sxs-lookup"><span data-stu-id="f0990-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="f0990-108">Ако потребителят изпраща съобщение с помощта на Outlook за Mac или Outlook в уеб, не можете да го спомните.</span><span class="sxs-lookup"><span data-stu-id="f0990-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="f0990-109">За да извикате или замените имейл съобщение:</span><span class="sxs-lookup"><span data-stu-id="f0990-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="f0990-110">В прозореца на папката вляво на прозореца на Outlook изберете папката Изпратени.</span><span class="sxs-lookup"><span data-stu-id="f0990-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="f0990-111">Щракнете двукратно върху съобщението, което искате да се върнете, за да го отворите.</span><span class="sxs-lookup"><span data-stu-id="f0990-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="f0990-112">Изберете раздела **Съобщение** и след това изберете **Действия** > **Запаметете това съобщение**.</span><span class="sxs-lookup"><span data-stu-id="f0990-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="f0990-113">Изберете **Изтриване на непрочетени копия на това съобщение** или Изтриване на **непрочетени копия и заменете с ново съобщение**, след което изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="f0990-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="f0990-114">Ако изпращате заместващо съобщение, съставете съобщението, след което изберете **Изпрати**.</span><span class="sxs-lookup"><span data-stu-id="f0990-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="f0990-115">Успехът или отказът на съобщението за извикване зависи от настройките на получателя в Outlook.</span><span class="sxs-lookup"><span data-stu-id="f0990-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="f0990-116">За стъпки, за да проверите оттеглянето вижте [тази статия](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="f0990-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="f0990-117">Търсене и изтриване на имейл съобщения във вашата организация</span><span class="sxs-lookup"><span data-stu-id="f0990-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="f0990-118">Ако не сте глобален администратор, вашият акаунт трябва да бъде добавен към ролята на мениджъра на eDiscovery или към ролята за управление на съответствието за търсене на съобщения.</span><span class="sxs-lookup"><span data-stu-id="f0990-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="f0990-119">За да изтриете съобщения, трябва да се присъедините към групата роля управление на организацията или ролята за управление на търсенето и изтриването.</span><span class="sxs-lookup"><span data-stu-id="f0990-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="f0990-120">Разрешенията за тези роли се присвояват в [центъра за защита и съответствие](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="f0990-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="f0990-121">[Създайте търсене на съдържание,](https://docs.microsoft.com/office365/securitycompliance/content-search) за да намерите съобщението за изтриване.</span><span class="sxs-lookup"><span data-stu-id="f0990-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="f0990-122">[Свързване със центъра за сигурност и съответствие PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="f0990-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="f0990-123">Ако използвате удостоверяване с много фактор, вижте [Свързване към Microsoft 365 защита и център за съответствие PowerShell с помощта на удостоверяване с много фактор](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="f0990-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>