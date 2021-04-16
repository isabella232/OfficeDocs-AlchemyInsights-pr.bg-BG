---
title: Шифроване с транспортни правила
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813857"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="fc035-102">Шифроване с транспортни правила</span><span class="sxs-lookup"><span data-stu-id="fc035-102">Encryption with transport rules</span></span>

<span data-ttu-id="fc035-103">В [център за администриране на Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), можете да използвате възможностите за шифроване на съобщения в Office (OME) в правилата за пощенския поток, за да задействате шифроването на съобщения.</span><span class="sxs-lookup"><span data-stu-id="fc035-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="fc035-104">Изберете опцията **Прилагане на шифроване на съобщения в Office 365 и защита на правата за достъп** към условието за правило за транспорт.</span><span class="sxs-lookup"><span data-stu-id="fc035-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="fc035-105">За повече информация вж. [Дефиниране на правилото за пощенския поток за шифроване](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="fc035-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="fc035-106">В PowerShell използвайте кратката команда [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) и настройте параметъра *ApplyOME* на $true.</span><span class="sxs-lookup"><span data-stu-id="fc035-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
