---
title: Използване на PowerShell за споделяне на правила и отношения в организацията
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709455"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Използване на PowerShell за споделяне на правила и отношения в организацията


За отношенията в организацията прегледайте подробната информация за синтаксиса и параметрите за: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) И [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

За създаване на правила за споделяне използвайте [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). За [прилагане на правила за споделяне към пощенска кутия или потребител](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) трябва да използвате комбинация от [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) и [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) с новосъздадените правила. За [промяна, забраняване или премахване на правила за споделяне](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) трябва да използвате [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) и [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**За пълно разбиране на тази тема прочетете:**

[Споделяне в Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)