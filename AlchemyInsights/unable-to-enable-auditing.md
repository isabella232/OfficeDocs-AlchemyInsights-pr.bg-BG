---
title: 2419 – неспособен за разрешаване – проверка
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767588"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="33e17-102">Не можете да разрешите единни проверки</span><span class="sxs-lookup"><span data-stu-id="33e17-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="33e17-103">Когато се опитате да разрешите единно проверяване за вашата организация, е възможно да получите съобщение за грешка, подобно на следното:</span><span class="sxs-lookup"><span data-stu-id="33e17-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="33e17-104">За да отстраните този проблем, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="33e17-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="33e17-105">[Свързване към PowerShell на Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="33e17-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="33e17-106">Изпълнете следната кратка команда:</span><span class="sxs-lookup"><span data-stu-id="33e17-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="33e17-107">Изчакайте 60 минути, за да влезе в сила предишната настройка.</span><span class="sxs-lookup"><span data-stu-id="33e17-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="33e17-108">Изпълнете следната команда в PowerShell на Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="33e17-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="33e17-109">За допълнителна информация вижте следните статии:</span><span class="sxs-lookup"><span data-stu-id="33e17-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="33e17-110">Свързване с PowerShell на Exchange Online чрез многофакторно удостоверяване</span><span class="sxs-lookup"><span data-stu-id="33e17-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="33e17-111">Включване или изключване на търсене в регистрационния файл за проверка</span><span class="sxs-lookup"><span data-stu-id="33e17-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
