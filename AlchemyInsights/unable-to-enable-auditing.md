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
# <a name="unable-to-enable-unified-auditing"></a>Не може да разрешите унифицирана проверка

Когато се опитате да разрешите унифицирана проверяването за вашата организация от Office 365, можете да получите грешка подобен следното:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

За да разрешите този проблем, изпълнете следните стъпки:

1. [Свързване към обмен на онлайн Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Изпълнете следната команда:

   ```
   Enable-OrganizationCustomization
   ```

3. Изчакайте 60 минути за предишната настройка да влязат в сила.

4. Изпълнете следната команда в Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

За допълнителна информация вижте следните статии:

- [Свързване към Exchange Online PowerShell чрез удостоверяване](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Включване или изключване на Office 365 одит регистрационния файл търсене](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
