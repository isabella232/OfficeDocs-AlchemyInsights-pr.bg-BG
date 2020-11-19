---
title: Оттегляне или заместване на имейл съобщение
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353495"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="b90be-102">Оттегляне или заместване на имейл съобщение в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b90be-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="b90be-103">Можете да **изтегляте само съобщенията, които са изпратени до хора във вашата организация**.</span><span class="sxs-lookup"><span data-stu-id="b90be-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="b90be-104">Например, ако съобщението е изпратено до адрес в Gmail, не можете да го припомните.</span><span class="sxs-lookup"><span data-stu-id="b90be-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="b90be-105">Можете да **изтегляте само съобщения, изпратени от Outlook за PC**.</span><span class="sxs-lookup"><span data-stu-id="b90be-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="b90be-106">Ако потребител изпрати съобщение с помощта на Outlook for Mac или Outlook в уеб, не можете да го припомните.</span><span class="sxs-lookup"><span data-stu-id="b90be-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="b90be-107">Като администратор на клиент, можете да **изтегляте съобщения от името на потребителите, като използвате PowerShell** (за повече информация вижте: [търсене и изтриване на имейл съобщения](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="b90be-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="b90be-108">Не можете да оттегляте съобщения от центъра за администриране.</span><span class="sxs-lookup"><span data-stu-id="b90be-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="b90be-109">Превъртете надолу до "търсене и изтриване на имейл съобщения във вашата организация" за повече информация.</span><span class="sxs-lookup"><span data-stu-id="b90be-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="b90be-110">**Оттегляне или заместване на имейл съобщение, което сте изпратили**</span><span class="sxs-lookup"><span data-stu-id="b90be-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="b90be-111">В екрана с папки отляво на прозореца на Outlook изберете папката изпратени.</span><span class="sxs-lookup"><span data-stu-id="b90be-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="b90be-112">Отворете съобщението, което искате да припомните.</span><span class="sxs-lookup"><span data-stu-id="b90be-112">Open the message that you want to recall.</span></span> <span data-ttu-id="b90be-113">Трябва да щракнете двукратно, за да отворите съобщението.</span><span class="sxs-lookup"><span data-stu-id="b90be-113">You must double-click to open the message.</span></span> <span data-ttu-id="b90be-114">Избирането на съобщението така, че да се появява в екрана за четене, не ви позволява да си припомните съобщението.</span><span class="sxs-lookup"><span data-stu-id="b90be-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="b90be-115">От раздела съобщение изберете **действия**  >  **оттегляне на това съобщение**.</span><span class="sxs-lookup"><span data-stu-id="b90be-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="b90be-116">Изберете **Изтрий непрочетените копия на това съобщение** или **Изтрийте непрочетените копия и го заместете с ново съобщение и** след това изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="b90be-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="b90be-117">Ако изпращате заместващо съобщение, Съставете съобщението, след което изберете **Изпрати**.</span><span class="sxs-lookup"><span data-stu-id="b90be-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="b90be-118">Успеха или неуспеха на оттегляне на съобщение зависи от настройките на получателите в Outlook.</span><span class="sxs-lookup"><span data-stu-id="b90be-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="b90be-119">За повече информация, включително как да проверите оттеглянето, вижте [оттегляне или заместване на имейл съобщение, което сте изпратили](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="b90be-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="b90be-120">**_За да потърсите и изтриете имейл съобщения във вашата организация_**, е най-лесно, ако сте глобален администратор. Ако не сте глобален администратор, Вашият акаунт трябва да бъде добавен към ролевата група на диспечера за откриване на електронни данни или към ролята за управление на търсенето за съответствие.</span><span class="sxs-lookup"><span data-stu-id="b90be-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="b90be-121">За да изтриете съобщения, ще трябва да се присъедините към ролевата група за управление на организацията или към ролята за управление на търсенето и изчистването.</span><span class="sxs-lookup"><span data-stu-id="b90be-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="b90be-122">Разрешенията за тези роли се присвояват в [центъра за съответствие на & за защита](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="b90be-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="b90be-123">[Създаване на търсене на съдържание](https://docs.microsoft.com/microsoft-365/compliance/content-search) , за да се намери съобщението за изтриване.</span><span class="sxs-lookup"><span data-stu-id="b90be-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="b90be-124">[Свързване към центъра за администриране на & на съвместимост на PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="b90be-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="b90be-125">Ако използвате МВНР (многофакторно удостоверяване), вижте [Свързване с Microsoft 365 Security & център за съответствие PowerShell чрез многофакторно удостоверяване](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="b90be-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
