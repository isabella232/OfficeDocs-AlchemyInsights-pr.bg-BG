---
title: Задаване на ClientAccessServerEnabled на "истина"
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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523301"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Задаване на ClientAccessServerEnabled на "истина"

Ако не можете да отворите шифровано имейл съобщение и вместо това видите прикачен файл на **rpmsg** , изпълнете следните стъпки:

1. Свързване към PowerShell на Exchange Online.

> [!NOTE]
> За да се свържете с PowerShell на Exchange Online, трябва да влезете, като използвате глобален администратор или акаунт за Exchange.

   на. Отворете Windows PowerShell и след това изпълнете следната команда: `$UserCredential = Get-Credential`
b. В диалоговия прозорец за **искане на идентификационни данни на Windows PowerShell** въведете своя служебен или учебен акаунт и парола, c. Щракнете върху **OK**. 

2. Изпълнете следната команда, за да създадете нова сесия:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    на. Изпълнете следната команда:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Командата ' ' изпълнение ' ' `Get-IRMConfiguration` .

4. Проверете настройката на **ClientAccessServerEnabled** . 

    на. Ако настройката **ClientAccessServerEnabled** е зададена на **FALSE**, изпълнете следната кратка команда: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Винаги затваряйте вашата сесия на PowerShell със следната команда: `Remove-PSSession $Session`

За повече информация вижте [PowerShell на Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

