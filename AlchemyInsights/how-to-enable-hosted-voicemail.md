---
title: Как се разрешава хоствана гласова поща
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/09/2020
ms.locfileid: "49676862"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="eedc6-102">Как се разрешава хоствана гласова поща</span><span class="sxs-lookup"><span data-stu-id="eedc6-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="eedc6-103">За да разрешите гласовата поща, **HostedVoicemail** трябва да бъде настроено на $True.</span><span class="sxs-lookup"><span data-stu-id="eedc6-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="eedc6-104">Свойството **HostedVoicemail** на потребителя чрез отдалечен POWERSHELL (RPS).</span><span class="sxs-lookup"><span data-stu-id="eedc6-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="eedc6-105">За повече информация относно свързването с RPS вижте [общ преглед на Microsoft Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) за повече информация относно свързването с RPS.</span><span class="sxs-lookup"><span data-stu-id="eedc6-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="eedc6-106">Администраторът на Teams трябва да бъде влязъл в отдалечен PowerShell за Teams.</span><span class="sxs-lookup"><span data-stu-id="eedc6-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="eedc6-107">От PowerShell подкана администраторът на Teams може да изпълни **Set-csuser user@contoso.com-HostedVoiceMail $True** , където SIP URI е от въпросния потребител.</span><span class="sxs-lookup"><span data-stu-id="eedc6-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="eedc6-108">Промените в правилата могат да са необходими до 24 часа, за да се копират.</span><span class="sxs-lookup"><span data-stu-id="eedc6-108">Changes to policies can take up to 24 hours to replicate.</span></span>