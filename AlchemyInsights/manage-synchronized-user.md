---
title: Управление на синхронизиран потребител
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823956"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Не можете да зададете основен имейл адрес, да промените потребителските атрибути или да премахнете/изтриете синхронизиран потребител

Ако синхронизирането на справочника е разрешено за вашата среда, някои атрибути на потребител или обект не могат да бъдат променяни с помощта на центъра за администриране на Microsoft 365.

За да управлявате напълно синхронизираните потребители и всички техни атрибути, използвайте своята локална конзола за управление на active directory и групи (adsiedit.msc).  

Като алтернатива можете да промените отделни потребители или атрибути за синхронизирани потребители с помощта на powershell, като например показани в тези често срещани примери:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
