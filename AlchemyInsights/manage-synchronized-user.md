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
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="8943f-102">Не можете да задавате първичен имейл адрес, да променяте потребителските атрибути или да премахвате/изтривате синхронизиран потребител</span><span class="sxs-lookup"><span data-stu-id="8943f-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="8943f-103">Ако Синхронизирането на справочен указател е разрешено за вашата среда, някои атрибути на потребител или обект не могат да бъдат променяни с помощта на центъра за администриране на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="8943f-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="8943f-104">За пълно управление на синхронизираните потребители и всички техни атрибути Използвайте локалната Конзола за управление на потребители и групи на Active Directory (Adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="8943f-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="8943f-105">Друга възможност е да промените отделни потребители или атрибути за синхронизирани потребители с помощта на PowerShell, както е показано в тези общи примери:</span><span class="sxs-lookup"><span data-stu-id="8943f-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
