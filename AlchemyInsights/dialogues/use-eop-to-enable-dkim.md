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
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523236"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="695b2-102">Използване на PowerShell на Exchange Online за разрешаване на DKIM за конкретен домейн</span><span class="sxs-lookup"><span data-stu-id="695b2-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="695b2-103">Ако не можете да създадете DKIM DNS Records в центъра за администриране, опитайте да използвате PowerShell на Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="695b2-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="695b2-104">За да създадете DKIM DNS запис с помощта на PowerShell на Exchange Online, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="695b2-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="695b2-105">Отворете Windows PowerShell като администратор и изпълнете следните команди в описаната последователност:</span><span class="sxs-lookup"><span data-stu-id="695b2-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="695b2-106">на.</span><span class="sxs-lookup"><span data-stu-id="695b2-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="695b2-107">b.</span><span class="sxs-lookup"><span data-stu-id="695b2-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="695b2-108">c.</span><span class="sxs-lookup"><span data-stu-id="695b2-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="695b2-109">Ако имате проблеми със свързването към PowerShell на Exchange Online, вижте [Свързване с PowerShell на Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="695b2-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="695b2-110">След като сте свързани към PowerShell на Exchange Online, изпълнете следната команда:</span><span class="sxs-lookup"><span data-stu-id="695b2-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="695b2-111">След като командата по-горе бъде изпълнена успешно, изпълнете следната команда, за да прекратите сесията на PowerShell на Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="695b2-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



