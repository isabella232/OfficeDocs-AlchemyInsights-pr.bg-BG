---
title: 2419-unable-to-enable-auditing
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
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007779"
---
# <a name="unable-to-enable-unified-auditing"></a>Не може да се разреши единно проверяване

Когато се опитате да разрешите единно проверяване за вашата организация, може да получите грешка, подобна на следната:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

За да разрешите този проблем, изпълнете следните стъпки:

1. [Свързване към Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Изпълнете следната кратка команда:

   ```
   Enable-OrganizationCustomization
   ```

3. Изчакайте 60 минути, за да в сила предишната настройка.

4. Изпълнете следната команда в Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

За допълнителна информация вижте следните статии:

- [Свързване да Exchange Online PowerShell с помощта на многофакторно удостоверяване](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Включване или изключване на търсенето в регистрационен файл за проверка](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
