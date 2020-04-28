---
title: Шифроване с транспортни правила
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915019"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="7586b-102">Шифроване с транспортни правила</span><span class="sxs-lookup"><span data-stu-id="7586b-102">Encryption with transport rules</span></span>

<span data-ttu-id="7586b-103">В [център за администриране на Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), можете да използвате възможностите за шифроване на съобщения в Office (OME) в правилата за пощенския поток, за да задействате шифроването на съобщения.</span><span class="sxs-lookup"><span data-stu-id="7586b-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="7586b-104">Изберете опцията **Прилагане на шифроване на съобщения в Office 365 и защита на правата за достъп** към условието за правило за транспорт.</span><span class="sxs-lookup"><span data-stu-id="7586b-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="7586b-105">За повече информация вж. [Дефиниране на правилото за пощенския поток за шифроване](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="7586b-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="7586b-106">В PowerShell използвайте кратката команда [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) и настройте параметъра *ApplyOME* на $true.</span><span class="sxs-lookup"><span data-stu-id="7586b-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
