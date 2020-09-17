---
title: Местене на имейл съобщения в архивната пощенска кутия
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799769"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="9cce4-102">Преминаване на имейл в пощенската кутия за архивиране</span><span class="sxs-lookup"><span data-stu-id="9cce4-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="9cce4-103">Ако искате да изпълняваме автоматизирани проверки за настройките, упоменати по-долу, изберете бутона "назад" < – в горния край на тази страница и след това въведете имейл адреса на потребителя, който има проблеми при преместване на имейла в своята архивна пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="9cce4-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="9cce4-104">Проверете дали е разрешена **пощенска кутия за архивиране** .</span><span class="sxs-lookup"><span data-stu-id="9cce4-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="9cce4-105">Ако не, използвайте стъпките в [тази статия](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) , за да разрешите архивната пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="9cce4-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="9cce4-106">За да архивирате съобщения автоматично в архивната пощенска кутия, трябва да се настрои етикет за съхранение с действието **за преминаване към архивиране** , за да се **Приложи автоматично към етикета на цялата пощенска кутия (по подразбиране)**.</span><span class="sxs-lookup"><span data-stu-id="9cce4-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="9cce4-107">Използвайте стъпките тук, за да създадете етикет: [Архивирай етикета по подразбиране](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="9cce4-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="9cce4-108">След това добавете етикета за **архивиране** към правилата за съхранение.</span><span class="sxs-lookup"><span data-stu-id="9cce4-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="9cce4-109">В центъра за администриране на Exchange изберете **правила за съхранение** > Добавете **етикета преминаване към архивиране** към правилата > **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="9cce4-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="9cce4-110">Сега [Задайте правилата за съхранение](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) за конкретната пощенска кутия на потребителя.</span><span class="sxs-lookup"><span data-stu-id="9cce4-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="9cce4-111">Същите правила ще бъдат прилагани както за **първичната** , така и за **архивната** пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="9cce4-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="9cce4-112">Може да се наложи да принудите помощника за управление на папки (МВНР) да изпълнява и да прилага новите настройки към пощенската кутия на потребителя.</span><span class="sxs-lookup"><span data-stu-id="9cce4-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="9cce4-113">Изпълнете следната команда, докато [сте свързани към ЕКСО PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , за да стартирате помощника за управление на папки за конкретна пощенска кутия:</span><span class="sxs-lookup"><span data-stu-id="9cce4-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="9cce4-114">Start-ManagedFolderAssistant-самоличност <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="9cce4-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="9cce4-115">За повече информация относно настройването на правила за архивиране вижте [Настройване на правила за архивиране и изтриване за пощенски кутии](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="9cce4-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  