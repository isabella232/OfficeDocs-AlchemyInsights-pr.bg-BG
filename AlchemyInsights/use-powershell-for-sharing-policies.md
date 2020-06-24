---
title: Използвайте PowerShell за споделяне на правила и организация връзки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862029"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="10652-102">Използвайте PowerShell за споделяне на правила и организация връзки</span><span class="sxs-lookup"><span data-stu-id="10652-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="10652-103">За организационните взаимоотношения прегледайте подробния синтаксис и информация за параметрите за: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [Нова организацияRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) and [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="10652-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="10652-104">За да създадете правила за споделяне, използвайте [new sharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="10652-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="10652-105">За да [приложите правила за споделяне на пощенска кутия или потребител,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) трябва да използвате комбинация от [Set-Пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) и [Get-пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) с новосъздадените правила.</span><span class="sxs-lookup"><span data-stu-id="10652-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="10652-106">За да [промените, деактивирате или премахнете правила за споделяне,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) трябва да използвате [Set-SharingПолийс](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) и [премахване на споделянеполи.](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)</span><span class="sxs-lookup"><span data-stu-id="10652-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="10652-107">**За пълно разбиране на тази тема, моля прочетете:**</span><span class="sxs-lookup"><span data-stu-id="10652-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="10652-108">Споделяне в Онлайн Exchange</span><span class="sxs-lookup"><span data-stu-id="10652-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)