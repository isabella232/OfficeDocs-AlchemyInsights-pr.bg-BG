---
title: Проблеми с многофакторните
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810473"
---
# <a name="issues-with-azure-mfa"></a>Проблеми с MFA на Azure
Има няколко неща, които трябва да проверите дали потребителите не могат да внедлят влизане с помощта на многофакторно удостоверяване (MFA)

1. Засегнатият потребител може да бъде блокиран в портала на Azure Active Directory. Ако случаят е такъв, опитите за удостоверяване за този конкретен потребител ще бъдат автоматично отказани. [Следвайте стъпките в тази статия, за да ги деблокирате.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ако деблокиране на потребителя не помогне или потребителят не е блокиран, можете да опитате да нулирате MFA за потребителя и те ще преминат през процеса на записване отново. [Следвайте стъпките в тази статия.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ако това е първият път, когато сте разрешили MFA и вашите потребители не могат да влезят в клиенти, които не са браузъри, като например Outlook, Skype и т.н., може би ADAL (библиотека за удостоверяване на Active Directory) не е разрешена във вашия абонамент за O365. В този случай ще трябва да се свържете към Powershell на Exchange Online и да изпълните тази кратка команда:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*