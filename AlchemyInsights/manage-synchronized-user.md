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
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Не може да се зададе основен имейл адрес, да се променят потребителски атрибути или премахване/изтриване на синхронизиран потребител

Ако синхронизирането на директории е разрешено за вашата среда, някои потребителски или обект атрибути не могат да бъдат променяни с помощта на центъра за администриране на Microsoft 365.

За да управлявате напълно синхронизираните потребители и всичките им атрибути, използвайте вашите локални потребители на active directory и конзолата за управление на групи (adsiedit.msc).  

Освен това можете да промените отделни потребители или атрибути за синхронизирани потребители с помощта на PowerShell, като например показани в тези общи примери: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
