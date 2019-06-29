---
title: 761 свързване към Exchange Online PowerShell когато МВНР е разрешено
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 4/26/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "761"
- "3500011"
ms.assetid: 9b0b89e3-d1d7-4e4d-93de-bb4cd00904d8
ms.openlocfilehash: 16137ae4f0324ca508676a7ba351e5f97e7125a1
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364506"
---
# <a name="connect-to-exchange-online-powershell-when-mfa-is-enabled"></a><span data-ttu-id="ff98c-102">Свързване към Exchange Online PowerShell когато МВНР е разрешено</span><span class="sxs-lookup"><span data-stu-id="ff98c-102">Connect to Exchange Online PowerShell when MFA is enabled</span></span>

<span data-ttu-id="ff98c-103">Ако вашият акаунт е многофакторен (МВНР) разрешено удостоверяване, трябва да следвате тези инструкции да се свърже с Exchange Online PowerShell: [Свързване към Exchange Online PowerShell използва удостоверяване](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="ff98c-103">If your account has multi-factor authentication (MFA) enabled, you need to follow these instructions to connect to Exchange Online PowerShell: [Connect to Exchange Online PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell).</span></span>

<span data-ttu-id="ff98c-104">**Забележка**: дори и ако сте се свързвали към Exchange Online PowerShell в миналото използвате [редовна връзка инструкции](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell), трябва да използвате инструкции за свързване на СМТТ след МВНР е разрешен за вашия акаунт.</span><span class="sxs-lookup"><span data-stu-id="ff98c-104">**Note**: Even if you've connected to Exchange Online PowerShell in the past using [the regular connection instructions](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell), you need to use the MFA connection instructions after MFA has been enabled for your account.</span></span>
