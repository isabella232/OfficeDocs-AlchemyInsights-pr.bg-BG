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
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098591"
---
# <a name="issues-with-azure-mfa"></a>Проблеми с MFA на Azure
Има няколко неща, които трябва да проверите дали потребителите не могат да внедлят влизане с помощта на многофакторно удостоверяване (MFA)

1. Засегнатият потребител може да бъде блокиран в Azure Active Directory портал. Ако случаят е такъв, опитите за удостоверяване за този конкретен потребител ще бъдат автоматично отказани. [Следвайте стъпките в тази статия, за да ги деблокирате.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ако деблокиране на потребителя не помогне или потребителят не е блокиран, можете да опитате да нулирате MFA за потребителя и те ще преминат през процеса на записване отново. [Следвайте стъпките в тази статия.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ако това е първият път, когато сте разрешили MFA и вашите потребители не могат да влезят в клиенти, които не са браузъри, като например Outlook, Skype и т.н., може би ADAL (библиотека за удостоверяване на Active Directory) не е разрешена във вашия абонамент за O365. В този случай ще трябва да се свържете с Exchange Online Powershell и да изпълните тази кратка команда: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*