---
title: Настолната версия на Outlook се отзовава или заменя имейл съобщение
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663979"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="15655-102">Оттегляне или заместване на имейл съобщение на Outlook</span><span class="sxs-lookup"><span data-stu-id="15655-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="15655-103">Като администратор можете да **оттегляте съобщения от името на потребители с помощта на PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="15655-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="15655-104">Не можете да оттегляте съобщения от центъра за администриране.</span><span class="sxs-lookup"><span data-stu-id="15655-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="15655-105">Можете да **изтегляте само съобщенията, които са изпратени до хора във вашата организация**.</span><span class="sxs-lookup"><span data-stu-id="15655-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="15655-106">Ако съобщението е изпратено до адрес в Gmail, например не можете да го припомните.</span><span class="sxs-lookup"><span data-stu-id="15655-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="15655-107">Можете да **оттегляте съобщения, изпратени от Outlook 2016 на компютъра**.</span><span class="sxs-lookup"><span data-stu-id="15655-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="15655-108">Ако потребител изпрати съобщение с помощта на Outlook for Mac или Outlook в уеб, не можете да го припомните.</span><span class="sxs-lookup"><span data-stu-id="15655-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="15655-109">За да оттеглите или заместите имейл съобщение:</span><span class="sxs-lookup"><span data-stu-id="15655-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="15655-110">В екрана с папки отляво на прозореца на Outlook изберете папката изпратени.</span><span class="sxs-lookup"><span data-stu-id="15655-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="15655-111">Щракнете двукратно върху съобщението, което искате да припомните, за да го отворите.</span><span class="sxs-lookup"><span data-stu-id="15655-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="15655-112">Изберете раздела **съобщение** и след това изберете **действия**  >  **оттегляне на това съобщение**.</span><span class="sxs-lookup"><span data-stu-id="15655-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="15655-113">Изберете **Изтрий непрочетените копия на това съобщение** или **Изтрийте непрочетените копия и го заместете с ново съобщение**и след това изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="15655-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="15655-114">Ако изпращате заместващо съобщение, Съставете съобщението и след това изберете **Изпрати**.</span><span class="sxs-lookup"><span data-stu-id="15655-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="15655-115">Успеха или неуспеха на оттегляне на съобщение зависи от настройките на получателя в Outlook.</span><span class="sxs-lookup"><span data-stu-id="15655-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="15655-116">За стъпки за проверка на оттеглянето вижте [тази статия](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="15655-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="15655-117">Търсене и изтриване на имейл съобщения във вашата организация</span><span class="sxs-lookup"><span data-stu-id="15655-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="15655-118">Ако не сте глобален администратор, Вашият акаунт трябва да бъде добавен към ролята на диспечера за откриване на електронни данни или към управлението за управление на съответствието при търсене на съобщения.</span><span class="sxs-lookup"><span data-stu-id="15655-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="15655-119">За да изтриете съобщения, ще трябва да се присъедините към ролевата група за управление на организацията или към ролята за управление на търсенето и изчистването.</span><span class="sxs-lookup"><span data-stu-id="15655-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="15655-120">Разрешенията за тези роли се присвояват в [центъра за защита и съответствие](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="15655-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="15655-121">[Създаване на търсене на съдържание](https://docs.microsoft.com/microsoft-365/compliance/content-search) , за да се намери съобщението за изтриване.</span><span class="sxs-lookup"><span data-stu-id="15655-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="15655-122">[Свързване към центъра за сигурност и съответствие на PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="15655-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="15655-123">Ако използвате многофакторно удостоверяване, вижте [Свързване към центъра за сигурност и съответствие на Microsoft 365, като използвате многофакторно удостоверяване](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="15655-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>