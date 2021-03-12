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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743770"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="8fec1-102">Задаване на ClientAccessServerEnabled на "истина"</span><span class="sxs-lookup"><span data-stu-id="8fec1-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="8fec1-103">Ако не можете да отворите шифровано имейл съобщение и вместо това видите прикачен файл на **rpmsg** , изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="8fec1-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="8fec1-104">Свързване към PowerShell на Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="8fec1-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="8fec1-105">За да се свържете с PowerShell на Exchange Online, трябва да влезете, като използвате глобален администратор или акаунт за Exchange.</span><span class="sxs-lookup"><span data-stu-id="8fec1-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="8fec1-106">на.</span><span class="sxs-lookup"><span data-stu-id="8fec1-106">a.</span></span> <span data-ttu-id="8fec1-107">Отворете Windows PowerShell и след това изпълнете следната команда: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="8fec1-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="8fec1-108">b.</span><span class="sxs-lookup"><span data-stu-id="8fec1-108">b.</span></span> <span data-ttu-id="8fec1-109">В диалоговия прозорец за **искане на идентификационни данни на Windows PowerShell** въведете своя служебен или учебен акаунт и парола, c.</span><span class="sxs-lookup"><span data-stu-id="8fec1-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="8fec1-110">Щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="8fec1-110">Click **OK**.</span></span> 

2. <span data-ttu-id="8fec1-111">Изпълнете следната команда, за да създадете нова сесия:</span><span class="sxs-lookup"><span data-stu-id="8fec1-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="8fec1-112">на.</span><span class="sxs-lookup"><span data-stu-id="8fec1-112">a.</span></span> <span data-ttu-id="8fec1-113">Изпълнете следната команда:</span><span class="sxs-lookup"><span data-stu-id="8fec1-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="8fec1-114">Командата ' ' изпълнение ' ' `Get-IRMConfiguration` .</span><span class="sxs-lookup"><span data-stu-id="8fec1-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="8fec1-115">Проверете настройката на **ClientAccessServerEnabled** .</span><span class="sxs-lookup"><span data-stu-id="8fec1-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="8fec1-116">на.</span><span class="sxs-lookup"><span data-stu-id="8fec1-116">a.</span></span> <span data-ttu-id="8fec1-117">Ако настройката **ClientAccessServerEnabled** е зададена на **FALSE**, изпълнете следната кратка команда: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="8fec1-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="8fec1-118">Винаги затваряйте вашата сесия на PowerShell със следната команда: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="8fec1-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="8fec1-119">За повече информация вижте [PowerShell на Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="8fec1-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

