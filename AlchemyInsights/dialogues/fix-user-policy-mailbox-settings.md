---
title: Коригиране на настройките на потребителските правила/пощенските кутии
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692830"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="8960f-102">Коригиране на настройките на потребителските правила/пощенските кутии</span><span class="sxs-lookup"><span data-stu-id="8960f-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="8960f-103">Настройките за нежелана поща в пощенската кутия са засегнали това съобщение.</span><span class="sxs-lookup"><span data-stu-id="8960f-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="8960f-104">За да прегледате настройките, направете следното:</span><span class="sxs-lookup"><span data-stu-id="8960f-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="8960f-105">Стартиране на обвивката за управление на Exchange.</span><span class="sxs-lookup"><span data-stu-id="8960f-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="8960f-106">За повече информация вижте [Отваряне на обвивката за управление на Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="8960f-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="8960f-107">Изпълнете тази команда (като използвате имейл адреса на потребителя):  **get-mailboxjunkmailconfiguration-самоличност "User@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="8960f-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="8960f-108">Проверете дали имейл адресът на подателя е част от **TrustedSendersAndDomains** , или **BlockedSendersAndDomains**.</span><span class="sxs-lookup"><span data-stu-id="8960f-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="8960f-109">Ако имейл адресът е в един от списъците, може да се наложи да го премахнете.</span><span class="sxs-lookup"><span data-stu-id="8960f-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="8960f-110">За да научите повече, вижте [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="8960f-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
