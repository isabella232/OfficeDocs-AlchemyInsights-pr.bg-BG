---
title: Задаване на ClientAccessServerEnabled на True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994854"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Задаване на ClientAccessServerEnabled на True

Ако не можете да отворите шифровано имейл съобщение и вместо това видите прикачен файл **с rpmsg,** изпълнете следните стъпки:

1. Свързване да Exchange Online PowerShell.

> [!NOTE]
> За да се свържете Exchange Online PowerShell, трябва да влезете с помощта на глобален администратор или Exchange администраторски акаунт.

   a. Отворете Windows PowerShell и след това изпълнете следната команда:`$UserCredential = Get-Credential`
b. В диалоговия **Windows PowerShell искане за идентификационни данни** въведете своя работен или учебен акаунт и парола, c. Щракнете върху **OK**. 

2. Изпълнете следната команда, за да създадете нова сесия:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Изпълнете следната команда:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Изпълнете `Get-IRMConfiguration` командата.

4. Проверете **настройката ClientAccessServerEnabled.** 

    a. Ако **настройката ClientAccessServerEnabled** е **зададена** на False , изпълнете следната кратка команда: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Винаги затваряйте сесията на Powershell със следната команда: `Remove-PSSession $Session`

За повече информация вж. [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

