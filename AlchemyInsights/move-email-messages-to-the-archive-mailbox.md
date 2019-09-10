---
title: Преместване на имейл съобщения в архивна пощенска кутия
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822151"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="907ed-102">Преместване на имейл в архивна пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="907ed-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="907ed-103">Потвърдете, че е разрешена **архивна пощенска кутия** .</span><span class="sxs-lookup"><span data-stu-id="907ed-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="907ed-104">Ако не, използвайте стъпките в [тази статия](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , за да разрешите архивна пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="907ed-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="907ed-105">За архивиране на съобщения автоматично в архивна пощенска кутия, маркер за задържане с **Преместване за архивиране** на действие трябва да бъде настроен да се **прилага автоматично към цялата пощенска кутия (по подразбиране) етикет**.</span><span class="sxs-lookup"><span data-stu-id="907ed-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="907ed-106">Използвайте стъпките тук, за да създадете маркера: [архивен маркер по подразбиране](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="907ed-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="907ed-107">След това добавете **Архивният** маркер към правилата си за задържане.</span><span class="sxs-lookup"><span data-stu-id="907ed-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="907ed-108">В центъра за администриране на Exchange изберете **правила за задържане** > Добавяне на **етикет за преместване на архив** на правилата > **Save**.</span><span class="sxs-lookup"><span data-stu-id="907ed-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="907ed-109">Сега [присвоите правила за задържане](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) на пощенската кутия на конкретния потребител.</span><span class="sxs-lookup"><span data-stu-id="907ed-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="907ed-110">Същата политика ще се прилага към **първичната** и **архивната** пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="907ed-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="907ed-111">Може да се наложи да принудите помощника за управлявана папка (МФП) да изпълнява и прилага новите настройки към пощенската кутия на потребителя.</span><span class="sxs-lookup"><span data-stu-id="907ed-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="907ed-112">Изпълнете следната команда, докато е [свързан към екзо PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) да стартирате помощника за управлявани папки за конкретна пощенска кутия:</span><span class="sxs-lookup"><span data-stu-id="907ed-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="907ed-113">Стартов помощник – самоличност<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="907ed-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="907ed-114">За повече информация относно настройването на правила за архивиране вижте [Настройване на правила за архивиране и изтриване на пощенски кутии](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="907ed-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  