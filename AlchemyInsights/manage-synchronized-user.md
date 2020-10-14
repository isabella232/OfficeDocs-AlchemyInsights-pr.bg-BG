---
title: Управление на синхронизиран потребител
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451389"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Не можете да задавате първичен имейл адрес, да променяте потребителските атрибути или да премахвате/изтривате синхронизиран потребител

Ако Синхронизирането на справочен указател е разрешено за вашата среда, някои атрибути на потребител или обект не могат да бъдат променяни с помощта на центъра за администриране на Microsoft 365.

За пълно управление на синхронизираните потребители и всички техни атрибути Използвайте локалната Конзола за управление на потребители и групи на Active Directory (Adsiedit. msc).  

Друга възможност е да промените отделни потребители или атрибути за синхронизирани потребители с помощта на PowerShell, както е показано в тези общи примери:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
