---
title: Преместване на имейл съобщения в архивната пощенска кутия
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522760"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="cebf3-102">Преместване на имейл в архивната пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="cebf3-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="cebf3-103">Ако искате да стартираме автоматизирани проверки за настройките, посочени по-долу, изберете бутона за връщане <-- в горната част на тази страница, и след това въведете имейл адреса на потребителя, който има проблеми при преместването на имейл в архивната пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="cebf3-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="cebf3-104">Потвърдете, че **архивна пощенска кутия** е разрешена.</span><span class="sxs-lookup"><span data-stu-id="cebf3-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="cebf3-105">Ако не, използвайте стъпките в [тази статия,](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) за да разрешите архивна пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="cebf3-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="cebf3-106">За да архивирате съобщенията автоматично в архивната пощенска кутия, трябва да бъде зададен маркер за задържане с действието **Преместване в архива,** който се **прилага автоматично към етикета на цялата пощенска кутия (по подразбиране)**.</span><span class="sxs-lookup"><span data-stu-id="cebf3-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="cebf3-107">Използвайте стъпките тук, за да създадете етикета: [Архив подразбиращ се етикет](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="cebf3-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="cebf3-108">След това добавете етикета **"Архив"** към правилата си за задържане.</span><span class="sxs-lookup"><span data-stu-id="cebf3-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="cebf3-109">В центъра за администриране на Exchange изберете **Правила за задържане** > добавите **етикета Премести в архива** към правилата > **Записване**.</span><span class="sxs-lookup"><span data-stu-id="cebf3-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="cebf3-110">Сега [присвоите правило](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) за съхранение на пощенска кутия на конкретен потребител.</span><span class="sxs-lookup"><span data-stu-id="cebf3-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="cebf3-111">Същите правила ще се прилагат към **първична** и **архивна** пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="cebf3-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="cebf3-112">Може да се наложи да накарате помощника за управлявани папки (МРН) да стартирате и приложите новите настройки на пощенската кутия на потребителя.</span><span class="sxs-lookup"><span data-stu-id="cebf3-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="cebf3-113">Изпълнете следната команда, докато [е свързан към EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) да стартирате помощника за управлявани папки за конкретна пощенска кутия:</span><span class="sxs-lookup"><span data-stu-id="cebf3-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="cebf3-114">Начален управляемпаксовразставник -идентичност<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="cebf3-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="cebf3-115">За повече информация относно настройването на правила за архивиране вижте [Настройване на правила за архивиране и изтриване на пощенски кутии](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="cebf3-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  