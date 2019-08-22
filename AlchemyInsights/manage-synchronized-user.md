---
title: Управление на синхронизиран потребител
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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541971"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Не може да зададете основния имейл адрес или промяна на потребителски атрибути

Ако Синхронизирането на директории е разрешен за вашата среда, някои потребител или обект атрибути не могат да бъдат променени с помощта на центъра за администрация на Microsoft 365.

За да управлявате напълно синхронизирани потребители и всички техни атрибути, използвайте вашата локалната услуга active directory потребители и групи управление конзола (adsiedit.msc).  

Алтернативно можете да промените отделни потребители или атрибути за синхронизирани потребители, използващи powershell, както е показано в тези общи примери: 
- Комплект-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Комплект-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Тестов потребител" - фамилия "Потребител"-заглавие "Мениджър"-отдел "Човешки ресурси"
- Премествам-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com