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
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777666"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Не можете да задавате първичен имейл адрес, да променяте потребителските атрибути или да премахвате/изтривате синхронизиран потребител

Ако Синхронизирането на справочен указател е разрешено за вашата среда, някои атрибути на потребител или обект не могат да бъдат променяни с помощта на центъра за администриране на Microsoft 365.

За пълно управление на синхронизираните потребители и всички техни атрибути Използвайте локалната Конзола за управление на потребители и групи на Active Directory (Adsiedit. msc).  

Друга възможност е да промените отделни потребители или атрибути за синхронизирани потребители с помощта на PowerShell, както е показано в тези общи примери: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
