---
title: Използване на PowerShell на Exchange Online за разрешаване на DKIM за конкретен домейн
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743733"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Използване на PowerShell на Exchange Online за разрешаване на DKIM за конкретен домейн

Ако не можете да създадете DKIM DNS Records в центъра за администриране, опитайте да използвате PowerShell на Exchange Online. 

За да създадете DKIM DNS запис с помощта на PowerShell на Exchange Online, изпълнете следните стъпки:

1. Отворете Windows PowerShell като администратор и изпълнете следните команди в описаната последователност:

    на. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Ако имате проблеми със свързването към PowerShell на Exchange Online, вижте [Свързване с PowerShell на Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. След като сте свързани към PowerShell на Exchange Online, изпълнете следната команда:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. След като командата по-горе бъде изпълнена успешно, изпълнете следната команда, за да прекратите сесията на PowerShell на Exchange Online:

    `Remove-PSSession $Session` 



