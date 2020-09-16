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
# <a name="unable-to-enable-unified-auditing"></a>Не можете да разрешите единни проверки

Когато се опитате да разрешите единно проверяване за вашата организация, е възможно да получите съобщение за грешка, подобно на следното:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

За да отстраните този проблем, изпълнете следните стъпки:

1. [Свързване към PowerShell на Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Изпълнете следната кратка команда:

   ```
   Enable-OrganizationCustomization
   ```

3. Изчакайте 60 минути, за да влезе в сила предишната настройка.

4. Изпълнете следната команда в PowerShell на Exchange Online:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

За допълнителна информация вижте следните статии:

- [Свързване с PowerShell на Exchange Online чрез многофакторно удостоверяване](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Включване или изключване на търсене в регистрационния файл за проверка](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
