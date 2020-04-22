---
title: Преместване на имейл съобщения в архивнапощенска кутия
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
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713635"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="9cfc1-102">Преместване на имейл а в архивната пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="9cfc1-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="9cfc1-103">Уверете се, че **архивнапощенска кутия** е разрешена.</span><span class="sxs-lookup"><span data-stu-id="9cfc1-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="9cfc1-104">Ако не, използвайте стъпките в [тази статия,](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) за да разрешите архивна пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="9cfc1-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="9cfc1-105">За да архивирате автоматично съобщения тава архивната пощенска кутия, етикет за задържане с **действие "Преместване в архив"** трябва да бъде зададен на **автоматично приложение към цялата пощенска кутия (по подразбиране) етикет**.</span><span class="sxs-lookup"><span data-stu-id="9cfc1-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="9cfc1-106">Използвайте стъпките тук, за да създадете маркера: [Архив по подразбиране таг](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="9cfc1-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="9cfc1-107">След това добавете **етикета "Архив"** към правилата за задържане.</span><span class="sxs-lookup"><span data-stu-id="9cfc1-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="9cfc1-108">В центъра за администриране на Exchange изберете **Правила за задържане** > добавите етикет **"Преместване в архив"** към правилата > **Записване**.</span><span class="sxs-lookup"><span data-stu-id="9cfc1-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="9cfc1-109">Сега [присвоите правило](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) за пощенска кутия на конкретен потребител.</span><span class="sxs-lookup"><span data-stu-id="9cfc1-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="9cfc1-110">Същата политика ще се прилагат за **основните** и **архивната** пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="9cfc1-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="9cfc1-111">Може да е необходимо да накарате помощника управлявани папки (МВНР) да изпълни и приложи новите настройки на пощенската кутия на потребителя.</span><span class="sxs-lookup"><span data-stu-id="9cfc1-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="9cfc1-112">Изпълнете следната команда, докато [е свързан към EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) да стартирате помощника за управлявани папки за конкретна пощенска кутия:</span><span class="sxs-lookup"><span data-stu-id="9cfc1-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="9cfc1-113">Асистент за начало на управлявани папки -самоличност<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="9cfc1-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="9cfc1-114">За повече информация относно настройването на правила за архивиране вижте [Настройване на правила за архивиране и изтриване на пощенски кутии](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="9cfc1-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  