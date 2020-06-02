---
title: 2419-не е възможно одитиране
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510417"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="695c0-102">Не може да се разреши унифицирана проверка</span><span class="sxs-lookup"><span data-stu-id="695c0-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="695c0-103">Когато се опитате да разрешите унифицирана проверка за вашата организация, можете да получите грешка подобно на следното:</span><span class="sxs-lookup"><span data-stu-id="695c0-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="695c0-104">За да разрешите този проблем, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="695c0-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="695c0-105">[Свързване към Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="695c0-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="695c0-106">Изпълнете следната команда:</span><span class="sxs-lookup"><span data-stu-id="695c0-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="695c0-107">Изчакайте 60 минути, за да влязат в сила предишната настройка.</span><span class="sxs-lookup"><span data-stu-id="695c0-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="695c0-108">Изпълнете следната команда в Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="695c0-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="695c0-109">За допълнителна информация вижте следните статии:</span><span class="sxs-lookup"><span data-stu-id="695c0-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="695c0-110">Свързване към Exchange Online PowerShell чрез удостоверяване</span><span class="sxs-lookup"><span data-stu-id="695c0-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="695c0-111">Включване или изключване на търсенето на регистрационен файл за проверка</span><span class="sxs-lookup"><span data-stu-id="695c0-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
