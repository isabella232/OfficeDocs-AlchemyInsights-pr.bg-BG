---
title: Използване Exchange Online PowerShell за разрешаване на DKIM за конкретен домейн
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
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070278"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Използване Exchange Online PowerShell за разрешаване на DKIM за конкретен домейн

Ако не можете да създадете DKIM DNS записите в центъра за администриране, опитайте да използвате Exchange Online PowerShell. 

За да създадете DKIM DNS запис с помощта Exchange Online PowerShell, изпълнете следните стъпки:

1. Отворете Windows PowerShell като администратор и изпълнете следните команди в описаната последователност:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Ако имате проблеми със свързването към Exchange Online PowerShell, [вижте Свързване към Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. След като сте свързани към Exchange Online PowerShell, изпълнете следната команда:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. След като командата по-горе е изпълнена успешно, изпълнете следната команда, за да прекратите Exchange Online сесия на PowerShell:

    `Remove-PSSession $Session` 



