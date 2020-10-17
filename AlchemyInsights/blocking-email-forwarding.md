---
title: 726, който блокира препращането на имейли
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478335"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="1b085-102">Блокиране или разблокиране на препращане на имейли</span><span class="sxs-lookup"><span data-stu-id="1b085-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="1b085-103">За да разрешите или забраните препращането на имейли за конкретна пощенска кутия, вижте [Конфигуриране на препращане на имейл](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="1b085-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="1b085-104">На ниво клиент контролата за външно препращане се осъществява чрез правилата за изходящи спам.</span><span class="sxs-lookup"><span data-stu-id="1b085-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="1b085-105">Можете да проверите правилата за изходящия филтър за нежелана поща от центъра за защита и съответствие [тук](https://protection.office.com/antispam) или с помощта на [командата get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="1b085-105">You can check the outbound spam filter policy from Security and Compliance Center [here](https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="1b085-106">Ако получавате следното съобщение за грешка: **"550 5.7.520 отказан достъп, вашата организация не разрешава външно препращане"**, моля, уверете се, че правилата са конфигурирани за разрешаване на външни автоматични препращания.</span><span class="sxs-lookup"><span data-stu-id="1b085-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="1b085-107">**Забележка:** Препоръчително е да запазите неактивираните външни автоматично препращане на правилата за изходящите филтри за нежелана поща и да я разрешите само за потребителите, които се нуждаят от външно препращане, като създадат правила по избор за тези потребители.</span><span class="sxs-lookup"><span data-stu-id="1b085-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="1b085-108">Можете да прочетете повече за [конфигурирането на външно препращане на имейли в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="1b085-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>