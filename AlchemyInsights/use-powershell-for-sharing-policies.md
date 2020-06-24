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
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Използвайте PowerShell за споделяне на правила и организация връзки


За организационните взаимоотношения прегледайте подробния синтаксис и информация за параметрите за: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [Нова организацияRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) and [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

За да създадете правила за споделяне, използвайте [new sharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). За да [приложите правила за споделяне на пощенска кутия или потребител,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) трябва да използвате комбинация от [Set-Пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) и [Get-пощенска кутия](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) с новосъздадените правила. За да [промените, деактивирате или премахнете правила за споделяне,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) трябва да използвате [Set-SharingПолийс](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) и [премахване на споделянеполи.](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)

**За пълно разбиране на тази тема, моля прочетете:**

[Споделяне в Онлайн Exchange](https://docs.microsoft.com/exchange/sharing/sharing)