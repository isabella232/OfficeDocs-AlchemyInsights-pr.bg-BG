---
title: 2419-не може да разрешаване одит
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065601"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="7b7d5-102">Не може да разрешите унифицирана проверка</span><span class="sxs-lookup"><span data-stu-id="7b7d5-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="7b7d5-103">Когато се опитате да разрешите унифицирана проверяването за вашата организация от Office 365, можете да получите грешка подобен следното:</span><span class="sxs-lookup"><span data-stu-id="7b7d5-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="7b7d5-104">За да разрешите този проблем, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="7b7d5-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="7b7d5-105">[Свързване към обмен на онлайн Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="7b7d5-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="7b7d5-106">Изпълнете следната команда:</span><span class="sxs-lookup"><span data-stu-id="7b7d5-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="7b7d5-107">Изчакайте 60 минути за предишната настройка да влязат в сила.</span><span class="sxs-lookup"><span data-stu-id="7b7d5-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="7b7d5-108">Изпълнете следната команда в Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="7b7d5-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="7b7d5-109">За допълнителна информация вижте следните статии:</span><span class="sxs-lookup"><span data-stu-id="7b7d5-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="7b7d5-110">Свързване към Exchange Online PowerShell чрез удостоверяване</span><span class="sxs-lookup"><span data-stu-id="7b7d5-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="7b7d5-111">Включване или изключване на Office 365 одит регистрационния файл търсене</span><span class="sxs-lookup"><span data-stu-id="7b7d5-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
