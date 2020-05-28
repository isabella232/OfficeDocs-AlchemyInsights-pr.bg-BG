---
title: Управление на синхронизирания потребител
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407339"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="57786-102">Не може да се зададе основен имейл адрес, да се променят потребителски атрибути или премахване/изтриване на синхронизиран потребител</span><span class="sxs-lookup"><span data-stu-id="57786-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="57786-103">Ако синхронизирането на директории е разрешено за вашата среда, някои потребителски или обект атрибути не могат да бъдат променяни с помощта на центъра за администриране на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="57786-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="57786-104">За да управлявате напълно синхронизираните потребители и всичките им атрибути, използвайте вашите локални потребители на active directory и конзолата за управление на групи (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="57786-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="57786-105">Освен това можете да промените отделни потребители или атрибути за синхронизирани потребители с помощта на PowerShell, като например показани в тези общи примери:</span><span class="sxs-lookup"><span data-stu-id="57786-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
